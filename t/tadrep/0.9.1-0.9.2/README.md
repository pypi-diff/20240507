# Comparing `tmp/tadrep-0.9.1.tar.gz` & `tmp/tadrep-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tadrep-0.9.1.tar", last modified: Mon Aug 21 13:09:00 2023, max compression
+gzip compressed data, was "tadrep-0.9.2.tar", last modified: Tue May  7 07:20:29 2024, max compression
```

## Comparing `tadrep-0.9.1.tar` & `tadrep-0.9.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:09:00.563187 tadrep-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-08-21 13:08:46.000000 tadrep-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17283 2023-08-21 13:09:00.563187 tadrep-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15989 2023-08-21 13:08:46.000000 tadrep-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-21 13:09:00.563187 tadrep-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-21 13:08:46.000000 tadrep-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:09:00.559187 tadrep-0.9.1/tadrep/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/blast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/characterize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:09:00.559187 tadrep-0.9.1/tadrep/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/database/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/database/plsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/database/refseq.py
--rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/plasmids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-21 13:08:46.000000 tadrep-0.9.1/tadrep/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:09:00.559187 tadrep-0.9.1/tadrep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17283 2023-08-21 13:09:00.000000 tadrep-0.9.1/tadrep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-21 13:09:00.000000 tadrep-0.9.1/tadrep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 13:09:00.000000 tadrep-0.9.1/tadrep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-21 13:09:00.000000 tadrep-0.9.1/tadrep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 13:09:00.000000 tadrep-0.9.1/tadrep.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-21 13:09:00.000000 tadrep-0.9.1/tadrep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-21 13:09:00.000000 tadrep-0.9.1/tadrep.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:09:00.559187 tadrep-0.9.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-08-21 13:08:46.000000 tadrep-0.9.1/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-21 13:08:46.000000 tadrep-0.9.1/test/test_blast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-08-21 13:08:46.000000 tadrep-0.9.1/test/test_plasmids.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-21 13:08:46.000000 tadrep-0.9.1/test/test_tadrep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:20:29.492183 tadrep-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-07 07:20:25.000000 tadrep-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17437 2024-05-07 07:20:29.488183 tadrep-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15989 2024-05-07 07:20:25.000000 tadrep-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:20:29.492183 tadrep-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-07 07:20:25.000000 tadrep-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:20:29.488183 tadrep-0.9.2/tadrep/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/blast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/characterize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:20:29.488183 tadrep-0.9.2/tadrep/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/database/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/database/plsdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/database/refseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/plasmids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-07 07:20:25.000000 tadrep-0.9.2/tadrep/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:20:29.488183 tadrep-0.9.2/tadrep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17437 2024-05-07 07:20:29.000000 tadrep-0.9.2/tadrep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-07 07:20:29.000000 tadrep-0.9.2/tadrep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:20:29.000000 tadrep-0.9.2/tadrep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 07:20:29.000000 tadrep-0.9.2/tadrep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:20:29.000000 tadrep-0.9.2/tadrep.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 07:20:29.000000 tadrep-0.9.2/tadrep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 07:20:29.000000 tadrep-0.9.2/tadrep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:20:29.488183 tadrep-0.9.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-07 07:20:25.000000 tadrep-0.9.2/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-07 07:20:25.000000 tadrep-0.9.2/test/test_blast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-07 07:20:25.000000 tadrep-0.9.2/test/test_plasmids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-07 07:20:25.000000 tadrep-0.9.2/test/test_tadrep.py
```

### Comparing `tadrep-0.9.1/LICENSE` & `tadrep-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/PKG-INFO` & `tadrep-0.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tadrep
-Version: 0.9.1
+Version: 0.9.2
 Summary: TaDRep: Targeted Detection and Reconstruction of Plasmids
 Home-page: https://github.com/oschwengers/tadrep
 Author: Oliver Schwengers
 Author-email: oliver.schwengers@computational.bio.uni-giessen.de
 License: GPLv3
 Project-URL: Documentation, https://github.com/oschwengers/tadrep/blob/main/README.md
 Project-URL: Source, https://github.com/oschwengers/tadrep
@@ -22,14 +22,19 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biopython>=1.78
+Requires-Dist: xopen>=1.5.0
+Requires-Dist: pyrodigal>=2.1.0
+Requires-Dist: matplotlib>=3.7
+Requires-Dist: pygenomeviz>=0.4
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-brightgreen.svg)](https://github.com/oschwengers/tadrep/blob/master/LICENSE)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tadrep.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/tadrep.svg)
 ![GitHub release](https://img.shields.io/github/release/oschwengers/tadrep.svg)
 [![PyPI](https://img.shields.io/pypi/v/tadrep.svg)](https://pypi.org/project/tadrep)
 [![Conda](https://img.shields.io/conda/v/bioconda/tadrep.svg)](https://bioconda.github.io/recipes/tadrep/README.html)
```

### Comparing `tadrep-0.9.1/README.md` & `tadrep-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/setup.py` & `tadrep-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/blast.py` & `tadrep-0.9.2/tadrep/blast.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/characterize.py` & `tadrep-0.9.2/tadrep/characterize.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/cluster.py` & `tadrep-0.9.2/tadrep/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     # cluster sequences
     cmd_cdhitest = [
         'cd-hit-est',
         '-i', str(fasta_path),
         '-o', str(cfg.tmp_path.joinpath('plasmids.clustered')),
         '-G', '1',  # use global sequence identity
         '-c', str(cfg.cluster_sequence_identity_threshold),  # sequence identity threshold
-        '-S', str(cfg.cluster_sequence_identity_threshold),  # sequence length threshold in bps
-        '-AL', str(cfg.cluster_sequence_identity_threshold),  # aligntment length threshold in bps
+        '-S', str(cfg.cluster_length_threshold),  # sequence length threshold in bps
+        '-AL', str(cfg.cluster_length_threshold),  # aligntment length threshold in bps
         '-g', '1',  # cluster to the most similar cluster (slower but more accurate)
         '-r', '1',  # do +/+ and +/- alignments
         '-mask', 'NX',  # mask N and X letters
         '-d', '0',  # provide entire Fasta identifier in cluster description file
         '-M', '0',  # allow unlimited memory consumption
         '-T', str(cfg.threads)
     ]
```

### Comparing `tadrep-0.9.1/tadrep/config.py` & `tadrep-0.9.2/tadrep/config.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/database/main.py` & `tadrep-0.9.2/tadrep/database/main.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/database/plsdb.py` & `tadrep-0.9.2/tadrep/database/plsdb.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/database/refseq.py` & `tadrep-0.9.2/tadrep/database/refseq.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/detect.py` & `tadrep-0.9.2/tadrep/detect.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/extract.py` & `tadrep-0.9.2/tadrep/extract.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/io.py` & `tadrep-0.9.2/tadrep/io.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/main.py` & `tadrep-0.9.2/tadrep/main.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/plasmids.py` & `tadrep-0.9.2/tadrep/plasmids.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/setup.py` & `tadrep-0.9.2/tadrep/setup.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/utils.py` & `tadrep-0.9.2/tadrep/utils.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep/visualize.py` & `tadrep-0.9.2/tadrep/visualize.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/tadrep.egg-info/PKG-INFO` & `tadrep-0.9.2/tadrep.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tadrep
-Version: 0.9.1
+Version: 0.9.2
 Summary: TaDRep: Targeted Detection and Reconstruction of Plasmids
 Home-page: https://github.com/oschwengers/tadrep
 Author: Oliver Schwengers
 Author-email: oliver.schwengers@computational.bio.uni-giessen.de
 License: GPLv3
 Project-URL: Documentation, https://github.com/oschwengers/tadrep/blob/main/README.md
 Project-URL: Source, https://github.com/oschwengers/tadrep
@@ -22,14 +22,19 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biopython>=1.78
+Requires-Dist: xopen>=1.5.0
+Requires-Dist: pyrodigal>=2.1.0
+Requires-Dist: matplotlib>=3.7
+Requires-Dist: pygenomeviz>=0.4
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-brightgreen.svg)](https://github.com/oschwengers/tadrep/blob/master/LICENSE)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tadrep.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/tadrep.svg)
 ![GitHub release](https://img.shields.io/github/release/oschwengers/tadrep.svg)
 [![PyPI](https://img.shields.io/pypi/v/tadrep.svg)](https://pypi.org/project/tadrep)
 [![Conda](https://img.shields.io/conda/v/bioconda/tadrep.svg)](https://bioconda.github.io/recipes/tadrep/README.html)
```

### Comparing `tadrep-0.9.1/tadrep.egg-info/SOURCES.txt` & `tadrep-0.9.2/tadrep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/test/test_args.py` & `tadrep-0.9.2/test/test_args.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/test/test_blast.py` & `tadrep-0.9.2/test/test_blast.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/test/test_plasmids.py` & `tadrep-0.9.2/test/test_plasmids.py`

 * *Files identical despite different names*

### Comparing `tadrep-0.9.1/test/test_tadrep.py` & `tadrep-0.9.2/test/test_tadrep.py`

 * *Files identical despite different names*

