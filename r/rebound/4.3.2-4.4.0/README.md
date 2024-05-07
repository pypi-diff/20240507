# Comparing `tmp/rebound-4.3.2.tar.gz` & `tmp/rebound-4.4.0-cp310-cp310-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rebound-4.3.2.tar", last modified: Mon Feb 19 16:13:28 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

