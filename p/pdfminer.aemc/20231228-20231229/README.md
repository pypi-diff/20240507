# Comparing `tmp/pdfminer_aemc-20231228.tar.gz` & `tmp/pdfminer_aemc-20231229.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfminer_aemc-20231228.tar", last modified: Sat May  4 04:32:45 2024, max compression
+gzip compressed data, was "pdfminer_aemc-20231229.tar", last modified: Tue May  7 12:24:06 2024, max compression
```

## Comparing `pdfminer_aemc-20231228.tar` & `pdfminer_aemc-20231229.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.612769 pdfminer_aemc-20231228/
--rw-rw-r--   0 jun        (501) staff       (20)    15840 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/CHANGELOG.md
--rw-rw-r--   0 jun        (501) staff       (20)     2397 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/CONTRIBUTING.md
--rw-rw-r--   0 jun        (501) staff       (20)     1093 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/LICENSE
--rw-rw-r--   0 jun        (501) staff       (20)      160 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/MANIFEST.in
--rw-rw-r--   0 jun        (501) staff       (20)     1141 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/Makefile
--rw-r--r--   0 jun        (501) staff       (20)     4144 2024-05-04 04:32:45.612523 pdfminer_aemc-20231228/PKG-INFO
--rw-rw-r--   0 jun        (501) staff       (20)     2573 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/README.md
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.573107 pdfminer_aemc-20231228/cmaprsrc/
--rw-rw-r--   0 jun        (501) staff       (20)     2917 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/cmaprsrc/README.txt
--rw-rw-r--   0 jun        (501) staff       (20)  2046762 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_CNS1.txt
--rw-rw-r--   0 jun        (501) staff       (20)  1900416 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_GB1.txt
--rw-rw-r--   0 jun        (501) staff       (20)  2681742 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_Japan1.txt
--rw-rw-r--   0 jun        (501) staff       (20)  1028252 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_Korea1.txt
--rw-rw-r--   0 jun        (501) staff       (20)     1310 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/noxfile.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.584051 pdfminer_aemc-20231228/pdfminer/
--rw-rw-r--   0 jun        (501) staff       (20)      196 2024-04-24 11:19:45.000000 pdfminer_aemc-20231228/pdfminer/__init__.py
--rw-rw-r--   0 jun        (501) staff       (20)     3600 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/_saslprep.py
--rw-rw-r--   0 jun        (501) staff       (20)      929 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/arcfour.py
--rw-rw-r--   0 jun        (501) staff       (20)     2097 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/ascii85.py
--rw-rw-r--   0 jun        (501) staff       (20)    21391 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/ccitt.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.606952 pdfminer_aemc-20231228/pdfminer/cmap/
--rw-rw-r--   0 jun        (501) staff       (20)    20532 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    20551 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    19882 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22969 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22990 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    19883 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25942 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78ms-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25964 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/78ms-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    26305 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/83pv-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    26305 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/83pv-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25732 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/90ms-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25757 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/90ms-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25670 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/90msp-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25688 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/90msp-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24226 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/90pv-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24021 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/90pv-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21027 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Add-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24275 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Add-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24079 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Add-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    20874 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Add-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    42594 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    42549 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    42602 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/B5pc-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    42557 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/B5pc-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    56990 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/CNS-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    56943 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/CNS-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    17615 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/CNS1-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    17564 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/CNS1-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21723 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/CNS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21723 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/CNS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    59548 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/ETHK-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    59481 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/ETHK-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    43982 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/ETen-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    43924 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/ETen-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      320 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/ETenms-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      438 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/ETenms-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    20429 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    20455 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22272 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Ext-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25721 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Ext-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25750 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Ext-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22307 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Ext-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22118 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GB-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22111 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GB-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21699 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GB-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21694 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GB-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    68254 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBK-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    68199 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBK-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    89917 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBK2K-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    89872 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBK2K-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    68148 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBKp-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    68102 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBKp-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23815 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBT-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23806 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBT-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23339 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBT-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23322 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBT-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23650 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBTpc-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23647 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBTpc-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21945 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBpc-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21956 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/GBpc-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    19781 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    45212 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKdla-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    45167 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKdla-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    44853 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKdlb-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    44816 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKdlb-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    53104 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKgccs-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    53050 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKgccs-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    43667 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKm314-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    43618 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKm314-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    44187 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKm471-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    44144 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKm471-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    59508 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKscs-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    59473 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/HKscs-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      840 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Hankaku-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      839 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Hankaku-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      391 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Hiragana-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      391 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Hiragana-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24040 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSC-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24078 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSC-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23563 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    55016 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSC-Johab-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    55041 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSC-Johab-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23644 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    51667 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    51788 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    51821 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    51698 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    27769 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSCpc-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    27820 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/KSCpc-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      404 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Katakana-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      404 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Katakana-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21708 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/NWP-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21779 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/NWP-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)     3917 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/README.txt
--rw-rw-r--   0 jun        (501) staff       (20)    23030 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23048 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      394 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Roman-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      394 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/Roman-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    67459 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    67395 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    87819 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    87751 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    87400 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    87327 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    82631 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    82562 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    97445 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UCS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    97441 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UCS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   101459 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   101331 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   101490 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   101357 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    90500 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    90368 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    35934 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      412 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-HW-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)     1402 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    35852 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    58054 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57928 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57910 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57780 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54764 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54684 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    58081 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57960 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57940 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57811 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54829 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54749 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57903 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57778 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57930 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57808 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    60683 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UCS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    60699 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UCS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    61278 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    61298 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    61286 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    61309 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54151 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54172 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    19826 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      505 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/WP-Symbol-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      505 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/WP-Symbol-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   138237 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   204425 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   112987 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   120859 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    16342 2024-04-24 11:07:22.000000 pdfminer_aemc-20231228/pdfminer/cmapdb.py
--rw-rw-r--   0 jun        (501) staff       (20)    35804 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/converter.py
--rw-rw-r--   0 jun        (501) staff       (20)     1654 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/data_structures.py
--rw-rw-r--   0 jun        (501) staff       (20)     3983 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/encodingdb.py
--rw-rw-r--   0 jun        (501) staff       (20)   112611 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/fontmetrics.py
--rw-rw-r--   0 jun        (501) staff       (20)   130804 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/glyphlist.py
--rw-rw-r--   0 jun        (501) staff       (20)     7276 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/high_level.py
--rw-rw-r--   0 jun        (501) staff       (20)     9305 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/image.py
--rw-rw-r--   0 jun        (501) staff       (20)    11391 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/jbig2.py
--rw-rw-r--   0 jun        (501) staff       (20)     8531 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/latin_enc.py
--rw-rw-r--   0 jun        (501) staff       (20)    35926 2024-04-24 11:12:53.000000 pdfminer_aemc-20231228/pdfminer/layout.py
--rw-rw-r--   0 jun        (501) staff       (20)     3177 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/lzw.py
--rw-rw-r--   0 jun        (501) staff       (20)      821 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdfcolor.py
--rw-rw-r--   0 jun        (501) staff       (20)     8787 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdfdevice.py
--rw-rw-r--   0 jun        (501) staff       (20)    37267 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdfdocument.py
--rw-rw-r--   0 jun        (501) staff       (20)    38109 2024-04-24 11:09:47.000000 pdfminer_aemc-20231228/pdfminer/pdffont.py
--rw-rw-r--   0 jun        (501) staff       (20)    34539 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdfinterp.py
--rw-rw-r--   0 jun        (501) staff       (20)     6803 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdfpage.py
--rw-rw-r--   0 jun        (501) staff       (20)     5896 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdfparser.py
--rw-rw-r--   0 jun        (501) staff       (20)    12109 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/pdftypes.py
--rwxr-xr-x   0 jun        (501) staff       (20)    19649 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/psparser.py
--rw-rw-r--   0 jun        (501) staff       (20)        0 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/py.typed
--rw-rw-r--   0 jun        (501) staff       (20)     1358 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/runlength.py
--rw-rw-r--   0 jun        (501) staff       (20)       15 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/settings.py
--rw-rw-r--   0 jun        (501) staff       (20)    20804 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/pdfminer/utils.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.611856 pdfminer_aemc-20231228/pdfminer.aemc.egg-info/
--rw-r--r--   0 jun        (501) staff       (20)     4144 2024-05-04 04:32:45.000000 pdfminer_aemc-20231228/pdfminer.aemc.egg-info/PKG-INFO
--rw-r--r--   0 jun        (501) staff       (20)     6914 2024-05-04 04:32:45.000000 pdfminer_aemc-20231228/pdfminer.aemc.egg-info/SOURCES.txt
--rw-r--r--   0 jun        (501) staff       (20)        1 2024-05-04 04:32:45.000000 pdfminer_aemc-20231228/pdfminer.aemc.egg-info/dependency_links.txt
--rw-r--r--   0 jun        (501) staff       (20)      194 2024-05-04 04:32:45.000000 pdfminer_aemc-20231228/pdfminer.aemc.egg-info/requires.txt
--rw-r--r--   0 jun        (501) staff       (20)        9 2024-05-04 04:32:45.000000 pdfminer_aemc-20231228/pdfminer.aemc.egg-info/top_level.txt
--rw-r--r--   0 jun        (501) staff       (20)       38 2024-05-04 04:32:45.612825 pdfminer_aemc-20231228/setup.cfg
--rw-rw-r--   0 jun        (501) staff       (20)     1980 2024-04-24 11:00:36.000000 pdfminer_aemc-20231228/setup.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.610459 pdfminer_aemc-20231228/tests/
--rw-rw-r--   0 jun        (501) staff       (20)     9692 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_converter.py
--rw-rw-r--   0 jun        (501) staff       (20)     5420 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_encodingdb.py
--rw-rw-r--   0 jun        (501) staff       (20)      779 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_font_size.py
--rw-rw-r--   0 jun        (501) staff       (20)     6451 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_highlevel_extracttext.py
--rw-rw-r--   0 jun        (501) staff       (20)     5038 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_layout.py
--rw-rw-r--   0 jun        (501) staff       (20)     1809 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdfdocument.py
--rw-rw-r--   0 jun        (501) staff       (20)     3972 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdfencoding.py
--rw-rw-r--   0 jun        (501) staff       (20)      604 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdffont.py
--rw-rw-r--   0 jun        (501) staff       (20)     4532 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdfminer_ccitt.py
--rw-rw-r--   0 jun        (501) staff       (20)     1598 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdfminer_crypto.py
--rw-rw-r--   0 jun        (501) staff       (20)     3405 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdfminer_psparser.py
--rw-rw-r--   0 jun        (501) staff       (20)      582 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_pdfpage.py
--rw-rw-r--   0 jun        (501) staff       (20)     1505 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_tools_dumppdf.py
--rw-rw-r--   0 jun        (501) staff       (20)     5497 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_tools_pdf2txt.py
--rw-rw-r--   0 jun        (501) staff       (20)     3912 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tests/test_utils.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-04 04:32:45.611675 pdfminer_aemc-20231228/tools/
--rw-rw-r--   0 jun        (501) staff       (20)        0 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/__init__.py
--rwxr-xr-x   0 jun        (501) staff       (20)     1646 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/conv_afm.py
--rwxr-xr-x   0 jun        (501) staff       (20)     6089 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/conv_cmap.py
--rwxr-xr-x   0 jun        (501) staff       (20)      911 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/conv_glyphlist.py
--rwxr-xr-x   0 jun        (501) staff       (20)    14316 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/dumppdf.py
--rwxr-xr-x   0 jun        (501) staff       (20)     9779 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/pdf2txt.py
--rw-rw-r--   0 jun        (501) staff       (20)     6266 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/pdfdiff.py
--rwxr-xr-x   0 jun        (501) staff       (20)     2761 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/pdfstats.py
--rw-rw-r--   0 jun        (501) staff       (20)     1415 2023-12-28 21:20:33.000000 pdfminer_aemc-20231228/tools/prof.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-07 12:24:06.487707 pdfminer_aemc-20231229/
+-rw-rw-r--   0 jun        (501) staff       (20)    15840 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/CHANGELOG.md
+-rw-rw-r--   0 jun        (501) staff       (20)     2397 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/CONTRIBUTING.md
+-rw-rw-r--   0 jun        (501) staff       (20)     1093 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/LICENSE
+-rw-rw-r--   0 jun        (501) staff       (20)      160 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/MANIFEST.in
+-rw-rw-r--   0 jun        (501) staff       (20)     1141 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/Makefile
+-rw-r--r--   0 jun        (501) staff       (20)     4144 2024-05-07 12:24:06.487466 pdfminer_aemc-20231229/PKG-INFO
+-rw-rw-r--   0 jun        (501) staff       (20)     2573 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/README.md
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-07 12:24:06.447502 pdfminer_aemc-20231229/cmaprsrc/
+-rw-rw-r--   0 jun        (501) staff       (20)     2917 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/cmaprsrc/README.txt
+-rw-rw-r--   0 jun        (501) staff       (20)  2046762 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/cmaprsrc/cid2code_Adobe_CNS1.txt
+-rw-rw-r--   0 jun        (501) staff       (20)  1900416 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/cmaprsrc/cid2code_Adobe_GB1.txt
+-rw-rw-r--   0 jun        (501) staff       (20)  2681742 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/cmaprsrc/cid2code_Adobe_Japan1.txt
+-rw-rw-r--   0 jun        (501) staff       (20)  1028252 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/cmaprsrc/cid2code_Adobe_Korea1.txt
+-rw-rw-r--   0 jun        (501) staff       (20)     1310 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/noxfile.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-07 12:24:06.457686 pdfminer_aemc-20231229/pdfminer/
+-rw-rw-r--   0 jun        (501) staff       (20)      196 2024-05-07 12:21:12.000000 pdfminer_aemc-20231229/pdfminer/__init__.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3600 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/_saslprep.py
+-rw-rw-r--   0 jun        (501) staff       (20)      929 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/arcfour.py
+-rw-rw-r--   0 jun        (501) staff       (20)     2097 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/ascii85.py
+-rw-rw-r--   0 jun        (501) staff       (20)    21391 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/ccitt.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-07 12:24:06.481782 pdfminer_aemc-20231229/pdfminer/cmap/
+-rw-rw-r--   0 jun        (501) staff       (20)    20532 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/78-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    20551 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/78-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    19882 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/78-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22969 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/78-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22990 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/78-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    19883 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/78-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25942 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/78ms-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25964 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/78ms-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    26305 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/83pv-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    26305 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/83pv-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25732 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/90ms-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25757 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/90ms-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25670 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/90msp-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25688 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/90msp-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24226 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/90pv-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24021 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/90pv-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21027 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Add-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24275 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Add-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24079 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Add-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    20874 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Add-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    42594 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    42549 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    42602 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/B5pc-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    42557 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/B5pc-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    56990 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/CNS-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    56943 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/CNS-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    17615 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/CNS1-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    17564 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/CNS1-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21723 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/CNS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21723 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/CNS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    59548 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/ETHK-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    59481 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/ETHK-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    43982 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/ETen-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    43924 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/ETen-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      320 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/ETenms-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      438 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/ETenms-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    20429 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    20455 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22272 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Ext-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25721 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Ext-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25750 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Ext-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22307 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Ext-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22118 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GB-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22111 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GB-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21699 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GB-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21694 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GB-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    68254 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBK-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    68199 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBK-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    89917 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBK2K-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    89872 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBK2K-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    68148 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBKp-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    68102 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBKp-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23815 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBT-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23806 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBT-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23339 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBT-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23322 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBT-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23650 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBTpc-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23647 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBTpc-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21945 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBpc-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21956 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/GBpc-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    19781 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    45212 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/HKdla-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    45167 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/HKdla-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    44853 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/HKdlb-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    44816 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/HKdlb-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    53104 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/HKgccs-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    53050 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/HKgccs-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    43667 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/HKm314-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    43618 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/HKm314-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    44187 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/HKm471-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    44144 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/HKm471-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    59508 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/HKscs-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    59473 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/HKscs-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      840 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Hankaku-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      839 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Hankaku-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      391 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Hiragana-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      391 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Hiragana-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24040 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/KSC-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24078 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/KSC-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23563 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/KSC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    55016 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/KSC-Johab-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    55041 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/KSC-Johab-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23644 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/KSC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    51667 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/KSCms-UHC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    51788 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    51821 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    51698 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/KSCms-UHC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    27769 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/KSCpc-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    27820 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/KSCpc-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      404 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Katakana-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      404 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Katakana-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21708 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/NWP-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21779 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/NWP-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)     3917 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/README.txt
+-rw-rw-r--   0 jun        (501) staff       (20)    23030 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23048 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      394 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Roman-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      394 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/Roman-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    67459 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    67395 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    87819 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    87751 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    87400 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    87327 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    82631 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    82562 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    97445 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UCS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    97441 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UCS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   101459 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   101331 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   101490 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   101357 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    90500 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    90368 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    35934 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      412 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UCS2-HW-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)     1402 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    35852 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    58054 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57928 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57910 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57780 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54764 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54684 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    58081 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57960 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57940 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57811 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54829 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54749 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57903 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57778 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57930 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57808 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    60683 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UCS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    60699 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UCS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    61278 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    61298 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    61286 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    61309 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54151 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54172 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    19826 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      505 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/WP-Symbol-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      505 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/WP-Symbol-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   138237 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   204425 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   112987 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   120859 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    16511 2024-05-07 12:21:04.000000 pdfminer_aemc-20231229/pdfminer/cmapdb.py
+-rw-rw-r--   0 jun        (501) staff       (20)    35804 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/converter.py
+-rw-rw-r--   0 jun        (501) staff       (20)     1654 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/data_structures.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3983 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/encodingdb.py
+-rw-rw-r--   0 jun        (501) staff       (20)   112611 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/fontmetrics.py
+-rw-rw-r--   0 jun        (501) staff       (20)   130804 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/glyphlist.py
+-rw-rw-r--   0 jun        (501) staff       (20)     7276 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/high_level.py
+-rw-rw-r--   0 jun        (501) staff       (20)     9305 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/image.py
+-rw-rw-r--   0 jun        (501) staff       (20)    11391 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/jbig2.py
+-rw-rw-r--   0 jun        (501) staff       (20)     8531 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/latin_enc.py
+-rw-rw-r--   0 jun        (501) staff       (20)    35926 2024-04-24 11:12:53.000000 pdfminer_aemc-20231229/pdfminer/layout.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3177 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/lzw.py
+-rw-rw-r--   0 jun        (501) staff       (20)      821 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/pdfcolor.py
+-rw-rw-r--   0 jun        (501) staff       (20)     8787 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/pdfdevice.py
+-rw-rw-r--   0 jun        (501) staff       (20)    37267 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/pdfdocument.py
+-rw-rw-r--   0 jun        (501) staff       (20)    38109 2024-04-24 11:09:47.000000 pdfminer_aemc-20231229/pdfminer/pdffont.py
+-rw-rw-r--   0 jun        (501) staff       (20)    34539 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/pdfinterp.py
+-rw-rw-r--   0 jun        (501) staff       (20)     6803 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/pdfpage.py
+-rw-rw-r--   0 jun        (501) staff       (20)     5896 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/pdfparser.py
+-rw-rw-r--   0 jun        (501) staff       (20)    12109 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/pdftypes.py
+-rwxr-xr-x   0 jun        (501) staff       (20)    19649 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/psparser.py
+-rw-rw-r--   0 jun        (501) staff       (20)        0 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/py.typed
+-rw-rw-r--   0 jun        (501) staff       (20)     1358 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/runlength.py
+-rw-rw-r--   0 jun        (501) staff       (20)       15 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/settings.py
+-rw-rw-r--   0 jun        (501) staff       (20)    20804 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/pdfminer/utils.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-07 12:24:06.486862 pdfminer_aemc-20231229/pdfminer.aemc.egg-info/
+-rw-r--r--   0 jun        (501) staff       (20)     4144 2024-05-07 12:24:06.000000 pdfminer_aemc-20231229/pdfminer.aemc.egg-info/PKG-INFO
+-rw-r--r--   0 jun        (501) staff       (20)     6914 2024-05-07 12:24:06.000000 pdfminer_aemc-20231229/pdfminer.aemc.egg-info/SOURCES.txt
+-rw-r--r--   0 jun        (501) staff       (20)        1 2024-05-07 12:24:06.000000 pdfminer_aemc-20231229/pdfminer.aemc.egg-info/dependency_links.txt
+-rw-r--r--   0 jun        (501) staff       (20)      194 2024-05-07 12:24:06.000000 pdfminer_aemc-20231229/pdfminer.aemc.egg-info/requires.txt
+-rw-r--r--   0 jun        (501) staff       (20)        9 2024-05-07 12:24:06.000000 pdfminer_aemc-20231229/pdfminer.aemc.egg-info/top_level.txt
+-rw-r--r--   0 jun        (501) staff       (20)       38 2024-05-07 12:24:06.487750 pdfminer_aemc-20231229/setup.cfg
+-rw-rw-r--   0 jun        (501) staff       (20)     1980 2024-04-24 11:00:36.000000 pdfminer_aemc-20231229/setup.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-07 12:24:06.485265 pdfminer_aemc-20231229/tests/
+-rw-rw-r--   0 jun        (501) staff       (20)     9692 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_converter.py
+-rw-rw-r--   0 jun        (501) staff       (20)     5420 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_encodingdb.py
+-rw-rw-r--   0 jun        (501) staff       (20)      779 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_font_size.py
+-rw-rw-r--   0 jun        (501) staff       (20)     6451 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_highlevel_extracttext.py
+-rw-rw-r--   0 jun        (501) staff       (20)     5038 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_layout.py
+-rw-rw-r--   0 jun        (501) staff       (20)     1809 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_pdfdocument.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3972 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_pdfencoding.py
+-rw-rw-r--   0 jun        (501) staff       (20)      604 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_pdffont.py
+-rw-rw-r--   0 jun        (501) staff       (20)     4532 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_pdfminer_ccitt.py
+-rw-rw-r--   0 jun        (501) staff       (20)     1598 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_pdfminer_crypto.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3405 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_pdfminer_psparser.py
+-rw-rw-r--   0 jun        (501) staff       (20)      582 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_pdfpage.py
+-rw-rw-r--   0 jun        (501) staff       (20)     1505 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_tools_dumppdf.py
+-rw-rw-r--   0 jun        (501) staff       (20)     5497 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_tools_pdf2txt.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3912 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tests/test_utils.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-05-07 12:24:06.486681 pdfminer_aemc-20231229/tools/
+-rw-rw-r--   0 jun        (501) staff       (20)        0 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tools/__init__.py
+-rwxr-xr-x   0 jun        (501) staff       (20)     1646 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tools/conv_afm.py
+-rwxr-xr-x   0 jun        (501) staff       (20)     6089 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tools/conv_cmap.py
+-rwxr-xr-x   0 jun        (501) staff       (20)      911 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tools/conv_glyphlist.py
+-rwxr-xr-x   0 jun        (501) staff       (20)    14316 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tools/dumppdf.py
+-rwxr-xr-x   0 jun        (501) staff       (20)     9779 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tools/pdf2txt.py
+-rw-rw-r--   0 jun        (501) staff       (20)     6266 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tools/pdfdiff.py
+-rwxr-xr-x   0 jun        (501) staff       (20)     2761 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tools/pdfstats.py
+-rw-rw-r--   0 jun        (501) staff       (20)     1415 2023-12-28 21:20:33.000000 pdfminer_aemc-20231229/tools/prof.py
```

### Comparing `pdfminer_aemc-20231228/CHANGELOG.md` & `pdfminer_aemc-20231229/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/CONTRIBUTING.md` & `pdfminer_aemc-20231229/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/LICENSE` & `pdfminer_aemc-20231229/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/Makefile` & `pdfminer_aemc-20231229/Makefile`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/PKG-INFO` & `pdfminer_aemc-20231229/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfminer.aemc
-Version: 20231228
+Version: 20231229
 Summary: PDF parser and analyzer
 Home-page: https://github.com/pdfminer/pdfminer.aemc
 Author: Yusuke Shinyama + Philippe Guglielmetti + Liew Chun Fui
 Author-email: wargreymon28@gmail.com
 License: MIT/X
 Keywords: pdf parser,pdf converter,layout analysis,text mining
 Classifier: Programming Language :: Python
```

### Comparing `pdfminer_aemc-20231228/README.md` & `pdfminer_aemc-20231229/README.md`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/cmaprsrc/README.txt` & `pdfminer_aemc-20231229/cmaprsrc/README.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_CNS1.txt` & `pdfminer_aemc-20231229/cmaprsrc/cid2code_Adobe_CNS1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_GB1.txt` & `pdfminer_aemc-20231229/cmaprsrc/cid2code_Adobe_GB1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_Japan1.txt` & `pdfminer_aemc-20231229/cmaprsrc/cid2code_Adobe_Japan1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/cmaprsrc/cid2code_Adobe_Korea1.txt` & `pdfminer_aemc-20231229/cmaprsrc/cid2code_Adobe_Korea1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/noxfile.py` & `pdfminer_aemc-20231229/noxfile.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/_saslprep.py` & `pdfminer_aemc-20231229/pdfminer/_saslprep.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/arcfour.py` & `pdfminer_aemc-20231229/pdfminer/arcfour.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/ascii85.py` & `pdfminer_aemc-20231229/pdfminer/ascii85.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/ccitt.py` & `pdfminer_aemc-20231229/pdfminer/ccitt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/78-EUC-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/78-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/78-EUC-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/78-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/78-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/78-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/78-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/78-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/78-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/78-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/78-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/78-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/78ms-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/78ms-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/78ms-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/78ms-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/83pv-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/83pv-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/83pv-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/83pv-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/90ms-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/90ms-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/90ms-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/90ms-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/90msp-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/90msp-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/90msp-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/90msp-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/90pv-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/90pv-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/90pv-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/90pv-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/Add-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/Add-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/Add-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/Add-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/Add-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/Add-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/Add-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/Add-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/B5-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/B5-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/B5pc-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/B5pc-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/B5pc-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/B5pc-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/CNS-EUC-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/CNS-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/CNS-EUC-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/CNS-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/CNS1-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/CNS1-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/CNS1-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/CNS1-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/CNS2-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/CNS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/CNS2-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/CNS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/ETHK-B5-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/ETHK-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/ETHK-B5-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/ETHK-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/ETen-B5-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/ETen-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/ETen-B5-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/ETen-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/EUC-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/EUC-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/Ext-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/Ext-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/Ext-RKSJ-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/Ext-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/Ext-RKSJ-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/Ext-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/Ext-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/Ext-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GB-EUC-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GB-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GB-EUC-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GB-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GB-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GB-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GB-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GB-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBK-EUC-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBK-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBK-EUC-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBK-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBK2K-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBK2K-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBK2K-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBK2K-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBKp-EUC-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBKp-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBKp-EUC-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBKp-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBT-EUC-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBT-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBT-EUC-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBT-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBT-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBT-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBT-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBT-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBTpc-EUC-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBTpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBTpc-EUC-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBTpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBpc-EUC-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/GBpc-EUC-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/GBpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/HKdla-B5-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/HKdla-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/HKdla-B5-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/HKdla-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/HKdlb-B5-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/HKdlb-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/HKdlb-B5-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/HKdlb-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/HKgccs-B5-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/HKgccs-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/HKgccs-B5-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/HKgccs-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/HKm314-B5-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/HKm314-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/HKm314-B5-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/HKm314-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/HKm471-B5-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/HKm471-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/HKm471-B5-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/HKm471-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/HKscs-B5-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/HKscs-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/HKscs-B5-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/HKscs-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/Hankaku-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/Hankaku-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/Hankaku-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/Hankaku-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/KSC-EUC-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/KSC-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/KSC-EUC-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/KSC-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/KSC-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/KSC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/KSC-Johab-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/KSC-Johab-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/KSC-Johab-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/KSC-Johab-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/KSC-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/KSC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/KSCms-UHC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/KSCms-UHC-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/KSCms-UHC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/KSCpc-EUC-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/KSCpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/KSCpc-EUC-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/KSCpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/NWP-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/NWP-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/NWP-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/NWP-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/README.txt` & `pdfminer_aemc-20231229/pdfminer/cmap/README.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/RKSJ-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/RKSJ-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UCS2-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UCS2-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF16-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF16-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF32-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF32-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF8-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniGB-UTF8-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniGB-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UCS2-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UCS2-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF16-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF16-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF32-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF32-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF8-H.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/UniKS-UTF8-V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/UniKS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/V.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz` & `pdfminer_aemc-20231229/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/cmapdb.py` & `pdfminer_aemc-20231229/pdfminer/cmapdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,21 @@
             unichr = chr(code)
         else:
             raise TypeError(code)
 
         # A0 = non-breaking space, some weird fonts can have a collision on a cid here.
         if unichr == "\u00A0" and self.cid2unichr.get(cid) == " ":
             return
-        self.cid2unichr[cid] = unichr
+
+        # bypass the strange ToUnicode map provided by Morisawa Inc.
+        if len(unichr) == 1:
+            self.cid2unichr[cid] = unichr
+        else:
+            self.cid2unichr[cid] = f"(cid2:{cid})"
+
 
 
 class PyCMap(CMap):
     def __init__(self, name: str, module: Any) -> None:
         super().__init__(CMapName=name)
         self.code2cid = module.CODE2CID
         if module.IS_VERTICAL:
```

### Comparing `pdfminer_aemc-20231228/pdfminer/converter.py` & `pdfminer_aemc-20231229/pdfminer/converter.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/data_structures.py` & `pdfminer_aemc-20231229/pdfminer/data_structures.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/encodingdb.py` & `pdfminer_aemc-20231229/pdfminer/encodingdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/fontmetrics.py` & `pdfminer_aemc-20231229/pdfminer/fontmetrics.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/glyphlist.py` & `pdfminer_aemc-20231229/pdfminer/glyphlist.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/high_level.py` & `pdfminer_aemc-20231229/pdfminer/high_level.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/image.py` & `pdfminer_aemc-20231229/pdfminer/image.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/jbig2.py` & `pdfminer_aemc-20231229/pdfminer/jbig2.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/latin_enc.py` & `pdfminer_aemc-20231229/pdfminer/latin_enc.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/layout.py` & `pdfminer_aemc-20231229/pdfminer/layout.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/lzw.py` & `pdfminer_aemc-20231229/pdfminer/lzw.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/pdfcolor.py` & `pdfminer_aemc-20231229/pdfminer/pdfcolor.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/pdfdevice.py` & `pdfminer_aemc-20231229/pdfminer/pdfdevice.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/pdfdocument.py` & `pdfminer_aemc-20231229/pdfminer/pdfdocument.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/pdffont.py` & `pdfminer_aemc-20231229/pdfminer/pdffont.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/pdfinterp.py` & `pdfminer_aemc-20231229/pdfminer/pdfinterp.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/pdfpage.py` & `pdfminer_aemc-20231229/pdfminer/pdfpage.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/pdfparser.py` & `pdfminer_aemc-20231229/pdfminer/pdfparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/pdftypes.py` & `pdfminer_aemc-20231229/pdfminer/pdftypes.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/psparser.py` & `pdfminer_aemc-20231229/pdfminer/psparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/runlength.py` & `pdfminer_aemc-20231229/pdfminer/runlength.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer/utils.py` & `pdfminer_aemc-20231229/pdfminer/utils.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/pdfminer.aemc.egg-info/PKG-INFO` & `pdfminer_aemc-20231229/pdfminer.aemc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfminer.aemc
-Version: 20231228
+Version: 20231229
 Summary: PDF parser and analyzer
 Home-page: https://github.com/pdfminer/pdfminer.aemc
 Author: Yusuke Shinyama + Philippe Guglielmetti + Liew Chun Fui
 Author-email: wargreymon28@gmail.com
 License: MIT/X
 Keywords: pdf parser,pdf converter,layout analysis,text mining
 Classifier: Programming Language :: Python
```

### Comparing `pdfminer_aemc-20231228/pdfminer.aemc.egg-info/SOURCES.txt` & `pdfminer_aemc-20231229/pdfminer.aemc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/setup.py` & `pdfminer_aemc-20231229/setup.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_converter.py` & `pdfminer_aemc-20231229/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_encodingdb.py` & `pdfminer_aemc-20231229/tests/test_encodingdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_font_size.py` & `pdfminer_aemc-20231229/tests/test_font_size.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_highlevel_extracttext.py` & `pdfminer_aemc-20231229/tests/test_highlevel_extracttext.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_layout.py` & `pdfminer_aemc-20231229/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_pdfdocument.py` & `pdfminer_aemc-20231229/tests/test_pdfdocument.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_pdfencoding.py` & `pdfminer_aemc-20231229/tests/test_pdfencoding.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_pdffont.py` & `pdfminer_aemc-20231229/tests/test_pdffont.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_pdfminer_ccitt.py` & `pdfminer_aemc-20231229/tests/test_pdfminer_ccitt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_pdfminer_crypto.py` & `pdfminer_aemc-20231229/tests/test_pdfminer_crypto.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_pdfminer_psparser.py` & `pdfminer_aemc-20231229/tests/test_pdfminer_psparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_pdfpage.py` & `pdfminer_aemc-20231229/tests/test_pdfpage.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_tools_dumppdf.py` & `pdfminer_aemc-20231229/tests/test_tools_dumppdf.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_tools_pdf2txt.py` & `pdfminer_aemc-20231229/tests/test_tools_pdf2txt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tests/test_utils.py` & `pdfminer_aemc-20231229/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tools/conv_afm.py` & `pdfminer_aemc-20231229/tools/conv_afm.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tools/conv_cmap.py` & `pdfminer_aemc-20231229/tools/conv_cmap.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tools/conv_glyphlist.py` & `pdfminer_aemc-20231229/tools/conv_glyphlist.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tools/dumppdf.py` & `pdfminer_aemc-20231229/tools/dumppdf.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tools/pdf2txt.py` & `pdfminer_aemc-20231229/tools/pdf2txt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tools/pdfdiff.py` & `pdfminer_aemc-20231229/tools/pdfdiff.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tools/pdfstats.py` & `pdfminer_aemc-20231229/tools/pdfstats.py`

 * *Files identical despite different names*

### Comparing `pdfminer_aemc-20231228/tools/prof.py` & `pdfminer_aemc-20231229/tools/prof.py`

 * *Files identical despite different names*

