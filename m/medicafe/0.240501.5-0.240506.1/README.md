# Comparing `tmp/medicafe-0.240501.5.tar.gz` & `tmp/medicafe-0.240506.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240501.5.tar", last modified: Thu May  2 03:08:46 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

