# Comparing `tmp/indusmes-0.0.5.tar.gz` & `tmp/indusmes-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indusmes-0.0.5.tar", last modified: Mon Apr 29 06:31:14 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

