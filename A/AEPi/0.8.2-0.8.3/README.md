# Comparing `tmp/AEPi-0.8.2.tar.gz` & `tmp/aepi-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AEPi-0.8.2.tar", last modified: Sat Mar 23 22:17:02 2024, max compression
+gzip compressed data, was "aepi-0.8.3.tar", last modified: Tue May  7 20:43:19 2024, max compression
```

## Comparing `AEPi-0.8.2.tar` & `aepi-0.8.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 22:17:02.350268 AEPi-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-23 22:16:49.000000 AEPi-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-03-23 22:17:02.350268 AEPi-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8742 2024-03-23 22:16:49.000000 AEPi-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-23 22:16:49.000000 AEPi-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-23 22:17:02.350268 AEPi-0.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 22:17:02.346267 AEPi-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 22:17:02.350268 AEPi-0.8.2/src/AEPi/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/codec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 22:17:02.350268 AEPi-0.8.2/src/AEPi/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/codecs/EtcPakCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/codecs/RawCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/codecs/Tex2ImgCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 22:17:02.350268 AEPi-0.8.2/src/AEPi/image/
--rw-r--r--   0 runner    (1001) docker     (127)    18996 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/image/AEI.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/image/texture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 22:17:02.350268 AEPi-0.8.2/src/AEPi/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/lib/binaryio.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/lib/imageOps.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-23 22:16:49.000000 AEPi-0.8.2/src/AEPi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 22:17:02.350268 AEPi-0.8.2/src/AEPi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-03-23 22:17:02.000000 AEPi-0.8.2/src/AEPi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-23 22:17:02.000000 AEPi-0.8.2/src/AEPi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 22:17:02.000000 AEPi-0.8.2/src/AEPi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-23 22:17:02.000000 AEPi-0.8.2/src/AEPi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-23 22:17:02.000000 AEPi-0.8.2/src/AEPi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:43:19.119432 aepi-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 20:43:09.000000 aepi-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-05-07 20:43:19.119432 aepi-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8742 2024-05-07 20:43:09.000000 aepi-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-07 20:43:09.000000 aepi-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-07 20:43:19.119432 aepi-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:43:19.115432 aepi-0.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:43:19.115432 aepi-0.8.3/src/AEPi/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/codec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:43:19.119432 aepi-0.8.3/src/AEPi/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/codecs/EtcPakCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/codecs/RawCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/codecs/Tex2ImgCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:43:19.119432 aepi-0.8.3/src/AEPi/image/
+-rw-r--r--   0 runner    (1001) docker     (127)    18996 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/image/AEI.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/image/texture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:43:19.119432 aepi-0.8.3/src/AEPi/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/lib/binaryio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/lib/imageOps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 20:43:09.000000 aepi-0.8.3/src/AEPi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:43:19.119432 aepi-0.8.3/src/AEPi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-05-07 20:43:19.000000 aepi-0.8.3/src/AEPi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-07 20:43:19.000000 aepi-0.8.3/src/AEPi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:43:19.000000 aepi-0.8.3/src/AEPi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 20:43:19.000000 aepi-0.8.3/src/AEPi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 20:43:19.000000 aepi-0.8.3/src/AEPi.egg-info/top_level.txt
```

### Comparing `AEPi-0.8.2/LICENSE` & `aepi-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AEPi-0.8.2/PKG-INFO` & `aepi-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AEPi
-Version: 0.8.2
+Version: 0.8.3
 Summary: Read and write Abyss Engine Image (AEI) files from python, for Galaxy on Fire 2
 Home-page: https://github.com/Trimatix/AEPi
 Author: Jasper Law
 Author-email: trimatix.music@gmail.com
 Project-URL: Bug Tracker, https://github.com/Trimatix/AEPi/issues
 Keywords: game,python,galaxy-on-fire,image-compression,image-conversion,game-mod-tool,abyss-engine
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AEPi Version: 0.8.2 Summary: Read and write Abyss
+Metadata-Version: 2.1 Name: AEPi Version: 0.8.3 Summary: Read and write Abyss
 Engine Image (AEI) files from python, for Galaxy on Fire 2 Home-page: https://
 github.com/Trimatix/AEPi Author: Jasper Law Author-email:
 trimatix.music@gmail.com Project-URL: Bug Tracker, https://github.com/Trimatix/
 AEPi/issues Keywords: game,python,galaxy-on-fire,image-compression,image-
 conversion,game-mod-tool,abyss-engine Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `AEPi-0.8.2/README.md` & `aepi-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `AEPi-0.8.2/pyproject.toml` & `aepi-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `AEPi-0.8.2/setup.cfg` & `aepi-0.8.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `AEPi-0.8.2/src/AEPi/codec.py` & `aepi-0.8.3/src/AEPi/codec.py`

 * *Files identical despite different names*

### Comparing `AEPi-0.8.2/src/AEPi/codecs/EtcPakCodec.py` & `aepi-0.8.3/src/AEPi/codecs/EtcPakCodec.py`

 * *Files identical despite different names*

### Comparing `AEPi-0.8.2/src/AEPi/codecs/RawCodec.py` & `aepi-0.8.3/src/AEPi/codecs/RawCodec.py`

 * *Files identical despite different names*

### Comparing `AEPi-0.8.2/src/AEPi/codecs/Tex2ImgCodec.py` & `aepi-0.8.3/src/AEPi/codecs/Tex2ImgCodec.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     raise DependancyMissingException("Tex2ImgCodec", "tex2img", e)
 
 TEX2IMG_FORMAT_MAP = {
     # CompressionFormat.PVRTC14A: 12, # Tex2ImgCodec segfaults decoding PVRTC with all tests (#29)
     CompressionFormat.ATC: 14,
     CompressionFormat.DXT1: 5,
     CompressionFormat.DXT5: 6,
-    CompressionFormat.ETC1: 0
+    CompressionFormat.ETC1: 0,
+    CompressionFormat.ETC2: 3
 }
 
 
 @supportsFormats(decompresses=TEX2IMG_FORMAT_MAP.keys())
 class Tex2ImgCodec(ImageCodecAdaptor):
     @classmethod
     def decompress(cls, fp: bytes, format: CompressionFormat, width: int, height: int, quality: Optional[CompressionQuality]) -> Image.Image:
```

### Comparing `AEPi-0.8.2/src/AEPi/constants.py` & `aepi-0.8.3/src/AEPi/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Literal, Dict, Set, Tuple
 from .lib.binaryio import Endianness
 from . import exceptions 
 
 FORMAT_PILLOW_MODES: Dict["CompressionFormat", str] = {}
 FORMAT_BITCOUNTS: Dict["CompressionFormat", int] = {}
 BGRA_FORMATS: Set["CompressionFormat"] = set()
+MIPMAPPABLE_FORMATS: Set["CompressionFormat"] = set()
 MASK_MIPMAPPED_FLAG = 0b00000010
 MASK_FORMAT_ID = 0b11111101
 
 class CompressionFormat(Enum):
     """Compression formats.
     Enum values correspond to the identifiers used within AEI files.
     """
@@ -21,19 +22,20 @@
     PVRTC12A =                  0b00001101
     PVRTC14A =                  0b00010000
     ATC =                       0b00010001
     DXT1 =                      0b00100000
     DXT3 =                      0b00100001
     DXT5 =                      0b00100100
     ETC1 =                      0b01000000
+    ETC2 =                      0b00010111
 
 
     @classmethod
     def fromBinary(cls, rawId: int) -> Tuple["CompressionFormat", bool]:
-        # Some non-mipmappable formats (uncompressed) have the mipmapping flag as 1, just as part of their ID
+        # Some non-mipmappable formats have the mipmapping flag as 1, just as part of their ID
         if any(f.value == rawId for f in CompressionFormat):
             return CompressionFormat(rawId), False
         
         mipmapped = rawId & MASK_MIPMAPPED_FLAG == 2
         id = rawId & MASK_FORMAT_ID
         
         if not any(f.value == id for f in CompressionFormat):
@@ -61,15 +63,15 @@
     def bitcount(self):
         return FORMAT_BITCOUNTS[self]
     
     
     @property
     def supportsMipmapping(self):
         # This will need some more testing to validate
-        return self.isCompressed
+        return self in MIPMAPPABLE_FORMATS
     
     
     @property
     def isBgra(self):
         return self in BGRA_FORMATS
 
 
@@ -80,25 +82,36 @@
 FORMAT_PILLOW_MODES[CompressionFormat.PVRTC12A] = "RGBA"
 FORMAT_PILLOW_MODES[CompressionFormat.PVRTC14A] = "RGBA"
 FORMAT_PILLOW_MODES[CompressionFormat.ATC] = "RGBA"
 FORMAT_PILLOW_MODES[CompressionFormat.DXT1] = "RGB"
 FORMAT_PILLOW_MODES[CompressionFormat.DXT3] = "RGBA"
 FORMAT_PILLOW_MODES[CompressionFormat.DXT5] = "RGBA"
 FORMAT_PILLOW_MODES[CompressionFormat.ETC1] = "RGB"
+FORMAT_PILLOW_MODES[CompressionFormat.ETC2] = "RGBA"
 
 FORMAT_BITCOUNTS[CompressionFormat.Uncompressed] = 8 # ?
 FORMAT_BITCOUNTS[CompressionFormat.Uncompressed_UI] = 8 # ?
 FORMAT_BITCOUNTS[CompressionFormat.Uncompressed_CubeMap_PC] = 8 # ?
 FORMAT_BITCOUNTS[CompressionFormat.Uncompressed_CubeMap] = 8 # ?
 FORMAT_BITCOUNTS[CompressionFormat.PVRTC12A] = 2
 FORMAT_BITCOUNTS[CompressionFormat.PVRTC14A] = 4
 FORMAT_BITCOUNTS[CompressionFormat.ATC] = 4
 FORMAT_BITCOUNTS[CompressionFormat.DXT1] = 4
 FORMAT_BITCOUNTS[CompressionFormat.DXT3] = 8
 FORMAT_BITCOUNTS[CompressionFormat.DXT5] = 8
 FORMAT_BITCOUNTS[CompressionFormat.ETC1] = 4
+FORMAT_BITCOUNTS[CompressionFormat.ETC2] = 8 # ?
 
 BGRA_FORMATS.add(CompressionFormat.ETC1)
+BGRA_FORMATS.add(CompressionFormat.ETC2)
+
+MIPMAPPABLE_FORMATS.add(CompressionFormat.PVRTC12A)
+MIPMAPPABLE_FORMATS.add(CompressionFormat.PVRTC14A)
+MIPMAPPABLE_FORMATS.add(CompressionFormat.ATC)
+MIPMAPPABLE_FORMATS.add(CompressionFormat.DXT1)
+MIPMAPPABLE_FORMATS.add(CompressionFormat.DXT3)
+MIPMAPPABLE_FORMATS.add(CompressionFormat.DXT5)
+MIPMAPPABLE_FORMATS.add(CompressionFormat.ETC1)
 
 FILE_TYPE_HEADER = b"AEimage\x00"
 ENDIANNESS = Endianness("little", "<")
 CompressionQuality = Literal[1, 2, 3]
```

### Comparing `AEPi-0.8.2/src/AEPi/exceptions.py` & `aepi-0.8.3/src/AEPi/exceptions.py`

 * *Files identical despite different names*

### Comparing `AEPi-0.8.2/src/AEPi/image/AEI.py` & `aepi-0.8.3/src/AEPi/image/AEI.py`

 * *Files identical despite different names*

### Comparing `AEPi-0.8.2/src/AEPi/image/texture.py` & `aepi-0.8.3/src/AEPi/image/texture.py`

 * *Files identical despite different names*

### Comparing `AEPi-0.8.2/src/AEPi/lib/binaryio.py` & `aepi-0.8.3/src/AEPi/lib/binaryio.py`

 * *Files identical despite different names*

### Comparing `AEPi-0.8.2/src/AEPi/lib/imageOps.py` & `aepi-0.8.3/src/AEPi/lib/imageOps.py`

 * *Files identical despite different names*

### Comparing `AEPi-0.8.2/src/AEPi.egg-info/PKG-INFO` & `aepi-0.8.3/src/AEPi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AEPi
-Version: 0.8.2
+Version: 0.8.3
 Summary: Read and write Abyss Engine Image (AEI) files from python, for Galaxy on Fire 2
 Home-page: https://github.com/Trimatix/AEPi
 Author: Jasper Law
 Author-email: trimatix.music@gmail.com
 Project-URL: Bug Tracker, https://github.com/Trimatix/AEPi/issues
 Keywords: game,python,galaxy-on-fire,image-compression,image-conversion,game-mod-tool,abyss-engine
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AEPi Version: 0.8.2 Summary: Read and write Abyss
+Metadata-Version: 2.1 Name: AEPi Version: 0.8.3 Summary: Read and write Abyss
 Engine Image (AEI) files from python, for Galaxy on Fire 2 Home-page: https://
 github.com/Trimatix/AEPi Author: Jasper Law Author-email:
 trimatix.music@gmail.com Project-URL: Bug Tracker, https://github.com/Trimatix/
 AEPi/issues Keywords: game,python,galaxy-on-fire,image-compression,image-
 conversion,game-mod-tool,abyss-engine Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `AEPi-0.8.2/src/AEPi.egg-info/SOURCES.txt` & `aepi-0.8.3/src/AEPi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

