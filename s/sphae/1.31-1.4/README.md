# Comparing `tmp/sphae-1.31.tar.gz` & `tmp/sphae-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphae-1.31.tar", last modified: Thu Nov 30 02:26:37 2023, max compression
+gzip compressed data, was "sphae-1.4.tar", last modified: Tue May  7 04:43:26 2024, max compression
```

## Comparing `sphae-1.31.tar` & `sphae-1.4.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 edwa0468 (352389) staff    (187448)        0 2023-11-30 02:27:22.469483 sphae-1.31/
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     1068 2023-11-21 09:17:59.000000 sphae-1.31/LICENSE
--rw-r--r--   0 edwa0468 (352389) staff    (187448)       13 2023-11-29 15:00:54.000000 sphae-1.31/MANIFEST.in
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     6103 2023-11-30 02:27:22.465482 sphae-1.31/PKG-INFO
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     4998 2023-11-28 01:39:31.000000 sphae-1.31/README.md
--rw-r--r--   0 edwa0468 (352389) staff    (187448)       38 2023-11-30 02:27:22.470483 sphae-1.31/setup.cfg
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     2145 2023-11-30 02:26:58.000000 sphae-1.31/setup.py
-drwxr-xr-x   0 edwa0468 (352389) staff    (187448)        0 2023-11-30 02:27:22.161458 sphae-1.31/sphae/
--rw-r--r--   0 edwa0468 (352389) staff    (187448)        0 2023-11-21 09:17:59.000000 sphae-1.31/sphae/__init__.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     5724 2023-11-21 09:17:59.000000 sphae-1.31/sphae/__main__.py
-drwxr-xr-x   0 edwa0468 (352389) staff    (187448)        0 2023-11-30 02:27:22.211462 sphae-1.31/sphae/config/
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      562 2023-11-21 09:17:59.000000 sphae-1.31/sphae/config/config.yaml
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      645 2023-11-21 09:17:59.000000 sphae-1.31/sphae/sphae.CITATION
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     1075 2023-11-21 09:17:59.000000 sphae-1.31/sphae/sphae.LICENSE
--rw-r--r--   0 edwa0468 (352389) staff    (187448)        5 2023-11-30 02:04:04.000000 sphae-1.31/sphae/sphae.VERSION
-drwxr-xr-x   0 edwa0468 (352389) staff    (187448)        0 2023-11-30 02:27:22.220463 sphae-1.31/sphae/workflow/
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     1537 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/Snakefile
-drwxr-xr-x   0 edwa0468 (352389) staff    (187448)        0 2023-11-30 02:27:22.270467 sphae-1.31/sphae/workflow/envs/
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      128 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/envs/checkv.yaml
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      109 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/envs/filtlong.yaml
--rw-r--r--   0 edwa0468 (352389) staff    (187448)       99 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/envs/flye.yaml
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      227 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/envs/graph.yaml
--rw-r--r--   0 edwa0468 (352389) staff    (187448)       98 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/envs/medaka.yaml
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      158 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/envs/megahit.yaml
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      162 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/envs/pharokka.yaml
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      156 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/envs/phynteny.yaml
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      107 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/envs/samtools.yaml
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      130 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/envs/trimnami.yaml
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      112 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/envs/viralverify.yaml
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     2353 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/install.smk
-drwxr-xr-x   0 edwa0468 (352389) staff    (187448)        0 2023-11-30 02:27:22.335472 sphae-1.31/sphae/workflow/rules/
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      938 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/rules/1.preflight-database.smk
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     2581 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/rules/1.preflight.smk
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     4813 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/rules/2.targets.smk
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     1574 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/rules/3.qc_qa.smk
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     4757 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/rules/4.assembly.smk
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     2169 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/rules/5.checkv.smk
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     1817 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/rules/5.components.smk
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     2198 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/rules/5.viralverify.smk
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     3065 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/rules/6.phage_genome.smk
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     1051 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/rules/6.stat_join.smk
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     5028 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/rules/7.pharokka.smk
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     1854 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/rules/7.phynteny.smk
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     2904 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/rules/8.final-reporting.smk
-drwxr-xr-x   0 edwa0468 (352389) staff    (187448)        0 2023-11-30 02:27:22.361474 sphae-1.31/sphae/workflow/scripts/
--rwxr-xr-x   0 edwa0468 (352389) staff    (187448)     5812 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/scripts/components.py
--rwxr-xr-x   0 edwa0468 (352389) staff    (187448)    32928 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/fastg2gfa
-drwxr-xr-x   0 edwa0468 (352389) staff    (187448)        0 2023-11-30 02:27:22.366474 sphae-1.31/sphae/workflow/scripts/graph_utils/
--rw-r--r--   0 edwa0468 (352389) staff    (187448)    20327 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/graph_utils/build_utils.py
--rwxr-xr-x   0 edwa0468 (352389) staff    (187448)     1651 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/scripts/joining_stats.py
--rwxr-xr-x   0 edwa0468 (352389) staff    (187448)     1898 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/scripts/pick_phage_contigs.py
--rwxr-xr-x   0 edwa0468 (352389) staff    (187448)     1758 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/rename_genomes.py
-drwxr-xr-x   0 edwa0468 (352389) staff    (187448)        0 2023-11-30 02:27:22.450481 sphae-1.31/sphae/workflow/scripts/roblib/
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     1547 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/__init__.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     1127 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/alignments.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      571 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/bcolors.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     1877 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/blast.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     2089 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/colours.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     4646 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/date_parsing.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     1390 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/dna.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     1818 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/dnadist.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      787 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/file_chooser.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     2914 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/functions.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)    10765 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/genbank.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     1923 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/geography.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     6633 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/newick.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      879 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/rob_error.py
--rwxr-xr-x   0 edwa0468 (352389) staff    (187448)     2355 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/seqio_filter.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)    10890 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/sequences.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     2790 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/stats.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      193 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/strings.py
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     4840 2023-11-21 09:17:59.000000 sphae-1.31/sphae/workflow/scripts/roblib/translate.py
--rwxr-xr-x   0 edwa0468 (352389) staff    (187448)     5824 2023-11-28 01:39:31.000000 sphae-1.31/sphae/workflow/scripts/summary.py
-drwxr-xr-x   0 edwa0468 (352389) staff    (187448)        0 2023-11-30 02:27:22.459482 sphae-1.31/sphae.egg-info/
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     6103 2023-11-30 02:27:21.000000 sphae-1.31/sphae.egg-info/PKG-INFO
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     2342 2023-11-30 02:27:21.000000 sphae-1.31/sphae.egg-info/SOURCES.txt
--rw-r--r--   0 edwa0468 (352389) staff    (187448)        1 2023-11-30 02:27:21.000000 sphae-1.31/sphae.egg-info/dependency_links.txt
--rw-r--r--   0 edwa0468 (352389) staff    (187448)       46 2023-11-30 02:27:21.000000 sphae-1.31/sphae.egg-info/entry_points.txt
--rw-r--r--   0 edwa0468 (352389) staff    (187448)      121 2023-11-30 02:27:21.000000 sphae-1.31/sphae.egg-info/requires.txt
--rw-r--r--   0 edwa0468 (352389) staff    (187448)        6 2023-11-30 02:27:21.000000 sphae-1.31/sphae.egg-info/top_level.txt
-drwxr-xr-x   0 edwa0468 (352389) staff    (187448)        0 2023-11-30 02:27:22.454481 sphae-1.31/tests/
--rw-r--r--   0 edwa0468 (352389) staff    (187448)     3314 2023-11-21 09:18:00.000000 sphae-1.31/tests/test_sphae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.771425 sphae-1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-07 04:43:22.000000 sphae-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 04:43:22.000000 sphae-1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-07 04:43:26.771425 sphae-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-05-07 04:43:22.000000 sphae-1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 04:43:26.771425 sphae-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-07 04:43:22.000000 sphae-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.763425 sphae-1.4/sphae/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:22.000000 sphae-1.4/sphae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-07 04:43:22.000000 sphae-1.4/sphae/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.763425 sphae-1.4/sphae/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-07 04:43:22.000000 sphae-1.4/sphae/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 04:43:22.000000 sphae-1.4/sphae/sphae.CITATION
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-07 04:43:22.000000 sphae-1.4/sphae/sphae.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 04:43:22.000000 sphae-1.4/sphae/sphae.VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.763425 sphae-1.4/sphae/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.763425 sphae-1.4/sphae/workflow/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/checkv.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/flye.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/graph.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/medaka.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/megahit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/pharokka.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/phold.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/phynteny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/samtools.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/trimnami.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/envs/viralverify.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/install.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.767425 sphae-1.4/sphae/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/1.preflight-database.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/1.preflight.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/10.final-reporting.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/2.targets.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/3.qc_qa.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/4.assembly.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/5.checkv.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/5.components.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/5.viralverify.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/6.phage_genome.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/6.stat_join.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/7.pharokka.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/8.phold.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/rules/9.phynteny.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.767425 sphae-1.4/sphae/workflow/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5812 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/components.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32928 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/fastg2gfa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.767425 sphae-1.4/sphae/workflow/scripts/graph_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/graph_utils/build_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1651 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/joining_stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1898 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/pick_phage_contigs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1758 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/rename_genomes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.771425 sphae-1.4/sphae/workflow/scripts/roblib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/alignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/bcolors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/blast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/colours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/date_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/dnadist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/file_chooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/genbank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/geography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/newick.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/rob_error.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2355 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/seqio_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/roblib/translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9164 2024-05-07 04:43:22.000000 sphae-1.4/sphae/workflow/scripts/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.771425 sphae-1.4/sphae.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-07 04:43:26.000000 sphae-1.4/sphae.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-07 04:43:26.000000 sphae-1.4/sphae.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 04:43:26.000000 sphae-1.4/sphae.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 04:43:26.000000 sphae-1.4/sphae.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 04:43:26.000000 sphae-1.4/sphae.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 04:43:26.000000 sphae-1.4/sphae.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:43:26.771425 sphae-1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-07 04:43:22.000000 sphae-1.4/tests/test_sphae.py
```

### Comparing `sphae-1.31/LICENSE` & `sphae-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sphae-1.31/setup.py` & `sphae-1.4/setup.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/__main__.py` & `sphae-1.4/sphae/__main__.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/config/config.yaml` & `sphae-1.4/sphae/config/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     cpu: 32
     mem: 64000
     time: 480
 
 trimnami:
   qc:
     subsample:
-      --bases 100M
+      --bases 1000M
   host: 
 
 params:
   medaka: "r1041_e82_400bps_sup_v4.2.0" # the current default in medaka v1.8 and the most recent model
   flye: "--nano-hq"
   genomeSize: 44k
 
@@ -24,8 +24,8 @@
   output: 
   db_dir: 
   sequencing: 
 
 db:
   pfam: "ftp://ftp.ebi.ac.uk/pub/databases/Pfam/releases/"
   pfam_file: 'Pfam35.0/Pfam-A.hmm.gz'
-  models: "https://zenodo.org/record/8198288/files/phynteny_models_v0.1.11.tar.gz"
+  models: "https://zenodo.org/record/8198288/files/phynteny_models_v0.1.11.tar.gz"
```

### Comparing `sphae-1.31/sphae/sphae.CITATION` & `sphae-1.4/sphae/sphae.CITATION`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/sphae.LICENSE` & `sphae-1.4/sphae/sphae.LICENSE`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/Snakefile` & `sphae-1.4/sphae/workflow/Snakefile`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 include: os.path.join("rules", "4.assembly.smk")
 include: os.path.join("rules", "5.components.smk")
 include: os.path.join("rules", "5.viralverify.smk")
 include: os.path.join("rules", "5.checkv.smk")
 include: os.path.join("rules", "6.stat_join.smk")
 include: os.path.join("rules", "6.phage_genome.smk")
 include: os.path.join("rules", "7.pharokka.smk")
-include: os.path.join("rules", "7.phynteny.smk")
-include: os.path.join("rules", "8.final-reporting.smk")
+include: os.path.join("rules", "8.phold.smk")
+include: os.path.join("rules", "9.phynteny.smk")
+include: os.path.join("rules", "10.final-reporting.smk")
 
 
 """Mark target rules"""
 target_rules = []
 def targetRule(fn):
     assert fn.__name__.startswith('__')
     target_rules.append(fn.__name__[2:])
```

### Comparing `sphae-1.31/sphae/workflow/install.smk` & `sphae-1.4/sphae/workflow/install.smk`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 targets.db = []
 
 targets.db.append(os.path.join(databaseDir, 'Pfam35.0', 'Pfam-A.hmm.gz'))
 targets.db.append(os.path.join(databaseDir, 'pharokka_db', 'phrogs_db.index'))
 targets.db.append(os.path.join(databaseDir, 'checkv-db-v1.5', 'README.txt'))
 targets.db.append(os.path.join(databaseDir, 'phynteny_models_zenodo', 'grid_search_model.m_400.b_256.lr_0.0001.dr_0.1.l_2.a_tanh.o_rmsprop.rep_0.best_val_loss.h5'))
-
+targets.db.append(os.path.join(databaseDir, "phold", "phold_annots.tsv"))
 
 """RUN SNAKEMAKE"""
 rule all:
     input:
         targets.db
 
 
@@ -83,7 +83,20 @@
     conda:
         os.path.join(dir.env, "phynteny.yaml")
     shell:
         """
             wget -O {params.download} {params.url}
             tar -xvzf {params.download} -C {params.models}
         """
+
+rule phold_install:
+    params:
+        phold_db=os.path.join(databaseDir, "phold")
+    output:
+        os.path.join(databaseDir, "phold", "phold_annots.tsv")
+    conda:
+        os.path.join(dir.env, "phold.yaml")
+    shell:
+        """
+        phold install -d {params.phold_db}
+        """
+
```

### Comparing `sphae-1.31/sphae/workflow/rules/1.preflight-database.smk` & `sphae-1.4/sphae/workflow/rules/1.preflight-database.smk`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/rules/1.preflight.smk` & `sphae-1.4/sphae/workflow/rules/1.preflight.smk`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 dir.assembly = os.path.join(dir.out, 'PROCESSING','assembly')
 dir.megahit = os.path.join(dir.assembly, 'megahit')
 dir.flye = os.path.join(dir.assembly, 'flye')
 dir.genome = os.path.join(dir.out, 'PROCESSING','genome')
 dir.cov = os.path.join(dir.out, 'PROCESSING','coverage')
 dir.pharokka = os.path.join(dir.out, 'PROCESSING','pharokka')
 dir.log = os.path.join(dir.out, 'logs')
-dir.bench = os.path.join(dir.out, 'PROCESSING','bench')
+dir.bench = os.path.join(dir.out, 'PROCESSING','benchmarks')
 dir.final = os.path.join(dir.out, 'RESULTS')
 
 dir.env = os.path.join(workflow.basedir, "envs")
 dir.script = os.path.join(workflow.basedir, "scripts")
 
 # database dir
 if config.args.db_dir is None:
```

### Comparing `sphae-1.31/sphae/workflow/rules/2.targets.smk` & `sphae-1.4/sphae/workflow/rules/2.targets.smk`

 * *Files 1% similar despite different names*

```diff
@@ -33,22 +33,26 @@
 targets.annotate = []
 if config.args.sequencing == 'paired':
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-pr", "{sample}.gbk"), sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-pr", "{sample}_pharokka_plot.png"), sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-pr", "top_hits_card.tsv"),sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-pr", "top_hits_vfdb.tsv"),sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-pr", "{sample}_minced_spacers.txt"),sample=samples.names))
+    targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-pr-phold", "{sample}.gbk"),sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-pr", "phynteny", "phynteny.gbk"), sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-pr", "{sample}_top_hits_mash_inphared.tsv"),sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.final, "{sample}-pr", "{sample}_summary.txt"), sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-pr", "{sample}_length_gc_cds_density.tsv"), sample=samples.names))
+    targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-pr", "{sample}_cds_functions.tsv"), sample=samples.names))
 elif config.args.sequencing == 'longread':
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-sr", "{sample}.gbk"), sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-sr", "{sample}_pharokka_plot.png"), sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-sr", "phynteny", "phynteny.gbk"), sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-sr", "top_hits_card.tsv"),sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-sr", "top_hits_vfdb.tsv"),sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-sr", "{sample}_minced_spacers.txt"),sample=samples.names))
+    targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-sr-phold", "{sample}.gbk"),sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-sr", "phynteny", "phynteny.gbk"), sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-sr", "{sample}_top_hits_mash_inphared.tsv"),sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.final, "{sample}-sr", "{sample}_summary.txt"), sample=samples.names))
     targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-sr", "{sample}_length_gc_cds_density.tsv"), sample=samples.names))
+    targets.annotate.append(expand(os.path.join(dir.pharokka, "{sample}-sr", "{sample}_cds_functions.tsv"), sample=samples.names))
```

### Comparing `sphae-1.31/sphae/workflow/rules/3.qc_qa.smk` & `sphae-1.4/sphae/workflow/rules/3.qc_qa.smk`

 * *Files 2% similar despite different names*

```diff
@@ -43,8 +43,10 @@
             --reads {input} \
             --output {params.dir} \
             --subsample \
             {params.trimmer} \
             {params.host} \
             {params.profile} \
             --log {log}
+
+            touch {output}
         """
```

### Comparing `sphae-1.31/sphae/workflow/rules/4.assembly.smk` & `sphae-1.4/sphae/workflow/rules/4.assembly.smk`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/rules/5.checkv.smk` & `sphae-1.4/sphae/workflow/rules/5.checkv.smk`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/rules/5.components.smk` & `sphae-1.4/sphae/workflow/rules/5.components.smk`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/rules/5.viralverify.smk` & `sphae-1.4/sphae/workflow/rules/5.viralverify.smk`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/rules/6.phage_genome.smk` & `sphae-1.4/sphae/workflow/rules/6.phage_genome.smk`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/rules/6.stat_join.smk` & `sphae-1.4/sphae/workflow/rules/6.stat_join.smk`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/rules/7.pharokka.smk` & `sphae-1.4/sphae/workflow/rules/7.pharokka.smk`

 * *Files 3% similar despite different names*

```diff
@@ -27,24 +27,27 @@
     output:
         gbk=os.path.join(dir.pharokka, "{sample}-pr", "{sample}.gbk"),
         plot=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_pharokka_plot.png"),
         card=os.path.join(dir.pharokka, "{sample}-pr", "top_hits_card.tsv"),
         vfdb=os.path.join(dir.pharokka, "{sample}-pr", "top_hits_vfdb.tsv"),
         spacers=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_minced_spacers.txt"),
         taxa=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_top_hits_mash_inphared.tsv"),
-        cdden=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_length_gc_cds_density.tsv")
+        cdden=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_length_gc_cds_density.tsv"),
+        cds=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_cds_functions.tsv")
     conda:
         os.path.join(dir.env, "pharokka.yaml")
     threads:
         config.resources.smalljob.cpu
     resources:
         mem_mb = config.resources.smalljob.mem,
         time = config.resources.smalljob.time
     log:
         os.path.join(dir.log, "pharokka.{sample}.log")
+    benchmark:
+        os.path.join(dir.bench,"pharokka_megahit_{sample}.txt")
     shell:
         """
         if [[ -s {input} ]] ; then
             pharokka.py \
                 -i {input} \
                 -o {params.o} \
                 -d {params.db} \
@@ -55,22 +58,24 @@
             touch {output.gbk}
             touch {output.plot}
             touch {output.card}
             touch {output.vfdb}
             touch {output.spacers}
             touch {output.taxa}
             touch {output.cdden}
+            touch {output.cds}
         else
             touch {output.gbk}
             touch {output.plot}
             touch {output.card}
             touch {output.vfdb}
             touch {output.spacers}
             touch {output.taxa}
             touch {output.cdden}
+            touch {output.cds}
         fi
         """
 
 rule rename_contigs_flye:
     input:
         fin=os.path.join(dir.genome, "{sample}-sr", "{sample}.fasta"),
     params:
@@ -95,24 +100,27 @@
     output:
         gbk=os.path.join(dir.pharokka, "{sample}-sr", "{sample}.gbk"),
         plot=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_pharokka_plot.png"),
         card=os.path.join(dir.pharokka, "{sample}-sr", "top_hits_card.tsv"),
         vfdb=os.path.join(dir.pharokka, "{sample}-sr", "top_hits_vfdb.tsv"),
         spacers=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_minced_spacers.txt"),
         taxa=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_top_hits_mash_inphared.tsv"),
-        cdden=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_length_gc_cds_density.tsv")
+        cdden=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_length_gc_cds_density.tsv"),
+        cds=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_cds_functions.tsv")
     conda:
         os.path.join(dir.env, "pharokka.yaml")
     threads:
         config.resources.smalljob.cpu
     resources:
         mem_mb = config.resources.smalljob.mem,
         time = config.resources.smalljob.time
     log:
         os.path.join(dir.log, "pharokka.{sample}.log")
+    benchmark:
+        os.path.join(dir.bench,"pharokka_flye_{sample}.txt")
     shell:
         """
         if [[ -s {input} ]] ; then
             pharokka.py \
                 -i {input} \
                 -o {params.o} \
                 -d {params.db} \
@@ -124,17 +132,19 @@
             touch {output.gbk}
             touch {output.plot}
             touch {output.card}
             touch {output.vfdb}
             touch {output.spacers}
             touch {output.taxa}
             touch {output.cdden}
+            touch {output.cds}
         else
             touch {output.gbk}
             touch {output.plot}
             touch {output.card}
             touch {output.vfdb}
             touch {output.spacers}
             touch {output.taxa}
             touch {output.cdden}
+            touch {output.cds}
         fi
         """
```

### Comparing `sphae-1.31/sphae/workflow/rules/7.phynteny.smk` & `sphae-1.4/sphae/workflow/rules/9.phynteny.smk`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 """
 Running phynteny to improve the anntoation 
 """
 rule phynteny_run_paired:
     input:
-        gbk=os.path.join(dir.pharokka, "{sample}-pr", "{sample}.gbk")
+        gbk=os.path.join(dir.pharokka,"{sample}-pr-phold","{sample}.gbk")
     params:
         odir=os.path.join(dir.pharokka, "{sample}-pr", "phynteny"),
         model=os.path.join(dir.db, "phynteny_models_zenodo")
     output:
         pkl=os.path.join(dir.pharokka, "{sample}-pr", "phynteny", "phynteny.gbk")
     conda:
         os.path.join(dir.env, "phynteny.yaml")
     threads:
         config.resources.smalljob.cpu
     resources:
         mem_mb = config.resources.smalljob.mem,
         time = config.resources.smalljob.time
     log:
         os.path.join(dir.log, "phynteny.{sample}.log")
+    benchmark:
+        os.path.join(dir.bench,"phynteny_megahit_{sample}.txt")
     shell:
         """
         if [[ -s {input.gbk} ]] ; then
             phynteny {input.gbk} -o {params.odir} \
                 -m {params.model} -f\
                 2> {log}
             touch {output.pkl}
         else
             touch {output.pkl}
         fi
         """
 
-
 rule phynteny_run_nanopore:
     input:
-        gbk=os.path.join(dir.pharokka, "{sample}-sr", "{sample}.gbk")
+        gbk=os.path.join(dir.pharokka,"{sample}-sr-phold","{sample}.gbk")
     params:
         odir=os.path.join(dir.pharokka, "{sample}-sr", "phynteny"),
         model=os.path.join(dir.db, "phynteny_models_zenodo")
     output:
         pkl=os.path.join(dir.pharokka, "{sample}-sr", "phynteny", "phynteny.gbk")
     conda:
         os.path.join(dir.env, "phynteny.yaml")
     threads:
         config.resources.smalljob.cpu
     resources:
         mem_mb = config.resources.smalljob.mem,
         time = config.resources.smalljob.time
     log:
         os.path.join(dir.log, "phynteny.{sample}.log")
+    benchmark:
+        os.path.join(dir.bench,"phynteny_nanopore_{sample}.txt")
     shell:
         """
         if [[ -s {input.gbk} ]] ; then
             phynteny {input.gbk} -o {params.odir} \
                 -m {params.model} -f\
                 2> {log}
             touch {output.pkl}
```

### Comparing `sphae-1.31/sphae/workflow/rules/8.final-reporting.smk` & `sphae-1.4/sphae/workflow/rules/10.final-reporting.smk`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         table= os.path.join(dir.genome, "{sample}-pr", "{sample}-genome-candidates.csv"),
         amr =os.path.join(dir.pharokka, "{sample}-pr", "top_hits_card.tsv"),
         vfdb=os.path.join(dir.pharokka, "{sample}-pr", "top_hits_vfdb.tsv"),
         spacers=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_minced_spacers.txt"),
         plot=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_pharokka_plot.png"),
         ph_taxa =os.path.join(dir.pharokka, "{sample}-pr", "{sample}_top_hits_mash_inphared.tsv"),
         cdden=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_length_gc_cds_density.tsv"),
+        cds=os.path.join(dir.pharokka, "{sample}-pr", "{sample}_cds_functions.tsv")
     output:
         summary=os.path.join(dir.final, "{sample}-pr", "{sample}_summary.txt")
     params:
         genomes= os.path.join(dir.final, "{sample}-pr", "{sample}_genome.fasta"),
         gbks=os.path.join(dir.final, "{sample}-pr", "{sample}.gbk"),
         plots=os.path.join(dir.final, "{sample}-pr", "{sample}_pharokka_plot.png"),
         outdir=os.path.join(dir.final),
@@ -35,14 +36,15 @@
         table= os.path.join(dir.genome, "{sample}-sr", "{sample}-genome-candidates.csv"),
         amr =os.path.join(dir.pharokka, "{sample}-sr", "top_hits_card.tsv"),
         vfdb=os.path.join(dir.pharokka, "{sample}-sr", "top_hits_vfdb.tsv"),
         plot=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_pharokka_plot.png"),
         spacers=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_minced_spacers.txt"),
         ph_taxa =os.path.join(dir.pharokka, "{sample}-sr", "{sample}_top_hits_mash_inphared.tsv"),
         cdden=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_length_gc_cds_density.tsv"),
+        cds=os.path.join(dir.pharokka, "{sample}-sr", "{sample}_cds_functions.tsv")
     output:
         summary=os.path.join(dir.final, "{sample}-sr", "{sample}_summary.txt")
     params:
         genomes= os.path.join(dir.final, "{sample}-sr", "{sample}_genome.fasta"),
         gbks=os.path.join(dir.final, "{sample}-sr", "{sample}.gbk"),
         plots=os.path.join(dir.final, "{sample}-sr", "{sample}_pharokka_plot.png"),
         sample="{sample}",
```

### Comparing `sphae-1.31/sphae/workflow/scripts/components.py` & `sphae-1.4/sphae/workflow/scripts/components.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/fastg2gfa` & `sphae-1.4/sphae/workflow/scripts/fastg2gfa`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/graph_utils/build_utils.py` & `sphae-1.4/sphae/workflow/scripts/graph_utils/build_utils.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/joining_stats.py` & `sphae-1.4/sphae/workflow/scripts/joining_stats.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/pick_phage_contigs.py` & `sphae-1.4/sphae/workflow/scripts/pick_phage_contigs.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/rename_genomes.py` & `sphae-1.4/sphae/workflow/scripts/rename_genomes.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/__init__.py` & `sphae-1.4/sphae/workflow/scripts/roblib/__init__.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/alignments.py` & `sphae-1.4/sphae/workflow/scripts/roblib/alignments.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/bcolors.py` & `sphae-1.4/sphae/workflow/scripts/roblib/bcolors.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/blast.py` & `sphae-1.4/sphae/workflow/scripts/roblib/blast.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/colours.py` & `sphae-1.4/sphae/workflow/scripts/roblib/colours.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/date_parsing.py` & `sphae-1.4/sphae/workflow/scripts/roblib/date_parsing.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/dna.py` & `sphae-1.4/sphae/workflow/scripts/roblib/dna.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/dnadist.py` & `sphae-1.4/sphae/workflow/scripts/roblib/dnadist.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/file_chooser.py` & `sphae-1.4/sphae/workflow/scripts/roblib/file_chooser.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/functions.py` & `sphae-1.4/sphae/workflow/scripts/roblib/functions.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/genbank.py` & `sphae-1.4/sphae/workflow/scripts/roblib/genbank.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/geography.py` & `sphae-1.4/sphae/workflow/scripts/roblib/geography.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/newick.py` & `sphae-1.4/sphae/workflow/scripts/roblib/newick.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/rob_error.py` & `sphae-1.4/sphae/workflow/scripts/roblib/rob_error.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/seqio_filter.py` & `sphae-1.4/sphae/workflow/scripts/roblib/seqio_filter.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/sequences.py` & `sphae-1.4/sphae/workflow/scripts/roblib/sequences.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/stats.py` & `sphae-1.4/sphae/workflow/scripts/roblib/stats.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae/workflow/scripts/roblib/translate.py` & `sphae-1.4/sphae/workflow/scripts/roblib/translate.py`

 * *Files identical despite different names*

### Comparing `sphae-1.31/sphae.egg-info/SOURCES.txt` & `sphae-1.4/sphae.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,37 +13,38 @@
 sphae.egg-info/entry_points.txt
 sphae.egg-info/requires.txt
 sphae.egg-info/top_level.txt
 sphae/config/config.yaml
 sphae/workflow/Snakefile
 sphae/workflow/install.smk
 sphae/workflow/envs/checkv.yaml
-sphae/workflow/envs/filtlong.yaml
 sphae/workflow/envs/flye.yaml
 sphae/workflow/envs/graph.yaml
 sphae/workflow/envs/medaka.yaml
 sphae/workflow/envs/megahit.yaml
 sphae/workflow/envs/pharokka.yaml
+sphae/workflow/envs/phold.yaml
 sphae/workflow/envs/phynteny.yaml
 sphae/workflow/envs/samtools.yaml
 sphae/workflow/envs/trimnami.yaml
 sphae/workflow/envs/viralverify.yaml
 sphae/workflow/rules/1.preflight-database.smk
 sphae/workflow/rules/1.preflight.smk
+sphae/workflow/rules/10.final-reporting.smk
 sphae/workflow/rules/2.targets.smk
 sphae/workflow/rules/3.qc_qa.smk
 sphae/workflow/rules/4.assembly.smk
 sphae/workflow/rules/5.checkv.smk
 sphae/workflow/rules/5.components.smk
 sphae/workflow/rules/5.viralverify.smk
 sphae/workflow/rules/6.phage_genome.smk
 sphae/workflow/rules/6.stat_join.smk
 sphae/workflow/rules/7.pharokka.smk
-sphae/workflow/rules/7.phynteny.smk
-sphae/workflow/rules/8.final-reporting.smk
+sphae/workflow/rules/8.phold.smk
+sphae/workflow/rules/9.phynteny.smk
 sphae/workflow/scripts/components.py
 sphae/workflow/scripts/fastg2gfa
 sphae/workflow/scripts/joining_stats.py
 sphae/workflow/scripts/pick_phage_contigs.py
 sphae/workflow/scripts/rename_genomes.py
 sphae/workflow/scripts/summary.py
 sphae/workflow/scripts/graph_utils/build_utils.py
```

### Comparing `sphae-1.31/tests/test_sphae.py` & `sphae-1.4/tests/test_sphae.py`

 * *Files identical despite different names*

