# Comparing `tmp/libsps-1.0.1.tar.gz` & `tmp/libsps-1.1.1-cp39-cp39-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsps-1.0.1.tar", last modified: Tue Oct 24 13:05:47 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

