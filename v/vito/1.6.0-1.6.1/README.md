# Comparing `tmp/vito-1.6.0.tar.gz` & `tmp/vito-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vito-1.6.0.tar", last modified: Thu Jul  7 22:32:00 2022, max compression
+gzip compressed data, was "vito-1.6.1.tar", last modified: Tue May  7 21:45:24 2024, max compression
```

## Comparing `vito-1.6.0.tar` & `vito-1.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 22:32:00.749644 vito-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-07-07 22:31:51.000000 vito-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8756 2022-07-07 22:32:00.749644 vito-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8256 2022-07-07 22:31:51.000000 vito-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-07 22:32:00.749644 vito-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-07-07 22:31:51.000000 vito-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 22:32:00.745644 vito-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-07 22:31:51.000000 vito-1.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8034 2022-07-07 22:31:51.000000 vito-1.6.0/tests/test_cam_projections.py
--rw-r--r--   0 runner    (1001) docker     (121)     7113 2022-07-07 22:31:51.000000 vito-1.6.0/tests/test_detection2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     3490 2022-07-07 22:31:51.000000 vito-1.6.0/tests/test_flowutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    23768 2022-07-07 22:31:51.000000 vito-1.6.0/tests/test_imutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10280 2022-07-07 22:31:51.000000 vito-1.6.0/tests/test_imvis.py
--rw-r--r--   0 runner    (1001) docker     (121)     5569 2022-07-07 22:31:51.000000 vito-1.6.0/tests/test_pyutils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 22:32:00.749644 vito-1.6.0/vito/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-07-07 22:31:51.000000 vito-1.6.0/vito/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13379 2022-07-07 22:31:51.000000 vito-1.6.0/vito/cam_projections.py
--rw-r--r--   0 runner    (1001) docker     (121)    78408 2022-07-07 22:31:51.000000 vito-1.6.0/vito/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (121)    11055 2022-07-07 22:31:51.000000 vito-1.6.0/vito/detection2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     4545 2022-07-07 22:31:51.000000 vito-1.6.0/vito/flowutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    15602 2022-07-07 22:31:51.000000 vito-1.6.0/vito/imutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8715 2022-07-07 22:31:51.000000 vito-1.6.0/vito/imvis.py
--rw-r--r--   0 runner    (1001) docker     (121)     8047 2022-07-07 22:31:51.000000 vito-1.6.0/vito/pyutils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-07 22:31:51.000000 vito-1.6.0/vito/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 22:32:00.749644 vito-1.6.0/vito.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8756 2022-07-07 22:32:00.000000 vito-1.6.0/vito.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-07-07 22:32:00.000000 vito-1.6.0/vito.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-07 22:32:00.000000 vito-1.6.0/vito.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-07 22:32:00.000000 vito-1.6.0/vito.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-07-07 22:32:00.000000 vito-1.6.0/vito.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:45:24.380648 vito-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 21:45:20.000000 vito-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-05-07 21:45:24.380648 vito-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-07 21:45:20.000000 vito-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 21:45:24.380648 vito-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-07 21:45:20.000000 vito-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:45:24.376648 vito-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:45:20.000000 vito-1.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8034 2024-05-07 21:45:20.000000 vito-1.6.1/tests/test_cam_projections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-05-07 21:45:20.000000 vito-1.6.1/tests/test_detection2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-07 21:45:20.000000 vito-1.6.1/tests/test_flowutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23701 2024-05-07 21:45:20.000000 vito-1.6.1/tests/test_imutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-07 21:45:20.000000 vito-1.6.1/tests/test_imvis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-07 21:45:20.000000 vito-1.6.1/tests/test_pyutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:45:24.376648 vito-1.6.1/vito/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-07 21:45:20.000000 vito-1.6.1/vito/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-05-07 21:45:20.000000 vito-1.6.1/vito/cam_projections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78422 2024-05-07 21:45:20.000000 vito-1.6.1/vito/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-05-07 21:45:20.000000 vito-1.6.1/vito/detection2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-07 21:45:20.000000 vito-1.6.1/vito/flowutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15807 2024-05-07 21:45:20.000000 vito-1.6.1/vito/imutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-05-07 21:45:20.000000 vito-1.6.1/vito/imvis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-07 21:45:20.000000 vito-1.6.1/vito/pyutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 21:45:20.000000 vito-1.6.1/vito/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:45:24.380648 vito-1.6.1/vito.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-05-07 21:45:24.000000 vito-1.6.1/vito.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-07 21:45:24.000000 vito-1.6.1/vito.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 21:45:24.000000 vito-1.6.1/vito.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 21:45:24.000000 vito-1.6.1/vito.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 21:45:24.000000 vito-1.6.1/vito.egg-info/top_level.txt
```

### Comparing `vito-1.6.0/LICENSE` & `vito-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vito-1.6.0/PKG-INFO` & `vito-1.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: vito
-Version: 1.6.0
+Version: 1.6.1
 Summary: Lightweight utility package for common computer vision tasks.
 Home-page: https://github.com/snototter/vito
 Author: snototter
 Author-email: snototter@users.noreply.github.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: Pillow>=5.0.0
 
 # vito - Vision Tools
 [![View on PyPI](https://badge.fury.io/py/vito.svg)](https://pypi.org/project/vito)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vito.svg)](https://pypi.org/project/vito)
 [![Build Status](https://app.travis-ci.com/snototter/vito.svg?branch=master)](https://app.travis-ci.com/snototter/vito)
 [![Coverage Status](https://coveralls.io/repos/github/snototter/vito/badge.svg?branch=master)](https://coveralls.io/github/snototter/vito?branch=master)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/snototter/vito/blob/master/LICENSE?raw=true)
@@ -76,17 +76,18 @@
 
 ## Dependencies
 * `numpy`
 * `Pillow`
 
 
 ## Changelog
-* Upcoming `1.6.1`
-  * TODO: Type hints and doc style for cam_projections, colormaps, det2d, flowutils
-  * TODO: flowutils: filenames should be str|pathlib.Path
+* `1.6.1`
+  * House keeping: Internal adaptations to fix deprecated (NumPy) and changed (PIL) library usage.
+  * CI updates to [PyPI's trusted publishing](https://docs.pypi.org/trusted-publishers/).
+  * Code clean up (added type hints, docstrings, ...).
 * `1.6.0`
   * Remove deprecated functionality (workarounds for Python versions older than 3.6).
   * Add type hints and update documentation.
   * Add parameter order check to `imsave` (that's the one thing I alwys mess up
     when coding without IDE).
   * `imsave` now creates the output directory structure if it did not exist.
 * `1.5.3`
@@ -185,9 +186,7 @@
     * `colormaps` - colormap definitions for visualization (jet, parula, magma, viridis, etc.)
     * `imutils` - image loading, conversion, RoI handling (e.g. apply functions on several patches of an image).
     * `imvis` - visualization helpers, e.g. pseudocoloring or overlaying images.
     * `pyutils` - common python functions (timing code, string manipulation, list sorting/search, etc.)
 * `0.0.1`
   * Initial public release.
   * Contains common python/language and camera projection utils.
-
-
```

### Comparing `vito-1.6.0/README.md` & `vito-1.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,17 +60,18 @@
 
 ## Dependencies
 * `numpy`
 * `Pillow`
 
 
 ## Changelog
-* Upcoming `1.6.1`
-  * TODO: Type hints and doc style for cam_projections, colormaps, det2d, flowutils
-  * TODO: flowutils: filenames should be str|pathlib.Path
+* `1.6.1`
+  * House keeping: Internal adaptations to fix deprecated (NumPy) and changed (PIL) library usage.
+  * CI updates to [PyPI's trusted publishing](https://docs.pypi.org/trusted-publishers/).
+  * Code clean up (added type hints, docstrings, ...).
 * `1.6.0`
   * Remove deprecated functionality (workarounds for Python versions older than 3.6).
   * Add type hints and update documentation.
   * Add parameter order check to `imsave` (that's the one thing I alwys mess up
     when coding without IDE).
   * `imsave` now creates the output directory structure if it did not exist.
 * `1.5.3`
```

### Comparing `vito-1.6.0/setup.py` & `vito-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `vito-1.6.0/tests/test_cam_projections.py` & `vito-1.6.1/tests/test_cam_projections.py`

 * *Files identical despite different names*

### Comparing `vito-1.6.0/tests/test_detection2d.py` & `vito-1.6.1/tests/test_detection2d.py`

 * *Files identical despite different names*

### Comparing `vito-1.6.0/tests/test_flowutils.py` & `vito-1.6.1/tests/test_flowutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import numpy as np
 import os
 import pytest
 from vito.flowutils import floread, flosave, colorize_flow
+from pathlib import Path
 
 
 def test_floread():
     exfile = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'examples', 'color_wheel.flo')
     eximg = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'examples', 'flamingo.jpg')
     assert floread(None) is None
-    for fn in ['', 'a-non-existing.file']:
+    for fn in ['', 'a-non-existing.file', Path(), Path('/')]:
         with pytest.raises(FileNotFoundError):
             floread(fn)
     # Load image as flow file
     with pytest.raises(ValueError):
         floread(eximg)
     # Load example .flo
     flow = floread(exfile)
+    flow = floread(Path(exfile))
     assert flow.ndim == 3 and flow.shape[2] == 2
     assert flow.shape[0] == 151
     assert flow.shape[1] == 151
     assert flow.dtype == np.float32
 
 
 def test_flosave(tmp_path):
```

### Comparing `vito-1.6.0/tests/test_imutils.py` & `vito-1.6.1/tests/test_imutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     assert img.dtype == np.uint8
     # ... all channels should contain the same information
     for c in [1, 2]:
         assert np.all(img[:, :, c] == img[:, :, 0])
     # Load 16-bit PNG
     img = imread(os.path.join(exdir, 'depth.png'))
     assert img.ndim == 2 or img.shape[2] == 1
-    assert img.dtype == np.int32
+    assert img.dtype == np.uint16
     # Load 16-bit PNG, specifying mode manually:
     img = imread(os.path.join(exdir, 'depth.png'), mode='I')
     assert img.ndim == 2 or img.shape[2] == 1
     assert img.dtype == np.int32
     # Load 1-bit PNG (requires specifying the mode!)
     img = imread(os.path.join(exdir, 'space-invader.png'), mode='L')
     assert img.ndim == 2 or img.shape[2] == 1
@@ -134,28 +134,26 @@
     _, finfo = safe_shell_output('file', out_fn)
     assert finfo.split(':')[1].strip() == 'PNG image data, 256 x 256, 8-bit grayscale, non-interlaced'
     img_out = imread(out_fn)
     assert img_out.ndim == 2 or img_out.shape[2] == 1
     assert img_out.dtype == np.uint8
     assert np.all(img_in[:] == img_out[:])
     ##########################################################################
-    # Test monochrome 16 bit (will be loaded as np.int32, using PIL's 'I' mode)
+    # Test monochrome 16 bit (PIL <= 8.1 loaded as np.int32, PIL >= 10.0 as
+    # np.uint16, not sure when the API change happened exactly)
     img_in = imread(os.path.join(exdir, 'depth.png'))
     assert img_in.ndim == 2 or img_in.shape[2] == 1
-    assert img_in.dtype == np.int32
-    # Explicitly cast to uint16
-    img_in = img_in.astype(np.uint16)
+    assert img_in.dtype == np.uint16
     # Save (lossless) and reload
     imsave(out_fn, img_in)
     _, finfo = safe_shell_output('file', out_fn)
     assert finfo.split(':')[1].strip() == 'PNG image data, 800 x 600, 16-bit grayscale, non-interlaced'
     img_out = imread(out_fn)
     assert img_out.ndim == 2 or img_out.shape[2] == 1
-    # Loading, however, will still produce a int32 image.
-    assert img_out.dtype == np.int32
+    assert img_out.dtype == np.uint16
     assert np.all(img_in[:] == img_out[:])
     ##########################################################################
     # Test 1-bit PNG (requires specifying the mode!)
     img_in = imread(os.path.join(exdir, 'space-invader.png'), mode='L').astype(bool)
     assert img_in.ndim == 2 or img_in.shape[2] == 1
     assert img_in.dtype == bool
     imsave(out_fn, img_in)
@@ -478,28 +476,28 @@
         c3 = ensure_c3(x)
         assert c3.ndim == 3 and c3.shape[2] == 3
         assert np.array_equal(x[:, :, :3], c3)
 
 
 def test_concat():
     # Invalid inputs
-    x = np.zeros((3,5))
-    y = np.ones((5,7))
+    x = np.zeros((3, 5))
+    y = np.ones((5, 7))
     assert concat(None, None, True) is None
     assert concat(None, None, False) is None
     assert np.array_equal(concat(None, x, True), x)
     assert np.array_equal(concat(None, x, False), x)
     assert np.array_equal(concat(x, None, True), x)
     assert np.array_equal(concat(x, None, False), x)
 
     with pytest.raises(ValueError):
         concat(x, y, True)
     with pytest.raises(ValueError):
         concat(x, y, False)
-    
+
     # ndim == 2, different dtype
     x = np.random.randint(0, 255, (5, 17), dtype=np.uint8)
     y = np.random.randint(0, 255, (5, 2), dtype=np.int32)
     c = concat(x, y, True)
     # The concatenation should have the "better" dtype of the two inputs
     assert c.dtype == y.dtype
     assert np.array_equal(x.astype(c.dtype), c[:, :x.shape[1]])
```

### Comparing `vito-1.6.0/tests/test_imvis.py` & `vito-1.6.1/tests/test_imvis.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
         img2 = 2 * img1
         for dt in [np.uint8, np.float32]:
             for mask in [np.zeros((imshape[0], imshape[1]), dtype=dt),
                          np.zeros((imshape[0], imshape[1], 1), dtype=dt)]:
                 for maskval in [1, 255]:
                     mask[1, 1] = maskval
                     out = overlay(img1, 0.2, img2, mask)
-                    expval = np.uint8(255 * (0.2 * (img1[1, 1] / 255.0)\
+                    expval = np.uint8(255 * (0.2 * (img1[1, 1] / 255.0)
                                       + 0.8 * (img2[1, 1] / 255.0)))
                     # Unmasked regions should be first image
                     assert np.all(out[:, 0] == img1[:, 0])
                     assert np.all(out[:, 2] == img1[:, 2])
                     assert np.all(out[0, :] == img1[0, :])
                     # Only masked regions should be blended
                     assert np.all(out[1, 1] == expval)
```

### Comparing `vito-1.6.0/tests/test_pyutils.py` & `vito-1.6.1/tests/test_pyutils.py`

 * *Files identical despite different names*

### Comparing `vito-1.6.0/vito/cam_projections.py` & `vito-1.6.1/vito/cam_projections.py`

 * *Files identical despite different names*

### Comparing `vito-1.6.0/vito/colormaps.py` & `vito-1.6.1/vito/colormaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     else:
         # Repeat the colormap as often as needed
         reps = int(N / len(cmap))
         rem = N % len(cmap)
         return cmap*reps + cmap[0:rem]
 
 
-def make_flow_color_wheel():
+def make_flow_color_wheel() -> np.ndarray:
     """Returns the standard color wheel (i.e. a 55x3 color map) used for
     optical flow visualization. This is a port of the C++/MATLAB code from
     https://people.csail.mit.edu/celiu/OpticalFlow, thus using similar/same
     names for variables.
     """
     # Color encoding schema
     RY = 15
```

### Comparing `vito-1.6.0/vito/detection2d.py` & `vito-1.6.1/vito/detection2d.py`

 * *Files identical despite different names*

### Comparing `vito-1.6.0/vito/flowutils.py` & `vito-1.6.1/vito/flowutils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,65 @@
 #!/usr/bin/env python
 # coding=utf-8
 """Optical flow I/O and visualization."""
 
-import os
 import sys
 import numpy as np
+from pathlib import Path
+from typing import Union
 from . import colormaps
 
 
-def floread(filename):
+def floread(filename: Union[str, Path]) -> np.ndarray:
     """
     Read optical flow (.flo) files stored in Middlebury format.
 
     Adapted from https://stackoverflow.com/a/28016469/400948
+
+    Args:
+      filename: Path to the input .flo file.
+
+    Returns:
+      HxWx2 numpy array of type `numpy.float32`.
     """
     if sys.byteorder != 'little':
         raise RuntimeError('Current .flo support requires little-endian architecture!')  # pragma: no cover
 
     if filename is None:
         return None
-    if not os.path.exists(filename):
+
+    if not Path(filename).exists():
         raise FileNotFoundError('File %s does not exist' % filename)
 
+    if not Path(filename).is_file():
+        raise FileNotFoundError('Path %s is not a file' % filename)
+
     with open(filename, 'rb') as f:
         # Check magic number
         magic = np.fromfile(f, np.float32, count=1)
-        if 202021.25 != magic:
-            raise ValueError('Invalid magic number in file "%s".' % filename)
+        if 202021.25 != magic[0]:
+            raise ValueError(
+                'Magic number should be 202021.25, but got %f in file "%s"' % (magic[0], filename))
         # Next, get the image dimensions
         w = int(np.fromfile(f, np.int32, count=1))
         h = int(np.fromfile(f, np.int32, count=1))
         # Load the data and reshape
         flow = np.fromfile(f, np.float32, count=2*w*h)
         return np.resize(flow, (h, w, 2))
 
 
-def flosave(filename, flow):
-    """Save HxWx2 optical flow to file in Middlebury format."""
+def flosave(filename: Union[str, Path], flow: np.ndarray) -> None:
+    """
+    Save HxWx2 optical flow to file in Middlebury format.
+
+    Args:
+      filename: Output file path.
+      flow: Optical flow components as HxWx2 numpy array of
+        type `numpy.float32`
+    """
     if len(flow.shape) != 3 or flow.shape[2] != 2:
         raise ValueError('Invalid flow shape!')
     # Prepare data
     h, w = flow.shape[0], flow.shape[1]
     data = np.zeros((h, w*2))
     data[:, np.arange(w)*2] = flow[:, :, 0]
     data[:, np.arange(w)*2 + 1] = flow[:, :, 1]
@@ -52,32 +71,39 @@
         np.array(w).astype(np.int32).tofile(f)
         np.array(h).astype(np.int32).tofile(f)
         # Write actual data
         data.astype(np.float32).tofile(f)
 
 
 def colorize_uv(
-        u, v, return_rgb=True, colorwheel=colormaps.make_flow_color_wheel()):
+        u: np.ndarray,
+        v: np.ndarray,
+        return_rgb: bool = True,
+        colorwheel: np.ndarray = colormaps.make_flow_color_wheel()
+        ) -> np.ndarray:
     """
     Colorizes the given optical flow using the flow color wheel.
     This function performs no normalization or sanity checks. Usually, you
     should prefer colorize_flow() instead!
 
     This is a port of the C++/MATLAB code from
     https://people.csail.mit.edu/celiu/OpticalFlow, also based on
     https://github.com/tomrunia/OpticalFlow_Visualization.
 
-    :param u: horizontal flow components as HxW np.ndarray
-    :param v: vertical flow components as HxW np.ndarray
-    :param return_rgb: bool, whether to return RGB or BGR
-    :param colorwheel: provide a num_colors-by-3 color numpy nd.array
-            which will be used as color wheel
-    :param convert_to_bgr: bool, whether to change ordering and
-         output BGR instead of RGB
-    :return:  HxWx3 uint8 numpy ndarray.
+    Args:
+      u: horizontal flow components as HxW np.ndarray
+      v: vertical flow components as HxW np.ndarray
+      return_rgb: bool, whether to return RGB or BGR
+      colorwheel: provide a num_colors-by-3 color numpy nd.array
+        which will be used as color wheel
+      convert_to_bgr: bool, whether to change ordering and
+        output BGR instead of RGB
+
+    Returns:
+      HxWx3 uint8 numpy ndarray.
     """
     vis = np.zeros((u.shape[0], u.shape[1], 3), np.uint8)
     ncols = colorwheel.shape[0]
 
     rad = np.sqrt(np.square(u) + np.square(v))
     a = np.arctan2(-v, -u) / np.pi
 
@@ -100,15 +126,18 @@
         col[~idx] = col[~idx] * 0.75
         # BGR or RGB?
         ch_idx = i if return_rgb else 2-i
         vis[:, :, ch_idx] = np.floor(255.0 * col)
     return vis
 
 
-def colorize_flow(flow, max_val=None, return_rgb=True):
+def colorize_flow(
+        flow: np.ndarray,
+        max_val: float = None,
+        return_rgb: bool = True) -> np.ndarray:
     """
     Returns the widely used flow visualization.
 
     This is a port of the C++/MATLAB code from
     https://people.csail.mit.edu/celiu/OpticalFlow, also based on
     https://github.com/tomrunia/OpticalFlow_Visualization.
```

### Comparing `vito-1.6.0/vito/imutils.py` & `vito-1.6.1/vito/imutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding=utf-8
 """Utilities you'll often need when working with images ;-)"""
 
 # TODOs:
 # * imread/imsave should use tifffile for tiff files - supports multi-band images
 
 import io
-import os
 from pathlib import Path
 from typing import Any, Sequence, Union
 import numpy as np
 from PIL import Image
 from PIL import ImageFilter
 
 
@@ -50,17 +49,23 @@
             return nparray[:, :, :3]
     raise ValueError("Invalid input to ensure_c3, input must be a 1-, 3- or 4-channel image.")
 
 
 def rgb2gray(
         nparray: np.ndarray,
         is_bgr: bool = False
-    ) -> np.ndarray:
+        ) -> np.ndarray:
     """
-    Converts the RGB image to grayscale using `L = 0.2989 R + 0.5870 G + 0.1140 B`.
+    Converts the RGB image to grayscale
+    using `L = 0.2989 R + 0.5870 G + 0.1140 B`.
+
+    Args:
+      nparray: HxWxC numpy array.
+      is_bgr: If True, the input channels are in BGR format. Otherwise, they
+        are assumed to be RGB.
     """
     if nparray is None:
         return None
     if nparray.ndim == 2 or (nparray.ndim == 3 and nparray.shape[2] == 1):
         return nparray
     if nparray.ndim == 3 and nparray.shape[2] == 2:
         raise ValueError('Cannot convert a 2 channel input image to grayscale.')
@@ -73,35 +78,36 @@
 # Alias for convenience
 grayscale = rgb2gray
 
 
 def __imsave_checks(
         filename: Union[str, Path],
         image: np.ndarray
-    ) -> None:
+        ) -> None:
     if not isinstance(filename, Path):
         filename = Path(filename)
     if not filename.exists():
         filename.absolute().parents[0].mkdir(parents=True, exist_ok=True)
     if not isinstance(image, np.ndarray):
         raise TypeError(
             f'Image is not a NumPy array, but `{type(image)}`. Check the'
             'parameter order: (`filename`, `image`, `flip_channels`)!')
 
+
 try:
     # Try to load OpenCV (in case you installed it in your workspace)
     import cv2
 
     def imsave(
             filename: Union[str, Path],
             image: np.ndarray,
             flip_channels: bool = False
-        ) -> None:  # pragma: no cover
+            ) -> None:  # pragma: no cover
         """Stores the image using OpenCV.
-        
+
         This function *will create the output directory* if it does not
         exist yet.
         If you have a BGR image, set `flip_channels = True` to store it
         correctly.
         """
         __imsave_checks(filename, image)
 
@@ -113,17 +119,17 @@
             cv2.imwrite(str(filename), image)
 except:
     # Fall back to Pillow
     def imsave(
             filename: Union[str, Path],
             image: np.ndarray,
             flip_channels: bool = False
-        ) -> None:
+            ) -> None:
         """Stores the image using PIL/Pillow.
-        
+
         This function *will create the output directory* if it does not
         exist yet.
         If you have a BGR image, set `flip_channels = True` to store it
         correctly.
         """
         __imsave_checks(filename, image)
         if flip_channels:
@@ -133,15 +139,15 @@
         Image.fromarray(im_np).save(str(filename))
 
 
 def imread(
         filename: Union[str, Path],
         flip_channels: bool = False,
         **kwargs
-    ) -> np.ndarray:
+        ) -> np.ndarray:
     """Loads an image (using PIL/Pillow) into a NumPy array.
 
     Multi-channel images are returned as RGB format unless you
     set `flip_channels=True` (which will swap the R & B channels).
 
     Optional kwargs will be passed on to PIL's Image.convert(). Thus, you can
     specify PIL's loading 'mode', e.g. 'RGB' for color, 'RGBA' for a
@@ -150,15 +156,16 @@
     if filename is None:
         return None
     if not isinstance(filename, Path):
         filename = Path(filename)
     if not filename.exists() or not filename.is_file():
         raise FileNotFoundError(f'Image `{filename}` does not exist')
     if not isinstance(flip_channels, bool):
-        raise TypeError(f'Parameter `flip_channels` must be bool, not `{type(flip_channels)}` '
+        raise TypeError(
+            f'Parameter `flip_channels` must be bool, not `{type(flip_channels)}` '
             '- you probably forgot the keyword for the PIL **kwargs!')
     # PIL loads 16-bit PNGs as np.int32 ndarray. If we need to support other
     # bit depths, we should look into using pypng, see documentation at
     # https://pythonhosted.org/pypng/ex.html#reading
     # For now, PIL provides all we need
     image = np.asarray(Image.open(filename).convert(**kwargs))
 
@@ -167,48 +174,52 @@
     else:
         return image
 
 
 def ndarray2memory_file(
         np_data: np.ndarray,
         format: str = 'png'
-    ) -> io.BytesIO:
+        ) -> io.BytesIO:
     """Converts the numpy (image) array to a BytesIO stream.
 
     Useful to transfer an image via sockets.
     """
     if np_data is None:
         return None
     img = Image.fromarray(np_data)
     img_memory_file = io.BytesIO()
     img.save(img_memory_file, format)
     return img_memory_file
 
 
 def memory_file2ndarray(
         memfile: io.BytesIO
-    ) -> np.ndarray:
+        ) -> np.ndarray:
     """Loads an image stored in the given BytesIO memory file."""
     if memfile is None:
         return None
     return np.asarray(Image.open(memfile))
 
 
 def clip_rect_to_image(
         rect: Sequence[Any],
         img_width: int,
         img_height: int
-    ) -> tuple:
+        ) -> tuple:
     """Ensures that the rectangle is within the image boundaries.
 
     Explicitly casts all entries to integer.
-    :param rect: list/tuple (l,t,w,h)
-    :param img_width: int
-    :param img_height: int
-    :return: (l, t, w, h)
+
+    Args:
+      rect: list/tuple (l,t,w,h)
+      img_width: int
+      img_height: int
+
+    Returns:
+      (l, t, w, h)
     """
     l, t, w, h = int(rect[0]), int(rect[1]), int(rect[2]), int(rect[3])
     # Right/bottom bounds are exclusive
     r = max(0, min(img_width, l+w))
     b = max(0, min(img_height, t+h))
     # Left/top bounds are inclusive
     l = max(0, l)
@@ -223,35 +234,39 @@
 
 def apply_on_bboxes(
         image_np: np.ndarray,
         bboxes: list,
         func,
         *args,
         **func_kwargs
-    ) -> np.ndarray:
-    """Applies the given function (which returns a modified image) on each
+        ) -> np.ndarray:
+    """
+    Applies the given function (which returns a modified image) on each
     bounding box.
-    
+
     This function takes care of proper clipping of each bounding box, roi
     extraction and copying back the results.
 
-    :param image_np: numpy ndarray, input image
-    :param bboxes: list of bounding boxes, i.e. [(l, t, w, h), (...)]
-    :param func: function handle to apply on each bounding box
-    :param func_kwargs: optional kwargs passed on to the function
-    :return: numpy ndarray, a copy of the input image after applying the given
-             function on each (valid) bounding box
+    Args:
+      image_np: numpy ndarray, input image
+      bboxes: list of bounding boxes, i.e. [(l, t, w, h), (...)]
+      func: function handle to apply on each bounding box
+      func_kwargs: optional kwargs passed on to the function
+
+    Returns:
+      numpy ndarray, a copy of the input image after applying the given
+      function on each (valid) bounding box
     """
     if image_np is None:
         return None
     # Ensure the image is writeable
     image_np = image_np.copy()
     # Prevent invalid memory access
     bboxes = [clip_rect_to_image(bb, image_np.shape[1], image_np.shape[0])
-            for bb in bboxes]
+              for bb in bboxes]
     bboxes = [b for b in bboxes if is_valid_bbox(b)]
     for bb in bboxes:
         l, t, w, h = bb
         roi = image_np[t:t+h, l:l+w]
         image_np[t:t+h, l:l+w] = func(roi, *args, **func_kwargs)
     return image_np
 
@@ -279,15 +294,15 @@
 crop = roi
 
 
 def pad(
         image_np: np.ndarray,
         border: int,
         color: tuple = None
-    ) -> np.ndarray:
+        ) -> np.ndarray:
     """Pads the image by 'border' pixels in each direction.
 
     :param image_np: HxWxC numpy ndarray.
     :param border: int > 0.
     :param color: If None, border will be transparent.
                   Otherwise, the border will be drawn in the
                   corresponding color (RGB/BGR tuple or scalar).
@@ -323,15 +338,15 @@
         return out
 
 
 def pixelate(
         image_np: np.ndarray,
         block_width: int = 5,
         block_height: int = -1
-    ) -> np.ndarray:
+        ) -> np.ndarray:
     """
     Pixelate the image into blocks of size WxH.
     If H is -1, then H=W. Otherwise, rectangular blocks will
     be used (unless W is negative, in which case W=H will be used).
     """
     if image_np is None:
         return None
@@ -346,29 +361,29 @@
         .resize((image_np.shape[1], image_np.shape[0]), resample=Image.NEAREST)
     return np.asarray(pixelized_roi)
 
 
 def gaussian_blur(
         image_np: np.ndarray,
         radius: int = 15
-    ) -> np.ndarray:
+        ) -> np.ndarray:
     """Blurs the image using a Gaussian kernel with the given radius."""
     if image_np is None:
         return None
     img = Image.fromarray(image_np).filter(
         ImageFilter.GaussianBlur(radius=radius))
     return np.asarray(img)
 
 
 def set_to(
         image_np: np.ndarray,
         value: Any
-    ) -> np.ndarray:
+        ) -> np.ndarray:
     """Sets the image pixels to the given value.
-    
+
     The parameter `value` can either be a tuple of float/int (specifying a
     color) or a scalar value (int/float).
     """
     if image_np is None or value is None:
         return None
     if isinstance(value, tuple):
         channels = 1 if image_np.ndim < 3 else image_np.shape[2]
@@ -384,15 +399,15 @@
     return image_np
 
 
 def _make_stack_compatible(
         img1: np.ndarray,
         img2: np.ndarray,
         horizontal: bool
-    ) -> tuple:
+        ) -> tuple:
     """
     Returns two "compatible" images to be used for horizontal or vertical
     stacking, i.e. they'll have the correct size, same dtype and number of
     channels.
     """
     # Check for compatible sizes
     if horizontal and img1.shape[0] != img2.shape[0]:
@@ -420,42 +435,42 @@
             raise ValueError('If channels are different, one of the inputs must be single-channel.')
     return img1, img2
 
 
 def hstack(
         img1: np.ndarray,
         img2: np.ndarray
-    ) -> np.ndarray:
+        ) -> np.ndarray:
     """Horizontally concatenates the two given images."""
     if img1 is None:
         return img2
     if img2 is None:
         return img1
     img1, img2 = _make_stack_compatible(img1, img2, True)
     return np.hstack((img1, img2))
 
 
 def vstack(
         img1: np.ndarray,
         img2: np.ndarray
-    ) -> np.ndarray:
+        ) -> np.ndarray:
     """Vertically concatenates the two given images."""
     if img1 is None:
         return img2
     if img2 is None:
         return img1
     img1, img2 = _make_stack_compatible(img1, img2, False)
     return np.vstack((img1, img2))
 
 
 def concat(
         img1: np.ndarray,
         img2: np.ndarray,
         horizontal: bool = True
-    ) -> np.ndarray:
+        ) -> np.ndarray:
     """Concatenates the two given images either horizontally or vertically."""
     if horizontal:
         return hstack(img1, img2)
     else:
         return vstack(img1, img2)
```

### Comparing `vito-1.6.0/vito/imvis.py` & `vito-1.6.1/vito/imvis.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,29 @@
                 be forwarded to the internal `cv2.waitKey()` call.
             flip_channels: If your input is BGR, set this to True for correct
                 color display.
 
         Returns:
             Pressed key code or -1, i.e. the `cv2.waitKey()` output.
         """
+        if img_np is None:
+            return -1
+        
         if not flip_channels:
             disp = imutils.flip_layers(img_np)
         else:
             disp = img_np
+        
+        # Common mistake: a boolean mask is not a valid input for cv2.imshow,
+        # this would cause a cv2.error and we would fall back to PIL's imshow
+        # which opens a new window for each image.
+        # To avoid this, we convert boolean masks to uint8 images:
+        if disp.dtype == bool:
+            disp = disp.astype(np.uint8) * 255
+
         try:
             cv2.imshow(title, disp)
             if wait_ms == 0:
                 return -1
             else:
                 return cv2.waitKey(wait_ms)
         except cv2.error:
```

### Comparing `vito-1.6.0/vito/pyutils.py` & `vito-1.6.1/vito/pyutils.py`

 * *Files identical despite different names*

### Comparing `vito-1.6.0/vito.egg-info/PKG-INFO` & `vito-1.6.1/vito.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: vito
-Version: 1.6.0
+Version: 1.6.1
 Summary: Lightweight utility package for common computer vision tasks.
 Home-page: https://github.com/snototter/vito
 Author: snototter
 Author-email: snototter@users.noreply.github.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: Pillow>=5.0.0
 
 # vito - Vision Tools
 [![View on PyPI](https://badge.fury.io/py/vito.svg)](https://pypi.org/project/vito)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vito.svg)](https://pypi.org/project/vito)
 [![Build Status](https://app.travis-ci.com/snototter/vito.svg?branch=master)](https://app.travis-ci.com/snototter/vito)
 [![Coverage Status](https://coveralls.io/repos/github/snototter/vito/badge.svg?branch=master)](https://coveralls.io/github/snototter/vito?branch=master)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/snototter/vito/blob/master/LICENSE?raw=true)
@@ -76,17 +76,18 @@
 
 ## Dependencies
 * `numpy`
 * `Pillow`
 
 
 ## Changelog
-* Upcoming `1.6.1`
-  * TODO: Type hints and doc style for cam_projections, colormaps, det2d, flowutils
-  * TODO: flowutils: filenames should be str|pathlib.Path
+* `1.6.1`
+  * House keeping: Internal adaptations to fix deprecated (NumPy) and changed (PIL) library usage.
+  * CI updates to [PyPI's trusted publishing](https://docs.pypi.org/trusted-publishers/).
+  * Code clean up (added type hints, docstrings, ...).
 * `1.6.0`
   * Remove deprecated functionality (workarounds for Python versions older than 3.6).
   * Add type hints and update documentation.
   * Add parameter order check to `imsave` (that's the one thing I alwys mess up
     when coding without IDE).
   * `imsave` now creates the output directory structure if it did not exist.
 * `1.5.3`
@@ -185,9 +186,7 @@
     * `colormaps` - colormap definitions for visualization (jet, parula, magma, viridis, etc.)
     * `imutils` - image loading, conversion, RoI handling (e.g. apply functions on several patches of an image).
     * `imvis` - visualization helpers, e.g. pseudocoloring or overlaying images.
     * `pyutils` - common python functions (timing code, string manipulation, list sorting/search, etc.)
 * `0.0.1`
   * Initial public release.
   * Contains common python/language and camera projection utils.
-
-
```

