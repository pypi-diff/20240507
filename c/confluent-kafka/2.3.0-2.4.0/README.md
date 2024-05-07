# Comparing `tmp/confluent-kafka-2.3.0.tar.gz` & `tmp/confluent_kafka-2.4.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confluent-kafka-2.3.0.tar", last modified: Wed Oct 25 18:25:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

