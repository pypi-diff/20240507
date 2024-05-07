# Comparing `tmp/moviesampler-1.1.tar.gz` & `tmp/moviesampler-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moviesampler-1.1.tar", last modified: Mon May  6 16:33:21 2024, max compression
+gzip compressed data, was "moviesampler-1.2.tar", last modified: Tue May  7 07:14:01 2024, max compression
```

## Comparing `moviesampler-1.1.tar` & `moviesampler-1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 javier    (1000) javier    (1000)        0 2024-05-06 16:33:21.205705 moviesampler-1.1/
--rw-rw-r--   0 javier    (1000) javier    (1000)     3820 2024-05-06 09:15:41.000000 moviesampler-1.1/LICENSE
--rw-r--r--   0 javier    (1000) javier    (1000)     2264 2024-05-06 16:33:21.205705 moviesampler-1.1/PKG-INFO
--rw-rw-r--   0 javier    (1000) javier    (1000)     1290 2024-05-06 09:23:13.000000 moviesampler-1.1/README.md
-drwxrwxr-x   0 javier    (1000) javier    (1000)        0 2024-05-06 16:33:21.205705 moviesampler-1.1/moviesampler/
--rw-rw-r--   0 javier    (1000) javier    (1000)       59 2024-05-06 15:59:45.000000 moviesampler-1.1/moviesampler/__init__.py
-drwxrwxr-x   0 javier    (1000) javier    (1000)        0 2024-05-06 16:33:21.205705 moviesampler-1.1/moviesampler/fonts/
--rw-r--r--   0 javier    (1000) javier    (1000)   208612 2024-05-06 07:21:14.000000 moviesampler-1.1/moviesampler/fonts/3270-Regular.otf
--rw-r--r--   0 javier    (1000) javier    (1000)   201596 2024-05-06 07:20:46.000000 moviesampler-1.1/moviesampler/fonts/3270Condensed-Regular.otf
--rw-rw-r--   0 javier    (1000) javier    (1000)     2396 2024-05-06 15:42:37.000000 moviesampler-1.1/moviesampler/framegrabber.py
--rw-rw-r--   0 javier    (1000) javier    (1000)     4168 2024-05-06 16:31:44.000000 moviesampler-1.1/moviesampler/imagecomposer.py
--rw-rw-r--   0 javier    (1000) javier    (1000)     3213 2024-05-06 08:42:18.000000 moviesampler-1.1/moviesampler/main.py
-drwxrwxr-x   0 javier    (1000) javier    (1000)        0 2024-05-06 16:33:21.205705 moviesampler-1.1/moviesampler.egg-info/
--rw-r--r--   0 javier    (1000) javier    (1000)     2264 2024-05-06 16:33:21.000000 moviesampler-1.1/moviesampler.egg-info/PKG-INFO
--rw-rw-r--   0 javier    (1000) javier    (1000)      436 2024-05-06 16:33:21.000000 moviesampler-1.1/moviesampler.egg-info/SOURCES.txt
--rw-rw-r--   0 javier    (1000) javier    (1000)        1 2024-05-06 16:33:21.000000 moviesampler-1.1/moviesampler.egg-info/dependency_links.txt
--rw-rw-r--   0 javier    (1000) javier    (1000)       56 2024-05-06 16:33:21.000000 moviesampler-1.1/moviesampler.egg-info/entry_points.txt
--rw-rw-r--   0 javier    (1000) javier    (1000)       10 2024-05-06 16:33:21.000000 moviesampler-1.1/moviesampler.egg-info/requires.txt
--rw-rw-r--   0 javier    (1000) javier    (1000)       44 2024-05-06 16:33:21.000000 moviesampler-1.1/moviesampler.egg-info/top_level.txt
--rw-rw-r--   0 javier    (1000) javier    (1000)     1284 2024-05-06 10:02:37.000000 moviesampler-1.1/pyproject.toml
--rw-rw-r--   0 javier    (1000) javier    (1000)       38 2024-05-06 16:33:21.205705 moviesampler-1.1/setup.cfg
+drwxrwxr-x   0 javier    (1000) javier    (1000)        0 2024-05-07 07:14:01.498382 moviesampler-1.2/
+-rw-rw-r--   0 javier    (1000) javier    (1000)     3820 2024-05-06 09:15:41.000000 moviesampler-1.2/LICENSE
+-rw-r--r--   0 javier    (1000) javier    (1000)     2264 2024-05-07 07:14:01.498382 moviesampler-1.2/PKG-INFO
+-rw-rw-r--   0 javier    (1000) javier    (1000)     1290 2024-05-06 09:23:13.000000 moviesampler-1.2/README.md
+drwxrwxr-x   0 javier    (1000) javier    (1000)        0 2024-05-07 07:14:01.494383 moviesampler-1.2/moviesampler/
+-rw-rw-r--   0 javier    (1000) javier    (1000)       59 2024-05-07 07:03:29.000000 moviesampler-1.2/moviesampler/__init__.py
+drwxrwxr-x   0 javier    (1000) javier    (1000)        0 2024-05-07 07:14:01.498382 moviesampler-1.2/moviesampler/fonts/
+-rw-r--r--   0 javier    (1000) javier    (1000)   208612 2024-05-06 07:21:14.000000 moviesampler-1.2/moviesampler/fonts/3270-Regular.otf
+-rw-r--r--   0 javier    (1000) javier    (1000)   201596 2024-05-06 07:20:46.000000 moviesampler-1.2/moviesampler/fonts/3270Condensed-Regular.otf
+-rw-rw-r--   0 javier    (1000) javier    (1000)     2396 2024-05-06 15:42:37.000000 moviesampler-1.2/moviesampler/framegrabber.py
+-rw-rw-r--   0 javier    (1000) javier    (1000)     4168 2024-05-06 16:31:44.000000 moviesampler-1.2/moviesampler/imagecomposer.py
+-rw-rw-r--   0 javier    (1000) javier    (1000)     3562 2024-05-07 07:06:01.000000 moviesampler-1.2/moviesampler/main.py
+drwxrwxr-x   0 javier    (1000) javier    (1000)        0 2024-05-07 07:14:01.498382 moviesampler-1.2/moviesampler.egg-info/
+-rw-r--r--   0 javier    (1000) javier    (1000)     2264 2024-05-07 07:14:01.000000 moviesampler-1.2/moviesampler.egg-info/PKG-INFO
+-rw-rw-r--   0 javier    (1000) javier    (1000)      436 2024-05-07 07:14:01.000000 moviesampler-1.2/moviesampler.egg-info/SOURCES.txt
+-rw-rw-r--   0 javier    (1000) javier    (1000)        1 2024-05-07 07:14:01.000000 moviesampler-1.2/moviesampler.egg-info/dependency_links.txt
+-rw-rw-r--   0 javier    (1000) javier    (1000)       56 2024-05-07 07:14:01.000000 moviesampler-1.2/moviesampler.egg-info/entry_points.txt
+-rw-rw-r--   0 javier    (1000) javier    (1000)       10 2024-05-07 07:14:01.000000 moviesampler-1.2/moviesampler.egg-info/requires.txt
+-rw-rw-r--   0 javier    (1000) javier    (1000)       44 2024-05-07 07:14:01.000000 moviesampler-1.2/moviesampler.egg-info/top_level.txt
+-rw-rw-r--   0 javier    (1000) javier    (1000)     1284 2024-05-06 10:02:37.000000 moviesampler-1.2/pyproject.toml
+-rw-rw-r--   0 javier    (1000) javier    (1000)       38 2024-05-07 07:14:01.498382 moviesampler-1.2/setup.cfg
```

### Comparing `moviesampler-1.1/LICENSE` & `moviesampler-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moviesampler-1.1/PKG-INFO` & `moviesampler-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moviesampler
-Version: 1.1
+Version: 1.2
 Summary: Video file thumbnailer
 Author-email: Javier Llopis <javier@llopis.me>
 Project-URL: Repository, https://github.com/destrangis/moviesampler
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `moviesampler-1.1/README.md` & `moviesampler-1.2/README.md`

 * *Files identical despite different names*

### Comparing `moviesampler-1.1/moviesampler/fonts/3270-Regular.otf` & `moviesampler-1.2/moviesampler/fonts/3270-Regular.otf`

 * *Files identical despite different names*

### Comparing `moviesampler-1.1/moviesampler/fonts/3270Condensed-Regular.otf` & `moviesampler-1.2/moviesampler/fonts/3270Condensed-Regular.otf`

 * *Files identical despite different names*

### Comparing `moviesampler-1.1/moviesampler/framegrabber.py` & `moviesampler-1.2/moviesampler/framegrabber.py`

 * *Files identical despite different names*

### Comparing `moviesampler-1.1/moviesampler/imagecomposer.py` & `moviesampler-1.2/moviesampler/imagecomposer.py`

 * *Files identical despite different names*

### Comparing `moviesampler-1.1/moviesampler/main.py` & `moviesampler-1.2/moviesampler/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pathlib
 import time
 import re
 import traceback
 
 from . import version
 from .framegrabber import FrameGrabber
-from .imagecomposer import ImageComposer
+from .imagecomposer import ImageComposer, DEFAULT_FRAME_HEIGHT
 
 NUM_ROWS = 4
 NUM_COLS = 3
 DEFAULT_SUFFIX = "_thumbs"
 GEOM_PATTERN = "(\d+)x(\d+)"
 
 def human_size(size):
@@ -39,14 +39,17 @@
     p.add_argument("--output-dir", "-o", metavar="DIRECTORY", default=".", type=pathlib.Path,
                     help="Directory on which to create the sampler. "
                     "Defaults current working directory")
     p.add_argument("--suffix", "-s", metavar="SUFFIX", default=DEFAULT_SUFFIX,
                     help=f"Suffix for the output file name. Default is '{DEFAULT_SUFFIX}' "
                          "e.g. if the file is named movie1.mp4, the output file will be "
                          "movie1_thumbs.jpg")
+    p.add_argument("--frame-height", "-f", metavar="HEIGHT", default=DEFAULT_FRAME_HEIGHT, type=int,
+                    help="Height of the component videoframes, in pixels. The width will be calculated "
+                         f"from the aspect ratio. Default {DEFAULT_FRAME_HEIGHT}")
     p.add_argument("videofile", nargs="*", type=pathlib.Path, help="Video file to process")
     return p.parse_args(argv)
 
 def get_rows_cols(geometry):
     match = re.search(GEOM_PATTERN, geometry)
     if match:
         rows = int(match.group(1))
@@ -67,15 +70,16 @@
     fg.close()
 
     if frames:
         header = (f"{movie.name} [{human_size(movie_size)}] "
                   f"{fg.str_duration}  {fg.fps} fps {human_size(fg.bit_rate)}ps\n"
                   f"{fg.vcodec_info}\n"
                   f"{fg.acodec_info}")
-        grid_img = ImageComposer(rows, cols, header).build_grid(frames)
+        ic = ImageComposer(rows, cols, header, options.frame_height)
+        grid_img = ic.build_grid(frames)
         outfile = options.output_dir / (movie.stem + options.suffix + ".jpg")
         grid_img.save(str(outfile))
 
 
 def main(argv=None):
     if argv is None:
         argv = sys.argv[1:]
```

### Comparing `moviesampler-1.1/moviesampler.egg-info/PKG-INFO` & `moviesampler-1.2/moviesampler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moviesampler
-Version: 1.1
+Version: 1.2
 Summary: Video file thumbnailer
 Author-email: Javier Llopis <javier@llopis.me>
 Project-URL: Repository, https://github.com/destrangis/moviesampler
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `moviesampler-1.1/pyproject.toml` & `moviesampler-1.2/pyproject.toml`

 * *Files identical despite different names*

