# Comparing `tmp/docprompt-0.4.2.tar.gz` & `tmp/docprompt-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docprompt-0.4.2.tar", max compression
+gzip compressed data, was "docprompt-0.4.3.tar", max compression
```

## Comparing `docprompt-0.4.2.tar` & `docprompt-0.4.3.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.4.2/LICENSE
--rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.4.2/README.md
--rw-r--r--   0        0        0      752 2024-05-06 05:10:41.797238 docprompt-0.4.2/docprompt/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.4.2/docprompt/_exec/__init__.py
--rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.4.2/docprompt/_exec/ghostscript.py
--rw-r--r--   0        0        0      107 2024-05-06 05:10:23.648879 docprompt-0.4.2/docprompt/provenance/__init__.py
--rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.4.2/docprompt/provenance/search.py
--rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.4.2/docprompt/provenance/source.py
--rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.4.2/docprompt/provenance/util.py
--rw-r--r--   0        0        0     7095 2024-04-23 00:30:13.055039 docprompt-0.4.2/docprompt/rasterize.py
--rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.4.2/docprompt/schema/__init__.py
--rw-r--r--   0        0        0     8916 2024-05-04 15:33:18.517588 docprompt-0.4.2/docprompt/schema/document.py
--rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.4.2/docprompt/schema/layout.py
--rw-r--r--   0        0        0     8849 2024-05-06 05:09:04.923864 docprompt-0.4.2/docprompt/schema/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.4.2/docprompt/tasks/__init__.py
--rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.4.2/docprompt/tasks/base.py
--rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.4.2/docprompt/tasks/classification/__init__.py
--rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.4.2/docprompt/tasks/message.py
--rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.4.2/docprompt/tasks/ocr/__init__.py
--rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.4.2/docprompt/tasks/ocr/gcp.py
--rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.4.2/docprompt/tasks/ocr/result.py
--rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.4.2/docprompt/tasks/table_extraction/__init__.py
--rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.4.2/docprompt/tasks/table_extraction/base.py
--rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.4.2/docprompt/tasks/table_extraction/providers/__init__.py
--rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.4.2/docprompt/tasks/table_extraction/providers/claude.py
--rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.4.2/docprompt/tasks/table_extraction/result.py
--rw-r--r--   0        0        0      375 2024-05-04 01:28:27.264357 docprompt-0.4.2/docprompt/utils/__init__.py
--rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.4.2/docprompt/utils/compressor.py
--rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.4.2/docprompt/utils/date_extraction.py
--rw-r--r--   0        0        0        0 2024-04-16 21:31:16.273985 docprompt-0.4.2/docprompt/utils/masking/__init__.py
--rw-r--r--   0        0        0      707 2024-04-17 06:27:28.658476 docprompt-0.4.2/docprompt/utils/masking/image.py
--rw-r--r--   0        0        0     4015 2024-04-13 03:01:14.714377 docprompt-0.4.2/docprompt/utils/splitter.py
--rw-r--r--   0        0        0     4061 2024-05-04 01:28:27.264357 docprompt-0.4.2/docprompt/utils/util.py
--rw-r--r--   0        0        0     4131 2024-05-06 05:10:35.477114 docprompt-0.4.2/pyproject.toml
--rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.4.2/tests/fixtures/1.pdf
--rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.4.2/tests/fixtures/1_ocr.json
--rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.4.2/tests/fixtures.py
--rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.4.2/tests/test_date_extraction.py
--rw-r--r--   0        0        0     5225 2024-05-04 01:28:27.264357 docprompt-0.4.2/tests/test_document.py
--rw-r--r--   0        0        0     1329 2024-05-06 01:10:26.569945 docprompt-0.4.2/tests/test_documentnode.py
--rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.4.2/tests/test_layout_models.py
--rw-r--r--   0        0        0     2517 2024-05-06 01:04:51.295282 docprompt-0.4.2/tests/test_search.py
--rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.4.2/tests/test_threadpool.py
--rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.4.2/tests/util.py
--rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 docprompt-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.4.3/LICENSE
+-rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.4.3/README.md
+-rw-r--r--   0        0        0      752 2024-05-06 23:52:04.333997 docprompt-0.4.3/docprompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.4.3/docprompt/_exec/__init__.py
+-rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.4.3/docprompt/_exec/ghostscript.py
+-rw-r--r--   0        0        0      900 2024-05-06 23:51:36.501689 docprompt-0.4.3/docprompt/_pdfium.py
+-rw-r--r--   0        0        0      107 2024-05-06 05:10:23.648879 docprompt-0.4.3/docprompt/provenance/__init__.py
+-rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.4.3/docprompt/provenance/search.py
+-rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.4.3/docprompt/provenance/source.py
+-rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.4.3/docprompt/provenance/util.py
+-rw-r--r--   0        0        0     7095 2024-04-23 00:30:13.055039 docprompt-0.4.3/docprompt/rasterize.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.4.3/docprompt/schema/__init__.py
+-rw-r--r--   0        0        0     8944 2024-05-06 23:51:36.485689 docprompt-0.4.3/docprompt/schema/document.py
+-rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.4.3/docprompt/schema/layout.py
+-rw-r--r--   0        0        0     8849 2024-05-06 05:09:04.923864 docprompt-0.4.3/docprompt/schema/pipeline.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.4.3/docprompt/tasks/__init__.py
+-rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.4.3/docprompt/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.4.3/docprompt/tasks/classification/__init__.py
+-rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.4.3/docprompt/tasks/message.py
+-rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.4.3/docprompt/tasks/ocr/__init__.py
+-rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.4.3/docprompt/tasks/ocr/gcp.py
+-rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.4.3/docprompt/tasks/ocr/result.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.4.3/docprompt/tasks/table_extraction/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.4.3/docprompt/tasks/table_extraction/base.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.4.3/docprompt/tasks/table_extraction/providers/__init__.py
+-rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.4.3/docprompt/tasks/table_extraction/providers/claude.py
+-rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.4.3/docprompt/tasks/table_extraction/result.py
+-rw-r--r--   0        0        0      375 2024-05-04 01:28:27.264357 docprompt-0.4.3/docprompt/utils/__init__.py
+-rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.4.3/docprompt/utils/compressor.py
+-rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.4.3/docprompt/utils/date_extraction.py
+-rw-r--r--   0        0        0        0 2024-04-16 21:31:16.273985 docprompt-0.4.3/docprompt/utils/masking/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-17 06:27:28.658476 docprompt-0.4.3/docprompt/utils/masking/image.py
+-rw-r--r--   0        0        0     3577 2024-05-06 23:51:36.501689 docprompt-0.4.3/docprompt/utils/splitter.py
+-rw-r--r--   0        0        0     4088 2024-05-06 23:51:36.485689 docprompt-0.4.3/docprompt/utils/util.py
+-rw-r--r--   0        0        0     4177 2024-05-06 23:52:12.446087 docprompt-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.4.3/tests/__init__.py
+-rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.4.3/tests/fixtures/1.pdf
+-rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.4.3/tests/fixtures/1_ocr.json
+-rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.4.3/tests/fixtures.py
+-rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.4.3/tests/test_date_extraction.py
+-rw-r--r--   0        0        0     5225 2024-05-04 01:28:27.264357 docprompt-0.4.3/tests/test_document.py
+-rw-r--r--   0        0        0     1329 2024-05-06 01:10:26.569945 docprompt-0.4.3/tests/test_documentnode.py
+-rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.4.3/tests/test_layout_models.py
+-rw-r--r--   0        0        0     2517 2024-05-06 01:04:51.295282 docprompt-0.4.3/tests/test_search.py
+-rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.4.3/tests/test_threadpool.py
+-rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.4.3/tests/util.py
+-rw-r--r--   0        0        0     7726 1970-01-01 00:00:00.000000 docprompt-0.4.3/PKG-INFO
```

### Comparing `docprompt-0.4.2/LICENSE` & `docprompt-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/README.md` & `docprompt-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/__init__.py` & `docprompt-0.4.3/docprompt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Docprompt."""
 
 __author__ = """Frankie Colson"""
 __email__ = "frank@pageleaf.io"
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 from docprompt.schema.document import Document, PdfDocument  # noqa
 from docprompt.schema.layout import NormBBox, TextBlock  # noqa
 from docprompt.schema.pipeline import DocumentCollection, DocumentNode, PageNode  # noqa
 from docprompt.utils import load_document, load_documents, hash_from_bytes  # noqa
 from docprompt.rasterize import ProviderResizeRatios
```

### Comparing `docprompt-0.4.2/docprompt/_exec/ghostscript.py` & `docprompt-0.4.3/docprompt/_exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/provenance/search.py` & `docprompt-0.4.3/docprompt/provenance/search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/provenance/source.py` & `docprompt-0.4.3/docprompt/provenance/source.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/provenance/util.py` & `docprompt-0.4.3/docprompt/provenance/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/rasterize.py` & `docprompt-0.4.3/docprompt/rasterize.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/schema/document.py` & `docprompt-0.4.3/docprompt/schema/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,53 +7,53 @@
 from io import BytesIO
 from os import PathLike
 from pathlib import Path
 from typing import Dict, Generator, Optional, Tuple, Union, Iterable
 from pydantic import Field
 
 import magic
-import pypdfium2 as pdfium
 from pydantic import (
     BaseModel,
     PositiveInt,
     computed_field,
     field_serializer,
     field_validator,
 )
 
 from docprompt._exec.ghostscript import (
     compress_pdf_to_bytes,
 )
 from docprompt.rasterize import process_raster_image, ResizeModes, AspectRatioRule
 import logging
+from docprompt._pdfium import get_pdfium_document
 
 DEFAULT_DPI = 100
 
 logger = logging.getLogger(__name__)
 
 
 def get_page_render_size_from_bytes(
     file_bytes: bytes, page_number: int, dpi: int = DEFAULT_DPI
 ):
     """
     Returns the render size of a page in pixels
     """
 
-    pdf = pdfium.PdfDocument(BytesIO(file_bytes))
-    page = pdf.get_page(page_number)
+    with get_pdfium_document(file_bytes) as pdf:
+        page = pdf.get_page(page_number)
 
-    mediabox = page.get_mediabox()
+        mediabox = page.get_mediabox()
 
-    base_width = int(mediabox[2] - mediabox[0])
-    base_height = int(mediabox[3] - mediabox[1])
+        base_width = int(mediabox[2] - mediabox[0])
+        base_height = int(mediabox[3] - mediabox[1])
 
-    width = int(base_width * dpi / 72)
-    height = int(base_height * dpi / 72)
+        width = int(base_width * dpi / 72)
+        height = int(base_height * dpi / 72)
 
-    return width, height
+        return width, height
 
 
 class PdfDocument(BaseModel):
     """
     Represents a PDF document
     """
 
@@ -171,20 +171,20 @@
         """
         Rasterizes a page of the document using Pdfium
         """
 
         if page_number < 0 or page_number > self.num_pages:
             raise ValueError(f"Page number must be between 0 and {self.num_pages}")
 
-        pdf = pdfium.PdfDocument(BytesIO(self.file_bytes))
-        page = pdf[page_number - 1]
+        with get_pdfium_document(self.file_bytes) as pdf:
+            page = pdf[page_number - 1]
 
-        bitmap = page.render(scale=(1 / 72) * dpi)
+            bitmap = page.render(scale=(1 / 72) * dpi)
 
-        pil = bitmap.to_pil().convert("RGB")
+            pil = bitmap.to_pil().convert("RGB")
 
         img_bytes = BytesIO()
         pil.save(img_bytes, format="PNG")
         rastered = img_bytes.getvalue()
 
         rastered = process_raster_image(
             rastered,
@@ -244,15 +244,14 @@
 
         result = {}
 
         for page_number in range(1, self.num_pages + 1):
             result[page_number] = self.rasterize_page(
                 page_number,
                 dpi=dpi,
-                use_cache=False,
                 max_file_size_bytes=max_file_size_bytes,
             )
 
         return result
 
     def split(self, start: Optional[int] = None, stop: Optional[int] = None):
         """
```

### Comparing `docprompt-0.4.2/docprompt/schema/layout.py` & `docprompt-0.4.3/docprompt/schema/layout.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/schema/pipeline.py` & `docprompt-0.4.3/docprompt/schema/pipeline.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/tasks/base.py` & `docprompt-0.4.3/docprompt/tasks/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/tasks/message.py` & `docprompt-0.4.3/docprompt/tasks/message.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/tasks/ocr/gcp.py` & `docprompt-0.4.3/docprompt/tasks/ocr/gcp.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/tasks/ocr/result.py` & `docprompt-0.4.3/docprompt/tasks/ocr/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/tasks/table_extraction/base.py` & `docprompt-0.4.3/docprompt/tasks/table_extraction/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/tasks/table_extraction/providers/claude.py` & `docprompt-0.4.3/docprompt/tasks/table_extraction/providers/claude.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/tasks/table_extraction/result.py` & `docprompt-0.4.3/docprompt/tasks/table_extraction/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/utils/date_extraction.py` & `docprompt-0.4.3/docprompt/utils/date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/utils/masking/image.py` & `docprompt-0.4.3/docprompt/utils/masking/image.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/docprompt/utils/splitter.py` & `docprompt-0.4.3/docprompt/utils/splitter.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,48 +3,25 @@
 import tempfile
 from typing import Iterator, Optional
 
 import pypdfium2 as pdfium
 
 from docprompt._exec.ghostscript import compress_pdf_to_bytes
 from docprompt.utils import get_page_count
-from threading import Lock
-import contextlib
 
+from docprompt._pdfium import get_pdfium_document, writable_temp_pdf
 
-logger = logging.getLogger(__name__)
 
-PDFIUM_WRITE_LOCK = Lock()  # Deadlocks occur in threaded environments without this lock
+logger = logging.getLogger(__name__)
 
 
 class UnsupportedDocumentType(ValueError):
     pass
 
 
-@contextlib.contextmanager
-def load_pdf_from_bytes(file_bytes: bytes):
-    pdf = pdfium.PdfDocument(file_bytes)
-
-    try:
-        yield pdf
-    finally:
-        pdf.close()
-
-
-@contextlib.contextmanager
-def writable_temp_pdf():
-    with PDFIUM_WRITE_LOCK:
-        pdf = pdfium.PdfDocument.new()
-
-        try:
-            yield pdf
-        finally:
-            pdf.close()
-
-
 def split_pdf_to_bytes(
     file_bytes: bytes,
     *,
     start_page: Optional[int] = None,
     stop_page: Optional[int] = None,
 ):
     """
@@ -55,15 +32,15 @@
     if stop_page is None:
         stop_page = get_page_count(file_bytes)
 
     if stop_page <= start_page:
         raise ValueError("stop_page must be greater than start_page")
 
     # Load the PDF from bytes
-    with load_pdf_from_bytes(file_bytes) as src_pdf:
+    with get_pdfium_document(file_bytes) as src_pdf:
         # Create a new PDF for the current batch
         dst_pdf = pdfium.PdfDocument.new()
 
         # Append pages to the batch
         dst_pdf.import_pages(src_pdf, list(range(start_page, stop_page)))
 
         # Save the batch PDF to a bytes buffer
@@ -75,15 +52,15 @@
         return pdf_bytes_buffer.getvalue()
 
 
 def pdf_split_iter_fast(file_bytes: bytes, max_page_count: int) -> Iterator[bytes]:
     """
     Splits a PDF into batches of pages up to `max_page_count` pages quickly.
     """
-    with load_pdf_from_bytes(file_bytes) as src_pdf:
+    with get_pdfium_document(file_bytes) as src_pdf:
         current_page = 0
         total_pages = len(src_pdf)
 
         while current_page < total_pages:
             # Determine the last page for the current batch
             last_page = min(current_page + max_page_count, total_pages)
```

### Comparing `docprompt-0.4.2/docprompt/utils/util.py` & `docprompt-0.4.3/docprompt/utils/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from pathlib import Path
 from typing import List, Optional, Union
 from urllib.parse import unquote, urlparse
 import warnings
 
 import fsspec
 import magic
-import pypdfium2 as pdfium
 
 from docprompt.schema.document import PdfDocument
+from docprompt._pdfium import get_pdfium_document
 
 
 def is_pdf(fd: Union[Path, PathLike, bytes]) -> bool:
     """
     Determines if a file is a PDF
     """
     if isinstance(fd, (bytes, str)):
@@ -32,17 +32,16 @@
     """
     Determines the number of pages in a PDF
     """
     if not isinstance(fd, bytes):
         with open(fd, "rb") as f:
             fd = f.read()
 
-    pdf = pdfium.PdfDocument(BytesIO(fd))
-
-    return len(pdf)
+    with get_pdfium_document(fd) as pdf:
+        return len(pdf)
 
 
 def name_from_path(path: Union[Path, PathLike]) -> str:
     if not isinstance(path, Path):
         path = Path(path)
 
     file_name = path.name
@@ -57,17 +56,16 @@
         return f.read()
 
 
 def determine_pdf_name_from_bytes(file_bytes: bytes) -> str:
     """
     Attempts to determine the name of a PDF by exaimining metadata
     """
-    pdf = pdfium.PdfDocument(BytesIO(file_bytes))
-
-    metadata_dict = pdf.get_metadata_dict(skip_empty=True)
+    with get_pdfium_document(file_bytes) as pdf:
+        metadata_dict = pdf.get_metadata_dict(skip_empty=True)
 
     name = None
 
     if metadata_dict:
         name = (
             metadata_dict.get("Title")
             or metadata_dict.get("Subject")
```

### Comparing `docprompt-0.4.2/pyproject.toml` & `docprompt-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "docprompt"
-version = "0.4.2"
+version = "0.4.3"
 homepage = "https://github.com/Page-Leaf/docprompt"
 description = "Documents and large language models."
 authors = ["Frankie Colson <frank@pageleaf.io>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -13,14 +13,15 @@
     'License :: OSI Approved :: Apache Software License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
 ]
 packages = [
     { include = "docprompt" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `docprompt-0.4.2/tests/fixtures/1.pdf` & `docprompt-0.4.3/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/tests/fixtures/1_ocr.json` & `docprompt-0.4.3/tests/fixtures/1_ocr.json`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/tests/test_date_extraction.py` & `docprompt-0.4.3/tests/test_date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/tests/test_document.py` & `docprompt-0.4.3/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/tests/test_documentnode.py` & `docprompt-0.4.3/tests/test_documentnode.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/tests/test_layout_models.py` & `docprompt-0.4.3/tests/test_layout_models.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/tests/test_search.py` & `docprompt-0.4.3/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/tests/test_threadpool.py` & `docprompt-0.4.3/tests/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/tests/util.py` & `docprompt-0.4.3/tests/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.2/PKG-INFO` & `docprompt-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: docprompt
-Version: 0.4.2
+Version: 0.4.3
 Summary: Documents and large language models.
 Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0
 Author: Frankie Colson
 Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: azure
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: google
 Provides-Extra: search
 Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,51 +1,51 @@
-Metadata-Version: 2.1 Name: docprompt Version: 0.4.2 Summary: Documents and
+Metadata-Version: 2.1 Name: docprompt Version: 0.4.3 Summary: Documents and
 large language models. Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0 Author: Frankie Colson Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.8 Provides-Extra: azure Provides-Extra: dev Provides-Extra: doc
-Provides-Extra: google Provides-Extra: search Provides-Extra: test Requires-
-Dist: azure-ai-formrecognizer (>=3.3.0) ; extra == "azure" Requires-Dist:
-bump2version (>=1.0.1,<2.0.0) ; extra == "dev" Requires-Dist: flake8
-(>=6.1.0,<7.0.0) ; extra == "test" Requires-Dist: flake8-docstrings
-(>=1.7.0,<2.0.0) ; extra == "test" Requires-Dist: fsspec (>=2022.11.0)
-Requires-Dist: google-cloud-documentai (>=2.20.0) ; extra == "google" Requires-
-Dist: isort (>=5.12.0,<6.0.0) ; extra == "test" Requires-Dist: mkdocs
-(>=1.1.2,<2.0.0) ; extra == "doc" Requires-Dist: mkdocs-autorefs
-(>=0.2.1,<0.3.0) ; extra == "doc" Requires-Dist: mkdocs-include-markdown-plugin
-(>=1.0.0,<2.0.0) ; extra == "doc" Requires-Dist: mkdocs-material
-(>=6.1.7,<7.0.0) ; extra == "doc" Requires-Dist: mkdocs-material-extensions
-(>=1.0.1,<2.0.0) Requires-Dist: mkdocstrings (>=0.15.2,<0.16.0) ; extra ==
-"doc" Requires-Dist: mypy (>=1.6.1,<2.0.0) ; extra == "test" Requires-Dist:
-networkx (>=2.8.8) ; extra == "search" Requires-Dist: numpy (>=1.20.3,<2.0.0)
-Requires-Dist: pillow (>=9.0.1) Requires-Dist: pip (>=20.3.1,<21.0.0) ; extra
-== "dev" Requires-Dist: pre-commit (>=2.12.0,<3.0.0) ; extra == "dev" Requires-
-Dist: pydantic (>=2.1.0) Requires-Dist: pypdfium2 (>=4.28.0,<5.0.0) Requires-
-Dist: pytest (>=7.4.2,<8.0.0) ; extra == "test" Requires-Dist: pytest-cov
-(>=4.1.0,<5.0.0) ; extra == "test" Requires-Dist: python-dateutil
-(>=2.8.2,<3.0.0) Requires-Dist: python-magic (>=0.4.24) Requires-Dist:
-rapidfuzz (>=3.0.0) Requires-Dist: rtree (>=1.2.0,<2.0.0) ; extra == "search"
-Requires-Dist: ruff (>=0.3.3,<0.4.0) ; extra == "test" Requires-Dist: tantivy
-(>=0.21.0,<0.22.0) ; extra == "search" Requires-Dist: tenacity (>=7.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev" Requires-Dist: tox
-(>=3.20.1,<4.0.0) ; extra == "dev" Requires-Dist: tqdm (>=4.61.0) Requires-
-Dist: twine (>=3.3.0,<4.0.0) ; extra == "dev" Requires-Dist: virtualenv
-(>=20.2.2,<21.0.0) ; extra == "dev" Description-Content-Type: text/markdown [!
-[pypi](https://img.shields.io/pypi/v/docprompt.svg)](https://pypi.org/project/
-docprompt/) [![python](https://img.shields.io/pypi/pyversions/docprompt.svg)]
-(https://pypi.org/project/docprompt/) [![Build Status](https://github.com/Page-
-Leaf/Docprompt/actions/workflows/dev.yml/badge.svg)](https://github.com/Page-
-Leaf/docprompt/actions/workflows/dev.yml) [![codecov](https://codecov.io/gh/
-Page-Leaf/Docprompt/branch/main/graphs/badge.svg)](https://codecov.io/github/
-Page-Leaf/Docprompt)
+Python :: 3.12 Classifier: Programming Language :: Python :: 3.8 Provides-
+Extra: azure Provides-Extra: dev Provides-Extra: doc Provides-Extra: google
+Provides-Extra: search Provides-Extra: test Requires-Dist: azure-ai-
+formrecognizer (>=3.3.0) ; extra == "azure" Requires-Dist: bump2version
+(>=1.0.1,<2.0.0) ; extra == "dev" Requires-Dist: flake8 (>=6.1.0,<7.0.0) ;
+extra == "test" Requires-Dist: flake8-docstrings (>=1.7.0,<2.0.0) ; extra ==
+"test" Requires-Dist: fsspec (>=2022.11.0) Requires-Dist: google-cloud-
+documentai (>=2.20.0) ; extra == "google" Requires-Dist: isort
+(>=5.12.0,<6.0.0) ; extra == "test" Requires-Dist: mkdocs (>=1.1.2,<2.0.0) ;
+extra == "doc" Requires-Dist: mkdocs-autorefs (>=0.2.1,<0.3.0) ; extra == "doc"
+Requires-Dist: mkdocs-include-markdown-plugin (>=1.0.0,<2.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-material (>=6.1.7,<7.0.0) ; extra == "doc" Requires-Dist:
+mkdocs-material-extensions (>=1.0.1,<2.0.0) Requires-Dist: mkdocstrings
+(>=0.15.2,<0.16.0) ; extra == "doc" Requires-Dist: mypy (>=1.6.1,<2.0.0) ;
+extra == "test" Requires-Dist: networkx (>=2.8.8) ; extra == "search" Requires-
+Dist: numpy (>=1.20.3,<2.0.0) Requires-Dist: pillow (>=9.0.1) Requires-Dist:
+pip (>=20.3.1,<21.0.0) ; extra == "dev" Requires-Dist: pre-commit
+(>=2.12.0,<3.0.0) ; extra == "dev" Requires-Dist: pydantic (>=2.1.0) Requires-
+Dist: pypdfium2 (>=4.28.0,<5.0.0) Requires-Dist: pytest (>=7.4.2,<8.0.0) ;
+extra == "test" Requires-Dist: pytest-cov (>=4.1.0,<5.0.0) ; extra == "test"
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: python-magic
+(>=0.4.24) Requires-Dist: rapidfuzz (>=3.0.0) Requires-Dist: rtree
+(>=1.2.0,<2.0.0) ; extra == "search" Requires-Dist: ruff (>=0.3.3,<0.4.0) ;
+extra == "test" Requires-Dist: tantivy (>=0.21.0,<0.22.0) ; extra == "search"
+Requires-Dist: tenacity (>=7.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) ;
+extra == "dev" Requires-Dist: tox (>=3.20.1,<4.0.0) ; extra == "dev" Requires-
+Dist: tqdm (>=4.61.0) Requires-Dist: twine (>=3.3.0,<4.0.0) ; extra == "dev"
+Requires-Dist: virtualenv (>=20.2.2,<21.0.0) ; extra == "dev" Description-
+Content-Type: text/markdown [![pypi](https://img.shields.io/pypi/v/
+docprompt.svg)](https://pypi.org/project/docprompt/) [![python](https://
+img.shields.io/pypi/pyversions/docprompt.svg)](https://pypi.org/project/
+docprompt/) [![Build Status](https://github.com/Page-Leaf/Docprompt/actions/
+workflows/dev.yml/badge.svg)](https://github.com/Page-Leaf/docprompt/actions/
+workflows/dev.yml) [![codecov](https://codecov.io/gh/Page-Leaf/Docprompt/
+branch/main/graphs/badge.svg)](https://codecov.io/github/Page-Leaf/Docprompt)
                                     _[_L_o_g_o_]
                               ******** DDooccpprroommpptt ********
                         Document AI, powered by LLM's
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                        Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 # About Docprompt is a library for Document AI. It aims to make enterprise-
```

