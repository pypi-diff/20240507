# Comparing `tmp/AkitaCode-2.0.6.tar.gz` & `tmp/AkitaCode-2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AkitaCode-2.0.6.tar", last modified: Tue May  7 10:02:11 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

