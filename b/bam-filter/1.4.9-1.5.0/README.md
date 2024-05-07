# Comparing `tmp/bam-filter-1.4.9.tar.gz` & `tmp/bam_filter-1.5.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bam-filter-1.4.9.tar", last modified: Wed May  1 19:56:28 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

