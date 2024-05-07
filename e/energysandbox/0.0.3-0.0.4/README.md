# Comparing `tmp/energysandbox-0.0.3.tar.gz` & `tmp/energysandbox-0.0.4.win-amd64.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energysandbox-0.0.3.tar", last modified: Sun May  5 19:56:55 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

