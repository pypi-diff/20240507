# Comparing `tmp/deflate-0.6.0.tar.gz` & `tmp/deflate-0.6.1-cp39-cp39-musllinux_1_1_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deflate-0.6.0.tar", last modified: Fri Apr 19 17:31:07 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

