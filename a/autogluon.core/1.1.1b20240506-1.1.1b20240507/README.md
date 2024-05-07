# Comparing `tmp/autogluon.core-1.1.1b20240506.tar.gz` & `tmp/autogluon.core-1.1.1b20240507-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-1.1.1b20240506.tar", last modified: Mon May  6 09:04:13 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

