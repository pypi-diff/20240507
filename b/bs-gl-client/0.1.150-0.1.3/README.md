# Comparing `tmp/bs_gl_client-0.1.150.tar.gz` & `tmp/bs_gl_client-0.1.3-cp37-abi3-manylinux_2_31_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

