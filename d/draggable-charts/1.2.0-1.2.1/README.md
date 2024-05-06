# Comparing `tmp/draggable-charts-1.2.0.tar.gz` & `tmp/draggable-charts-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draggable-charts-1.2.0.tar", last modified: Thu May  2 20:32:31 2024, max compression
+gzip compressed data, was "draggable-charts-1.2.1.tar", last modified: Mon May  6 22:01:07 2024, max compression
```

## Comparing `draggable-charts-1.2.0.tar` & `draggable-charts-1.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.567503 draggable-charts-1.2.0/
--rw-rw-rw-   0        0        0     1057 2024-04-29 05:02:10.000000 draggable-charts-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       53 2024-04-23 23:20:49.000000 draggable-charts-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6106 2024-05-02 20:32:31.564608 draggable-charts-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5613 2024-04-24 01:12:42.000000 draggable-charts-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.419854 draggable-charts-1.2.0/draggable_charts/
--rw-rw-rw-   0        0        0       41 2024-05-02 20:31:31.000000 draggable-charts-1.2.0/draggable_charts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.390388 draggable-charts-1.2.0/draggable_charts/frontend/
-drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.466528 draggable-charts-1.2.0/draggable_charts/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-04-29 22:13:44.000000 draggable-charts-1.2.0/draggable_charts/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-04-23 23:20:49.000000 draggable-charts-1.2.0/draggable_charts/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2024-04-29 22:13:44.000000 draggable-charts-1.2.0/draggable_charts/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.393325 draggable-charts-1.2.0/draggable_charts/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.492314 draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/
--rw-rw-rw-   0        0        0   605045 2024-04-29 22:13:44.000000 draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/main.96151505.js
--rw-rw-rw-   0        0        0     1831 2024-04-29 22:13:44.000000 draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/main.96151505.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2585172 2024-04-29 22:13:44.000000 draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/main.96151505.js.map
-drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.527673 draggable-charts-1.2.0/draggable_charts/utils/
--rw-rw-rw-   0        0        0      149 2024-04-25 23:36:44.000000 draggable-charts-1.2.0/draggable_charts/utils/__init__.py
--rw-rw-rw-   0        0        0     1797 2024-04-25 23:34:16.000000 draggable-charts-1.2.0/draggable_charts/utils/callback.py
--rw-rw-rw-   0        0        0     1220 2024-04-23 23:20:49.000000 draggable-charts-1.2.0/draggable_charts/utils/component_func.py
--rw-rw-rw-   0        0        0     1816 2024-05-02 20:23:06.000000 draggable-charts-1.2.0/draggable_charts/utils/options.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.557595 draggable-charts-1.2.0/draggable_charts/widgets/
--rw-rw-rw-   0        0        0      163 2024-04-29 05:02:10.000000 draggable-charts-1.2.0/draggable_charts/widgets/__init__.py
--rw-rw-rw-   0        0        0     3757 2024-05-02 19:52:35.000000 draggable-charts-1.2.0/draggable_charts/widgets/bezierchart.py
--rw-rw-rw-   0        0        0     5258 2024-05-02 19:52:32.000000 draggable-charts-1.2.0/draggable_charts/widgets/cubicbezierchart.py
--rw-rw-rw-   0        0        0     4459 2024-05-02 16:56:46.000000 draggable-charts-1.2.0/draggable_charts/widgets/linechart.py
--rw-rw-rw-   0        0        0     2324 2024-05-02 19:52:11.000000 draggable-charts-1.2.0/draggable_charts/widgets/scatterchart.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:32:31.445246 draggable-charts-1.2.0/draggable_charts.egg-info/
--rw-rw-rw-   0        0        0     6106 2024-05-02 20:32:31.000000 draggable-charts-1.2.0/draggable_charts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      950 2024-05-02 20:32:31.000000 draggable-charts-1.2.0/draggable_charts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 20:32:31.000000 draggable-charts-1.2.0/draggable_charts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-05-02 20:32:31.000000 draggable-charts-1.2.0/draggable_charts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-02 20:32:31.000000 draggable-charts-1.2.0/draggable_charts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 20:32:31.568499 draggable-charts-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1115 2024-05-02 20:31:42.000000 draggable-charts-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:01:07.750383 draggable-charts-1.2.1/
+-rw-rw-rw-   0        0        0     1057 2024-04-29 05:02:10.000000 draggable-charts-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-04-23 23:20:49.000000 draggable-charts-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6106 2024-05-06 22:01:07.745229 draggable-charts-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5613 2024-04-24 01:12:42.000000 draggable-charts-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 22:01:07.430894 draggable-charts-1.2.1/draggable_charts/
+-rw-rw-rw-   0        0        0       41 2024-05-06 22:00:41.000000 draggable-charts-1.2.1/draggable_charts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:01:07.383090 draggable-charts-1.2.1/draggable_charts/frontend/
+drwxrwxrwx   0        0        0        0 2024-05-06 22:01:07.536610 draggable-charts-1.2.1/draggable_charts/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-04-29 22:13:44.000000 draggable-charts-1.2.1/draggable_charts/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-23 23:20:49.000000 draggable-charts-1.2.1/draggable_charts/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      492 2024-04-29 22:13:44.000000 draggable-charts-1.2.1/draggable_charts/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-05-06 22:01:07.388008 draggable-charts-1.2.1/draggable_charts/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-05-06 22:01:07.618759 draggable-charts-1.2.1/draggable_charts/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   605045 2024-04-29 22:13:44.000000 draggable-charts-1.2.1/draggable_charts/frontend/build/static/js/main.96151505.js
+-rw-rw-rw-   0        0        0     1831 2024-04-29 22:13:44.000000 draggable-charts-1.2.1/draggable_charts/frontend/build/static/js/main.96151505.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2585172 2024-04-29 22:13:44.000000 draggable-charts-1.2.1/draggable_charts/frontend/build/static/js/main.96151505.js.map
+drwxrwxrwx   0        0        0        0 2024-05-06 22:01:07.684392 draggable-charts-1.2.1/draggable_charts/utils/
+-rw-rw-rw-   0        0        0      149 2024-04-25 23:36:44.000000 draggable-charts-1.2.1/draggable_charts/utils/__init__.py
+-rw-rw-rw-   0        0        0     1797 2024-04-25 23:34:16.000000 draggable-charts-1.2.1/draggable_charts/utils/callback.py
+-rw-rw-rw-   0        0        0     1220 2024-04-23 23:20:49.000000 draggable-charts-1.2.1/draggable_charts/utils/component_func.py
+-rw-rw-rw-   0        0        0     1909 2024-05-06 16:07:13.000000 draggable-charts-1.2.1/draggable_charts/utils/options.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:01:07.735256 draggable-charts-1.2.1/draggable_charts/widgets/
+-rw-rw-rw-   0        0        0      163 2024-04-29 05:02:10.000000 draggable-charts-1.2.1/draggable_charts/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3757 2024-05-02 19:52:35.000000 draggable-charts-1.2.1/draggable_charts/widgets/bezierchart.py
+-rw-rw-rw-   0        0        0     5258 2024-05-02 19:52:32.000000 draggable-charts-1.2.1/draggable_charts/widgets/cubicbezierchart.py
+-rw-rw-rw-   0        0        0     4459 2024-05-02 16:56:46.000000 draggable-charts-1.2.1/draggable_charts/widgets/linechart.py
+-rw-rw-rw-   0        0        0     2324 2024-05-02 19:52:11.000000 draggable-charts-1.2.1/draggable_charts/widgets/scatterchart.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:01:07.481758 draggable-charts-1.2.1/draggable_charts.egg-info/
+-rw-rw-rw-   0        0        0     6106 2024-05-06 22:01:06.000000 draggable-charts-1.2.1/draggable_charts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      950 2024-05-06 22:01:07.000000 draggable-charts-1.2.1/draggable_charts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 22:01:06.000000 draggable-charts-1.2.1/draggable_charts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-05-06 22:01:06.000000 draggable-charts-1.2.1/draggable_charts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-06 22:01:07.000000 draggable-charts-1.2.1/draggable_charts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 22:01:07.752211 draggable-charts-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1115 2024-05-06 22:00:35.000000 draggable-charts-1.2.1/setup.py
```

### Comparing `draggable-charts-1.2.0/LICENSE` & `draggable-charts-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.0/PKG-INFO` & `draggable-charts-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-charts
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.
 Home-page: https://github.com/balexandermunoz/draggable-charts
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
```

### Comparing `draggable-charts-1.2.0/README.md` & `draggable-charts-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.0/draggable_charts/frontend/build/bootstrap.min.css` & `draggable-charts-1.2.1/draggable_charts/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/main.96151505.js` & `draggable-charts-1.2.1/draggable_charts/frontend/build/static/js/main.96151505.js`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/main.96151505.js.LICENSE.txt` & `draggable-charts-1.2.1/draggable_charts/frontend/build/static/js/main.96151505.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.0/draggable_charts/frontend/build/static/js/main.96151505.js.map` & `draggable-charts-1.2.1/draggable_charts/frontend/build/static/js/main.96151505.js.map`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.0/draggable_charts/utils/callback.py` & `draggable-charts-1.2.1/draggable_charts/utils/callback.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.0/draggable_charts/utils/component_func.py` & `draggable-charts-1.2.1/draggable_charts/utils/component_func.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.0/draggable_charts/utils/options.py` & `draggable-charts-1.2.1/draggable_charts/utils/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,27 @@
     "colors": [
         "#3366CC", "#DC3912", "#FF9900", "#109618", "#990099", "#3B3EAC", "#0099C6",
         "#DD4477", "#66AA00", "#B82E2E", "#316395", "#994499", "#22AA99", "#AAAA11",
         "#6633CC", "#E67300", "#8B0707", "#329262", "#5574A6", "#651067"
     ],
     "point_radius": [3],
     "fill_gaps": False,
+    "labels": {},
 }
 
 
 def set_options(data: dict, options: dict) -> dict:
     if not options:
         options = DEFAULT_OPTIONS.copy()
     options['x_type'] = _get_scale_type(data, 'x')
     options['y_type'] = _get_scale_type(data, 'y')
     options['colors'] = options.get('colors', DEFAULT_OPTIONS['colors'])
     options['point_radius'] = options.get('point_radius', DEFAULT_OPTIONS['point_radius'])
     options['fill_gaps'] = options.get('fill_gaps', DEFAULT_OPTIONS['fill_gaps'])
+    options['labels'] = options.get('labels', DEFAULT_OPTIONS['labels'])
     
     data = include_colors(data, options)
     data = include_point_radius(data, options)
     return data, options
 
 
 def include_colors(data: dict, options: dict) -> dict:
```

### Comparing `draggable-charts-1.2.0/draggable_charts/widgets/bezierchart.py` & `draggable-charts-1.2.1/draggable_charts/widgets/bezierchart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.0/draggable_charts/widgets/cubicbezierchart.py` & `draggable-charts-1.2.1/draggable_charts/widgets/cubicbezierchart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.0/draggable_charts/widgets/linechart.py` & `draggable-charts-1.2.1/draggable_charts/widgets/linechart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.0/draggable_charts/widgets/scatterchart.py` & `draggable-charts-1.2.1/draggable_charts/widgets/scatterchart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.0/draggable_charts.egg-info/PKG-INFO` & `draggable-charts-1.2.1/draggable_charts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-charts
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.
 Home-page: https://github.com/balexandermunoz/draggable-charts
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
```

### Comparing `draggable-charts-1.2.0/draggable_charts.egg-info/SOURCES.txt` & `draggable-charts-1.2.1/draggable_charts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.0/setup.py` & `draggable-charts-1.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="draggable-charts",
-    version="1.2.0",
+    version="1.2.1",
     author="Brayan Munoz",
     author_email="balexander.munoz@udea.edu.co",
     description="A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/balexandermunoz/draggable-charts",
     packages=setuptools.find_packages(),
```

