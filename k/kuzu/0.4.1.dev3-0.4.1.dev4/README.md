# Comparing `tmp/kuzu-0.4.1.dev3.tar.gz` & `tmp/kuzu-0.4.1.dev4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.4.1.dev3.tar", last modified: Mon May  6 08:04:44 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

