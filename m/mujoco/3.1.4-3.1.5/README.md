# Comparing `tmp/mujoco-3.1.4.tar.gz` & `tmp/mujoco-3.1.5-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mujoco-3.1.4.tar", last modified: Wed Apr 10 17:15:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

