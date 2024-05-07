# Comparing `tmp/xarray_graph-0.2.2.tar.gz` & `tmp/xarray_graph-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_graph-0.2.2.tar", last modified: Mon May  6 21:13:11 2024, max compression
+gzip compressed data, was "xarray_graph-0.2.3.tar", last modified: Tue May  7 19:58:05 2024, max compression
```

## Comparing `xarray_graph-0.2.2.tar` & `xarray_graph-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-01-11 15:44:26.780358 xarray_graph-0.2.2/LICENSE
--rw-r--r--   0        0        0      238 2024-04-30 22:54:33.783557 xarray_graph-0.2.2/README.md
--rw-r--r--   0        0        0     1393 2024-05-06 21:13:11.601174 xarray_graph-0.2.2/pyproject.toml
--rw-r--r--   0        0        0   100555 2024-05-03 22:59:36.397265 xarray_graph-0.2.2/src/xarray_graph/XarrayGraph.py
--rw-r--r--   0        0        0       48 2024-01-11 15:44:26.782449 xarray_graph-0.2.2/src/xarray_graph/__init__.py
--rw-r--r--   0        0        0     2274 2024-04-30 22:51:19.174738 xarray_graph-0.2.2/src/xarray_graph/__main__.py
--rw-r--r--   0        0        0     1841 2024-04-30 14:22:30.897258 xarray_graph-0.2.2/src/xarray_graph/tmp/RegionsManager.py
--rw-r--r--   0        0        0        0 2024-01-11 15:44:26.782628 xarray_graph-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 xarray_graph-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-11 15:44:26.780358 xarray_graph-0.2.3/LICENSE
+-rw-r--r--   0        0        0      238 2024-04-30 22:54:33.783557 xarray_graph-0.2.3/README.md
+-rw-r--r--   0        0        0     1393 2024-05-07 19:58:05.303616 xarray_graph-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0   102020 2024-05-07 19:50:51.521706 xarray_graph-0.2.3/src/xarray_graph/XarrayGraph.py
+-rw-r--r--   0        0        0       48 2024-01-11 15:44:26.782449 xarray_graph-0.2.3/src/xarray_graph/__init__.py
+-rw-r--r--   0        0        0     2274 2024-04-30 22:51:19.174738 xarray_graph-0.2.3/src/xarray_graph/__main__.py
+-rw-r--r--   0        0        0     1841 2024-04-30 14:22:30.897258 xarray_graph-0.2.3/src/xarray_graph/tmp/RegionsManager.py
+-rw-r--r--   0        0        0        0 2024-01-11 15:44:26.782628 xarray_graph-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 xarray_graph-0.2.3/PKG-INFO
```

### Comparing `xarray_graph-0.2.2/LICENSE` & `xarray_graph-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray_graph-0.2.2/pyproject.toml` & `xarray_graph-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-version = "0.2.2"
+version = "0.2.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/marcel-goldschen-ohm/xarray-graph"
 repository = "https://github.com/marcel-goldschen-ohm/xarray-graph"
```

### Comparing `xarray_graph-0.2.2/src/xarray_graph/XarrayGraph.py` & `xarray_graph-0.2.3/src/xarray_graph/XarrayGraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -901,30 +901,33 @@
             item.toDict(region, dim=self.xdim)
             
             # remove the added region item and readd it so that it is added correctly as a region to all plots
             view.removeItem(item)
             item.deleteLater()
             self.add_region(region)
             
-            # stop drawing regions (draw one at a time)
-            self._set_region_drawing_mode(False)
+            # stop drawing regions (draw one at a time)?
+            if self._draw_single_region_action.isChecked():
+                self._set_region_drawing_mode(False)
 
     def _setup_ui(self) -> None:
         self._setup_menubar()
 
         self._control_panel_toolbar = QToolBar()
         self._control_panel_toolbar.setOrientation(Qt.Orientation.Vertical)
         self._control_panel_toolbar.setStyleSheet("QToolBar{spacing:2px;}")
         self._control_panel_toolbar.setIconSize(QSize(DEFAULT_ICON_SIZE, DEFAULT_ICON_SIZE))
         self._control_panel_toolbar.setMovable(False)
+        self._control_panel_toolbar.setContextMenuPolicy(Qt.ContextMenuPolicy.PreventContextMenu)
 
         self._plot_grid_toolbar = QToolBar()
         self._plot_grid_toolbar.setStyleSheet("QToolBar{spacing:2px;}")
         self._plot_grid_toolbar.setIconSize(QSize(DEFAULT_ICON_SIZE, DEFAULT_ICON_SIZE))
         self._plot_grid_toolbar.setMovable(False)
+        self._plot_grid_toolbar.setContextMenuPolicy(Qt.ContextMenuPolicy.PreventContextMenu)
         icon_button = QToolButton()
         icon_button.setIcon(qta.icon('fa5s.cubes', options=[{'opacity': 0.5}]))
         icon_button.pressed.connect(self.refresh)
         self._plot_grid_toolbar.addWidget(icon_button)
 
         self.addToolBar(Qt.ToolBarArea.TopToolBarArea, self._plot_grid_toolbar)
         self.addToolBar(Qt.ToolBarArea.LeftToolBarArea, self._control_panel_toolbar)
@@ -987,14 +990,26 @@
         self._region_button.setIcon(qta.icon('mdi.arrow-expand-horizontal', options=[{'opacity': 0.5}]))
         self._region_button.setToolTip('Draw X axis region')
         self._region_button.setCheckable(True)
         self._region_button.setChecked(False)
         self._region_button.clicked.connect(self._set_region_drawing_mode)
         self._action_after_dim_iter_things = self._plot_grid_toolbar.addWidget(self._region_button)
 
+        self._region_button_menu = QMenu()
+        self._draw_single_region_action = QAction('Draw single region', self._region_button_menu, checkable=True, checked=True)
+        self._draw_multiple_regions_action = QAction('Draw multiple regions', self._region_button_menu, checkable=True, checked=False)
+        self._region_button_menu.addAction(self._draw_single_region_action)
+        self._region_button_menu.addAction(self._draw_multiple_regions_action)
+        group = QActionGroup(self._region_button_menu)
+        group.addAction(self._draw_single_region_action)
+        group.addAction(self._draw_multiple_regions_action)
+        group.setExclusive(True)
+        self._region_button.setContextMenuPolicy(Qt.ContextMenuPolicy.CustomContextMenu)
+        self._region_button.customContextMenuRequested.connect(lambda pos: self._region_button_menu.exec_(self._region_button.mapToGlobal(pos)))
+
         self._home_button = QToolButton()
         self._home_button.setIcon(qta.icon('mdi.home-outline', options=[{'opacity': 0.5}]))
         self._home_button.setToolTip('Autoscale all plots')
         self._home_button.clicked.connect(lambda: self.autoscale_plots())
         self._plot_grid_toolbar.addWidget(self._home_button)
     
     def _setup_control_panel_toolbar(self) -> None:
@@ -1493,14 +1508,21 @@
         scroll_area = QScrollArea()
         scroll_area.setFrameShape(QFrame.NoFrame)
         scroll_area.setWidget(panel)
         scroll_area.setWidgetResizable(True)
 
         self._control_panel.addWidget(scroll_area)
     
+    # def _show_region_context_menu(self, pos: QPoint) -> None:
+    #     if not hasattr(self, '_region_button_menu'):
+    #         self._region_button_menu = QMenu()
+    #     menu = QMenu()
+    #     menu.addAction('Draw X-axis regions until unchecked', self.clear_regions)
+    #     menu.exec(self.sender().mapToGlobal(pos))
+    
     def _set_region_drawing_mode(self, draw: bool | None = None) -> None:
         if draw is None:
             draw = self._region_button.isChecked()
         self._region_button.setChecked(draw)
         
         try:
             rowmin, rowmax = self._grid_rowlim
@@ -1721,15 +1743,15 @@
         measure_type = self._measure_type_combobox.currentText()
         if measure_type in ['Mean', 'Median', 'Standard Deviation', 'Variance']:
             def existing_median(x):
                 # ensures picking an existing data point for the central value
                 i = np.argpartition(x, len(x) // 2)[len(x) // 2]
                 return x[i]
         if measure_type in ['Min', 'Max', 'AbsMax', 'Peaks']:
-            peak_width = self._peak_width_spinbox.value()
+            peak_width = self._peak_half_width_spinbox.value()
             if peak_width > 0:
                 def get_peak_index_range(mask, center_index):
                     start, stop = center_index, center_index + 1
                     for w in range(peak_width):
                         if center_index - w >= 0 and mask[center_index - w] and start == center_index - w + 1:
                             start = center_index - w
                         if center_index + w < len(mask) and mask[center_index + w] and stop == center_index + w:
@@ -2006,29 +2028,29 @@
                 except:
                     continue
                 
                 # dimensions
                 dims = yarr.dims
                 
                 # region mask for fit optimization and/or evaluation
-                if regions and (self._curve_fit_optimize_in_visible_regions_checkbox.isChecked() or self._curve_fit_evaluate_in_visible_regions_checkbox.isChecked()):
+                if regions and (self._curve_fit_optimize_in_regions_checkbox.isChecked() or self._curve_fit_evaluate_in_regions_checkbox.isChecked()):
                     # mask for combined regions
                     regions_mask = np.full(xdata.shape, False)
                     for region in regions:
                         xmin, xmax = region
                         regions_mask[(xdata >= xmin) & (xdata <= xmax)] = True
 
-                if regions and self._curve_fit_optimize_in_visible_regions_checkbox.isChecked():
+                if regions and self._curve_fit_optimize_in_regions_checkbox.isChecked():
                     xinput = xdata[regions_mask]
                     yinput = ydata[regions_mask]
                 else:
                     xinput = xdata
                     yinput = ydata
 
-                if regions and self._curve_fit_evaluate_in_visible_regions_checkbox.isChecked():
+                if regions and self._curve_fit_evaluate_in_regions_checkbox.isChecked():
                     xoutput = xdata[regions_mask]
                 else:
                     xoutput = xdata
                 
                 # fit
                 if fit_type == 'Mean':
                     youtput = np.full(len(xoutput), np.mean(yinput))
```

### Comparing `xarray_graph-0.2.2/src/xarray_graph/__main__.py` & `xarray_graph-0.2.3/src/xarray_graph/__main__.py`

 * *Files identical despite different names*

### Comparing `xarray_graph-0.2.2/src/xarray_graph/tmp/RegionsManager.py` & `xarray_graph-0.2.3/src/xarray_graph/tmp/RegionsManager.py`

 * *Files identical despite different names*

### Comparing `xarray_graph-0.2.2/PKG-INFO` & `xarray_graph-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-graph
-Version: 0.2.2
+Version: 0.2.3
 Summary: PyQt/PySide UI for graphing (x,y) slices of Xarray datasets.
 Keywords: PyQt,PySide,xarray,graph
 Home-page: https://github.com/marcel-goldschen-ohm/xarray-graph
 Author-Email: Marcel Goldschen-Ohm <goldschen-ohm@utexas.edu>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

