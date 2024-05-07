# Comparing `tmp/ngstoolkits-1.0.0rc2.tar.gz` & `tmp/ngstoolkits-1.0.0rc3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/liubo/git_sync/ngstoolkits/dist/.tmp-h06qxnah/ngstoolkits-1.0.0rc2.tar", last modified: Mon May  6 09:39:08 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

