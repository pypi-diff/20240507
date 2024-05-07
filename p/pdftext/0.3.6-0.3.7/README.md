# Comparing `tmp/pdftext-0.3.6.tar.gz` & `tmp/pdftext-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdftext-0.3.6.tar", max compression
+gzip compressed data, was "pdftext-0.3.7.tar", max compression
```

## Comparing `pdftext-0.3.6.tar` & `pdftext-0.3.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11269 2024-05-06 17:27:02.808858 pdftext-0.3.6/LICENSE
--rw-r--r--   0        0        0     7170 2024-05-06 17:27:02.808858 pdftext-0.3.6/README.md
--rw-r--r--   0        0        0     1726 2024-05-06 17:27:02.808858 pdftext-0.3.6/extract_text.py
--rw-r--r--   0        0        0    14097 2024-05-06 17:27:02.808858 pdftext-0.3.6/models/dt.joblib
--rw-r--r--   0        0        0     2426 2024-05-06 17:27:02.808858 pdftext-0.3.6/pdftext/extraction.py
--rw-r--r--   0        0        0     7212 2024-05-06 17:27:02.812858 pdftext-0.3.6/pdftext/inference.py
--rw-r--r--   0        0        0      153 2024-05-06 17:27:02.812858 pdftext-0.3.6/pdftext/model.py
--rw-r--r--   0        0        0     3877 2024-05-06 17:27:02.812858 pdftext-0.3.6/pdftext/pdf/chars.py
--rw-r--r--   0        0        0     4613 2024-05-06 17:27:02.812858 pdftext-0.3.6/pdftext/pdf/utils.py
--rw-r--r--   0        0        0     3222 2024-05-06 17:27:02.812858 pdftext-0.3.6/pdftext/postprocessing.py
--rw-r--r--   0        0        0      488 2024-05-06 17:27:02.812858 pdftext-0.3.6/pdftext/settings.py
--rw-r--r--   0        0        0      856 2024-05-06 17:27:02.812858 pdftext-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     8146 1970-01-01 00:00:00.000000 pdftext-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11269 2024-05-07 20:14:47.002582 pdftext-0.3.7/LICENSE
+-rw-r--r--   0        0        0     7170 2024-05-07 20:14:47.002582 pdftext-0.3.7/README.md
+-rw-r--r--   0        0        0     1726 2024-05-07 20:14:47.002582 pdftext-0.3.7/extract_text.py
+-rw-r--r--   0        0        0    14097 2024-05-07 20:14:47.002582 pdftext-0.3.7/models/dt.joblib
+-rw-r--r--   0        0        0     2426 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/extraction.py
+-rw-r--r--   0        0        0     7382 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/inference.py
+-rw-r--r--   0        0        0      153 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/model.py
+-rw-r--r--   0        0        0     3880 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/pdf/chars.py
+-rw-r--r--   0        0        0     4613 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/pdf/utils.py
+-rw-r--r--   0        0        0     3222 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/postprocessing.py
+-rw-r--r--   0        0        0      488 2024-05-07 20:14:47.002582 pdftext-0.3.7/pdftext/settings.py
+-rw-r--r--   0        0        0      856 2024-05-07 20:14:47.002582 pdftext-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     8146 1970-01-01 00:00:00.000000 pdftext-0.3.7/PKG-INFO
```

### Comparing `pdftext-0.3.6/LICENSE` & `pdftext-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.6/README.md` & `pdftext-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.6/extract_text.py` & `pdftext-0.3.7/extract_text.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.6/models/dt.joblib` & `pdftext-0.3.7/models/dt.joblib`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.6/pdftext/extraction.py` & `pdftext-0.3.7/pdftext/extraction.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.6/pdftext/inference.py` & `pdftext-0.3.7/pdftext/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,17 @@
             training_row = create_training_row(char_info, prev_char, block, line)
             sorted_keys = sorted(training_row.keys())
             training_row = [training_row[key] for key in sorted_keys]
 
             prediction_probs = yield training_row
             # First item is probability of same line/block, second is probability of new line, third is probability of new block
             if prediction_probs[0] >= .5:
-                pass
+                # Ensure we update spans properly for font info when predicting no new line
+                if prev_font_info != font_info:
+                    span = update_span(line, span)
             elif prediction_probs[2] > block_threshold:
                 span = update_span(line, span)
                 line = update_line(block, line)
                 block = update_block(blocks, block)
             elif prev_char["char"] in LINE_BREAKS: # Look for newline character as a forcing signal for a new line
                 span = update_span(line, span)
                 line = update_line(block, line)
```

### Comparing `pdftext-0.3.6/pdftext/pdf/chars.py` & `pdftext-0.3.7/pdftext/pdf/chars.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 prev_fontflags = fontflags
                 fontname, fontflags = get_fontname(text_page, i)
                 if (fontname != prev_fontname or fontflags != prev_fontflags) and i > 0:
                     update_previous_fonts(text_chars, i, prev_fontname, prev_fontflags, text_page, fontname_sample_freq)
 
             rotation = pdfium_c.FPDFText_GetCharAngle(text_page, i)
             rotation = rotation * 180 / math.pi # convert from radians to degrees
-            coords = text_page.get_charbox(i, loose=rotation == 0) # Loose doesn't work properly when page is rotated
+            coords = text_page.get_charbox(i, loose=rotation == 0) # Loose doesn't work properly when charbox is rotated
             device_coords = page_bbox_to_device_bbox(page, coords, page_width, page_height, bl_origin, page_rotation, normalize=True)
 
             char_info = {
                 "font": {
                     "size": fontsize,
                     "weight": fontweight,
                     "name": fontname,
```

### Comparing `pdftext-0.3.6/pdftext/pdf/utils.py` & `pdftext-0.3.7/pdftext/pdf/utils.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.6/pdftext/postprocessing.py` & `pdftext-0.3.7/pdftext/postprocessing.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.6/pyproject.toml` & `pdftext-0.3.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdftext"
-version = "0.3.6"
+version = "0.3.7"
 description = "Extract structured text from pdfs quickly"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/VikParuchuri/pdftext"
 keywords = ["pdf", "text", "extraction"]
 packages = [
```

### Comparing `pdftext-0.3.6/PKG-INFO` & `pdftext-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftext
-Version: 0.3.6
+Version: 0.3.7
 Summary: Extract structured text from pdfs quickly
 Home-page: https://github.com/VikParuchuri/pdftext
 License: Apache-2.0
 Keywords: pdf,text,extraction
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
```

