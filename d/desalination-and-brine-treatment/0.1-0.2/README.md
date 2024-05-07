# Comparing `tmp/desalination_and_brine_treatment-0.1.tar.gz` & `tmp/desalination_and_brine_treatment-0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desalination_and_brine_treatment-0.1.tar", last modified: Tue May  7 07:13:38 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

