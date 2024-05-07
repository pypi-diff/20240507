# Comparing `tmp/csp-cryspy-1.2.3.tar.gz` & `tmp/csp_cryspy-1.2.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csp-cryspy-1.2.3.tar", last modified: Sat Oct 21 10:15:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

