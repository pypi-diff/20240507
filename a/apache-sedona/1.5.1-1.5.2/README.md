# Comparing `tmp/apache-sedona-1.5.1.tar.gz` & `tmp/apache_sedona-1.5.2-cp311-cp311-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-sedona-1.5.1.tar", last modified: Wed Jan 17 18:11:20 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

