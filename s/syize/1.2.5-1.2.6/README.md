# Comparing `tmp/syize-1.2.5.tar.gz` & `tmp/syize-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syize-1.2.5.tar", last modified: Fri Sep  8 07:10:09 2023, max compression
+gzip compressed data, was "syize-1.2.6.tar", last modified: Tue May  7 07:28:34 2024, max compression
```

## Comparing `syize-1.2.5.tar` & `syize-1.2.6.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 syize     (1000) syize     (1000)        0 2023-09-08 07:10:09.259246 syize-1.2.5/
--rw-r--r--   0 syize     (1000) syize     (1000)     2028 2023-09-08 07:10:09.259246 syize-1.2.5/PKG-INFO
--rw-r--r--   0 syize     (1000) syize     (1000)     1602 2023-09-08 07:00:05.000000 syize-1.2.5/README-pypi.md
--rw-r--r--   0 syize     (1000) syize     (1000)     4207 2023-09-08 07:05:55.000000 syize-1.2.5/README.md
--rw-r--r--   0 syize     (1000) syize     (1000)      583 2023-09-08 07:03:27.000000 syize-1.2.5/pyproject.toml
--rw-r--r--   0 syize     (1000) syize     (1000)      475 2023-09-08 07:10:09.259246 syize-1.2.5/setup.cfg
-drwxr-xr-x   0 syize     (1000) syize     (1000)        0 2023-09-08 07:10:09.255913 syize-1.2.5/syize/
--rw-r--r--   0 syize     (1000) syize     (1000)       53 2023-06-29 08:53:53.000000 syize-1.2.5/syize/__init__.py
--rw-r--r--   0 syize     (1000) syize     (1000)      974 2023-06-26 05:19:53.000000 syize-1.2.5/syize/diff.py
--rw-r--r--   0 syize     (1000) syize     (1000)     2299 2023-09-07 08:46:16.000000 syize-1.2.5/syize/diff_run.py
--rw-r--r--   0 syize     (1000) syize     (1000)     1394 2023-06-08 11:40:39.000000 syize-1.2.5/syize/picture.py
--rw-r--r--   0 syize     (1000) syize     (1000)     3014 2023-06-08 11:38:49.000000 syize-1.2.5/syize/picture_run.py
--rw-r--r--   0 syize     (1000) syize     (1000)     6113 2023-09-07 07:38:07.000000 syize-1.2.5/syize/plot.py
--rw-r--r--   0 syize     (1000) syize     (1000)      626 2023-06-08 06:22:07.000000 syize-1.2.5/syize/string.py
--rw-r--r--   0 syize     (1000) syize     (1000)     1780 2023-06-08 06:05:03.000000 syize-1.2.5/syize/string_run.py
--rw-r--r--   0 syize     (1000) syize     (1000)      195 2023-09-07 09:03:06.000000 syize-1.2.5/syize/utils.py
-drwxr-xr-x   0 syize     (1000) syize     (1000)        0 2023-09-08 07:10:09.259246 syize-1.2.5/syize.egg-info/
--rw-r--r--   0 syize     (1000) syize     (1000)     2028 2023-09-08 07:10:09.000000 syize-1.2.5/syize.egg-info/PKG-INFO
--rw-r--r--   0 syize     (1000) syize     (1000)      385 2023-09-08 07:10:09.000000 syize-1.2.5/syize.egg-info/SOURCES.txt
--rw-r--r--   0 syize     (1000) syize     (1000)        1 2023-09-08 07:10:09.000000 syize-1.2.5/syize.egg-info/dependency_links.txt
--rw-r--r--   0 syize     (1000) syize     (1000)      108 2023-09-08 07:10:09.000000 syize-1.2.5/syize.egg-info/entry_points.txt
--rw-r--r--   0 syize     (1000) syize     (1000)       70 2023-09-08 07:10:09.000000 syize-1.2.5/syize.egg-info/requires.txt
--rw-r--r--   0 syize     (1000) syize     (1000)        6 2023-09-08 07:10:09.000000 syize-1.2.5/syize.egg-info/top_level.txt
+drwxr-xr-x   0 syize     (1000) syize     (1000)        0 2024-05-07 07:28:34.913080 syize-1.2.6/
+-rw-r--r--   0 syize     (1000) syize     (1000)      300 2024-05-07 07:28:34.913080 syize-1.2.6/PKG-INFO
+-rw-r--r--   0 syize     (1000) syize     (1000)      186 2024-05-07 07:28:04.000000 syize-1.2.6/README.md
+-rw-r--r--   0 syize     (1000) syize     (1000)      470 2024-05-07 07:28:04.000000 syize-1.2.6/pyproject.toml
+-rw-r--r--   0 syize     (1000) syize     (1000)      467 2024-05-07 07:28:34.913080 syize-1.2.6/setup.cfg
+drwxr-xr-x   0 syize     (1000) syize     (1000)        0 2024-05-07 07:28:34.913080 syize-1.2.6/syize/
+-rw-r--r--   0 syize     (1000) syize     (1000)       53 2024-05-07 07:28:04.000000 syize-1.2.6/syize/__init__.py
+-rw-r--r--   0 syize     (1000) syize     (1000)      974 2024-05-07 07:28:04.000000 syize-1.2.6/syize/diff.py
+-rw-r--r--   0 syize     (1000) syize     (1000)     2325 2024-05-07 07:28:04.000000 syize-1.2.6/syize/diff_run.py
+-rw-r--r--   0 syize     (1000) syize     (1000)     1394 2024-05-07 07:28:04.000000 syize-1.2.6/syize/picture.py
+-rw-r--r--   0 syize     (1000) syize     (1000)     3014 2024-05-07 07:28:04.000000 syize-1.2.6/syize/picture_run.py
+-rw-r--r--   0 syize     (1000) syize     (1000)     5086 2024-05-07 07:28:04.000000 syize-1.2.6/syize/plot.py
+-rw-r--r--   0 syize     (1000) syize     (1000)      626 2024-05-07 07:28:04.000000 syize-1.2.6/syize/string.py
+-rw-r--r--   0 syize     (1000) syize     (1000)     1780 2024-05-07 07:28:04.000000 syize-1.2.6/syize/string_run.py
+-rw-r--r--   0 syize     (1000) syize     (1000)      195 2024-05-07 07:28:04.000000 syize-1.2.6/syize/utils.py
+drwxr-xr-x   0 syize     (1000) syize     (1000)        0 2024-05-07 07:28:34.913080 syize-1.2.6/syize.egg-info/
+-rw-r--r--   0 syize     (1000) syize     (1000)      300 2024-05-07 07:28:34.000000 syize-1.2.6/syize.egg-info/PKG-INFO
+-rw-r--r--   0 syize     (1000) syize     (1000)      363 2024-05-07 07:28:34.000000 syize-1.2.6/syize.egg-info/SOURCES.txt
+-rw-r--r--   0 syize     (1000) syize     (1000)        1 2024-05-07 07:28:34.000000 syize-1.2.6/syize.egg-info/dependency_links.txt
+-rw-r--r--   0 syize     (1000) syize     (1000)      108 2024-05-07 07:28:34.000000 syize-1.2.6/syize.egg-info/entry_points.txt
+-rw-r--r--   0 syize     (1000) syize     (1000)       63 2024-05-07 07:28:34.000000 syize-1.2.6/syize.egg-info/requires.txt
+-rw-r--r--   0 syize     (1000) syize     (1000)        6 2024-05-07 07:28:34.000000 syize-1.2.6/syize.egg-info/top_level.txt
```

### Comparing `syize-1.2.5/syize/diff.py` & `syize-1.2.6/syize/diff.py`

 * *Files identical despite different names*

### Comparing `syize-1.2.5/syize/diff_run.py` & `syize-1.2.6/syize/diff_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from rich import print as rprint
 from os import listdir
+from os.path import isdir
 from getopt import getopt, GetoptError
 from sys import exit, argv
 from syize.diff import diff
 
 
 def help():
     print("Usage for pydiff:\n"
```

### Comparing `syize-1.2.5/syize/picture.py` & `syize-1.2.6/syize/picture.py`

 * *Files identical despite different names*

### Comparing `syize-1.2.5/syize/picture_run.py` & `syize-1.2.6/syize/picture_run.py`

 * *Files identical despite different names*

### Comparing `syize-1.2.5/syize/plot.py` & `syize-1.2.6/syize/plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,98 +2,112 @@
 
 from cartopy.mpl.geoaxes import GeoAxes
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.transforms import Bbox
 from haversine import inverse_haversine
 import numpy as np
-import cartopy.crs as ccrs
-from cnmaps import get_adm_maps, draw_maps
 
 
 class OnResize:
     """
     listen on figure resize event and change colorbar position and size dynamically
     """
-    def __init__(self, ax: Union[GeoAxes, Axes, tuple[float, ...]], cax: Axes):
+    def __init__(self, ax: Union[GeoAxes, Axes, tuple[GeoAxes, GeoAxes], tuple[Axes, Axes]], cax: Axes):
         self.ax = ax
         self.cax = cax
+
         # get position to calculate width and vertical
         if isinstance(ax, tuple):
-            ax_position = ax
+            ax_position = (ax[0].get_position().x0, ax[0].get_position().y0, ax[1].get_position().x1, ax[1].get_position().y1)
         else:
             ax_position = (ax.get_position().x0, ax.get_position().y0, ax.get_position().x1, ax.get_position().y1)
         cax_position = (cax.get_position().x0, cax.get_position().y0, cax.get_position().x1, cax.get_position().y1)
+
         # check if is vertical
         diff_x = cax_position[2] - cax_position[0]
         diff_y = cax_position[3] - cax_position[1]
+
         if diff_x > diff_y:
             self.vertical = False
             self.width = diff_y
         else:
             self.vertical = True
             self.width = diff_x
+
         # get padding
         if self.vertical:
             self.padding = cax_position[0] - ax_position[2]
         else:
             self.padding = ax_position[1] - cax_position[3]
 
     def __call__(self, event):
-        ax_position = self.ax.get_position()
-        x0, y0, x1, y1 = ax_position.x0, ax_position.y0, ax_position.x1, ax_position.y1
+        # get ax new position so we can change cax's position
+        if isinstance(self.ax, tuple):
+            x0, y0, x1, y1 = self.ax[0].get_position().x0, self.ax[0].get_position().y0, self.ax[1].get_position().x1, self.ax[1].get_position().y1
+        else:
+            ax_position = self.ax.get_position()
+            x0, y0, x1, y1 = ax_position.x0, ax_position.y0, ax_position.x1, ax_position.y1
+
         if not self.vertical:
             cax1_position = Bbox.from_extents(
                 x0, y0 - self.padding - self.width,
                 x1, y0 - self.padding
             )
         else:
             cax1_position = Bbox.from_extents(
                 x1 + self.padding, y0,
                 x1 + self.padding + self.width, y1
             )
 
         self.cax.set_position(cax1_position)
 
 
-def prepare_colorbar(fig: Figure, ax: Union[GeoAxes, Axes] = None, vertical=False, pad=0.09, width=0.02,
-                     position: Union[tuple[float, float, float, float], list[float, float, float, float]] = None)\
-         -> Axes:
-    """
-    add cax to fig
-    :param position: x0, y0, x1, y1. If ax is not None, use ax.get_position() instead
-    :param width: colorbar width.
-    :param pad: width between colorbar and axes
-    :param vertical: if colorbar is vertical or horizontal
-    :param fig: figure
-    :param ax: Axes or GeoAxes
-    :return: colorbar axes
+def prepare_colorbar(fig: Figure, ax: Union[GeoAxes, Axes, tuple[GeoAxes, GeoAxes], tuple[Axes, Axes]] = None,
+                     vertical=False, pad=0.09, width=0.02,
+                     position: Union[tuple[float, float, float, float], list[float, float, float, float]] = None) -> Axes:
+    """
+    Add cax to fig.
+    :param fig: Matplotlib Figure object.
+    :param ax: A single or two Axes(GeoAxes).
+               For single Axes(GeoAxes), will add cax to the ax.
+               For two Axes(GeoAxes), which should be the left-bottom and right-top ax of an ax group, will add cax to the ax group.
+    :param vertical: If the cax is vertical.
+    :param pad: The distance length between cax and ax (group).
+    :param width: The width of the cax.
+    :param position: A tuple (x0, y0, x1, y1) to set ax (group) area. This param won't be used if `ax` isn't None.
+    :return:
     """
+    # get position to add cax
     if ax is not None:
-        ax_position: Bbox = ax.get_position()
-        x0, y0, x1, y1 = ax_position.x0, ax_position.y0, ax_position.x1, ax_position.y1
+        if isinstance(ax, tuple):
+            x0, y0 = ax[0].get_position().x0, ax[0].get_position().y0
+            x1, y1 = ax[1].get_position().x1, ax[1].get_position().y1
+        else:
+            x0, y0, x1, y1 = ax.get_position().x0, ax.get_position().y0, ax.get_position().x1, ax.get_position().y1
     elif position is not None:
         x0, y0, x1, y1 = position
     else:
         raise Exception('ax and position can\'t be None at the same time!')
-    # y0 = ax_position.y0 - 0.01
-    # y1 = ax_position.y1 - 0.03
-    pad = pad
-    width = width
+    
+    # add cax
     if not vertical:
         cax1_position = Bbox.from_extents(
             x0, y0 - pad - width,
             x1, y0 - pad
         )
     else:
         cax1_position = Bbox.from_extents(
             x1 + pad, y0,
             x1 + pad + width, y1
         )
+        
     cax = fig.add_axes(cax1_position)
+    
+    # add callback to make cax change size automatically
     if ax is not None:
         fig.canvas.mpl_connect("resize_event", OnResize(ax, cax))
     else:
         fig.canvas.mpl_connect("resize_event", OnResize(position, cax))
     return cax
 
 
@@ -109,62 +123,8 @@
     lon1 = inverse_haversine(radar_position, distance, np.pi * 1.5)[1]
     lon2 = inverse_haversine(radar_position, distance, np.pi * 0.5)[1]
     lat1 = inverse_haversine(radar_position, distance, np.pi * 1)[0]
     lat2 = inverse_haversine(radar_position, distance, np.pi * 0)[0]
     return (lon1, lon2), (lat1, lat2)
 
 
-def add_map_to_axes(fig: Figure, ax: Axes, lon: Union[tuple, list], lat: Union[tuple, list], zorder='top',
-                    map_level: str = None, province: str = None, city: str = None) -> GeoAxes:
-    """
-    add map to radar plot
-    :param city: City name to plot
-    :param province: Province name to plot
-    :param map_level: cnmaps' level
-    :param lat: latitude range, [-90, 90]
-    :param lon: longitude range, [-180, 180]
-    :param zorder: where map line plot. `top` means map plot on the original axes. `bottom` means under the original axes.
-    :param fig:
-    :param ax: original axes
-    :return:
-    """
-    # get original axes position
-    x0 = ax.get_position().x0
-    y0 = ax.get_position().y0
-    x1 = ax.get_position().x1
-    y1 = ax.get_position().y1
-    proj = ccrs.PlateCarree()
-    # add another axes
-    ax2: GeoAxes = fig.add_axes((x0, y0, x1 - x0, y1 - y0), projection=proj)
-    if zorder == 'top':
-        ax.set_zorder(0)
-        ax2.set_zorder(1)
-        ax2.patch.set_alpha(0)
-    elif zorder == 'bottom':
-        ax2.set_zorder(0)
-        ax.set_zorder(1)
-        ax.patch.set_alpha(0)
-    else:
-        raise Exception('zorder should be `top` or `bottom`, but {}'.format(zorder))
-    ax2.axis('off')
-    # plot map
-    draw_maps(get_adm_maps(level=map_level, province=province, city=city), color='black', ax=ax2)
-    diff_lat = lat[1] - lat[0]
-    diff_lon = lon[1] - lon[0]
-    if diff_lat > diff_lon:
-        diff_lon = (diff_lat - diff_lon) / 2
-        lon1 = lon[0] - diff_lon
-        lon2 = lon[1] + diff_lon
-        lat1 = lat[0]
-        lat2 = lat[1]
-    else:
-        diff_lat = - (diff_lat - diff_lon) / 2
-        lat1 = lat[0] - diff_lat
-        lat2 = lat[1] + diff_lat
-        lon1 = lon[0]
-        lon2 = lon[1]
-    ax2.set_xlim(lon1, lon2)
-    ax2.set_ylim(lat1, lat2)
-    return ax2
-
-
-__all__ = ['prepare_colorbar', 'get_lon_lat_range', 'add_map_to_axes']
+__all__ = ['prepare_colorbar', 'get_lon_lat_range']
```

### Comparing `syize-1.2.5/syize/string.py` & `syize-1.2.6/syize/string.py`

 * *Files identical despite different names*

### Comparing `syize-1.2.5/syize/string_run.py` & `syize-1.2.6/syize/string_run.py`

 * *Files identical despite different names*

