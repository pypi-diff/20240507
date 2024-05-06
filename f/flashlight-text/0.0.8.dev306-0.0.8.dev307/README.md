# Comparing `tmp/flashlight_text-0.0.8.dev306.tar.gz` & `tmp/flashlight_text-0.0.8.dev307-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashlight_text-0.0.8.dev306.tar", last modified: Fri Apr 19 18:46:35 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

