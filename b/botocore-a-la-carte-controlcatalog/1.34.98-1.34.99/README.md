# Comparing `tmp/botocore-a-la-carte-controlcatalog-1.34.98.tar.gz` & `tmp/botocore_a_la_carte_controlcatalog-1.34.99-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-controlcatalog-1.34.98.tar", last modified: Sat May  4 01:01:21 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

