# Comparing `tmp/guibot-0.50.1.tar.gz` & `tmp/guibot-0.51.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guibot-0.50.1.tar", last modified: Fri Jan 28 16:20:37 2022, max compression
+gzip compressed data, was "guibot-0.51.1.tar", last modified: Tue May  7 05:15:26 2024, max compression
```

## Comparing `guibot-0.50.1.tar` & `guibot-0.51.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-28 16:20:37.213319 guibot-0.50.1/
--rw-r--r--   0 root         (0) root         (0)     5168 2022-01-28 16:20:37.213319 guibot-0.50.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-28 16:20:37.213319 guibot-0.50.1/guibot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5168 2022-01-28 16:20:37.000000 guibot-0.50.1/guibot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      560 2022-01-28 16:20:37.000000 guibot-0.50.1/guibot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-28 16:20:37.000000 guibot-0.50.1/guibot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-01-28 16:20:37.000000 guibot-0.50.1/guibot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-01-28 16:20:37.000000 guibot-0.50.1/guibot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-28 16:20:37.213319 guibot-0.50.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1531 2022-01-28 16:18:34.000000 guibot-0.50.1/setup.py
+drwxr-xr-x   0 pevogam   (1000) pevogam   (1000)        0 2024-05-07 05:15:26.845714 guibot-0.51.1/
+-rw-r--r--   0 pevogam   (1000) pevogam   (1000)     4746 2024-05-07 05:15:26.845714 guibot-0.51.1/PKG-INFO
+drwxr-xr-x   0 pevogam   (1000) pevogam   (1000)        0 2024-05-07 05:15:26.845714 guibot-0.51.1/guibot.egg-info/
+-rw-r--r--   0 pevogam   (1000) pevogam   (1000)     4746 2024-05-07 05:15:26.000000 guibot-0.51.1/guibot.egg-info/PKG-INFO
+-rw-r--r--   0 pevogam   (1000) pevogam   (1000)      560 2024-05-07 05:15:26.000000 guibot-0.51.1/guibot.egg-info/SOURCES.txt
+-rw-r--r--   0 pevogam   (1000) pevogam   (1000)        1 2024-05-07 05:15:26.000000 guibot-0.51.1/guibot.egg-info/dependency_links.txt
+-rw-r--r--   0 pevogam   (1000) pevogam   (1000)        7 2024-05-07 05:15:26.000000 guibot-0.51.1/guibot.egg-info/requires.txt
+-rw-r--r--   0 pevogam   (1000) pevogam   (1000)        7 2024-05-07 05:15:26.000000 guibot-0.51.1/guibot.egg-info/top_level.txt
+-rw-r--r--   0 pevogam   (1000) pevogam   (1000)       38 2024-05-07 05:15:26.845714 guibot-0.51.1/setup.cfg
+-rw-r--r--   0 pevogam   (1000) pevogam   (1000)     1531 2024-05-07 04:19:46.000000 guibot-0.51.1/setup.py
```

### Comparing `guibot-0.50.1/PKG-INFO` & `guibot-0.51.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,15 @@
 Metadata-Version: 2.1
 Name: guibot
-Version: 0.50.1
+Version: 0.51.1
 Summary: GUI automation tool
 Home-page: http://guibot.org
+Download-URL: 
 Maintainer: Intra2net
 Maintainer-email: opensource@intra2net.com
-License: UNKNOWN
-Description: # Guibot [![Build Status](https://travis-ci.org/intra2net/guibot.svg?branch=master)](https://travis-ci.org/intra2net/guibot) [![Documentation Status](https://readthedocs.org/projects/guibot/badge/?version=latest)](http://guibot.readthedocs.io/en/latest/?badge=latest) [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/intra2net/guibot.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/intra2net/guibot/context:python) [![codecov](https://codecov.io/gh/intra2net/guibot/branch/master/graph/badge.svg)](https://codecov.io/gh/intra2net/guibot)
-        
-        A tool for GUI automation using a variety of computer vision and display control backends.
-        
-        ## Introduction and concepts
-        
-        In order to do GUI automation you usually need to solve two problems: first, you need to have a way to control and interact with the interface and platform you are automating and second, you need to be able to locate the objects you are interested in on the screen. Guibot helps you do both.
-        
-        To interact with GUIs, Guibot provides the [`controller`](https://github.com/intra2net/guibot/blob/master/guibot/controller.py) module which contains a common interface for different display backends, with methods to move the mouse, take screenshots, type characters and so on. The backend to use will depend on how your platform is accessible, with some backends running directly as native binaries or python scripts on Windows, macOS, and Linux while others connecting through remote VNC displays.
-        
-        To locate an element on the screen, you will need an image representing the screen, a [`target`](https://github.com/intra2net/guibot/blob/master/guibot/target.py) representing the element (an image or a text in the simplest cases) and a [`finder`](https://github.com/intra2net/guibot/blob/master/guibot/finder.py) configured for the target. The finder looks for the target within the screenshot image and returns the coordinates to the region where that target appears. Finders, just like display controllers, are wrappers around different backends supported by Guibot that could vary from a simplest 1:1 pixel matching by controller backends, to template or feature matching mix by OpenCV, to OCR and ML solutions by Tesseract and AI frameworks.
-        
-        Finally, to bridge the gap between controlling the GUI and finding target elements, the [`region`](https://github.com/intra2net/guibot/blob/master/guibot/region.py) module is provided. It represents a subregion of a screen and contains methods to locate targets in this region using a choice of finder and interact with the graphical interface using a choice of controller.
-        
-        ## Supported backends
-        
-        Supported Computer Vision (CV) backends are based on
-        
-        - [OpenCV](https://github.com/opencv/opencv)
-            - Template matching
-            - Contour matching
-            - Feature matching
-            - Haar cascade matching
-            - Template-feature and mixed matching
-        - [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)
-            - Text matching through pytesseract, tesserocr, or OpenCV's bindings
-        - [PyTorch](https://github.com/pytorch/pytorch)
-            - R-CNN matching through Faster R-CNN or Mask R-CNN
-        - [autopy](https://github.com/msanders/autopy)
-            - AutoPy matching
-        
-        Supported Display Controller (DC) backends are based on
-        
-        - [PyAutoGUI](https://github.com/asweigart/pyautogui)
-        - [AutoPy](https://github.com/msanders/autopy)
-        - [VNCDoTool](https://github.com/sibson/vncdotool)
-        - [XDoTool](https://www.semicomplete.com/projects/xdotool)
-        
-        ## Further resources
-        
-        Homepage: http://guibot.org
-        
-        Documentation: http://guibot.readthedocs.io
-        
-        Installation: https://github.com/intra2net/guibot/wiki/Packaging
-        
-        Issue tracking: https://github.com/intra2net/guibot/issues
-        
-        Project wiki: https://github.com/intra2net/guibot/wiki
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
@@ -69,7 +18,57 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Desktop Environment
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+
+# Guibot [![GH Actions](https://github.com/intra2net/guibot/actions/workflows/ci.yml/badge.svg)](https://github.com/intra2net/guibot/actions/workflows/ci.yml) [![Documentation Status](https://readthedocs.org/projects/guibot/badge/?version=latest)](http://guibot.readthedocs.io/en/latest/?badge=latest) [![CodeQL](https://github.com/intra2net/guibot/actions/workflows/codeql.yml/badge.svg)](https://github.com/intra2net/guibot/actions/workflows/codeql.yml) [![codecov](https://codecov.io/gh/intra2net/guibot/branch/master/graph/badge.svg)](https://codecov.io/gh/intra2net/guibot)
+
+A tool for GUI automation using a variety of computer vision and display control backends.
+
+## Introduction and concepts
+
+In order to do GUI automation you usually need to solve two problems: first, you need to have a way to control and interact with the interface and platform you are automating and second, you need to be able to locate the objects you are interested in on the screen. Guibot helps you do both.
+
+To interact with GUIs, Guibot provides the [controller](https://github.com/intra2net/guibot/blob/master/guibot/controller.py) module which contains a common interface for different display backends, with methods to move the mouse, take screenshots, type characters and so on. The backend to use will depend on how your platform is accessible, with some backends running directly as native binaries or python scripts on Windows, macOS, and Linux while others connecting through remote VNC displays.
+
+To locate an element on the screen, you will need an image representing the screen, a [target](https://github.com/intra2net/guibot/blob/master/guibot/target.py) representing the element (an image or a text in the simplest cases) and a [finder](https://github.com/intra2net/guibot/blob/master/guibot/finder.py) configured for the target. The finder looks for the target within the screenshot image and returns the coordinates to the region where that target appears. Finders, just like display controllers, are wrappers around different backends supported by Guibot that could vary from a simplest 1:1 pixel matching by controller backends, to template or feature matching mix by OpenCV, to OCR and ML solutions by Tesseract and AI frameworks.
+
+Finally, to bridge the gap between controlling the GUI and finding target elements, the [region](https://github.com/intra2net/guibot/blob/master/guibot/region.py) module is provided. It represents a subregion of a screen and contains methods to locate targets in this region using a choice of finder and interact with the graphical interface using a choice of controller.
+
+## Supported backends
+
+Supported Computer Vision (CV) backends are based on
+
+- [OpenCV](https://github.com/opencv/opencv)
+    - Template matching
+    - Contour matching
+    - Feature matching
+    - Haar cascade matching
+    - Template-feature and mixed matching
+- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)
+    - Text matching through pytesseract, tesserocr, or OpenCV's bindings
+- [PyTorch](https://github.com/pytorch/pytorch)
+    - R-CNN matching through Faster R-CNN or Mask R-CNN
+- [autopy](https://github.com/msanders/autopy)
+    - AutoPy matching
+
+Supported Display Controller (DC) backends are based on
+
+- [PyAutoGUI](https://github.com/asweigart/pyautogui)
+- [AutoPy](https://github.com/msanders/autopy)
+- [VNCDoTool](https://github.com/sibson/vncdotool)
+- [XDoTool](https://www.semicomplete.com/projects/xdotool)
+
+## Further resources
+
+Homepage: http://guibot.org
+
+Documentation: http://guibot.readthedocs.io
+
+Installation: https://github.com/intra2net/guibot/wiki/Packaging
+
+Issue tracking: https://github.com/intra2net/guibot/issues
+
+Project wiki: https://github.com/intra2net/guibot/wiki
```

### Comparing `guibot-0.50.1/guibot.egg-info/PKG-INFO` & `guibot-0.51.1/guibot.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,15 @@
 Metadata-Version: 2.1
 Name: guibot
-Version: 0.50.1
+Version: 0.51.1
 Summary: GUI automation tool
 Home-page: http://guibot.org
+Download-URL: 
 Maintainer: Intra2net
 Maintainer-email: opensource@intra2net.com
-License: UNKNOWN
-Description: # Guibot [![Build Status](https://travis-ci.org/intra2net/guibot.svg?branch=master)](https://travis-ci.org/intra2net/guibot) [![Documentation Status](https://readthedocs.org/projects/guibot/badge/?version=latest)](http://guibot.readthedocs.io/en/latest/?badge=latest) [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/intra2net/guibot.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/intra2net/guibot/context:python) [![codecov](https://codecov.io/gh/intra2net/guibot/branch/master/graph/badge.svg)](https://codecov.io/gh/intra2net/guibot)
-        
-        A tool for GUI automation using a variety of computer vision and display control backends.
-        
-        ## Introduction and concepts
-        
-        In order to do GUI automation you usually need to solve two problems: first, you need to have a way to control and interact with the interface and platform you are automating and second, you need to be able to locate the objects you are interested in on the screen. Guibot helps you do both.
-        
-        To interact with GUIs, Guibot provides the [`controller`](https://github.com/intra2net/guibot/blob/master/guibot/controller.py) module which contains a common interface for different display backends, with methods to move the mouse, take screenshots, type characters and so on. The backend to use will depend on how your platform is accessible, with some backends running directly as native binaries or python scripts on Windows, macOS, and Linux while others connecting through remote VNC displays.
-        
-        To locate an element on the screen, you will need an image representing the screen, a [`target`](https://github.com/intra2net/guibot/blob/master/guibot/target.py) representing the element (an image or a text in the simplest cases) and a [`finder`](https://github.com/intra2net/guibot/blob/master/guibot/finder.py) configured for the target. The finder looks for the target within the screenshot image and returns the coordinates to the region where that target appears. Finders, just like display controllers, are wrappers around different backends supported by Guibot that could vary from a simplest 1:1 pixel matching by controller backends, to template or feature matching mix by OpenCV, to OCR and ML solutions by Tesseract and AI frameworks.
-        
-        Finally, to bridge the gap between controlling the GUI and finding target elements, the [`region`](https://github.com/intra2net/guibot/blob/master/guibot/region.py) module is provided. It represents a subregion of a screen and contains methods to locate targets in this region using a choice of finder and interact with the graphical interface using a choice of controller.
-        
-        ## Supported backends
-        
-        Supported Computer Vision (CV) backends are based on
-        
-        - [OpenCV](https://github.com/opencv/opencv)
-            - Template matching
-            - Contour matching
-            - Feature matching
-            - Haar cascade matching
-            - Template-feature and mixed matching
-        - [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)
-            - Text matching through pytesseract, tesserocr, or OpenCV's bindings
-        - [PyTorch](https://github.com/pytorch/pytorch)
-            - R-CNN matching through Faster R-CNN or Mask R-CNN
-        - [autopy](https://github.com/msanders/autopy)
-            - AutoPy matching
-        
-        Supported Display Controller (DC) backends are based on
-        
-        - [PyAutoGUI](https://github.com/asweigart/pyautogui)
-        - [AutoPy](https://github.com/msanders/autopy)
-        - [VNCDoTool](https://github.com/sibson/vncdotool)
-        - [XDoTool](https://www.semicomplete.com/projects/xdotool)
-        
-        ## Further resources
-        
-        Homepage: http://guibot.org
-        
-        Documentation: http://guibot.readthedocs.io
-        
-        Installation: https://github.com/intra2net/guibot/wiki/Packaging
-        
-        Issue tracking: https://github.com/intra2net/guibot/issues
-        
-        Project wiki: https://github.com/intra2net/guibot/wiki
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
@@ -69,7 +18,57 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Desktop Environment
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+
+# Guibot [![GH Actions](https://github.com/intra2net/guibot/actions/workflows/ci.yml/badge.svg)](https://github.com/intra2net/guibot/actions/workflows/ci.yml) [![Documentation Status](https://readthedocs.org/projects/guibot/badge/?version=latest)](http://guibot.readthedocs.io/en/latest/?badge=latest) [![CodeQL](https://github.com/intra2net/guibot/actions/workflows/codeql.yml/badge.svg)](https://github.com/intra2net/guibot/actions/workflows/codeql.yml) [![codecov](https://codecov.io/gh/intra2net/guibot/branch/master/graph/badge.svg)](https://codecov.io/gh/intra2net/guibot)
+
+A tool for GUI automation using a variety of computer vision and display control backends.
+
+## Introduction and concepts
+
+In order to do GUI automation you usually need to solve two problems: first, you need to have a way to control and interact with the interface and platform you are automating and second, you need to be able to locate the objects you are interested in on the screen. Guibot helps you do both.
+
+To interact with GUIs, Guibot provides the [controller](https://github.com/intra2net/guibot/blob/master/guibot/controller.py) module which contains a common interface for different display backends, with methods to move the mouse, take screenshots, type characters and so on. The backend to use will depend on how your platform is accessible, with some backends running directly as native binaries or python scripts on Windows, macOS, and Linux while others connecting through remote VNC displays.
+
+To locate an element on the screen, you will need an image representing the screen, a [target](https://github.com/intra2net/guibot/blob/master/guibot/target.py) representing the element (an image or a text in the simplest cases) and a [finder](https://github.com/intra2net/guibot/blob/master/guibot/finder.py) configured for the target. The finder looks for the target within the screenshot image and returns the coordinates to the region where that target appears. Finders, just like display controllers, are wrappers around different backends supported by Guibot that could vary from a simplest 1:1 pixel matching by controller backends, to template or feature matching mix by OpenCV, to OCR and ML solutions by Tesseract and AI frameworks.
+
+Finally, to bridge the gap between controlling the GUI and finding target elements, the [region](https://github.com/intra2net/guibot/blob/master/guibot/region.py) module is provided. It represents a subregion of a screen and contains methods to locate targets in this region using a choice of finder and interact with the graphical interface using a choice of controller.
+
+## Supported backends
+
+Supported Computer Vision (CV) backends are based on
+
+- [OpenCV](https://github.com/opencv/opencv)
+    - Template matching
+    - Contour matching
+    - Feature matching
+    - Haar cascade matching
+    - Template-feature and mixed matching
+- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)
+    - Text matching through pytesseract, tesserocr, or OpenCV's bindings
+- [PyTorch](https://github.com/pytorch/pytorch)
+    - R-CNN matching through Faster R-CNN or Mask R-CNN
+- [autopy](https://github.com/msanders/autopy)
+    - AutoPy matching
+
+Supported Display Controller (DC) backends are based on
+
+- [PyAutoGUI](https://github.com/asweigart/pyautogui)
+- [AutoPy](https://github.com/msanders/autopy)
+- [VNCDoTool](https://github.com/sibson/vncdotool)
+- [XDoTool](https://www.semicomplete.com/projects/xdotool)
+
+## Further resources
+
+Homepage: http://guibot.org
+
+Documentation: http://guibot.readthedocs.io
+
+Installation: https://github.com/intra2net/guibot/wiki/Packaging
+
+Issue tracking: https://github.com/intra2net/guibot/issues
+
+Project wiki: https://github.com/intra2net/guibot/wiki
```

### Comparing `guibot-0.50.1/guibot.egg-info/SOURCES.txt` & `guibot-0.51.1/guibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guibot-0.50.1/setup.py` & `guibot-0.51.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 p = path.abspath(path.dirname(__file__))
 with open(path.join(p, '../README.md')) as f:
     README = f.read()
 
 setup(
     name='guibot',
-    version='0.50.1',
+    version='0.51.1',
     description='GUI automation tool',
     long_description=README,
     long_description_content_type='text/markdown',
 
     install_requires=[
         "Pillow",
     ],
```

