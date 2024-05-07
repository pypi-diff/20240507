# Comparing `tmp/rebound-4.4.0.tar.gz` & `tmp/rebound-4.4.1-cp37-cp37m-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rebound-4.4.0.tar", last modified: Tue May  7 13:54:54 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

