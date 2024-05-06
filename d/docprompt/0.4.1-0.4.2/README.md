# Comparing `tmp/docprompt-0.4.1.tar.gz` & `tmp/docprompt-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docprompt-0.4.1.tar", max compression
+gzip compressed data, was "docprompt-0.4.2.tar", max compression
```

## Comparing `docprompt-0.4.1.tar` & `docprompt-0.4.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.4.1/LICENSE
--rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.4.1/README.md
--rw-r--r--   0        0        0      752 2024-05-06 01:13:33.499643 docprompt-0.4.1/docprompt/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.4.1/docprompt/_exec/__init__.py
--rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.4.1/docprompt/_exec/ghostscript.py
--rw-r--r--   0        0        0        0 2024-03-18 23:40:35.967506 docprompt-0.4.1/docprompt/provenance/__init__.py
--rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.4.1/docprompt/provenance/search.py
--rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.4.1/docprompt/provenance/source.py
--rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.4.1/docprompt/provenance/util.py
--rw-r--r--   0        0        0     7095 2024-04-23 00:30:13.055039 docprompt-0.4.1/docprompt/rasterize.py
--rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.4.1/docprompt/schema/__init__.py
--rw-r--r--   0        0        0     8916 2024-05-04 15:33:18.517588 docprompt-0.4.1/docprompt/schema/document.py
--rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.4.1/docprompt/schema/layout.py
--rw-r--r--   0        0        0     8585 2024-05-06 01:07:35.940590 docprompt-0.4.1/docprompt/schema/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.4.1/docprompt/tasks/__init__.py
--rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.4.1/docprompt/tasks/base.py
--rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.4.1/docprompt/tasks/classification/__init__.py
--rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.4.1/docprompt/tasks/message.py
--rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.4.1/docprompt/tasks/ocr/__init__.py
--rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.4.1/docprompt/tasks/ocr/gcp.py
--rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.4.1/docprompt/tasks/ocr/result.py
--rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.4.1/docprompt/tasks/table_extraction/__init__.py
--rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.4.1/docprompt/tasks/table_extraction/base.py
--rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.4.1/docprompt/tasks/table_extraction/providers/__init__.py
--rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.4.1/docprompt/tasks/table_extraction/providers/claude.py
--rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.4.1/docprompt/tasks/table_extraction/result.py
--rw-r--r--   0        0        0      375 2024-05-04 01:28:27.264357 docprompt-0.4.1/docprompt/utils/__init__.py
--rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.4.1/docprompt/utils/compressor.py
--rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.4.1/docprompt/utils/date_extraction.py
--rw-r--r--   0        0        0        0 2024-04-16 21:31:16.273985 docprompt-0.4.1/docprompt/utils/masking/__init__.py
--rw-r--r--   0        0        0      707 2024-04-17 06:27:28.658476 docprompt-0.4.1/docprompt/utils/masking/image.py
--rw-r--r--   0        0        0     4015 2024-04-13 03:01:14.714377 docprompt-0.4.1/docprompt/utils/splitter.py
--rw-r--r--   0        0        0     4061 2024-05-04 01:28:27.264357 docprompt-0.4.1/docprompt/utils/util.py
--rw-r--r--   0        0        0     4131 2024-05-06 01:13:20.571235 docprompt-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.4.1/tests/fixtures/1.pdf
--rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.4.1/tests/fixtures/1_ocr.json
--rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.4.1/tests/fixtures.py
--rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.4.1/tests/test_date_extraction.py
--rw-r--r--   0        0        0     5225 2024-05-04 01:28:27.264357 docprompt-0.4.1/tests/test_document.py
--rw-r--r--   0        0        0     1329 2024-05-06 01:10:26.569945 docprompt-0.4.1/tests/test_documentnode.py
--rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.4.1/tests/test_layout_models.py
--rw-r--r--   0        0        0     2517 2024-05-06 01:04:51.295282 docprompt-0.4.1/tests/test_search.py
--rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.4.1/tests/test_threadpool.py
--rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.4.1/tests/util.py
--rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 docprompt-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.4.2/README.md
+-rw-r--r--   0        0        0      752 2024-05-06 05:10:41.797238 docprompt-0.4.2/docprompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.4.2/docprompt/_exec/__init__.py
+-rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.4.2/docprompt/_exec/ghostscript.py
+-rw-r--r--   0        0        0      107 2024-05-06 05:10:23.648879 docprompt-0.4.2/docprompt/provenance/__init__.py
+-rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.4.2/docprompt/provenance/search.py
+-rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.4.2/docprompt/provenance/source.py
+-rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.4.2/docprompt/provenance/util.py
+-rw-r--r--   0        0        0     7095 2024-04-23 00:30:13.055039 docprompt-0.4.2/docprompt/rasterize.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.4.2/docprompt/schema/__init__.py
+-rw-r--r--   0        0        0     8916 2024-05-04 15:33:18.517588 docprompt-0.4.2/docprompt/schema/document.py
+-rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.4.2/docprompt/schema/layout.py
+-rw-r--r--   0        0        0     8849 2024-05-06 05:09:04.923864 docprompt-0.4.2/docprompt/schema/pipeline.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.4.2/docprompt/tasks/__init__.py
+-rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.4.2/docprompt/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.4.2/docprompt/tasks/classification/__init__.py
+-rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.4.2/docprompt/tasks/message.py
+-rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.4.2/docprompt/tasks/ocr/__init__.py
+-rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.4.2/docprompt/tasks/ocr/gcp.py
+-rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.4.2/docprompt/tasks/ocr/result.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.4.2/docprompt/tasks/table_extraction/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.4.2/docprompt/tasks/table_extraction/base.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.4.2/docprompt/tasks/table_extraction/providers/__init__.py
+-rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.4.2/docprompt/tasks/table_extraction/providers/claude.py
+-rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.4.2/docprompt/tasks/table_extraction/result.py
+-rw-r--r--   0        0        0      375 2024-05-04 01:28:27.264357 docprompt-0.4.2/docprompt/utils/__init__.py
+-rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.4.2/docprompt/utils/compressor.py
+-rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.4.2/docprompt/utils/date_extraction.py
+-rw-r--r--   0        0        0        0 2024-04-16 21:31:16.273985 docprompt-0.4.2/docprompt/utils/masking/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-17 06:27:28.658476 docprompt-0.4.2/docprompt/utils/masking/image.py
+-rw-r--r--   0        0        0     4015 2024-04-13 03:01:14.714377 docprompt-0.4.2/docprompt/utils/splitter.py
+-rw-r--r--   0        0        0     4061 2024-05-04 01:28:27.264357 docprompt-0.4.2/docprompt/utils/util.py
+-rw-r--r--   0        0        0     4131 2024-05-06 05:10:35.477114 docprompt-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.4.2/tests/fixtures/1.pdf
+-rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.4.2/tests/fixtures/1_ocr.json
+-rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.4.2/tests/fixtures.py
+-rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.4.2/tests/test_date_extraction.py
+-rw-r--r--   0        0        0     5225 2024-05-04 01:28:27.264357 docprompt-0.4.2/tests/test_document.py
+-rw-r--r--   0        0        0     1329 2024-05-06 01:10:26.569945 docprompt-0.4.2/tests/test_documentnode.py
+-rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.4.2/tests/test_layout_models.py
+-rw-r--r--   0        0        0     2517 2024-05-06 01:04:51.295282 docprompt-0.4.2/tests/test_search.py
+-rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.4.2/tests/test_threadpool.py
+-rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.4.2/tests/util.py
+-rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 docprompt-0.4.2/PKG-INFO
```

### Comparing `docprompt-0.4.1/LICENSE` & `docprompt-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/README.md` & `docprompt-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/__init__.py` & `docprompt-0.4.2/docprompt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Docprompt."""
 
 __author__ = """Frankie Colson"""
 __email__ = "frank@pageleaf.io"
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 from docprompt.schema.document import Document, PdfDocument  # noqa
 from docprompt.schema.layout import NormBBox, TextBlock  # noqa
 from docprompt.schema.pipeline import DocumentCollection, DocumentNode, PageNode  # noqa
 from docprompt.utils import load_document, load_documents, hash_from_bytes  # noqa
 from docprompt.rasterize import ProviderResizeRatios
```

### Comparing `docprompt-0.4.1/docprompt/_exec/ghostscript.py` & `docprompt-0.4.2/docprompt/_exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/provenance/search.py` & `docprompt-0.4.2/docprompt/provenance/search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/provenance/source.py` & `docprompt-0.4.2/docprompt/provenance/source.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/provenance/util.py` & `docprompt-0.4.2/docprompt/provenance/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/rasterize.py` & `docprompt-0.4.2/docprompt/rasterize.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/schema/document.py` & `docprompt-0.4.2/docprompt/schema/document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/schema/layout.py` & `docprompt-0.4.2/docprompt/schema/layout.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/schema/pipeline.py` & `docprompt-0.4.2/docprompt/schema/pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import (
     Dict,
     Generic,
     Iterable,
     List,
     Literal,
     Optional,
+    Tuple,
     TypeVar,
     TYPE_CHECKING,
     Union,
 )
 
 from pydantic import BaseModel, Field, PositiveInt, PrivateAttr
 
@@ -51,28 +52,30 @@
 
     def rasterize(
         self,
         name: Optional[str] = None,
         *,
         return_mode: Literal["bytes", "pil"] = "bytes",
         dpi: int = 100,
+        downscale_size: Optional[Tuple[int, int]] = None,
         resize_mode: ResizeModes = "thumbnail",
         resize_aspect_ratios: Optional[Iterable[AspectRatioRule]] = None,
         do_convert: bool = False,
         image_convert_mode: str = "L",
         do_quantize: bool = False,
         quantize_color_count: int = 8,
         max_file_size_bytes: Optional[int] = None,
         mask_bounding_boxes: List[NormBBox] = [],
     ) -> Union[bytes, Image.Image]:
         cache_key = (
             name
             if name
             else self._construct_cache_key(
                 dpi=dpi,
+                downscale_size=downscale_size,
                 resize_mode=resize_mode,
                 resize_aspect_ratios=resize_aspect_ratios,
                 do_convert=do_convert,
                 image_covert_mode=image_convert_mode,
                 do_quantize=do_quantize,
                 quantize_color_count=quantize_color_count,
                 max_file_size_bytes=max_file_size_bytes,
@@ -82,14 +85,15 @@
 
         if cache_key in self.raster_cache:
             rastered = self.raster_cache[cache_key]
         else:
             rastered = self.owner.document.document.rasterize_page(
                 self.owner.page_number,
                 dpi=dpi,
+                downscale_size=downscale_size,
                 resize_mode=resize_mode,
                 resize_aspect_ratios=resize_aspect_ratios,
                 do_convert=do_convert,
                 image_covert_mode=image_convert_mode,
                 do_quantize=do_quantize,
                 quantize_color_count=quantize_color_count,
                 max_file_size_bytes=max_file_size_bytes,
@@ -111,27 +115,29 @@
         return rastered
 
     def rasterize_to_data_uri(
         self,
         name: str,
         *,
         dpi: int = 100,
+        downscale_size: Optional[Tuple[int, int]] = None,
         resize_mode: ResizeModes = "thumbnail",
         resize_aspect_ratios: Optional[Iterable[AspectRatioRule]] = None,
         do_convert: bool = False,
         image_convert_mode: str = "L",
         do_quantize: bool = False,
         quantize_color_count: int = 8,
         max_file_size_bytes: Optional[int] = None,
         mask_bounding_boxes: List[NormBBox] = [],
     ) -> str:
         rastered = self.rasterize(
             name,
             return_mode="bytes",
             dpi=dpi,
+            downscale_size=downscale_size,
             resize_mode=resize_mode,
             resize_aspect_ratios=resize_aspect_ratios,
             do_convert=do_convert,
             image_convert_mode=image_convert_mode,
             do_quantize=do_quantize,
             quantize_color_count=quantize_color_count,
             max_file_size_bytes=max_file_size_bytes,
```

### Comparing `docprompt-0.4.1/docprompt/tasks/base.py` & `docprompt-0.4.2/docprompt/tasks/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/tasks/message.py` & `docprompt-0.4.2/docprompt/tasks/message.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/tasks/ocr/gcp.py` & `docprompt-0.4.2/docprompt/tasks/ocr/gcp.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/tasks/ocr/result.py` & `docprompt-0.4.2/docprompt/tasks/ocr/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/tasks/table_extraction/base.py` & `docprompt-0.4.2/docprompt/tasks/table_extraction/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/tasks/table_extraction/providers/claude.py` & `docprompt-0.4.2/docprompt/tasks/table_extraction/providers/claude.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/tasks/table_extraction/result.py` & `docprompt-0.4.2/docprompt/tasks/table_extraction/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/utils/date_extraction.py` & `docprompt-0.4.2/docprompt/utils/date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/utils/masking/image.py` & `docprompt-0.4.2/docprompt/utils/masking/image.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/utils/splitter.py` & `docprompt-0.4.2/docprompt/utils/splitter.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/docprompt/utils/util.py` & `docprompt-0.4.2/docprompt/utils/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/pyproject.toml` & `docprompt-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "docprompt"
-version = "0.4.1"
+version = "0.4.2"
 homepage = "https://github.com/Page-Leaf/docprompt"
 description = "Documents and large language models."
 authors = ["Frankie Colson <frank@pageleaf.io>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `docprompt-0.4.1/tests/fixtures/1.pdf` & `docprompt-0.4.2/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/tests/fixtures/1_ocr.json` & `docprompt-0.4.2/tests/fixtures/1_ocr.json`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/tests/test_date_extraction.py` & `docprompt-0.4.2/tests/test_date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/tests/test_document.py` & `docprompt-0.4.2/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/tests/test_documentnode.py` & `docprompt-0.4.2/tests/test_documentnode.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/tests/test_layout_models.py` & `docprompt-0.4.2/tests/test_layout_models.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/tests/test_search.py` & `docprompt-0.4.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/tests/test_threadpool.py` & `docprompt-0.4.2/tests/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/tests/util.py` & `docprompt-0.4.2/tests/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.1/PKG-INFO` & `docprompt-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docprompt
-Version: 0.4.1
+Version: 0.4.2
 Summary: Documents and large language models.
 Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0
 Author: Frankie Colson
 Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docprompt Version: 0.4.1 Summary: Documents and
+Metadata-Version: 2.1 Name: docprompt Version: 0.4.2 Summary: Documents and
 large language models. Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0 Author: Frankie Colson Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

