# Comparing `tmp/plotpy-2.3.1.tar.gz` & `tmp/plotpy-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotpy-2.3.1.tar", last modified: Mon May  6 16:41:15 2024, max compression
+gzip compressed data, was "plotpy-2.3.2.tar", last modified: Tue May  7 08:01:16 2024, max compression
```

## Comparing `plotpy-2.3.1.tar` & `plotpy-2.3.2.tar`

### file list

```diff
@@ -1,577 +1,577 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.583426 plotpy-2.3.1/
--rw-rw-rw-   0        0        0    15956 2024-05-06 16:40:26.000000 plotpy-2.3.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1563 2023-11-23 17:46:00.000000 plotpy-2.3.1/LICENSE
--rw-rw-rw-   0        0        0      143 2024-04-10 16:39:34.000000 plotpy-2.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     8668 2024-05-06 16:41:15.583426 plotpy-2.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.583426 plotpy-2.3.1/PlotPy.egg-info/
--rw-rw-rw-   0        0        0     8668 2024-05-06 16:41:10.000000 plotpy-2.3.1/PlotPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    16880 2024-05-06 16:41:10.000000 plotpy-2.3.1/PlotPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 16:41:10.000000 plotpy-2.3.1/PlotPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-06 16:41:10.000000 plotpy-2.3.1/PlotPy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      224 2024-05-06 16:41:10.000000 plotpy-2.3.1/PlotPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-06 16:41:10.000000 plotpy-2.3.1/PlotPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4379 2023-11-23 17:46:00.000000 plotpy-2.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.114675 plotpy-2.3.1/colormaps/
--rw-rw-rw-   0        0        0      170 2024-02-08 10:33:36.000000 plotpy-2.3.1/colormaps/README.md
--rw-rw-rw-   0        0        0   421433 2024-02-08 10:33:36.000000 plotpy-2.3.1/colormaps/_cm.py
--rw-rw-rw-   0        0        0     3083 2024-02-09 17:39:23.000000 plotpy-2.3.1/colormaps/colormap.py
--rw-rw-rw-   0        0        0     9391 2024-03-04 13:28:35.000000 plotpy-2.3.1/colormaps/matplotlib_cmaps.py
--rw-rw-rw-   0        0        0      189 2024-04-10 16:39:34.000000 plotpy-2.3.1/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.161549 plotpy-2.3.1/doc/
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.177175 plotpy-2.3.1/doc/_static/
--rw-rw-rw-   0        0        0   110568 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/_static/favicon.ico
--rw-rw-rw-   0        0        0       79 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/changelog.rst
--rw-rw-rw-   0        0        0     2273 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/conf.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.270926 plotpy-2.3.1/doc/dev/
--rw-rw-rw-   0        0        0     1003 2024-04-10 16:39:34.000000 plotpy-2.3.1/doc/dev/build.rst
--rw-rw-rw-   0        0        0     4374 2024-04-10 16:39:34.000000 plotpy-2.3.1/doc/dev/contribute.rst
--rw-rw-rw-   0        0        0     3108 2024-02-09 17:39:23.000000 plotpy-2.3.1/doc/dev/guiqwt_to_plotpy.csv
--rw-rw-rw-   0        0        0     9868 2024-02-16 08:53:28.000000 plotpy-2.3.1/doc/dev/guiqwt_to_plotpy.rst
--rw-rw-rw-   0        0        0      158 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/dev/index.rst
--rw-rw-rw-   0        0        0     5039 2024-04-10 16:39:34.000000 plotpy-2.3.1/doc/dev/platforms.rst
--rw-rw-rw-   0        0        0      389 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/dev/v1_to_guidata_v3.csv
--rw-rw-rw-   0        0        0     2489 2024-02-09 17:39:23.000000 plotpy-2.3.1/doc/dev/v1_to_v2.csv
--rw-rw-rw-   0        0        0     3374 2024-02-16 08:53:28.000000 plotpy-2.3.1/doc/dev/v1_to_v2.rst
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.333428 plotpy-2.3.1/doc/features/
--rw-rw-rw-   0        0        0       41 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/colormapmanager.rst
--rw-rw-rw-   0        0        0       31 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/events.rst
--rw-rw-rw-   0        0        0       36 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/fit.rst
--rw-rw-rw-   0        0        0       43 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/fliprotate.rst
--rw-rw-rw-   0        0        0       42 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/imagefile.rst
--rw-rw-rw-   0        0        0      327 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/index.rst
--rw-rw-rw-   0        0        0       25 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/io.rst
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.364677 plotpy-2.3.1/doc/features/items/
--rw-rw-rw-   0        0        0      784 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/items/builder.rst
--rw-rw-rw-   0        0        0     4830 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/items/examples.rst
--rw-rw-rw-   0        0        0      149 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/items/index.rst
--rw-rw-rw-   0        0        0     2311 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/items/overview.rst
--rw-rw-rw-   0        0        0     3319 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/items/reference.rst
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.380298 plotpy-2.3.1/doc/features/mathutils/
--rw-rw-rw-   0        0        0       41 2024-02-09 17:39:23.000000 plotpy-2.3.1/doc/features/mathutils/colormaps.rst
--rw-rw-rw-   0        0        0       41 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/mathutils/geometry.rst
--rw-rw-rw-   0        0        0      119 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/mathutils/index.rst
--rw-rw-rw-   0        0        0       39 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/mathutils/scaler.rst
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.395923 plotpy-2.3.1/doc/features/panels/
--rw-rw-rw-   0        0        0      127 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/panels/index.rst
--rw-rw-rw-   0        0        0      891 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/panels/overview.rst
--rw-rw-rw-   0        0        0      212 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/panels/reference.rst
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.411548 plotpy-2.3.1/doc/features/plot/
--rw-rw-rw-   0        0        0     1012 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/plot/examples.rst
--rw-rw-rw-   0        0        0     1560 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/plot/index.rst
--rw-rw-rw-   0        0        0     1150 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/plot/overview.rst
--rw-rw-rw-   0        0        0      625 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/plot/reference.rst
--rw-rw-rw-   0        0        0       51 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/pyplot.rst
--rw-rw-rw-   0        0        0       45 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/resizedialog.rst
--rw-rw-rw-   0        0        0       43 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/rotatecrop.rst
--rw-rw-rw-   0        0        0       45 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/selectdialog.rst
--rw-rw-rw-   0        0        0     1754 2024-03-04 12:33:14.000000 plotpy-2.3.1/doc/features/signals.rst
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.442798 plotpy-2.3.1/doc/features/styles/
--rw-rw-rw-   0        0        0      157 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/styles/index.rst
--rw-rw-rw-   0        0        0      540 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/styles/overview.rst
--rw-rw-rw-   0        0        0     1921 2024-02-08 10:33:36.000000 plotpy-2.3.1/doc/features/styles/reference.rst
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.474049 plotpy-2.3.1/doc/features/tools/
--rw-rw-rw-   0        0        0      289 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/tools/examples.rst
--rw-rw-rw-   0        0        0      137 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/features/tools/index.rst
--rw-rw-rw-   0        0        0     2747 2024-03-11 08:11:54.000000 plotpy-2.3.1/doc/features/tools/overview.rst
--rw-rw-rw-   0        0        0     3717 2024-03-11 08:11:54.000000 plotpy-2.3.1/doc/features/tools/reference.rst
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.599052 plotpy-2.3.1/doc/images/
--rw-rw-rw-   0        0        0    42675 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/my_plot_manager.png
--rw-rw-rw-   0        0        0    31164 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/my_plot_manager.svg
--rw-rw-rw-   0        0        0   240381 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/panorama.png
--rw-rw-rw-   0        0        0  1914412 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/panorama.svg
--rw-rw-rw-   0        0        0    55886 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/plot_widgets.png
--rw-rw-rw-   0        0        0    30549 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/plot_widgets.svg
--rw-rw-rw-   0        0        0     9809 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/plotpy-banner.png
--rw-rw-rw-   0        0        0     7460 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/plotpy-vertical.png
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.817797 plotpy-2.3.1/doc/images/screenshots/
--rw-rw-rw-   0        0        0    64597 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/__init__.png
--rw-rw-rw-   0        0        0    37530 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/computations.png
--rw-rw-rw-   0        0        0   179050 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/contrast.png
--rw-rw-rw-   0        0        0   210107 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/cross_section.png
--rw-rw-rw-   0        0        0   210494 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/cross_section2.png
--rw-rw-rw-   0        0        0    81254 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/dotarraydemo.png
--rw-rw-rw-   0        0        0    41879 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/filtertest1.png
--rw-rw-rw-   0        0        0    49232 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/filtertest2.png
--rw-rw-rw-   0        0        0    44646 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/fit.png
--rw-rw-rw-   0        0        0    32653 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/get_point.png
--rw-rw-rw-   0        0        0    77053 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/hist2d.png
--rw-rw-rw-   0        0        0   269545 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/image_plot_tools.png
--rw-rw-rw-   0        0        0   230644 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/imagefilter.png
--rw-rw-rw-   0        0        0   163887 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/imagesuperp.png
--rw-rw-rw-   0        0        0   143730 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/imagexy.png
--rw-rw-rw-   0        0        0   168112 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/manager.png
--rw-rw-rw-   0        0        0   231418 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/mandelbrot.png
--rw-rw-rw-   0        0        0   172858 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/pcolor.png
--rw-rw-rw-   0        0        0    76448 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/plot.png
--rw-rw-rw-   0        0        0   173690 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/simple_dialog.png
--rw-rw-rw-   0        0        0    59433 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/simple_window.png
--rw-rw-rw-   0        0        0   456556 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/images/screenshots/transform.png
--rw-rw-rw-   0        0        0     1651 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/index.rst
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:11.911550 plotpy-2.3.1/doc/intro/
--rw-rw-rw-   0        0        0     2862 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/intro/examples.rst
--rw-rw-rw-   0        0        0      164 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/intro/index.rst
--rw-rw-rw-   0        0        0      675 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/intro/installation.rst
--rw-rw-rw-   0        0        0   107599 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/intro/licenses.rst
--rw-rw-rw-   0        0        0     2299 2024-04-10 16:39:34.000000 plotpy-2.3.1/doc/intro/motivation.rst
--rw-rw-rw-   0        0        0     4815 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/intro/overview.rst
--rw-rw-rw-   0        0        0     2429 2024-03-11 08:11:54.000000 plotpy-2.3.1/doc/requirements.rst
--rw-rw-rw-   0        0        0      721 2023-11-23 17:46:00.000000 plotpy-2.3.1/doc/update_requirements.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.005302 plotpy-2.3.1/plotpy/
--rw-rw-rw-   0        0        0     1053 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.114675 plotpy-2.3.1/plotpy/builder/
--rw-rw-rw-   0        0        0     1114 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/builder/__init__.py
--rw-rw-rw-   0        0        0    13033 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/builder/annotation.py
--rw-rw-rw-   0        0        0    31776 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/builder/curvemarker.py
--rw-rw-rw-   0        0        0    33708 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/builder/image.py
--rw-rw-rw-   0        0        0    10062 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/builder/label.py
--rw-rw-rw-   0        0        0    17119 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/builder/plot.py
--rw-rw-rw-   0        0        0     5886 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/builder/shape.py
--rw-rw-rw-   0        0        0    34344 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/config.py
--rw-rw-rw-   0        0        0     4756 2024-02-16 08:53:28.000000 plotpy-2.3.1/plotpy/constants.py
--rw-rw-rw-   0        0        0     2385 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/coords.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.130299 plotpy-2.3.1/plotpy/data/
--rw-rw-rw-   0        0        0   328300 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/colormaps_default.json
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.458424 plotpy-2.3.1/plotpy/data/icons/
--rw-rw-rw-   0        0        0      595 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/apply.png
--rw-rw-rw-   0        0        0      897 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/arredit.png
--rw-rw-rw-   0        0        0      637 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/arrow_down.png
--rw-rw-rw-   0        0        0      638 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/arrow_up.png
--rw-rw-rw-   0        0        0      868 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/autorefresh.png
--rw-rw-rw-   0        0        0     1012 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/autoscale.png
--rw-rw-rw-   0        0        0      513 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/axes.png
--rw-rw-rw-   0        0        0      474 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/busy.png
--rw-rw-rw-   0        0        0      478 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/cell_edit.png
--rw-rw-rw-   0        0        0      346 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/center.png
--rw-rw-rw-   0        0        0      495 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/cmap_edit.png
--rw-rw-rw-   0        0        0      316 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/contrast.png
--rw-rw-rw-   0        0        0      620 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/copy.png
--rw-rw-rw-   0        0        0      979 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/copytoclipboard.png
--rw-rw-rw-   0        0        0      705 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csapplylut.png
--rw-rw-rw-   0        0        0      178 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csautoscale.png
--rw-rw-rw-   0        0        0      346 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csection.png
--rw-rw-rw-   0        0        0      310 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csection_a.png
--rw-rw-rw-   0        0        0      375 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csection_line.png
--rw-rw-rw-   0        0        0      711 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csection_oblique.png
--rw-rw-rw-   0        0        0      160 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/csperimage.png
--rw-rw-rw-   0        0        0      758 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curve_downsample.png
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.505301 plotpy-2.3.1/plotpy/data/icons/curvestyles/
--rw-rw-rw-   0        0        0      121 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curvestyles/dots.png
--rw-rw-rw-   0        0        0      164 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curvestyles/lines.png
--rw-rw-rw-   0        0        0      136 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curvestyles/steps.png
--rw-rw-rw-   0        0        0      187 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curvestyles/sticks.png
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.505301 plotpy-2.3.1/plotpy/data/icons/curvetypes/
--rw-rw-rw-   0        0        0      322 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curvetypes/xfy.png
--rw-rw-rw-   0        0        0      322 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/curvetypes/yfx.png
--rw-rw-rw-   0        0        0      496 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/delete.png
--rw-rw-rw-   0        0        0      718 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/edit.png
--rw-rw-rw-   0        0        0      793 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/edit_point_selection.png
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.614680 plotpy-2.3.1/plotpy/data/icons/editors/
--rw-rw-rw-   0        0        0      718 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/edit.png
--rw-rw-rw-   0        0        0      790 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/edit_add.png
--rw-rw-rw-   0        0        0      837 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/editcopy.png
--rw-rw-rw-   0        0        0     1242 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/editdelete.png
--rw-rw-rw-   0        0        0     1084 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/editpaste.png
--rw-rw-rw-   0        0        0     2065 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/fileimport.png
--rw-rw-rw-   0        0        0      970 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/filesave.png
--rw-rw-rw-   0        0        0      516 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/imshow.png
--rw-rw-rw-   0        0        0      314 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/insert.png
--rw-rw-rw-   0        0        0      304 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/plot.png
--rw-rw-rw-   0        0        0      478 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/editors/rename.png
--rw-rw-rw-   0        0        0      183 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/eliminate_outliers.png
--rw-rw-rw-   0        0        0      671 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/eraser.png
--rw-rw-rw-   0        0        0      974 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/exit.png
--rw-rw-rw-   0        0        0      191 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/expander_down.png
--rw-rw-rw-   0        0        0      184 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/expander_right.png
--rw-rw-rw-   0        0        0      861 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/export.png
--rw-rw-rw-   0        0        0      304 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/file.png
--rw-rw-rw-   0        0        0     1213 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/fileclose.png
--rw-rw-rw-   0        0        0     1383 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/fileimport.png
--rw-rw-rw-   0        0        0      271 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filenew.png
--rw-rw-rw-   0        0        0     1349 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/fileopen.png
--rw-rw-rw-   0        0        0      970 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filesave.png
--rw-rw-rw-   0        0        0     1264 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filesaveas.png
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.724050 plotpy-2.3.1/plotpy/data/icons/filetypes/
--rw-rw-rw-   0        0        0     1389 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/doc.png
--rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/gif.png
--rw-rw-rw-   0        0        0     1658 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/html.png
--rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/jpg.png
--rw-rw-rw-   0        0        0     1352 2024-03-04 13:28:35.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/pdf.png
--rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/png.png
--rw-rw-rw-   0        0        0     1226 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/pps.png
--rw-rw-rw-   0        0        0     1217 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/ps.png
--rw-rw-rw-   0        0        0     1385 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/tar.png
--rw-rw-rw-   0        0        0     1385 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/tgz.png
--rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/tif.png
--rw-rw-rw-   0        0        0     1609 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/txt.png
--rw-rw-rw-   0        0        0     1026 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/xls.png
--rw-rw-rw-   0        0        0     1385 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/filetypes/zip.png
--rw-rw-rw-   0        0        0      244 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/font.png
--rw-rw-rw-   0        0        0      185 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/full_range.png
--rw-rw-rw-   0        0        0      922 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/funct.png
--rw-rw-rw-   0        0        0      151 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/hcursor.png
--rw-rw-rw-   0        0        0      433 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/hflip.png
--rw-rw-rw-   0        0        0      793 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/imagestats.png
--rw-rw-rw-   0        0        0      437 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/item_list.png
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.770923 plotpy-2.3.1/plotpy/data/icons/items/
--rw-rw-rw-   0        0        0      687 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/annotation.png
--rw-rw-rw-   0        0        0      305 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/curve.png
--rw-rw-rw-   0        0        0      172 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/errorbar.png
--rw-rw-rw-   0        0        0      120 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/grid.png
--rw-rw-rw-   0        0        0      140 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/histogram.png
--rw-rw-rw-   0        0        0      857 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/histogram2d.png
--rw-rw-rw-   0        0        0      852 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/image.png
--rw-rw-rw-   0        0        0      531 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/label.png
--rw-rw-rw-   0        0        0      317 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/legend.png
--rw-rw-rw-   0        0        0      448 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/items/polygonmap.png
--rw-rw-rw-   0        0        0      673 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/magnifier.png
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.849049 plotpy-2.3.1/plotpy/data/icons/markers/
--rw-rw-rw-   0        0        0      123 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/cross.png
--rw-rw-rw-   0        0        0      194 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/diamond.png
--rw-rw-rw-   0        0        0      241 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/ellipse.png
--rw-rw-rw-   0        0        0      260 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/hexagon.png
--rw-rw-rw-   0        0        0      105 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/point.png
--rw-rw-rw-   0        0        0      137 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/square.png
--rw-rw-rw-   0        0        0      160 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/star.png
--rw-rw-rw-   0        0        0      223 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/triangle_d.png
--rw-rw-rw-   0        0        0      220 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/triangle_l.png
--rw-rw-rw-   0        0        0      212 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/triangle_r.png
--rw-rw-rw-   0        0        0      224 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/triangle_u.png
--rw-rw-rw-   0        0        0      145 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markers/xcross.png
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.849049 plotpy-2.3.1/plotpy/data/icons/markerstyles/
--rw-rw-rw-   0        0        0       96 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markerstyles/cross_marker.png
--rw-rw-rw-   0        0        0       82 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markerstyles/horiz_marker.png
--rw-rw-rw-   0        0        0       84 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/markerstyles/vert_marker.png
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.864674 plotpy-2.3.1/plotpy/data/icons/mask/
--rw-rw-rw-   0        0        0      368 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/mask/mask_circle.png
--rw-rw-rw-   0        0        0      374 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/mask/mask_circle_outside.png
--rw-rw-rw-   0        0        0      199 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/mask/mask_rectangle.png
--rw-rw-rw-   0        0        0      200 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/mask/mask_rectangle_outside.png
--rw-rw-rw-   0        0        0      164 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/mask/mask_tool.png
--rw-rw-rw-   0        0        0      130 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/max.png
--rw-rw-rw-   0        0        0      125 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/min.png
--rw-rw-rw-   0        0        0      132 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/move.png
--rw-rw-rw-   0        0        0      729 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/multipoint_selection.png
--rw-rw-rw-   0        0        0       83 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/none.png
--rw-rw-rw-   0        0        0      284 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/not_found.png
--rw-rw-rw-   0        0        0      397 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/on_curve.png
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.895922 plotpy-2.3.1/plotpy/data/icons/patterns/
--rw-rw-rw-   0        0        0      104 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/bdiagpattern.png
--rw-rw-rw-   0        0        0       90 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/crosspattern.png
--rw-rw-rw-   0        0        0       76 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense1pattern.png
--rw-rw-rw-   0        0        0       78 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense2pattern.png
--rw-rw-rw-   0        0        0       83 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense3pattern.png
--rw-rw-rw-   0        0        0       73 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense4pattern.png
--rw-rw-rw-   0        0        0       88 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense5pattern.png
--rw-rw-rw-   0        0        0       87 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense6pattern.png
--rw-rw-rw-   0        0        0       84 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/dense7pattern.png
--rw-rw-rw-   0        0        0      114 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/diagcrosspattern.png
--rw-rw-rw-   0        0        0      112 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/fdiagpattern.png
--rw-rw-rw-   0        0        0       82 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/horpattern.png
--rw-rw-rw-   0        0        0       74 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/nobrush.png
--rw-rw-rw-   0        0        0       69 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/solidpattern.png
--rw-rw-rw-   0        0        0       83 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/patterns/verpattern.png
--rw-rw-rw-   0        0        0    17636 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/plotpy-banner.svg
--rw-rw-rw-   0        0        0    17614 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/plotpy-vertical.svg
--rw-rw-rw-   0        0        0    16339 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/plotpy.svg
--rw-rw-rw-   0        0        0      216 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/point_selection.png
--rw-rw-rw-   0        0        0      723 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/print.png
--rw-rw-rw-   0        0        0      697 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/python.png
--rw-rw-rw-   0        0        0      677 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/quickview.png
--rw-rw-rw-   0        0        0      823 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/rectangular_select.png
--rw-rw-rw-   0        0        0      740 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/refresh.png
--rw-rw-rw-   0        0        0     1428 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/save_all.png
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:12.911548 plotpy-2.3.1/plotpy/data/icons/scales/
--rw-rw-rw-   0        0        0      203 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/scales/lin_lin.png
--rw-rw-rw-   0        0        0      208 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/scales/lin_log.png
--rw-rw-rw-   0        0        0      219 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/scales/log_lin.png
--rw-rw-rw-   0        0        0      222 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/scales/log_log.png
--rw-rw-rw-   0        0        0      518 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/selection.png
--rw-rw-rw-   0        0        0      851 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/settings.png
--rw-rw-rw-   0        0        0      135 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shape.png
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.005297 plotpy-2.3.1/plotpy/data/icons/shapes/
--rw-rw-rw-   0        0        0      530 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/circle.png
--rw-rw-rw-   0        0        0      622 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/contour.png
--rw-rw-rw-   0        0        0      547 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/ellipse_shape.png
--rw-rw-rw-   0        0        0      305 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/freeform.png
--rw-rw-rw-   0        0        0      321 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/gtaxes.png
--rw-rw-rw-   0        0        0      179 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/marker.png
--rw-rw-rw-   0        0        0      650 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/oblique_rectangle.png
--rw-rw-rw-   0        0        0      118 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/point_shape.png
--rw-rw-rw-   0        0        0      232 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/polyline.png
--rw-rw-rw-   0        0        0      179 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/rectangle.png
--rw-rw-rw-   0        0        0      220 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/shapes/segment.png
--rw-rw-rw-   0        0        0     1150 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/snapshot.png
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.036556 plotpy-2.3.1/plotpy/data/icons/styles/
--rw-rw-rw-   0        0        0       85 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/styles/dash.png
--rw-rw-rw-   0        0        0       90 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/styles/dashdot.png
--rw-rw-rw-   0        0        0       84 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/styles/dashdotdot.png
--rw-rw-rw-   0        0        0       80 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/styles/dot.png
--rw-rw-rw-   0        0        0       80 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/styles/solid.png
--rw-rw-rw-   0        0        0      236 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/trash.png
--rw-rw-rw-   0        0        0      932 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/trimage_lock.png
--rw-rw-rw-   0        0        0      958 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/trimage_unlock.png
--rw-rw-rw-   0        0        0      159 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/vcursor.png
--rw-rw-rw-   0        0        0      432 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/vflip.png
--rw-rw-rw-   0        0        0      127 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/xcursor.png
--rw-rw-rw-   0        0        0      128 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/xmax.png
--rw-rw-rw-   0        0        0      127 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/xmin.png
--rw-rw-rw-   0        0        0      170 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/data/icons/xrange.png
--rw-rw-rw-   0        0        0    46755 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/events.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.052174 plotpy-2.3.1/plotpy/external/
--rw-rw-rw-   0        0        0      399 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/external/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.130302 plotpy-2.3.1/plotpy/external/sliders/
--rw-rw-rw-   0        0        0     2108 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/external/sliders/__init__.py
--rw-rw-rw-   0        0        0    14101 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/external/sliders/_generic_range_slider.py
--rw-rw-rw-   0        0        0    20447 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/external/sliders/_generic_slider.py
--rw-rw-rw-   0        0        0    23960 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/external/sliders/_labeled.py
--rw-rw-rw-   0        0        0      758 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/external/sliders/_misc.py
--rw-rw-rw-   0        0        0     9829 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/external/sliders/_range_style.py
--rw-rw-rw-   0        0        0     1126 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/external/sliders/_sliders.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.192801 plotpy-2.3.1/plotpy/interfaces/
--rw-rw-rw-   0        0        0      517 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/interfaces/__init__.py
--rw-rw-rw-   0        0        0    14685 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/interfaces/items.py
--rw-rw-rw-   0        0        0      461 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/interfaces/panel.py
--rw-rw-rw-   0        0        0     1049 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/interfaces/plotmanager.py
--rw-rw-rw-   0        0        0    24077 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/io.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.302177 plotpy-2.3.1/plotpy/items/
--rw-rw-rw-   0        0        0     1517 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/items/__init__.py
--rw-rw-rw-   0        0        0    30198 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/annotation.py
--rw-rw-rw-   0        0        0     6355 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/items/contour.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.364675 plotpy-2.3.1/plotpy/items/curve/
--rw-rw-rw-   0        0        0      176 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/items/curve/__init__.py
--rw-rw-rw-   0        0        0    18860 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/curve/base.py
--rw-rw-rw-   0        0        0    12987 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/curve/errorbar.py
--rw-rw-rw-   0        0        0     7632 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/grid.py
--rw-rw-rw-   0        0        0     7118 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/histogram.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.427172 plotpy-2.3.1/plotpy/items/image/
--rw-rw-rw-   0        0        0      608 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/items/image/__init__.py
--rw-rw-rw-   0        0        0    44532 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/image/base.py
--rw-rw-rw-   0        0        0    11447 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/image/filter.py
--rw-rw-rw-   0        0        0    28332 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/image/image_items.py
--rw-rw-rw-   0        0        0    24911 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/image/masked.py
--rw-rw-rw-   0        0        0    25205 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/image/misc.py
--rw-rw-rw-   0        0        0    23529 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/image/transform.py
--rw-rw-rw-   0        0        0    32816 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/items/label.py
--rw-rw-rw-   0        0        0    13551 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/polygonmap.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.567800 plotpy-2.3.1/plotpy/items/shape/
--rw-rw-rw-   0        0        0      457 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/items/shape/__init__.py
--rw-rw-rw-   0        0        0     9972 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/axis.py
--rw-rw-rw-   0        0        0     8592 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/base.py
--rw-rw-rw-   0        0        0    11893 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/ellipse.py
--rw-rw-rw-   0        0        0    16554 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/marker.py
--rw-rw-rw-   0        0        0     2611 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/point.py
--rw-rw-rw-   0        0        0    14718 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/polygon.py
--rw-rw-rw-   0        0        0     9735 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/items/shape/range.py
--rw-rw-rw-   0        0        0    11459 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/rectangle.py
--rw-rw-rw-   0        0        0     4581 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/items/shape/segment.py
--rw-rw-rw-   0        0        0     4619 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/items/shape/svg.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:10.958428 plotpy-2.3.1/plotpy/locale/
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:10.958428 plotpy-2.3.1/plotpy/locale/fr/
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.599056 plotpy-2.3.1/plotpy/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    32854 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/locale/fr/LC_MESSAGES/plotpy.mo
--rw-rw-rw-   0        0        0     1918 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/lutrange.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.645928 plotpy-2.3.1/plotpy/mathutils/
--rw-rw-rw-   0        0        0       25 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/mathutils/__init__.py
--rw-rw-rw-   0        0        0     1739 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/mathutils/arrayfuncs.py
--rw-rw-rw-   0        0        0    10325 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/mathutils/colormap.py
--rw-rw-rw-   0        0        0     6803 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/mathutils/geometry.py
--rw-rw-rw-   0        0        0     1892 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/mathutils/scaler.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.724050 plotpy-2.3.1/plotpy/panels/
--rw-rw-rw-   0        0        0      270 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/panels/__init__.py
--rw-rw-rw-   0        0        0     2345 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/panels/base.py
--rw-rw-rw-   0        0        0    19745 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/panels/contrastadjustment.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.786551 plotpy-2.3.1/plotpy/panels/csection/
--rw-rw-rw-   0        0        0      480 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/panels/csection/__init__.py
--rw-rw-rw-   0        0        0    17094 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/panels/csection/csitem.py
--rw-rw-rw-   0        0        0    16887 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/panels/csection/csplot.py
--rw-rw-rw-   0        0        0    12868 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/panels/csection/cswidget.py
--rw-rw-rw-   0        0        0     9425 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/panels/itemlist.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:13.864676 plotpy-2.3.1/plotpy/plot/
--rw-rw-rw-   0        0        0      325 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/plot/__init__.py
--rw-rw-rw-   0        0        0    85147 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/plot/base.py
--rw-rw-rw-   0        0        0    22002 2024-02-09 17:39:23.000000 plotpy-2.3.1/plotpy/plot/interactive.py
--rw-rw-rw-   0        0        0    25295 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/plot/manager.py
--rw-rw-rw-   0        0        0    34516 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/plot/plotwidget.py
--rw-rw-rw-   0        0        0     2762 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/pyplot.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.005300 plotpy-2.3.1/plotpy/styles/
--rw-rw-rw-   0        0        0     1738 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/styles/__init__.py
--rw-rw-rw-   0        0        0     4155 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/styles/axes.py
--rw-rw-rw-   0        0        0    19338 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/styles/base.py
--rw-rw-rw-   0        0        0     3172 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/styles/curve.py
--rw-rw-rw-   0        0        0     1552 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/styles/errorbar.py
--rw-rw-rw-   0        0        0     3896 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/styles/histogram.py
--rw-rw-rw-   0        0        0    18053 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/styles/image.py
--rw-rw-rw-   0        0        0     8365 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/styles/label.py
--rw-rw-rw-   0        0        0     1631 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/styles/polygonmap.py
--rw-rw-rw-   0        0        0    13088 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/styles/shape.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.052176 plotpy-2.3.1/plotpy/tests/
--rw-rw-rw-   0        0        0      712 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.099055 plotpy-2.3.1/plotpy/tests/benchmarks/
--rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/benchmarks/__init__.py
--rw-rw-rw-   0        0        0     4226 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/benchmarks/test_benchmarks.py
--rw-rw-rw-   0        0        0      836 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/benchmarks/test_bigimages.py
--rw-rw-rw-   0        0        0     2847 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/benchmarks/test_loadtest.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.224050 plotpy-2.3.1/plotpy/tests/data/
--rw-rw-rw-   0        0        0    39666 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/data/brain.png
--rw-rw-rw-   0        0        0    35354 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/data/brain_cylinder.png
--rw-rw-rw-   0        0        0   525620 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/data/mr-brain.dcm
--rw-rw-rw-   0        0        0     1991 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/data/svg_target.svg
--rw-rw-rw-   0        0        0     1765 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/data/svg_tool.svg
--rw-rw-rw-   0        0        0     4363 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/data.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.520928 plotpy-2.3.1/plotpy/tests/features/
--rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/__init__.py
--rw-rw-rw-   0        0        0      906 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_auto_curve_image.py
--rw-rw-rw-   0        0        0     2542 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/features/test_autoscale_shapes.py
--rw-rw-rw-   0        0        0     1660 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_builder.py
--rw-rw-rw-   0        0        0     3014 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/features/test_colormap_editor.py
--rw-rw-rw-   0        0        0     2221 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/features/test_colormap_manager.py
--rw-rw-rw-   0        0        0     1381 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_computations.py
--rw-rw-rw-   0        0        0     1275 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_contrast.py
--rw-rw-rw-   0        0        0     1064 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_cursors.py
--rw-rw-rw-   0        0        0     1164 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_dicom_image.py
--rw-rw-rw-   0        0        0      798 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_fit.py
--rw-rw-rw-   0        0        0     1483 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_image_coords.py
--rw-rw-rw-   0        0        0     1648 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/features/test_imagefilter.py
--rw-rw-rw-   0        0        0     1576 2024-02-16 08:53:28.000000 plotpy-2.3.1/plotpy/tests/features/test_imagesuperp.py
--rw-rw-rw-   0        0        0     1116 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/tests/features/test_loadsaveitems_hdf5.py
--rw-rw-rw-   0        0        0     1453 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/tests/features/test_loadsaveitems_json.py
--rw-rw-rw-   0        0        0     6395 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/tests/features/test_loadsaveitems_pickle.py
--rw-rw-rw-   0        0        0     3123 2023-12-14 19:00:47.000000 plotpy-2.3.1/plotpy/tests/features/test_manager.py
--rw-rw-rw-   0        0        0      718 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_no_auto_tools.py
--rw-rw-rw-   0        0        0      927 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_plot_log.py
--rw-rw-rw-   0        0        0     1214 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_plot_types.py
--rw-rw-rw-   0        0        0      846 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_plot_yreverse.py
--rw-rw-rw-   0        0        0     2114 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_pyplot.py
--rw-rw-rw-   0        0        0      694 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/features/test_resize.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.645933 plotpy-2.3.1/plotpy/tests/items/
--rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/__init__.py
--rw-rw-rw-   0        0        0     1159 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_annotations.py
--rw-rw-rw-   0        0        0     1534 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/items/test_curves.py
--rw-rw-rw-   0        0        0     1660 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/items/test_curves_highdpi.py
--rw-rw-rw-   0        0        0     2298 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_hist2d.py
--rw-rw-rw-   0        0        0      710 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_histogram.py
--rw-rw-rw-   0        0        0      840 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_image.py
--rw-rw-rw-   0        0        0      989 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_image_contour.py
--rw-rw-rw-   0        0        0     1231 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_image_masked.py
--rw-rw-rw-   0        0        0     1336 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_image_masked_xy.py
--rw-rw-rw-   0        0        0      759 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_image_rgb.py
--rw-rw-rw-   0        0        0      758 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_image_xy.py
--rw-rw-rw-   0        0        0     2763 2023-12-14 19:00:47.000000 plotpy-2.3.1/plotpy/tests/items/test_mandelbrot.py
--rw-rw-rw-   0        0        0     2340 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_pcolor.py
--rw-rw-rw-   0        0        0     2363 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/tests/items/test_polygons.py
--rw-rw-rw-   0        0        0      881 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/items/test_svgshapes.py
--rw-rw-rw-   0        0        0     6217 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/items/test_transform.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:14.817807 plotpy-2.3.1/plotpy/tests/tools/
--rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/tools/__init__.py
--rw-rw-rw-   0        0        0     1492 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/tools/test_actiontool.py
--rw-rw-rw-   0        0        0     1151 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/tools/test_cross_section.py
--rw-rw-rw-   0        0        0     2466 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_cross_section_line.py
--rw-rw-rw-   0        0        0     1097 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_cross_section_oblique.py
--rw-rw-rw-   0        0        0     1804 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/tools/test_customize_shape_tool.py
--rw-rw-rw-   0        0        0     1692 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_downsample_curve.py
--rw-rw-rw-   0        0        0     2865 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_edit_point.py
--rw-rw-rw-   0        0        0     1757 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_get_point.py
--rw-rw-rw-   0        0        0     2215 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_get_points.py
--rw-rw-rw-   0        0        0     1118 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/tools/test_get_rectangle.py
--rw-rw-rw-   0        0        0     1741 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/tests/tools/test_get_rectangle_with_svg.py
--rw-rw-rw-   0        0        0     1954 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/tools/test_get_segment.py
--rw-rw-rw-   0        0        0     2155 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/tools/test_image_plot_tools.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.067803 plotpy-2.3.1/plotpy/tests/unit/
--rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/__init__.py
--rw-rw-rw-   0        0        0     3867 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_annotation_tools.py
--rw-rw-rw-   0        0        0     1125 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/unit/test_aspect_ratio_tool.py
--rw-rw-rw-   0        0        0     2165 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/unit/test_baseplot.py
--rw-rw-rw-   0        0        0     2728 2024-02-08 11:53:54.000000 plotpy-2.3.1/plotpy/tests/unit/test_builder_annotation.py
--rw-rw-rw-   0        0        0     6112 2024-02-08 11:53:54.000000 plotpy-2.3.1/plotpy/tests/unit/test_builder_curve.py
--rw-rw-rw-   0        0        0     3291 2024-02-16 08:53:28.000000 plotpy-2.3.1/plotpy/tests/unit/test_builder_image.py
--rw-rw-rw-   0        0        0     1655 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/unit/test_builder_shape.py
--rw-rw-rw-   0        0        0     2352 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_contour.py
--rw-rw-rw-   0        0        0     1497 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_cursor_tools.py
--rw-rw-rw-   0        0        0     7980 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_curve_tools.py
--rw-rw-rw-   0        0        0     2071 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_display_coords_tool.py
--rw-rw-rw-   0        0        0     5505 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_events.py
--rw-rw-rw-   0        0        0      415 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_fontparam.py
--rw-rw-rw-   0        0        0     2840 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_geometry.py
--rw-rw-rw-   0        0        0      937 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_highprecisionxy.py
--rw-rw-rw-   0        0        0     3234 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_io.py
--rw-rw-rw-   0        0        0     1702 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_line.py
--rw-rw-rw-   0        0        0      888 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/tests/unit/test_line_cross_section_tool.py
--rw-rw-rw-   0        0        0    14442 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_manipulate_selection.py
--rw-rw-rw-   0        0        0     2021 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_mask_tool.py
--rw-rw-rw-   0        0        0     2600 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_multiline_tools.py
--rw-rw-rw-   0        0        0      909 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/tests/unit/test_oblique_cross_section_tool.py
--rw-rw-rw-   0        0        0     2368 2024-02-08 11:53:54.000000 plotpy-2.3.1/plotpy/tests/unit/test_plot_curve.py
--rw-rw-rw-   0        0        0     5331 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/test_plot_image.py
--rw-rw-rw-   0        0        0     2165 2024-03-04 13:28:36.000000 plotpy-2.3.1/plotpy/tests/unit/test_rect_zoom.py
--rw-rw-rw-   0        0        0      839 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_seg_dist.py
--rw-rw-rw-   0        0        0     3032 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_styles.py
--rw-rw-rw-   0        0        0      854 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/unit/test_tools_export.py
--rw-rw-rw-   0        0        0     8320 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tests/unit/utils.py
--rw-rw-rw-   0        0        0     1320 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/tests/vistools.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.177182 plotpy-2.3.1/plotpy/tests/widgets/
--rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/widgets/__init__.py
--rw-rw-rw-   0        0        0     6910 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_dotarraydemo.py
--rw-rw-rw-   0        0        0     2725 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_filtertest1.py
--rw-rw-rw-   0        0        0     3530 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_filtertest2.py
--rw-rw-rw-   0        0        0     1698 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_fliprotate.py
--rw-rw-rw-   0        0        0    14422 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/widgets/test_plot_timecurve.py
--rw-rw-rw-   0        0        0     1185 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/widgets/test_qtdesigner.py
--rw-rw-rw-   0        0        0      763 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/widgets/test_qtdesigner.ui
--rw-rw-rw-   0        0        0     2173 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_resize_dialog.py
--rw-rw-rw-   0        0        0     2920 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_rotatecrop.py
--rw-rw-rw-   0        0        0     3740 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tests/widgets/test_simple_dialog.py
--rw-rw-rw-   0        0        0    10267 2023-12-14 19:00:47.000000 plotpy-2.3.1/plotpy/tests/widgets/test_simple_window.py
--rw-rw-rw-   0        0        0     2846 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tests/widgets/test_syncplot.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.317805 plotpy-2.3.1/plotpy/tools/
--rw-rw-rw-   0        0        0     1993 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/tools/__init__.py
--rw-rw-rw-   0        0        0     1945 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/annotation.py
--rw-rw-rw-   0        0        0     3382 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/axes.py
--rw-rw-rw-   0        0        0    18826 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tools/base.py
--rw-rw-rw-   0        0        0     4654 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/tools/cross_section.py
--rw-rw-rw-   0        0        0     3447 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/cursor.py
--rw-rw-rw-   0        0        0    42249 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tools/curve.py
--rw-rw-rw-   0        0        0    42618 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/tools/image.py
--rw-rw-rw-   0        0        0     6460 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/item.py
--rw-rw-rw-   0        0        0     3054 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/label.py
--rw-rw-rw-   0        0        0    11326 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/tools/misc.py
--rw-rw-rw-   0        0        0     6115 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/plot.py
--rw-rw-rw-   0        0        0     5730 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/selection.py
--rw-rw-rw-   0        0        0     9273 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/tools/shape.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.474052 plotpy-2.3.1/plotpy/widgets/
--rw-rw-rw-   0        0        0       25 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/widgets/__init__.py
--rw-rw-rw-   0        0        0     1777 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/widgets/about.py
--rw-rw-rw-   0        0        0    10076 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/widgets/basetransform.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.505304 plotpy-2.3.1/plotpy/widgets/colormap/
--rw-rw-rw-   0        0        0      358 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/widgets/colormap/__init__.py
--rw-rw-rw-   0        0        0     2221 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/widgets/colormap/_slider.py
--rw-rw-rw-   0        0        0    10513 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/widgets/colormap/editor.py
--rw-rw-rw-   0        0        0    15875 2024-05-06 16:40:26.000000 plotpy-2.3.1/plotpy/widgets/colormap/manager.py
--rw-rw-rw-   0        0        0    25006 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/widgets/colormap/widget.py
--rw-rw-rw-   0        0        0    30905 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/widgets/fit.py
--rw-rw-rw-   0        0        0     8505 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/widgets/fliprotate.py
--rw-rw-rw-   0        0        0     6375 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/widgets/imagefile.py
--rw-rw-rw-   0        0        0     4120 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy/widgets/qtdesigner.py
--rw-rw-rw-   0        0        0     4988 2024-02-08 10:33:36.000000 plotpy-2.3.1/plotpy/widgets/resizedialog.py
--rw-rw-rw-   0        0        0     8046 2024-04-10 16:39:34.000000 plotpy-2.3.1/plotpy/widgets/rotatecrop.py
--rw-rw-rw-   0        0        0     5841 2024-03-11 08:11:54.000000 plotpy-2.3.1/plotpy/widgets/selectdialog.py
--rw-rw-rw-   0        0        0      276 2023-11-23 17:46:00.000000 plotpy-2.3.1/plotpy-tests.desktop
--rw-rw-rw-   0        0        0     3410 2024-04-10 16:39:34.000000 plotpy-2.3.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.520927 plotpy-2.3.1/qtdesigner/
--rw-rw-rw-   0        0        0      361 2023-11-23 17:46:00.000000 plotpy-2.3.1/qtdesigner/plotplugin.py
--rw-rw-rw-   0        0        0      220 2024-04-10 16:39:34.000000 plotpy-2.3.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 16:41:15.583426 plotpy-2.3.1/setup.cfg
--rw-rw-rw-   0        0        0     3257 2023-12-22 08:06:28.000000 plotpy-2.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:41:15.567802 plotpy-2.3.1/src/
--rw-rw-rw-   0        0        0     5676 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/arrays.hpp
--rw-rw-rw-   0        0        0  1210847 2024-05-06 16:41:09.000000 plotpy-2.3.1/src/contour2d.c
--rw-rw-rw-   0        0        0    12546 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/contour2d.pyx
--rw-rw-rw-   0        0        0     1162 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/debug.hpp
--rw-rw-rw-   0        0        0   302415 2024-05-06 16:41:10.000000 plotpy-2.3.1/src/histogram2d.c
--rw-rw-rw-   0        0        0     3407 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/histogram2d.pyx
--rw-rw-rw-   0        0        0   240674 2024-05-06 16:41:10.000000 plotpy-2.3.1/src/mandelbrot.c
--rw-rw-rw-   0        0        0     1114 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/mandelbrot.pyx
--rw-rw-rw-   0        0        0    15123 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/pcolor.cpp
--rw-rw-rw-   0        0        0     7785 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/points.hpp
--rw-rw-rw-   0        0        0    26596 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/scaler.cpp
--rw-rw-rw-   0        0        0     2555 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/scaler.hpp
--rw-rw-rw-   0        0        0     4105 2023-11-23 17:46:00.000000 plotpy-2.3.1/src/traits.hpp
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:16.126802 plotpy-2.3.2/
+-rw-rw-rw-   0        0        0    16118 2024-05-07 08:00:25.000000 plotpy-2.3.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1563 2023-11-23 17:46:00.000000 plotpy-2.3.2/LICENSE
+-rw-rw-rw-   0        0        0      143 2024-04-10 16:39:34.000000 plotpy-2.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     8668 2024-05-07 08:01:16.126802 plotpy-2.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:16.126802 plotpy-2.3.2/PlotPy.egg-info/
+-rw-rw-rw-   0        0        0     8668 2024-05-07 08:01:12.000000 plotpy-2.3.2/PlotPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    16880 2024-05-07 08:01:12.000000 plotpy-2.3.2/PlotPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 08:01:12.000000 plotpy-2.3.2/PlotPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-07 08:01:12.000000 plotpy-2.3.2/PlotPy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      224 2024-05-07 08:01:12.000000 plotpy-2.3.2/PlotPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-07 08:01:12.000000 plotpy-2.3.2/PlotPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4379 2023-11-23 17:46:00.000000 plotpy-2.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:12.486181 plotpy-2.3.2/colormaps/
+-rw-rw-rw-   0        0        0      170 2024-02-08 10:33:36.000000 plotpy-2.3.2/colormaps/README.md
+-rw-rw-rw-   0        0        0   421433 2024-02-08 10:33:36.000000 plotpy-2.3.2/colormaps/_cm.py
+-rw-rw-rw-   0        0        0     3083 2024-02-09 17:39:23.000000 plotpy-2.3.2/colormaps/colormap.py
+-rw-rw-rw-   0        0        0     9391 2024-03-04 13:28:35.000000 plotpy-2.3.2/colormaps/matplotlib_cmaps.py
+-rw-rw-rw-   0        0        0      189 2024-04-10 16:39:34.000000 plotpy-2.3.2/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:12.533055 plotpy-2.3.2/doc/
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:12.548679 plotpy-2.3.2/doc/_static/
+-rw-rw-rw-   0        0        0   110568 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/_static/favicon.ico
+-rw-rw-rw-   0        0        0       79 2024-02-08 10:33:36.000000 plotpy-2.3.2/doc/changelog.rst
+-rw-rw-rw-   0        0        0     2273 2024-02-08 10:33:36.000000 plotpy-2.3.2/doc/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:12.673679 plotpy-2.3.2/doc/dev/
+-rw-rw-rw-   0        0        0     1003 2024-04-10 16:39:34.000000 plotpy-2.3.2/doc/dev/build.rst
+-rw-rw-rw-   0        0        0     4374 2024-04-10 16:39:34.000000 plotpy-2.3.2/doc/dev/contribute.rst
+-rw-rw-rw-   0        0        0     3108 2024-02-09 17:39:23.000000 plotpy-2.3.2/doc/dev/guiqwt_to_plotpy.csv
+-rw-rw-rw-   0        0        0     9868 2024-02-16 08:53:28.000000 plotpy-2.3.2/doc/dev/guiqwt_to_plotpy.rst
+-rw-rw-rw-   0        0        0      158 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/dev/index.rst
+-rw-rw-rw-   0        0        0     5039 2024-04-10 16:39:34.000000 plotpy-2.3.2/doc/dev/platforms.rst
+-rw-rw-rw-   0        0        0      389 2024-02-08 10:33:36.000000 plotpy-2.3.2/doc/dev/v1_to_guidata_v3.csv
+-rw-rw-rw-   0        0        0     2489 2024-02-09 17:39:23.000000 plotpy-2.3.2/doc/dev/v1_to_v2.csv
+-rw-rw-rw-   0        0        0     3374 2024-02-16 08:53:28.000000 plotpy-2.3.2/doc/dev/v1_to_v2.rst
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:12.720560 plotpy-2.3.2/doc/features/
+-rw-rw-rw-   0        0        0       41 2024-02-08 10:33:36.000000 plotpy-2.3.2/doc/features/colormapmanager.rst
+-rw-rw-rw-   0        0        0       31 2024-02-08 10:33:36.000000 plotpy-2.3.2/doc/features/events.rst
+-rw-rw-rw-   0        0        0       36 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/fit.rst
+-rw-rw-rw-   0        0        0       43 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/fliprotate.rst
+-rw-rw-rw-   0        0        0       42 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/imagefile.rst
+-rw-rw-rw-   0        0        0      327 2024-02-08 10:33:36.000000 plotpy-2.3.2/doc/features/index.rst
+-rw-rw-rw-   0        0        0       25 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/io.rst
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:12.767439 plotpy-2.3.2/doc/features/items/
+-rw-rw-rw-   0        0        0      784 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/items/builder.rst
+-rw-rw-rw-   0        0        0     4830 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/items/examples.rst
+-rw-rw-rw-   0        0        0      149 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/items/index.rst
+-rw-rw-rw-   0        0        0     2311 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/items/overview.rst
+-rw-rw-rw-   0        0        0     3319 2024-02-08 10:33:36.000000 plotpy-2.3.2/doc/features/items/reference.rst
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:12.783052 plotpy-2.3.2/doc/features/mathutils/
+-rw-rw-rw-   0        0        0       41 2024-02-09 17:39:23.000000 plotpy-2.3.2/doc/features/mathutils/colormaps.rst
+-rw-rw-rw-   0        0        0       41 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/mathutils/geometry.rst
+-rw-rw-rw-   0        0        0      119 2024-02-08 10:33:36.000000 plotpy-2.3.2/doc/features/mathutils/index.rst
+-rw-rw-rw-   0        0        0       39 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/mathutils/scaler.rst
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:12.798679 plotpy-2.3.2/doc/features/panels/
+-rw-rw-rw-   0        0        0      127 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/panels/index.rst
+-rw-rw-rw-   0        0        0      891 2024-02-08 10:33:36.000000 plotpy-2.3.2/doc/features/panels/overview.rst
+-rw-rw-rw-   0        0        0      212 2024-02-08 10:33:36.000000 plotpy-2.3.2/doc/features/panels/reference.rst
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:12.814310 plotpy-2.3.2/doc/features/plot/
+-rw-rw-rw-   0        0        0     1012 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/plot/examples.rst
+-rw-rw-rw-   0        0        0     1560 2024-02-08 10:33:36.000000 plotpy-2.3.2/doc/features/plot/index.rst
+-rw-rw-rw-   0        0        0     1150 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/plot/overview.rst
+-rw-rw-rw-   0        0        0      625 2024-02-08 10:33:36.000000 plotpy-2.3.2/doc/features/plot/reference.rst
+-rw-rw-rw-   0        0        0       51 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/pyplot.rst
+-rw-rw-rw-   0        0        0       45 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/resizedialog.rst
+-rw-rw-rw-   0        0        0       43 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/rotatecrop.rst
+-rw-rw-rw-   0        0        0       45 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/selectdialog.rst
+-rw-rw-rw-   0        0        0     1754 2024-03-04 12:33:14.000000 plotpy-2.3.2/doc/features/signals.rst
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:12.829934 plotpy-2.3.2/doc/features/styles/
+-rw-rw-rw-   0        0        0      157 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/styles/index.rst
+-rw-rw-rw-   0        0        0      540 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/styles/overview.rst
+-rw-rw-rw-   0        0        0     1921 2024-02-08 10:33:36.000000 plotpy-2.3.2/doc/features/styles/reference.rst
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:12.892431 plotpy-2.3.2/doc/features/tools/
+-rw-rw-rw-   0        0        0      289 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/tools/examples.rst
+-rw-rw-rw-   0        0        0      137 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/features/tools/index.rst
+-rw-rw-rw-   0        0        0     2747 2024-03-11 08:11:54.000000 plotpy-2.3.2/doc/features/tools/overview.rst
+-rw-rw-rw-   0        0        0     3717 2024-03-11 08:11:54.000000 plotpy-2.3.2/doc/features/tools/reference.rst
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.017429 plotpy-2.3.2/doc/images/
+-rw-rw-rw-   0        0        0    42675 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/my_plot_manager.png
+-rw-rw-rw-   0        0        0    31164 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/my_plot_manager.svg
+-rw-rw-rw-   0        0        0   240381 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/panorama.png
+-rw-rw-rw-   0        0        0  1914412 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/panorama.svg
+-rw-rw-rw-   0        0        0    55886 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/plot_widgets.png
+-rw-rw-rw-   0        0        0    30549 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/plot_widgets.svg
+-rw-rw-rw-   0        0        0     9809 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/plotpy-banner.png
+-rw-rw-rw-   0        0        0     7460 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/plotpy-vertical.png
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.158054 plotpy-2.3.2/doc/images/screenshots/
+-rw-rw-rw-   0        0        0    64597 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/__init__.png
+-rw-rw-rw-   0        0        0    37530 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/computations.png
+-rw-rw-rw-   0        0        0   179050 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/contrast.png
+-rw-rw-rw-   0        0        0   210107 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/cross_section.png
+-rw-rw-rw-   0        0        0   210494 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/cross_section2.png
+-rw-rw-rw-   0        0        0    81254 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/dotarraydemo.png
+-rw-rw-rw-   0        0        0    41879 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/filtertest1.png
+-rw-rw-rw-   0        0        0    49232 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/filtertest2.png
+-rw-rw-rw-   0        0        0    44646 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/fit.png
+-rw-rw-rw-   0        0        0    32653 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/get_point.png
+-rw-rw-rw-   0        0        0    77053 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/hist2d.png
+-rw-rw-rw-   0        0        0   269545 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/image_plot_tools.png
+-rw-rw-rw-   0        0        0   230644 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/imagefilter.png
+-rw-rw-rw-   0        0        0   163887 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/imagesuperp.png
+-rw-rw-rw-   0        0        0   143730 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/imagexy.png
+-rw-rw-rw-   0        0        0   168112 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/manager.png
+-rw-rw-rw-   0        0        0   231418 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/mandelbrot.png
+-rw-rw-rw-   0        0        0   172858 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/pcolor.png
+-rw-rw-rw-   0        0        0    76448 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/plot.png
+-rw-rw-rw-   0        0        0   173690 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/simple_dialog.png
+-rw-rw-rw-   0        0        0    59433 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/simple_window.png
+-rw-rw-rw-   0        0        0   456556 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/images/screenshots/transform.png
+-rw-rw-rw-   0        0        0     1651 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/index.rst
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.204928 plotpy-2.3.2/doc/intro/
+-rw-rw-rw-   0        0        0     2862 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/intro/examples.rst
+-rw-rw-rw-   0        0        0      164 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/intro/index.rst
+-rw-rw-rw-   0        0        0      675 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/intro/installation.rst
+-rw-rw-rw-   0        0        0   107599 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/intro/licenses.rst
+-rw-rw-rw-   0        0        0     2299 2024-04-10 16:39:34.000000 plotpy-2.3.2/doc/intro/motivation.rst
+-rw-rw-rw-   0        0        0     4815 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/intro/overview.rst
+-rw-rw-rw-   0        0        0     2429 2024-03-11 08:11:54.000000 plotpy-2.3.2/doc/requirements.rst
+-rw-rw-rw-   0        0        0      721 2023-11-23 17:46:00.000000 plotpy-2.3.2/doc/update_requirements.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.314308 plotpy-2.3.2/plotpy/
+-rw-rw-rw-   0        0        0     1053 2024-05-07 08:00:25.000000 plotpy-2.3.2/plotpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.392432 plotpy-2.3.2/plotpy/builder/
+-rw-rw-rw-   0        0        0     1114 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/builder/__init__.py
+-rw-rw-rw-   0        0        0    13033 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/builder/annotation.py
+-rw-rw-rw-   0        0        0    31776 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/builder/curvemarker.py
+-rw-rw-rw-   0        0        0    33708 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/builder/image.py
+-rw-rw-rw-   0        0        0    10062 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/builder/label.py
+-rw-rw-rw-   0        0        0    17119 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/builder/plot.py
+-rw-rw-rw-   0        0        0     5886 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/builder/shape.py
+-rw-rw-rw-   0        0        0    34344 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/config.py
+-rw-rw-rw-   0        0        0     4756 2024-02-16 08:53:28.000000 plotpy-2.3.2/plotpy/constants.py
+-rw-rw-rw-   0        0        0     2385 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/coords.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.408056 plotpy-2.3.2/plotpy/data/
+-rw-rw-rw-   0        0        0   328300 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/colormaps_default.json
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.611177 plotpy-2.3.2/plotpy/data/icons/
+-rw-rw-rw-   0        0        0      595 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/apply.png
+-rw-rw-rw-   0        0        0      897 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/arredit.png
+-rw-rw-rw-   0        0        0      637 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/arrow_down.png
+-rw-rw-rw-   0        0        0      638 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/arrow_up.png
+-rw-rw-rw-   0        0        0      868 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/autorefresh.png
+-rw-rw-rw-   0        0        0     1012 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/autoscale.png
+-rw-rw-rw-   0        0        0      513 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/axes.png
+-rw-rw-rw-   0        0        0      474 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/busy.png
+-rw-rw-rw-   0        0        0      478 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/cell_edit.png
+-rw-rw-rw-   0        0        0      346 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/center.png
+-rw-rw-rw-   0        0        0      495 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/cmap_edit.png
+-rw-rw-rw-   0        0        0      316 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/contrast.png
+-rw-rw-rw-   0        0        0      620 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/copy.png
+-rw-rw-rw-   0        0        0      979 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/copytoclipboard.png
+-rw-rw-rw-   0        0        0      705 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/csapplylut.png
+-rw-rw-rw-   0        0        0      178 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/csautoscale.png
+-rw-rw-rw-   0        0        0      346 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/csection.png
+-rw-rw-rw-   0        0        0      310 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/csection_a.png
+-rw-rw-rw-   0        0        0      375 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/csection_line.png
+-rw-rw-rw-   0        0        0      711 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/csection_oblique.png
+-rw-rw-rw-   0        0        0      160 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/csperimage.png
+-rw-rw-rw-   0        0        0      758 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/curve_downsample.png
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.611177 plotpy-2.3.2/plotpy/data/icons/curvestyles/
+-rw-rw-rw-   0        0        0      121 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/curvestyles/dots.png
+-rw-rw-rw-   0        0        0      164 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/curvestyles/lines.png
+-rw-rw-rw-   0        0        0      136 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/curvestyles/steps.png
+-rw-rw-rw-   0        0        0      187 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/curvestyles/sticks.png
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.626801 plotpy-2.3.2/plotpy/data/icons/curvetypes/
+-rw-rw-rw-   0        0        0      322 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/curvetypes/xfy.png
+-rw-rw-rw-   0        0        0      322 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/curvetypes/yfx.png
+-rw-rw-rw-   0        0        0      496 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/delete.png
+-rw-rw-rw-   0        0        0      718 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/edit.png
+-rw-rw-rw-   0        0        0      793 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/edit_point_selection.png
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.673678 plotpy-2.3.2/plotpy/data/icons/editors/
+-rw-rw-rw-   0        0        0      718 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/editors/edit.png
+-rw-rw-rw-   0        0        0      790 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/editors/edit_add.png
+-rw-rw-rw-   0        0        0      837 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/editors/editcopy.png
+-rw-rw-rw-   0        0        0     1242 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/editors/editdelete.png
+-rw-rw-rw-   0        0        0     1084 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/editors/editpaste.png
+-rw-rw-rw-   0        0        0     2065 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/editors/fileimport.png
+-rw-rw-rw-   0        0        0      970 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/editors/filesave.png
+-rw-rw-rw-   0        0        0      516 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/editors/imshow.png
+-rw-rw-rw-   0        0        0      314 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/editors/insert.png
+-rw-rw-rw-   0        0        0      304 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/editors/plot.png
+-rw-rw-rw-   0        0        0      478 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/editors/rename.png
+-rw-rw-rw-   0        0        0      183 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/eliminate_outliers.png
+-rw-rw-rw-   0        0        0      671 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/eraser.png
+-rw-rw-rw-   0        0        0      974 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/exit.png
+-rw-rw-rw-   0        0        0      191 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/expander_down.png
+-rw-rw-rw-   0        0        0      184 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/expander_right.png
+-rw-rw-rw-   0        0        0      861 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/export.png
+-rw-rw-rw-   0        0        0      304 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/file.png
+-rw-rw-rw-   0        0        0     1213 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/fileclose.png
+-rw-rw-rw-   0        0        0     1383 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/fileimport.png
+-rw-rw-rw-   0        0        0      271 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/filenew.png
+-rw-rw-rw-   0        0        0     1349 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/fileopen.png
+-rw-rw-rw-   0        0        0      970 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/filesave.png
+-rw-rw-rw-   0        0        0     1264 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/filesaveas.png
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.689307 plotpy-2.3.2/plotpy/data/icons/filetypes/
+-rw-rw-rw-   0        0        0     1389 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/doc.png
+-rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/gif.png
+-rw-rw-rw-   0        0        0     1658 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/html.png
+-rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/jpg.png
+-rw-rw-rw-   0        0        0     1352 2024-03-04 13:28:35.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/pdf.png
+-rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/png.png
+-rw-rw-rw-   0        0        0     1226 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/pps.png
+-rw-rw-rw-   0        0        0     1217 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/ps.png
+-rw-rw-rw-   0        0        0     1385 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/tar.png
+-rw-rw-rw-   0        0        0     1385 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/tgz.png
+-rw-rw-rw-   0        0        0     1319 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/tif.png
+-rw-rw-rw-   0        0        0     1609 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/txt.png
+-rw-rw-rw-   0        0        0     1026 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/xls.png
+-rw-rw-rw-   0        0        0     1385 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/filetypes/zip.png
+-rw-rw-rw-   0        0        0      244 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/font.png
+-rw-rw-rw-   0        0        0      185 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/full_range.png
+-rw-rw-rw-   0        0        0      922 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/funct.png
+-rw-rw-rw-   0        0        0      151 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/hcursor.png
+-rw-rw-rw-   0        0        0      433 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/hflip.png
+-rw-rw-rw-   0        0        0      793 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/imagestats.png
+-rw-rw-rw-   0        0        0      437 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/item_list.png
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.704927 plotpy-2.3.2/plotpy/data/icons/items/
+-rw-rw-rw-   0        0        0      687 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/items/annotation.png
+-rw-rw-rw-   0        0        0      305 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/items/curve.png
+-rw-rw-rw-   0        0        0      172 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/items/errorbar.png
+-rw-rw-rw-   0        0        0      120 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/items/grid.png
+-rw-rw-rw-   0        0        0      140 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/items/histogram.png
+-rw-rw-rw-   0        0        0      857 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/items/histogram2d.png
+-rw-rw-rw-   0        0        0      852 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/items/image.png
+-rw-rw-rw-   0        0        0      531 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/items/label.png
+-rw-rw-rw-   0        0        0      317 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/items/legend.png
+-rw-rw-rw-   0        0        0      448 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/items/polygonmap.png
+-rw-rw-rw-   0        0        0      673 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/magnifier.png
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.720551 plotpy-2.3.2/plotpy/data/icons/markers/
+-rw-rw-rw-   0        0        0      123 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markers/cross.png
+-rw-rw-rw-   0        0        0      194 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markers/diamond.png
+-rw-rw-rw-   0        0        0      241 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markers/ellipse.png
+-rw-rw-rw-   0        0        0      260 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markers/hexagon.png
+-rw-rw-rw-   0        0        0      105 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markers/point.png
+-rw-rw-rw-   0        0        0      137 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markers/square.png
+-rw-rw-rw-   0        0        0      160 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markers/star.png
+-rw-rw-rw-   0        0        0      223 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markers/triangle_d.png
+-rw-rw-rw-   0        0        0      220 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markers/triangle_l.png
+-rw-rw-rw-   0        0        0      212 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markers/triangle_r.png
+-rw-rw-rw-   0        0        0      224 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markers/triangle_u.png
+-rw-rw-rw-   0        0        0      145 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markers/xcross.png
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.720551 plotpy-2.3.2/plotpy/data/icons/markerstyles/
+-rw-rw-rw-   0        0        0       96 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markerstyles/cross_marker.png
+-rw-rw-rw-   0        0        0       82 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markerstyles/horiz_marker.png
+-rw-rw-rw-   0        0        0       84 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/markerstyles/vert_marker.png
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.720551 plotpy-2.3.2/plotpy/data/icons/mask/
+-rw-rw-rw-   0        0        0      368 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/mask/mask_circle.png
+-rw-rw-rw-   0        0        0      374 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/mask/mask_circle_outside.png
+-rw-rw-rw-   0        0        0      199 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/mask/mask_rectangle.png
+-rw-rw-rw-   0        0        0      200 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/mask/mask_rectangle_outside.png
+-rw-rw-rw-   0        0        0      164 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/mask/mask_tool.png
+-rw-rw-rw-   0        0        0      130 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/max.png
+-rw-rw-rw-   0        0        0      125 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/min.png
+-rw-rw-rw-   0        0        0      132 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/move.png
+-rw-rw-rw-   0        0        0      729 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/multipoint_selection.png
+-rw-rw-rw-   0        0        0       83 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/none.png
+-rw-rw-rw-   0        0        0      284 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/not_found.png
+-rw-rw-rw-   0        0        0      397 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/on_curve.png
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.736176 plotpy-2.3.2/plotpy/data/icons/patterns/
+-rw-rw-rw-   0        0        0      104 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/bdiagpattern.png
+-rw-rw-rw-   0        0        0       90 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/crosspattern.png
+-rw-rw-rw-   0        0        0       76 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/dense1pattern.png
+-rw-rw-rw-   0        0        0       78 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/dense2pattern.png
+-rw-rw-rw-   0        0        0       83 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/dense3pattern.png
+-rw-rw-rw-   0        0        0       73 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/dense4pattern.png
+-rw-rw-rw-   0        0        0       88 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/dense5pattern.png
+-rw-rw-rw-   0        0        0       87 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/dense6pattern.png
+-rw-rw-rw-   0        0        0       84 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/dense7pattern.png
+-rw-rw-rw-   0        0        0      114 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/diagcrosspattern.png
+-rw-rw-rw-   0        0        0      112 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/fdiagpattern.png
+-rw-rw-rw-   0        0        0       82 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/horpattern.png
+-rw-rw-rw-   0        0        0       74 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/nobrush.png
+-rw-rw-rw-   0        0        0       69 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/solidpattern.png
+-rw-rw-rw-   0        0        0       83 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/patterns/verpattern.png
+-rw-rw-rw-   0        0        0    17636 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/plotpy-banner.svg
+-rw-rw-rw-   0        0        0    17614 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/plotpy-vertical.svg
+-rw-rw-rw-   0        0        0    16339 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/plotpy.svg
+-rw-rw-rw-   0        0        0      216 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/point_selection.png
+-rw-rw-rw-   0        0        0      723 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/print.png
+-rw-rw-rw-   0        0        0      697 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/python.png
+-rw-rw-rw-   0        0        0      677 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/quickview.png
+-rw-rw-rw-   0        0        0      823 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/rectangular_select.png
+-rw-rw-rw-   0        0        0      740 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/refresh.png
+-rw-rw-rw-   0        0        0     1428 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/save_all.png
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.736176 plotpy-2.3.2/plotpy/data/icons/scales/
+-rw-rw-rw-   0        0        0      203 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/scales/lin_lin.png
+-rw-rw-rw-   0        0        0      208 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/scales/lin_log.png
+-rw-rw-rw-   0        0        0      219 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/scales/log_lin.png
+-rw-rw-rw-   0        0        0      222 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/scales/log_log.png
+-rw-rw-rw-   0        0        0      518 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/selection.png
+-rw-rw-rw-   0        0        0      851 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/settings.png
+-rw-rw-rw-   0        0        0      135 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/shape.png
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.751802 plotpy-2.3.2/plotpy/data/icons/shapes/
+-rw-rw-rw-   0        0        0      530 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/shapes/circle.png
+-rw-rw-rw-   0        0        0      622 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/shapes/contour.png
+-rw-rw-rw-   0        0        0      547 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/shapes/ellipse_shape.png
+-rw-rw-rw-   0        0        0      305 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/shapes/freeform.png
+-rw-rw-rw-   0        0        0      321 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/shapes/gtaxes.png
+-rw-rw-rw-   0        0        0      179 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/shapes/marker.png
+-rw-rw-rw-   0        0        0      650 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/shapes/oblique_rectangle.png
+-rw-rw-rw-   0        0        0      118 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/shapes/point_shape.png
+-rw-rw-rw-   0        0        0      232 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/shapes/polyline.png
+-rw-rw-rw-   0        0        0      179 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/shapes/rectangle.png
+-rw-rw-rw-   0        0        0      220 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/shapes/segment.png
+-rw-rw-rw-   0        0        0     1150 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/snapshot.png
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.751802 plotpy-2.3.2/plotpy/data/icons/styles/
+-rw-rw-rw-   0        0        0       85 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/styles/dash.png
+-rw-rw-rw-   0        0        0       90 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/styles/dashdot.png
+-rw-rw-rw-   0        0        0       84 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/styles/dashdotdot.png
+-rw-rw-rw-   0        0        0       80 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/styles/dot.png
+-rw-rw-rw-   0        0        0       80 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/styles/solid.png
+-rw-rw-rw-   0        0        0      236 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/trash.png
+-rw-rw-rw-   0        0        0      932 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/trimage_lock.png
+-rw-rw-rw-   0        0        0      958 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/trimage_unlock.png
+-rw-rw-rw-   0        0        0      159 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/vcursor.png
+-rw-rw-rw-   0        0        0      432 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/vflip.png
+-rw-rw-rw-   0        0        0      127 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/xcursor.png
+-rw-rw-rw-   0        0        0      128 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/xmax.png
+-rw-rw-rw-   0        0        0      127 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/xmin.png
+-rw-rw-rw-   0        0        0      170 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/data/icons/xrange.png
+-rw-rw-rw-   0        0        0    46755 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/events.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.767429 plotpy-2.3.2/plotpy/external/
+-rw-rw-rw-   0        0        0      399 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/external/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.876805 plotpy-2.3.2/plotpy/external/sliders/
+-rw-rw-rw-   0        0        0     2108 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/external/sliders/__init__.py
+-rw-rw-rw-   0        0        0    14101 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/external/sliders/_generic_range_slider.py
+-rw-rw-rw-   0        0        0    20447 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/external/sliders/_generic_slider.py
+-rw-rw-rw-   0        0        0    23960 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/external/sliders/_labeled.py
+-rw-rw-rw-   0        0        0      758 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/external/sliders/_misc.py
+-rw-rw-rw-   0        0        0     9829 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/external/sliders/_range_style.py
+-rw-rw-rw-   0        0        0     1126 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/external/sliders/_sliders.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:13.923674 plotpy-2.3.2/plotpy/interfaces/
+-rw-rw-rw-   0        0        0      517 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/interfaces/__init__.py
+-rw-rw-rw-   0        0        0    14685 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/interfaces/items.py
+-rw-rw-rw-   0        0        0      461 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/interfaces/panel.py
+-rw-rw-rw-   0        0        0     1049 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/interfaces/plotmanager.py
+-rw-rw-rw-   0        0        0    24077 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/io.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.033058 plotpy-2.3.2/plotpy/items/
+-rw-rw-rw-   0        0        0     1517 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/items/__init__.py
+-rw-rw-rw-   0        0        0    30198 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/annotation.py
+-rw-rw-rw-   0        0        0     6355 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/items/contour.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.095563 plotpy-2.3.2/plotpy/items/curve/
+-rw-rw-rw-   0        0        0      176 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/items/curve/__init__.py
+-rw-rw-rw-   0        0        0    18860 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/curve/base.py
+-rw-rw-rw-   0        0        0    12987 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/curve/errorbar.py
+-rw-rw-rw-   0        0        0     7632 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/grid.py
+-rw-rw-rw-   0        0        0     7118 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/histogram.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.189305 plotpy-2.3.2/plotpy/items/image/
+-rw-rw-rw-   0        0        0      608 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/items/image/__init__.py
+-rw-rw-rw-   0        0        0    44532 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/image/base.py
+-rw-rw-rw-   0        0        0    11447 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/image/filter.py
+-rw-rw-rw-   0        0        0    28332 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/image/image_items.py
+-rw-rw-rw-   0        0        0    24911 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/image/masked.py
+-rw-rw-rw-   0        0        0    25205 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/image/misc.py
+-rw-rw-rw-   0        0        0    23529 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/image/transform.py
+-rw-rw-rw-   0        0        0    32816 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/items/label.py
+-rw-rw-rw-   0        0        0    13551 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/polygonmap.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.298679 plotpy-2.3.2/plotpy/items/shape/
+-rw-rw-rw-   0        0        0      457 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/items/shape/__init__.py
+-rw-rw-rw-   0        0        0     9972 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/shape/axis.py
+-rw-rw-rw-   0        0        0     8592 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/shape/base.py
+-rw-rw-rw-   0        0        0    11893 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/shape/ellipse.py
+-rw-rw-rw-   0        0        0    16554 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/shape/marker.py
+-rw-rw-rw-   0        0        0     2611 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/shape/point.py
+-rw-rw-rw-   0        0        0    14718 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/shape/polygon.py
+-rw-rw-rw-   0        0        0     9735 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/items/shape/range.py
+-rw-rw-rw-   0        0        0    11459 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/shape/rectangle.py
+-rw-rw-rw-   0        0        0     4581 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/items/shape/segment.py
+-rw-rw-rw-   0        0        0     4619 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/items/shape/svg.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:12.298682 plotpy-2.3.2/plotpy/locale/
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:12.298682 plotpy-2.3.2/plotpy/locale/fr/
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.298679 plotpy-2.3.2/plotpy/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    32854 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/locale/fr/LC_MESSAGES/plotpy.mo
+-rw-rw-rw-   0        0        0     1918 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/lutrange.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.376801 plotpy-2.3.2/plotpy/mathutils/
+-rw-rw-rw-   0        0        0       25 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/mathutils/__init__.py
+-rw-rw-rw-   0        0        0     1739 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/mathutils/arrayfuncs.py
+-rw-rw-rw-   0        0        0    10325 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/mathutils/colormap.py
+-rw-rw-rw-   0        0        0     6803 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/mathutils/geometry.py
+-rw-rw-rw-   0        0        0     1892 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/mathutils/scaler.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.423687 plotpy-2.3.2/plotpy/panels/
+-rw-rw-rw-   0        0        0      270 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/panels/__init__.py
+-rw-rw-rw-   0        0        0     2345 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/panels/base.py
+-rw-rw-rw-   0        0        0    19745 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/panels/contrastadjustment.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.454940 plotpy-2.3.2/plotpy/panels/csection/
+-rw-rw-rw-   0        0        0      480 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/panels/csection/__init__.py
+-rw-rw-rw-   0        0        0    17094 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/panels/csection/csitem.py
+-rw-rw-rw-   0        0        0    16887 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/panels/csection/csplot.py
+-rw-rw-rw-   0        0        0    12868 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/panels/csection/cswidget.py
+-rw-rw-rw-   0        0        0     9425 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/panels/itemlist.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.548674 plotpy-2.3.2/plotpy/plot/
+-rw-rw-rw-   0        0        0      325 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/plot/__init__.py
+-rw-rw-rw-   0        0        0    85147 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/plot/base.py
+-rw-rw-rw-   0        0        0    22002 2024-02-09 17:39:23.000000 plotpy-2.3.2/plotpy/plot/interactive.py
+-rw-rw-rw-   0        0        0    25295 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/plot/manager.py
+-rw-rw-rw-   0        0        0    34516 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/plot/plotwidget.py
+-rw-rw-rw-   0        0        0     2762 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/pyplot.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.642430 plotpy-2.3.2/plotpy/styles/
+-rw-rw-rw-   0        0        0     1738 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/styles/__init__.py
+-rw-rw-rw-   0        0        0     4155 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/styles/axes.py
+-rw-rw-rw-   0        0        0    19338 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/styles/base.py
+-rw-rw-rw-   0        0        0     3172 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/styles/curve.py
+-rw-rw-rw-   0        0        0     1552 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/styles/errorbar.py
+-rw-rw-rw-   0        0        0     3896 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/styles/histogram.py
+-rw-rw-rw-   0        0        0    18053 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/styles/image.py
+-rw-rw-rw-   0        0        0     8365 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/styles/label.py
+-rw-rw-rw-   0        0        0     1631 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/styles/polygonmap.py
+-rw-rw-rw-   0        0        0    13088 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/styles/shape.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.673682 plotpy-2.3.2/plotpy/tests/
+-rw-rw-rw-   0        0        0      712 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.689306 plotpy-2.3.2/plotpy/tests/benchmarks/
+-rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/benchmarks/__init__.py
+-rw-rw-rw-   0        0        0     4226 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/benchmarks/test_benchmarks.py
+-rw-rw-rw-   0        0        0      836 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/benchmarks/test_bigimages.py
+-rw-rw-rw-   0        0        0     2847 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/benchmarks/test_loadtest.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.704935 plotpy-2.3.2/plotpy/tests/data/
+-rw-rw-rw-   0        0        0    39666 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/data/brain.png
+-rw-rw-rw-   0        0        0    35354 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/data/brain_cylinder.png
+-rw-rw-rw-   0        0        0   525620 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/data/mr-brain.dcm
+-rw-rw-rw-   0        0        0     1991 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/data/svg_target.svg
+-rw-rw-rw-   0        0        0     1765 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/data/svg_tool.svg
+-rw-rw-rw-   0        0        0     4363 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/data.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:14.939306 plotpy-2.3.2/plotpy/tests/features/
+-rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/__init__.py
+-rw-rw-rw-   0        0        0      906 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_auto_curve_image.py
+-rw-rw-rw-   0        0        0     2542 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/features/test_autoscale_shapes.py
+-rw-rw-rw-   0        0        0     1660 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_builder.py
+-rw-rw-rw-   0        0        0     3014 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/features/test_colormap_editor.py
+-rw-rw-rw-   0        0        0     2210 2024-05-07 08:00:25.000000 plotpy-2.3.2/plotpy/tests/features/test_colormap_manager.py
+-rw-rw-rw-   0        0        0     1381 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_computations.py
+-rw-rw-rw-   0        0        0     1275 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_contrast.py
+-rw-rw-rw-   0        0        0     1064 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_cursors.py
+-rw-rw-rw-   0        0        0     1164 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_dicom_image.py
+-rw-rw-rw-   0        0        0      798 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_fit.py
+-rw-rw-rw-   0        0        0     1483 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_image_coords.py
+-rw-rw-rw-   0        0        0     1648 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/features/test_imagefilter.py
+-rw-rw-rw-   0        0        0     1576 2024-02-16 08:53:28.000000 plotpy-2.3.2/plotpy/tests/features/test_imagesuperp.py
+-rw-rw-rw-   0        0        0     1116 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/tests/features/test_loadsaveitems_hdf5.py
+-rw-rw-rw-   0        0        0     1453 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/tests/features/test_loadsaveitems_json.py
+-rw-rw-rw-   0        0        0     6395 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/tests/features/test_loadsaveitems_pickle.py
+-rw-rw-rw-   0        0        0     3123 2023-12-14 19:00:47.000000 plotpy-2.3.2/plotpy/tests/features/test_manager.py
+-rw-rw-rw-   0        0        0      718 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_no_auto_tools.py
+-rw-rw-rw-   0        0        0      927 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_plot_log.py
+-rw-rw-rw-   0        0        0     1214 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_plot_types.py
+-rw-rw-rw-   0        0        0      846 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_plot_yreverse.py
+-rw-rw-rw-   0        0        0     2114 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_pyplot.py
+-rw-rw-rw-   0        0        0      694 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/features/test_resize.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:15.064311 plotpy-2.3.2/plotpy/tests/items/
+-rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/items/__init__.py
+-rw-rw-rw-   0        0        0     1159 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/items/test_annotations.py
+-rw-rw-rw-   0        0        0     1493 2024-05-07 08:00:25.000000 plotpy-2.3.2/plotpy/tests/items/test_curves.py
+-rw-rw-rw-   0        0        0     1660 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/tests/items/test_curves_highdpi.py
+-rw-rw-rw-   0        0        0     2298 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/items/test_hist2d.py
+-rw-rw-rw-   0        0        0      710 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/items/test_histogram.py
+-rw-rw-rw-   0        0        0      840 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/items/test_image.py
+-rw-rw-rw-   0        0        0      989 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/items/test_image_contour.py
+-rw-rw-rw-   0        0        0     1231 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/items/test_image_masked.py
+-rw-rw-rw-   0        0        0     1336 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/items/test_image_masked_xy.py
+-rw-rw-rw-   0        0        0      759 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/items/test_image_rgb.py
+-rw-rw-rw-   0        0        0      758 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/items/test_image_xy.py
+-rw-rw-rw-   0        0        0     2763 2023-12-14 19:00:47.000000 plotpy-2.3.2/plotpy/tests/items/test_mandelbrot.py
+-rw-rw-rw-   0        0        0     2340 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/items/test_pcolor.py
+-rw-rw-rw-   0        0        0     2363 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/tests/items/test_polygons.py
+-rw-rw-rw-   0        0        0      881 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/items/test_svgshapes.py
+-rw-rw-rw-   0        0        0     6217 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/items/test_transform.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:15.251806 plotpy-2.3.2/plotpy/tests/tools/
+-rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/tools/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/tools/test_actiontool.py
+-rw-rw-rw-   0        0        0     1151 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/tools/test_cross_section.py
+-rw-rw-rw-   0        0        0     2466 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/tests/tools/test_cross_section_line.py
+-rw-rw-rw-   0        0        0     1097 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/tests/tools/test_cross_section_oblique.py
+-rw-rw-rw-   0        0        0     1804 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/tools/test_customize_shape_tool.py
+-rw-rw-rw-   0        0        0     1692 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/tests/tools/test_downsample_curve.py
+-rw-rw-rw-   0        0        0     2865 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/tests/tools/test_edit_point.py
+-rw-rw-rw-   0        0        0     1757 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/tests/tools/test_get_point.py
+-rw-rw-rw-   0        0        0     2215 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/tests/tools/test_get_points.py
+-rw-rw-rw-   0        0        0     1118 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/tools/test_get_rectangle.py
+-rw-rw-rw-   0        0        0     1741 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/tests/tools/test_get_rectangle_with_svg.py
+-rw-rw-rw-   0        0        0     1954 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/tools/test_get_segment.py
+-rw-rw-rw-   0        0        0     2155 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/tools/test_image_plot_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:15.595556 plotpy-2.3.2/plotpy/tests/unit/
+-rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/unit/__init__.py
+-rw-rw-rw-   0        0        0     3867 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/tests/unit/test_annotation_tools.py
+-rw-rw-rw-   0        0        0     1125 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/unit/test_aspect_ratio_tool.py
+-rw-rw-rw-   0        0        0     2165 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/unit/test_baseplot.py
+-rw-rw-rw-   0        0        0     2728 2024-02-08 11:53:54.000000 plotpy-2.3.2/plotpy/tests/unit/test_builder_annotation.py
+-rw-rw-rw-   0        0        0     6112 2024-02-08 11:53:54.000000 plotpy-2.3.2/plotpy/tests/unit/test_builder_curve.py
+-rw-rw-rw-   0        0        0     3291 2024-02-16 08:53:28.000000 plotpy-2.3.2/plotpy/tests/unit/test_builder_image.py
+-rw-rw-rw-   0        0        0     1655 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/unit/test_builder_shape.py
+-rw-rw-rw-   0        0        0     2352 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/unit/test_contour.py
+-rw-rw-rw-   0        0        0     1497 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/tests/unit/test_cursor_tools.py
+-rw-rw-rw-   0        0        0     7980 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/tests/unit/test_curve_tools.py
+-rw-rw-rw-   0        0        0     2071 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/tests/unit/test_display_coords_tool.py
+-rw-rw-rw-   0        0        0     5505 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/tests/unit/test_events.py
+-rw-rw-rw-   0        0        0      415 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/unit/test_fontparam.py
+-rw-rw-rw-   0        0        0     2840 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/unit/test_geometry.py
+-rw-rw-rw-   0        0        0      937 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/unit/test_highprecisionxy.py
+-rw-rw-rw-   0        0        0     3234 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/unit/test_io.py
+-rw-rw-rw-   0        0        0     1702 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/unit/test_line.py
+-rw-rw-rw-   0        0        0      888 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/tests/unit/test_line_cross_section_tool.py
+-rw-rw-rw-   0        0        0    14442 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/tests/unit/test_manipulate_selection.py
+-rw-rw-rw-   0        0        0     2021 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/tests/unit/test_mask_tool.py
+-rw-rw-rw-   0        0        0     2600 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/tests/unit/test_multiline_tools.py
+-rw-rw-rw-   0        0        0      909 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/tests/unit/test_oblique_cross_section_tool.py
+-rw-rw-rw-   0        0        0     2368 2024-02-08 11:53:54.000000 plotpy-2.3.2/plotpy/tests/unit/test_plot_curve.py
+-rw-rw-rw-   0        0        0     5331 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/tests/unit/test_plot_image.py
+-rw-rw-rw-   0        0        0     2165 2024-03-04 13:28:36.000000 plotpy-2.3.2/plotpy/tests/unit/test_rect_zoom.py
+-rw-rw-rw-   0        0        0      839 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/unit/test_seg_dist.py
+-rw-rw-rw-   0        0        0     3032 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/unit/test_styles.py
+-rw-rw-rw-   0        0        0      854 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/unit/test_tools_export.py
+-rw-rw-rw-   0        0        0     8320 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/tests/unit/utils.py
+-rw-rw-rw-   0        0        0     1320 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/tests/vistools.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:15.736181 plotpy-2.3.2/plotpy/tests/widgets/
+-rw-rw-rw-   0        0        0        0 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/widgets/__init__.py
+-rw-rw-rw-   0        0        0     6910 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/widgets/test_dotarraydemo.py
+-rw-rw-rw-   0        0        0     2725 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/widgets/test_filtertest1.py
+-rw-rw-rw-   0        0        0     3530 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/widgets/test_filtertest2.py
+-rw-rw-rw-   0        0        0     1698 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/widgets/test_fliprotate.py
+-rw-rw-rw-   0        0        0    14422 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/widgets/test_plot_timecurve.py
+-rw-rw-rw-   0        0        0     1185 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/widgets/test_qtdesigner.py
+-rw-rw-rw-   0        0        0      763 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/widgets/test_qtdesigner.ui
+-rw-rw-rw-   0        0        0     2173 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/widgets/test_resize_dialog.py
+-rw-rw-rw-   0        0        0     2920 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/widgets/test_rotatecrop.py
+-rw-rw-rw-   0        0        0     3740 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tests/widgets/test_simple_dialog.py
+-rw-rw-rw-   0        0        0    10267 2023-12-14 19:00:47.000000 plotpy-2.3.2/plotpy/tests/widgets/test_simple_window.py
+-rw-rw-rw-   0        0        0     2846 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tests/widgets/test_syncplot.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:15.876805 plotpy-2.3.2/plotpy/tools/
+-rw-rw-rw-   0        0        0     1993 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/tools/__init__.py
+-rw-rw-rw-   0        0        0     1945 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tools/annotation.py
+-rw-rw-rw-   0        0        0     3382 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tools/axes.py
+-rw-rw-rw-   0        0        0    18826 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tools/base.py
+-rw-rw-rw-   0        0        0     4654 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/tools/cross_section.py
+-rw-rw-rw-   0        0        0     3447 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tools/cursor.py
+-rw-rw-rw-   0        0        0    42249 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/tools/curve.py
+-rw-rw-rw-   0        0        0    42618 2024-05-06 16:40:26.000000 plotpy-2.3.2/plotpy/tools/image.py
+-rw-rw-rw-   0        0        0     6460 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tools/item.py
+-rw-rw-rw-   0        0        0     3054 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tools/label.py
+-rw-rw-rw-   0        0        0    11326 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/tools/misc.py
+-rw-rw-rw-   0        0        0     6115 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tools/plot.py
+-rw-rw-rw-   0        0        0     5730 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tools/selection.py
+-rw-rw-rw-   0        0        0     9273 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/tools/shape.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:16.033059 plotpy-2.3.2/plotpy/widgets/
+-rw-rw-rw-   0        0        0       25 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1777 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/widgets/about.py
+-rw-rw-rw-   0        0        0    10076 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/widgets/basetransform.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:16.064306 plotpy-2.3.2/plotpy/widgets/colormap/
+-rw-rw-rw-   0        0        0      358 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/widgets/colormap/__init__.py
+-rw-rw-rw-   0        0        0     2221 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/widgets/colormap/_slider.py
+-rw-rw-rw-   0        0        0    10513 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/widgets/colormap/editor.py
+-rw-rw-rw-   0        0        0    16039 2024-05-07 08:00:25.000000 plotpy-2.3.2/plotpy/widgets/colormap/manager.py
+-rw-rw-rw-   0        0        0    25006 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/widgets/colormap/widget.py
+-rw-rw-rw-   0        0        0    30905 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/widgets/fit.py
+-rw-rw-rw-   0        0        0     8505 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/widgets/fliprotate.py
+-rw-rw-rw-   0        0        0     6375 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/widgets/imagefile.py
+-rw-rw-rw-   0        0        0     4120 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy/widgets/qtdesigner.py
+-rw-rw-rw-   0        0        0     4988 2024-02-08 10:33:36.000000 plotpy-2.3.2/plotpy/widgets/resizedialog.py
+-rw-rw-rw-   0        0        0     8046 2024-04-10 16:39:34.000000 plotpy-2.3.2/plotpy/widgets/rotatecrop.py
+-rw-rw-rw-   0        0        0     5841 2024-03-11 08:11:54.000000 plotpy-2.3.2/plotpy/widgets/selectdialog.py
+-rw-rw-rw-   0        0        0      276 2023-11-23 17:46:00.000000 plotpy-2.3.2/plotpy-tests.desktop
+-rw-rw-rw-   0        0        0     3410 2024-04-10 16:39:34.000000 plotpy-2.3.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:16.064306 plotpy-2.3.2/qtdesigner/
+-rw-rw-rw-   0        0        0      361 2023-11-23 17:46:00.000000 plotpy-2.3.2/qtdesigner/plotplugin.py
+-rw-rw-rw-   0        0        0      220 2024-04-10 16:39:34.000000 plotpy-2.3.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 08:01:16.126802 plotpy-2.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     3257 2023-12-22 08:06:28.000000 plotpy-2.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:01:16.126802 plotpy-2.3.2/src/
+-rw-rw-rw-   0        0        0     5676 2023-11-23 17:46:00.000000 plotpy-2.3.2/src/arrays.hpp
+-rw-rw-rw-   0        0        0  1210847 2024-05-07 08:01:11.000000 plotpy-2.3.2/src/contour2d.c
+-rw-rw-rw-   0        0        0    12546 2023-11-23 17:46:00.000000 plotpy-2.3.2/src/contour2d.pyx
+-rw-rw-rw-   0        0        0     1162 2023-11-23 17:46:00.000000 plotpy-2.3.2/src/debug.hpp
+-rw-rw-rw-   0        0        0   302415 2024-05-07 08:01:11.000000 plotpy-2.3.2/src/histogram2d.c
+-rw-rw-rw-   0        0        0     3407 2023-11-23 17:46:00.000000 plotpy-2.3.2/src/histogram2d.pyx
+-rw-rw-rw-   0        0        0   240674 2024-05-07 08:01:11.000000 plotpy-2.3.2/src/mandelbrot.c
+-rw-rw-rw-   0        0        0     1114 2023-11-23 17:46:00.000000 plotpy-2.3.2/src/mandelbrot.pyx
+-rw-rw-rw-   0        0        0    15123 2023-11-23 17:46:00.000000 plotpy-2.3.2/src/pcolor.cpp
+-rw-rw-rw-   0        0        0     7785 2023-11-23 17:46:00.000000 plotpy-2.3.2/src/points.hpp
+-rw-rw-rw-   0        0        0    26596 2023-11-23 17:46:00.000000 plotpy-2.3.2/src/scaler.cpp
+-rw-rw-rw-   0        0        0     2555 2023-11-23 17:46:00.000000 plotpy-2.3.2/src/scaler.hpp
+-rw-rw-rw-   0        0        0     4105 2023-11-23 17:46:00.000000 plotpy-2.3.2/src/traits.hpp
```

### Comparing `plotpy-2.3.1/CHANGELOG.md` & `plotpy-2.3.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # Changelog #
 
-## Version 2.3.1 ##
+## Version 2.3.2 ##
 
 In this release, test coverage is 79%.
 
+Version 2.3.2 fixes a blocking issue with the colormap editor unit test introduced
+in version 2.3.1. The latter is a fugitive release that was not announced.
+
 💥 New features / Enhancements:
 
 * Colormap: added "Apply" button to the colormap manager
 * Automated test suite:
   * Test coverage has been improved from 75% to 79%
   * The following features are now covered by unit tests:
     * Panning with the mouse move events
```

### Comparing `plotpy-2.3.1/LICENSE` & `plotpy-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/PKG-INFO` & `plotpy-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlotPy
-Version: 2.3.1
+Version: 2.3.2
 Summary: Curve and image plotting tools for Python/Qt applications
 Author-email: Codra <p.raybaut@codra.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CEA-Codra, Pierre Raybaut.
         All rights reserved.
```

### Comparing `plotpy-2.3.1/PlotPy.egg-info/PKG-INFO` & `plotpy-2.3.2/PlotPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlotPy
-Version: 2.3.1
+Version: 2.3.2
 Summary: Curve and image plotting tools for Python/Qt applications
 Author-email: Codra <p.raybaut@codra.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CEA-Codra, Pierre Raybaut.
         All rights reserved.
```

### Comparing `plotpy-2.3.1/PlotPy.egg-info/SOURCES.txt` & `plotpy-2.3.2/PlotPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/README.md` & `plotpy-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/colormaps/_cm.py` & `plotpy-2.3.2/colormaps/_cm.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/colormaps/colormap.py` & `plotpy-2.3.2/colormaps/colormap.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/colormaps/matplotlib_cmaps.py` & `plotpy-2.3.2/colormaps/matplotlib_cmaps.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/_static/favicon.ico` & `plotpy-2.3.2/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/conf.py` & `plotpy-2.3.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/dev/build.rst` & `plotpy-2.3.2/doc/dev/build.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/dev/contribute.rst` & `plotpy-2.3.2/doc/dev/contribute.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/dev/guiqwt_to_plotpy.csv` & `plotpy-2.3.2/doc/dev/guiqwt_to_plotpy.csv`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/dev/guiqwt_to_plotpy.rst` & `plotpy-2.3.2/doc/dev/guiqwt_to_plotpy.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/dev/platforms.rst` & `plotpy-2.3.2/doc/dev/platforms.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/dev/v1_to_v2.csv` & `plotpy-2.3.2/doc/dev/v1_to_v2.csv`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/dev/v1_to_v2.rst` & `plotpy-2.3.2/doc/dev/v1_to_v2.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/items/builder.rst` & `plotpy-2.3.2/doc/features/items/builder.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/items/examples.rst` & `plotpy-2.3.2/doc/features/items/examples.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/items/overview.rst` & `plotpy-2.3.2/doc/features/items/overview.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/items/reference.rst` & `plotpy-2.3.2/doc/features/items/reference.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/panels/overview.rst` & `plotpy-2.3.2/doc/features/panels/overview.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/plot/examples.rst` & `plotpy-2.3.2/doc/features/plot/examples.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/plot/index.rst` & `plotpy-2.3.2/doc/features/plot/index.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/plot/overview.rst` & `plotpy-2.3.2/doc/features/plot/overview.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/plot/reference.rst` & `plotpy-2.3.2/doc/features/plot/reference.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/signals.rst` & `plotpy-2.3.2/doc/features/signals.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/styles/overview.rst` & `plotpy-2.3.2/doc/features/styles/overview.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/styles/reference.rst` & `plotpy-2.3.2/doc/features/styles/reference.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/tools/overview.rst` & `plotpy-2.3.2/doc/features/tools/overview.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/features/tools/reference.rst` & `plotpy-2.3.2/doc/features/tools/reference.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/my_plot_manager.png` & `plotpy-2.3.2/doc/images/my_plot_manager.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/my_plot_manager.svg` & `plotpy-2.3.2/doc/images/my_plot_manager.svg`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/panorama.png` & `plotpy-2.3.2/doc/images/panorama.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/panorama.svg` & `plotpy-2.3.2/doc/images/panorama.svg`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/plot_widgets.png` & `plotpy-2.3.2/doc/images/plot_widgets.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/plot_widgets.svg` & `plotpy-2.3.2/doc/images/plot_widgets.svg`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/plotpy-banner.png` & `plotpy-2.3.2/doc/images/plotpy-banner.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/plotpy-vertical.png` & `plotpy-2.3.2/doc/images/plotpy-vertical.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/__init__.png` & `plotpy-2.3.2/doc/images/screenshots/__init__.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/computations.png` & `plotpy-2.3.2/doc/images/screenshots/computations.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/contrast.png` & `plotpy-2.3.2/doc/images/screenshots/contrast.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/cross_section.png` & `plotpy-2.3.2/doc/images/screenshots/cross_section.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/cross_section2.png` & `plotpy-2.3.2/doc/images/screenshots/cross_section2.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/dotarraydemo.png` & `plotpy-2.3.2/doc/images/screenshots/dotarraydemo.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/filtertest1.png` & `plotpy-2.3.2/doc/images/screenshots/filtertest1.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/filtertest2.png` & `plotpy-2.3.2/doc/images/screenshots/filtertest2.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/fit.png` & `plotpy-2.3.2/doc/images/screenshots/fit.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/get_point.png` & `plotpy-2.3.2/doc/images/screenshots/get_point.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/hist2d.png` & `plotpy-2.3.2/doc/images/screenshots/hist2d.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/image_plot_tools.png` & `plotpy-2.3.2/doc/images/screenshots/image_plot_tools.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/imagefilter.png` & `plotpy-2.3.2/doc/images/screenshots/imagefilter.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/imagesuperp.png` & `plotpy-2.3.2/doc/images/screenshots/imagesuperp.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/imagexy.png` & `plotpy-2.3.2/doc/images/screenshots/imagexy.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/manager.png` & `plotpy-2.3.2/doc/images/screenshots/manager.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/mandelbrot.png` & `plotpy-2.3.2/doc/images/screenshots/mandelbrot.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/pcolor.png` & `plotpy-2.3.2/doc/images/screenshots/pcolor.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/plot.png` & `plotpy-2.3.2/doc/images/screenshots/plot.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/simple_dialog.png` & `plotpy-2.3.2/doc/images/screenshots/simple_dialog.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/simple_window.png` & `plotpy-2.3.2/doc/images/screenshots/simple_window.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/images/screenshots/transform.png` & `plotpy-2.3.2/doc/images/screenshots/transform.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/index.rst` & `plotpy-2.3.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/intro/examples.rst` & `plotpy-2.3.2/doc/intro/examples.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/intro/installation.rst` & `plotpy-2.3.2/doc/intro/installation.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/intro/licenses.rst` & `plotpy-2.3.2/doc/intro/licenses.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/intro/motivation.rst` & `plotpy-2.3.2/doc/intro/motivation.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/intro/overview.rst` & `plotpy-2.3.2/doc/intro/overview.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/requirements.rst` & `plotpy-2.3.2/doc/requirements.rst`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/doc/update_requirements.py` & `plotpy-2.3.2/doc/update_requirements.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/__init__.py` & `plotpy-2.3.2/plotpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     * Python Package Index: `PyPI`_
     * Bug reports and feature requests: `GitHub`_
 
 .. _PyPI: https://pypi.python.org/pypi/plotpy
 .. _GitHub: https://github.com/PierreRaybaut/plotpy
 """
 
-__version__ = "2.3.1"
+__version__ = "2.3.2"
 __VERSION__ = tuple([int(number) for number in __version__.split(".")])
 
 # --- Important note: DATAPATH and LOCALEPATH are used by guidata.configtools
 # ---                 to retrieve data and translation files paths
 #
 # Dear (Debian, RPM, ...) package makers, please feel free to customize the
 # following path to module's data (e.g. icons) and translations:
```

### Comparing `plotpy-2.3.1/plotpy/builder/__init__.py` & `plotpy-2.3.2/plotpy/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/builder/annotation.py` & `plotpy-2.3.2/plotpy/builder/annotation.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/builder/curvemarker.py` & `plotpy-2.3.2/plotpy/builder/curvemarker.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/builder/image.py` & `plotpy-2.3.2/plotpy/builder/image.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/builder/label.py` & `plotpy-2.3.2/plotpy/builder/label.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/builder/plot.py` & `plotpy-2.3.2/plotpy/builder/plot.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/builder/shape.py` & `plotpy-2.3.2/plotpy/builder/shape.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/config.py` & `plotpy-2.3.2/plotpy/config.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/constants.py` & `plotpy-2.3.2/plotpy/constants.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/coords.py` & `plotpy-2.3.2/plotpy/coords.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/colormaps_default.json` & `plotpy-2.3.2/plotpy/data/colormaps_default.json`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/apply.png` & `plotpy-2.3.2/plotpy/data/icons/apply.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/arredit.png` & `plotpy-2.3.2/plotpy/data/icons/arredit.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/arrow_down.png` & `plotpy-2.3.2/plotpy/data/icons/arrow_down.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/arrow_up.png` & `plotpy-2.3.2/plotpy/data/icons/arrow_up.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/autorefresh.png` & `plotpy-2.3.2/plotpy/data/icons/autorefresh.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/autoscale.png` & `plotpy-2.3.2/plotpy/data/icons/autoscale.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/axes.png` & `plotpy-2.3.2/plotpy/data/icons/axes.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/copy.png` & `plotpy-2.3.2/plotpy/data/icons/copy.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/copytoclipboard.png` & `plotpy-2.3.2/plotpy/data/icons/copytoclipboard.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/csapplylut.png` & `plotpy-2.3.2/plotpy/data/icons/csapplylut.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/csection_oblique.png` & `plotpy-2.3.2/plotpy/data/icons/csection_oblique.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/curve_downsample.png` & `plotpy-2.3.2/plotpy/data/icons/curve_downsample.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/edit.png` & `plotpy-2.3.2/plotpy/data/icons/edit.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/edit_point_selection.png` & `plotpy-2.3.2/plotpy/data/icons/edit_point_selection.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/editors/edit.png` & `plotpy-2.3.2/plotpy/data/icons/editors/edit.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/editors/edit_add.png` & `plotpy-2.3.2/plotpy/data/icons/editors/edit_add.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/editors/editcopy.png` & `plotpy-2.3.2/plotpy/data/icons/editors/editcopy.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/editors/editdelete.png` & `plotpy-2.3.2/plotpy/data/icons/editors/editdelete.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/editors/editpaste.png` & `plotpy-2.3.2/plotpy/data/icons/editors/editpaste.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/editors/fileimport.png` & `plotpy-2.3.2/plotpy/data/icons/editors/fileimport.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/editors/filesave.png` & `plotpy-2.3.2/plotpy/data/icons/editors/filesave.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/editors/imshow.png` & `plotpy-2.3.2/plotpy/data/icons/editors/imshow.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/eraser.png` & `plotpy-2.3.2/plotpy/data/icons/eraser.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/exit.png` & `plotpy-2.3.2/plotpy/data/icons/exit.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/export.png` & `plotpy-2.3.2/plotpy/data/icons/export.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/fileclose.png` & `plotpy-2.3.2/plotpy/data/icons/fileclose.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/fileimport.png` & `plotpy-2.3.2/plotpy/data/icons/fileimport.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/fileopen.png` & `plotpy-2.3.2/plotpy/data/icons/fileopen.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filesave.png` & `plotpy-2.3.2/plotpy/data/icons/filesave.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filesaveas.png` & `plotpy-2.3.2/plotpy/data/icons/filesaveas.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/doc.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/doc.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/gif.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/gif.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/html.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/html.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/jpg.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/jpg.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/pdf.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/pdf.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/png.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/png.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/pps.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/pps.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/ps.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/ps.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/tar.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/tar.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/tgz.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/tgz.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/tif.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/tif.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/txt.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/txt.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/xls.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/xls.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/filetypes/zip.png` & `plotpy-2.3.2/plotpy/data/icons/filetypes/zip.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/funct.png` & `plotpy-2.3.2/plotpy/data/icons/funct.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/imagestats.png` & `plotpy-2.3.2/plotpy/data/icons/imagestats.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/items/annotation.png` & `plotpy-2.3.2/plotpy/data/icons/items/annotation.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/items/histogram2d.png` & `plotpy-2.3.2/plotpy/data/icons/items/histogram2d.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/items/image.png` & `plotpy-2.3.2/plotpy/data/icons/items/image.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/items/label.png` & `plotpy-2.3.2/plotpy/data/icons/items/label.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/magnifier.png` & `plotpy-2.3.2/plotpy/data/icons/magnifier.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/multipoint_selection.png` & `plotpy-2.3.2/plotpy/data/icons/multipoint_selection.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/plotpy-banner.svg` & `plotpy-2.3.2/plotpy/data/icons/plotpy-banner.svg`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/plotpy-vertical.svg` & `plotpy-2.3.2/plotpy/data/icons/plotpy-vertical.svg`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/plotpy.svg` & `plotpy-2.3.2/plotpy/data/icons/plotpy.svg`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/print.png` & `plotpy-2.3.2/plotpy/data/icons/print.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/python.png` & `plotpy-2.3.2/plotpy/data/icons/python.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/quickview.png` & `plotpy-2.3.2/plotpy/data/icons/quickview.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/rectangular_select.png` & `plotpy-2.3.2/plotpy/data/icons/rectangular_select.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/refresh.png` & `plotpy-2.3.2/plotpy/data/icons/refresh.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/save_all.png` & `plotpy-2.3.2/plotpy/data/icons/save_all.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/selection.png` & `plotpy-2.3.2/plotpy/data/icons/selection.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/settings.png` & `plotpy-2.3.2/plotpy/data/icons/settings.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/shapes/circle.png` & `plotpy-2.3.2/plotpy/data/icons/shapes/circle.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/shapes/contour.png` & `plotpy-2.3.2/plotpy/data/icons/shapes/contour.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/shapes/ellipse_shape.png` & `plotpy-2.3.2/plotpy/data/icons/shapes/ellipse_shape.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/shapes/oblique_rectangle.png` & `plotpy-2.3.2/plotpy/data/icons/shapes/oblique_rectangle.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/snapshot.png` & `plotpy-2.3.2/plotpy/data/icons/snapshot.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/trimage_lock.png` & `plotpy-2.3.2/plotpy/data/icons/trimage_lock.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/data/icons/trimage_unlock.png` & `plotpy-2.3.2/plotpy/data/icons/trimage_unlock.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/events.py` & `plotpy-2.3.2/plotpy/events.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/external/sliders/__init__.py` & `plotpy-2.3.2/plotpy/external/sliders/__init__.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/external/sliders/_generic_range_slider.py` & `plotpy-2.3.2/plotpy/external/sliders/_generic_range_slider.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/external/sliders/_generic_slider.py` & `plotpy-2.3.2/plotpy/external/sliders/_generic_slider.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/external/sliders/_labeled.py` & `plotpy-2.3.2/plotpy/external/sliders/_labeled.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/external/sliders/_misc.py` & `plotpy-2.3.2/plotpy/external/sliders/_misc.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/external/sliders/_range_style.py` & `plotpy-2.3.2/plotpy/external/sliders/_range_style.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/external/sliders/_sliders.py` & `plotpy-2.3.2/plotpy/external/sliders/_sliders.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/interfaces/__init__.py` & `plotpy-2.3.2/plotpy/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/interfaces/items.py` & `plotpy-2.3.2/plotpy/interfaces/items.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/interfaces/plotmanager.py` & `plotpy-2.3.2/plotpy/interfaces/plotmanager.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/io.py` & `plotpy-2.3.2/plotpy/io.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/__init__.py` & `plotpy-2.3.2/plotpy/items/__init__.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/annotation.py` & `plotpy-2.3.2/plotpy/items/annotation.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/contour.py` & `plotpy-2.3.2/plotpy/items/contour.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/curve/base.py` & `plotpy-2.3.2/plotpy/items/curve/base.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/curve/errorbar.py` & `plotpy-2.3.2/plotpy/items/curve/errorbar.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/grid.py` & `plotpy-2.3.2/plotpy/items/grid.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/histogram.py` & `plotpy-2.3.2/plotpy/items/histogram.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/image/__init__.py` & `plotpy-2.3.2/plotpy/items/image/__init__.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/image/base.py` & `plotpy-2.3.2/plotpy/items/image/base.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/image/filter.py` & `plotpy-2.3.2/plotpy/items/image/filter.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/image/image_items.py` & `plotpy-2.3.2/plotpy/items/image/image_items.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/image/masked.py` & `plotpy-2.3.2/plotpy/items/image/masked.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/image/misc.py` & `plotpy-2.3.2/plotpy/items/image/misc.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/image/transform.py` & `plotpy-2.3.2/plotpy/items/image/transform.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/label.py` & `plotpy-2.3.2/plotpy/items/label.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/polygonmap.py` & `plotpy-2.3.2/plotpy/items/polygonmap.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/shape/axis.py` & `plotpy-2.3.2/plotpy/items/shape/axis.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/shape/base.py` & `plotpy-2.3.2/plotpy/items/shape/base.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/shape/ellipse.py` & `plotpy-2.3.2/plotpy/items/shape/ellipse.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/shape/marker.py` & `plotpy-2.3.2/plotpy/items/shape/marker.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/shape/point.py` & `plotpy-2.3.2/plotpy/items/shape/point.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/shape/polygon.py` & `plotpy-2.3.2/plotpy/items/shape/polygon.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/shape/range.py` & `plotpy-2.3.2/plotpy/items/shape/range.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/shape/rectangle.py` & `plotpy-2.3.2/plotpy/items/shape/rectangle.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/shape/segment.py` & `plotpy-2.3.2/plotpy/items/shape/segment.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/items/shape/svg.py` & `plotpy-2.3.2/plotpy/items/shape/svg.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/locale/fr/LC_MESSAGES/plotpy.mo` & `plotpy-2.3.2/plotpy/locale/fr/LC_MESSAGES/plotpy.mo`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/lutrange.py` & `plotpy-2.3.2/plotpy/lutrange.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/mathutils/arrayfuncs.py` & `plotpy-2.3.2/plotpy/mathutils/arrayfuncs.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/mathutils/colormap.py` & `plotpy-2.3.2/plotpy/mathutils/colormap.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/mathutils/geometry.py` & `plotpy-2.3.2/plotpy/mathutils/geometry.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/mathutils/scaler.py` & `plotpy-2.3.2/plotpy/mathutils/scaler.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/panels/base.py` & `plotpy-2.3.2/plotpy/panels/base.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/panels/contrastadjustment.py` & `plotpy-2.3.2/plotpy/panels/contrastadjustment.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/panels/csection/csitem.py` & `plotpy-2.3.2/plotpy/panels/csection/csitem.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/panels/csection/csplot.py` & `plotpy-2.3.2/plotpy/panels/csection/csplot.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/panels/csection/cswidget.py` & `plotpy-2.3.2/plotpy/panels/csection/cswidget.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/panels/itemlist.py` & `plotpy-2.3.2/plotpy/panels/itemlist.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/plot/base.py` & `plotpy-2.3.2/plotpy/plot/base.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/plot/interactive.py` & `plotpy-2.3.2/plotpy/plot/interactive.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/plot/manager.py` & `plotpy-2.3.2/plotpy/plot/manager.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/plot/plotwidget.py` & `plotpy-2.3.2/plotpy/plot/plotwidget.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/pyplot.py` & `plotpy-2.3.2/plotpy/pyplot.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/styles/__init__.py` & `plotpy-2.3.2/plotpy/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/styles/axes.py` & `plotpy-2.3.2/plotpy/styles/axes.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/styles/base.py` & `plotpy-2.3.2/plotpy/styles/base.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/styles/curve.py` & `plotpy-2.3.2/plotpy/styles/curve.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/styles/errorbar.py` & `plotpy-2.3.2/plotpy/styles/errorbar.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/styles/histogram.py` & `plotpy-2.3.2/plotpy/styles/histogram.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/styles/image.py` & `plotpy-2.3.2/plotpy/styles/image.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/styles/label.py` & `plotpy-2.3.2/plotpy/styles/label.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/styles/polygonmap.py` & `plotpy-2.3.2/plotpy/styles/polygonmap.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/styles/shape.py` & `plotpy-2.3.2/plotpy/styles/shape.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/__init__.py` & `plotpy-2.3.2/plotpy/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/benchmarks/test_benchmarks.py` & `plotpy-2.3.2/plotpy/tests/benchmarks/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/benchmarks/test_bigimages.py` & `plotpy-2.3.2/plotpy/tests/benchmarks/test_bigimages.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/benchmarks/test_loadtest.py` & `plotpy-2.3.2/plotpy/tests/benchmarks/test_loadtest.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/data/brain.png` & `plotpy-2.3.2/plotpy/tests/data/brain.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/data/brain_cylinder.png` & `plotpy-2.3.2/plotpy/tests/data/brain_cylinder.png`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/data/mr-brain.dcm` & `plotpy-2.3.2/plotpy/tests/data/mr-brain.dcm`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/data/svg_target.svg` & `plotpy-2.3.2/plotpy/tests/data/svg_target.svg`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/data/svg_tool.svg` & `plotpy-2.3.2/plotpy/tests/data/svg_tool.svg`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/data.py` & `plotpy-2.3.2/plotpy/tests/data.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_auto_curve_image.py` & `plotpy-2.3.2/plotpy/tests/features/test_auto_curve_image.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_autoscale_shapes.py` & `plotpy-2.3.2/plotpy/tests/features/test_autoscale_shapes.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_builder.py` & `plotpy-2.3.2/plotpy/tests/features/test_builder.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_colormap_editor.py` & `plotpy-2.3.2/plotpy/tests/features/test_colormap_editor.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_colormap_manager.py` & `plotpy-2.3.2/plotpy/tests/features/test_colormap_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pytest
 import qtpy.QtCore as QC
 import qtpy.QtGui as QG
 from guidata.env import execenv
 from guidata.qthelpers import exec_dialog, qt_app_context
 
-from plotpy.mathutils.colormap import ALL_COLORMAPS, delete_cmap, get_cmap
+from plotpy.mathutils.colormap import delete_cmap, get_cmap
 from plotpy.widgets.colormap.manager import ColorMapManager
 from plotpy.widgets.colormap.widget import EditableColormap
 
 
 @pytest.fixture
 def test_cmap(cmap_name="Kinda Viridis"):
     cmap = EditableColormap(
@@ -46,16 +46,16 @@
         cmap_editor.get_colormap()
         cmap_editor.colormap_editor.update_colormap_widget()
         cmap_editor.colormap_editor.update_current_dataset()
 
         # set the colormap to last one
         with execenv.context(accept_dialogs=True):
             cmap_editor.remove_colormap()
+            result = exec_dialog(cmap_editor)
 
-        result = exec_dialog(cmap_editor)
         execenv.print("Dialog result:", result)
         cmap = cmap_editor.get_colormap()
         execenv.print("Selected colormap:", None if cmap is None else cmap.name)
         delete_cmap(test_cmap)
 
 
 if __name__ == "__main__":
```

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_computations.py` & `plotpy-2.3.2/plotpy/tests/features/test_computations.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_contrast.py` & `plotpy-2.3.2/plotpy/tests/features/test_contrast.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_cursors.py` & `plotpy-2.3.2/plotpy/tests/features/test_cursors.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_dicom_image.py` & `plotpy-2.3.2/plotpy/tests/features/test_dicom_image.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_fit.py` & `plotpy-2.3.2/plotpy/tests/features/test_fit.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_image_coords.py` & `plotpy-2.3.2/plotpy/tests/features/test_image_coords.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_imagefilter.py` & `plotpy-2.3.2/plotpy/tests/features/test_imagefilter.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_imagesuperp.py` & `plotpy-2.3.2/plotpy/tests/features/test_imagesuperp.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_loadsaveitems_hdf5.py` & `plotpy-2.3.2/plotpy/tests/features/test_loadsaveitems_hdf5.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_loadsaveitems_json.py` & `plotpy-2.3.2/plotpy/tests/features/test_loadsaveitems_json.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_loadsaveitems_pickle.py` & `plotpy-2.3.2/plotpy/tests/features/test_loadsaveitems_pickle.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_manager.py` & `plotpy-2.3.2/plotpy/tests/features/test_manager.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_no_auto_tools.py` & `plotpy-2.3.2/plotpy/tests/features/test_no_auto_tools.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_plot_log.py` & `plotpy-2.3.2/plotpy/tests/features/test_plot_log.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_plot_types.py` & `plotpy-2.3.2/plotpy/tests/features/test_plot_types.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_plot_yreverse.py` & `plotpy-2.3.2/plotpy/tests/features/test_plot_yreverse.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_pyplot.py` & `plotpy-2.3.2/plotpy/tests/features/test_pyplot.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/features/test_resize.py` & `plotpy-2.3.2/plotpy/tests/features/test_resize.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_annotations.py` & `plotpy-2.3.2/plotpy/tests/items/test_annotations.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_curves.py` & `plotpy-2.3.2/plotpy/tests/items/test_curves.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # guitest: show
 
 import numpy as np
 from guidata.qthelpers import qt_app_context
 
 from plotpy.builder import make
 from plotpy.tests import vistools as ptv
-from plotpy.tools import CurveStatsTool
 
 
 def test_plot():
     """Curve plotting test"""
     x = np.linspace(-10, 10, 200)
     dy = x / 100.0
     y = np.sin(np.sin(np.sin(x)))
```

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_curves_highdpi.py` & `plotpy-2.3.2/plotpy/tests/items/test_curves_highdpi.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_hist2d.py` & `plotpy-2.3.2/plotpy/tests/items/test_hist2d.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_histogram.py` & `plotpy-2.3.2/plotpy/tests/items/test_histogram.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_image.py` & `plotpy-2.3.2/plotpy/tests/items/test_image.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_image_contour.py` & `plotpy-2.3.2/plotpy/tests/items/test_image_contour.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_image_masked.py` & `plotpy-2.3.2/plotpy/tests/items/test_image_masked.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_image_masked_xy.py` & `plotpy-2.3.2/plotpy/tests/items/test_image_masked_xy.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_image_rgb.py` & `plotpy-2.3.2/plotpy/tests/items/test_image_rgb.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_image_xy.py` & `plotpy-2.3.2/plotpy/tests/items/test_image_xy.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_mandelbrot.py` & `plotpy-2.3.2/plotpy/tests/items/test_mandelbrot.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_pcolor.py` & `plotpy-2.3.2/plotpy/tests/items/test_pcolor.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_polygons.py` & `plotpy-2.3.2/plotpy/tests/items/test_polygons.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_svgshapes.py` & `plotpy-2.3.2/plotpy/tests/items/test_svgshapes.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/items/test_transform.py` & `plotpy-2.3.2/plotpy/tests/items/test_transform.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/tools/test_actiontool.py` & `plotpy-2.3.2/plotpy/tests/tools/test_actiontool.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/tools/test_cross_section.py` & `plotpy-2.3.2/plotpy/tests/tools/test_cross_section.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/tools/test_cross_section_line.py` & `plotpy-2.3.2/plotpy/tests/tools/test_cross_section_line.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/tools/test_cross_section_oblique.py` & `plotpy-2.3.2/plotpy/tests/tools/test_cross_section_oblique.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/tools/test_customize_shape_tool.py` & `plotpy-2.3.2/plotpy/tests/tools/test_customize_shape_tool.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/tools/test_downsample_curve.py` & `plotpy-2.3.2/plotpy/tests/tools/test_downsample_curve.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/tools/test_edit_point.py` & `plotpy-2.3.2/plotpy/tests/tools/test_edit_point.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/tools/test_get_point.py` & `plotpy-2.3.2/plotpy/tests/tools/test_get_point.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/tools/test_get_points.py` & `plotpy-2.3.2/plotpy/tests/tools/test_get_points.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/tools/test_get_rectangle.py` & `plotpy-2.3.2/plotpy/tests/tools/test_get_rectangle.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/tools/test_get_rectangle_with_svg.py` & `plotpy-2.3.2/plotpy/tests/tools/test_get_rectangle_with_svg.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/tools/test_get_segment.py` & `plotpy-2.3.2/plotpy/tests/tools/test_get_segment.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/tools/test_image_plot_tools.py` & `plotpy-2.3.2/plotpy/tests/tools/test_image_plot_tools.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_annotation_tools.py` & `plotpy-2.3.2/plotpy/tests/unit/test_annotation_tools.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_aspect_ratio_tool.py` & `plotpy-2.3.2/plotpy/tests/unit/test_aspect_ratio_tool.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_baseplot.py` & `plotpy-2.3.2/plotpy/tests/unit/test_baseplot.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_builder_annotation.py` & `plotpy-2.3.2/plotpy/tests/unit/test_builder_annotation.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_builder_curve.py` & `plotpy-2.3.2/plotpy/tests/unit/test_builder_curve.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_builder_image.py` & `plotpy-2.3.2/plotpy/tests/unit/test_builder_image.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_builder_shape.py` & `plotpy-2.3.2/plotpy/tests/unit/test_builder_shape.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_contour.py` & `plotpy-2.3.2/plotpy/tests/unit/test_contour.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_cursor_tools.py` & `plotpy-2.3.2/plotpy/tests/unit/test_cursor_tools.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_curve_tools.py` & `plotpy-2.3.2/plotpy/tests/unit/test_curve_tools.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_display_coords_tool.py` & `plotpy-2.3.2/plotpy/tests/unit/test_display_coords_tool.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_events.py` & `plotpy-2.3.2/plotpy/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_geometry.py` & `plotpy-2.3.2/plotpy/tests/unit/test_geometry.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_highprecisionxy.py` & `plotpy-2.3.2/plotpy/tests/unit/test_highprecisionxy.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_io.py` & `plotpy-2.3.2/plotpy/tests/unit/test_io.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_line.py` & `plotpy-2.3.2/plotpy/tests/unit/test_line.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_line_cross_section_tool.py` & `plotpy-2.3.2/plotpy/tests/unit/test_line_cross_section_tool.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_manipulate_selection.py` & `plotpy-2.3.2/plotpy/tests/unit/test_manipulate_selection.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_mask_tool.py` & `plotpy-2.3.2/plotpy/tests/unit/test_mask_tool.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_multiline_tools.py` & `plotpy-2.3.2/plotpy/tests/unit/test_multiline_tools.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_oblique_cross_section_tool.py` & `plotpy-2.3.2/plotpy/tests/unit/test_oblique_cross_section_tool.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_plot_curve.py` & `plotpy-2.3.2/plotpy/tests/unit/test_plot_curve.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_plot_image.py` & `plotpy-2.3.2/plotpy/tests/unit/test_plot_image.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_rect_zoom.py` & `plotpy-2.3.2/plotpy/tests/unit/test_rect_zoom.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_seg_dist.py` & `plotpy-2.3.2/plotpy/tests/unit/test_seg_dist.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_styles.py` & `plotpy-2.3.2/plotpy/tests/unit/test_styles.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/test_tools_export.py` & `plotpy-2.3.2/plotpy/tests/unit/test_tools_export.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/unit/utils.py` & `plotpy-2.3.2/plotpy/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/vistools.py` & `plotpy-2.3.2/plotpy/tests/vistools.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/widgets/test_dotarraydemo.py` & `plotpy-2.3.2/plotpy/tests/widgets/test_dotarraydemo.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/widgets/test_filtertest1.py` & `plotpy-2.3.2/plotpy/tests/widgets/test_filtertest1.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/widgets/test_filtertest2.py` & `plotpy-2.3.2/plotpy/tests/widgets/test_filtertest2.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/widgets/test_fliprotate.py` & `plotpy-2.3.2/plotpy/tests/widgets/test_fliprotate.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/widgets/test_plot_timecurve.py` & `plotpy-2.3.2/plotpy/tests/widgets/test_plot_timecurve.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/widgets/test_qtdesigner.py` & `plotpy-2.3.2/plotpy/tests/widgets/test_qtdesigner.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/widgets/test_qtdesigner.ui` & `plotpy-2.3.2/plotpy/tests/widgets/test_qtdesigner.ui`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/widgets/test_resize_dialog.py` & `plotpy-2.3.2/plotpy/tests/widgets/test_resize_dialog.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/widgets/test_rotatecrop.py` & `plotpy-2.3.2/plotpy/tests/widgets/test_rotatecrop.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/widgets/test_simple_dialog.py` & `plotpy-2.3.2/plotpy/tests/widgets/test_simple_dialog.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/widgets/test_simple_window.py` & `plotpy-2.3.2/plotpy/tests/widgets/test_simple_window.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tests/widgets/test_syncplot.py` & `plotpy-2.3.2/plotpy/tests/widgets/test_syncplot.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/__init__.py` & `plotpy-2.3.2/plotpy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/annotation.py` & `plotpy-2.3.2/plotpy/tools/annotation.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/axes.py` & `plotpy-2.3.2/plotpy/tools/axes.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/base.py` & `plotpy-2.3.2/plotpy/tools/base.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/cross_section.py` & `plotpy-2.3.2/plotpy/tools/cross_section.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/cursor.py` & `plotpy-2.3.2/plotpy/tools/cursor.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/curve.py` & `plotpy-2.3.2/plotpy/tools/curve.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/image.py` & `plotpy-2.3.2/plotpy/tools/image.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/item.py` & `plotpy-2.3.2/plotpy/tools/item.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/label.py` & `plotpy-2.3.2/plotpy/tools/label.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/misc.py` & `plotpy-2.3.2/plotpy/tools/misc.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/plot.py` & `plotpy-2.3.2/plotpy/tools/plot.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/selection.py` & `plotpy-2.3.2/plotpy/tools/selection.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/tools/shape.py` & `plotpy-2.3.2/plotpy/tools/shape.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/widgets/about.py` & `plotpy-2.3.2/plotpy/widgets/about.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/widgets/basetransform.py` & `plotpy-2.3.2/plotpy/widgets/basetransform.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/widgets/colormap/_slider.py` & `plotpy-2.3.2/plotpy/widgets/colormap/_slider.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/widgets/colormap/editor.py` & `plotpy-2.3.2/plotpy/widgets/colormap/editor.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/widgets/colormap/manager.py` & `plotpy-2.3.2/plotpy/widgets/colormap/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from copy import deepcopy
 
 import qtpy.QtCore as QC
 import qtpy.QtGui as QG
 import qtpy.QtWidgets as QW
 from guidata.configtools import get_icon
+from guidata.env import execenv
 from guidata.qthelpers import exec_dialog
 
 from plotpy.config import _
 from plotpy.mathutils.colormap import (
     ALL_COLORMAPS,
     CUSTOM_COLORMAPS,
     DEFAULT_COLORMAPS,
@@ -348,15 +349,18 @@
             QW.QMessageBox.warning(
                 self,
                 _("Remove"),
                 msg % name + "<br>" + _("Thus, this colormap cannot be removed."),
                 QW.QMessageBox.Ok,
             )
             return
-        if (
+        if execenv.unattended:  # For testing purposes only
+            if not execenv.accept_dialogs:
+                return
+        elif (
             QW.QMessageBox.question(
                 self,
                 _("Remove"),
                 _("Do you want to delete colormap <b>%s</b>?") % name,
                 QW.QMessageBox.Yes | QW.QMessageBox.No,
                 QW.QMessageBox.No,
             )
```

### Comparing `plotpy-2.3.1/plotpy/widgets/colormap/widget.py` & `plotpy-2.3.2/plotpy/widgets/colormap/widget.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/widgets/fit.py` & `plotpy-2.3.2/plotpy/widgets/fit.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/widgets/fliprotate.py` & `plotpy-2.3.2/plotpy/widgets/fliprotate.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/widgets/imagefile.py` & `plotpy-2.3.2/plotpy/widgets/imagefile.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/widgets/qtdesigner.py` & `plotpy-2.3.2/plotpy/widgets/qtdesigner.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/widgets/resizedialog.py` & `plotpy-2.3.2/plotpy/widgets/resizedialog.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/widgets/rotatecrop.py` & `plotpy-2.3.2/plotpy/widgets/rotatecrop.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/plotpy/widgets/selectdialog.py` & `plotpy-2.3.2/plotpy/widgets/selectdialog.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/pyproject.toml` & `plotpy-2.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/setup.py` & `plotpy-2.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/src/arrays.hpp` & `plotpy-2.3.2/src/arrays.hpp`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/src/contour2d.c` & `plotpy-2.3.2/src/contour2d.c`

 * *Files 1% similar despite different names*

```diff
@@ -1101,177 +1101,177 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":688
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":695
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":702
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":712
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":716
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":723
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1310,42 +1310,42 @@
 struct __pyx_obj_9contour2d_CoordGrid;
 struct __pyx_obj_9contour2d_Contour;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":727
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -9499,15 +9499,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_x, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_y, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":731
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -9516,29 +9516,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":732
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":731
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -9549,15 +9549,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -9566,29 +9566,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -9599,15 +9599,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -9616,29 +9616,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -9649,15 +9649,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -9666,29 +9666,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -9699,15 +9699,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -9716,29 +9716,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -9749,89 +9749,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":748
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":747
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":926
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -9839,33 +9839,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":927
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 928, __pyx_L1_error)
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":926
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -9873,96 +9873,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":930
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":931
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":933
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":932
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":938
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -9978,15 +9978,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -9994,53 +9994,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":940
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 940, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 942, __pyx_L5_except_error)
@@ -10048,30 +10048,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":938
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -10086,15 +10086,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":944
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10110,15 +10110,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -10126,53 +10126,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":946
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 946, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 948, __pyx_L5_except_error)
@@ -10180,30 +10180,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10218,15 +10218,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":950
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10242,15 +10242,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -10258,53 +10258,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":952
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 952, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 954, __pyx_L5_except_error)
@@ -10312,30 +10312,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10350,176 +10350,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":964
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":976
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":964
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":979
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":991
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":979
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":994
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1001
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":994
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1004
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1008
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1004
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1015
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -25746,26 +25746,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":942
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":948
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 948, __pyx_L1_error)
```

### Comparing `plotpy-2.3.1/src/contour2d.pyx` & `plotpy-2.3.2/src/contour2d.pyx`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/src/debug.hpp` & `plotpy-2.3.2/src/debug.hpp`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/src/histogram2d.c` & `plotpy-2.3.2/src/histogram2d.c`

 * *Files 3% similar despite different names*

```diff
@@ -1026,177 +1026,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":688
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":695
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":702
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":712
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":716
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":723
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1223,42 +1223,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":727
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3125,15 +3125,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_tmp.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":731
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3142,29 +3142,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":732
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":731
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3175,15 +3175,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3192,29 +3192,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3225,15 +3225,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3242,29 +3242,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3275,15 +3275,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3292,29 +3292,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3325,15 +3325,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3342,29 +3342,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3375,89 +3375,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":748
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":747
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":926
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -3465,33 +3465,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":927
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 928, __pyx_L1_error)
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":926
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -3499,96 +3499,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":930
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":931
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":933
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":932
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":938
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3604,15 +3604,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3620,53 +3620,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":940
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 940, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 942, __pyx_L5_except_error)
@@ -3674,30 +3674,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":938
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3712,15 +3712,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":944
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3736,15 +3736,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3752,53 +3752,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":946
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 946, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 948, __pyx_L5_except_error)
@@ -3806,30 +3806,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3844,15 +3844,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":950
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3868,15 +3868,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3884,53 +3884,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":952
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 952, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 954, __pyx_L5_except_error)
@@ -3938,30 +3938,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3976,176 +3976,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":964
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":976
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":964
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":979
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":991
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":979
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":994
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1001
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":994
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1004
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1008
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1004
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1015
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4244,26 +4244,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":942
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":948
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 948, __pyx_L1_error)
@@ -4647,15 +4647,15 @@
  * # Licensed under the terms of the BSD 3-Clause
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `plotpy-2.3.1/src/histogram2d.pyx` & `plotpy-2.3.2/src/histogram2d.pyx`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/src/mandelbrot.c` & `plotpy-2.3.2/src/mandelbrot.c`

 * *Files 2% similar despite different names*

```diff
@@ -989,177 +989,177 @@
 
 static const char *__pyx_f[] = {
   "src\\mandelbrot.pyx",
   "__init__.pxd",
   "type.pxd",
 };
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":688
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":689
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":695
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":696
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":702
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":703
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":712
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":713
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":716
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":721
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":723
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1186,42 +1186,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":727
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2148,15 +2148,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":731
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2165,29 +2165,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":732
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":731
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2198,15 +2198,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":734
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2215,29 +2215,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":734
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2248,15 +2248,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":737
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2265,29 +2265,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":737
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2298,15 +2298,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":740
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2315,29 +2315,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":740
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2348,15 +2348,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":743
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2365,29 +2365,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":743
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2398,89 +2398,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":746
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":748
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":747
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":746
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":926
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -2488,33 +2488,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":927
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":928
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 928, __pyx_L1_error)
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":926
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -2522,96 +2522,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":930
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":931
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":932
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":933
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":932
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":938
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2627,15 +2627,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -2643,53 +2643,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":940
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 940, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":941
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 942, __pyx_L5_except_error)
@@ -2697,30 +2697,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":939
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":938
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2735,15 +2735,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":944
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2759,15 +2759,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -2775,53 +2775,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":946
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 946, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":947
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 948, __pyx_L5_except_error)
@@ -2829,30 +2829,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":945
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":944
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2867,15 +2867,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":950
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2891,15 +2891,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -2907,53 +2907,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":952
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 952, __pyx_L3_error)
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":953
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 954, __pyx_L5_except_error)
@@ -2961,30 +2961,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":951
+    /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":950
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2999,176 +2999,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":964
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":976
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":964
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":979
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":991
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":979
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":994
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1001
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":994
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1004
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1008
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1004
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
+/* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1015
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -3258,26 +3258,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":942
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":948
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 948, __pyx_L1_error)
@@ -3627,15 +3627,15 @@
  * # Licensed under the terms of the BSD 3-Clause
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../Users/admin/AppData/Local/Temp/build-env-l4a2ars7/lib/site-packages/numpy/__init__.pxd":1011
+  /* "../../../Users/admin/AppData/Local/Temp/build-env-38yfxnkc/lib/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `plotpy-2.3.1/src/mandelbrot.pyx` & `plotpy-2.3.2/src/mandelbrot.pyx`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/src/pcolor.cpp` & `plotpy-2.3.2/src/pcolor.cpp`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/src/points.hpp` & `plotpy-2.3.2/src/points.hpp`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/src/scaler.cpp` & `plotpy-2.3.2/src/scaler.cpp`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/src/scaler.hpp` & `plotpy-2.3.2/src/scaler.hpp`

 * *Files identical despite different names*

### Comparing `plotpy-2.3.1/src/traits.hpp` & `plotpy-2.3.2/src/traits.hpp`

 * *Files identical despite different names*

