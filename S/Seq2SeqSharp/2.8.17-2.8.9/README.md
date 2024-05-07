# Comparing `tmp/Seq2SeqSharp-2.8.17.tar.gz` & `tmp/Seq2SeqSharp-2.8.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Works/Projects/Seq2SeqSharp/PyPackage/dist/.tmp-m0f2onn4/Seq2SeqSharp-2.8.17.tar", last modified: Tue May  7 20:20:46 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

