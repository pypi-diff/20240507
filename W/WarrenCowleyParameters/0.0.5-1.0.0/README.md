# Comparing `tmp/WarrenCowleyParameters-0.0.5.tar.gz` & `tmp/WarrenCowleyParameters-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WarrenCowleyParameters-0.0.5.tar", last modified: Wed Aug 16 23:22:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

