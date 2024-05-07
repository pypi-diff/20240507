# Comparing `tmp/flashlight_text-0.0.8.dev307.tar.gz` & `tmp/flashlight_text-0.0.8.dev308-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashlight_text-0.0.8.dev307.tar", last modified: Mon May  6 23:18:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

