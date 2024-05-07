# Comparing `tmp/novita_client-0.5.4.tar.gz` & `tmp/novita_client-0.5.5.tar.gz`

## Comparing `novita_client-0.5.4.tar` & `novita_client-0.5.5.tar`

### file list

```diff
@@ -1,63 +1,65 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 novita_client-0.5.4/.python-version
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 novita_client-0.5.4/Makefile
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 novita_client-0.5.4/generate-readme.sh
--rw-r--r--   0        0        0    88494 2020-02-02 00:00:00.000000 novita_client-0.5.4/image.jpg
--rw-r--r--   0        0        0   101219 2020-02-02 00:00:00.000000 novita_client-0.5.4/image1 copy.jpg
--rw-r--r--   0        0        0    35406 2020-02-02 00:00:00.000000 novita_client-0.5.4/image1.jpg
--rw-r--r--   0        0        0    97725 2020-02-02 00:00:00.000000 novita_client-0.5.4/image2.jpg
--rw-r--r--   0        0        0   696352 2020-02-02 00:00:00.000000 novita_client-0.5.4/img2img-controlnet.png
--rw-r--r--   0        0        0   288795 2020-02-02 00:00:00.000000 novita_client-0.5.4/img2img-logo.png
--rw-r--r--   0        0        0   159522 2020-02-02 00:00:00.000000 novita_client-0.5.4/img2img.png
--rw-r--r--   0        0        0   195126 2020-02-02 00:00:00.000000 novita_client-0.5.4/instantid.png
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 novita_client-0.5.4/logo.py
--rw-r--r--   0        0        0   583721 2020-02-02 00:00:00.000000 novita_client-0.5.4/outpainting.png
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 novita_client-0.5.4/ow.py
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 novita_client-0.5.4/requirements-dev.lock
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 novita_client-0.5.4/requirements.lock
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 novita_client-0.5.4/shanginn.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 novita_client-0.5.4/susubot.py
--rw-r--r--   0        0        0   382237 2020-02-02 00:00:00.000000 novita_client-0.5.4/test.mp4
--rw-r--r--   0        0        0   490142 2020-02-02 00:00:00.000000 novita_client-0.5.4/test.png
--rw-r--r--   0        0        0  2297297 2020-02-02 00:00:00.000000 novita_client-0.5.4/txt2img-lora-compare.png
--rw-r--r--   0        0        0   711146 2020-02-02 00:00:00.000000 novita_client-0.5.4/txt2img_with_hiresfix.png
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/cleanup.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/controlnet.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/create-tile.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/doodle.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/img2img.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/img2video.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/instantid.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/latent-consistency-txt2img.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/lcm-img2img.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/lcm-vs-txt2img.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/make-photo.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/merge-face.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/mixpose.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/model-search.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/outpainting.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/reimagine.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/remove-background.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/remove-text.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/replace-background.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/replace-object.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/replace-sky.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/txt2img-with-hiresfix.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/txt2img-with-lora.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/txt2img-with-refiner.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/fixtures/qrcode.png
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/exceptions.py
--rw-r--r--   0        0        0    45566 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/novita.py
--rw-r--r--   0        0        0    37956 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/proto.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/serializer.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/settings.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/utils.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/version.py
--rw-r--r--   0        0        0    12841 2020-02-02 00:00:00.000000 novita_client-0.5.4/tests/test_basics.py
--rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 novita_client-0.5.4/tests/test_enhance.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 novita_client-0.5.4/tests/test_model.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 novita_client-0.5.4/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 novita_client-0.5.4/LICENSE
--rw-r--r--   0        0        0    22761 2020-02-02 00:00:00.000000 novita_client-0.5.4/README.md
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 novita_client-0.5.4/pyproject.toml
--rw-r--r--   0        0        0    24574 2020-02-02 00:00:00.000000 novita_client-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 novita_client-0.5.5/.python-version
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 novita_client-0.5.5/Makefile
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 novita_client-0.5.5/generate-readme.sh
+-rw-r--r--   0        0        0    88494 2020-02-02 00:00:00.000000 novita_client-0.5.5/image.jpg
+-rw-r--r--   0        0        0   101219 2020-02-02 00:00:00.000000 novita_client-0.5.5/image1 copy.jpg
+-rw-r--r--   0        0        0    35406 2020-02-02 00:00:00.000000 novita_client-0.5.5/image1.jpg
+-rw-r--r--   0        0        0    97725 2020-02-02 00:00:00.000000 novita_client-0.5.5/image2.jpg
+-rw-r--r--   0        0        0   696352 2020-02-02 00:00:00.000000 novita_client-0.5.5/img2img-controlnet.png
+-rw-r--r--   0        0        0   288795 2020-02-02 00:00:00.000000 novita_client-0.5.5/img2img-logo.png
+-rw-r--r--   0        0        0   159522 2020-02-02 00:00:00.000000 novita_client-0.5.5/img2img.png
+-rw-r--r--   0        0        0   195126 2020-02-02 00:00:00.000000 novita_client-0.5.5/instantid.png
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 novita_client-0.5.5/logo.py
+-rw-r--r--   0        0        0   583721 2020-02-02 00:00:00.000000 novita_client-0.5.5/outpainting.png
+-rw-r--r--   0        0        0    79016 2020-02-02 00:00:00.000000 novita_client-0.5.5/output.jpg
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 novita_client-0.5.5/ow.py
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 novita_client-0.5.5/requirements-dev.lock
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 novita_client-0.5.5/requirements.lock
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 novita_client-0.5.5/shanginn.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 novita_client-0.5.5/susubot-v3.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 novita_client-0.5.5/susubot.py
+-rw-r--r--   0        0        0   382237 2020-02-02 00:00:00.000000 novita_client-0.5.5/test.mp4
+-rw-r--r--   0        0        0   490142 2020-02-02 00:00:00.000000 novita_client-0.5.5/test.png
+-rw-r--r--   0        0        0  2297297 2020-02-02 00:00:00.000000 novita_client-0.5.5/txt2img-lora-compare.png
+-rw-r--r--   0        0        0   711146 2020-02-02 00:00:00.000000 novita_client-0.5.5/txt2img_with_hiresfix.png
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/cleanup.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/controlnet.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/create-tile.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/doodle.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/img2img.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/img2video.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/instantid.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/latent-consistency-txt2img.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/lcm-img2img.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/lcm-vs-txt2img.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/make-photo.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/merge-face.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/mixpose.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/model-search.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/outpainting.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/reimagine.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/remove-background.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/remove-text.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/replace-background.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/replace-object.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/replace-sky.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/txt2img-with-hiresfix.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/txt2img-with-lora.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/txt2img-with-refiner.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 novita_client-0.5.5/examples/fixtures/qrcode.png
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 novita_client-0.5.5/src/novita_client/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 novita_client-0.5.5/src/novita_client/exceptions.py
+-rw-r--r--   0        0        0    47713 2020-02-02 00:00:00.000000 novita_client-0.5.5/src/novita_client/novita.py
+-rw-r--r--   0        0        0    37791 2020-02-02 00:00:00.000000 novita_client-0.5.5/src/novita_client/proto.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 novita_client-0.5.5/src/novita_client/serializer.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 novita_client-0.5.5/src/novita_client/settings.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 novita_client-0.5.5/src/novita_client/utils.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 novita_client-0.5.5/src/novita_client/version.py
+-rw-r--r--   0        0        0    12841 2020-02-02 00:00:00.000000 novita_client-0.5.5/tests/test_basics.py
+-rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 novita_client-0.5.5/tests/test_enhance.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 novita_client-0.5.5/tests/test_model.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 novita_client-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 novita_client-0.5.5/LICENSE
+-rw-r--r--   0        0        0    22761 2020-02-02 00:00:00.000000 novita_client-0.5.5/README.md
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 novita_client-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0    24574 2020-02-02 00:00:00.000000 novita_client-0.5.5/PKG-INFO
```

### Comparing `novita_client-0.5.4/generate-readme.sh` & `novita_client-0.5.5/generate-readme.sh`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/image.jpg` & `novita_client-0.5.5/image.jpg`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/image1 copy.jpg` & `novita_client-0.5.5/image1 copy.jpg`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/image1.jpg` & `novita_client-0.5.5/image1.jpg`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/image2.jpg` & `novita_client-0.5.5/image2.jpg`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/img2img-controlnet.png` & `novita_client-0.5.5/img2img-controlnet.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/img2img-logo.png` & `novita_client-0.5.5/img2img-logo.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/img2img.png` & `novita_client-0.5.5/img2img.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/instantid.png` & `novita_client-0.5.5/instantid.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/logo.py` & `novita_client-0.5.5/logo.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/outpainting.png` & `novita_client-0.5.5/outpainting.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/ow.py` & `novita_client-0.5.5/ow.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/requirements-dev.lock` & `novita_client-0.5.5/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/shanginn.py` & `novita_client-0.5.5/shanginn.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/susubot.py` & `novita_client-0.5.5/susubot.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/test.mp4` & `novita_client-0.5.5/test.mp4`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/test.png` & `novita_client-0.5.5/test.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/txt2img-lora-compare.png` & `novita_client-0.5.5/txt2img-lora-compare.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/txt2img_with_hiresfix.png` & `novita_client-0.5.5/txt2img_with_hiresfix.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/examples/cleanup.py` & `novita_client-0.5.5/examples/cleanup.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/examples/controlnet.py` & `novita_client-0.5.5/examples/controlnet.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/examples/img2img.py` & `novita_client-0.5.5/examples/img2img.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/examples/instantid.py` & `novita_client-0.5.5/examples/instantid.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/examples/latent-consistency-txt2img.py` & `novita_client-0.5.5/examples/latent-consistency-txt2img.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/examples/lcm-vs-txt2img.py` & `novita_client-0.5.5/examples/lcm-vs-txt2img.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/examples/make-photo.py` & `novita_client-0.5.5/examples/make-photo.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/examples/model-search.py` & `novita_client-0.5.5/examples/model-search.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/examples/txt2img-with-hiresfix.py` & `novita_client-0.5.5/examples/txt2img-with-hiresfix.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/examples/txt2img-with-lora.py` & `novita_client-0.5.5/examples/txt2img-with-lora.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/examples/txt2img-with-refiner.py` & `novita_client-0.5.5/examples/txt2img-with-refiner.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/examples/fixtures/qrcode.png` & `novita_client-0.5.5/examples/fixtures/qrcode.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/src/novita_client/novita.py` & `novita_client-0.5.5/src/novita_client/novita.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,44 +287,90 @@
         Returns:
             UpscaleResponse: An object containing the task status and the URL of the upscaled image.
         """
         response = self._post('/v2/upscale', request.to_dict())
 
         return UpscaleResponse.from_dict(response)
 
-    def adetailer(self, model_name: str, image: InputImage, prompt: str, steps=None, strength=None, negative_prompt=None, vae=None, seed=None, clip_skip=None,  download_images=True, callback: callable = None) -> ProgressResponse:
-        response = self.async_adetailer(model_name, image, prompt, steps, strength, negative_prompt, vae, seed, clip_skip)
-        if response.data is None:
-            raise NovitaResponseError(f"Upscale failed with response {response.msg}, code: {response.code}")
-
-        res = self.wait_for_task(response.data.task_id, callback=callback)
-        if download_images:
-            res.download_images()
-        return res
+    def raw_adetailer(self, req: ADETailerRequest, extra: CommonV3Extra = None) -> ADETailerResponse:
+        _req = CommonV3Request(request=req, extra=extra)
 
-    def async_adetailer(self, model_name: str, image: InputImage, prompt: str, steps=None, strength=None, negative_prompt=None, vae=None, seed=None, clip_skip=None) -> ProgressResponse:
-        image_b64 = input_image_to_base64(image)
-        request = ADETailerRequest(
+        return ADETailerResponse.from_dict(self._post('/v3/async/adetailer', _req.to_dict()))
+
+    def adetailer(self, model_name: str, input_images: List[InputImage], prompt: str, sampler_name=None, guidance_scale=None, steps=None, strength=None, loras: List[ADETailerLoRA] = None, embeddings: List[ADETailerEmbedding] = None, negative_prompt=None, sd_vae=None, seed=None, clip_skip=None,  download_images=True, callback: callable = None) -> V3TaskResponse:
+        req = ADETailerRequest(
             model_name=model_name,
-            input_image=image_b64,
             prompt=prompt,
         )
         if steps is not None:
-            request.steps = steps
+            req.steps = steps
         if strength is not None:
-            request.strength = strength
+            req.strength = strength
         if negative_prompt is not None:
-            request.negative_prompt = negative_prompt
-        if vae is not None:
-            request.vae = vae
+            req.negative_prompt = negative_prompt
+        if sd_vae is not None:
+            req.sd_vae = sd_vae
         if seed is not None:
-            request.seed = seed
+            req.seed = seed
         if clip_skip is not None:
-            request.clip_skip = clip_skip
-        return ADETailerResponse.from_dict(self._post('/v2/adetailer', request.to_dict()))
+            req.clip_skip = clip_skip
+        if loras is not None:
+            req.loras = loras
+        if embeddings is not None:
+            req.embeddings = embeddings
+        if guidance_scale is not None:
+            req.guidance_scale = guidance_scale
+        if sampler_name is not None:
+            req.sampler_name = sampler_name
+
+        mode = "assets"  # or assets
+        for input_image in input_images:
+            if isinstance(input_image, str) and input_image.startswith("https://faas-output-image"):
+                mode = "s3_url"
+                break
+
+        if mode == "assets":
+            req.image_assets_ids = self.upload_assets([input_image_to_base64(image) for image in input_images])
+        else:
+            req.image_urls = input_images
+
+        res = self.raw_adetailer(req)
+
+        return self.wait_for_task_v3(res.task_id, callback=callback)
+
+        # def adetailer(self, model_name: str, image: InputImage, prompt: str, steps=None, strength=None, negative_prompt=None, vae=None, seed=None, clip_skip=None,  download_images=True, callback: callable = None) -> ProgressResponse:
+        #     response = self.async_adetailer(model_name, image, prompt, steps, strength, negative_prompt, vae, seed, clip_skip)
+        #     if response.data is None:
+        #         raise NovitaResponseError(f"Upscale failed with response {response.msg}, code: {response.code}")
+
+        #     res = self.wait_for_task(response.data.task_id, callback=callback)
+        #     if download_images:
+        #         res.download_images()
+        #     return res
+
+        # def async_adetailer(self, model_name: str, image: InputImage, prompt: str, steps=None, strength=None, negative_prompt=None, vae=None, seed=None, clip_skip=None) -> ProgressResponse:
+        #     image_b64 = input_image_to_base64(image)
+        #     request = ADETailerRequest(
+        #         model_name=model_name,
+        #         input_image=image_b64,
+        #         prompt=prompt,
+        #     )
+        #     if steps is not None:
+        #         request.steps = steps
+        #     if strength is not None:
+        #         request.strength = strength
+        #     if negative_prompt is not None:
+        #         request.negative_prompt = negative_prompt
+        #     if vae is not None:
+        #         request.vae = vae
+        #     if seed is not None:
+        #         request.seed = seed
+        #     if clip_skip is not None:
+        #         request.clip_skip = clip_skip
+        #     return ADETailerResponse.from_dict(self._post('/v2/adetailer', request.to_dict()))
 
     def cleanup(self, image: InputImage, mask: InputImage, response_image_type=None) -> CleanupResponse:
         image_b64 = input_image_to_base64(image)
         mask_b64 = input_image_to_base64(mask)
         request = CleanupRequest(image_file=image_b64, mask_file=mask_b64)
         if response_image_type is None:
             request.set_image_type(self._default_response_image_type)
```

### Comparing `novita_client-0.5.4/src/novita_client/proto.py` & `novita_client-0.5.5/src/novita_client/proto.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,15 @@
 
 @dataclass
 class Img2ImgExtra(JSONe):
     enable_nsfw_detection: bool = False
     nsfw_detection_level: int = 0
     enable_progress_info: bool = True
 
+
 @dataclass
 class Img2ImgRequest(JSONe):
     model_name: str = 'dreamshaper_5BakedVae.safetensors'
     sampler_name: str = None
     init_images: List[str] = None
     mask: Optional[str] = None
     resize_mode: Optional[int] = 0
@@ -794,59 +795,46 @@
 @dataclass
 class LCMTxt2ImgResponse(JSONe):
     images: List[LCMTxt2ImgResponseImage]
 
 # --------------- ADEtailer ---------------
 
 
-class ADETailerResponseCode(Enum):
-    NORMAL = 0
-    INTERNAL_ERROR = -1
-    INVALID_JSON = 1
-    MODEL_NOT_EXISTS = 2
-    TASK_ID_NOT_EXISTS = 3
-    INVALID_AUTH = 4
-    HOST_UNAVAILABLE = 5
-    PARAM_RANGE_ERROR = 6
-    COST_BALANCE_ERROR = 7
-    SAMPLER_NOT_EXISTS = 8
-    TIMEOUT = 9
+@dataclass
+class ADETailerLoRA(JSONe):
+    model_name: str
+    strength: Optional[float] = 1.0
 
-    UNKNOWN = 100
 
-    @classmethod
-    def _missing_(cls, number):
-        return cls(cls.UNKNOWN)
+@dataclass
+class ADETailerEmbedding(JSONe):
+    model_name: str
 
 
 @dataclass
 class ADETailerRequest(JSONe):
     model_name: str
-    input_image: str
     prompt: str
+    image_assets_ids: List[str] = None
+    image_urls: List[str] = None
+    loras: List[ADETailerLoRA] = None
+    embeddings: List[ADETailerEmbedding] = None
+    guidance_scale: Optional[float] = 7.5
+    sampler_name: Optional[str] = Samplers.DPMPP_KARRAS
     steps: Optional[int] = 20
     strength: Optional[float] = 0.3
     negative_prompt: Optional[str] = None
-    vae: Optional[str] = None
+    sd_vae: Optional[str] = None
     seed: Optional[int] = None
     clip_skip: Optional[int] = None
 
 
 @dataclass
-class ADETailerResponseData(JSONe):
-    task_id: str
-    warn: Optional[str] = None
-
-
-@dataclass
 class ADETailerResponse(JSONe):
-    code: ADETailerResponseCode
-    msg: str
-    data: Optional[ADETailerResponseData] = None
-
+    task_id: str
 
 # --------------- Training ---------------
 
 
 @dataclass
 class UploadAssetRequest(JSONe):
     file_extension: str = "png"
```

### Comparing `novita_client-0.5.4/src/novita_client/utils.py` & `novita_client-0.5.5/src/novita_client/utils.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/tests/test_basics.py` & `novita_client-0.5.5/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/tests/test_enhance.py` & `novita_client-0.5.5/tests/test_enhance.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/tests/test_model.py` & `novita_client-0.5.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/.gitignore` & `novita_client-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/LICENSE` & `novita_client-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/README.md` & `novita_client-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.4/pyproject.toml` & `novita_client-0.5.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "novita_client"
-version = "0.5.4"
+version = "0.5.5"
 description = "novita SDK for Python"
 authors = [
     { name = "novita", email = "novitalabs@gmail.com" }
 ]
 
 
 dependencies = [
```

### Comparing `novita_client-0.5.4/PKG-INFO` & `novita_client-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: novita_client
-Version: 0.5.4
+Version: 0.5.5
 Summary: novita SDK for Python
 Project-URL: Homepage, https://github.com/novita/python-sdk
 Project-URL: Bug Tracker, https://discord.gg/nzqq8UScpx
 Author-email: novita <novitalabs@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 novita.ai
```

