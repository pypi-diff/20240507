# Comparing `tmp/verovio-4.1.0.tar.gz` & `tmp/verovio-4.2.1-cp310-cp310-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verovio-4.1.0.tar", last modified: Fri Dec 15 10:18:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

