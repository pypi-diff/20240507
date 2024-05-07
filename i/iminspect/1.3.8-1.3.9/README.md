# Comparing `tmp/iminspect-1.3.8.tar.gz` & `tmp/iminspect-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iminspect-1.3.8.tar", last modified: Tue Nov 24 17:37:02 2020, max compression
+gzip compressed data, was "dist/iminspect-1.3.9.tar", last modified: Wed Nov 25 13:20:08 2020, max compression
```

## Comparing `iminspect-1.3.8.tar` & `iminspect-1.3.9.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-24 17:37:02.659352 iminspect-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (116)     7724 2020-11-24 17:37:02.659352 iminspect-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6164 2020-11-24 17:36:56.000000 iminspect-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-24 17:37:02.659352 iminspect-1.3.8/iminspect/
--rw-r--r--   0 runner    (1001) docker     (116)      763 2020-11-24 17:36:56.000000 iminspect-1.3.8/iminspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      452 2020-11-24 17:36:56.000000 iminspect-1.3.8/iminspect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)    24970 2020-11-24 17:36:56.000000 iminspect-1.3.8/iminspect/imgview.py
--rw-r--r--   0 runner    (1001) docker     (116)    38882 2020-11-24 17:36:56.000000 iminspect-1.3.8/iminspect/inputs.py
--rw-r--r--   0 runner    (1001) docker     (116)     4695 2020-11-24 17:36:56.000000 iminspect-1.3.8/iminspect/inspection_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    22344 2020-11-24 17:36:56.000000 iminspect-1.3.8/iminspect/inspection_widgets.py
--rw-r--r--   0 runner    (1001) docker     (116)    60526 2020-11-24 17:36:56.000000 iminspect-1.3.8/iminspect/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-24 17:37:02.659352 iminspect-1.3.8/iminspect/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-24 17:36:56.000000 iminspect-1.3.8/iminspect/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2518 2020-11-24 17:36:56.000000 iminspect-1.3.8/iminspect/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (116)       22 2020-11-24 17:36:56.000000 iminspect-1.3.8/iminspect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-24 17:37:02.659352 iminspect-1.3.8/iminspect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7724 2020-11-24 17:37:02.000000 iminspect-1.3.8/iminspect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      435 2020-11-24 17:37:02.000000 iminspect-1.3.8/iminspect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-24 17:37:02.000000 iminspect-1.3.8/iminspect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       39 2020-11-24 17:37:02.000000 iminspect-1.3.8/iminspect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2020-11-24 17:37:02.000000 iminspect-1.3.8/iminspect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-11-24 17:37:02.659352 iminspect-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1246 2020-11-24 17:36:56.000000 iminspect-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-25 13:20:08.919321 iminspect-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     8964 2020-11-25 13:20:08.919321 iminspect-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     7228 2020-11-25 13:19:58.000000 iminspect-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-25 13:20:08.919321 iminspect-1.3.9/iminspect/
+-rw-r--r--   0 runner    (1001) docker     (116)      763 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      452 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24970 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/imgview.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-25 13:20:08.919321 iminspect-1.3.9/iminspect/iminspect_assets/
+-rw-r--r--   0 runner    (1001) docker     (116)     6302 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/iminspect_assets/iminspect.svg
+-rw-r--r--   0 runner    (1001) docker     (116)    38882 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4942 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/inspection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25564 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/inspection_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (116)    65043 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-25 13:20:08.919321 iminspect-1.3.9/iminspect/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2518 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-25 13:20:08.919321 iminspect-1.3.9/iminspect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     8964 2020-11-25 13:20:08.000000 iminspect-1.3.9/iminspect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      476 2020-11-25 13:20:08.000000 iminspect-1.3.9/iminspect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-25 13:20:08.000000 iminspect-1.3.9/iminspect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       39 2020-11-25 13:20:08.000000 iminspect-1.3.9/iminspect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       10 2020-11-25 13:20:08.000000 iminspect-1.3.9/iminspect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-11-25 13:20:08.919321 iminspect-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1350 2020-11-25 13:19:58.000000 iminspect-1.3.9/setup.py
```

### Comparing `iminspect-1.3.8/PKG-INFO` & `iminspect-1.3.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: iminspect
-Version: 1.3.8
+Version: 1.3.9
 Summary: Qt-based GUI to visualize image-like data.
 Home-page: https://github.com/snototter/iminspect
 Author: snototter
 Author-email: muspellr@gmail.com
 License: UNKNOWN
 Description: # iminspect
         [![View on PyPI](https://img.shields.io/pypi/v/iminspect.svg)](https://pypi.org/project/iminspect)
         [![PyPI - Downloads](https://img.shields.io/pypi/dm/iminspect.svg)](https://pypi.org/project/iminspect)
         [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/snototter/iminspect/blob/master/LICENSE?raw=true)
         
         A python utility package for image/matrix visualization.
         
         Moving from MATLAB to python I was missing fast and easy-to-use inspection tools for image data.
-        Thus, `iminspect` provides a collection of visualization/inspection capabilities along with a Qt-based GUI.
+        Thus, `iminspect` provides a collection of visualization/inspection capabilities along with a simplistic Qt-based GUI.
         The goal is to enable quick and easy visualization/analysis of:
         * color images,
         * monochrome images (i.e. any type of 2D matrices),
         * label images (i.e. categorical data),
         * binary masks,
         * depth maps, and
         * optical flow data.
         
         
-        ## Example usage:
+        ## Example usage (within a Python script):
         ```python
         from iminspect.inspector import inspect, DataType
         import numpy as np
         
         # Show random noise image:
         inspect(np.random.rand(4096,4096) - 0.5)
         
@@ -47,14 +47,31 @@
         
         Example: visualizing a mask image<br/>
         ![Screenshot binary data](https://github.com/snototter/iminspect/blob/master/screenshots/mask.jpg?raw=true "iminspect GUI")
         
         Example: visualizing RGB image and optical flow<br/>
         ![Screenshot optical flow](https://github.com/snototter/iminspect/blob/master/screenshots/rgb-flow.jpg?raw=true "iminspect GUI")
         
+        
+        ## Example usage (standalone):
+        The `iminspect` package can be run as a standalone application, so you could create a launcher, add it to your system's binary/executable path, etc.
+        1. Set up a virtual environment (in this example, I'll use a separate `util-iminspect` folder to install the `iminspect` package):
+            ```bash
+            cd desired/installation/path
+            python3 -m venv util-iminspect
+            source util-iminspect/bin/activate
+            pip install -U pip
+            pip install iminspect
+            ```
+        2. Run `iminspect` standalone via:
+            ```bash
+            desired/installation/path/util-iminspect/bin/python3 -m iminspect
+            ```
+        
+        
         ## Custom input widgets:
         The `iminspect.inputs` subpackage provides common user input widgets, e.g. to select a rectangular region-of-interest, enter an IP address, etc. See the `examples/inputs_demo.py` application on how to use it. Exemplary screenshot:<br/>
         ![Screenshot inputs demo](https://github.com/snototter/iminspect/blob/master/screenshots/input-widgets.jpg?raw=true "Common input widgets")
         
         
         ## Dependencies
         * `numpy`, for matrix manipulation
@@ -79,17 +96,22 @@
           * `Ctrl+Shift+{Up|Down|Left|Right}` to scroll faster/further. 
           * Press and move left/right button to drag the image if zoomed in.
         * Keyboard shortcuts:
           * `Ctrl+Q` and `Ctrl+W` close the inspection GUI.
           * `Ctrl+O` shows a dialog to open another file.
           * `Ctrl+S` shows a dialog to save either the (raw) input or its current visualization.
           * `Ctrl+T` toggle tool tip display when moving the mouse over the data.
+          * `Ctrl+R` reloads the current data such that the user can select a different visualization/data type.
         
         
         ## Changelog
+        * `1.3.9`
+          * Handle non-finite values: Info/caution message shows in the data summary label, non-finite values are ignored in computing the data statistics.
+          * Option (Shortcut and toolbar button) to reload the currently inspected data with a different visualization/data type.
+          * Added application icon.
         * `1.3.8`
           * Added support for opening files via dropping them from external image viewer applications. Tested with common Linux viewers (`eog` and `geeqie`).
         * `1.3.7`
           * Support opening files by dropping them into the viewer.
           * Added `__main__` to run module (open the inspector) via `python -m iminspect`
         * `1.3.6`
           * Inspector handles 1D inputs.
```

### Comparing `iminspect-1.3.8/README.md` & `iminspect-1.3.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 [![View on PyPI](https://img.shields.io/pypi/v/iminspect.svg)](https://pypi.org/project/iminspect)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/iminspect.svg)](https://pypi.org/project/iminspect)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/snototter/iminspect/blob/master/LICENSE?raw=true)
 
 A python utility package for image/matrix visualization.
 
 Moving from MATLAB to python I was missing fast and easy-to-use inspection tools for image data.
-Thus, `iminspect` provides a collection of visualization/inspection capabilities along with a Qt-based GUI.
+Thus, `iminspect` provides a collection of visualization/inspection capabilities along with a simplistic Qt-based GUI.
 The goal is to enable quick and easy visualization/analysis of:
 * color images,
 * monochrome images (i.e. any type of 2D matrices),
 * label images (i.e. categorical data),
 * binary masks,
 * depth maps, and
 * optical flow data.
 
 
-## Example usage:
+## Example usage (within a Python script):
 ```python
 from iminspect.inspector import inspect, DataType
 import numpy as np
 
 # Show random noise image:
 inspect(np.random.rand(4096,4096) - 0.5)
 
@@ -39,14 +39,31 @@
 
 Example: visualizing a mask image<br/>
 ![Screenshot binary data](https://github.com/snototter/iminspect/blob/master/screenshots/mask.jpg?raw=true "iminspect GUI")
 
 Example: visualizing RGB image and optical flow<br/>
 ![Screenshot optical flow](https://github.com/snototter/iminspect/blob/master/screenshots/rgb-flow.jpg?raw=true "iminspect GUI")
 
+
+## Example usage (standalone):
+The `iminspect` package can be run as a standalone application, so you could create a launcher, add it to your system's binary/executable path, etc.
+1. Set up a virtual environment (in this example, I'll use a separate `util-iminspect` folder to install the `iminspect` package):
+    ```bash
+    cd desired/installation/path
+    python3 -m venv util-iminspect
+    source util-iminspect/bin/activate
+    pip install -U pip
+    pip install iminspect
+    ```
+2. Run `iminspect` standalone via:
+    ```bash
+    desired/installation/path/util-iminspect/bin/python3 -m iminspect
+    ```
+
+
 ## Custom input widgets:
 The `iminspect.inputs` subpackage provides common user input widgets, e.g. to select a rectangular region-of-interest, enter an IP address, etc. See the `examples/inputs_demo.py` application on how to use it. Exemplary screenshot:<br/>
 ![Screenshot inputs demo](https://github.com/snototter/iminspect/blob/master/screenshots/input-widgets.jpg?raw=true "Common input widgets")
 
 
 ## Dependencies
 * `numpy`, for matrix manipulation
@@ -71,17 +88,22 @@
   * `Ctrl+Shift+{Up|Down|Left|Right}` to scroll faster/further. 
   * Press and move left/right button to drag the image if zoomed in.
 * Keyboard shortcuts:
   * `Ctrl+Q` and `Ctrl+W` close the inspection GUI.
   * `Ctrl+O` shows a dialog to open another file.
   * `Ctrl+S` shows a dialog to save either the (raw) input or its current visualization.
   * `Ctrl+T` toggle tool tip display when moving the mouse over the data.
+  * `Ctrl+R` reloads the current data such that the user can select a different visualization/data type.
 
 
 ## Changelog
+* `1.3.9`
+  * Handle non-finite values: Info/caution message shows in the data summary label, non-finite values are ignored in computing the data statistics.
+  * Option (Shortcut and toolbar button) to reload the currently inspected data with a different visualization/data type.
+  * Added application icon.
 * `1.3.8`
   * Added support for opening files via dropping them from external image viewer applications. Tested with common Linux viewers (`eog` and `geeqie`).
 * `1.3.7`
   * Support opening files by dropping them into the viewer.
   * Added `__main__` to run module (open the inspector) via `python -m iminspect`
 * `1.3.6`
   * Inspector handles 1D inputs.
```

### Comparing `iminspect-1.3.8/iminspect/__init__.py` & `iminspect-1.3.9/iminspect/__init__.py`

 * *Files identical despite different names*

### Comparing `iminspect-1.3.8/iminspect/imgview.py` & `iminspect-1.3.9/iminspect/imgview.py`

 * *Files identical despite different names*

### Comparing `iminspect-1.3.8/iminspect/inputs.py` & `iminspect-1.3.9/iminspect/inputs.py`

 * *Files identical despite different names*

### Comparing `iminspect-1.3.8/iminspect/inspection_utils.py` & `iminspect-1.3.9/iminspect/inspection_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 # coding=utf-8
 import os
+import math
 import qimage2ndarray
 
 # from PyQt5.QtWidgets import QMainWindow, QApplication, QWidget, \
 #     QHBoxLayout, QVBoxLayout, QGridLayout, QPushButton, QLabel, QFrame, QToolTip, \
 #     QShortcut, QDialog, QMessageBox, QToolButton, QScrollArea
 from PyQt5.QtCore import Qt
 from PyQt5.QtGui import QPainter, QFont, QColor, QPixmap, QImage, QPen
@@ -28,14 +29,16 @@
 
 
 def fmt1f(v):
     return '{:.1f}'.format(v)
 
 
 def fmti(v):
+    if not math.isfinite(v):
+        return '?'  #TODO
     return '{:d}'.format(int(v))
 
 
 def fmtb(v):
     return 'True' if v else 'False'
 
 
@@ -97,17 +100,22 @@
     qp.setRenderHint(QPainter.HighQualityAntialiasing)
     qp.setPen(QPen(QColor(200, 0, 0)))
     font = QFont()
     font.setPointSize(20)
     font.setBold(True)
     font.setFamily('Helvetica')
     qp.setFont(font)
-    qp.drawText(qimage.rect(), Qt.AlignCenter, "No data given!")
+    qp.drawText(qimage.rect(), Qt.AlignCenter, "No data selected for inspection!")
     qp.end()
     return qimage2ndarray.rgb_view(qimage)
+    # import numpy as np
+    # npi = qimage2ndarray.rgb_view(qimage).astype(np.float32)
+    # npi[0,0,0] = np.Inf
+    # npi[10, 100, 2] = np.NaN
+    # return npi
 
 class FilenameUtils(object):
     @staticmethod
     def ensureFileExtension(filename, extensions):
         """Ensures that the given filename has one of the given extensions.
         Otherwise, the first element of extensions will be appended.
         :param filename: string
```

### Comparing `iminspect-1.3.8/iminspect/inspection_widgets.py` & `iminspect-1.3.9/iminspect/inspection_widgets.py`

 * *Files 7% similar despite different names*

```diff
@@ -421,20 +421,100 @@
 
     def getSelection(self):
         if self._confirmed:
             return (self._filename, self._save_as)
         return None
 
 
+class ChangeDataTypeDialog(QDialog):
+    def __init__(self, data_type, thumbnail, parent=None):
+        """
+        Dialog to reload/change the data type of the currently loaded data.
+
+        data_type:  None or inspector.DataType of the currently loaded data.
+        thumbnail:  None or QPixmap of the currently displayed data.
+        """
+        super(ChangeDataTypeDialog, self).__init__(parent)
+        self._data_type = data_type
+        self._confirmed = False
+        self.__prepareLayout(data_type, thumbnail)
+
+    def __prepareLayout(self, current_data_type, current_thumbnail):
+        self.setWindowTitle('Reload / Change Data Type')
+        layout = QVBoxLayout()
+        
+        self._type_widget = inputs.DropDownSelectionWidget('Type:',
+            [(inspector.DataType.COLOR, 'Color'),
+            (inspector.DataType.MONOCHROME, 'Monochrome'),
+            (inspector.DataType.BOOL, 'Boolean Mask'),
+            (inspector.DataType.CATEGORICAL, 'Categories / Labels'),
+            (inspector.DataType.DEPTH, 'Depth'),
+            (inspector.DataType.FLOW, 'Optical Flow'),
+            (inspector.DataType.MULTICHANNEL, 'Multi-channel')])
+        layout.addWidget(self._type_widget)
+
+        btn_layout = QHBoxLayout()
+        btn_cancel = QPushButton('Cancel')
+        btn_cancel.clicked.connect(self.__onCancel)
+        btn_layout.addWidget(btn_cancel)
+
+        self._btn_confirm = QPushButton('Reload Data')
+        self._btn_confirm.clicked.connect(self.__onConfirm)
+        btn_layout.addWidget(self._btn_confirm)
+
+        layout.addLayout(btn_layout)
+
+        if current_thumbnail is None:
+            self.setLayout(layout)
+        else:
+            # Show thumbnail left of input widgets, so the user knows which
+            # viewer he is going to load the file into.
+            thumb_layout = QVBoxLayout()
+            thumb_layout.addWidget(QLabel('Currently shown:'))
+            thumb_layout.addWidget(imgview.ImageLabel(current_thumbnail))
+            hlayout = QHBoxLayout()
+            hlayout.addLayout(thumb_layout)
+            hlayout.addWidget(inputs.VLine())
+            hlayout.addLayout(layout)
+            self.setLayout(hlayout)
+
+        # Pre-set data type
+        if current_data_type is not None:
+            self._type_widget.set_value(current_data_type)
+
+    def open(self):
+        super(ChangeDataTypeDialog, self).open()
+
+    @pyqtSlot()
+    def __onCancel(self):
+        self.reject()
+
+    @pyqtSlot()
+    def __onConfirm(self):
+        type_tuple = self._type_widget.get_input()
+        if type_tuple is None:
+            self._data_type = None
+        else:
+            self._data_type = type_tuple[0]
+        self._confirmed = True
+        self.accept()
+
+    def getSelection(self):
+        if self._confirmed:
+            return self._data_type
+        return None
+
+
 class ToolbarFileIOWidget(QWidget):
     """
     Provides buttons to issue open/save file requests.
     """
     fileOpenRequest = pyqtSignal()
     fileSaveRequest = pyqtSignal()
+    visualizationChangeRequest = pyqtSignal()
 
     def __init__(self, vertical=False, icon_size=QSize(20, 20), parent=None):
         """
         Shows two clickable icons to open a file and save the currently
         inspected data to disk.
         Buttons can be arranged horizontally or vertially, set the "vertical"
         flag accordingly.
@@ -459,18 +539,29 @@
         # Add "Save as..." button
         btn = QToolButton()
         btn.setIcon(QIcon.fromTheme('document-save-as'))
         btn.setIconSize(icon_size)
         btn.setToolTip('Save as... (Ctrl+S)')
         btn.clicked.connect(self.fileSaveRequest)
         layout.addWidget(btn)
+        
+        # Add "Change visualization" button
+        btn = QToolButton()
+        btn.setIcon(QIcon.fromTheme('view-refresh'))
+        btn.setIconSize(icon_size)
+        btn.setToolTip('Reload/Change visualization (Ctrl+R)')
+        btn.clicked.connect(self.visualizationChangeRequest)
+        layout.addWidget(btn)
+
+        # Align toolbar
         if vertical:
             layout.setAlignment(Qt.AlignTop)
         else:
             layout.setAlignment(Qt.AlignRight)
+
         # Important to avoid unnecessary widget margins:
         layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(layout)
 
 
 class ToolbarZoomWidget(QWidget):
     """
```

### Comparing `iminspect-1.3.8/iminspect/inspector.py` & `iminspect-1.3.9/iminspect/inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 
 # TODO Ideas and potential usability improvements:
 # * Load multiple files via drag & drop from file browser/external image viewer
 #   => requires layout reset; potential issue: variable number of inspection
 #      widgets (what's the expected behavior if there are already multple widgets
 #      open for inspection?)
 #
-# * Handle infinite and NaN values
-#   => Extend the data overview/summary label: "Contains special values: NaN, Inf" 
-#      (list only those that are actually present)
-#
 # * Add input boxes to range slider for manually typing the upper/lower limits
 #
+# * Usability Improvement:
+#   Thumbnail in "Open File"/"Reload Visualization" dialogs could be larger.
+#
 # * GUI issue:
 #   Initial window resize won't scale to the exact specified size.
 #   QApplication().instance().processEvents() doesn't help either. The widgets
 #   (e.g. image canvas) will be resized "shortly" after initializing the QMainWindow
 #   for a second time. Needs thorough investigation.
 #
 # * Usability improvement:
@@ -54,15 +53,15 @@
 import numpy as np
 import os
 from enum import Enum
 from PyQt5.QtWidgets import QMainWindow, QApplication, QWidget, \
     QHBoxLayout, QVBoxLayout, QGridLayout, QLabel, QFrame, QToolTip, \
     QShortcut, QMessageBox, QScrollArea, QSizePolicy
 from PyQt5.QtCore import Qt, QSize, QPoint, pyqtSignal, pyqtSlot
-from PyQt5.QtGui import QCursor, QFont, QKeySequence, QResizeEvent
+from PyQt5.QtGui import QCursor, QFont, QKeySequence, QResizeEvent, QIcon
 from PIL import UnidentifiedImageError
 
 from vito import imutils
 from vito import colormaps
 from vito import imvis
 from vito import flowutils
 
@@ -250,14 +249,15 @@
         # Function handle to format data values
         self.__fmt_fx = None
         # Category labels to be displayed if data is CATEGORICAL
         self._categorical_labels = None
         # Handles to file I/O dialogs
         self._save_file_dialog = None
         self._open_file_dialog = None
+        self._reload_visualization_dialog = None
         # Now, show the given data:
         self.inspectData(data, data_type, display_settings, categorical_labels)
 
     def getData(self):
         return self._data
 
     def getDataType(self):
@@ -527,31 +527,94 @@
             msg.setIcon(QMessageBox.Critical)
             msg.setText('Error loading file as type "{:s}"'.format(
                 DataType.toStr(data_type)))
             msg.setInformativeText('Logged exception:\n{:s}'.format(str(e)))
             msg.setWindowTitle('Error')
             msg.exec()
 
+    @pyqtSlot()
+    def showVisualizationChangeDialog(self):
+        self._reload_visualization_dialog = inspection_widgets.ChangeDataTypeDialog(
+            self._data_type, self._img_viewer.imagePixmap(), parent=self)
+        self._reload_visualization_dialog.finished.connect(self.__onReloadDialogFinished)
+        self._reload_visualization_dialog.open()
+
+    @pyqtSlot()
+    def __onReloadDialogFinished(self):
+        new_data_type = self._reload_visualization_dialog.getSelection()
+        if new_data_type is None:
+            return
+        if new_data_type == self._data_type:
+            print('The same data type has been selected. Reload request will be ignored.')
+            return
+        try:
+            reload_data = self._data
+            if self._data_type == DataType.BOOL:
+                if new_data_type in [DataType.COLOR, DataType.MONOCHROME]:
+                    reload_data = self._data.astype(np.uint8)
+                elif new_data_type == DataType.CATEGORICAL:
+                    reload_data = self._data.astype(np.int32)
+                elif new_data_type in [DataType.FLOW, DataType.DEPTH, DataType.MULTICHANNEL]:
+                    reload_data = self._data.astype(np.float32)
+                else:
+                    raise NotImplementedError("Reloading Boolean as '{}' is not yet supported.".format(new_data_type.toStr()))
+            self.inspectData(reload_data, new_data_type)
+            # Notify observers of loaded data
+            self.fileOpened.emit(self._inspector_id)
+        except Exception as e:
+            msg = QMessageBox()
+            msg.setIcon(QMessageBox.Critical)
+            msg.setText('Error reloading data as type "{:s}"'.format(
+                DataType.toStr(new_data_type)))
+            msg.setInformativeText('Logged exception:\n{:s}'.format(str(e)))
+            msg.setWindowTitle('Error')
+            msg.exec()
+
     def __prepareDataStatistics(self):
         """
         Analyzes the internal _data field (range, data type, channels,
         etc.) and sets member variables accordingly.
         Additionally, information will be printed to stdout and shown on
         the GUI.
         """
-        self._data_limits = [np.min(self._data[:]), np.max(self._data[:])]
+        contains_nan = np.any(np.isnan(self._data))
+        contains_inf = np.any(np.isinf(self._data))
+        if contains_nan or contains_inf:
+            # Prepare output string
+            nonfin_str = ''
+            if contains_inf:
+                nonfin_str += 'Inf'
+            if contains_nan:
+                if len(nonfin_str) > 0:
+                    nonfin_str += ', '
+                nonfin_str += 'NaN'
+            # Compute limits on finite data only
+            finite_data = self._data[np.isfinite(self._data)]
+        else:
+            finite_data = self._data
+        self._data_limits = [np.min(finite_data[:]), np.max(finite_data[:])]
+        # self._data_limits = [np.min(self._data[:]), np.max(self._data[:])]
 
+        # Prepare 'header' for stdout summary
         stdout_str = list()
         stdout_str.append('##################################################')
         stdout_str.append('Data inspection widget [{:d}]:\n'.format(self._inspector_id))
+        if contains_inf or contains_nan:
+            stdout_str.append('!! Data contains non-finite values: {}'.format(nonfin_str))
+            stdout_str.append('   These values will be ignored for the following statistics !!\n')
         stdout_str.append('Data type: {} ({})'.format(
             self._data.dtype, DataType.toStr(self._data_type)))
         stdout_str.append('Shape:     {}\n'.format(self._data.shape))
 
+        # Prepare label for GUI summary
         lbl_txt = '<table cellpadding="5">'
+        if contains_inf or contains_nan:
+            lbl_txt += '<tr><td colspan="2"><font color="red"><b>Contains non-finite values: {:s}</b></font></td></tr>'.format(
+                nonfin_str)
+            lbl_txt += '<tr><td colspan="2">Non-finite values are ignored for these statistics!</td></tr>'
         lbl_txt += '<tr><td><b>Type:</b> {} ({})</td><td><b>Shape:</b> {}</td></tr>'.format(
             self._data.dtype, DataType.toStr(self._data_type), self._data.shape)
 
         if self._data_type == DataType.BOOL:
             self._data_limits = [float(v) for v in self._data_limits]
             self.__fmt_fx = inspection_utils.fmtb
             self._colorbar.setBoolean(True)
@@ -598,35 +661,46 @@
                     len(self._data_categories))
             else:
                 stdout_str.append('Label image with {:d}/{:d} categories'.format(
                     num_present_categories, len(self._data_categories)))
                 lbl_txt += '<tr><td colspan="2"><b>Label image, {:d}/{:d} classes.</b></td></tr>'.format(
                     num_present_categories, len(self._data_categories))
         else:
-            global_mean = np.mean(self._data[:])
-            global_std = np.std(self._data[:])
+            # global_mean = np.mean(self._data[:])
+            # global_std = np.std(self._data[:])
+            global_mean = np.mean(finite_data[:])
+            global_std = np.std(finite_data[:])
             self._visualization_range_slider.set_range(0, 255)
 
             stdout_str.append('Minimum: {}'.format(self._data_limits[0]))
             stdout_str.append('Maximum: {}'.format(self._data_limits[1]))
             stdout_str.append('Mean:    {} +/- {}\n'.format(global_mean, global_std))
 
             lbl_txt += '<tr><td><b>Range:</b> [{}, {}]</td><td><b>Mean:</b> {} &#177; {}</td></tr>'.format(
                 self.__fmt_fx(self._data_limits[0]),
                 self.__fmt_fx(self._data_limits[1]),
                 self.__fmt_fx(global_mean),
                 self.__fmt_fx(global_std))
 
             if not self._is_single_channel:
                 for c in range(self._data.shape[2]):
-                    cmin = np.min(self._data[:, :, c])
-                    cmax = np.max(self._data[:, :, c])
-                    cmean = np.mean(self._data[:, :, c])
-                    cstd = np.std(self._data[:, :, c])
+                    layer_data = self._data[:, :, c]
+                    is_finite = np.isfinite(layer_data)
+                    finite_layer_data = layer_data[is_finite]
+                    # cmin = np.min(self._data[:, :, c])
+                    # cmax = np.max(self._data[:, :, c])
+                    # cmean = np.mean(self._data[:, :, c])
+                    # cstd = np.std(self._data[:, :, c])
+                    cmin = np.min(finite_layer_data)
+                    cmax = np.max(finite_layer_data)
+                    cmean = np.mean(finite_layer_data)
+                    cstd = np.std(finite_layer_data)
 
+                    if not np.all(is_finite):
+                        stdout_str.append('!! Channel {} contains non-finite values !!'.format(c))
                     stdout_str.append('Minimum on channel {}: {}'.format(c, cmin))
                     stdout_str.append('Maximum on channel {}: {}'.format(c, cmax))
                     stdout_str.append('Mean on channel {}:    {} +/- {}\n'.format(c, cmean, cstd))
 
                     lbl_txt += '<tr><td>Channel {} range: [{}, {}]</td><td>Mean: {} &#177; {}</td></tr>'.format(
                         c, self.__fmt_fx(cmin), self.__fmt_fx(cmax), self.__fmt_fx(cmean), self.__fmt_fx(cstd))
         # Print to stdout
@@ -642,14 +716,15 @@
     def __resetLayout(self):
         # Add a file I/O widget to open/save an image from this
         # inspection widget:
         file_io_widget = inspection_widgets.ToolbarFileIOWidget(
             vertical=True, icon_size=QSize(24, 24))
         file_io_widget.fileSaveRequest.connect(self.showFileSaveDialog)
         file_io_widget.fileOpenRequest.connect(self.showFileOpenDialog)
+        file_io_widget.visualizationChangeRequest.connect(self.showVisualizationChangeDialog)
 
         input_layout = QVBoxLayout()
         # Let user select a single channel if multi-channel input is provided
         if not self._is_single_channel:
             if self._data_type == DataType.FLOW and self._data.shape[2] == 2:
                 dd_options = [(-1, 'All'), (0, 'Horizontal'), (1, 'Vertical')]
             else:
@@ -881,18 +956,21 @@
         super(Inspector, self).__init__()
         self._initial_window_size = initial_window_size
         self._user_defined_window_title = window_title
         self._should_link_viewers = False
         self._display_tooltip = True
         self._open_file_dialog = None
         self._save_file_dialog = None
-        # Create the central widget (layout will be adjusted withi
+        # Create the central widget (layout will be adjusted within
         # inspectData()
         self._main_widget = QWidget()
         self.setCentralWidget(self._main_widget)
+        # Set icon
+        self.setWindowIcon(QIcon(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'iminspect_assets', 'iminspect.svg')))
+        #convert iminspect-16.png iminspect-32.png iminspect-64.png iminspect-128.png iminspect-256.png -colors 256 iminspect.ico
         # Set up keyboard shortcuts
         self.__addShortcuts()
         # Add a zoom widget (scale original, fit window, ...) to the status bar
         self._zoom_widget = inspection_widgets.ToolbarZoomWidget(self.centralWidget())
         self._zoom_widget.zoomBestFitRequest.connect(self.scaleImagesFit)
         self._zoom_widget.zoomOriginalSizeRequest.connect(self.scaleImagesOriginal)
         self.statusBar().addPermanentWidget(self._zoom_widget)
@@ -1022,14 +1100,17 @@
     def __addShortcuts(self):
         # Open file
         shortcut_open = QShortcut(QKeySequence('Ctrl+O'), self)
         shortcut_open.activated.connect(self.__onOpenShortcut)
         # Save file
         shortcut_save = QShortcut(QKeySequence('Ctrl+S'), self)
         shortcut_save.activated.connect(self.__onSaveShortcut)
+        # Reload/change visualization
+        shortcut_reload = QShortcut(QKeySequence('Ctrl+R'), self)
+        shortcut_reload.activated.connect(self.__onReloadShortcut)
         # Close window
         shortcut_exit_q = QShortcut(QKeySequence('Ctrl+Q'), self)
         shortcut_exit_q.activated.connect(QApplication.instance().quit)
         shortcut_exit_w = QShortcut(QKeySequence('Ctrl+W'), self)
         shortcut_exit_w.activated.connect(QApplication.instance().quit)
         # Zooming
         shortcut_zoom_in = QShortcut(QKeySequence('Ctrl++'), self)
@@ -1187,14 +1268,19 @@
         inspector_id = self.__getActiveInspector()
         self._inspectors[inspector_id].showFileOpenDialog()
 
     @pyqtSlot()
     def __onSaveShortcut(self):
         inspector_id = self.__getActiveInspector()
         self._inspectors[inspector_id].showFileSaveDialog()
+    
+    @pyqtSlot()
+    def __onReloadShortcut(self):
+        inspector_id = self.__getActiveInspector()
+        self._inspectors[inspector_id].showVisualizationChangeDialog()
 
 
 def inspect(
         data,
         data_type=None,
         flip_channels=False,
         label=None,
```

### Comparing `iminspect-1.3.8/iminspect/tests/test_inspector.py` & `iminspect-1.3.9/iminspect/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `iminspect-1.3.8/iminspect.egg-info/PKG-INFO` & `iminspect-1.3.9/iminspect.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: iminspect
-Version: 1.3.8
+Version: 1.3.9
 Summary: Qt-based GUI to visualize image-like data.
 Home-page: https://github.com/snototter/iminspect
 Author: snototter
 Author-email: muspellr@gmail.com
 License: UNKNOWN
 Description: # iminspect
         [![View on PyPI](https://img.shields.io/pypi/v/iminspect.svg)](https://pypi.org/project/iminspect)
         [![PyPI - Downloads](https://img.shields.io/pypi/dm/iminspect.svg)](https://pypi.org/project/iminspect)
         [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/snototter/iminspect/blob/master/LICENSE?raw=true)
         
         A python utility package for image/matrix visualization.
         
         Moving from MATLAB to python I was missing fast and easy-to-use inspection tools for image data.
-        Thus, `iminspect` provides a collection of visualization/inspection capabilities along with a Qt-based GUI.
+        Thus, `iminspect` provides a collection of visualization/inspection capabilities along with a simplistic Qt-based GUI.
         The goal is to enable quick and easy visualization/analysis of:
         * color images,
         * monochrome images (i.e. any type of 2D matrices),
         * label images (i.e. categorical data),
         * binary masks,
         * depth maps, and
         * optical flow data.
         
         
-        ## Example usage:
+        ## Example usage (within a Python script):
         ```python
         from iminspect.inspector import inspect, DataType
         import numpy as np
         
         # Show random noise image:
         inspect(np.random.rand(4096,4096) - 0.5)
         
@@ -47,14 +47,31 @@
         
         Example: visualizing a mask image<br/>
         ![Screenshot binary data](https://github.com/snototter/iminspect/blob/master/screenshots/mask.jpg?raw=true "iminspect GUI")
         
         Example: visualizing RGB image and optical flow<br/>
         ![Screenshot optical flow](https://github.com/snototter/iminspect/blob/master/screenshots/rgb-flow.jpg?raw=true "iminspect GUI")
         
+        
+        ## Example usage (standalone):
+        The `iminspect` package can be run as a standalone application, so you could create a launcher, add it to your system's binary/executable path, etc.
+        1. Set up a virtual environment (in this example, I'll use a separate `util-iminspect` folder to install the `iminspect` package):
+            ```bash
+            cd desired/installation/path
+            python3 -m venv util-iminspect
+            source util-iminspect/bin/activate
+            pip install -U pip
+            pip install iminspect
+            ```
+        2. Run `iminspect` standalone via:
+            ```bash
+            desired/installation/path/util-iminspect/bin/python3 -m iminspect
+            ```
+        
+        
         ## Custom input widgets:
         The `iminspect.inputs` subpackage provides common user input widgets, e.g. to select a rectangular region-of-interest, enter an IP address, etc. See the `examples/inputs_demo.py` application on how to use it. Exemplary screenshot:<br/>
         ![Screenshot inputs demo](https://github.com/snototter/iminspect/blob/master/screenshots/input-widgets.jpg?raw=true "Common input widgets")
         
         
         ## Dependencies
         * `numpy`, for matrix manipulation
@@ -79,17 +96,22 @@
           * `Ctrl+Shift+{Up|Down|Left|Right}` to scroll faster/further. 
           * Press and move left/right button to drag the image if zoomed in.
         * Keyboard shortcuts:
           * `Ctrl+Q` and `Ctrl+W` close the inspection GUI.
           * `Ctrl+O` shows a dialog to open another file.
           * `Ctrl+S` shows a dialog to save either the (raw) input or its current visualization.
           * `Ctrl+T` toggle tool tip display when moving the mouse over the data.
+          * `Ctrl+R` reloads the current data such that the user can select a different visualization/data type.
         
         
         ## Changelog
+        * `1.3.9`
+          * Handle non-finite values: Info/caution message shows in the data summary label, non-finite values are ignored in computing the data statistics.
+          * Option (Shortcut and toolbar button) to reload the currently inspected data with a different visualization/data type.
+          * Added application icon.
         * `1.3.8`
           * Added support for opening files via dropping them from external image viewer applications. Tested with common Linux viewers (`eog` and `geeqie`).
         * `1.3.7`
           * Support opening files by dropping them into the viewer.
           * Added `__main__` to run module (open the inspector) via `python -m iminspect`
         * `1.3.6`
           * Inspector handles 1D inputs.
```

### Comparing `iminspect-1.3.8/setup.py` & `iminspect-1.3.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,9 +39,11 @@
         'qimage2ndarray',
         'vito>=1.1.4'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    package_dir={'iminspect': 'iminspect'},
+    package_data={'iminspect': ['iminspect_assets/*.svg']},
     python_requires='>=3.5',
 )
```

