# Comparing `tmp/Ciw-3.1.4.tar.gz` & `tmp/ciw-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ciw-3.1.4.tar", last modified: Tue Apr  9 12:06:26 2024, max compression
+gzip compressed data, was "ciw-3.2.0.tar", last modified: Tue May  7 14:00:49 2024, max compression
```

## Comparing `Ciw-3.1.4.tar` & `ciw-3.2.0.tar`

### file list

```diff
@@ -1,225 +1,254 @@
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.414260 Ciw-3.1.4/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       43 2019-10-02 14:24:32.000000 Ciw-3.1.4/.gitattributes
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.047223 Ciw-3.1.4/.github/
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.074753 Ciw-3.1.4/.github/workflows/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1192 2023-08-22 13:40:54.000000 Ciw-3.1.4/.github/workflows/tests.yml
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      149 2023-08-22 13:40:54.000000 Ciw-3.1.4/.gitignore
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      733 2023-08-16 14:03:09.000000 Ciw-3.1.4/.readthedocs.yaml
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      984 2023-10-31 15:56:51.000000 Ciw-3.1.4/AUTHORS.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     9806 2024-04-09 12:01:17.000000 Ciw-3.1.4/CHANGES.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      597 2019-10-02 14:24:32.000000 Ciw-3.1.4/CITATION.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1514 2023-08-16 14:03:09.000000 Ciw-3.1.4/CONTRIBUTING.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.411595 Ciw-3.1.4/Ciw.egg-info/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    15034 2024-04-09 12:06:25.000000 Ciw-3.1.4/Ciw.egg-info/PKG-INFO
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     7189 2024-04-09 12:06:26.000000 Ciw-3.1.4/Ciw.egg-info/SOURCES.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)        1 2024-04-09 12:06:25.000000 Ciw-3.1.4/Ciw.egg-info/dependency_links.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       41 2024-04-09 12:06:26.000000 Ciw-3.1.4/Ciw.egg-info/requires.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)        4 2024-04-09 12:06:26.000000 Ciw-3.1.4/Ciw.egg-info/top_level.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1080 2019-10-02 14:24:32.000000 Ciw-3.1.4/LICENSE.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       56 2019-10-02 14:24:32.000000 Ciw-3.1.4/MANIFEST.in
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    15034 2024-04-09 12:06:26.412954 Ciw-3.1.4/PKG-INFO
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3854 2023-12-03 11:49:12.000000 Ciw-3.1.4/README.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.113919 Ciw-3.1.4/ciw/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      575 2023-12-03 11:30:34.000000 Ciw-3.1.4/ciw/__init__.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     6681 2024-04-04 09:45:57.000000 Ciw-3.1.4/ciw/arrival_node.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1770 2023-08-22 13:40:54.000000 Ciw-3.1.4/ciw/auxiliary.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      498 2023-08-22 13:40:54.000000 Ciw-3.1.4/ciw/data_record.py
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.115675 Ciw-3.1.4/ciw/deadlock/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/deadlock/__init__.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4446 2023-08-22 13:40:54.000000 Ciw-3.1.4/ciw/deadlock/deadlock_detector.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1361 2024-04-04 12:54:15.000000 Ciw-3.1.4/ciw/disciplines.py
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.117493 Ciw-3.1.4/ciw/dists/
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.051655 Ciw-3.1.4/ciw/dists/.hypothesis/
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.050960 Ciw-3.1.4/ciw/dists/.hypothesis/examples/
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.160286 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/097e547b92b91adb
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/0af454191959d613
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/1189a64b3a63541c
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/12acac2df3df48b6
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/24d6e7fc3069832b
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/4da15fd7a09586c7
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/550f5aa3832b4fc3
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/628039b293dd5254
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/668938c233269c64
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/7db861381701d4e1
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/7fc1725f753ed55f
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/9c29b872c797bf63
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       49 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/9d0de032dbc8ead3
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/b20d02d8f503a893
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/d08fa35e321f216d
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/d3be39602ef9c5c4
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/d8cccc4895f8a7c0
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/1a542554bc6caead/de3c78fe5b956e64
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.208478 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2823a3eaa9e3c5ba
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       28 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2a4930297c79ff33
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2cfb623d346ecd57
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2dbf20c932203d22
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/406bbe627cd1c44f
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/4119c7a3257670d6
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/44f025d4566fcf0c
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/48d7a891c63260e5
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5bde08a3480d1870
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5cbee9898702bbf5
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      197 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5d8a93fd16b829b5
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5e86df951ef52a16
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/601bbc65f8304262
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/7cd123fe7f4978f8
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/852cb323bed40f7d
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/b15db0ff5f98ebc2
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       37 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/ba81a7b179458d39
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/c3263c7fd9b5885f
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/c6327af1d657f71b
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/c7d326df3641c9fe
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/d4a3e75cd97512cf
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       41 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/da68315e076fdb9e
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/df6ee214f7db1f01
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/dfd06dd224d1ba64
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/ef3bdf5c7f89578a
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/f4cb653a6cb0fe75
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/f7823ac27f9552ef
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.052046 Ciw-3.1.4/ciw/dists/.hypothesis/unicodedata/
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.209524 Ciw-3.1.4/ciw/dists/.hypothesis/unicodedata/8.0.0/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    15457 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/.hypothesis/unicodedata/8.0.0/charmap.pickle.gz
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       29 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/dists/__init__.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    22936 2024-04-08 14:10:07.000000 Ciw-3.1.4/ciw/dists/distributions.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1896 2023-12-03 11:30:34.000000 Ciw-3.1.4/ciw/exactnode.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1046 2023-08-22 13:40:54.000000 Ciw-3.1.4/ciw/exit_node.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    16230 2024-04-08 22:07:37.000000 Ciw-3.1.4/ciw/import_params.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4108 2023-12-01 23:16:34.000000 Ciw-3.1.4/ciw/individual.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3663 2023-12-03 11:30:34.000000 Ciw-3.1.4/ciw/network.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    42213 2024-04-09 11:58:41.000000 Ciw-3.1.4/ciw/node.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4045 2023-12-03 11:30:34.000000 Ciw-3.1.4/ciw/processor_sharing.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5003 2024-04-03 14:32:52.000000 Ciw-3.1.4/ciw/schedules.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      851 2023-08-22 13:40:54.000000 Ciw-3.1.4/ciw/server.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    11587 2023-12-03 01:41:53.000000 Ciw-3.1.4/ciw/simulation.py
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.274840 Ciw-3.1.4/ciw/tests/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)        0 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/tests/__init__.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    21026 2023-08-22 13:40:54.000000 Ciw-3.1.4/ciw/tests/test_arrival_node.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3536 2023-08-22 13:40:54.000000 Ciw-3.1.4/ciw/tests/test_auxiliary.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5651 2023-08-22 13:40:55.000000 Ciw-3.1.4/ciw/tests/test_data_record.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1584 2023-08-22 13:40:55.000000 Ciw-3.1.4/ciw/tests/test_exit_node.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5146 2023-08-22 13:40:55.000000 Ciw-3.1.4/ciw/tests/test_individual.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    43757 2024-04-03 14:32:52.000000 Ciw-3.1.4/ciw/tests/test_network.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    86319 2024-04-04 12:54:15.000000 Ciw-3.1.4/ciw/tests/test_node.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    11284 2024-04-08 22:04:49.000000 Ciw-3.1.4/ciw/tests/test_process_based.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    31330 2023-12-03 11:30:34.000000 Ciw-3.1.4/ciw/tests/test_processor_sharing.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    67284 2024-04-03 14:32:52.000000 Ciw-3.1.4/ciw/tests/test_sampling.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    38818 2024-04-09 11:57:28.000000 Ciw-3.1.4/ciw/tests/test_scheduling.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5029 2023-08-22 13:40:55.000000 Ciw-3.1.4/ciw/tests/test_server.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    55060 2024-04-04 12:54:15.000000 Ciw-3.1.4/ciw/tests/test_simulation.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    70650 2023-08-22 13:40:55.000000 Ciw-3.1.4/ciw/tests/test_state_tracker.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      193 2023-08-17 16:01:41.000000 Ciw-3.1.4/ciw/tests/test_version.py
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.277258 Ciw-3.1.4/ciw/trackers/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       29 2019-10-02 14:24:32.000000 Ciw-3.1.4/ciw/trackers/__init__.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    14360 2024-04-03 14:32:52.000000 Ciw-3.1.4/ciw/trackers/state_tracker.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       22 2024-04-09 12:01:24.000000 Ciw-3.1.4/ciw/version.py
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.285996 Ciw-3.1.4/docs/
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.301511 Ciw-3.1.4/docs/Background/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      482 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/Background/codestructure.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      177 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/Background/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2071 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Background/kendall.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3038 2023-11-14 12:21:00.000000 Ciw-3.1.4/docs/Background/mechanisms.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      910 2024-04-03 14:32:52.000000 Ciw-3.1.4/docs/Background/other.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      658 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Background/references.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3482 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Background/simulationpractice.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.332777 Ciw-3.1.4/docs/Guides/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3866 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Guides/batching.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2991 2024-04-04 12:54:09.000000 Ciw-3.1.4/docs/Guides/baulking.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.341127 Ciw-3.1.4/docs/Guides/behaviour/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3160 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Guides/behaviour/custom_arrivals.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3330 2023-12-03 11:30:34.000000 Ciw-3.1.4/docs/Guides/behaviour/custom_number_servers.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3932 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Guides/behaviour/custom_routing.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     8332 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Guides/behaviour/hybrid.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1606 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Guides/behaviour/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3322 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Guides/behaviour/ps_routing.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4590 2023-08-17 09:42:42.000000 Ciw-3.1.4/docs/Guides/behaviour/server_dependent_dist.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2575 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Guides/change-class-after-service.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4157 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Guides/change-class-while-queueing.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2377 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Guides/deadlock.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      525 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Guides/dynamic_customerclasses.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1707 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Guides/exact.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      619 2023-12-03 11:30:34.000000 Ciw-3.1.4/docs/Guides/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2393 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Guides/parallel_process.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2121 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Guides/pause_restart.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     7318 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Guides/phasetype.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5003 2023-12-03 11:30:34.000000 Ciw-3.1.4/docs/Guides/preemption.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2810 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Guides/priority.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4600 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Guides/process_based.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     7125 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Guides/processor-sharing.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1144 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/Guides/progressbar.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4376 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Guides/reneging.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1524 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Guides/seed.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5564 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Guides/server_priority.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3251 2023-12-03 11:30:34.000000 Ciw-3.1.4/docs/Guides/server_schedule.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3504 2024-04-04 12:54:15.000000 Ciw-3.1.4/docs/Guides/service_disciplines.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     8988 2024-04-03 14:32:52.000000 Ciw-3.1.4/docs/Guides/set_distributions.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2115 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Guides/sim_numcusts.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3880 2023-12-03 11:30:34.000000 Ciw-3.1.4/docs/Guides/slotted.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3080 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Guides/state_trackers.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     9506 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Guides/time_dependent.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     7413 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/Makefile
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.353321 Ciw-3.1.4/docs/Reference/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       69 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/Reference/authors.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       78 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/Reference/changelog.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1494 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Reference/citation.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      109 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/Reference/contributing.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    10862 2024-04-03 14:32:52.000000 Ciw-3.1.4/docs/Reference/distributions.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3561 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/Reference/glossary.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      225 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/Reference/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     6083 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Reference/parameters.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3254 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Reference/results.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5378 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Reference/state_trackers.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.359124 Ciw-3.1.4/docs/Tutorial-I/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      237 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/Tutorial-I/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3004 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Tutorial-I/tutorial_i.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2993 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/Tutorial-I/tutorial_ii.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     3339 2023-11-14 12:21:00.000000 Ciw-3.1.4/docs/Tutorial-I/tutorial_iii.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4434 2023-11-14 12:22:13.000000 Ciw-3.1.4/docs/Tutorial-I/tutorial_iv.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.363745 Ciw-3.1.4/docs/Tutorial-II/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      320 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/Tutorial-II/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4708 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Tutorial-II/tutorial_v.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5637 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Tutorial-II/tutorial_vi.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     5535 2023-08-22 13:40:55.000000 Ciw-3.1.4/docs/Tutorial-II/tutorial_vii.rst
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.407912 Ciw-3.1.4/docs/_static/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    17655 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/_static/2nodes.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)   116215 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/_static/2nodesindeadlock.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    14663 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/_static/cafe.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    65346 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/_static/codestructure.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4968 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/_static/codestructure.tex
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    27837 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/coxian.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    15838 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/custom_number_servers_with.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    16887 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/custom_number_servers_without.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    74719 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/custom_routing_with.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    71055 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/custom_routing_without.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    95903 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/des+sd_hybrid.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     8422 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/erlang.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     4286 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/_static/favicon.ico
--rw-r--r--   0 geraintpalmer   (502) staff       (20)   207124 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/hybrid.png
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    46236 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/hypererlang.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    15698 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/hyperexponential.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     2603 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/_static/logo.pdf
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     8889 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/_static/logo.png
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     1561 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/_static/logo.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)     7299 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/_static/logo_small.png
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    20608 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/phasetype.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    21468 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/_static/progress_bar_customers.png
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    22909 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/_static/progress_bar_time.png
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    32489 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/ps_capacitated_verification.svg
-drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-04-09 12:06:26.410264 Ciw-3.1.4/docs/_static/script_for_parallel_processing/
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      214 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/script_for_parallel_processing/README.md
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      823 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/script_for_parallel_processing/main.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    48896 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/server_dependent_dist_with.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    37013 2023-08-16 14:03:09.000000 Ciw-3.1.4/docs/_static/server_dependent_dist_without.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      194 2023-08-22 16:10:56.000000 Ciw-3.1.4/docs/_static/style.css
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    14539 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/_static/tutorial_iii_waitshist.svg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)    10027 2023-08-22 16:30:04.000000 Ciw-3.1.4/docs/conf.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      891 2023-12-03 11:38:09.000000 Ciw-3.1.4/docs/index.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      299 2019-10-02 14:24:32.000000 Ciw-3.1.4/docs/installation.rst
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       20 2024-04-03 14:32:52.000000 Ciw-3.1.4/docs/requirements.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      492 2023-08-22 13:40:55.000000 Ciw-3.1.4/doctests.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      322 2023-08-16 14:03:09.000000 Ciw-3.1.4/new_release_checklist.md
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       40 2023-08-22 13:40:55.000000 Ciw-3.1.4/requirements.txt
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       38 2024-04-09 12:06:26.414495 Ciw-3.1.4/setup.cfg
--rw-r--r--   0 geraintpalmer   (502) staff       (20)      956 2023-08-22 13:40:55.000000 Ciw-3.1.4/setup.py
--rw-r--r--   0 geraintpalmer   (502) staff       (20)       55 2023-08-22 13:40:55.000000 Ciw-3.1.4/test_requirements.txt
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.199509 ciw-3.2.0/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       43 2019-10-02 14:24:32.000000 ciw-3.2.0/.gitattributes
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:48.851245 ciw-3.2.0/.github/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:48.879516 ciw-3.2.0/.github/workflows/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1193 2024-05-07 13:44:53.000000 ciw-3.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      149 2023-08-22 13:40:54.000000 ciw-3.2.0/.gitignore
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      733 2023-08-16 14:03:09.000000 ciw-3.2.0/.readthedocs.yaml
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      984 2023-10-31 15:56:51.000000 ciw-3.2.0/AUTHORS.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    10473 2024-05-07 13:54:31.000000 ciw-3.2.0/CHANGES.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      597 2019-10-02 14:24:32.000000 ciw-3.2.0/CITATION.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1514 2023-08-16 14:03:09.000000 ciw-3.2.0/CONTRIBUTING.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.195927 ciw-3.2.0/Ciw.egg-info/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    16186 2024-05-07 14:00:48.000000 ciw-3.2.0/Ciw.egg-info/PKG-INFO
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     8201 2024-05-07 14:00:48.000000 ciw-3.2.0/Ciw.egg-info/SOURCES.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)        1 2024-05-07 14:00:48.000000 ciw-3.2.0/Ciw.egg-info/dependency_links.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       56 2024-05-07 14:00:48.000000 ciw-3.2.0/Ciw.egg-info/requires.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)        4 2024-05-07 14:00:48.000000 ciw-3.2.0/Ciw.egg-info/top_level.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1080 2019-10-02 14:24:32.000000 ciw-3.2.0/LICENSE.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       56 2019-10-02 14:24:32.000000 ciw-3.2.0/MANIFEST.in
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    16186 2024-05-07 14:00:49.197865 ciw-3.2.0/PKG-INFO
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4309 2024-05-07 13:44:53.000000 ciw-3.2.0/README.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:48.900138 ciw-3.2.0/ciw/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      575 2023-12-03 11:30:34.000000 ciw-3.2.0/ciw/__init__.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     6780 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/arrival_node.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1770 2023-08-22 13:40:54.000000 ciw-3.2.0/ciw/auxiliary.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      498 2023-08-22 13:40:54.000000 ciw-3.2.0/ciw/data_record.py
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:48.901597 ciw-3.2.0/ciw/deadlock/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/deadlock/__init__.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4446 2023-08-22 13:40:54.000000 ciw-3.2.0/ciw/deadlock/deadlock_detector.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1361 2024-04-04 12:54:15.000000 ciw-3.2.0/ciw/disciplines.py
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:48.909085 ciw-3.2.0/ciw/dists/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:48.857147 ciw-3.2.0/ciw/dists/.hypothesis/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:48.856876 ciw-3.2.0/ciw/dists/.hypothesis/examples/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:48.937704 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/097e547b92b91adb
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/0af454191959d613
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/1189a64b3a63541c
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/12acac2df3df48b6
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/24d6e7fc3069832b
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/4da15fd7a09586c7
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/550f5aa3832b4fc3
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/628039b293dd5254
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/668938c233269c64
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/7db861381701d4e1
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/7fc1725f753ed55f
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/9c29b872c797bf63
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       49 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/9d0de032dbc8ead3
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/b20d02d8f503a893
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/d08fa35e321f216d
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/d3be39602ef9c5c4
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/d8cccc4895f8a7c0
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       33 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/1a542554bc6caead/de3c78fe5b956e64
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:48.980003 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2823a3eaa9e3c5ba
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       28 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2a4930297c79ff33
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2cfb623d346ecd57
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/2dbf20c932203d22
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/406bbe627cd1c44f
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/4119c7a3257670d6
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/44f025d4566fcf0c
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/48d7a891c63260e5
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5bde08a3480d1870
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5cbee9898702bbf5
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      197 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5d8a93fd16b829b5
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/5e86df951ef52a16
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/601bbc65f8304262
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/7cd123fe7f4978f8
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/852cb323bed40f7d
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/b15db0ff5f98ebc2
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       37 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/ba81a7b179458d39
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/c3263c7fd9b5885f
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/c6327af1d657f71b
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/c7d326df3641c9fe
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/d4a3e75cd97512cf
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       41 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/da68315e076fdb9e
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/df6ee214f7db1f01
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/dfd06dd224d1ba64
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/ef3bdf5c7f89578a
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/f4cb653a6cb0fe75
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       26 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/examples/3144b0e1d2aac2fd/f7823ac27f9552ef
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:48.857347 ciw-3.2.0/ciw/dists/.hypothesis/unicodedata/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:48.983435 ciw-3.2.0/ciw/dists/.hypothesis/unicodedata/8.0.0/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    15457 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/.hypothesis/unicodedata/8.0.0/charmap.pickle.gz
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       29 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/dists/__init__.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    22936 2024-04-08 14:10:07.000000 ciw-3.2.0/ciw/dists/distributions.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1896 2023-12-03 11:30:34.000000 ciw-3.2.0/ciw/exactnode.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1046 2024-04-12 13:00:47.000000 ciw-3.2.0/ciw/exit_node.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    13922 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/import_params.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4108 2023-12-01 23:16:34.000000 ciw-3.2.0/ciw/individual.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3663 2023-12-03 11:30:34.000000 ciw-3.2.0/ciw/network.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    42076 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/node.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4045 2023-12-03 11:30:34.000000 ciw-3.2.0/ciw/processor_sharing.py
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:48.988525 ciw-3.2.0/ciw/routing/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       23 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/routing/__init__.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    11353 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/routing/routing.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5700 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/schedules.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      851 2023-08-22 13:40:54.000000 ciw-3.2.0/ciw/server.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    12223 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/simulation.py
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.008284 ciw-3.2.0/ciw/tests/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)        0 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/tests/__init__.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    21026 2023-08-22 13:40:54.000000 ciw-3.2.0/ciw/tests/test_arrival_node.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3536 2023-08-22 13:40:54.000000 ciw-3.2.0/ciw/tests/test_auxiliary.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5651 2023-08-22 13:40:55.000000 ciw-3.2.0/ciw/tests/test_data_record.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1584 2023-08-22 13:40:55.000000 ciw-3.2.0/ciw/tests/test_exit_node.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5146 2023-08-22 13:40:55.000000 ciw-3.2.0/ciw/tests/test_individual.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    50250 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/tests/test_network.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    86505 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/tests/test_node.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    10552 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/tests/test_process_based.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    32987 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/tests/test_processor_sharing.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    14818 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/tests/test_routing.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    67284 2024-04-03 14:32:52.000000 ciw-3.2.0/ciw/tests/test_sampling.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    42360 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/tests/test_scheduling.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5029 2023-08-22 13:40:55.000000 ciw-3.2.0/ciw/tests/test_server.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    73621 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/tests/test_simulation.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    74427 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/tests/test_state_tracker.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      193 2023-08-17 16:01:41.000000 ciw-3.2.0/ciw/tests/test_version.py
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.010264 ciw-3.2.0/ciw/trackers/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       29 2019-10-02 14:24:32.000000 ciw-3.2.0/ciw/trackers/__init__.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    16232 2024-05-07 13:44:53.000000 ciw-3.2.0/ciw/trackers/state_tracker.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       22 2024-05-07 13:47:21.000000 ciw-3.2.0/ciw/version.py
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.016970 ciw-3.2.0/docs/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.042183 ciw-3.2.0/docs/Background/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      156 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Background/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2071 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/Background/kendall.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1988 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Background/mechanisms.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      910 2024-04-03 14:32:52.000000 ciw-3.2.0/docs/Background/other.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      736 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Background/references.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3493 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Background/simulationpractice.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.045219 ciw-3.2.0/docs/Guides/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.047599 ciw-3.2.0/docs/Guides/Arrivals/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3866 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Arrivals/batching.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       76 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Arrivals/index.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.050243 ciw-3.2.0/docs/Guides/CustomerBehaviour/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2991 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/CustomerBehaviour/baulking.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      112 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/CustomerBehaviour/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4384 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/CustomerBehaviour/reneging.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.054964 ciw-3.2.0/docs/Guides/CustomerClasses/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2575 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/CustomerClasses/change-class-after-service.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4157 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/CustomerClasses/change-class-while-queueing.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3544 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/CustomerClasses/customer-classes.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      185 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/CustomerClasses/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2748 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/CustomerClasses/priority.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.060235 ciw-3.2.0/docs/Guides/Distributions/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2980 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Distributions/combining_distributions.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      165 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Distributions/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     7333 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Distributions/phasetype.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     6327 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Distributions/set_distributions.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     9506 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Distributions/time_dependent.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.063566 ciw-3.2.0/docs/Guides/Queues/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      103 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Queues/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5117 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Queues/queue_capacities.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1745 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Queues/system_capacity.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.075178 ciw-3.2.0/docs/Guides/Routing/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5490 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Routing/custom_routing.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      181 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Routing/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     7682 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Routing/join_shortest_queue.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     8673 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Routing/process_based.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4614 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Routing/routing_objects.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3043 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Routing/transition_matrix.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.103711 ciw-3.2.0/docs/Guides/Services/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      191 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Services/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     6158 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Services/preemption.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     7128 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Services/processor-sharing.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5500 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Services/server_priority.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5075 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Services/server_schedule.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3505 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Services/service_disciplines.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5438 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Services/slotted.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.111082 ciw-3.2.0/docs/Guides/Simulation/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1707 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Simulation/exact.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      207 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Simulation/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2399 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Simulation/parallel_process.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2121 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Simulation/pause_restart.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1150 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Simulation/progressbar.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3517 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Simulation/results.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1524 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Simulation/seed.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1415 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Simulation/sim_maxtime.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2115 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/Simulation/sim_numcusts.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.113528 ciw-3.2.0/docs/Guides/System/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.118286 ciw-3.2.0/docs/Guides/System/behaviour/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3160 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/System/behaviour/custom_arrivals.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3336 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/System/behaviour/custom_number_servers.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     8338 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/System/behaviour/hybrid.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1566 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/System/behaviour/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4596 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/System/behaviour/server_dependent_dist.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2380 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/System/deadlock.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      117 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/System/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3080 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/System/state_trackers.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      456 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Guides/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     7413 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/Makefile
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.129058 ciw-3.2.0/docs/Reference/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       69 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/Reference/authors.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       78 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/Reference/changelog.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1494 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/Reference/citation.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      109 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/Reference/contributing.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    10862 2024-04-03 14:32:52.000000 ciw-3.2.0/docs/Reference/distributions.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3561 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/Reference/glossary.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      240 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Reference/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     8722 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Reference/parameters.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3256 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Reference/results.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5775 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Reference/routers.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     6571 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Reference/state_trackers.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.133210 ciw-3.2.0/docs/Tutorial/
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.139181 ciw-3.2.0/docs/Tutorial/GettingStarted/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      158 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Tutorial/GettingStarted/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3030 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Tutorial/GettingStarted/part_1.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3012 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Tutorial/GettingStarted/part_2.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     3352 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Tutorial/GettingStarted/part_3.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4448 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Tutorial/GettingStarted/part_4.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      436 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Tutorial/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4712 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Tutorial/tutorial_ii.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5641 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Tutorial/tutorial_iii.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     5531 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/Tutorial/tutorial_iv.rst
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.187270 ciw-3.2.0/docs/_static/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    17655 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/_static/2nodes.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)   116215 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/_static/2nodesindeadlock.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    14663 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/_static/cafe.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    65346 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/_static/codestructure.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4968 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/_static/codestructure.tex
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    27837 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/coxian.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    15838 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/custom_number_servers_with.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    16887 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/custom_number_servers_without.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    63764 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/_static/custom_routing_with.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    63474 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/_static/custom_routing_without.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    95903 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/des+sd_hybrid.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     8422 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/erlang.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     4286 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)   207124 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/hybrid.png
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    46236 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/hypererlang.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    15698 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/hyperexponential.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     2603 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/_static/logo.pdf
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     8889 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/_static/logo.png
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     1561 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/_static/logo.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)     7299 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/_static/logo_small.png
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    20608 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/phasetype.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    21468 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/_static/progress_bar_customers.png
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    22909 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/_static/progress_bar_time.png
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    32489 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/ps_capacitated_verification.svg
+drwxr-xr-x   0 geraintpalmer   (502) staff       (20)        0 2024-05-07 14:00:49.192671 ciw-3.2.0/docs/_static/script_for_parallel_processing/
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      214 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/script_for_parallel_processing/README.md
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      823 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/script_for_parallel_processing/main.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    48896 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/server_dependent_dist_with.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    37013 2023-08-16 14:03:09.000000 ciw-3.2.0/docs/_static/server_dependent_dist_without.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      233 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/_static/style.css
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    14539 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/_static/tutorial_iii_waitshist.svg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)    10027 2024-04-26 12:05:43.000000 ciw-3.2.0/docs/conf.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      865 2024-05-07 13:44:53.000000 ciw-3.2.0/docs/index.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      299 2019-10-02 14:24:32.000000 ciw-3.2.0/docs/installation.rst
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       20 2024-04-26 14:54:05.000000 ciw-3.2.0/docs/requirements.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      492 2023-08-22 13:40:55.000000 ciw-3.2.0/doctests.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      322 2023-08-16 14:03:09.000000 ciw-3.2.0/new_release_checklist.md
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       55 2024-05-07 13:44:53.000000 ciw-3.2.0/requirements.txt
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       38 2024-05-07 14:00:49.199724 ciw-3.2.0/setup.cfg
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)      956 2024-04-26 15:06:50.000000 ciw-3.2.0/setup.py
+-rw-r--r--   0 geraintpalmer   (502) staff       (20)       55 2023-08-22 13:40:55.000000 ciw-3.2.0/test_requirements.txt
```

### Comparing `Ciw-3.1.4/.github/workflows/tests.yml` & `ciw-3.2.0/.github/workflows/tests.yml`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macOS-latest, windows-latest]
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `Ciw-3.1.4/.readthedocs.yaml` & `ciw-3.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/AUTHORS.rst` & `ciw-3.2.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/CHANGES.rst` & `ciw-3.2.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 History
 -------
 
++ **3.2.0 (2024-05-07)**
+    + System capacity implemented.
+    + Server schedules objects now take `numbers_of_servers` and `shift_end_dates` keywards, instead of `schedule`.
+    + Server schedules and slotted services can be `offset`.
+    + Added a GroupedNodePopulation tracker.
+    + Restructures documentation, adds more guides, and updates reference pages.
+    + Routing objects implemented: TransitionMatrix object, ProcessBased object, FlexibleProcessBased object, NetworkRouting object, Direct object, Leave object, Probabilistic object, JoinShortestQueue object, LoadBalancing object
+    + Added `reroute` as an option for interrupted preemptive services.
+
 + **3.1.4 (2024-04-09)**
     + Fix bug where Individual's server isn't reset after a slotted service.
 
 + **3.1.3 (2024-04-08)**
     + Allows class methods as generator functions for process-based routing.
 
 + **3.1.2 (2024-04-08)**
```

### Comparing `Ciw-3.1.4/CITATION.rst` & `ciw-3.2.0/CITATION.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/CONTRIBUTING.rst` & `ciw-3.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/Ciw.egg-info/PKG-INFO` & `ciw-3.2.0/Ciw.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: Ciw
-Version: 3.1.4
+Version: 3.2.0
 Summary: A discrete event simulation library for open queueing networks
 Home-page: https://github.com/CiwPython/Ciw
 Author: Geraint Palmer, Vincent Knight
 Author-email: palmer.geraint@googlemail.com
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
+Requires-Dist: setuptools>=69
 Requires-Dist: networkx>=2.3
 Requires-Dist: tqdm>=4.64.0
 Requires-Dist: numpy>=1.21.6
 
 Ciw
 ===
 
@@ -41,19 +42,19 @@
 - `Contribution guidelines <https://github.com/CiwPython/Ciw/blob/master/CONTRIBUTING.rst>`_
 - `Our great contributors <https://github.com/CiwPython/Ciw/blob/master/AUTHORS.rst>`_
 
 Install with :code:`pip install ciw`.
 
 Current supported version of Python:
 
-- Python 3.7
 - Python 3.8
 - Python 3.9
 - Python 3.10
 - Python 3.11
+- Python 3.12
 
 Usage
 -----
 
 Import Ciw::
 
     >>> import ciw
@@ -84,39 +85,50 @@
 
 
 Features
 --------
 
 A number of other features are also implemented, including:
 
-+ `Type I blocking <https://ciw.readthedocs.io/en/latest/Tutorial-II/tutorial_vi.html>`_
++ `Type I blocking <https://ciw.readthedocs.io/en/latest/Guides/Queues/queue_capacities.html>`_
 + `A large range of sampling distributions <https://ciw.readthedocs.io/en/latest/Reference/distributions.html>`_
-+ `Phase-Type distributions <https://ciw.readthedocs.io/en/latest/Guides/phasetype.html>`_
-+ `Time-dependent and state-dependent distributions <https://ciw.readthedocs.io/en/latest/Guides/time_dependent.html>`_
-+ `Batch arrivals <https://ciw.readthedocs.io/en/latest/Guides/batching.html>`_
-+ `Baulking customers <https://ciw.readthedocs.io/en/latest/Guides/baulking.html>`_
-+ `Reneging customers <https://ciw.readthedocs.io/en/latest/Guides/reneging.html>`_
-+ `Processor sharing <https://ciw.readthedocs.io/en/latest/Guides/processor-sharing.html>`_
-+ `Multiple customer classes <https://ciw.readthedocs.io/en/latest/Tutorial-II/tutorial_vii.html>`_
-+ `Priorities <https://ciw.readthedocs.io/en/latest/Guides/priority.html>`_
-+ `Server priorities <https://ciw.readthedocs.io/en/latest/Guides/server_priority.html>`_
-+ `Service disciplines <https://ciw.readthedocs.io/en/latest/Guides/service_disciplines.html>`_
-+ `Customers changing classes <https://ciw.readthedocs.io/en/latest/Guides/dynamic_customerclasses.html>`_
-+ `Server schedules <https://ciw.readthedocs.io/en/latest/Guides/server_schedule.html>`_
-+ `Slotted services <https://ciw.readthedocs.io/en/latest/Guides/slotted.html>`_
-+ `State tracking <https://ciw.readthedocs.io/en/latest/Guides/state_trackers.html>`_
-+ `Stopping the simulation after a certain amount of customers <https://ciw.readthedocs.io/en/latest/Guides/sim_numcusts.html>`_
-+ `Process-based routing <https://ciw.readthedocs.io/en/latest/Guides/process_based.html>`_
-+ `Deadlock detection <https://ciw.readthedocs.io/en/latest/Guides/deadlock.html>`_
++ `Phase-Type distributions <https://ciw.readthedocs.io/en/latest/Guides/Distributions/phasetype.html>`_
++ `Time-dependent and state-dependent distributions <https://ciw.readthedocs.io/en/latest/Guides/Distributions/time_dependent.html>`_
++ `Batch arrivals <https://ciw.readthedocs.io/en/latest/Guides/Arrivals/batching.html>`_
++ `Baulking customers <https://ciw.readthedocs.io/en/latest/Guides/CustomerBehaviour/baulking.html>`_
++ `Reneging customers <https://ciw.readthedocs.io/en/latest/Guides/CustomerBehaviour/reneging.html>`_
++ `Processor sharing <https://ciw.readthedocs.io/en/latest/Guides/Services/processor-sharing.html>`_
++ `Multiple customer classes <https://ciw.readthedocs.io/en/latest/Guides/CustomerClasses/customer-classes.html>`_
++ `Priorities <https://ciw.readthedocs.io/en/latest/Guides/CustomerClasses/priority.html>`_
++ `Server priorities <https://ciw.readthedocs.io/en/latest/Guides/Services/server_priority.html>`_
++ `Service disciplines <https://ciw.readthedocs.io/en/latest/Guides/Services/service_disciplines.html>`_
++ `Customers changing classes while queueing <https://ciw.readthedocs.io/en/latest/Guides/CustomerClasses/change-class-while-queueing.html>`_
++ `Customers changing classes after service <https://ciw.readthedocs.io/en/latest/Guides/CustomerClasses/change-class-after-service.html>`_
++ `Server schedules <https://ciw.readthedocs.io/en/latest/Guides/Services/server_schedule.html>`_
++ `Slotted services <https://ciw.readthedocs.io/en/latest/Guides/Services/slotted.html>`_
++ `State tracking <https://ciw.readthedocs.io/en/latest/Guides/System/state_trackers.html>`_
++ `Stopping the simulation after a certain amount of customers <https://ciw.readthedocs.io/en/latest/Guides/Simulation/sim_numcusts.html>`_
++ `Process-based routing <https://ciw.readthedocs.io/en/latest/Guides/Routing/process_based.html>`_
++ `Logical routing <https://ciw.readthedocs.io/en/latest/Guides/Reference/routers.html>`_
++ `Deadlock detection <https://ciw.readthedocs.io/en/latest/Guides/System/deadlock.html>`_
 
 
 
 History
 -------
 
++ **3.2.0 (2024-05-07)**
+    + System capacity implemented.
+    + Server schedules objects now take `numbers_of_servers` and `shift_end_dates` keywards, instead of `schedule`.
+    + Server schedules and slotted services can be `offset`.
+    + Added a GroupedNodePopulation tracker.
+    + Restructures documentation, adds more guides, and updates reference pages.
+    + Routing objects implemented: TransitionMatrix object, ProcessBased object, FlexibleProcessBased object, NetworkRouting object, Direct object, Leave object, Probabilistic object, JoinShortestQueue object, LoadBalancing object
+    + Added `reroute` as an option for interrupted preemptive services.
+
 + **3.1.4 (2024-04-09)**
     + Fix bug where Individual's server isn't reset after a slotted service.
 
 + **3.1.3 (2024-04-08)**
     + Allows class methods as generator functions for process-based routing.
 
 + **3.1.2 (2024-04-08)**
```

### Comparing `Ciw-3.1.4/LICENSE.txt` & `ciw-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/PKG-INFO` & `ciw-3.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: Ciw
-Version: 3.1.4
+Version: 3.2.0
 Summary: A discrete event simulation library for open queueing networks
 Home-page: https://github.com/CiwPython/Ciw
 Author: Geraint Palmer, Vincent Knight
 Author-email: palmer.geraint@googlemail.com
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
+Requires-Dist: setuptools>=69
 Requires-Dist: networkx>=2.3
 Requires-Dist: tqdm>=4.64.0
 Requires-Dist: numpy>=1.21.6
 
 Ciw
 ===
 
@@ -41,19 +42,19 @@
 - `Contribution guidelines <https://github.com/CiwPython/Ciw/blob/master/CONTRIBUTING.rst>`_
 - `Our great contributors <https://github.com/CiwPython/Ciw/blob/master/AUTHORS.rst>`_
 
 Install with :code:`pip install ciw`.
 
 Current supported version of Python:
 
-- Python 3.7
 - Python 3.8
 - Python 3.9
 - Python 3.10
 - Python 3.11
+- Python 3.12
 
 Usage
 -----
 
 Import Ciw::
 
     >>> import ciw
@@ -84,39 +85,50 @@
 
 
 Features
 --------
 
 A number of other features are also implemented, including:
 
-+ `Type I blocking <https://ciw.readthedocs.io/en/latest/Tutorial-II/tutorial_vi.html>`_
++ `Type I blocking <https://ciw.readthedocs.io/en/latest/Guides/Queues/queue_capacities.html>`_
 + `A large range of sampling distributions <https://ciw.readthedocs.io/en/latest/Reference/distributions.html>`_
-+ `Phase-Type distributions <https://ciw.readthedocs.io/en/latest/Guides/phasetype.html>`_
-+ `Time-dependent and state-dependent distributions <https://ciw.readthedocs.io/en/latest/Guides/time_dependent.html>`_
-+ `Batch arrivals <https://ciw.readthedocs.io/en/latest/Guides/batching.html>`_
-+ `Baulking customers <https://ciw.readthedocs.io/en/latest/Guides/baulking.html>`_
-+ `Reneging customers <https://ciw.readthedocs.io/en/latest/Guides/reneging.html>`_
-+ `Processor sharing <https://ciw.readthedocs.io/en/latest/Guides/processor-sharing.html>`_
-+ `Multiple customer classes <https://ciw.readthedocs.io/en/latest/Tutorial-II/tutorial_vii.html>`_
-+ `Priorities <https://ciw.readthedocs.io/en/latest/Guides/priority.html>`_
-+ `Server priorities <https://ciw.readthedocs.io/en/latest/Guides/server_priority.html>`_
-+ `Service disciplines <https://ciw.readthedocs.io/en/latest/Guides/service_disciplines.html>`_
-+ `Customers changing classes <https://ciw.readthedocs.io/en/latest/Guides/dynamic_customerclasses.html>`_
-+ `Server schedules <https://ciw.readthedocs.io/en/latest/Guides/server_schedule.html>`_
-+ `Slotted services <https://ciw.readthedocs.io/en/latest/Guides/slotted.html>`_
-+ `State tracking <https://ciw.readthedocs.io/en/latest/Guides/state_trackers.html>`_
-+ `Stopping the simulation after a certain amount of customers <https://ciw.readthedocs.io/en/latest/Guides/sim_numcusts.html>`_
-+ `Process-based routing <https://ciw.readthedocs.io/en/latest/Guides/process_based.html>`_
-+ `Deadlock detection <https://ciw.readthedocs.io/en/latest/Guides/deadlock.html>`_
++ `Phase-Type distributions <https://ciw.readthedocs.io/en/latest/Guides/Distributions/phasetype.html>`_
++ `Time-dependent and state-dependent distributions <https://ciw.readthedocs.io/en/latest/Guides/Distributions/time_dependent.html>`_
++ `Batch arrivals <https://ciw.readthedocs.io/en/latest/Guides/Arrivals/batching.html>`_
++ `Baulking customers <https://ciw.readthedocs.io/en/latest/Guides/CustomerBehaviour/baulking.html>`_
++ `Reneging customers <https://ciw.readthedocs.io/en/latest/Guides/CustomerBehaviour/reneging.html>`_
++ `Processor sharing <https://ciw.readthedocs.io/en/latest/Guides/Services/processor-sharing.html>`_
++ `Multiple customer classes <https://ciw.readthedocs.io/en/latest/Guides/CustomerClasses/customer-classes.html>`_
++ `Priorities <https://ciw.readthedocs.io/en/latest/Guides/CustomerClasses/priority.html>`_
++ `Server priorities <https://ciw.readthedocs.io/en/latest/Guides/Services/server_priority.html>`_
++ `Service disciplines <https://ciw.readthedocs.io/en/latest/Guides/Services/service_disciplines.html>`_
++ `Customers changing classes while queueing <https://ciw.readthedocs.io/en/latest/Guides/CustomerClasses/change-class-while-queueing.html>`_
++ `Customers changing classes after service <https://ciw.readthedocs.io/en/latest/Guides/CustomerClasses/change-class-after-service.html>`_
++ `Server schedules <https://ciw.readthedocs.io/en/latest/Guides/Services/server_schedule.html>`_
++ `Slotted services <https://ciw.readthedocs.io/en/latest/Guides/Services/slotted.html>`_
++ `State tracking <https://ciw.readthedocs.io/en/latest/Guides/System/state_trackers.html>`_
++ `Stopping the simulation after a certain amount of customers <https://ciw.readthedocs.io/en/latest/Guides/Simulation/sim_numcusts.html>`_
++ `Process-based routing <https://ciw.readthedocs.io/en/latest/Guides/Routing/process_based.html>`_
++ `Logical routing <https://ciw.readthedocs.io/en/latest/Guides/Reference/routers.html>`_
++ `Deadlock detection <https://ciw.readthedocs.io/en/latest/Guides/System/deadlock.html>`_
 
 
 
 History
 -------
 
++ **3.2.0 (2024-05-07)**
+    + System capacity implemented.
+    + Server schedules objects now take `numbers_of_servers` and `shift_end_dates` keywards, instead of `schedule`.
+    + Server schedules and slotted services can be `offset`.
+    + Added a GroupedNodePopulation tracker.
+    + Restructures documentation, adds more guides, and updates reference pages.
+    + Routing objects implemented: TransitionMatrix object, ProcessBased object, FlexibleProcessBased object, NetworkRouting object, Direct object, Leave object, Probabilistic object, JoinShortestQueue object, LoadBalancing object
+    + Added `reroute` as an option for interrupted preemptive services.
+
 + **3.1.4 (2024-04-09)**
     + Fix bug where Individual's server isn't reset after a slotted service.
 
 + **3.1.3 (2024-04-08)**
     + Allows class methods as generator functions for process-based routing.
 
 + **3.1.2 (2024-04-08)**
```

### Comparing `Ciw-3.1.4/README.rst` & `ciw-3.2.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 - `Contribution guidelines <https://github.com/CiwPython/Ciw/blob/master/CONTRIBUTING.rst>`_
 - `Our great contributors <https://github.com/CiwPython/Ciw/blob/master/AUTHORS.rst>`_
 
 Install with :code:`pip install ciw`.
 
 Current supported version of Python:
 
-- Python 3.7
 - Python 3.8
 - Python 3.9
 - Python 3.10
 - Python 3.11
+- Python 3.12
 
 Usage
 -----
 
 Import Ciw::
 
     >>> import ciw
@@ -71,27 +71,29 @@
 
 
 Features
 --------
 
 A number of other features are also implemented, including:
 
-+ `Type I blocking <https://ciw.readthedocs.io/en/latest/Tutorial-II/tutorial_vi.html>`_
++ `Type I blocking <https://ciw.readthedocs.io/en/latest/Guides/Queues/queue_capacities.html>`_
 + `A large range of sampling distributions <https://ciw.readthedocs.io/en/latest/Reference/distributions.html>`_
-+ `Phase-Type distributions <https://ciw.readthedocs.io/en/latest/Guides/phasetype.html>`_
-+ `Time-dependent and state-dependent distributions <https://ciw.readthedocs.io/en/latest/Guides/time_dependent.html>`_
-+ `Batch arrivals <https://ciw.readthedocs.io/en/latest/Guides/batching.html>`_
-+ `Baulking customers <https://ciw.readthedocs.io/en/latest/Guides/baulking.html>`_
-+ `Reneging customers <https://ciw.readthedocs.io/en/latest/Guides/reneging.html>`_
-+ `Processor sharing <https://ciw.readthedocs.io/en/latest/Guides/processor-sharing.html>`_
-+ `Multiple customer classes <https://ciw.readthedocs.io/en/latest/Tutorial-II/tutorial_vii.html>`_
-+ `Priorities <https://ciw.readthedocs.io/en/latest/Guides/priority.html>`_
-+ `Server priorities <https://ciw.readthedocs.io/en/latest/Guides/server_priority.html>`_
-+ `Service disciplines <https://ciw.readthedocs.io/en/latest/Guides/service_disciplines.html>`_
-+ `Customers changing classes <https://ciw.readthedocs.io/en/latest/Guides/dynamic_customerclasses.html>`_
-+ `Server schedules <https://ciw.readthedocs.io/en/latest/Guides/server_schedule.html>`_
-+ `Slotted services <https://ciw.readthedocs.io/en/latest/Guides/slotted.html>`_
-+ `State tracking <https://ciw.readthedocs.io/en/latest/Guides/state_trackers.html>`_
-+ `Stopping the simulation after a certain amount of customers <https://ciw.readthedocs.io/en/latest/Guides/sim_numcusts.html>`_
-+ `Process-based routing <https://ciw.readthedocs.io/en/latest/Guides/process_based.html>`_
-+ `Deadlock detection <https://ciw.readthedocs.io/en/latest/Guides/deadlock.html>`_
++ `Phase-Type distributions <https://ciw.readthedocs.io/en/latest/Guides/Distributions/phasetype.html>`_
++ `Time-dependent and state-dependent distributions <https://ciw.readthedocs.io/en/latest/Guides/Distributions/time_dependent.html>`_
++ `Batch arrivals <https://ciw.readthedocs.io/en/latest/Guides/Arrivals/batching.html>`_
++ `Baulking customers <https://ciw.readthedocs.io/en/latest/Guides/CustomerBehaviour/baulking.html>`_
++ `Reneging customers <https://ciw.readthedocs.io/en/latest/Guides/CustomerBehaviour/reneging.html>`_
++ `Processor sharing <https://ciw.readthedocs.io/en/latest/Guides/Services/processor-sharing.html>`_
++ `Multiple customer classes <https://ciw.readthedocs.io/en/latest/Guides/CustomerClasses/customer-classes.html>`_
++ `Priorities <https://ciw.readthedocs.io/en/latest/Guides/CustomerClasses/priority.html>`_
++ `Server priorities <https://ciw.readthedocs.io/en/latest/Guides/Services/server_priority.html>`_
++ `Service disciplines <https://ciw.readthedocs.io/en/latest/Guides/Services/service_disciplines.html>`_
++ `Customers changing classes while queueing <https://ciw.readthedocs.io/en/latest/Guides/CustomerClasses/change-class-while-queueing.html>`_
++ `Customers changing classes after service <https://ciw.readthedocs.io/en/latest/Guides/CustomerClasses/change-class-after-service.html>`_
++ `Server schedules <https://ciw.readthedocs.io/en/latest/Guides/Services/server_schedule.html>`_
++ `Slotted services <https://ciw.readthedocs.io/en/latest/Guides/Services/slotted.html>`_
++ `State tracking <https://ciw.readthedocs.io/en/latest/Guides/System/state_trackers.html>`_
++ `Stopping the simulation after a certain amount of customers <https://ciw.readthedocs.io/en/latest/Guides/Simulation/sim_numcusts.html>`_
++ `Process-based routing <https://ciw.readthedocs.io/en/latest/Guides/Routing/process_based.html>`_
++ `Logical routing <https://ciw.readthedocs.io/en/latest/Guides/Reference/routers.html>`_
++ `Deadlock detection <https://ciw.readthedocs.io/en/latest/Guides/System/deadlock.html>`_
```

### Comparing `Ciw-3.1.4/ciw/__init__.py` & `ciw-3.2.0/ciw/__init__.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/arrival_node.py` & `ciw-3.2.0/ciw/arrival_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
             The simulation to which this arrival node belongs.
         """
         self.simulation = simulation
         self.number_of_individuals = 0
         self.number_of_individuals_per_class = {clss: 0 for clss in self.simulation.network.customer_class_names}
         self.number_accepted_individuals = 0
         self.number_accepted_individuals_per_class = {clss: 0 for clss in self.simulation.network.customer_class_names}
+        self.system_capacity = self.simulation.network.system_capacity
         self.event_dates_dict = {
             nd + 1: {clss: False for clss in self.simulation.network.customer_class_names
             } for nd in range(self.simulation.network.number_of_nodes)
         }
 
     def initialise(self):
         self.initialise_event_dates_dict()
@@ -87,17 +88,17 @@
             priority_class = self.simulation.network.priority_class_mapping[self.next_class]
             next_individual = self.simulation.IndividualType(
                 self.number_of_individuals,
                 self.next_class,
                 priority_class,
                 simulation=self.simulation,
             )
-            if self.simulation.network.process_based:
-                next_individual.route = self.simulation.network.customer_classes[next_individual.customer_class].routing[self.next_node - 1](next_individual)
             next_node = self.simulation.transitive_nodes[self.next_node - 1]
+            next_individual.starting_node = next_node.id_number
+            self.simulation.routers[next_individual.customer_class].initialise_individual(next_individual)
             self.release_individual(next_node, next_individual)
 
         self.event_dates_dict[self.next_node][self.next_class] = self.increment_time(
             self.event_dates_dict[self.next_node][self.next_class],
             self.inter_arrival(self.next_node, self.next_class),
         )
         self.find_next_event_date()
@@ -149,15 +150,15 @@
         next_node.write_baulking_or_rejection_record(individual, record_type="rejection")
 
     def release_individual(self, next_node, next_individual):
         """
         Either rejects the next_individual die to lack of capacity,
         or sends that individual to baulk or not.
         """
-        if next_node.number_of_individuals >= next_node.node_capacity:
+        if (next_node.number_of_individuals >= next_node.node_capacity) or (self.simulation.number_of_individuals >= self.system_capacity):
             self.record_rejection(next_node, next_individual)
             self.simulation.nodes[-1].accept(next_individual, completed=False)
         else:
             self.decide_baulk(next_node, next_individual)
 
     def send_individual(self, next_node, next_individual):
         """
```

### Comparing `Ciw-3.1.4/ciw/auxiliary.py` & `ciw-3.2.0/ciw/auxiliary.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/deadlock/deadlock_detector.py` & `ciw-3.2.0/ciw/deadlock/deadlock_detector.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/disciplines.py` & `ciw-3.2.0/ciw/disciplines.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/dists/.hypothesis/unicodedata/8.0.0/charmap.pickle.gz` & `ciw-3.2.0/ciw/dists/.hypothesis/unicodedata/8.0.0/charmap.pickle.gz`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/dists/distributions.py` & `ciw-3.2.0/ciw/dists/distributions.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/exactnode.py` & `ciw-3.2.0/ciw/exactnode.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/exit_node.py` & `ciw-3.2.0/ciw/exit_node.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/import_params.py` & `ciw-3.2.0/ciw/import_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 import types
 import ciw.dists
 from .network import *
 from .schedules import *
+from .routing import *
 
 
 def create_network(
     arrival_distributions=None,
     baulking_functions=None,
     class_change_matrices=None,
     class_change_time_distributions=None,
@@ -17,14 +18,15 @@
     routing=None,
     batching_distributions=None,
     ps_thresholds=None,
     server_priority_functions=None,
     reneging_time_distributions=None,
     reneging_destinations=None,
     service_disciplines=None,
+    system_capacity=float('inf')
 ):
     """
     Takes in kwargs, creates dictionary.
     """
     # print(arrival_distributions)
     # print(service_distributions)
     # print(number_of_servers)
@@ -37,14 +39,15 @@
             "arrival_distributions, service_distributions and number_of_servers are required arguments."
         )
 
     params = {
         "arrival_distributions": arrival_distributions,
         "number_of_servers": number_of_servers,
         "service_distributions": service_distributions,
+        'system_capacity': system_capacity
     }
 
     if baulking_functions is not None:
         params["baulking_functions"] = baulking_functions
     if class_change_matrices is not None:
         params["class_change_matrices"] = class_change_matrices
     if class_change_time_distributions is not None:
@@ -111,43 +114,27 @@
                 preempt_priorities[nd],
                 params["ps_thresholds"][nd],
                 params["server_priority_functions"][nd],
                 params["service_disciplines"][nd],
             )
         )
     for clss_name in params['customer_class_names']:
-        if all(isinstance(f, types.FunctionType) or isinstance(f, types.MethodType) for f in params["routing"]):
-            classes[clss_name] = CustomerClass(
-                params['arrival_distributions'][clss_name],
-                params['service_distributions'][clss_name],
-                params['routing'],
-                params["priority_classes"][clss_name],
-                params["baulking_functions"][clss_name],
-                params["batching_distributions"][clss_name],
-                params["reneging_time_distributions"][clss_name],
-                params["reneging_destinations"][clss_name],
-                class_change_time_distributions[clss_name],
-            )
-        else:
-            classes[clss_name] = CustomerClass(
-                params['arrival_distributions'][clss_name],
-                params['service_distributions'][clss_name],
-                params['routing'][clss_name],
-                params["priority_classes"][clss_name],
-                params["baulking_functions"][clss_name],
-                params["batching_distributions"][clss_name],
-                params["reneging_time_distributions"][clss_name],
-                params["reneging_destinations"][clss_name],
-                class_change_time_distributions[clss_name],
-            )
+        classes[clss_name] = CustomerClass(
+            params['arrival_distributions'][clss_name],
+            params['service_distributions'][clss_name],
+            params['routing'][clss_name],
+            params["priority_classes"][clss_name],
+            params["baulking_functions"][clss_name],
+            params["batching_distributions"][clss_name],
+            params["reneging_time_distributions"][clss_name],
+            params["reneging_destinations"][clss_name],
+            class_change_time_distributions[clss_name],
+        )
     n = Network(nodes, classes)
-    if all(isinstance(f, types.FunctionType) or isinstance(f, types.MethodType) for f in params["routing"]):
-        n.process_based = True
-    else:
-        n.process_based = False
+    n.system_capacity = params['system_capacity']
     return n
 
 
 def fill_out_dictionary(params):
     """
     Fills out the parameters dictionary with the
     default values of the optional arguments.
@@ -155,17 +142,24 @@
     if isinstance(params["arrival_distributions"], list):
         arr_dists = params["arrival_distributions"]
         params["arrival_distributions"] = {"Customer": arr_dists}
     if isinstance(params["service_distributions"], list):
         srv_dists = params["service_distributions"]
         params["service_distributions"] = {"Customer": srv_dists}
     if "routing" in params:
-        if all(isinstance(f, list) for f in params["routing"]):
-            rtng_mat = params["routing"]
-            params["routing"] = {"Customer": rtng_mat}
+        if isinstance(params["routing"], list):
+            transition_matrix = params["routing"]
+            params["routing"] = {"Customer": routing.TransitionMatrix(transition_matrix=transition_matrix)}
+        elif isinstance(params["routing"], dict):
+            for clss in params["routing"]:
+                if isinstance(params["routing"][clss], list):
+                    transition_matrix = params["routing"][clss]
+                    params["routing"][clss] = routing.TransitionMatrix(transition_matrix=transition_matrix)
+        else:
+            params["routing"] = {"Customer": params["routing"]}
     if "baulking_functions" in params:
         if isinstance(params["baulking_functions"], list):
             blk_fncs = params["baulking_functions"]
             params["baulking_functions"] = {"Customer": blk_fncs}
     if "batching_distributions" in params:
         if isinstance(params["batching_distributions"], list):
             btch_dists = params["batching_distributions"]
@@ -180,15 +174,15 @@
             params["reneging_destinations"] = {"Customer": reneging_dests}
 
     class_names = sorted(params["arrival_distributions"].keys())
     params["customer_class_names"] = class_names
 
     default_dict = {
         "name": "Simulation",
-        "routing": {class_name: [[0.0]] for class_name in class_names},
+        "routing": {class_name: routing.TransitionMatrix(transition_matrix=[[0.0]]) for class_name in class_names},
         "number_of_nodes": len(params["number_of_servers"]),
         "number_of_classes": len(class_names),
         "queue_capacities": [float("inf") for _ in range(len(params["number_of_servers"]))],
         "priority_classes": {class_name: 0 for class_name in class_names},
         "baulking_functions": {class_name: [None for _ in range(len(params["number_of_servers"]))]for class_name in class_names},
         "batching_distributions": {class_name: [
                 ciw.dists.Deterministic(1) for _ in range(len(params["number_of_servers"]))
@@ -204,107 +198,67 @@
         "reneging_destinations": {
             class_name: [-1 for _ in range(len(params["number_of_servers"]))]
             for class_name in class_names
         },
         "service_disciplines": [
             ciw.disciplines.FIFO for _ in range(len(params["number_of_servers"]))
         ],
+        "system_capacity": float('inf')
     }
 
     for a in default_dict:
         params[a] = params.get(a, default_dict[a])
     return params
 
 
 def validify_dictionary(params):
     """
     Raises errors if there is something wrong with the
     parameters dictionary.
     """
-    if all(isinstance(f, types.FunctionType) or isinstance(f, types.MethodType) for f in params["routing"]):
-        consistant_num_classes = (
-            params["number_of_classes"]
-            == len(params["arrival_distributions"])
-            == len(params["service_distributions"])
-            == len(params["batching_distributions"])
-            == len(params["reneging_time_distributions"])
-            == len(params["reneging_destinations"])
-        )
-    else:
-        consistant_num_classes = (
-            params["number_of_classes"]
-            == len(params["arrival_distributions"])
-            == len(params["service_distributions"])
-            == len(params["routing"])
-            == len(params["batching_distributions"])
-            == len(params["reneging_time_distributions"])
-            == len(params["reneging_destinations"])
-        )
+    consistant_num_classes = (
+        params["number_of_classes"]
+        == len(params["arrival_distributions"])
+        == len(params["service_distributions"])
+        == len(params["routing"])
+        == len(params["batching_distributions"])
+        == len(params["reneging_time_distributions"])
+        == len(params["reneging_destinations"])
+    )
     if not consistant_num_classes:
         raise ValueError("Ensure consistant number of classes is used throughout.")
-    if all(isinstance(f, types.FunctionType) or isinstance(f, types.MethodType) for f in params["routing"]):
-        consistant_class_names = (
-            set(params["arrival_distributions"])
-            == set(params["service_distributions"])
-            == set(params["batching_distributions"])
-            == set(params["reneging_time_distributions"])
-            == set(params["reneging_destinations"])
-        )
-    else:
-        consistant_class_names = (
-            set(params["arrival_distributions"])
-            == set(params["service_distributions"])
-            == set(params["routing"])
-            == set(params["batching_distributions"])
-            == set(params["reneging_time_distributions"])
-            == set(params["reneging_destinations"])
-        ) and (
-            len(params["arrival_distributions"])
-            == len(params["service_distributions"])
-            == len(params["batching_distributions"])
-            == len(params["reneging_time_distributions"])
-            == len(params["reneging_destinations"])
-        )
+    consistant_class_names = (
+        set(params["arrival_distributions"])
+        == set(params["service_distributions"])
+        == set(params["routing"])
+        == set(params["batching_distributions"])
+        == set(params["reneging_time_distributions"])
+        == set(params["reneging_destinations"])
+    ) and (
+        len(params["arrival_distributions"])
+        == len(params["service_distributions"])
+        == len(params["batching_distributions"])
+        == len(params["reneging_time_distributions"])
+        == len(params["reneging_destinations"])
+    )
     if not consistant_class_names:
         raise ValueError("Ensure consistant names for customer classes.")
-    if all(isinstance(f, types.FunctionType) or isinstance(f, types.MethodType) for f in params["routing"]):
-        num_nodes_count = (
-            [params["number_of_nodes"]]
-            + [len(obs) for obs in params["arrival_distributions"].values()]
-            + [len(obs) for obs in params["service_distributions"].values()]
-            + [len(obs) for obs in params["batching_distributions"].values()]
-            + [len(obs) for obs in params["reneging_time_distributions"].values()]
-            + [len(obs) for obs in params["reneging_destinations"].values()]
-            + [len(params["routing"])]
-            + [len(params["number_of_servers"])]
-            + [len(params["server_priority_functions"])]
-            + [len(params["queue_capacities"])]
-        )
-    else:
-        num_nodes_count = (
-            [params["number_of_nodes"]]
-            + [len(obs) for obs in params["arrival_distributions"].values()]
-            + [len(obs) for obs in params["service_distributions"].values()]
-            + [len(obs) for obs in params["routing"].values()]
-            + [len(obs) for obs in params["batching_distributions"].values()]
-            + [len(obs) for obs in params["reneging_time_distributions"].values()]
-            + [len(obs) for obs in params["reneging_destinations"].values()]
-            + [len(row) for row in [obs for obs in params["routing"].values()][0]]
-            + [len(params["number_of_servers"])]
-            + [len(params["server_priority_functions"])]
-            + [len(params["queue_capacities"])]
-            + [len(params["service_disciplines"])]
-        )
+    num_nodes_count = (
+        [params["number_of_nodes"]]
+        + [len(obs) for obs in params["arrival_distributions"].values()]
+        + [len(obs) for obs in params["service_distributions"].values()]
+        + [len(obs) for obs in params["batching_distributions"].values()]
+        + [len(obs) for obs in params["reneging_time_distributions"].values()]
+        + [len(obs) for obs in params["reneging_destinations"].values()]
+        + [len(params["number_of_servers"])]
+        + [len(params["server_priority_functions"])]
+        + [len(params["queue_capacities"])]
+    )
     if len(set(num_nodes_count)) != 1:
         raise ValueError("Ensure consistant number of nodes is used throughout.")
-    if not all(isinstance(f, types.FunctionType) or isinstance(f, types.MethodType) for f in params["routing"]):
-        for clss in params["routing"].values():
-            for row in clss:
-                if sum(row) > 1.0 or min(row) < 0.0 or max(row) > 1.0:
-                    raise ValueError("Ensure that routing matrix is valid.")
     neg_numservers = any(
         [(isinstance(obs, int) and obs < 0) for obs in params["number_of_servers"]]
     )
     valid_capacities = all(
         [
             ((isinstance(obs, int) and obs >= 0) or obs == float("inf") or obs == "Inf")
             for obs in params["queue_capacities"]
@@ -348,7 +302,12 @@
     possible_destinations = list(range(1, params["number_of_nodes"] + 1)) + [-1]
     for dests in params["reneging_destinations"]:
         correct_destinations = all(
             d in possible_destinations for d in params["reneging_destinations"][dests]
         )
         if not correct_destinations:
             raise ValueError("Ensure all reneging destinations are possible.")
+
+    if not isinstance(params['system_capacity'], int) and params['system_capacity'] != float('inf'):
+        raise ValueError("Ensure system capacity is a positive integer.")
+    if params['system_capacity'] <= 0:
+        raise ValueError("Ensure system capacity is a positive integer.")
```

### Comparing `Ciw-3.1.4/ciw/individual.py` & `ciw-3.2.0/ciw/individual.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/network.py` & `ciw-3.2.0/ciw/network.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/node.py` & `ciw-3.2.0/ciw/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,14 @@
         else:
             self.c = node.number_of_servers
             self.schedule = None
             self.slotted = False
             self.next_event_date = float("Inf")
             self.next_shift_change = float("Inf")
         self.node_capacity = node.queueing_capacity + self.c
-        if not self.simulation.network.process_based:
-            self.transition_row = {
-                clss: self.simulation.network.customer_classes[clss].routing[id_ - 1] + [1.0 - sum(self.simulation.network.customer_classes[clss].routing[id_ - 1])]
-                for clss in self.simulation.network.customer_class_names
-            }
         self.class_change = node.class_change_matrix
         self.individuals = [[] for _ in range(simulation.number_of_priority_classes)]
         self.number_of_individuals = 0
         self.number_in_service = 0
         self.id_number = id_
         self.baulking_functions = {
             clss: self.simulation.network.customer_classes[clss].baulking_functions[id_ - 1]
@@ -530,55 +525,47 @@
         self.all_servers_total.append(srvr.total_time)
         indx = self.servers.index(srvr)
         del self.servers[indx]
 
     def next_node(self, ind):
         """
         Finds the next node according the routing method:
-          - if not process-based then sample from transition matrix
-          - if process-based then take the next value from the predefined route,
-            removing the current node from the route
-        """
-        if not self.simulation.network.process_based:
-            customer_class = ind.customer_class
-            return random_choice(
-                self.simulation.nodes[1:],
-                self.transition_row[customer_class],
-            )
-        else:
-            if ind.route == [] or ind.route[0] != self.id_number:
-                raise ValueError("Individual process route sent to wrong node")
-            ind.route.pop(0)
-            if len(ind.route) == 0:
-                next_node_number = -1
-            else:
-                next_node_number = ind.route[0]
-            return self.simulation.nodes[next_node_number]
+        """
+        return self.simulation.routers[ind.customer_class].next_node(ind, self.id_number)
+
+    def next_node_for_rerouting(self, ind):
+        """
+        Finds the next node (for rerouting) according the routing method:
+        """
+        return self.simulation.routers[ind.customer_class].next_node_for_rerouting(ind, self.id_number)
 
     def preempt(self, individual_to_preempt, next_individual):
         """
         Removes individual_to_preempt from service and replaces them with next_individual
         """
         server = individual_to_preempt.server
         individual_to_preempt.original_service_time = individual_to_preempt.service_time
-        self.write_interruption_record(individual_to_preempt)
-        individual_to_preempt.service_start_date = False
-        individual_to_preempt.time_left = individual_to_preempt.service_end_date - self.now
-        individual_to_preempt.service_time = self.priority_preempt
-        individual_to_preempt.service_end_date = False
-        self.detatch_server(server, individual_to_preempt)
-        self.decide_class_change(individual_to_preempt)
+        if self.priority_preempt == 'reroute':
+            self.reroute(individual_to_preempt)
+        else:
+            self.write_interruption_record(individual_to_preempt)
+            individual_to_preempt.service_start_date = False
+            individual_to_preempt.time_left = individual_to_preempt.service_end_date - self.now
+            individual_to_preempt.service_time = self.priority_preempt
+            individual_to_preempt.service_end_date = False
+            self.detatch_server(server, individual_to_preempt)
+            self.decide_class_change(individual_to_preempt)
         self.attach_server(server, next_individual)
         next_individual.service_start_date = self.now
         next_individual.service_time = self.get_service_time(next_individual)
         next_individual.service_end_date = self.now + next_individual.service_time
         self.reset_class_change(next_individual)
         server.next_end_service_date = next_individual.service_end_date
 
-    def release(self, next_individual, next_node):
+    def release(self, next_individual, next_node, reroute=False):
         """
         Update node when an individual is released:
           - find the individual to release
           - remove from queue
           - record relevant information to data record
           - detatch individual from server
           - write record
@@ -588,28 +575,31 @@
           - release any individuals blocked by this node
         """
         self.individuals[next_individual.prev_priority_class].remove(next_individual)
         self.number_of_individuals -= 1
         self.number_in_service -= 1
         next_individual.queue_size_at_departure = self.number_of_individuals
         next_individual.exit_date = self.now
-        self.write_individual_record(next_individual)
+        if not reroute:
+            self.write_individual_record(next_individual)
         newly_free_server = None
         if not isinf(self.c) and not self.slotted:
             newly_free_server = next_individual.server
             self.detatch_server(newly_free_server, next_individual)
         if self.slotted:
             next_individual.server = False
         self.reset_individual_attributes(next_individual)
         self.simulation.statetracker.change_state_release(
             self, next_node, next_individual, next_individual.is_blocked
         )
-        self.begin_service_if_possible_release(next_individual, newly_free_server)
+        if not reroute:
+            self.begin_service_if_possible_release(next_individual, newly_free_server)
         next_node.accept(next_individual)
-        self.release_blocked_individual()
+        if not reroute:
+            self.release_blocked_individual()
 
     def release_blocked_individual(self):
         """
         Releases an individual who becomes unblocked when
         another individual is released:
           - check if anyone is blocked by this node
           - find the individual who has been blocked the longest
@@ -702,32 +692,43 @@
             self.kill_server(obs)
 
     def interrupt_service(self, individual):
         """
         Interrupts the service of an individual and places them in an
         interrupted queue, and writes an interruption record for them.
         """
-        self.interrupted_individuals.append(individual)
-        individual.interrupted = True
-        self.number_interrupted_individuals += 1
         individual.original_service_time = individual.service_time
-        self.write_interruption_record(individual)
-        individual.original_service_start_date = individual.service_start_date
-        individual.service_start_date = False
-        individual.time_left = individual.service_end_date - self.now
-        individual.service_time = self.schedule.preemption
-        individual.service_end_date = False
-        self.number_in_service -= 1
+        if self.schedule.preemption == 'reroute':
+            self.reroute(individual)
+        else:
+            self.interrupted_individuals.append(individual)
+            individual.interrupted = True
+            self.number_interrupted_individuals += 1
+            self.write_interruption_record(individual)
+            individual.original_service_start_date = individual.service_start_date
+            individual.service_start_date = False
+            individual.time_left = individual.service_end_date - self.now
+            individual.service_time = self.schedule.preemption
+            individual.service_end_date = False
+            self.number_in_service -= 1
 
     def sort_interrupted_individuals(self):
         """
         Sorts the list of interrupted individuals by priority class and arrival date.
         """
         self.interrupted_individuals.sort(key=lambda x: (x.priority_class, x.arrival_date))
 
+    def reroute(self, individual):
+        """
+        Rerouts a preempted individual
+        """
+        next_node = self.next_node_for_rerouting(individual)
+        self.write_interruption_record(individual, destination=next_node.id_number)
+        self.release(individual, next_node, reroute=True)
+
     def update_next_end_service_without_server(self):
         """
         Updates the next end of a slotted service in the `possible_next_events` dictionary.
         """
         if self.slotted or isinf(self.c):
             next_end_service_date = float("Inf")
             for ind in self.all_individuals:
@@ -863,15 +864,15 @@
             queue_size_at_arrival=individual.queue_size_at_arrival,
             queue_size_at_departure=individual.queue_size_at_departure,
             server_id=server_id,
             record_type="service",
         )
         individual.data_records.append(record)
 
-    def write_interruption_record(self, individual):
+    def write_interruption_record(self, individual, destination=nan):
         """
         Write a data record for an individual when being interrupted.
         """
         if self.slotted:
             server_id = False
         else:
             server_id = individual.server.id_number
@@ -884,15 +885,15 @@
             arrival_date=individual.arrival_date,
             waiting_time=individual.service_start_date - individual.arrival_date,
             service_start_date=individual.service_start_date,
             service_time=individual.original_service_time,
             service_end_date=nan,
             time_blocked=nan,
             exit_date=self.now,
-            destination=nan,
+            destination=destination,
             queue_size_at_arrival=individual.queue_size_at_arrival,
             queue_size_at_departure=individual.queue_size_at_departure,
             server_id=server_id,
             record_type="interrupted service",
         )
         individual.data_records.append(record)
```

### Comparing `Ciw-3.1.4/ciw/processor_sharing.py` & `ciw-3.2.0/ciw/processor_sharing.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/schedules.py` & `ciw-3.2.0/ciw/schedules.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,17 +14,17 @@
         Pre-emption option, should be either 'resume', 'restart', 'resample',
         or False. Default is False.
 
     Attributes
     ----------
     schedule_type : str
         Type of the schedule.
-    schedule_dates : List[float]
+    shift_end_dates : List[float]
         List of shift end dates.
-    schedule_servers : List[int]
+    numbers_of_servers : List[int]
         List of corresponding server numbers.
     preemption : Union[bool, str]
         Pre-emption option.
     cyclelength : float
         Length of the schedule cycle.
 
     Methods
@@ -33,45 +33,52 @@
         Initializes the generator object at the beginning of a simulation.
     get_schedule_generator(boundaries, values)
         A generator that yields the next time and number of servers according
         to a given schedule.
     get_next_shift()
         Updates the next shifts from the generator.
     """
-    def __init__(self, schedule: List[Tuple[int, float]], preemption: Union[bool, str] = False) -> NoReturn:
+    def __init__(self, numbers_of_servers: List[int], shift_end_dates: List[float], preemption: Union[bool, str] = False, offset: float = 0.0) -> NoReturn:
         """
         Initializes the instance of the Schedule object.
 
         Parameters
         ----------
-        schedule : List[Tuple[int, float]]
-            A list of tuples representing shifts, where each tuple contains
-            the number of servers and the shift date.
+        numbers_of_servers : List[int]
+            A list containing the number of servers working at each shift
+        shift_end_dates : List[float]
+            A list containing the end dates of each shift.
         preemption : Union[bool, str], optional
             Pre-emption option, should be either 'resume', 'restart',
             'resample', or False.
             Default is False.
         """
-        if preemption not in [False, 'resume', 'restart', 'resample']:
-            raise ValueError("Pre-emption options should be either 'resume', 'restart', 'resample', or False.")
+        if preemption not in [False, 'resume', 'restart', 'resample', 'reroute']:
+            raise ValueError("Pre-emption options should be either 'resume', 'restart', 'resample', 'reroute', or False.")
+        if not isinstance(offset, float):
+            raise ValueError("Offset should be a positive float.")
+        if offset < 0.0:
+            raise ValueError("Offset should be a positive float.")
         self.schedule_type = 'schedule'
-        self.schedule_dates = [shift[1] for shift in schedule]
-        self.schedule_servers = [shift[0] for shift in schedule]
+        self.shift_end_dates = shift_end_dates
+        self.numbers_of_servers = numbers_of_servers
         self.preemption = preemption
-        self.cyclelength = self.schedule_dates[-1]
+        self.cyclelength = self.shift_end_dates[-1]
+        self.offset = offset
 
     def initialise(self) -> NoReturn:
         """
         Initializes the generator object at the beginning of a simulation.
         """
-        self.next_c = self.schedule_servers[0]
-        self.schedule_generator = self.get_schedule_generator(self.schedule_dates, self.schedule_servers)
-        self.get_next_shift()
+        self.c = 0
+        self.next_shift_change_date = self.offset
+        self.next_c = self.numbers_of_servers[0]
+        self.schedule_generator = self.get_schedule_generator(self.shift_end_dates, self.numbers_of_servers, self.offset)
 
-    def get_schedule_generator(self, boundaries: List[float], values:List[int]) -> Generator[Tuple[float, int], None, None]:
+    def get_schedule_generator(self, boundaries:List[float], values:List[int], offset:float) -> Generator[Tuple[float, int], None, None]:
         """
         A generator that yields the next time and number of servers according
         to a given schedule.
 
         Parameters
         ----------
         boundaries : List[float]
@@ -84,52 +91,57 @@
         Tuple[float, int]
             A tuple representing the next shift date and the number of servers.
         """
         num_boundaries = len(boundaries)
         index = 0
         date = 0
         while True:
-            date = boundaries[index % num_boundaries] + ((index) // num_boundaries * self.cyclelength)
+            date = offset + boundaries[index % num_boundaries] + ((index) // num_boundaries * self.cyclelength)
             index += 1
             yield date, values[index % num_boundaries]
 
     def get_next_shift(self) -> NoReturn:
         """
         Updates the next shifts from the generator.
         """
         self.c = self.next_c
         date, c = next(self.schedule_generator)
         self.next_shift_change_date = date
         self.next_c = c
 
 
 class Slotted(Schedule):
-    def __init__(self, slots, slot_sizes, capacitated=False, preemption=False):
+    def __init__(self, slots, slot_sizes, capacitated=False, preemption=False, offset=0.0):
         """
         Initialises the instance of the Slotted Schedule object
         """
         if not capacitated:
             if preemption is not False:
                 raise ValueError("Pre-emption options not availale for non-capacitated slots.")
         if preemption not in [False, 'resume', 'restart', 'resample']:
             raise ValueError("Pre-emption options should be either 'resume', 'restart', 'resample', or False.")
+        if not isinstance(offset, float):
+            raise ValueError("Offset should be a positive float.")
+        if offset < 0.0:
+            raise ValueError("Offset should be a positive float.")
         self.schedule_type = 'slotted'
+        self.offset = offset
         self.slots = slots
         self.slot_sizes = slot_sizes
+        self.next_slot_sizes = [self.slot_sizes[-1]] + self.slot_sizes[:-1]
         self.capacitated = capacitated
         self.preemption = preemption
         self.cyclelength = self.slots[-1]
         self.c = 0
 
-
     def initialise(self):
         """
         Initialises the generator object at the beginning of a simulation
         """
-        self.schedule_generator = self.get_schedule_generator(self.slots, [self.slot_sizes[-1]] + self.slot_sizes[:-1])
+        self.schedule_generator = self.get_schedule_generator(self.slots, self.next_slot_sizes, self.offset)
         self.get_next_slot()
 
     def get_next_slot(self):
         """
         Updates the next slot time and size from the generator
         """
         date, size = next(self.schedule_generator)
```

### Comparing `Ciw-3.1.4/ciw/server.py` & `ciw-3.2.0/ciw/server.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/simulation.py` & `ciw-3.2.0/ciw/simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         self.service_times = self.find_service_dists()
         self.batch_sizes = self.find_batching_dists()
         self.show_simulation_to_distributions()
         self.number_of_priority_classes = self.network.number_of_priority_classes
         self.transitive_nodes = [node_type(i + 1, self) for i, node_type in enumerate(self.NodeTypes)]
         self.nodes = [self.ArrivalNodeType(self)] + self.transitive_nodes + [ExitNode()]
         self.active_nodes = self.nodes[:-1]
+        self.routers = self.find_and_initialise_routers()
         self.nodes[0].initialise()
         if tracker is None:
             self.statetracker = trackers.StateTracker()
         else:
             self.statetracker = tracker
         self.statetracker.initialise(self)
         self.times_dictionary = {self.statetracker.hash_state(): 0.0}
@@ -62,14 +63,21 @@
 
     def __repr__(self):
         """
         Representation of the simulation.
         """
         return self.name
 
+    @property    
+    def number_of_individuals(self):
+        """
+        The number of individuals currently in the system.
+        """
+        return (self.nodes[0].number_of_individuals - 1) - self.nodes[-1].number_of_individuals
+
     def find_arrival_dists(self):
         """
         Create the dictionary of arrival time distribution
         objects for each node for each customer class.
         """
         return {
             node + 1: {
@@ -109,14 +117,24 @@
         for clss in self.network.customer_class_names:
             for nd in range(self.network.number_of_nodes):
                 if self.inter_arrival_times[nd + 1][clss] is not None:
                     self.inter_arrival_times[nd + 1][clss].simulation = self
                     self.service_times[nd + 1][clss].simulation = self
                     self.batch_sizes[nd + 1][clss].simulation = self
 
+    def find_and_initialise_routers(self):
+        """
+        Initialises the routing objects.
+        """
+        routers_dict = {}
+        for clss in self.network.customer_class_names:
+            routers_dict[clss] = self.network.customer_classes[clss].routing
+            routers_dict[clss].initialise(self)
+        return routers_dict
+
     def find_next_active_node(self):
         """
         Returns the next active node, the node whose next_event_date is next:
         """
         mindate = float("Inf")
         next_active_nodes = []
         for nd in self.active_nodes:
```

### Comparing `Ciw-3.1.4/ciw/tests/test_arrival_node.py` & `ciw-3.2.0/ciw/tests/test_arrival_node.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/tests/test_auxiliary.py` & `ciw-3.2.0/ciw/tests/test_auxiliary.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/tests/test_data_record.py` & `ciw-3.2.0/ciw/tests/test_data_record.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/tests/test_exit_node.py` & `ciw-3.2.0/ciw/tests/test_exit_node.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/tests/test_individual.py` & `ciw-3.2.0/ciw/tests/test_individual.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/tests/test_network.py` & `ciw-3.2.0/ciw/tests/test_network.py`

 * *Files 17% similar despite different names*

```diff
@@ -187,51 +187,59 @@
             [str(d) for d in N.customer_classes['Class 0'].arrival_distributions],
             ["Exponential(rate=3.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 0'].service_distributions],
             ["Exponential(rate=7.0)"],
         )
-        self.assertEqual(N.customer_classes['Class 0'].routing, [[0.5]])
+
+        router0 = N.customer_classes['Class 0'].routing
+        self.assertEqual(router0.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router0.routers[0].probs], [0.5, 0.5])
         self.assertEqual(N.number_of_priority_classes, 1)
         self.assertEqual(N.priority_class_mapping, {'Class 0': 0})
 
         params = {
             "arrival_distributions": [
                 ciw.dists.Exponential(3.0),
                 ciw.dists.Uniform(0.2, 0.6),
             ],
             "service_distributions": [
                 ciw.dists.Exponential(7.0),
                 ciw.dists.Deterministic(0.7),
             ],
-            "number_of_servers": [ciw.Schedule(schedule=[[1, 20], [4, 50]]), 3],
+            "number_of_servers": [ciw.Schedule(numbers_of_servers=[1, 4], shift_end_dates=[20, 50]), 3],
             "routing": [[0.5, 0.2], [0.0, 0.0]],
             "queue_capacities": [10, float("inf")],
         }
         N = ciw.create_network_from_dictionary(params)
         self.assertEqual(N.number_of_nodes, 2)
         self.assertEqual(N.number_of_classes, 1)
         self.assertEqual(N.service_centres[0].queueing_capacity, 10)
         self.assertTrue(type(N.service_centres[0].number_of_servers), ciw.schedules.Schedule)
         self.assertEqual(N.service_centres[0].class_change_matrix, None)
-        self.assertEqual(N.service_centres[0].number_of_servers.schedule_dates, [20, 50])
-        self.assertEqual(N.service_centres[0].number_of_servers.schedule_servers, [1, 4])
+        self.assertEqual(N.service_centres[0].number_of_servers.shift_end_dates, [20, 50])
+        self.assertEqual(N.service_centres[0].number_of_servers.numbers_of_servers, [1, 4])
         self.assertEqual(N.service_centres[1].queueing_capacity, float("inf"))
         self.assertEqual(N.service_centres[1].number_of_servers, 3)
         self.assertEqual(N.service_centres[1].class_change_matrix, None)
         self.assertEqual(
             [str(d) for d in N.customer_classes['Customer'].arrival_distributions],
             ["Exponential(rate=3.0)", "Uniform(lower=0.2, upper=0.6)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Customer'].service_distributions],
             ["Exponential(rate=7.0)", "Deterministic(value=0.7)"],
         )
-        self.assertEqual(N.customer_classes['Customer'].routing, [[0.5, 0.2], [0.0, 0.0]])
+        router = N.customer_classes['Customer'].routing
+        self.assertEqual(router.routers[0].destinations, [1, 2, -1])
+        self.assertEqual([round(p, 2) for p in router.routers[0].probs], [0.5, 0.2, 0.3])
+        self.assertEqual(router.routers[1].destinations, [1, 2, -1])
+        self.assertEqual([round(p, 2) for p in router.routers[1].probs], [0.0, 0.0, 1.0])
+
         self.assertEqual(N.number_of_priority_classes, 1)
         self.assertEqual(N.priority_class_mapping, {'Customer': 0})
 
         params = {
             "arrival_distributions": {
                 "Class 0": [ciw.dists.Exponential(3.0)],
                 "Class 1": [ciw.dists.Exponential(4.0)],
@@ -258,24 +266,28 @@
             [str(d) for d in N.customer_classes['Class 0'].arrival_distributions],
             ["Exponential(rate=3.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 0'].service_distributions],
             ["Exponential(rate=7.0)"],
         )
-        self.assertEqual(N.customer_classes['Class 0'].routing, [[0.5]])
+        router0 = N.customer_classes['Class 0'].routing
+        router1 = N.customer_classes['Class 1'].routing
+        self.assertEqual(router0.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router0.routers[0].probs], [0.5, 0.5])
+        self.assertEqual(router1.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router1.routers[0].probs], [0.0, 1.0])
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 1'].arrival_distributions],
             ["Exponential(rate=4.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 1'].service_distributions],
             ["Uniform(lower=0.4, upper=1.2)"],
         )
-        self.assertEqual(N.customer_classes['Class 1'].routing, [[0.0]])
         self.assertEqual(N.number_of_priority_classes, 1)
         self.assertEqual(N.priority_class_mapping, {'Class 0': 0, 'Class 1': 0})
 
         params = {
             "arrival_distributions": {
                 "Class 0": [ciw.dists.Exponential(3.0)],
                 "Class 1": [ciw.dists.Exponential(4.0)],
@@ -309,24 +321,28 @@
             [str(d) for d in N.customer_classes['Class 0'].arrival_distributions],
             ["Exponential(rate=3.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 0'].service_distributions],
             ["Exponential(rate=7.0)"],
         )
-        self.assertEqual(N.customer_classes['Class 0'].routing, [[0.5]])
+        router0 = N.customer_classes['Class 0'].routing
+        router1 = N.customer_classes['Class 1'].routing
+        self.assertEqual(router0.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router0.routers[0].probs], [0.5, 0.5])
+        self.assertEqual(router1.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router1.routers[0].probs], [0.0, 1.0])
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 1'].arrival_distributions],
             ["Exponential(rate=4.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 1'].service_distributions],
             ["Uniform(lower=0.4, upper=1.2)"],
         )
-        self.assertEqual(N.customer_classes['Class 1'].routing, [[0.0]])
         self.assertEqual(N.number_of_priority_classes, 1)
         self.assertEqual(N.priority_class_mapping, {'Class 0': 0, 'Class 1': 0})
 
         params = {
             "arrival_distributions": {
                 "Class 0": [ciw.dists.Exponential(3.0)],
                 "Class 1": [ciw.dists.Exponential(4.0)],
@@ -350,24 +366,28 @@
             [str(d) for d in N.customer_classes['Class 0'].arrival_distributions],
             ["Exponential(rate=3.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 0'].service_distributions],
             ["Exponential(rate=7.0)"],
         )
-        self.assertEqual(N.customer_classes['Class 0'].routing, [[0.5]])
+        router0 = N.customer_classes['Class 0'].routing
+        router1 = N.customer_classes['Class 1'].routing
+        self.assertEqual(router0.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router0.routers[0].probs], [0.5, 0.5])
+        self.assertEqual(router1.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router1.routers[0].probs], [0.0, 1.0])
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 1'].arrival_distributions],
             ["Exponential(rate=4.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 1'].service_distributions],
             ["Uniform(lower=0.4, upper=1.2)"],
         )
-        self.assertEqual(N.customer_classes['Class 1'].routing, [[0.0]])
         self.assertEqual(N.customer_classes['Class 0'].priority_class, 1)
         self.assertEqual(N.customer_classes['Class 1'].priority_class, 0)
         self.assertEqual(N.number_of_priority_classes, 2)
         self.assertEqual(N.priority_class_mapping, {'Class 0': 1, 'Class 1': 0})
 
         params = {
             "arrival_distributions": [
@@ -399,18 +419,21 @@
             [str(d) for d in N.customer_classes['Customer'].arrival_distributions],
             ["Exponential(rate=3.0)", "Exponential(rate=4.0)", "Exponential(rate=2.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Customer'].service_distributions],
             ["Exponential(rate=7.0)", "Uniform(lower=0.4, upper=1.2)", "Deterministic(value=5.33)"],
         )
-        self.assertEqual(
-            N.customer_classes['Customer'].routing,
-            [[0.5, 0.0, 0.1], [0.2, 0.1, 0.0], [0.0, 0.0, 0.0]],
-        )
+        router = N.customer_classes['Customer'].routing
+        self.assertEqual(router.routers[0].destinations, [1, 2, 3, -1])
+        self.assertEqual([round(p, 2) for p in router.routers[0].probs], [0.5, 0.0, 0.1, 0.4])
+        self.assertEqual(router.routers[1].destinations, [1, 2, 3, -1])
+        self.assertEqual([round(p, 2) for p in router.routers[1].probs], [0.2, 0.1, 0.0, 0.7])
+        self.assertEqual(router.routers[2].destinations, [1, 2, 3, -1])
+        self.assertEqual([round(p, 2) for p in router.routers[2].probs], [0.0, 0.0, 0.0, 1.0])
         self.assertEqual(
             N.customer_classes['Customer'].baulking_functions,
             [None, None, example_baulking_function],
         )
         self.assertEqual(N.number_of_priority_classes, 1)
 
 
@@ -420,15 +443,15 @@
             "service_distributions": {"Class 0": [ciw.dists.Exponential(7.0)]},
             "number_of_servers": [9],
             "number_of_classes": 1,
             "routing": {"Class 0": [[0.5]]},
             "number_of_nodes": 1,
             "queue_capacities": [float("inf")],
         }
-        params_list = [copy.deepcopy(params) for i in range(27)]
+        params_list = [copy.deepcopy(params) for i in range(28)]
 
         params_list[0]["number_of_classes"] = -2
         self.assertRaises(
             ValueError,
             ciw.create_network_from_dictionary,
             params_list[0]
         )
@@ -527,24 +550,26 @@
         params_list[14]["routing"] = {"Patient 0": [[0.5]]}
         self.assertRaises(
             ValueError,
             ciw.create_network_from_dictionary,
             params_list[14]
         )
         params_list[15]["routing"]["Class 0"] = [[0.2], [0.1]]
+        N = ciw.create_network_from_dictionary(params_list[15])
         self.assertRaises(
             ValueError,
-            ciw.create_network_from_dictionary,
-            params_list[15]
+            ciw.Simulation,
+            N
         )
         params_list[16]["routing"]["Class 0"] = [[0.2, 0.1]]
+        N = ciw.create_network_from_dictionary(params_list[16])
         self.assertRaises(
             ValueError,
-            ciw.create_network_from_dictionary,
-            params_list[16]
+            ciw.Simulation,
+            N
         )
         params_list[17]["routing"]["Class 0"] = [[-0.6]]
         self.assertRaises(
             ValueError,
             ciw.create_network_from_dictionary,
             params_list[17]
         )
@@ -598,54 +623,108 @@
         )
         params_list[26]["class_change_time_distributions"] = {'Class 0': {'Class 0': None}, 'Class 1': {'Class 0': None, 'Class 1': None}}
         self.assertRaises(
             ValueError,
             ciw.create_network_from_dictionary,
             params_list[26]
         )
+        params_list[27]["routing"]["Class 0"] = [['0.5']]
+        self.assertRaises(
+            ValueError,
+            ciw.create_network_from_dictionary,
+            params_list[27]
+        )
+
+    def test_raising_errors_routing(self):
+        params = {
+            'arrival_distributions': [ciw.dists.Exponential(1.0), ciw.dists.Exponential(1.0)],
+            'service_distributions': [ciw.dists.Exponential(2.0), ciw.dists.Exponential(2.0)],
+            'number_of_servers': [2, 1],
+            'routing': [[0.5, 0.6], [0.0, 0.3]]
+        }
+        self.assertRaises(
+            ValueError,
+            ciw.create_network_from_dictionary,
+            params
+        )
+
+        N = ciw.create_network(
+            arrival_distributions=[ciw.dists.Exponential(1.0), ciw.dists.Exponential(1.0)],
+            service_distributions=[ciw.dists.Exponential(2.0), ciw.dists.Exponential(2.0)],
+            number_of_servers=[2, 1],
+            routing=[[0.5, 0.2, 0.0], [0.0, 0.3, 0.0], [0.1, 0.1, 0.3]]
+        )
+        self.assertRaises(
+            ValueError,
+            ciw.Simulation,
+            N
+        )
+
+        N = ciw.create_network(
+            arrival_distributions=[ciw.dists.Exponential(1.0), ciw.dists.Exponential(1.0)],
+            service_distributions=[ciw.dists.Exponential(2.0), ciw.dists.Exponential(2.0)],
+            number_of_servers=[2, 1],
+            routing=ciw.routing.NetworkRouting(routers=[
+                ciw.routing.Probabilistic(destinations=[0, 1], probs=[0.5, 0.2]),
+                ciw.routing.Probabilistic(destinations=[0, 2], probs=[0.5, 0.2])
+            ])
+        )
+        self.assertRaises(
+            ValueError,
+            ciw.Simulation,
+            N
+        )
 
 
 class TestImportNoMatrix(unittest.TestCase):
     def test_optional_transition_matrix(self):
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Exponential(1.0)],
             service_distributions=[ciw.dists.Exponential(2.0)],
             number_of_servers=[1],
         )
-        self.assertEqual([c.routing for c in N.customer_classes.values()], [[[0.0]]])
+        router = N.customer_classes['Customer'].routing
+        self.assertEqual(router.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router.routers[0].probs], [0.0, 1.0])
 
         N = ciw.create_network(
             arrival_distributions={
                 "Class 0": [ciw.dists.Exponential(1.0)],
                 "Class 1": [ciw.dists.Exponential(1.0)],
             },
             service_distributions={
                 "Class 0": [ciw.dists.Exponential(2.0)],
                 "Class 1": [ciw.dists.Exponential(1.0)],
             },
             number_of_servers=[1],
         )
 
-        self.assertEqual([c.routing for c in N.customer_classes.values()], [[[0.0]], [[0.0]]])
+        router0 = N.customer_classes['Class 0'].routing
+        router1 = N.customer_classes['Class 1'].routing
+        self.assertEqual(router0.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router0.routers[0].probs], [0.0, 1.0])
+        self.assertEqual(router1.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router1.routers[0].probs], [0.0, 1.0])
 
         params = {
             "arrival_distributions": [
                 ciw.dists.Exponential(1.0),
                 ciw.dists.Exponential(1.0),
             ],
             "service_distributions": [
                 ciw.dists.Exponential(2.0),
                 ciw.dists.Exponential(2.0),
             ],
             "number_of_servers": [1, 2],
         }
+        N = ciw.create_network(**params)
         self.assertRaises(
             ValueError,
-            ciw.create_network_from_dictionary,
-            params
+            ciw.Simulation,
+            N
         )
 
 
 class TestCreateNetworkKwargs(unittest.TestCase):
     def test_network_from_kwargs(self):
         N = ciw.create_network(
             arrival_distributions={"Class 0": [ciw.dists.Exponential(3.0)]},
@@ -664,52 +743,59 @@
             [str(d) for d in N.customer_classes['Class 0'].arrival_distributions],
             ["Exponential(rate=3.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 0'].service_distributions],
             ["Exponential(rate=7.0)"],
         )
-        self.assertEqual(N.customer_classes['Class 0'].routing, [[0.5]])
+        router0 = N.customer_classes['Class 0'].routing
+        self.assertEqual(router0.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router0.routers[0].probs], [0.5, 0.5])
         self.assertEqual(N.number_of_priority_classes, 1)
         self.assertEqual(N.priority_class_mapping, {'Class 0': 0})
 
         N = ciw.create_network(
             arrival_distributions=[
                 ciw.dists.Exponential(3.0),
                 ciw.dists.Uniform(0.2, 0.6),
             ],
             service_distributions=[
                 ciw.dists.Exponential(7.0),
                 ciw.dists.Deterministic(0.7),
             ],
-            number_of_servers=[ciw.Schedule(schedule=[[1, 20], [4, 50]]), 3],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 4], shift_end_dates=[20, 50]), 3],
             routing=[[0.5, 0.2], [0.0, 0.0]],
             queue_capacities=[10, float("inf")],
         )
 
         self.assertEqual(N.number_of_nodes, 2)
         self.assertEqual(N.number_of_classes, 1)
         self.assertEqual(N.service_centres[0].queueing_capacity, 10)
         self.assertEqual(type(N.service_centres[0].number_of_servers), ciw.schedules.Schedule)
         self.assertEqual(N.service_centres[0].class_change_matrix, None)
-        self.assertEqual(N.service_centres[0].number_of_servers.schedule_dates, [20, 50])
-        self.assertEqual(N.service_centres[0].number_of_servers.schedule_servers, [1, 4])
+        self.assertEqual(N.service_centres[0].number_of_servers.shift_end_dates, [20, 50])
+        self.assertEqual(N.service_centres[0].number_of_servers.numbers_of_servers, [1, 4])
         self.assertFalse(N.service_centres[0].number_of_servers.preemption)
         self.assertEqual(N.service_centres[1].queueing_capacity, float("inf"))
         self.assertEqual(N.service_centres[1].number_of_servers, 3)
         self.assertEqual(N.service_centres[1].class_change_matrix, None)
         self.assertEqual(
             [str(d) for d in N.customer_classes['Customer'].arrival_distributions],
             ["Exponential(rate=3.0)", "Uniform(lower=0.2, upper=0.6)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Customer'].service_distributions],
             ["Exponential(rate=7.0)", "Deterministic(value=0.7)"],
         )
-        self.assertEqual(N.customer_classes['Customer'].routing, [[0.5, 0.2], [0.0, 0.0]])
+        router = N.customer_classes['Customer'].routing
+        self.assertEqual(router.routers[0].destinations, [1, 2, -1])
+        self.assertEqual([round(p, 2) for p in router.routers[0].probs], [0.5, 0.2, 0.3])
+        self.assertEqual(router.routers[1].destinations, [1, 2, -1])
+        self.assertEqual([round(p, 2) for p in router.routers[1].probs], [0.0, 0.0, 1.0])
+
         self.assertEqual(N.number_of_priority_classes, 1)
         self.assertEqual(N.priority_class_mapping, {'Customer': 0})
 
         N = ciw.create_network(
             arrival_distributions={
                 "Class 0": [ciw.dists.Exponential(3.0)],
                 "Class 1": [ciw.dists.Exponential(4.0)],
@@ -735,24 +821,28 @@
             [str(d) for d in N.customer_classes['Class 0'].arrival_distributions],
             ["Exponential(rate=3.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 0'].service_distributions],
             ["Exponential(rate=7.0)"],
         )
-        self.assertEqual(N.customer_classes['Class 0'].routing, [[0.5]])
+        router0 = N.customer_classes['Class 0'].routing
+        router1 = N.customer_classes['Class 1'].routing
+        self.assertEqual(router0.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router0.routers[0].probs], [0.5, 0.5])
+        self.assertEqual(router1.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router1.routers[0].probs], [0.0, 1.0])
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 1'].arrival_distributions],
             ["Exponential(rate=4.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 1'].service_distributions],
             ["Uniform(lower=0.4, upper=1.2)"],
         )
-        self.assertEqual(N.customer_classes['Class 1'].routing, [[0.0]])
         self.assertEqual(N.number_of_priority_classes, 1)
         self.assertEqual(N.priority_class_mapping, {'Class 0': 0, 'Class 1': 0})
 
         N = ciw.create_network(
             arrival_distributions={
                 "Class 0": [ciw.dists.Exponential(3.0)],
                 "Class 1": [ciw.dists.Exponential(4.0)],
@@ -775,24 +865,28 @@
             [str(d) for d in N.customer_classes['Class 0'].arrival_distributions],
             ["Exponential(rate=3.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 0'].service_distributions],
             ["Exponential(rate=7.0)"],
         )
-        self.assertEqual(N.customer_classes['Class 0'].routing, [[0.5]])
+        router0 = N.customer_classes['Class 0'].routing
+        router1 = N.customer_classes['Class 1'].routing
+        self.assertEqual(router0.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router0.routers[0].probs], [0.5, 0.5])
+        self.assertEqual(router1.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router1.routers[0].probs], [0.0, 1.0])
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 1'].arrival_distributions],
             ["Exponential(rate=4.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 1'].service_distributions],
             ["Uniform(lower=0.4, upper=1.2)"],
         )
-        self.assertEqual(N.customer_classes['Class 1'].routing, [[0.0]])
         self.assertEqual(N.customer_classes['Class 0'].priority_class, 1)
         self.assertEqual(N.customer_classes['Class 1'].priority_class, 0)
         self.assertEqual(N.number_of_priority_classes, 2)
         self.assertEqual(N.priority_class_mapping, {'Class 0': 1, 'Class 1': 0})
 
         N = ciw.create_network(
             arrival_distributions=[
@@ -824,18 +918,22 @@
             [str(d) for d in N.customer_classes['Customer'].arrival_distributions],
             ["Exponential(rate=3.0)", "Exponential(rate=4.0)", "Exponential(rate=2.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Customer'].service_distributions],
             ["Exponential(rate=7.0)", "Uniform(lower=0.4, upper=1.2)", "Deterministic(value=5.33)"],
         )
-        self.assertEqual(
-            N.customer_classes['Customer'].routing,
-            [[0.5, 0.0, 0.1], [0.2, 0.1, 0.0], [0.0, 0.0, 0.0]],
-        )
+        router = N.customer_classes['Customer'].routing
+        self.assertEqual(router.routers[0].destinations, [1, 2, 3, -1])
+        self.assertEqual([round(p, 2) for p in router.routers[0].probs], [0.5, 0.0, 0.1, 0.4])
+        self.assertEqual(router.routers[1].destinations, [1, 2, 3, -1])
+        self.assertEqual([round(p, 2) for p in router.routers[1].probs], [0.2, 0.1, 0.0, 0.7])
+        self.assertEqual(router.routers[2].destinations, [1, 2, 3, -1])
+        self.assertEqual([round(p, 2) for p in router.routers[2].probs], [0.0, 0.0, 0.0, 1.0])
+
         self.assertEqual(
             N.customer_classes['Customer'].baulking_functions,
             [None, None, example_baulking_function],
         )
         self.assertEqual(N.number_of_priority_classes, 1)
 
         N = ciw.create_network(
@@ -894,24 +992,29 @@
             [str(d) for d in N.customer_classes['Class 0'].arrival_distributions],
             ["Exponential(rate=3.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 0'].service_distributions],
             ["Exponential(rate=7.0)"],
         )
-        self.assertEqual(N.customer_classes['Class 0'].routing, [[0.5]])
+        router0 = N.customer_classes['Class 0'].routing
+        router1 = N.customer_classes['Class 1'].routing
+        self.assertEqual(router0.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router0.routers[0].probs], [0.5, 0.5])
+        self.assertEqual(router1.routers[0].destinations, [1, -1])
+        self.assertEqual([round(p, 2) for p in router1.routers[0].probs], [0.0, 1.0])
+
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 1'].arrival_distributions],
             ["Exponential(rate=4.0)"],
         )
         self.assertEqual(
             [str(d) for d in N.customer_classes['Class 1'].service_distributions],
             ["Uniform(lower=0.4, upper=1.2)"],
         )
-        self.assertEqual(N.customer_classes['Class 1'].routing, [[0.0]])
         self.assertEqual(N.number_of_priority_classes, 1)
         self.assertEqual(N.priority_class_mapping, {'Class 0': 0, 'Class 1': 0})
 
     def test_create_network_preempt_priorities(self):
         N = ciw.create_network(
             arrival_distributions={
                 "Class 0": [ciw.dists.Exponential(3.0), ciw.dists.Exponential(2.0)],
@@ -1020,7 +1123,27 @@
                  'Class 1': {'Class 0': 1.0, 'Class 1': 0.0}}
             ]
         }
         with self.assertRaises(ValueError):
             ciw.create_network(**params_geq1)
         with self.assertRaises(ValueError):
             ciw.create_network(**params_neg)
+
+    def test_raising_errors_system_capacity(self):
+        params_neg = {
+            'arrival_distributions': [ciw.dists.Exponential(10), ciw.dists.Exponential(10)],
+            'service_distributions': [ciw.dists.Exponential(30), ciw.dists.Exponential(20)],
+            'number_of_servers': [2, 2],
+            'routing': [[0.0, 0.0], [0.0, 0.0]],
+            'system_capacity': -4
+        }
+        params_str = {
+            'arrival_distributions': [ciw.dists.Exponential(10), ciw.dists.Exponential(10)],
+            'service_distributions': [ciw.dists.Exponential(30), ciw.dists.Exponential(20)],
+            'number_of_servers': [2, 2],
+            'routing': [[0.0, 0.0], [0.0, 0.0]],
+            'system_capacity': '77'
+        }
+        with self.assertRaises(ValueError):
+            ciw.create_network(**params_neg)
+        with self.assertRaises(ValueError):
+            ciw.create_network(**params_str)
```

### Comparing `Ciw-3.1.4/ciw/tests/test_node.py` & `ciw-3.2.0/ciw/tests/test_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,18 +94,14 @@
 
 
 class TestNode(unittest.TestCase):
     def test_init_method(self):
         Q = ciw.Simulation(N_params)
         N = ciw.Node(1, Q)
         self.assertEqual(N.c, 9)
-        self.assertEqual(
-            [[round(p, 10) for p in row] for row in N.transition_row.values()],
-            [[0.1, 0.2, 0.1, 0.4, 0.2], [0.6, 0.0, 0.0, 0.2, 0.2], [0.0, 0.0, 0.4, 0.3, 0.3]],
-        )
         self.assertEqual(N.next_event_date, float("inf"))
         self.assertEqual(N.all_individuals, [])
         self.assertEqual(N.id_number, 1)
         self.assertEqual(N.interrupted_individuals, [])
         self.assertFalse(N.reneging)
 
         Net = ciw.create_network(
@@ -139,37 +135,41 @@
         self.assertEqual(N.interrupted_individuals, [])
 
         N_schedule = ciw.create_network(
             arrival_distributions={
                 "Class 0": [ciw.dists.Exponential(0.05), ciw.dists.Exponential(0.04)],
                 "Class 1": [ciw.dists.Exponential(0.04), ciw.dists.Exponential(0.06)],
             },
-            number_of_servers=[ciw.Schedule(schedule=[[1, 30], [2, 60], [1, 90], [3, 100]]), 3],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 2, 1, 3], shift_end_dates=[30, 60, 90, 100]), 3],
             queue_capacities=[float("Inf"), 10],
             service_distributions={
                 "Class 0": [ciw.dists.Deterministic(5.0), ciw.dists.Exponential(0.2)],
                 "Class 1": [ciw.dists.Deterministic(10.0), ciw.dists.Exponential(0.1)],
             },
             routing={
                 "Class 0": [[0.8, 0.1], [0.0, 0.0]],
                 "Class 1": [[0.8, 0.1], [0.2, 0.0]],
             },
         )
         Q = ciw.Simulation(N_schedule)
         N = Q.transitive_nodes[0]
+        N.have_event()
+        N.update_next_event_date()
         self.assertEqual(N.schedule.cyclelength, 100)
         self.assertEqual(N.c, 1)
-        self.assertEqual(N.schedule.schedule_dates, [30, 60, 90, 100])
-        self.assertEqual(N.schedule.schedule_servers, [1, 2, 1, 3])
+        self.assertEqual(N.schedule.shift_end_dates, [30, 60, 90, 100])
+        self.assertEqual(N.schedule.numbers_of_servers, [1, 2, 1, 3])
         self.assertEqual(N.next_event_date, 30)
         self.assertEqual(N.interrupted_individuals, [])
         self.assertFalse(N.reneging)
 
         Q = ciw.Simulation(N_priorities)
         N = Q.transitive_nodes[0]
+        N.have_event()
+        N.update_next_event_date()
         self.assertEqual(N.c, 4)
         self.assertEqual(Q.network.priority_class_mapping, {'Class 0': 0, 'Class 1': 1})
         self.assertEqual(Q.number_of_priority_classes, 2)
         self.assertEqual(N.interrupted_individuals, [])
         self.assertFalse(N.reneging)
 
     def test_repr_method(self):
@@ -749,26 +749,28 @@
         N.reset_individual_attributes(ind)
         self.assertFalse(ind.arrival_date)
         self.assertFalse(ind.service_start_date)
         self.assertFalse(ind.service_end_date)
         self.assertFalse(ind.exit_date)
 
     def test_date_from_schedule_generator(self):
-        sg = ciw.Schedule(schedule=[[1, 30], [0, 60], [2, 90], [3, 100]])
+        sg = ciw.Schedule(numbers_of_servers=[1, 0, 2, 3], shift_end_dates=[30, 60, 90, 100])
         sg.initialise()
+        sg.get_next_shift()
         self.assertEqual(sg.c, 1)
         self.assertEqual(sg.next_c, 0)
         self.assertEqual(sg.next_shift_change_date, 30)
         self.assertEqual(next(sg.schedule_generator), (60, 2))
         self.assertEqual(next(sg.schedule_generator), (90, 3))
         self.assertEqual(next(sg.schedule_generator), (100, 1))
         self.assertEqual(next(sg.schedule_generator), (130, 0))
         self.assertEqual(next(sg.schedule_generator), (160, 2))
 
         sg.initialise()
+        sg.get_next_shift()
         self.assertEqual(sg.c, 1)
         self.assertEqual(sg.next_c, 0)
         self.assertEqual(sg.next_shift_change_date, 30)
         self.assertEqual(next(sg.schedule_generator), (60, 2))
         self.assertEqual(next(sg.schedule_generator), (90, 3))
         self.assertEqual(next(sg.schedule_generator), (100, 1))
         self.assertEqual(next(sg.schedule_generator), (130, 0))
@@ -881,15 +883,15 @@
         Q.simulate_until_max_time(20.0)
         self.assertEqual(Q.transitive_nodes[0].server_utilisation, 4.0 / 15.0)
 
     def test_server_utilisation_with_schedules(self):
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Sequential([2.0, 4.0, 4.0, 0.0, 7.0, 1000.0])],
             service_distributions=[ciw.dists.Sequential([4.0, 2.0, 6.0, 6.0, 3.0])],
-            number_of_servers=[ciw.Schedule(schedule=[[1, 9], [2, 23]])],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 2], shift_end_dates=[9, 23])],
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(23)
         recs = Q.get_all_records()
         self.assertEqual(Q.transitive_nodes[0].server_utilisation, 21.0 / 37.0)
 
     def test_server_utilisation_with_wrapup(self):
@@ -1008,15 +1010,15 @@
             return -srv.id_number
 
         ciw.seed(0)
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Exponential(1), ciw.dists.Exponential(1)],
             service_distributions=[ciw.dists.Exponential(2), ciw.dists.Exponential(2)],
             number_of_servers=[2, 2],
-            routing=[[0, 0], [0, 0]],
+            routing=[[0.0, 0.0], [0.0, 0.0]],
             server_priority_functions=[prioritise_less_busy, prioritise_highest_id],
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(1000)
         expected_times_node_1 = [256.2457715650031, 257.59339967047254]
         expected_times_node_2 = [157.35577182806387, 356.41473247082365]
 
@@ -1152,15 +1154,15 @@
         self.assertEqual([r.queue_size_at_arrival for r in reneging_recs], [1, 1])
         self.assertEqual([r.queue_size_at_departure for r in reneging_recs], [1, 1])
 
     def test_reneging_sends_to_destination(self):
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Deterministic(7), None],
             service_distributions=[ciw.dists.Deterministic(11), ciw.dists.Deterministic(2)],
-            routing=[[0, 0], [0, 0]],
+            routing=[[0.0, 0.0], [0.0, 0.0]],
             number_of_servers=[1, 1],
             reneging_time_distributions=[ciw.dists.Deterministic(3), None],
             reneging_destinations=[2, -1],
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(20)
         recs = Q.get_all_records()
@@ -1218,15 +1220,15 @@
         self.assertEqual(Q.nodes[1].next_event_date, 29)
         self.assertEqual(Q.nodes[1].next_event_type, 'end_service')
 
     def test_reneging_with_schedules(self):
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Deterministic(7)],
             service_distributions=[ciw.dists.Deterministic(11)],
-            number_of_servers=[ciw.Schedule(schedule=[[1, 16], [0, 10000]])],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0], shift_end_dates=[16, 10000])],
             reneging_time_distributions=[ciw.dists.Deterministic(3)],
         )
         Q = ciw.Simulation(N)
         self.assertTrue(Q.nodes[1].reneging)
         #### We would expect:
         # t=7  arrival cust 1
         # t=14 arrival cust 2
@@ -1852,15 +1854,15 @@
         There is one server, who goes off duty at time 24 and comes back at time 29.
         There will be one interrupted individual:
           - ind 3; arrives 21; interrupted 24; resumed 29; finishes 30.
         """
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Deterministic(7)],
             service_distributions=[ciw.dists.Deterministic(4)],
-            number_of_servers=[ciw.Schedule(schedule=[[1, 24], [0, 29], [1, 37]], preemption="resume")],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0, 1], shift_end_dates=[24, 29, 37], preemption="resume")],
         )
         ciw.seed(0)
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(36)
         recs = Q.get_all_records()
 
         recs_ind3 = [r for r in recs if r.id_number == 3]
@@ -1902,15 +1904,15 @@
                 "Class 0": [ciw.dists.Sequential([3, float("inf")])],
                 "Class 1": [ciw.dists.Sequential([1, float("inf")])],
             },
             service_distributions={
                 "Class 0": [ciw.dists.Deterministic(10)],
                 "Class 1": [ciw.dists.Sequential([6, 3])],
             },
-            number_of_servers=[ciw.Schedule(schedule=[[1, 5], [2, 100]])],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 2], shift_end_dates=[5, 100])],
             priority_classes=({"Class 0": 0, "Class 1": 1}, ["restart"]),
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(20)
         recs = Q.get_all_records(only=["service"])
         r2, r1 = recs
         self.assertEqual(r1.arrival_date, 3)
@@ -1931,15 +1933,15 @@
                 "Class 0": [ciw.dists.Sequential([3, float("inf")])],
                 "Class 1": [ciw.dists.Sequential([1, float("inf")])],
             },
             service_distributions={
                 "Class 0": [ciw.dists.Deterministic(10)],
                 "Class 1": [ciw.dists.Sequential([6, 3])],
             },
-            number_of_servers=[ciw.Schedule(schedule=[[1, 5], [2, 100]])],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 2], shift_end_dates=[5, 100])],
             priority_classes=({"Class 0": 0, "Class 1": 1}, ["resume"]),
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(20)
         recs = Q.get_all_records(only="service")
         r2, r1 = recs
         self.assertEqual(r1.arrival_date, 3)
@@ -1960,15 +1962,15 @@
                 "Class 0": [ciw.dists.Sequential([3, float("inf")])],
                 "Class 1": [ciw.dists.Sequential([1, float("inf")])],
             },
             service_distributions={
                 "Class 0": [ciw.dists.Deterministic(10)],
                 "Class 1": [ciw.dists.Sequential([6, 3])],
             },
-            number_of_servers=[ciw.Schedule(schedule=[[1, 5], [2, 100]])],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 2], shift_end_dates=[5, 100])],
             priority_classes=({"Class 0": 0, "Class 1": 1}, ["resample"]),
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(20)
         recs = Q.get_all_records(only=["service"])
         r2, r1 = recs
         self.assertEqual(r1.arrival_date, 3)
@@ -2010,13 +2012,13 @@
         ]
         self.assertEqual(set(Q.nodes[2].blocked_queue), set(expected_blocked_queue))
 
     def test_shift_change_before_arrival(self):
          N = ciw.create_network(
             arrival_distributions=[ciw.dists.Sequential(sequence=[2.0, float('inf')])],
             service_distributions=[ciw.dists.Deterministic(value=1.0)],
-            number_of_servers=[ciw.Schedule(schedule=[[1, 1.0], [2, 10.0]], preemption=False)]
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 2], shift_end_dates=[1.0, 10.0], preemption=False)]
          )
          Q = ciw.Simulation(N)
          Q.simulate_until_max_time(10.5)
          recs = Q.get_all_records()
          self.assertEqual(len(recs), 1)
```

### Comparing `Ciw-3.1.4/ciw/tests/test_process_based.py` & `ciw-3.2.0/ciw/tests/test_process_based.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,116 +1,94 @@
 import unittest
 import ciw
 import random
 from collections import Counter
 
+def generator_function_1(ind, simulation):
+    return [1, 1]
 
-def generator_function_1(ind):
-    return [1, 1, 1]
 
+def generator_function_2(ind, simulation):
+    return [1, 2, 1, 3]
 
-def generator_function_2(ind):
-    return [1, 1, 2, 1, 3]
 
-
-def generator_function_3(ind):
+def generator_function_3(ind, simulation):
     rnd = random.random()
     if rnd < 0.4:
-        return [1, 2, 2, 3, 2]
+        return [2, 2, 3, 2]
     if rnd < 0.5:
-        return [1, 1]
-    return [1, 3, 2, 3]
-
-
-def generator_function_4(ind):
-    return [2, 1, 3, 1, 1]
-
-
-def generator_function_5(ind):
-    return [3, 2, 3, 2, 3]
-
-
-def generator_function_6(ind):
-    return [3]
-
-
-def generator_function_7(ind):
-    rnd = random.random()
-    if rnd < 0.4:
-        return [2, 1, 2]
-    return [2, 1, 1, 2]
-
-
-def generator_function_8(ind):
-    if ind.customer_class == 'Class 0':
         return [1]
-    return [1, 1, 1]
+    return [3, 2, 3]
+
+def generator_function_4(ind, simulation):
+    return []
 
 class ClassForProcessBasedMethod:
     def __init__(self, n):
         self.n = n
-    def generator_method(self, ind):
-        return [1, 1, 1]
+    def generator_method(self, ind, simulation):
+        return [1, 1]
 
+def flexible_generator_1(ind, simulation):
+    return [[2], [3, 4, 5], [6]]
 
 class TestProcessBased(unittest.TestCase):
     def test_network_takes_routing_function(self):
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Exponential(1)],
             service_distributions=[ciw.dists.Exponential(2)],
             number_of_servers=[1],
-            routing=[generator_function_1],
+            routing=ciw.routing.ProcessBased(generator_function_1),
         )
-        self.assertEqual(N.process_based, True)
         Q = ciw.Simulation(N)
         self.assertEqual(str(Q), "Simulation")
 
     def test_individuals_recieve_route(self):
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Deterministic(1)],
             service_distributions=[ciw.dists.Deterministic(1000)],
             number_of_servers=[1],
-            routing=[generator_function_1],
+            routing=ciw.routing.ProcessBased(generator_function_1),
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(4.5)
         inds = Q.nodes[1].all_individuals
         for ind in inds:
-            self.assertEqual(ind.route, [1, 1, 1])
+            self.assertEqual(ind.route, [1, 1])
 
     def test_routing_correct(self):
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Sequential([1, 10000]), None, None],
             service_distributions=[
                 ciw.dists.Deterministic(2),
                 ciw.dists.Deterministic(2),
                 ciw.dists.Deterministic(2),
             ],
             number_of_servers=[1, 1, 1],
-            routing=[generator_function_2, ciw.no_routing, ciw.no_routing],
+            routing=ciw.routing.ProcessBased(generator_function_2),
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(4)
         ind = Q.get_all_individuals()[0]
-        self.assertEqual(ind.route, [1, 2, 1, 3])
+        self.assertEqual(ind.route, [2, 1, 3])
         self.assertEqual([dr.node for dr in ind.data_records], [1])
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(6)
         ind = Q.get_all_individuals()[0]
-        self.assertEqual(ind.route, [2, 1, 3])
+        self.assertEqual(ind.route, [1, 3])
         self.assertEqual([dr.node for dr in ind.data_records], [1, 1])
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(8)
         ind = Q.get_all_individuals()[0]
-        self.assertEqual(ind.route, [1, 3])
+        self.assertEqual(ind.route, [3])
         self.assertEqual([dr.node for dr in ind.data_records], [1, 1, 2])
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(10)
         ind = Q.get_all_individuals()[0]
-        self.assertEqual(ind.route, [3])
+        self.assertEqual(ind.route, [])
         self.assertEqual([dr.node for dr in ind.data_records], [1, 1, 2, 1])
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(12)
         ind = Q.get_all_individuals()[0]
         self.assertEqual(ind.route, [])
         self.assertEqual([dr.node for dr in ind.data_records], [1, 1, 2, 1, 3])
 
@@ -119,200 +97,159 @@
             arrival_distributions=[ciw.dists.Exponential(1), None, None],
             service_distributions=[
                 ciw.dists.Exponential(2),
                 ciw.dists.Exponential(2),
                 ciw.dists.Exponential(2),
             ],
             number_of_servers=[1, 1, 1],
-            routing=[generator_function_3, ciw.no_routing, ciw.no_routing],
+            routing=ciw.routing.ProcessBased(generator_function_3),
         )
         ciw.seed(0)
         Q = ciw.Simulation(N)
         Q.simulate_until_max_customers(500, method="Finish")
         inds = Q.nodes[-1].all_individuals
         routes_counter = Counter(
             [tuple(dr.node for dr in ind.data_records) for ind in inds]
         )
         self.assertEqual(
             routes_counter,
             Counter({(1, 3, 2, 3): 244, (1, 2, 2, 3, 2): 204, (1, 1): 52}),
         )
 
-    def test_error_when_ind_sent_wrong_place(self):
+    def test_customer_class_based_routing(self):
         N = ciw.create_network(
-            arrival_distributions=[ciw.dists.Exponential(1)],
-            service_distributions=[ciw.dists.Exponential(2)],
+            arrival_distributions={
+                "Class 0": [ciw.dists.Exponential(1)],
+                "Class 1": [ciw.dists.Exponential(1)],
+            },
+            service_distributions={
+                "Class 0": [ciw.dists.Exponential(2)],
+                "Class 1": [ciw.dists.Exponential(2)],
+            },
             number_of_servers=[1],
-            routing=[ciw.no_routing],
-        )
-        Q = ciw.Simulation(N)
-        self.assertRaises(ValueError, Q.simulate_until_max_time, 20)
-
-        N = ciw.create_network(
-            arrival_distributions=[None, ciw.dists.Exponential(1), None],
-            service_distributions=[
-                ciw.dists.Exponential(2),
-                ciw.dists.Exponential(2),
-                ciw.dists.Exponential(2),
-            ],
-            number_of_servers=[1, 1, 1],
-            routing=[ciw.no_routing, generator_function_2, ciw.no_routing],
-        )
-        Q = ciw.Simulation(N)
-        self.assertRaises(ValueError, Q.simulate_until_max_time, 20)
-
-    def test_routing_from_different_starting_points(self):
-        N = ciw.create_network(
-            arrival_distributions=[
-                ciw.dists.Exponential(1),
-                ciw.dists.Exponential(1),
-                None,
-            ],
-            service_distributions=[
-                ciw.dists.Exponential(2),
-                ciw.dists.Exponential(2),
-                ciw.dists.Exponential(2),
-            ],
-            number_of_servers=[1, 1, 1],
-            routing=[generator_function_2, generator_function_4, ciw.no_routing],
+            routing={
+                "Class 0": ciw.routing.ProcessBased(generator_function_4),
+                "Class 1": ciw.routing.ProcessBased(generator_function_1)
+            }
         )
         ciw.seed(0)
         Q = ciw.Simulation(N)
         Q.simulate_until_max_customers(500, method="Finish")
         inds = Q.nodes[-1].all_individuals
-        routes_counter = Counter([tuple(dr.node for dr in ind.data_records) for ind in inds])
-        self.assertEqual(
-            routes_counter,
-            Counter({(1, 1, 2, 1, 3): 245, (2, 1, 3, 1, 1): 255})
-        )
+        routes_counter = set([tuple([ind.customer_class, tuple(dr.node for dr in ind.data_records)]) for ind in inds])
+        self.assertEqual(routes_counter, {('Class 1', (1, 1, 1)), ('Class 0', (1,))})
 
+    def test_process_based_takes_methods(self):
+        import types
+        G = ClassForProcessBasedMethod(5)
+        self.assertTrue(isinstance(G.generator_method, types.MethodType))
         N = ciw.create_network(
-            arrival_distributions=[
-                ciw.dists.Exponential(1),
-                ciw.dists.Exponential(1),
-                ciw.dists.Exponential(1),
-            ],
-            service_distributions=[
-                ciw.dists.Exponential(2),
-                ciw.dists.Exponential(2),
-                ciw.dists.Exponential(2),
-            ],
-            number_of_servers=[1, 1, 1],
-            routing=[generator_function_1, generator_function_4, generator_function_5],
+            arrival_distributions=[ciw.dists.Deterministic(1)],
+            service_distributions=[ciw.dists.Deterministic(1000)],
+            number_of_servers=[1],
+            routing=ciw.routing.ProcessBased(G.generator_method),
         )
-        ciw.seed(0)
         Q = ciw.Simulation(N)
-        Q.simulate_until_max_customers(500, method="Finish")
-        inds = Q.nodes[-1].all_individuals
-        routes_counter = Counter([tuple(dr.node for dr in ind.data_records) for ind in inds])
-        self.assertEqual(
-            routes_counter,
-            Counter({(3, 2, 3, 2, 3): 256, (1, 1, 1): 155, (2, 1, 3, 1, 1): 89}),
-        )
+        Q.simulate_until_max_time(4.5)
+        inds = Q.nodes[1].all_individuals
+        for ind in inds:
+            self.assertEqual(ind.route, [1, 1])
 
+    def test_flexible_process_based(self):
+        ## First test 'any-random':
         N = ciw.create_network(
-            arrival_distributions=[
-                ciw.dists.Exponential(1),
-                ciw.dists.Exponential(1),
-                ciw.dists.Exponential(1),
-            ],
-            service_distributions=[
-                ciw.dists.Exponential(2),
-                ciw.dists.Exponential(2),
-                ciw.dists.Exponential(2),
-            ],
-            number_of_servers=[1, 1, 1],
-            routing=[generator_function_2, generator_function_4, generator_function_5],
+            arrival_distributions=[ciw.dists.Exponential(rate=1), None, None, None, None, None],
+            service_distributions=[ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2)],
+            number_of_servers=[3, 3, 3, 3, 3, 3],
+            routing=ciw.routing.FlexibleProcessBased(
+                route_function=flexible_generator_1,
+                rule='any',
+                choice='random'
+            )
         )
         ciw.seed(0)
         Q = ciw.Simulation(N)
-        Q.simulate_until_max_customers(500, method="Finish")
+        Q.simulate_until_max_customers(1000)
         inds = Q.nodes[-1].all_individuals
-        routes_counter = Counter([tuple(dr.node for dr in ind.data_records) for ind in inds])
+        routes_counter = Counter(
+            [tuple(dr.node for dr in ind.data_records) for ind in inds]
+        )
         self.assertEqual(
             routes_counter,
-            Counter({(3, 2, 3, 2, 3): 233, (1, 1, 2, 1, 3): 148, (2, 1, 3, 1, 1): 119}),
+            Counter({(1, 2, 4, 6): 350, (1, 2, 5, 6): 333, (1, 2, 3, 6): 317}), # all evenly spread
         )
 
+        ## Now test 'any-jsq' (flooding Node 4 so no customers ever go here):
         N = ciw.create_network(
-            arrival_distributions=[
-                ciw.dists.Exponential(1),
-                ciw.dists.Exponential(1),
-                ciw.dists.Exponential(1),
-            ],
-            service_distributions=[
-                ciw.dists.Exponential(2),
-                ciw.dists.Exponential(2),
-                ciw.dists.Exponential(2),
-            ],
-            number_of_servers=[1, 1, 1],
-            routing=[generator_function_2, generator_function_4, generator_function_6],
+            arrival_distributions=[ciw.dists.Exponential(rate=1), None, None, None, None, None],
+            service_distributions=[ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Deterministic(value=200000), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2)],
+            number_of_servers=[3, 3, 3, 3, 3, 3],
+            routing=ciw.routing.FlexibleProcessBased(
+                route_function=flexible_generator_1,
+                rule='any',
+                choice='jsq'
+            )
         )
         ciw.seed(0)
         Q = ciw.Simulation(N)
-        Q.simulate_until_max_customers(500, method="Finish")
+        Q.simulate_until_max_customers(1000)
         inds = Q.nodes[-1].all_individuals
-        routes_counter = Counter([tuple(dr.node for dr in ind.data_records) for ind in inds])
+        routes_counter = Counter(
+            [tuple(dr.node for dr in ind.data_records) for ind in inds]
+        )
         self.assertEqual(
             routes_counter,
-            Counter({(3,): 385, (1, 1, 2, 1, 3): 57, (2, 1, 3, 1, 1): 58}),
+            Counter({(1, 2, 5, 6): 503, (1, 2, 3, 6): 497}),  # evenly spread between the two unflooded nodes
         )
 
+        ## Now test 'any-lb' (flooding Node 4 so no customers ever go here):
         N = ciw.create_network(
-            arrival_distributions=[
-                ciw.dists.Exponential(1),
-                ciw.dists.Exponential(1),
-                None,
-            ],
-            service_distributions=[
-                ciw.dists.Exponential(2),
-                ciw.dists.Exponential(2),
-                ciw.dists.Exponential(2),
-            ],
-            number_of_servers=[1, 1, 1],
-            routing=[generator_function_1, generator_function_7, ciw.no_routing],
+            arrival_distributions=[ciw.dists.Exponential(rate=1), None, None, None, None, None],
+            service_distributions=[ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Deterministic(value=200000), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2)],
+            number_of_servers=[3, 3, 3, 3, 3, 3],
+            routing=ciw.routing.FlexibleProcessBased(
+                route_function=flexible_generator_1,
+                rule='any',
+                choice='lb'
+            )
         )
         ciw.seed(0)
         Q = ciw.Simulation(N)
-        Q.simulate_until_max_customers(500, method="Finish")
+        Q.simulate_until_max_customers(1000)
         inds = Q.nodes[-1].all_individuals
-        routes_counter = Counter([tuple(dr.node for dr in ind.data_records) for ind in inds])
+        routes_counter = Counter(
+            [tuple(dr.node for dr in ind.data_records) for ind in inds]
+        )
         self.assertEqual(
             routes_counter,
-            Counter({(2, 1, 1, 2): 172, (2, 1, 2): 169, (1, 1, 1): 159})
+            Counter({(1, 2, 5, 6): 508, (1, 2, 3, 6): 492}),  # evenly spread between the two unflooded nodes
         )
 
-    def test_customer_class_based_routing(self):
+
+        ## Now test 'all-random':
         N = ciw.create_network(
-            arrival_distributions={
-                "Class 0": [ciw.dists.Exponential(1)],
-                "Class 1": [ciw.dists.Exponential(1)],
-            },
-            service_distributions={
-                "Class 0": [ciw.dists.Exponential(2)],
-                "Class 1": [ciw.dists.Exponential(2)],
-            },
-            number_of_servers=[1],
-            routing=[generator_function_8],
+            arrival_distributions=[ciw.dists.Exponential(rate=1), None, None, None, None, None],
+            service_distributions=[ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2)],
+            number_of_servers=[3, 3, 3, 3, 3, 3],
+            routing=ciw.routing.FlexibleProcessBased(
+                route_function=flexible_generator_1,
+                rule='all',
+                choice='random'
+            )
         )
         ciw.seed(0)
         Q = ciw.Simulation(N)
-        Q.simulate_until_max_customers(500, method="Finish")
+        Q.simulate_until_max_customers(1000)
         inds = Q.nodes[-1].all_individuals
-        routes_counter = set([tuple([ind.customer_class, tuple(dr.node for dr in ind.data_records)]) for ind in inds])
-        self.assertEqual(routes_counter, {('Class 1', (1, 1, 1)), ('Class 0', (1,))})
-
-    def test_process_based_takes_methods(self):
-        import types
-        G = ClassForProcessBasedMethod(5)
-        self.assertTrue(isinstance(G.generator_method, types.MethodType))
-        N = ciw.create_network(
-            arrival_distributions=[ciw.dists.Deterministic(1)],
-            service_distributions=[ciw.dists.Deterministic(1000)],
-            number_of_servers=[1],
-            routing=[G.generator_method],
+        routes_counter = Counter(
+            [tuple(dr.node for dr in ind.data_records) for ind in inds]
         )
-        Q = ciw.Simulation(N)
-        Q.simulate_until_max_time(4.5)
-        inds = Q.nodes[1].all_individuals
-        for ind in inds:
-            self.assertEqual(ind.route, [1, 1, 1])
+        self.assertEqual(routes_counter[(1, 2, 3, 4, 5, 6)], 169)
+        self.assertEqual(routes_counter[(1, 2, 3, 5, 4, 6)], 139)
+        self.assertEqual(routes_counter[(1, 2, 4, 3, 5, 6)], 185)
+        self.assertEqual(routes_counter[(1, 2, 4, 5, 3, 6)], 166)
+        self.assertEqual(routes_counter[(1, 2, 5, 3, 4, 6)], 186)
+        self.assertEqual(routes_counter[(1, 2, 5, 4, 3, 6)], 155)
+
+    def test_flexible_process_based_error_raising(self):
+        self.assertRaises(ValueError, ciw.routing.FlexibleProcessBased, flexible_generator_1, 'something', 'random')
+        self.assertRaises(ValueError, ciw.routing.FlexibleProcessBased, flexible_generator_1, 'all', 'something')
```

### Comparing `Ciw-3.1.4/ciw/tests/test_processor_sharing.py` & `ciw-3.2.0/ciw/tests/test_processor_sharing.py`

 * *Files 13% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 )
 
 N_schedule = ciw.create_network(
     arrival_distributions={
         "Class 0": [ciw.dists.Exponential(0.05), ciw.dists.Exponential(0.04)],
         "Class 1": [ciw.dists.Exponential(0.04), ciw.dists.Exponential(0.06)],
     },
-    number_of_servers=[ciw.Schedule(schedule=[[1, 30], [2, 60], [1, 90], [3, 100]]), 3],
+    number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 2, 1, 3], shift_end_dates=[30, 60, 90, 100]), 3],
     queue_capacities=[float("Inf"), 10],
     service_distributions={
         "Class 0": [ciw.dists.Deterministic(5.0), ciw.dists.Exponential(0.2)],
         "Class 1": [ciw.dists.Deterministic(10.0), ciw.dists.Exponential(0.1)],
     },
     routing={"Class 0": [[0.8, 0.1], [0.0, 0.0]], "Class 1": [[0.8, 0.1], [0.2, 0.0]]},
 )
@@ -116,44 +116,59 @@
 
 class TestProcessorSharing(unittest.TestCase):
     def test_init_method(self):
         Q = ciw.Simulation(N_params, node_class=ciw.PSNode)
         N = ciw.PSNode(1, Q)
         self.assertEqual(N.ps_capacity, 9)
         self.assertEqual(N.c, float("inf"))
-        self.assertEqual(
-            [[round(p, 10) for p in row] for row in N.transition_row.values()],
-            [[0.1, 0.2, 0.1, 0.4, 0.2], [0.6, 0.0, 0.0, 0.2, 0.2], [0.0, 0.0, 0.4, 0.3, 0.3]],
-        )
+        router0 = Q.network.customer_classes["Class 0"].routing
+        router1 = Q.network.customer_classes["Class 1"].routing
+        router2 = Q.network.customer_classes["Class 2"].routing
+        self.assertEqual(router0.routers[0].destinations, [1, 2, 3, 4, -1])
+        self.assertEqual(router0.routers[1].destinations, [1, 2, 3, 4, -1])
+        self.assertEqual(router0.routers[2].destinations, [1, 2, 3, 4, -1])
+        self.assertEqual(router0.routers[3].destinations, [1, 2, 3, 4, -1])
+        self.assertEqual(router1.routers[0].destinations, [1, 2, 3, 4, -1])
+        self.assertEqual(router1.routers[1].destinations, [1, 2, 3, 4, -1])
+        self.assertEqual(router1.routers[2].destinations, [1, 2, 3, 4, -1])
+        self.assertEqual(router1.routers[3].destinations, [1, 2, 3, 4, -1])
+        self.assertEqual(router2.routers[0].destinations, [1, 2, 3, 4, -1])
+        self.assertEqual(router2.routers[1].destinations, [1, 2, 3, 4, -1])
+        self.assertEqual(router2.routers[2].destinations, [1, 2, 3, 4, -1])
+        self.assertEqual(router2.routers[3].destinations, [1, 2, 3, 4, -1])
+        self.assertEqual([round(p, 2) for p in router0.routers[0].probs], [0.1, 0.2, 0.1, 0.4, 0.2])
+        self.assertEqual([round(p, 2) for p in router0.routers[1].probs], [0.2, 0.2, 0.0, 0.1, 0.5])
+        self.assertEqual([round(p, 2) for p in router0.routers[2].probs], [0.0, 0.8, 0.1, 0.1, 0.0])
+        self.assertEqual([round(p, 2) for p in router0.routers[3].probs], [0.4, 0.1, 0.1, 0.0, 0.4])
+        self.assertEqual([round(p, 2) for p in router1.routers[0].probs], [0.6, 0.0, 0.0, 0.2, 0.2])
+        self.assertEqual([round(p, 2) for p in router1.routers[1].probs], [0.1, 0.1, 0.2, 0.2, 0.4])
+        self.assertEqual([round(p, 2) for p in router1.routers[2].probs], [0.9, 0.0, 0.0, 0.0, 0.1])
+        self.assertEqual([round(p, 2) for p in router1.routers[3].probs], [0.2, 0.1, 0.1, 0.1, 0.5])
+        self.assertEqual([round(p, 2) for p in router2.routers[0].probs], [0.0, 0.0, 0.4, 0.3, 0.3])
+        self.assertEqual([round(p, 2) for p in router2.routers[1].probs], [0.1, 0.1, 0.1, 0.1, 0.6])
+        self.assertEqual([round(p, 2) for p in router2.routers[2].probs], [0.1, 0.3, 0.2, 0.2, 0.2])
+        self.assertEqual([round(p, 2) for p in router2.routers[3].probs], [0.0, 0.0, 0.0, 0.3, 0.7])
+
         self.assertEqual(N.next_event_date, float("inf"))
         self.assertEqual(N.all_individuals, [])
         self.assertEqual(N.id_number, 1)
         self.assertEqual(N.interrupted_individuals, [])
         self.assertEqual(N.last_occupancy, 0)
 
         Q = ciw.Simulation(N_classchange, node_class=ciw.PSNode)
         N1 = Q.transitive_nodes[0]
         self.assertEqual(N1.class_change, {'Class 0': {'Class 0': 0.5, 'Class 1': 0.5}, 'Class 1': {'Class 0': 0.5, 'Class 1': 0.5}})
         N2 = Q.transitive_nodes[1]
         self.assertEqual(N2.class_change, {'Class 0': {'Class 0': 1.0, 'Class 1': 0.0}, 'Class 1': {'Class 0': 0.0, 'Class 1': 1.0}})
         self.assertEqual(N.interrupted_individuals, [])
 
-        Q = ciw.Simulation(N_schedule, node_class=ciw.PSNode)
-        N = Q.transitive_nodes[0]
-        self.assertEqual(N.schedule.cyclelength, 100)
-        self.assertEqual(N.ps_capacity, 1)
-        self.assertEqual(N.c, float("inf"))
-        self.assertEqual(N.schedule.schedule_dates, [30, 60, 90, 100])
-        self.assertEqual(N.schedule.schedule_servers, [1, 2, 1, 3])
-        self.assertEqual(N.next_event_date, 30)
-        self.assertEqual(N.interrupted_individuals, [])
-        self.assertEqual(N.last_occupancy, 0)
-
         Q = ciw.Simulation(N_priorities, node_class=ciw.PSNode)
         N = Q.transitive_nodes[0]
+        N.have_event()
+        N.update_next_event_date()
         self.assertEqual(N.ps_capacity, 4)
         self.assertEqual(N.c, float("inf"))
         self.assertEqual(Q.network.priority_class_mapping, {'Class 0': 0, 'Class 1': 1})
         self.assertEqual(Q.number_of_priority_classes, 2)
         self.assertEqual(N.interrupted_individuals, [])
         self.assertEqual(N.last_occupancy, 0)
```

### Comparing `Ciw-3.1.4/ciw/tests/test_sampling.py` & `ciw-3.2.0/ciw/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/tests/test_scheduling.py` & `ciw-3.2.0/ciw/tests/test_scheduling.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 import math
 
 N_schedule = ciw.create_network(
     arrival_distributions={
         "Class 0": [ciw.dists.Exponential(0.05), ciw.dists.Exponential(0.04)],
         "Class 1": [ciw.dists.Exponential(0.04), ciw.dists.Exponential(0.06)],
     },
-    number_of_servers=[ciw.Schedule(schedule=[[1, 30], [2, 60], [1, 90], [3, 100]]), 3],
+    number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 2, 1, 3], shift_end_dates=[30, 60, 90, 100]), 3],
     queue_capacities=[float("Inf"), 10],
     service_distributions={
         "Class 0": [ciw.dists.Deterministic(5.0), ciw.dists.Exponential(0.2)],
         "Class 1": [ciw.dists.Deterministic(10.0), ciw.dists.Exponential(0.1)],
     },
     routing={"Class 0": [[0.8, 0.1], [0.0, 0.0]], "Class 1": [[0.8, 0.1], [0.2, 0.0]]},
 )
 
 
 class TestScheduling(unittest.TestCase):
     def test_change_shift_method(self):
         Q = ciw.Simulation(N_schedule)
         N = Q.transitive_nodes[0]
+        N.have_event()
         N.next_event_date = 30
         self.assertEqual([str(obs) for obs in N.servers], ["Server 1 at Node 1"])
         self.assertEqual([obs.busy for obs in N.servers], [False])
         self.assertEqual([obs.offduty for obs in N.servers], [False])
         self.assertEqual(N.c, 1)
         N.change_shift()
         self.assertEqual(
@@ -59,14 +60,15 @@
         self.assertEqual([obs.busy for obs in N.servers], [True, False, False, False])
         self.assertEqual([obs.offduty for obs in N.servers], [True, False, False, False])
         self.assertEqual(N.c, 3)
 
     def test_take_servers_off_duty_method(self):
         Q = ciw.Simulation(N_schedule)
         N = Q.transitive_nodes[0]
+        N.have_event()
         N.add_new_servers(3)
         self.assertEqual(
             [str(obs) for obs in N.servers],
             [
                 "Server 1 at Node 1",
                 "Server 2 at Node 1",
                 "Server 3 at Node 1",
@@ -102,14 +104,15 @@
         self.assertEqual(ind2.service_end_date, 0.4321)
         self.assertEqual(N.interrupted_individuals, [])
 
 
     def test_kill_server_method(self):
         Q = ciw.Simulation(N_schedule)
         N = Q.transitive_nodes[0]
+        N.have_event()
         s = N.servers[0]
         self.assertEqual([str(obs) for obs in N.servers], ["Server 1 at Node 1"])
         N.kill_server(s)
         self.assertEqual(N.servers, [])
         N.next_event_date = 30
         N.next_event_type = "shift_change"
         N.have_event()
@@ -124,14 +127,15 @@
         self.assertEqual([obs.offduty for obs in N.servers], [True, False])
         N.detatch_server(N.servers[0], ind)
         self.assertEqual([str(obs) for obs in N.servers], ["Server 3 at Node 1"])
 
     def test_add_new_servers_method(self):
         Q = ciw.Simulation(N_schedule)
         N = Q.transitive_nodes[0]
+        N.have_event()
         self.assertEqual([str(obs) for obs in N.servers], ["Server 1 at Node 1"])
         N.add_new_servers(3)
         self.assertEqual(
             [str(obs) for obs in N.servers],
             [
                 "Server 1 at Node 1",
                 "Server 2 at Node 1",
@@ -175,14 +179,15 @@
         )
 
     def test_take_servers_off_duty_preempt_method(self):
         N = N_schedule
         N.service_centres[0].number_of_servers.preemption = 'resample'
         Q = ciw.Simulation(N)
         N = Q.transitive_nodes[0]
+        N.have_event()
         N.add_new_servers(3)
         self.assertEqual(
             [str(obs) for obs in N.servers],
             [
                 "Server 1 at Node 1",
                 "Server 2 at Node 1",
                 "Server 3 at Node 1",
@@ -229,15 +234,15 @@
 
     def test_full_preemptive_simulation(self):
         # Run until an individal gets interrupted
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Deterministic(7.0)],
             service_distributions=[ciw.dists.Deterministic(5.0)],
             routing=[[0.0]],
-            number_of_servers=[ciw.Schedule(schedule=[[1, 15], [0, 17], [2, 100]], preemption="resample")],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0, 2], shift_end_dates=[15, 17, 100], preemption="resample")],
         )
         Q = ciw.Simulation(N)
 
         self.assertEqual(Q.nodes[1].schedule.preemption, 'resample')
 
         Q.simulate_until_max_time(15.5)
 
@@ -253,15 +258,15 @@
         self.assertEqual(interrupted_ind.service_end_date, False)
 
         # Run until interrupted individual finishes service
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Deterministic(7.0)],
             service_distributions=[ciw.dists.Deterministic(5.0)],
             routing=[[0.0]],
-            number_of_servers=[ciw.Schedule(schedule=[[1, 15], [0, 17], [2, 100]], preemption="resume")],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0, 2], shift_end_dates=[15, 17, 100], preemption="resume")],
         )
         Q = ciw.Simulation(N)
 
         self.assertEqual(Q.nodes[1].schedule.preemption, 'resume')
 
         Q.simulate_until_max_time(22.5)
         recs = Q.get_all_records()
@@ -273,15 +278,15 @@
         # 4 due to the 1 time unit in service before interruption not counting.
 
         # Example where more customers are interrupted than can restart service
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Deterministic(3.0)],
             service_distributions=[ciw.dists.Deterministic(10.0)],
             routing=[[0.0]],
-            number_of_servers=[ciw.Schedule(schedule=[[4, 12.5], [0, 17], [1, 100]], preemption="resume")],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[4, 0, 1], shift_end_dates=[12.5, 17, 100], preemption="resume")],
         )
         Q = ciw.Simulation(N)
         self.assertEqual(Q.nodes[1].schedule.preemption, 'resume')
 
         Q.simulate_until_max_time(27.5)
         recs = Q.get_all_records(only=["service"])
         self.assertEqual(len(Q.nodes[1].interrupted_individuals), 1)
@@ -295,28 +300,28 @@
         # once the first customer has finished their second service, at time 17.5,
         # and there are 3.5 time units left.
 
     def test_overtime(self):
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Sequential([1.0, 0.0, 0.0, 8.0, 0.0, 3.0, 10000.0])],
             service_distributions=[ciw.dists.Sequential([5.0, 7.0, 9.0, 4.0, 5.0, 5.0])],
-            number_of_servers=[ciw.Schedule(schedule=[[3, 7.0], [2, 11.0], [1, 20.0]], preemption=False)],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[3, 2, 1], shift_end_dates=[7.0, 11.0, 20.0], preemption=False)],
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(19.0)
 
         nd = Q.transitive_nodes[0]
         self.assertEqual(nd.overtime, [0.0, 1.0, 3.0, 2.0, 3.0])
         self.assertEqual(sum(nd.overtime) / len(nd.overtime), 1.8)
 
     def test_overtime_exact(self):
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Sequential([1.0, 0.0, 0.0, 8.0, 0.0, 3.0, 10000.0])],
             service_distributions=[ciw.dists.Sequential([5.0, 7.0, 9.0, 4.0, 5.0, 5.0])],
-            number_of_servers=[ciw.Schedule(schedule=[[3, 7.0], [2, 11.0], [1, 20.0]], preemption=False)],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[3, 2, 1], shift_end_dates=[7.0, 11.0, 20.0], preemption=False)],
         )
         Q = ciw.Simulation(N, exact=26)
         Q.simulate_until_max_time(19.0)
 
         nd = Q.transitive_nodes[0]
         self.assertEqual(
             nd.overtime,
@@ -347,15 +352,15 @@
             - Under "resample" we would expect them to leave at time 29
             (service time = 20)
         """
         # Testing under restart
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Sequential([1, float("inf")])],
             service_distributions=[ciw.dists.Sequential([10, 20])],
-            number_of_servers=[ciw.Schedule(schedule=[[1, 5], [0, 9], [1, 100]], preemption="restart")],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0, 1], shift_end_dates=[5, 9, 100], preemption="restart")],
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(40)
         recs = Q.get_all_records(only=["service"])
         r1 = recs[0]
         self.assertEqual(r1.arrival_date, 1)
         self.assertEqual(r1.service_start_date, 9)
@@ -363,15 +368,15 @@
         self.assertEqual(r1.service_time, 10)
         self.assertEqual(r1.waiting_time, 8)
 
         # Testing under resume
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Sequential([1, float("inf")])],
             service_distributions=[ciw.dists.Sequential([10, 20])],
-            number_of_servers=[ciw.Schedule(schedule=[[1, 5], [0, 9], [1, 100]], preemption="resume")],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0, 1], shift_end_dates=[5, 9, 100], preemption="resume")],
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(40)
         recs = Q.get_all_records(only=["service"])
         r1 = recs[0]
         self.assertEqual(r1.arrival_date, 1)
         self.assertEqual(r1.service_start_date, 9)
@@ -379,15 +384,15 @@
         self.assertEqual(r1.service_time, 6)
         self.assertEqual(r1.waiting_time, 8)
 
         # Testing under resample
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Sequential([1, float("inf")])],
             service_distributions=[ciw.dists.Sequential([10, 20])],
-            number_of_servers=[ciw.Schedule(schedule=[[1, 5], [0, 9], [1, 100]], preemption="resample")],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0, 1], shift_end_dates=[5, 9, 100], preemption="resample")],
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(40)
         recs = Q.get_all_records(only=["service"])
         r1 = recs[0]
         self.assertEqual(r1.arrival_date, 1)
         self.assertEqual(r1.service_start_date, 9)
@@ -409,15 +414,15 @@
                 "Class 0": [ciw.dists.Deterministic(7)],
                 "Class 1": [ciw.dists.Deterministic(13)],
             },
             service_distributions={
                 "Class 0": [ciw.dists.Deterministic(5.5)],
                 "Class 1": [ciw.dists.Deterministic(1.5)],
             },
-            number_of_servers=[ciw.Schedule(schedule=[[1, 20.3], [0, 20.6], [1, 100]])],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0, 1], shift_end_dates=[20.3, 20.6, 100])],
             priority_classes=({"Class 0": 1, "Class 1": 0}, ["resume"]),
         )
 
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(35)
 
         recs = Q.get_all_records()
@@ -476,15 +481,15 @@
                 "Class 0": [ciw.dists.Deterministic(7)],
                 "Class 1": [ciw.dists.Deterministic(13)],
             },
             service_distributions={
                 "Class 0": [ciw.dists.Deterministic(5.5)],
                 "Class 1": [ciw.dists.Deterministic(1.5)],
             },
-            number_of_servers=[ciw.Schedule(schedule=[[1, 20.3], [0, 22], [1, 100]])],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0, 1], shift_end_dates=[20.3, 22, 100])],
             priority_classes=({"Class 0": 1, "Class 1": 0}, ["resume"]),
         )
 
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(35)
 
         recs = Q.get_all_records()
@@ -537,15 +542,15 @@
         self.assertEqual(recs[6].service_end_date, 34.5)
         self.assertEqual(recs[6].record_type, "service")
 
     def test_resuming_interruption_after_blockage(self):
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Sequential([5, float('inf')]), ciw.dists.Sequential([1, float('inf')])],
             service_distributions=[ciw.dists.Deterministic(1), ciw.dists.Deterministic(9)],
-            number_of_servers=[ciw.Schedule(schedule=[[1, 8], [0, 200]], preemption='resume'), 1],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0], shift_end_dates=[8, 200], preemption='resume'), 1],
             queue_capacities=[float('inf'), 0],
             routing=[[0.0, 1.0], [0.0, 0.0]]
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(35)
 
         C1 = Q.nodes[-1].all_individuals[0]
@@ -624,14 +629,38 @@
         self.assertEqual(len(Q.nodes[-1].all_individuals), 9)
 
         expected_service_dates = [1, 1, 1, 2, 2, 3, 3, 3, 4]
         observed_service_dates = [r.service_start_date for r in recs]
         self.assertEqual(observed_service_dates, expected_service_dates)
         self.assertFalse(any([ind.server for ind in Q.nodes[-1].all_individuals]))
 
+    def test_slotted_services_with_offset(self):
+        """
+        Arrivals occur at times [0.3, 0.5, 0.7, 1.2, 1.3, 1.8, 2.6, 2.7, 3.1]
+        All services last 0.5 time units
+        Services are slotted at times [1.05, 2.05, 3.05, 4.05]
+        Slotted services have capacities [3, 2, 5, 3]
+        """
+        N = ciw.create_network(
+            arrival_distributions=[ciw.dists.Sequential([0.3, 0.2, 0.2, 0.5, 0.1, 0.5, 0.8, 0.1, 0.4, float('inf')])],
+            service_distributions=[ciw.dists.Deterministic(0.5)],
+            number_of_servers=[ciw.Slotted(slots=[1, 2, 3, 4], slot_sizes=[3, 2, 5, 3], offset=0.05)]
+        )
+        Q = ciw.Simulation(N)
+        Q.simulate_until_max_time(5.6)
+        recs = Q.get_all_records()
+        recs = sorted(recs, key=lambda rec: rec.id_number)
+
+        self.assertEqual(len(Q.nodes[-1].all_individuals), 9)
+
+        expected_service_dates = [1.05, 1.05, 1.05, 2.05, 2.05, 3.05, 3.05, 3.05, 4.05]
+        observed_service_dates = [r.service_start_date for r in recs]
+        self.assertEqual(observed_service_dates, expected_service_dates)
+        self.assertFalse(any([ind.server for ind in Q.nodes[-1].all_individuals]))
+
     def test_slotted_services_repeat(self):
         """
         Arrivals occur at times [0.7, 1.4, 2.6, 2.9, 4.3, 5.5, 6.1, 15.0]
         All services last 0.2 time units
         Services are slotted at times [1.5, 4.4, 5.9, 8.8, 10.3, 13.2, 14.7, 17.6, etc...]
         Slotted services have capacities [1, 3, 1, 3, 1, 3, 1, 3 etc....]
         """
@@ -713,15 +742,15 @@
         recs = sorted(recs, key=lambda rec: rec.id_number)
         self.assertEqual(len(Q.nodes[-1].all_individuals), 5)
         expected_service_dates = [2, 2, 2, 2, 5]
         observed_service_dates = [r.service_start_date for r in recs]
         self.assertEqual(observed_service_dates, expected_service_dates)
 
     def test_invalid_preemption_options(self):
-        self.assertRaises(ValueError, lambda: ciw.Schedule(schedule=[[2, 10], [1, 12]], preemption='something'))
+        self.assertRaises(ValueError, lambda: ciw.Schedule(numbers_of_servers=[2, 1], shift_end_dates=[10, 12], preemption='something'))
         self.assertRaises(ValueError, lambda: ciw.Slotted(slots=[2, 3], slot_sizes=[4, 1], capacitated=False, preemption='resume'))
         self.assertRaises(ValueError, lambda: ciw.Slotted(slots=[2, 3], slot_sizes=[4, 1], capacitated=True, preemption='something'))
 
     def test_slotted_services_capacitated_preemption(self):
         """
         Tests when the service times of slotted services last longer
         than the gap between the slots, and jobs are pre-empted
@@ -859,7 +888,45 @@
         self.assertEqual(recs[2].arrival_date, 0.5)
         self.assertEqual(recs[2].service_start_date, 15)
         self.assertEqual(recs[2].service_time, 10)
         self.assertEqual(recs[2].service_end_date, 25)
         self.assertEqual(recs[2].exit_date, 25)
         self.assertEqual(recs[2].record_type, 'service')
 
+    def test_offset_error_raising(self):
+        self.assertRaises(ValueError, lambda: ciw.Slotted(slots=[4, 11], slot_sizes=[3, 1], offset='something'))
+        self.assertRaises(ValueError, lambda: ciw.Slotted(slots=[4, 11], slot_sizes=[3, 1], offset=-6.7))
+        self.assertRaises(ValueError, lambda: ciw.Schedule(numbers_of_servers=[1, 2], shift_end_dates=[10, 25], offset='something'))
+        self.assertRaises(ValueError, lambda: ciw.Schedule(numbers_of_servers=[1, 2], shift_end_dates=[10, 25], offset=-6.7))
+
+    def test_schedules_with_offset(self):
+        """
+        First with no offset
+        """
+        N = ciw.create_network(
+            arrival_distributions=[ciw.dists.Sequential([0.1, float('inf')])],
+            service_distributions=[ciw.dists.Deterministic(10)],
+            batching_distributions=[ciw.dists.Deterministic(10)],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0, 6, 0], shift_end_dates=[5, 20, 23, 30])]
+        )
+        Q = ciw.Simulation(N)
+        Q.simulate_until_max_time(3000)
+        recs = Q.get_all_records()
+
+        expected_service_dates = [0.1, 20, 20, 20, 20, 20, 20, 30, 50, 50]
+        self.assertEqual(expected_service_dates, [r.service_start_date for r in recs])
+        """
+        Now with an offset
+        """
+        N = ciw.create_network(
+            arrival_distributions=[ciw.dists.Sequential([0.1, float('inf')])],
+            service_distributions=[ciw.dists.Deterministic(10)],
+            batching_distributions=[ciw.dists.Deterministic(10)],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0, 6, 0], shift_end_dates=[5, 20, 23, 30], offset=0.5)]
+        )
+        Q = ciw.Simulation(N)
+        Q.simulate_until_max_time(3000)
+        recs = Q.get_all_records()
+
+        expected_service_dates = [0.5, 20.5, 20.5, 20.5, 20.5, 20.5, 20.5, 30.5, 50.5, 50.5]
+        self.assertEqual(expected_service_dates, [r.service_start_date for r in recs])
+
```

### Comparing `Ciw-3.1.4/ciw/tests/test_server.py` & `ciw-3.2.0/ciw/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/ciw/tests/test_simulation.py` & `ciw-3.2.0/ciw/tests/test_simulation.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from hypothesis.strategies import floats, integers, random_module
 import os
 from decimal import Decimal
 import networkx as nx
 import csv
 from itertools import cycle
 import types
+import math
 
 N_params = ciw.create_network(
     arrival_distributions={
         "Class 0": [
             ciw.dists.Exponential(3.0),
             ciw.dists.Exponential(7.0),
             ciw.dists.Exponential(4.0),
@@ -412,15 +413,15 @@
         self.assertAlmostEqual(completed_inds.count(2) / float(1000), 1 / 4.0, places=1)
 
     def test_exactness(self):
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Exponential(20)],
             service_distributions=[ciw.dists.Deterministic(0.01)],
             routing=[[0.0]],
-            number_of_servers=[ciw.Schedule(schedule=[[0, 0.5], [1, 0.55], [0, 3.0]])],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[0, 1, 0], shift_end_dates=[0.5, 0.55, 3.0])],
         )
         ciw.seed(777)
         Q = ciw.Simulation(N)
         Q.simulate_until_max_time(10)
         recs = Q.get_all_records()
         mod_service_starts = [obs % 3 for obs in [r[6] for r in recs]]
         self.assertNotEqual(
@@ -433,15 +434,15 @@
             set([0.50, 0.51, 0.52, 0.53, 0.54, 0.55])
         )
 
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Exponential(20)],
             service_distributions=[ciw.dists.Deterministic(0.01)],
             routing=[[0.0]],
-            number_of_servers=[ciw.Schedule(schedule=[[0, 0.5], [1, 0.55], [0, 3.0]])],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[0, 1, 0], shift_end_dates=[0.5, 0.55, 3.0])],
         )
 
         ciw.seed(777)
         Q = ciw.Simulation(N, exact=14)
         Q.simulate_until_max_time(10)
         recs = Q.get_all_records()
         mod_service_starts = [obs % 3 for obs in [r[6] for r in recs]]
@@ -574,15 +575,15 @@
         class DummyArrivalNode(ciw.ArrivalNode):
             pass
 
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Exponential(20)],
             service_distributions=[ciw.dists.Deterministic(0.01)],
             routing=[[0.0]],
-            number_of_servers=[ciw.Schedule(schedule=[[0, 0.5], [1, 0.55], [0, 3.0]])],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[0, 1, 0], shift_end_dates=[0.5, 0.55, 3.0])],
         )
         Q = ciw.Simulation(N, node_class=None, arrival_node_class=None)
         self.assertEqual(Q.NodeTypes, [ciw.Node])
         self.assertEqual(Q.ArrivalNodeType, ciw.ArrivalNode)
         self.assertIsInstance(Q.nodes[1], ciw.Node)
         self.assertIsInstance(Q.nodes[0], ciw.ArrivalNode)
         self.assertFalse(isinstance(Q.nodes[1], DummyNode))
@@ -625,15 +626,15 @@
                 ciw.dists.Exponential(10),
             ],
             service_distributions=[
                 ciw.dists.Exponential(10),
                 ciw.dists.Exponential(10),
                 ciw.dists.Exponential(10),
             ],
-            routing=[[0, 0, 0], [0, 0, 0], [0, 0, 0]],
+            routing=[[0.0, 0.0, 0.0], [0.0, 0.0, 0.0], [0.0, 0.0, 0.0]],
             number_of_servers=[1, 1, 1],
         )
 
         Q = ciw.Simulation(N)
         self.assertEqual(Q.NodeTypes, [ciw.Node, ciw.Node, ciw.Node])
         self.assertIsInstance(Q.nodes[1], ciw.Node)
         self.assertIsInstance(Q.nodes[2], ciw.Node)
@@ -711,15 +712,15 @@
                     ciw.dists.Exponential(10),
                 ],
                 service_distributions=[
                     ciw.dists.Exponential(10),
                     ciw.dists.Exponential(10),
                     ciw.dists.Exponential(10),
                 ],
-                routing=[[0, 0, 0], [0, 0, 0], [0, 0, 0]],
+                routing=[[0.0, 0.0, 0.0], [0.0, 0.0, 0.0], [0.0, 0.0, 0.0]],
                 number_of_servers=[1, 1, 1],
             )
             return ciw.Simulation(N, node_class=node_classes)
 
         two_nodes = [DummyNode, DummyNode]
         four_nodes = [DummyNode, DummyNode, DummyNode, DummyNode]
         self.assertRaises(ValueError, create_simulation_with_node_classes, two_nodes)
@@ -1090,42 +1091,42 @@
                 "Class 0": [ciw.dists.Exponential(0.5), ciw.dists.Exponential(0.9)],
                 "Class 1": [ciw.dists.Exponential(0.6), ciw.dists.Exponential(1.0)],
             },
             service_distributions={
                 "Class 0": [ciw.dists.Exponential(0.8), ciw.dists.Exponential(1.2)],
                 "Class 1": [ciw.dists.Exponential(0.5), ciw.dists.Exponential(1.0)],
             },
-            number_of_servers=[ciw.Schedule(schedule=[[1, 10], [0, 20], [2, 30]], preemption="resample"), 2],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0, 2], shift_end_dates=[10, 20, 30], preemption="resample"), 2],
             routing={
                 "Class 0": [[0.1, 0.3], [0.2, 0.2]],
                 "Class 1": [[0.0, 0.6], [0.2, 0.1]],
             },
             class_change_matrices=[
                 {'Class 0': {'Class 0': 0.8, 'Class 1': 0.2}, 'Class 1': {'Class 0': 0.5, 'Class 1': 0.5}},
                 {'Class 0': {'Class 0': 1.0, 'Class 1': 0.0}, 'Class 1': {'Class 0': 0.1, 'Class 1': 0.9}}
             ],
             queue_capacities=[2, 2],
         )
-        ciw.seed(11)
+        ciw.seed(10)
         Q = ciw.Simulation(
             N,
             deadlock_detector=ciw.deadlock.StateDigraph(),
             tracker=ciw.trackers.NaiveBlocking(),
         )
         Q.simulate_until_deadlock()
         ttd = Q.times_to_deadlock[((0, 0), (0, 0))]
-        self.assertEqual(round(ttd, 5), 119.65819)
+        self.assertEqual(round(ttd, 5), 51.75691)
 
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Deterministic(1.0), None],
             service_distributions=[
                 ciw.dists.Deterministic(0.1),
                 ciw.dists.Deterministic(3.0),
             ],
-            number_of_servers=[ciw.Schedule(schedule=[[1, 2.5], [0, 2.8]], preemption="resample"), 1],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0], shift_end_dates=[2.5, 2.8], preemption="resample"), 1],
             queue_capacities=[float("inf"), 0],
             routing=[[0.0, 1.0], [0.0, 0.0]],
         )
         Q = ciw.Simulation(N)
         Q.simulate_until_max_customers(3, method="Finish")
         inds = Q.nodes[-1].all_individuals
         service_times = [
@@ -1136,14 +1137,381 @@
         ]
         self.assertEqual(service_times, [0.1, 3.0, 0.1, 3.0, 0.1, 3.0])
 
     def test_generic_deadlock_detector(self):
         DD = ciw.deadlock.NoDetection()
         self.assertEqual(DD.detect_deadlock(), False)
 
+    def test_system_capacity(self):
+        """
+        Expected results would be:
+
+        node    id  arrival_date  current_capacity  start_date  end_date
+        ----------------------------------------------------------------
+           1     1           0.8                 1         0.8       5.9
+           2     2           1.0                 2         1.0       6.1
+           1     3           1.6                 3         5.9      11.0
+           2     4           2.0                 4         6.1      11.2
+           1     5           2.4                 5        11.0      16.1
+           2     6           3.0                 reject
+           1     7           3.2                 reject
+          1,2  8,9           4.0                 reject
+           1    10           4.8                 reject
+           2    11           5.0                 reject
+           1    12           5.6                 reject
+           2    13           6.0                 5        11.2      16.3
+           1    14           6.4                 5        16.1      21.2
+           2    15           7.0                 reject
+           1    16           7.2                 reject
+          1,2  17,18         8.0                 reject
+           1    19           8.8                 reject
+           2    20           9.0                 reject
+           1    21           9.6                 reject
+           2    22          10.0                 reject
+           1    23          10.4                 reject
+           2    24          11.0                 5      16.3       21.4
+           1    25          11.2                 5      21.2       26.3  (incomplete)
+           2    26          12.0                 reject
+           1    27          12.0                 reject
+        """
+        N = ciw.create_network(
+            arrival_distributions=[ciw.dists.Deterministic(0.8), ciw.dists.Deterministic(1)],
+            service_distributions=[ciw.dists.Deterministic(5.1), ciw.dists.Deterministic(5.1)],
+            routing=[[0.0, 0.0], [0.0, 0.0]],
+            number_of_servers=[1, 1],
+            system_capacity=5
+        )
+        ciw.seed(0) ## Set seed to exactly replicate simultaneous events
+        Q = ciw.Simulation(N, tracker=ciw.trackers.SystemPopulation())
+        Q.simulate_until_max_time(22)
+        recs_service = sorted(Q.get_all_records(only=['service']), key=lambda r: r.arrival_date)
+        recs_reject = sorted(Q.get_all_records(only=['rejection']), key=lambda r: r.arrival_date)
+
+        expected_arrivals = [0.8, 1.0, 1.6, 2.0, 2.4, 6.0, 6.4, 11.0]
+        expected_ssds = [0.8, 1.0, 5.9, 6.1, 11.0, 11.2, 16.1, 16.3]
+        expected_seds = [5.9, 6.1, 11.0, 11.2, 16.1, 16.3, 21.2, 21.4]
+        expected_nodes = [1, 2, 1, 2, 1, 2, 1, 2]
+        expected_first_10_rejection_times = [3.0, 3.2, 4.0, 4.0, 4.8, 5.0, 5.6, 7.0, 7.2, 8.0]
+
+        self.assertTrue(all([s[1] <= 5 for s in Q.statetracker.history]))
+        self.assertEqual([round(r.arrival_date, 2) for r in recs_service], expected_arrivals)
+        self.assertEqual([r.node for r in recs_service], expected_nodes)
+        self.assertEqual([round(r.service_start_date, 2) for r in recs_service], expected_ssds)
+        self.assertEqual([round(r.service_end_date, 2) for r in recs_service], expected_seds)
+        self.assertEqual([round(r.arrival_date, 2) for r in recs_reject][:10], expected_first_10_rejection_times)
+
+    def test_reroute_preemption_classpriorities(self):
+        """
+        Class 0 arrive to Node 1 every 0.7, service lasts 0.2
+        Class 1 arrive to Node 1 every 1.0, service lasts 0.2
+        Class 0 have priority over class 1
+        Class 1 rerouted to Node 2 upon preemption
+
+        Ind    arr    clss    end
+          1    0.7       0    0.9
+          2    1.0       1    1.2
+          3    1.4       0    1.6
+          4    2.0       1    interrupted (goes to Node 2 for 0.5)
+          5    2.1       0    2.3
+        """
+        class Reroute(ciw.routing.NodeRouting):
+            def next_node(self, ind):
+                """
+                Chooses the exit node with probability 1.
+                """
+                return self.simulation.nodes[-1]
+
+            def next_node_for_rerouting(self, ind):
+                """
+                Chooses Node 2
+                """
+                return self.simulation.nodes[2]
+
+        N = ciw.create_network(
+            arrival_distributions={
+                'Class 0': [ciw.dists.Deterministic(value=0.7), None],
+                'Class 1': [ciw.dists.Deterministic(value=1.0), None]
+            },
+            service_distributions={
+                'Class 0': [ciw.dists.Deterministic(value=0.2), ciw.dists.Deterministic(value=0.5)],
+                'Class 1': [ciw.dists.Deterministic(value=0.2), ciw.dists.Deterministic(value=0.5)]
+            },
+            number_of_servers=[1, 1],
+            priority_classes=({'Class 0': 0, 'Class 1': 1}, ['reroute', False]),
+            routing={
+                'Class 0': ciw.routing.NetworkRouting(routers=[ciw.routing.Leave(), ciw.routing.Leave()]),
+                'Class 1': ciw.routing.NetworkRouting(routers=[Reroute(), ciw.routing.Leave()])
+            }
+        )
+        Q = ciw.Simulation(N)
+        Q.simulate_until_max_time(2.7)
+        recs = Q.get_all_records()
+
+        nd_1 = sorted([r for r in recs if r.node == 1], key=lambda r: r.arrival_date)
+        self.assertEqual([round(r.arrival_date, 5) for r in nd_1], [0.7, 1.0, 1.4, 2.0, 2.1])
+        self.assertEqual([round(r.service_time, 5) for r in nd_1], [0.2, 0.2, 0.2, 0.2, 0.2])
+        self.assertEqual([round(r.exit_date, 5) for r in nd_1], [0.9, 1.2, 1.6, 2.1, 2.3])
+        self.assertEqual([r.destination for r in nd_1], [-1, -1, -1, 2, -1])
+        self.assertEqual([r.record_type for r in nd_1], ['service', 'service', 'service', 'interrupted service', 'service'])
+
+        nd_2 = sorted([r for r in recs if r.node == 2], key=lambda r: r.arrival_date)
+        self.assertEqual([round(r.arrival_date, 5) for r in nd_2], [2.1])
+        self.assertEqual([round(r.service_time, 5) for r in nd_2], [0.5])
+        self.assertEqual([round(r.exit_date, 5) for r in nd_2], [2.6])
+        self.assertEqual([r.destination for r in nd_2], [-1])
+        self.assertEqual([r.record_type for r in nd_2], ['service'])
+
+        """
+        Class 0 arrive to Node 1 every 0.7, service lasts 0.2
+        Class 1 arrive to Node 1 every 1.0, service lasts 0.2
+        Class 0 have priority over class 1
+        All classes go Node 1 then Node 2
+
+        Node 1
+        Ind    arr    clss    end
+          1    0.7       0    0.9
+          2    1.0       1    1.2
+          3    1.4       0    1.6
+          4    2.0       1    interrupted
+          5    2.1       0    2.3
+
+        Node 2
+        Ind    arr    clss    end
+          1    0.9       0    1.0
+          2    1.2       1    1.3
+          3    1.6       0    1.7
+          4    2.1       1    2.2
+          5    2.3       0    2.4
+        """
+        N = ciw.create_network(
+            arrival_distributions={
+                'Class 0': [ciw.dists.Deterministic(value=0.7), None],
+                'Class 1': [ciw.dists.Deterministic(value=1.0), None]
+            },
+            service_distributions={
+                'Class 0': [ciw.dists.Deterministic(value=0.2), ciw.dists.Deterministic(value=0.1)],
+                'Class 1': [ciw.dists.Deterministic(value=0.2), ciw.dists.Deterministic(value=0.1)]
+            },
+            number_of_servers=[1, 1],
+            priority_classes=({'Class 0': 0, 'Class 1': 1}, ['reroute', False]),
+            routing={
+                'Class 0': ciw.routing.TransitionMatrix(transition_matrix=[[0.0, 1.0], [0.0, 0.0]]),
+                'Class 1': ciw.routing.TransitionMatrix(transition_matrix=[[0.0, 1.0], [0.0, 0.0]])
+            }
+        )
+        Q = ciw.Simulation(N)
+        Q.simulate_until_max_time(2.7)
+        recs = Q.get_all_records()
+
+        nd_1 = sorted([r for r in recs if r.node == 1], key=lambda r: r.arrival_date)
+        self.assertEqual([round(r.arrival_date, 5) for r in nd_1], [0.7, 1.0, 1.4, 2.0, 2.1])
+        self.assertEqual([round(r.service_time, 5) for r in nd_1], [0.2, 0.2, 0.2, 0.2, 0.2])
+        self.assertEqual([round(r.exit_date, 5) for r in nd_1], [0.9, 1.2, 1.6, 2.1, 2.3])
+        self.assertEqual([r.destination for r in nd_1], [2, 2, 2, 2, 2])
+        self.assertEqual([r.record_type for r in nd_1], ['service', 'service', 'service', 'interrupted service', 'service'])
+
+        nd_2 = sorted([r for r in recs if r.node == 2], key=lambda r: r.arrival_date)
+        self.assertEqual([round(r.arrival_date, 5) for r in nd_2], [0.9, 1.2, 1.6, 2.1, 2.3])
+        self.assertEqual([round(r.service_time, 5) for r in nd_2], [0.1, 0.1, 0.1, 0.1, 0.1])
+        self.assertEqual([round(r.exit_date, 5) for r in nd_2], [1.0, 1.3, 1.7, 2.2, 2.4])
+        self.assertEqual([r.destination for r in nd_2], [-1, -1, -1, -1, -1])
+        self.assertEqual([r.record_type for r in nd_2], ['service', 'service', 'service', 'service', 'service'])
+
+    def test_reroute_preemption_classpriorities_process_based(self):
+        """
+        Class 0 arrive to Node 1 every 0.7, service lasts 0.2
+        Class 1 arrive to Node 1 every 1.0, service lasts 0.2
+        Class 0 have priority over class 1
+        All classes go Node 1 then Node 2
+
+        Node 1
+        Ind    arr    clss    end
+          1    0.7       0    0.9
+          2    1.0       1    1.2
+          3    1.4       0    1.6
+          4    2.0       1    interrupted
+          5    2.1       0    2.3
+
+        Node 2
+        Ind    arr    clss    end
+          1    0.9       0    1.0
+          2    1.2       1    1.3
+          3    1.6       0    1.7
+          4    2.1       1    2.2
+          5    2.3       0    2.4
+        """
+        def from_1_to_2(ind, simulation):
+            return [2]
+
+        N = ciw.create_network(
+            arrival_distributions={
+                'Class 0': [ciw.dists.Deterministic(value=0.7), None],
+                'Class 1': [ciw.dists.Deterministic(value=1.0), None]
+            },
+            service_distributions={
+                'Class 0': [ciw.dists.Deterministic(value=0.2), ciw.dists.Deterministic(value=0.1)],
+                'Class 1': [ciw.dists.Deterministic(value=0.2), ciw.dists.Deterministic(value=0.1)]
+            },
+            number_of_servers=[1, 1],
+            priority_classes=({'Class 0': 0, 'Class 1': 1}, ['reroute', False]),
+            routing={
+                'Class 0': ciw.routing.ProcessBased(from_1_to_2),
+                'Class 1': ciw.routing.ProcessBased(from_1_to_2)
+            }
+        )
+        Q = ciw.Simulation(N)
+        Q.simulate_until_max_time(2.7)
+        recs = Q.get_all_records()
+
+        nd_1 = sorted([r for r in recs if r.node == 1], key=lambda r: r.arrival_date)
+        self.assertEqual([round(r.arrival_date, 5) for r in nd_1], [0.7, 1.0, 1.4, 2.0, 2.1])
+        self.assertEqual([round(r.service_time, 5) for r in nd_1], [0.2, 0.2, 0.2, 0.2, 0.2])
+        self.assertEqual([round(r.exit_date, 5) for r in nd_1], [0.9, 1.2, 1.6, 2.1, 2.3])
+        self.assertEqual([r.destination for r in nd_1], [2, 2, 2, 2, 2])
+        self.assertEqual([r.record_type for r in nd_1], ['service', 'service', 'service', 'interrupted service', 'service'])
+
+        nd_2 = sorted([r for r in recs if r.node == 2], key=lambda r: r.arrival_date)
+        self.assertEqual([round(r.arrival_date, 5) for r in nd_2], [0.9, 1.2, 1.6, 2.1, 2.3])
+        self.assertEqual([round(r.service_time, 5) for r in nd_2], [0.1, 0.1, 0.1, 0.1, 0.1])
+        self.assertEqual([round(r.exit_date, 5) for r in nd_2], [1.0, 1.3, 1.7, 2.2, 2.4])
+        self.assertEqual([r.destination for r in nd_2], [-1, -1, -1, -1, -1])
+        self.assertEqual([r.record_type for r in nd_2], ['service', 'service', 'service', 'service', 'service'])
+
+    def test_rerouting_ignores_queue_capacities(self):
+        """
+        Class 0 arrive to Node 1 every 0.7, service lasts 0.2
+        Class 1 arrive to Node 1 every 1.0, service lasts 0.2
+        Class 0 have priority over class 1
+        Class 1 rerouted to Node 2 upon preemption
+        Class 2 arrive at Node 2 every 0.6
+        
+        Node 1
+        Ind    arr    clss    end
+          2    0.7       0    0.9
+          3    1.0       1    1.2
+          5    1.4       0    1.6
+          6    2.0       1    interrupted (goes to Node 2 for 0.5)
+          7    2.1       0    2.3
+
+        Node 2
+        Ind    arr    clss    end
+          1    0.6       2    1.3
+          4    1.2       2    rejected
+          3    1.8       2    2.5
+          6    2.1       1    (2.5 + 0.7 =) 3.2 (individual is accepted even though a queue capacity of 0)
+          8    2.4       2    rejected
+        """
+        class Reroute(ciw.routing.NodeRouting):
+            def next_node(self, ind):
+                """
+                Chooses the exit node with probability 1.
+                """
+                return self.simulation.nodes[-1]
+
+            def next_node_for_rerouting(self, ind):
+                """
+                Chooses Node 2
+                """
+                return self.simulation.nodes[2]
+
+        N = ciw.create_network(
+            arrival_distributions={
+                'Class 0': [ciw.dists.Deterministic(value=0.7), None],
+                'Class 1': [ciw.dists.Deterministic(value=1.0), None],
+                'Class 2': [None, ciw.dists.Deterministic(value=0.6)]
+            },
+            service_distributions={
+                'Class 0': [ciw.dists.Deterministic(value=0.2), ciw.dists.Deterministic(value=0.7)],
+                'Class 1': [ciw.dists.Deterministic(value=0.2), ciw.dists.Deterministic(value=0.7)],
+                'Class 2': [ciw.dists.Deterministic(value=0.2), ciw.dists.Deterministic(value=0.7)]
+            },
+            number_of_servers=[1, 1],
+            queue_capacities=[float('inf'), 0],
+            priority_classes=({'Class 0': 0, 'Class 1': 1, 'Class 2': 1}, ['reroute', False]),
+            routing={
+                'Class 0': ciw.routing.NetworkRouting(routers=[ciw.routing.Leave(), ciw.routing.Leave()]),
+                'Class 1': ciw.routing.NetworkRouting(routers=[Reroute(), ciw.routing.Leave()]),
+                'Class 2': ciw.routing.NetworkRouting(routers=[ciw.routing.Leave(), ciw.routing.Leave()])
+            }
+        )
+        Q = ciw.Simulation(N)
+        Q.simulate_until_max_time(3.3)
+        recs = Q.get_all_records()
+
+        nd_1 = sorted([r for r in recs if r.node == 1], key=lambda r: r.arrival_date)[:5]
+        self.assertEqual([round(r.arrival_date, 5) for r in nd_1], [0.7, 1.0, 1.4, 2.0, 2.1])
+        self.assertEqual([round(r.service_time, 5) for r in nd_1], [0.2, 0.2, 0.2, 0.2, 0.2])
+        self.assertEqual([round(r.exit_date, 5) for r in nd_1], [0.9, 1.2, 1.6, 2.1, 2.3])
+        self.assertEqual([r.destination for r in nd_1], [-1, -1, -1, 2, -1])
+        self.assertEqual([r.record_type for r in nd_1], ['service', 'service', 'service', 'interrupted service', 'service'])
+
+        nd_2 = sorted([r for r in recs if r.node == 2], key=lambda r: r.arrival_date)[:5]
+        self.assertEqual([round(r.arrival_date, 5) for r in nd_2], [0.6, 1.2, 1.8, 2.1, 2.4])
+        self.assertEqual([str(round(r.service_time, 5)) for r in nd_2], ['0.7', 'nan', '0.7', '0.7', 'nan'])
+        self.assertEqual([round(r.exit_date, 5) for r in nd_2], [1.3, 1.2, 2.5, 3.2, 2.4])
+        self.assertEqual([str(r.destination) for r in nd_2], ['-1', 'nan', '-1', '-1', 'nan'])
+        self.assertEqual([r.record_type for r in nd_2], ['service', 'rejection', 'service', 'service', 'rejection'])
+
+    def test_reroute_at_shift_change(self):
+        """
+        Two nodes: arrivals to Node 1 every 1 time unit; service lasts 0.4 time units.
+        One server on duty from - to 4.2; 0 from 4.2 to 6.1; 1 from 6.1 to 100.
+        Interrupted individuals go to node 2, have service time 1.
+
+        Node 1
+        Ind    arr    exit
+          1    1.0     1.4
+          2    2.0     2.4
+          3    3.0     4.4
+          4    4.0     4.2 (interrupted)
+          5    5.0     6.5 (service started at 6.1 when server back on duty)
+          6    6.0     6.9 (service starts after ind 5 finishes service)
+          7    7.0     7.4
+
+        Node 2
+        Ind    arr    exit
+          4    4.2     5.2
+        """
+        class Reroute(ciw.routing.NodeRouting):
+            def next_node(self, ind):
+                """
+                Chooses the exit node with probability 1.
+                """
+                return self.simulation.nodes[-1]
+
+            def next_node_for_rerouting(self, ind):
+                """
+                Chooses Node 2
+                """
+                return self.simulation.nodes[2]
+
+        N = ciw.create_network(
+            arrival_distributions=[ciw.dists.Deterministic(value=1.0), None],
+            service_distributions=[ciw.dists.Deterministic(value=0.4), ciw.dists.Deterministic(value=1.0)],
+            number_of_servers=[ciw.Schedule(numbers_of_servers=[1, 0, 1], shift_end_dates=[4.2, 6.1, 100], preemption="reroute"), 1],
+            routing=ciw.routing.NetworkRouting(routers=[Reroute(), ciw.routing.Leave()])
+        )
+        Q = ciw.Simulation(N)
+        Q.simulate_until_max_time(7.5)
+
+        recs = Q.get_all_records()
+        nd_1 = sorted([r for r in recs if r.node == 1], key=lambda r: r.arrival_date)
+        self.assertEqual([round(r.arrival_date, 5) for r in nd_1], [1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0])
+        self.assertEqual([round(r.service_time, 5) for r in nd_1], [0.4, 0.4, 0.4, 0.4, 0.4, 0.4, 0.4])
+        self.assertEqual([round(r.exit_date, 5) for r in nd_1], [1.4, 2.4, 3.4, 4.2, 6.5, 6.9, 7.4])
+        self.assertEqual([r.destination for r in nd_1], [-1, -1, -1, 2, -1, -1, -1])
+        self.assertEqual([r.record_type for r in nd_1], ['service', 'service', 'service', 'interrupted service', 'service', 'service', 'service'])
+
+        nd_2 = sorted([r for r in recs if r.node == 2], key=lambda r: r.arrival_date)
+        self.assertEqual([round(r.arrival_date, 5) for r in nd_2], [4.2])
+        self.assertEqual([round(r.service_time, 5) for r in nd_2], [1.0])
+        self.assertEqual([round(r.exit_date, 5) for r in nd_2], [5.2])
+        self.assertEqual([r.destination for r in nd_2], [-1])
+        self.assertEqual([r.record_type for r in nd_2], ['service'])
+
 
 class TestServiceDisciplines(unittest.TestCase):
     def test_first_in_first_out(self):
         N = ciw.create_network(
             arrival_distributions=[ciw.dists.Deterministic(1)],
             service_distributions=[ciw.dists.Deterministic(1.5)],
             service_disciplines=[ciw.disciplines.FIFO],
@@ -1322,7 +1690,8 @@
         recs = Q.get_all_records()
         adult_waits = [r.waiting_time for r in recs if r.customer_class=='Adult']
         child_waits = [r.waiting_time for r in recs if r.customer_class=='Child']
         mean_adult_wait = sum(adult_waits) / len(adult_waits)
         mean_child_wait = sum(child_waits) / len(child_waits)
         self.assertEqual(round(mean_adult_wait, 8), 0.00301455)
         self.assertEqual(round(mean_child_wait, 8), 0.00208601)
+
```

### Comparing `Ciw-3.1.4/ciw/tests/test_state_tracker.py` & `ciw-3.2.0/ciw/tests/test_state_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1918,7 +1918,97 @@
         self.assertEqual(
             Q.statetracker.state,
             [[0, 0, 0],
              [0, 0, 0],
              [0, 0, 1],
              [0, 0, 0]]
         )
+
+class TestGroupedNodePopulation(unittest.TestCase):
+    def test_groupednodepop_init_method(self):
+        Q = ciw.Simulation(N_params)
+        B = ciw.trackers.GroupedNodePopulation(groups=[[0, 2, 3], [1]])
+        B.initialise(Q)
+        self.assertEqual(B.simulation, Q)
+        self.assertEqual(B.state, [0, 0])
+
+    def test_groupednodepop_change_state_accept_method(self):
+        Q = ciw.Simulation(N_params)
+        B = ciw.trackers.GroupedNodePopulation(groups=[[0, 2, 3], [1]])
+        B.initialise(Q)
+        N = Q.nodes[1]
+        ind = ciw.Individual(1)
+        self.assertEqual(B.state, [0, 0])
+        B.change_state_accept(N, ind)
+        self.assertEqual(B.state, [1, 0])
+
+    def test_groupednodepop_change_state_block_method(self):
+        Q = ciw.Simulation(N_params)
+        B = ciw.trackers.GroupedNodePopulation(groups=[[0, 2, 3], [1]])
+        B.initialise(Q)
+        N1 = Q.nodes[1]
+        N2 = Q.nodes[2]
+        ind = ciw.Individual(1)
+        B.state = [1, 0]
+        B.change_state_block(N1, N2, ind)
+        self.assertEqual(B.state, [1, 0])
+
+    def test_groupednodepop_change_state_release_method(self):
+        Q = ciw.Simulation(N_params)
+        B = ciw.trackers.GroupedNodePopulation(groups=[[0, 2, 3], [1]])
+        B.initialise(Q)
+        N = Q.nodes[1]
+        N2 = Q.nodes[2]
+        Nex = Q.nodes[-1]
+        ind1 = ciw.Individual(1)
+        ind2 = ciw.Individual(2)
+        ind3 = ciw.Individual(3)
+        B.state = [12, 3]
+        B.change_state_release(N, Nex, ind1, False)
+        self.assertEqual(B.state, [11, 3])
+        B.change_state_release(N, Nex, ind2, True)
+        self.assertEqual(B.state, [10, 3])
+        B.change_state_release(N2, Nex, ind3, True)
+        self.assertEqual(B.state, [10, 2])
+
+    def test_groupednodepop_hash_state_method(self):
+        Q = ciw.Simulation(N_params)
+        B = ciw.trackers.GroupedNodePopulation(groups=[[0, 2, 3], [1]])
+        B.initialise(Q)
+        B.state = [7, 3]
+        self.assertEqual(B.hash_state(), (7, 3))
+
+    def test_groupednodepop_release_method_within_simulation(self):
+        Q = ciw.Simulation(N_params, tracker=ciw.trackers.GroupedNodePopulation(groups=[[0, 2, 3], [1]]))
+        N = Q.transitive_nodes[2]
+        inds = [ciw.Individual(i, 'Class 0') for i in range(5)]
+        N.individuals = [inds]
+        for ind in N.individuals[0]:
+            srvr = N.find_free_server(ind)
+            N.attach_server(srvr, ind)
+        Q.statetracker.state = [11, 3]
+        self.assertEqual(Q.statetracker.state, [11, 3])
+        Q.current_time = 43.11
+        N.release(N.all_individuals[0], Q.nodes[1])
+        self.assertEqual(Q.statetracker.state, [11, 3])
+        N.all_individuals[1].is_blocked = True
+        Q.current_time = 46.72
+        N.release(N.all_individuals[1], Q.nodes[1])
+        self.assertEqual(Q.statetracker.state, [11, 3])
+        N.release(N.all_individuals[1], Q.nodes[-1])
+        self.assertEqual(Q.statetracker.state, [10, 3])
+
+    def test_groupednodepop_block_method_within_simulation(self):
+        Q = ciw.Simulation(N_params, tracker=ciw.trackers.GroupedNodePopulation(groups=[[0, 2, 3], [1]]))
+        N = Q.transitive_nodes[2]
+        Q.statetracker.state = [11, 3]
+        self.assertEqual(Q.statetracker.state, [11, 3])
+        N.block_individual(ciw.Individual(1), Q.nodes[1])
+        self.assertEqual(Q.statetracker.state, [11, 3])
+
+    def test_groupednodepop_accept_method_within_simulation(self):
+        Q = ciw.Simulation(N_params, tracker=ciw.trackers.GroupedNodePopulation(groups=[[0, 2, 3], [1]]))
+        N = Q.transitive_nodes[2]
+        self.assertEqual(Q.statetracker.state, [0, 0])
+        Q.current_time = 45.6
+        N.accept(ciw.Individual(3, 'Class 2'))
+        self.assertEqual(Q.statetracker.state, [1, 0])
```

### Comparing `Ciw-3.1.4/ciw/trackers/state_tracker.py` & `ciw-3.2.0/ciw/trackers/state_tracker.py`

 * *Files 11% similar despite different names*

```diff
@@ -238,14 +238,71 @@
     def hash_state(self):
         """
         Returns a hashable state.
         """
         return tuple(self.state)
 
 
+class GroupedNodePopulation(StateTracker):
+    """
+    The node population tracker records the number of customers at each group
+    of nodes, where node groups are defined by the user.
+
+    Example:
+        (3, 1)
+        This denotes 3 customers at the first node group, and 1 customer at the
+        second node group.
+    """
+
+    def __init__(self, groups):
+        """
+        Pre-initialises the object with keyword `observed_nodes`
+        """
+        self.groups = groups
+        self.observed_nodes = [nd for group in groups for nd in group] 
+
+    def initialise(self, simulation):
+        """
+        Initialises the state tracker class.
+        """
+        self.simulation = simulation
+        self.state = [0 for i in self.groups]
+        self.history = [[self.simulation.current_time, self.hash_state()]]
+
+    def change_state_accept(self, node, ind):
+        """
+        Changes the state of the system when a customer is accepted.
+        """
+        if node.id_number - 1 in self.observed_nodes:
+            node_in_group = [(node.id_number - 1) in group for group in self.groups]
+            group_index = node_in_group.index(True)
+            self.state[group_index] += 1
+
+    def change_state_block(self, node, destination, ind):
+        """
+        Changes the state of the system when a customer gets blocked.
+        """
+        pass
+
+    def change_state_release(self, node, destination, ind, blocked):
+        """
+        Changes the state of the system when a customer is released.
+        """
+        if node.id_number - 1 in self.observed_nodes:
+            node_in_group = [(node.id_number - 1) in group for group in self.groups]
+            group_index = node_in_group.index(True)
+            self.state[group_index] -= 1
+
+    def hash_state(self):
+        """
+        Returns a hashable state.
+        """
+        return tuple(self.state)
+
+
 class NodeClassMatrix(StateTracker):
     """
     The node-class matrix tracker records the number of customers of each
     class at each node.
 
     Example:
         ((3, 1),
```

### Comparing `Ciw-3.1.4/docs/Background/kendall.rst` & `ciw-3.2.0/docs/Background/kendall.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Background/mechanisms.rst` & `ciw-3.2.0/docs/Background/mechanisms.rst`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 =========================
 Notes on Ciw's Mechanisms
 =========================
 
 General
 ~~~~~~~
 
-Ciw uses the *event scheduling* approach [SW14]_ , similar to the three phase approach.
+Ciw uses the *event scheduling* approach [SR14]_ , similar to the three phase approach.
 In the event scheduling approach, three types of event take place: **A Events** move the clock forward, **B Events** are prescheduled events, and **C Events** are events that arise because a **B Event** has happened.
 
 Here **A-events** correspond to moving the clock forward to the next **B-event**.
 **B-events** correspond to either an external arrival, a customer finishing service, or a server shift change.
 **C-events** correspond to a customer starting service, customer being released from a node, and being blocked or unblocked.
 
 In event scheduling the following process occurs:
@@ -20,31 +20,14 @@
 2. **A Phase**: move the clock to the next scheduled event
 3. Take a **B Event** scheduled for now, carry out the event
 4. Carry out all **C Events** that arose due to the event carried out in (3.)
 5. Repeat (3.) - (4.) until all **B Event** scheduled for that date have been carried out
 6. Repeat (2.) - (5.) until a terminating criteria has been satisfied
 
 
-Blocking Mechanism
-~~~~~~~~~~~~~~~~~~
-
-In Ciw, Type I blocking (blocking after service) is implemented for restricted networks.
-
-After service, a customer's next destination is sampled from the transition matrix.
-If there is space at the destination node, that customer will join the queue there.
-Else if the destination node's queueing capacity is full, then that customer will be blocked.
-That customer remains at that node, with its server, until space becomes available at the destination.
-This means the server that was serving that customer remains attached to that customer, being unable to serve anyone else until that customer is unblocked.
-
-At the time of blockage, information about this customer is added to the destination node's :code:`blocked_queue`, a virtual queue containing information about all the customers blocked to that node, and *the order in which they became blocked*.
-Thus, the sequence of unblockages happen in the order which customers were blocked.
-
-Circular blockages can lead to :ref:`deadlock <detect-deadlock>`.
-
-
 
 .. _simultaneous_events:
 
 Simultaneous Events
 ~~~~~~~~~~~~~~~~~~~
 
 In discrete event simulation, simultaneous event are inevitable.
```

### Comparing `Ciw-3.1.4/docs/Background/other.rst` & `ciw-3.2.0/docs/Background/other.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Background/references.rst` & `ciw-3.2.0/docs/Background/references.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .. _bibliography-page:
 
 ============
 Bibliography
 ============
 
-.. [SW14] S. Robinson. *Simulation: the practice of model development and use.* Palgrave Macmillan, 2014.
+.. [SR14] S. Robinson. *Simulation: the practice of model development and use.* Palgrave Macmillan, 2014.
 .. [WS09] W. Stewart. *Probability, markov chains, queues, and simulation.* Princeton university press, 2009.
+.. [JJ57] J. Jackson. *Networks of Waiting Lines.* Operations Research, 1957.
 .. [JZ09] J. Zhang. G. Dai, and B. Zwart. *Law of large number limits of limited processor-sharing queues.* Mathematics of Operations Research 34.4, pp937-970, 2009.
 .. [XL09] X. Li. *Radio Access Network Dimensioning for 3G UMTS.* PhD Thesis, 2009.
 .. [GP21] G. Palmer and Y. Tian. *Implementing hybrid simulations that integrate DES+SD in Python.* Journal of Simulation, 2021.
```

### Comparing `Ciw-3.1.4/docs/Background/simulationpractice.rst` & `ciw-3.2.0/docs/Background/simulationpractice.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 .. _simulation-practice:
 
 ===================
 Simulation Practice
 ===================
 
 Ensuring good practice when simulation modelling is important to get meaningful analyses from the models.
-This is shown in :ref:`Tutorial IV <tutorial-iv>`.
-A recommended resource on the subject is [SW14]_.
+This is shown in :ref:`Part 4 of Tutorial I <tutorial-i-p4>`.
+A recommended resource on the subject is [SR14]_.
 This page will briefly summarise some important aspects of carrying out simulation model analysis.
 
 -------------------------------
 Performing Multiple Repetitions
 -------------------------------
 
 Users should not rely on the results of a single run of the simulation due to the intrinsic stochastic nature of simulation.
```

### Comparing `Ciw-3.1.4/docs/Guides/batching.rst` & `ciw-3.2.0/docs/Guides/Arrivals/batching.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Guides/baulking.rst` & `ciw-3.2.0/docs/Guides/CustomerBehaviour/baulking.rst`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,14 @@
 	>>> ciw.seed(0)
 	>>> Q = ciw.Simulation(N)
 	>>> Q.simulate_until_max_time(45.0)
 	>>> recs = Q.get_all_records()
 	>>> baulked_recs = [r for r in recs if r.record_type=="baulk"]
 	>>> r = baulked_recs[0]
 	>>> (r.id_number, r.customer_class, r.node, r.arrival_date)
-	(44, 'Class 0', 1, 9.45892050639243)
+	(44, 'Class 0', 1, 9.45892050639...)
 
 Note that baulking works and behaves differently to simply setting a queue capacity.
 Filling a queue's capacity results in arriving customers being *rejected* (and recorded as data records of type :code:`"rejection"`), and transitioning customers to be blocked.
 Baulking on the other hand does not effect transitioning customers.
 This means that if you set a deterministic baulking threshold of 5, but do not set a queue capacity, then the number of individuals at that node may exceed 5, due to customers transitioning from other nodes ignoring the baulking threshold.
 This also means you can use baulking and limited capacities in conjunction with one another.
```

### Comparing `Ciw-3.1.4/docs/Guides/behaviour/custom_arrivals.rst` & `ciw-3.2.0/docs/Guides/System/behaviour/custom_arrivals.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Guides/behaviour/custom_number_servers.rst` & `ciw-3.2.0/docs/Guides/System/behaviour/custom_number_servers.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 Now let's plot the system population over time::
 
     >>> plt.plot(
     ...     [row[0] for row in Q.statetracker.history],
     ...     [row[1] for row in Q.statetracker.history]
     ... ); # doctest:+SKIP
 
-.. image:: ../../_static/custom_number_servers_without.svg
+.. image:: ../../../_static/custom_number_servers_without.svg
    :alt: Plot of system population increasing over time.
    :align: center
 
 
 With desired behaviour
 ~~~~~~~~~~~~~~~~~~~~~~
 
@@ -66,13 +66,13 @@
 Now let's plot the system population over time::
 
     >>> plt.plot(
     ...     [row[0] for row in Q.statetracker.history],
     ...     [row[1] for row in Q.statetracker.history]
     ... ); # doctest:+SKIP
 
-.. image:: ../../_static/custom_number_servers_with.svg
+.. image:: ../../../_static/custom_number_servers_with.svg
    :alt: Plot of system population over time.
    :align: center
 
 We see the system population is now better under control.
 Furthermore, large changes in the system population tends occur at the times where servers were added and removed.
```

### Comparing `Ciw-3.1.4/docs/Guides/behaviour/custom_routing.rst` & `ciw-3.2.0/docs/Guides/CustomerClasses/customer-classes.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,71 @@
-State-dependent Routing
-=======================
+.. _customer-classes:
 
-In this example we will consider a network where customers are routed differently depending on the system state. We will look at a system without this behaviour first, and then the system with the desired behaviour, for comparison.
+=======================================
+How to Set Multiple Classes of Customer
+=======================================
 
+Ciw allows us to define different system parameters for different sets of customers sharing the same system infrastructure. These sets of customers are called different customers classes. This is defined by inserting dictionaries of parameters for the keywords in :code:`ciw.create_network`; these dictionaries will have keys of strings representing customer class names, and values corresponding to the parameters themselves.
 
-Without desired behaviour
-~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Consider the following three node network, where arrivals only occur at the first node, then customers are randomly routed to either the 2nd or 3rd node before leaving::
+For example, consider an M/M/3 queue::
 
     >>> import ciw
+    >>> N = ciw.create_network(
+    ...     arrival_distributions=[ciw.dists.Exponential(rate=5)],
+    ...     service_distributions=[ciw.dists.Exponential(rate=7)],
+    ...     number_of_servers=[2]
+    ... )
+
+Now imagine we had two different types of customer: 40% of customers are Adults, while 60% of customers are children. Children twice as long to process than adults, and so will have a different service time distribution. In this case, Children and Adults will also have different arrival distributions: remember that arrival distributions define the distribution of inter-arrival times, and the inter-arrival times are defined as the inter-arrival times between two customers of the same class.
+
+Hence we would get::
 
     >>> N = ciw.create_network(
-    ...     arrival_distributions=[
-    ...         ciw.dists.Exponential(rate=10),
-    ...         None,
-    ...         None],
-    ...     service_distributions=[
-    ...         ciw.dists.Exponential(rate=25),
-    ...         ciw.dists.Exponential(rate=6),
-    ...         ciw.dists.Exponential(rate=8)],
-    ...     routing=[[0.0, 0.5, 0.5],
-    ...              [0.0, 0.0, 0.0],
-    ...              [0.0, 0.0, 0.0]],
-    ...     number_of_servers=[1, 1, 1]
+    ...     arrival_distributions={
+    ...         "Adult": [ciw.dists.Exponential(rate=5 * 0.4)],
+    ...         "Child": [ciw.dists.Exponential(rate=5 * 0.6)]
+    ...     },
+    ...     service_distributions={
+    ...         "Adult": [ciw.dists.Exponential(rate=7)],
+    ...         "Child": [ciw.dists.Exponential(rate=3.5)]
+    ...     },
+    ...     number_of_servers=[2]
     ... )
 
-Now we run the system for 80 time units using a state tracker to track the number of customers at Node 1 and Node 2::
+The decomposition of the arrival rates is due to `thinning of Poisson processes <(https://galton.uchicago.edu/~lalley/Courses/312/PoissonProcesses.pdf>`_. However, in general, think of arrival distributions as the distribution of inter-arrival times between customers of the same class.
 
-    >>> ciw.seed(0)
-    >>> Q = ciw.Simulation(N, tracker=ciw.trackers.NodePopulation())
-    >>> Q.simulate_until_max_time(80)
-    
-    >>> ts = [ts[0] for ts in Q.statetracker.history]
-    >>> n2 = [ts[1][1] for ts in Q.statetracker.history]
-    >>> n3 = [ts[1][2] for ts in Q.statetracker.history]
-
-Plotting `n2` and `n3` we see that the numbers of customers at each node can diverge greatly::
-
-    >>> import matplotlib.pyplot as plt # doctest:+SKIP
-    >>> plt.plot(ts, n2); # doctest:+SKIP
-    >>> plt.plot(ts, n3); # doctest:+SKIP
-
-.. image:: ../../_static/custom_routing_without.svg
-   :alt: Plot of node populations diverging.
-   :align: center
-
-
-With desired behaviour
-~~~~~~~~~~~~~~~~~~~~~~
-
-We will now create a new :code:`CustomRouting` for Node 1, that will send its customers to the least busy of Nodes 2 and 3.
-First create the :code:`CustomRouting` that inherits from :code:`ciw.Node`, and overwrites the :code:`next_node` method::
-
-    >>> class CustomRouting(ciw.Node):
-    ...     """
-    ...     Chooses either Node 2 or Node 3 as the destination node,
-    ...     whichever has the least customers. Chooses randomly in
-    ...     the event of a tie.
-    ...     """
-    ...     def next_node(self, ind):
-    ...         n2 = self.simulation.nodes[2].number_of_individuals
-    ...         n3 = self.simulation.nodes[3].number_of_individuals
-    ...         if n2 < n3:
-    ...             return self.simulation.nodes[2]
-    ...         elif n3 < n2:
-    ...             return self.simulation.nodes[3]
-    ...         return ciw.random_choice([self.simulation.nodes[2], self.simulation.nodes[3]])
-
-Now rerun the same system, using the same network object :code:`N` (notice the transition matrix will be unused now).
-We tell Ciw which node class to use for each node of the network, by giving the :code:`node_class` argumument a list of classes.
-We'll use the new :code:`CustomRouting` class for Node 1, and the regular :code:`ciw.Node` class for Nodes 2 and 3::
+It is important that the keys of these parameter dictionaries are the same throughout. If splitting one keyword by customer class, then *all* keywords that can be split by customer class need to be split by customer class.
+
+When collecting results, the class of the customer associated with each service is also recorded::
 
     >>> ciw.seed(0)
-    >>> Q = ciw.Simulation(
-    ...     N, tracker=ciw.trackers.NodePopulation(),
-    ...     node_class=[CustomRouting, ciw.Node, ciw.Node])
-    >>> Q.simulate_until_max_time(80)
-    
-    >>> ts = [ts[0] for ts in Q.statetracker.history]
-    >>> n2 = [ts[1][1] for ts in Q.statetracker.history]
-    >>> n3 = [ts[1][2] for ts in Q.statetracker.history]
-
-Plotting `n2` and `n3` now, we see that the numbers of customers at each node can follow one another closely, as we are always 'evening out' the nodes' busyness by always filling up the least busy node::
-
-    >>> plt.plot(ts, n2); # doctest:+SKIP
-    >>> plt.plot(ts, n3); # doctest:+SKIP
-
-.. image:: ../../_static/custom_routing_with.svg
-   :alt: Plot of node populations closely following each other.
-   :align: center
+    >>> Q = ciw.Simulation(N)
+    >>> Q.simulate_until_max_time(50)
+    >>> recs = Q.get_all_records()
+    >>> recs[0].customer_class
+    'Child'
+
+    >>> from collections import Counter
+    >>> Counter([r.customer_class for r in recs])
+    Counter({'Child': 138, 'Adult': 89})
+
+Nearly all parameters of :code:`ciw.create_network` can be split by customer class, unless they describe the architecture of the network itself. Those that can and cannot be split by customer class are listed below:
+
+Can be split by customer class:
+    + :code:`arrival_distributions`,
+    + :code:`baulking_functions`,
+    + :code:`class_change_matrices`,
+    + :code:`class_change_time_distributions`,
+    + :code:`service_distributions`,
+    + :code:`routing`,
+    + :code:`batching_distributions`,
+    + :code:`reneging_time_distributions`,
+    + :code:`reneging_destinations`,
+
+Cannot be split by customer class:
+    + :code:`number_of_servers`,
+    + :code:`priority_classes`,
+    + :code:`queue_capacities`,
+    + :code:`ps_thresholds`,
+    + :code:`server_priority_functions`,
+    + :code:`service_disciplines`,
+    + :code:`system_capacity`
```

### Comparing `Ciw-3.1.4/docs/Guides/behaviour/hybrid.rst` & `ciw-3.2.0/docs/Guides/System/behaviour/hybrid.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 DES+SD Hybrid Simulation with Ciw
 =================================
 
 In the paper [GP21]_ a DES+SD hybrid simulation is defined using Ciw and Scipy. This is achieved by defining new :code:`Simulation` and :code:`Node` objects that solve a set of differential equations that update parameters of the DES continuously. We give an example here.
 
 Consider a supermarket modelled as an :math:`M/M/k` queue, whose customers are living in an SIMD disease model. This is show below:
 
-.. image:: ../../_static/hybrid.png
+.. image:: ../../../_static/hybrid.png
    :alt: Stock and Flow / Queueing diagram of the hybrid system.
    :align: center
 
 Here:
 
 + :math:`S` is the number of people in the population susceptible to the disease,
 + :math:`I` is the number of people in the population infected with the disease,
@@ -154,10 +154,10 @@
         results['I'] = Q.SD.I
         results['M'] = Q.SD.M
         results['D'] = Q.SD.D
         return results
 
 Running these for one trial only (this is bad practice, :ref:`see here <simulation-practice>`), we can plot the stock levels over time. We see that changing the number of servers from :math:`k = 1` to :math:`k = 3`, a parameter associated with the discrete component, changes the stock levels, results associated with the continuous component.
 
-.. image:: ../../_static/des+sd_hybrid.svg
+.. image:: ../../../_static/des+sd_hybrid.svg
    :alt: Stock level plots of the hybrid simulation results.
    :align: center
```

### Comparing `Ciw-3.1.4/docs/Guides/behaviour/index.rst` & `ciw-3.2.0/docs/Guides/System/behaviour/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -21,13 +21,11 @@
 -------------------
 
 Here's a library of examples of this functionality:
 
 .. toctree::
    :maxdepth: 1
    
-   custom_routing.rst
    custom_arrivals.rst
    custom_number_servers.rst
-   ps_routing.rst
    server_dependent_dist.rst
    hybrid.rst
```

### Comparing `Ciw-3.1.4/docs/Guides/behaviour/ps_routing.rst` & `ciw-3.2.0/docs/Tutorial/GettingStarted/part_3.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,88 @@
-.. _ps-routing:
+.. _tutorial-i-p3:
 
-================================================
-Join Shortest Queue in Processor Sharing Systems
-================================================
+=======================================
+Tutorial I: Part 3 - Collecting Results
+=======================================
 
-In this example we will consider multiple parallel processor sharing queues, where customers are routed to the least busy node. This is calles a Join Shortest Queue, or JSQ system.
-
-Consider three independent parallel processor sharing nodes. Customers arrive and are sent to the least busy node.
-This can be modelled as a 4 node system: the first node is a dummy node where customers arrive, and routes the customer to one of the thee remaining processor sharing nodes.
-If the arrival distribution is Poisson with rate 8, and required service times are exponentially distributed with parameter 10, then our network is::
+In the previous parts, we defined and simulated our bank for a week, and saw how to access parts of the simulation engine::
 
     >>> import ciw
     >>> N = ciw.create_network(
-    ...     arrival_distributions=[ciw.dists.Exponential(rate=8),
-    ...                            None,
-    ...                            None,
-    ...                            None],
-    ...     service_distributions=[ciw.dists.Deterministic(value=0),
-    ...                            ciw.dists.Exponential(rate=10),
-    ...                            ciw.dists.Exponential(rate=10),
-    ...                            ciw.dists.Exponential(rate=10)],
-    ...     number_of_servers=[float('inf'),
-    ...                        float('inf'),
-    ...                        float('inf'),
-    ...                        float('inf')],
-    ...     routing=[[0, 0, 0, 0],
-    ...              [0, 0, 0, 0],
-    ...              [0, 0, 0, 0],
-    ...              [0, 0, 0, 0]]
+    ...     arrival_distributions=[ciw.dists.Exponential(rate=0.2)],
+    ...     service_distributions=[ciw.dists.Exponential(rate=0.1)],
+    ...     number_of_servers=[3]
     ... )
+    >>> ciw.seed(1)
+    >>> Q = ciw.Simulation(N)
+    >>> Q.simulate_until_max_time(1440)
+
+We can quickly get a list of all data records collected by all customers have have finished at least one service, using the :code:`get_all_records` method of the Simulation object::
+
+    >>> recs = Q.get_all_records()
+
+This returns a list of named tuples. Each named tuple contains the following information:
+
+    - :code:`id_number`
+    - :code:`customer_class`
+    - :code:`node`
+    - :code:`arrival_date`
+    - :code:`waiting_time`
+    - :code:`service_start_date`
+    - :code:`service_time`
+    - :code:`service_end_date`
+    - :code:`time_blocked`
+    - :code:`exit_date`
+    - :code:`destination`
+    - :code:`queue_size_at_arrival`
+    - :code:`queue_size_at_departure`
+    - :code:`server_id`
+    - :code:`record_type`
+
+More information on each of these is given in :ref:`refs-results`.
+
+Using a list comprehension, we can get lists on whichever statistic we like::
+
+    >>> # A list of service times
+    >>> servicetimes = [r.service_time for r in recs]
+    >>> servicetimes
+    [2.94463..., 5.96912..., 18.80156..., ..., 33.18376...]
+
+    >>> # A list of waits
+    >>> waits = [r.waiting_time for r in recs]
+    >>> waits
+    [0.0, 0.0, 0.0, 0.20439..., ..., 0.0]
+
+Now we can get summary statistics simply by manipulating these lists::
+
+    >>> mean_service_time = sum(servicetimes) / len(servicetimes)
+    >>> mean_service_time
+    10.647482...
+
+    >>> mean_waiting_time = sum(waits) / len(waits)
+    >>> mean_waiting_time
+    4.230543...
+
+We now know the mean waiting time of the customers!
+In next part we will show how to get more representative results (as we have only simulated one given day here).
+
+Further summary statistics can be obtained using external libraries.
+We recommend `numpy <http://www.numpy.org/>`_, `pandas <http://pandas.pydata.org/>`_ and `matplotlib <http://matplotlib.org/>`_. 
+Using these further statistics and plots can be explored.
+The histogram of waits below was created using matplotlib, using the following code::
+
+    >>> import matplotlib.pyplot as plt # doctest:+SKIP
+    >>> plt.hist(waits); # doctest:+SKIP
+
+.. image:: ../../_static/tutorial_iii_waitshist.svg
+   :alt: Histogram of waits for Tutorial III.
+   :align: center
+
+If we'd like to see how busy or idle the servers have been throughout the simulation run, we can look at the :code:`server_utilisation` of a Node.
+This is the average utilisation of each server, which is the amount of time a server was busy (with a customer), divided by the total amount of time the server was on duty::
+
+    >>> Q.transitive_nodes[0].server_utilisation
+    0.75288...
+
+Thus in our bank, on average the servers were busy 75.3% of the time.
 
-For each of the three parallel processor sharing nodes, we can use the :code:`ciw.PSNode` class.
-However, we now need a custom node class for the initial dummy node, to take care of the routing decisions.
-We'll call this class :code:`RoutingDecision`::
-
-    >>> class RoutingDecision(ciw.Node):
-    ...     def next_node(self, ind):
-    ...         """
-    ...         Finds the next node by looking at nodes 2, 3, and 4,
-    ...         seeing how busy they are, and routing to the least busy.
-    ...         """
-    ...         busyness = {n: self.simulation.nodes[n].number_of_individuals for n in [2, 3, 4]}
-    ...         chosen_n = sorted(busyness.keys(), key=lambda x: busyness[x])[0]
-    ...         return self.simulation.nodes[chosen_n]
-
-Now let's build a simulation object, where the first node uses our custom :code:`RoutingDecision` class, and the others use the built-in :code:`ciw.PSNode` class. We'll also add a state tracker for analysis::
-
-    >>> ciw.seed(0)
-    >>> Q = ciw.Simulation(
-    ...     N, tracker=ciw.trackers.SystemPopulation(),
-    ...     node_class=[RoutingDecision, ciw.PSNode, ciw.PSNode, ciw.PSNode])
-
-We'll run this for 100 time units::
-
-    >>> Q.simulate_until_max_time(100)
-
-We can look at the state probabilities, that is, the proportion of time the system spent in each state, where a state represents the number of customers present in the system::
-
-    >>> Q.statetracker.state_probabilities(observation_period=(10, 90)) # doctest:+SKIP
-    {0: 0.425095024227593,
-     1: 0.35989517302304014,
-     2: 0.14629711075255158,
-     3: 0.054182634504608064,
-     4: 0.01124224242623659,
-     5: 0.002061285633093934,
-     6: 0.0012265294328765105}
+The next part will show how to use Ciw to get trustworthy results, and finally find out the average waiting time at the bank.
```

### Comparing `Ciw-3.1.4/docs/Guides/behaviour/server_dependent_dist.rst` & `ciw-3.2.0/docs/Guides/System/behaviour/server_dependent_dist.rst`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     >>> for s in Q.nodes[1].servers:
     ...     plt.plot(
     ...         [0] + [t for t in s.served_inds],
     ...         [0] + [i + 1 for i, t in enumerate(s.served_inds)],
     ...     label=f"Server {s.id_number}") # doctest:+SKIP
     >>>     plt.legend() # doctest:+SKIP
 
-.. image:: ../../_static/server_dependent_dist_without.svg
+.. image:: ../../../_static/server_dependent_dist_without.svg
    :alt: Plot server commission over time, all with the same behaviour.
    :align: center
 
 
 With desired behaviour
 ~~~~~~~~~~~~~~~~~~~~~~
 
@@ -90,13 +90,13 @@
     >>> for s in Q.nodes[1].servers:
     ...     plt.plot(
     ...         [0] + [t for t in s.served_inds],
     ...         [0] + [i + 1 for i, t in enumerate(s.served_inds)],
     ...     label=f"Server {s.id_number}") # doctest:+SKIP
     >>>     plt.legend() # doctest:+SKIP
 
-.. image:: ../../_static/server_dependent_dist_with.svg
+.. image:: ../../../_static/server_dependent_dist_with.svg
    :alt: Plot server commission over time, all with the different behaviour.
    :align: center
 
 We now see that each of the servers has a different rate at which they gain commission.
```

### Comparing `Ciw-3.1.4/docs/Guides/change-class-after-service.rst` & `ciw-3.2.0/docs/Guides/CustomerClasses/change-class-after-service.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Guides/change-class-while-queueing.rst` & `ciw-3.2.0/docs/Guides/CustomerClasses/change-class-while-queueing.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Guides/deadlock.rst` & `ciw-3.2.0/docs/Guides/System/deadlock.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 How to Detect Deadlock
 ======================
 
 Deadlock is the phenomenon whereby all movement and customer flow in a restricted queueing network ceases, due to circular blocking.
 The diagram below shows an example, where the customer at the top node is blocked to the bottom node, and the customer at the bottom node is blocked to the top node.
 This circular blockage results is no more natural movement happening.
 
-.. image:: ../_static/2nodesindeadlock.svg
+.. image:: ../../_static/2nodesindeadlock.svg
    :alt: A 2 node queueing network in deadlock.
    :align: center
 
 Ciw's has built in deadlock detection capability.
 With Ciw, a queueing network can be simulated until it reaches deadlock.
 Ciw then records the time until deadlock from each state.
 (Please see the documentation on :ref:`state trackers <state-trackers>`.)
```

### Comparing `Ciw-3.1.4/docs/Guides/exact.rst` & `ciw-3.2.0/docs/Guides/Simulation/exact.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Guides/parallel_process.rst` & `ciw-3.2.0/docs/Guides/Simulation/parallel_process.rst`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,18 @@
     >>> mean_waits = [get_mean_wait(network=N, max_time=max_time, seed=seed) for seed in range(repetitions)]
     >>> sum(mean_waits) / repetitions
     3.762233...
 
 To obtain the above by running 2 simulations at the same time (assuming that 2
 cores are available), the :code:`multiprocessing` library can be used. In which
 case the following :download:`main.py
-<../_static/script_for_parallel_processing/main.py>` script gives a working
+<../../_static/script_for_parallel_processing/main.py>` script gives a working
 example:
 
-.. literalinclude:: ../_static/script_for_parallel_processing/main.py
+.. literalinclude:: ../../_static/script_for_parallel_processing/main.py
 
 It is possible to use :code:`multiprocessing.cpu_count()` to obtain the number
 of available cores.
 
 Note that the conditional :code:`if __name__ == '__main__':` is needed to ensure
 that :code:`get_mean_wait` can be pickled. This is necessary to ensure that it
 can be used by the parallel processing pool.
```

### Comparing `Ciw-3.1.4/docs/Guides/pause_restart.rst` & `ciw-3.2.0/docs/Guides/Simulation/pause_restart.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Guides/phasetype.rst` & `ciw-3.2.0/docs/Guides/Distributions/phasetype.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 One particular subset of distributions offered by Ciw is Phase-Type distributions.
 These are very useful and versatile family of distributions defined by absorbing Markov chains.
 That is, given a probability vector :math:`\alpha` representing the probability of the starting state, and an transition rate matrix :math:`M` of an absorbing Markov chain, these are distributions given by the time to absorption.
 It is therefore a random sum of exponential variables.
 
 The diagram below gives a general representation of an absorbing Markov chain with four states, 1, 2, 3, and the absorbing state :math:`\star`:
 
-.. image:: ../_static/phasetype.svg
+.. image:: ../../_static/phasetype.svg
    :width: 100%
    :alt: Absorbing Markov chain of a general Phase-Type distribution.
    :align: center
 
 The corresponding Phase-Type distribution would be defined by an initial state probability vector:
 
 .. math::
@@ -48,15 +48,15 @@
 Some Phase-Type distributions that have particular structures to their underlying absorbing Markov chain can be particularly useful, and Ciw offers helper classes for some of these to build the transition matrix for you. They are outlined below.
 
 Erlang Distributions
 --------------------
 
 An Erlang distribution with parameters :math:`\lambda` and :math:`n` is the sum of :math:`n` Exponential distributions with parameter :math:`\lambda`. This can be equivalently defined as the Phase-Type distribution with the following structure:
 
-.. image:: ../_static/erlang.svg
+.. image:: ../../_static/erlang.svg
    :width: 100%
    :alt: Absorbing Markov chain of an Erlang distribution.
    :align: center
 
 The corresponding Phase-Type distribution would be defined by an initial state probability vector:
 
 .. math::
@@ -80,15 +80,15 @@
 
 
 HyperExponential Distributions
 ------------------------------
 
 An HyperExponential distribution is defined by a probability vector :math:`\mathbf{p}` and rate vector :math:`\mathbf{\lambda}`, and samples an Exponential distribution with parameter :math:`\lambda_i` with probability :math:`p_i`. This can be equivalently defined as the Phase-Type distribution with the following structure:
 
-.. image:: ../_static/hyperexponential.svg
+.. image:: ../../_static/hyperexponential.svg
    :width: 100%
    :alt: Absorbing Markov chain of a HyperExponential distribution.
    :align: center
 
 When :math:`\mathbf{p} = \left(p_1, p_2, \dots, p_n\right)` and :math:`\mathbf{\lambda} = \left(\lambda_1, \lambda_2, \dots, \lambda_n\right)` the corresponding Phase-Type distribution would be defined by an initial state probability vector:
 
 .. math::
@@ -113,15 +113,15 @@
 
 HyperErlang Distributions
 -------------------------
 
 A HyperErlang distribution is defined by parameters :math:`\mathbf{\lambda}`, :math:`\mathbf{p}`, and :math:`\mathbf{n}`, and samples an Erlang distribution of size :math:`n_i` with parameter :math:`\lambda_i` with probability :math:`p_i`. This can be equivalently defined as the Phase-Type distribution with the following structure:
 
 
-.. image:: ../_static/hypererlang.svg
+.. image:: ../../_static/hypererlang.svg
    :width: 100%
    :alt: Absorbing Markov chain of a HyperErlang distribution.
    :align: center
 
 When :math:`\mathbf{p} = \left(0.5, 0.25, 0.25\right)`, :math:`\mathbf{\lambda} = \left(5, 2, 3\right)`, and :math:`\mathbf{n} = \left(2, 1, 2\right)` the corresponding Phase-Type distribution would be defined by an initial state probability vector:
 
 .. math::
@@ -146,15 +146,15 @@
 
 Coxian Distributions
 --------------------
 
 A Coxian distribution is defined by parameters :math:`\mathbf{\lambda}`, the rates of each phase, and :math:`\mathbf{p}`, the probability of going to the absorbing state after each phase. This can be equivalently defined as the Phase-Type distribution with the following structure:
 
 
-.. image:: ../_static/coxian.svg
+.. image:: ../../_static/coxian.svg
    :width: 100%
    :alt: Absorbing Markov chain of a general Coxian distribution.
    :align: center
 
 When :math:`\mathbf{p} = \left(p_1, p_2, \dots, p_n\right)` and :math:`\mathbf{\lambda} = \left(\lambda_1, \lambda_2, \dots, \lambda_n\right)` the corresponding Phase-Type distribution would be defined by an initial state probability vector:
```

### Comparing `Ciw-3.1.4/docs/Guides/priority.rst` & `ciw-3.2.0/docs/Guides/CustomerClasses/priority.rst`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,7 @@
 Pre-emption
 -----------
 
 There are a number of options that can be used to pre-emptively replace lower priority customers from service. See the following page:
 
 + :ref:`Pre-emption options <preemption>`.
 
-.. toctree::
-   :maxdepth: 1
-   :hidden:
-
-   preemption.rst
-
-
```

### Comparing `Ciw-3.1.4/docs/Guides/process_based.rst` & `ciw-3.2.0/docs/Guides/Routing/routing_objects.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,101 +1,83 @@
-.. _process-based:
+.. _routing-objects:
 
-===================================
-How to Define Process-Based Routing
-===================================
+==========================
+How to Use Routing Objects
+==========================
 
-Ciw has the capability to run simulations with process-based routing. This means a customer's entire route is determined at the start and not determined probablistically as they progress through the network.
-This allows routes to account for an individuals history, for example, repeating nodes a certain number of times.
+Routing objects in Ciw are objects that determine what an individual's next node will be. There are two types:
 
-A customer's entire route is determined at the start, generated from a routing function, that takes in an individual and returns a route, which is a list of the order of the nodes. For example::
++ **Network routing objects**: these determine routing for the entire network;
++ **Node routing objects**: these determine routing from a particular node.
 
-    >>> def routing_function(ind):
-    ...     return [1, 2, 2, 1]
+Ciw has a number of these built in, however their primary use is to be defined by the user. Examples of Network routing objects are:
 
-This takes in an individual at Node 1 and assigns it the route [1, 2, 2, 1]. Then after service at Node 1 the individual is sent to Node 2, then back Node 2, then back to Node 1, before exiting the system. Ensuring the exact repetition of these nodes would not be possible in a purely probabilistic system. 
++ :code:`ciw.routing.TransitionMatrix`, allowing users to define :ref:`transition matrices<transition-matrix>`, that is a matrix of probabilities of being transferred to each node in the network after service at every other node.
++ :code:`ciw.routing.ProcessBased`, allowing pre-defined routes to be given to individuals when they arrive, that is :ref:`process-based routing<process-based>`.
 
-In order to utilise this, we replace the routing matrix with a list of these routing functions to be used at each starting point. For example::
+However, the most flexible Network routing object is the generic :code:`ciw.routing.NetworkRouting`. This takes in a list of Node routing objects. Node routing objects are objects that determine routing out of a particular node. A :ref:`full list is given<refs-routing>` in the References section. The following are some of the most basic built-in routers available in Ciw, but importantly, they can also be user defined:
 
-    >>> import ciw
-    
-    >>> def repeating_route(ind):
-    ...     return [1, 1, 1]
-
-    >>> N = ciw.create_network(
-    ...     arrival_distributions=[ciw.dists.Exponential(rate=1)],
-    ...     service_distributions=[ciw.dists.Exponential(rate=2)],
-    ...     number_of_servers=[1], 
-    ...     routing=[repeating_route]
-    ... )
-
-Here, customers arrive at Node 1, and have service there and then repeat this two more times before exiting the system. 
-
-Let's run this and look at the routes of those that have left the system. 
-
-    >>> ciw.seed(0)
-    >>> Q = ciw.Simulation(N)
-    >>> Q.simulate_until_max_time(100.0)
-
-    >>> inds = Q.nodes[-1].all_individuals # Get's all individuals from exit node
-    >>> set([tuple(dr.node for dr in ind.data_records) for ind in inds]) # Get's all unique routes of completed individuals
-    {(1, 1, 1)}
-
-Now we can see that all individuals who have left the system, that is they have completed their route, repeated service at Node 1 three times. 
-        
-Important Notice
-----------------
-
-**How it works:** You can think of this as, when an individual arrives at their first node, based on their :code:`arrival_distributions`, it is assigned a route that should start at this Node. This will ensure that the first Node which an individual arrives at is the same as the first Node in their assigned route. 
++ :code:`ciw.routing.Direct(to=2)`: Sends the individual directly to another node. For example here, a customer is always send to node 2.
++ :code:`ciw.routing.Leave()`: The individual leaves the system.
++ :code:`ciw.routing.Probabilistic(destinations=[1, 3], probs=[0.1, 0.4])`: Probabilistically sends the individual to either of the destination, according to their corresponding probabilities. In this case, they are send to node 1 with probability 0.1, node 3 with probability 0.4, and leave the system with the rest of the probability, 0.5.
 
-If this is not the case then the error :code:`'Individual process route sent to wrong node'` will occur. 
 
-*Make sure that the routing function for Node* :math:`i` *yields routes that begin with Node* :math:`i`.
+Example
+~~~~~~~
 
-Further example
----------------
+Consider a four node system:
+  + At the node 1 customers are send directly to node 2;
+  + At node 2 customers can be send to either nodes 1, 3 or 4 with probabilities 0.1, 0.5, and 0.4;
+  + At node 3 customers can either repeat service there with probability 0.25, or leave the system;
+  + At node 4, all customers leave the system.
 
-The routing functions can be as complicated as necessary. They take in an individual, and therefore can take in any attribute of an individual when determining the route (including their :code:`customer_class`).
+We can construct a network routing object for this by choosing a set of node routing obejects from the list above. We place them in a list and use the :code:`routers` keyword to create the network object. In this case, the network object would be::
 
-Lets make a network with three nodes with the following routes:
-
-* For customers arriving at Node 1:
+    >>> import ciw
+    >>> R = ciw.routing.NetworkRouting(
+    ...     routers=[
+    ...         ciw.routing.Direct(to=2),
+    ...         ciw.routing.Probabilistic(destinations=[1, 3, 4], probs=[0.1, 0.5, 0.4]),
+    ...         ciw.routing.Probabilistic(destinations=[3], probs=[0.25]),
+    ...         ciw.routing.Leave()
+    ...     ]
+    ... )
 
-  * if individual has an even :code:`id_number`, repeat Node 1 twice, then exit.
+This network object can then be used to create a network::
 
-  * otherwise route from Node 1 to Node 2, to Node 3, and then exit.
-  
-* Arrivals at Node 2:
+    >>> N = ciw.create_network(
+    ...     arrival_distributions=[ciw.dists.Exponential(rate=1), ciw.dists.Exponential(rate=1), ciw.dists.Exponential(rate=1), ciw.dists.Exponential(rate=1)],
+    ...     service_distributions=[ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2), ciw.dists.Exponential(rate=2)],
+    ...     number_of_servers=[1, 2, 3, 1],
+    ...     routing=R
+    ... )
 
-  * have 50% chance of routing to Node 3, and then exit.
 
-  * have 50% chance of routing to Node 1, and then exit.
+Notes
+~~~~~
 
-* There are no arrivals at Node 3.
++ Note that a the :code:`routing` keywork when creating a network object requires a network routing object, *not* a node routing object. This is true even when there is only one node in the network.
++ Note also that, similar to the use of most other keywords when creating a network object, that routing can be customer class dependent.
 
-For this we will require two routing functions: :code:`routing_function_Node_1`, :code:`routing_function_Node_2`::
+For example, a one node network with two customer classes, both classes having different routing::
 
-    >>> def routing_function_Node_1(ind):
-    ...     if ind.id_number % 2 == 0:
-    ...         return [1, 1, 1]
-    ...     return [1, 2, 3]
+    >>> N = ciw.create_network(
+    ...     arrival_distributions={
+    ...         "Class 0": [ciw.dists.Exponential(rate=1)],
+    ...         "Class 1": [ciw.dists.Exponential(rate=3)]
+    ...     },
+    ...     service_distributions={
+    ...         "Class 0": [ciw.dists.Exponential(rate=2)],
+    ...         "Class 1": [ciw.dists.Exponential(rate=2)]
+    ...     },
+    ...     number_of_servers=[2],
+    ...     routing={
+    ...         "Class 0": ciw.routing.NetworkRouting(routers=[ciw.routing.Leave()]),
+    ...         "Class 1": ciw.routing.TransitionMatrix(transition_matrix=[[0.3]])
+    ...     }
+    ... )
 
-    >>> import random
-    >>> def routing_function_Node_2(ind):
-    ...     if random.random() <= 0.5:
-    ...         return [2, 3]
-    ...     return [2, 1]
 
-As there are no arrivals at Node 3, no customer will need routing assigned here. However, we need to use the placeholder function :code:`ciw.no_routing` to account for this::
+Custom Routing Objects
+~~~~~~~~~~~~~~~~~~~~~~
 
-    >>> N = ciw.create_network(
-    ...     arrival_distributions=[ciw.dists.Exponential(rate=1),
-    ...                            ciw.dists.Deterministic(value=1),
-    ...                            None],
-    ...     service_distributions=[ciw.dists.Exponential(rate=2),
-    ...                            ciw.dists.Exponential(rate=2),
-    ...                            ciw.dists.Exponential(rate=2)],
-    ...     number_of_servers=[1,1,1],
-    ...     routing=[routing_function_Node_1,
-    ...              routing_function_Node_2,
-    ...              ciw.no_routing]
-    ... )
+Ciw allows for custom built routing objects. These allow for both time and state dependent routing, allowing flexible and routing logic. A guide is given :ref:`here<custom-routing>`.
```

### Comparing `Ciw-3.1.4/docs/Guides/processor-sharing.rst` & `ciw-3.2.0/docs/Guides/Services/processor-sharing.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 Now we create a simulation object using :code:`ciw.PSNode` rather than :code:`ciw.Node`::
     
     >>> ciw.seed(0)
     >>> Q = ciw.Simulation(N, node_class=ciw.PSNode)
 
 Note that this applies the process sharing node to every node of the network.
-Alternatively we could provide a list of different node classes, for use on each different node of the network (see :ref:`this example <ps-routing>` for an in depth example of this)::
+Alternatively we could provide a list of different node classes, for use on each different node of the network (see :ref:`this example <example_lb>` for an in depth example of this)::
 
     >>> ciw.seed(0)
     >>> Q = ciw.Simulation(N, node_class=[ciw.PSNode])
 
 Now let's run the simulation until 1000 customers have passed though::
 
     >>> Q.simulate_until_max_customers(1000)
@@ -133,11 +133,11 @@
     \frac{A^R}{R!} \cdot \frac{R}{R-A}
     }{
     \left(\frac{A^R}{R!} \cdot \frac{R}{R-A}\right) + \sum_{i=0}^{R-1}\frac{A^i}{i!}
     }
 
 Plotting these theoretical results against a single run of our simulation shows a good alignment:
 
-.. image:: ../_static/ps_capacitated_verification.svg
+.. image:: ../../_static/ps_capacitated_verification.svg
    :alt: Alignment of theoretical and simulation results for a capacitated PS queue.
    :align: center
```

### Comparing `Ciw-3.1.4/docs/Guides/progressbar.rst` & `ciw-3.2.0/docs/Guides/Simulation/progressbar.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 An example when using the :code:`simulate_until_max_time` method::
 
     >>> Q.simulate_until_max_time(2000.0, progress_bar=True) # doctest:+SKIP
 
 The image below shows an example of the output:
 
-.. image:: ../_static/progress_bar_time.png
+.. image:: ../../_static/progress_bar_time.png
    :scale: 100 %
    :alt: Output of progress bar (simulate_until_max_time).
    :align: center
 
 An example when using the :code:`simulate_until_max_customers` method::
 
     >>> Q.simulate_until_max_customers(20000, progress_bar=True) # doctest:+SKIP
 
 And the image below shows the output:
 
-.. image:: ../_static/progress_bar_customers.png
+.. image:: ../../_static/progress_bar_customers.png
    :scale: 100 %
    :alt: Output of progress bar (simulate_until_max_customers).
    :align: center
```

### Comparing `Ciw-3.1.4/docs/Guides/reneging.rst` & `ciw-3.2.0/docs/Guides/CustomerBehaviour/reneging.rst`

 * *Files 5% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 
     >>> N = ciw.create_network(
     ...     arrival_distributions=[ciw.dists.Exponential(5),
     ...                            None],
     ...     service_distributions=[ciw.dists.Exponential(2),
     ...                            ciw.dists.Exponential(4)],
     ...     number_of_servers=[1, 1],
-    ...     routing=[[0, 0],
-    ...              [0, 0]],
+    ...     routing=[[0.0, 0.0],
+    ...              [0.0, 0.0]],
     ...     reneging_time_distributions=[ciw.dists.Deterministic(6),
     ...                                  None],
     ...     reneging_destinations=[2, -1]
     ... )
 
     >>> ciw.seed(0)
     >>> Q = ciw.Simulation(N, exact=5)
```

### Comparing `Ciw-3.1.4/docs/Guides/seed.rst` & `ciw-3.2.0/docs/Guides/Simulation/seed.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Guides/server_priority.rst` & `ciw-3.2.0/docs/Guides/Services/server_priority.rst`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ... )
 
     >>> ciw.seed(0)
     >>> Q = ciw.Simulation(N)
     >>> Q.simulate_until_max_time(1000)
 
     >>> [srv.utilisation for srv in Q.nodes[1].servers]
-    [0.3184942440259139, 0.1437617661984246, 0.04196395909329539]
+    [0.31849424..., 0.14376176..., 0.04196395...]
 
 
 Ciw allows servers to be prioritised according to a custom server priority function. 
 We can define a custom server priority function that returns the cumulative amount of time a server was busy::
 
     >>> def server_busy_time(server, ind):
     ...     return server.busy_time
@@ -48,15 +48,15 @@
     ... )
 
     >>> ciw.seed(0)
     >>> Q = ciw.Simulation(N)
     >>> Q.simulate_until_max_time(1000)
 
     >>> [srv.utilisation for srv in Q.nodes[1].servers]
-    [0.16784616228588892, 0.16882711899030475, 0.1675466880414403]
+    [0.16784616..., 0.16882711..., 0.16754668...]
 
 
 
 Prioritising Using the Individual
 ---------------------------------
 
 It is also possible to use the individual to be served as a way to determine the priority of the servers. 
@@ -91,15 +91,15 @@
     ...     server_priority_functions=[custom_server_priority]
     ... )
 
     >>> ciw.seed(0)
     >>> Q = ciw.Simulation(N)
     >>> Q.simulate_until_max_time(1000)
     >>> [srv.utilisation for srv in Q.nodes[1].servers]
-    [0.36132860028585134, 0.3667939476202799, 0.2580202674603771]
+    [0.36132860..., 0.36679394..., 0.25802026...]
 
 Utilisation is fairly even between the first two servers, with the third server picking up any slack. Now let's see what happens when there is three times as many individuals of class 0 entering the system as there are of class 1::
 
     >>> N = ciw.create_network(
     ...     arrival_distributions={
     ...         'Class 0': [ciw.dists.Exponential(1.5)],
     ...         'Class 1': [ciw.dists.Exponential(0.5)]
@@ -112,15 +112,15 @@
     ...     server_priority_functions=[custom_server_priority]
     ... )
 
     >>> ciw.seed(0)
     >>> Q = ciw.Simulation(N)
     >>> Q.simulate_until_max_time(1000)
     >>> [srv.utilisation for srv in Q.nodes[1].servers]
-    [0.447650059165907, 0.2678754897968868, 0.29112382084389343]
+    [0.44765005..., 0.26787548..., 0.29112382...]
 
 Now the first server is much busier than the others.
 
 
 Important Notice
 ----------------
```

### Comparing `Ciw-3.1.4/docs/Guides/service_disciplines.rst` & `ciw-3.2.0/docs/Guides/Services/service_disciplines.rst`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 Custom Disciplines
 ------------------
 
 Other service disciplines can also be implemented by writing a custom service discipline function. These functions take in a list of individuals, and the current time, and returns an individual from that list that represents the next individual to be served. As this is a list of individuals, we can access the individuals' attributes when making the service discipline decision.
 
-For example, say we wish to implement a service discipline that chooses the customers randomly, but with probability proportional to their arrival order, we could write:
+For example, say we wish to implement a service discipline that chooses the customers randomly, but with probability proportional to their arrival order, we could write::
 
     >>> def SIRO_proportional(individuals, t):
     ...     n = len(inds)
     ...     denominator = (n * (n + 1)) / 2
     ...     probs = [(n - i) / denominator for i in range(n)]
     ...     return ciw.random_choice(individuals, probs=probs)
```

### Comparing `Ciw-3.1.4/docs/Guides/set_distributions.rst` & `ciw-3.2.0/docs/Guides/Distributions/set_distributions.rst`

 * *Files 18% similar despite different names*

```diff
@@ -109,64 +109,7 @@
     >>> class CustomDistribution(ciw.dists.Distribution):
     ...     def sample(self, t=None, ind=None):
     ...         if random.random() < 0.5:
     ...             return 3.0
     ...         return random.random()
 
 This can then be implemented into a :code:`Network` object in the usual way.
-
-
-Combined Distributions
-----------------------
-
-As distribution objects inherit from the generic distirbution function, they can be *combined* using the operations :code:`+`, :code:`-`, :code:`*`, and :code:`/`.
-
-For example, let's combine an Exponential distribution with a Deterministic distribution in all four ways::
-
-    >>> Exp_add_Det = ciw.dists.Exponential(rate=0.05) + ciw.dists.Deterministic(value=3.0)
-    >>> Exp_sub_Det = ciw.dists.Exponential(rate=0.05) - ciw.dists.Deterministic(value=3.0)
-    >>> Exp_mul_Det = ciw.dists.Exponential(rate=0.05) * ciw.dists.Deterministic(value=3.0)
-    >>> Exp_div_Det = ciw.dists.Exponential(rate=0.05) / ciw.dists.Deterministic(value=3.0)
-
-These combined distributions return the combined sampled values:
-
-    >>> ciw.seed(10)
-    >>> Ex = ciw.dists.Exponential(rate=0.05)
-    >>> Dt = ciw.dists.Deterministic(value=3.0)
-    >>> [round(Ex.sample(), 2) for _ in range(5)]
-    [16.94, 11.2, 17.26, 4.62, 33.57]
-    >>> [round(Dt.sample(), 2) for _ in range(5)]
-    [3.0, 3.0, 3.0, 3.0, 3.0]
-
-    >>> # Addition
-    >>> ciw.seed(10)
-    >>> [round(Exp_add_Det.sample(), 2) for _ in range(5)]
-    [19.94, 14.2, 20.26, 7.62, 36.57]
-
-    >>> # Subtraction
-    >>> ciw.seed(10)
-    >>> [round(Exp_sub_Det.sample(), 2) for _ in range(5)]
-    [13.94, 8.2, 14.26, 1.62, 30.57]
-
-    >>> # Multiplication
-    >>> ciw.seed(10)
-    >>> [round(Exp_mul_Det.sample(), 2) for _ in range(5)]
-    [50.83, 33.61, 51.78, 13.85, 100.7]
-
-    >>> # Division
-    >>> ciw.seed(10)
-    >>> [round(Exp_div_Det.sample(), 2) for _ in range(5)]
-    [5.65, 3.73, 5.75, 1.54, 11.19]
-
-
-Mixture Distributions
----------------------
-Distributions can also be combined probabilistically. A countable and finite mixture distriubtion probabilistically chooses to sample from one of a number of given distributions. Given a number of distributions each with PDF :math:`D_i(x)`, each with a probability :math:`p_i`, such that :math:`\sum_i p_i = 1`, then the Mixture distribution has PMF :math:`f(x) = \sum_i p_i D_i(x)`
-
-For example, say let's make a mixture distribution that samples from an Exponential distribution rate 1 with probability 0.5, another Exponential distribution rate 2 with probability 0.2, a Uniform distribution between 0.2 and 0.8 with probability 0.2, and returns a Deterministic value of 0.5 with probability 0.1. We can do this with:
-
-    >>> Exp1 = ciw.dists.Exponential(rate=1)
-    >>> Exp2 = ciw.dists.Exponential(rate=2)
-    >>> Unif = ciw.dists.Uniform(lower=0.2, upper=0.8)
-    >>> Det5 = ciw.dists.Deterministic(0.5)
-
-    >>> M = ciw.dists.MixtureDistribution(dists=[Exp1, Exp2, Unif, Det5], probs=[0.5, 0.2, 0.2, 0.1])
```

### Comparing `Ciw-3.1.4/docs/Guides/sim_numcusts.rst` & `ciw-3.2.0/docs/Guides/Simulation/sim_numcusts.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Guides/slotted.rst` & `ciw-3.2.0/docs/Guides/Services/slotted.rst`

 * *Files 21% similar despite different names*

```diff
@@ -43,26 +43,58 @@
     >>> Q.simulate_until_max_time(7)
     >>> recs = Q.get_all_records()
     
     >>> set([r.service_start_date for r in recs])
     {1.5, 2.3, 2.8, 4.3, 5.1, 5.6}
 
 
+Schedule Offsets
+----------------
+
+A slotted schedule can be offset by a given amount of time. This means that the cyclic schedule will have a delayed start. This is defined using the :code:`offset` keyword. It's effect can be compared below::
+
+    ciw.Slotted(slots=[1.5, 2.3, 2.8], slot_sizes=[2, 5, 3])
+
+gives:
+
+    +----------------------------+------+------+------+------+------+------+------+------+
+    |   Slot Times :math:`t`     |  1.5 |  2.3 |  2.8 |  4.3 |  5.1 |  5.6 |  7.1 |  ... |
+    +----------------------------+------+------+------+------+------+------+------+------+
+    |   Slot Sizes :math:`s_t`   |    2 |    5 |    3 |    2 |    5 |    3 |    2 |  ... |
+    +----------------------------+------+------+------+------+------+------+------+------+
+
+whereas::
+
+    ciw.Slotted(slots=[1.5, 2.3, 2.8], slot_sizes=[2, 5, 3], offset=10.0)
+
+gives:
+
+    +----------------------------+-------+-------+-------+-------+-------+-------+-------+------+
+    |   Slot Times :math:`t`     |  11.5 |  12.3 |  12.8 |  14.3 |  15.1 |  15.6 |  17.1 |  ... |
+    +----------------------------+-------+-------+-------+-------+-------+-------+-------+------+
+    |   Slot Sizes :math:`s_t`   |     2 |     5 |     3 |     2 |     5 |     3 |     2 |  ... |
+    +----------------------------+-------+-------+-------+-------+-------+-------+-------+------+
+
+
+An offset of 10 here delays the beginning of the first slot by 10 time units, and that offset does not appear again in the cyclic schedule. The offset should only be defined as a positive float.
+
+
+
 
 Capacitated & Non-capacitated Slots
 -----------------------------------
 
 Slots can be capacitated or non-capacitated. This effects their behaviour when service times last longer than the gaps between slots:
 
   +  **Capacitated**: At each slot :math:`t`, only :math:`s_t` customers are allowed in service. That means that if any customers are still being served at time :math:`t`, then less than :math:`s_t` customers will begin service, ensuring only :math:`s_t` customers are in service at a time.
   + **Non-capacitated**: At each time slot :math:`t`, :math:`s_t` customers *begin* service, regardless of any pervious customers still being in service.
 
 This is shown visually below:
 
-.. image:: ../_static/slotted.svg
+.. image:: ../../_static/slotted.svg
    :scale: 20 %
    :alt: Comparing capacitated and non-capacitated slotted schedules.
    :align: center
 
 In order to specify capacitated or non-capacitated slotted schedules, use the keyword :code:`capacitated` when creating the :code:`ciw.Slotted` object. Non-capacitated is the default::
 
     ciw.Slotted(slots=[1.5, 2.3, 2.8], slot_sizes=[2, 5, 3])  # Non-capacitated
```

### Comparing `Ciw-3.1.4/docs/Guides/state_trackers.rst` & `ciw-3.2.0/docs/Guides/System/state_trackers.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Guides/time_dependent.rst` & `ciw-3.2.0/docs/Guides/Distributions/time_dependent.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Makefile` & `ciw-3.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Reference/citation.rst` & `ciw-3.2.0/docs/Reference/citation.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Reference/distributions.rst` & `ciw-3.2.0/docs/Reference/distributions.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Reference/glossary.rst` & `ciw-3.2.0/docs/Reference/glossary.rst`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/Reference/results.rst` & `ciw-3.2.0/docs/Reference/results.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
    :stub-columns: 1
 
    * - Attribute
      - Description
    * - :code:`id_number`
      - The unique identification number for that customer.
    * - :code:`customer_class`
-     - The number of that customer's customer class. If dynamic customer classes are used, this is the customer's class that they were when they recieved service at that node.
+     - The number of that customer's customer class. If dynamic customer classes are used, this is the customer's class that they were when they received service at that node.
    * - :code:`original_customer_class`
      - The number of the customer's class when they arrived at the node.
    * - :code:`node`
      - The number of the node at which the service took place.
    * - :code:`arrival_date`
      - The date of arrival to that node, the date which the customer joined the queue.
    * - :code:`waiting_time`
@@ -30,37 +30,37 @@
    * - :code:`service_time`
      - The amount of time spent in service at that node.
    * - :code:`service_end_date`
      - The date which the customer finished their service at that node.
    * - :code:`time_blocked`
      - The amount of time spent blocked at that node. That is the time between finishing service at exiting the node.
    * - :code:`exit_date`
-     - The date which the customer exited the node. This may be immediatly after service if no blocking occured, or after some period of being blocked.
+     - The date which the customer exited the node. This may be immediately after service if no blocking occured, or after some period of being blocked.
    * - :code:`destination`
      - The number of the customer's destination, that is the next node the customer will join after leaving the current node. If the customer leaves the system, this will be -1.
    * - :code:`queue_size_at_arrival`
      - The size of the queue at the customer's arrival date. Does not include the individual themselves.
    * - :code:`queue_size_at_departure`
      - The size of the queue at the customer's exit date. Does not include the individual themselves.
    * - :code:`server_id`
      - The unique identification number of the server that served that customer.
    * - :code:`record_type`
      - Indicates what type of data record this is. See below.
 
 
 The attribute :code:`record_type` can be one of:
     - :code:`"service"`: a completed service
-    - :code:`"interrupted service"`: an interupted service
+    - :code:`"interrupted service"`: an interrupted service
     - :code:`"renege"`: the waiting time while a customer waited before reneging
     - :code:`"baulk"`: the record of a customer baulking
     - :code:`"rejection"`: the record of a customer being rejected due to the queue being full
 
 
 
 You may access these records as a list of named tuples, using the Simulation's :code:`get_all_records` method::
 
     >>> recs = Q.get_all_records() # doctest:+SKIP
 
-By default, all record types are included. However, we may only want some of the record types, and these can be filtered by passing a list of desired record types to the :code:`only` keyword argument. For example, to only recieve service and reneging customers, we can use::
+By default, all record types are included. However, we may only want some of the record types, and these can be filtered by passing a list of desired record types to the :code:`only` keyword argument. For example, to only receive service and reneging customers, we can use::
 
     >>> recs = Q.get_all_records(only=["service", "renege"]) # doctest:+SKIP
```

### Comparing `Ciw-3.1.4/docs/Reference/state_trackers.rst` & `ciw-3.2.0/docs/Reference/state_trackers.rst`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ==================================
 
 Currently Ciw has the following state trackers:
 
 - :ref:`population`
 - :ref:`nodepop`
 - :ref:`nodepopsubset`
+- :ref:`groupednodepop`
 - :ref:`nodeclssmatrix`
 - :ref:`naiveblock`
 - :ref:`matrixblock`
 
 
 .. _population:
 
@@ -64,14 +65,32 @@
 This denotes that there are two customers at the first observed node, no customers at the second observed node, and five customers at the third observed node.
 
 The Simulation object takes in the optional argument :code:`tracker`, which takes an argument :code:`observed_nodes` a list of node numbers to observe, used as follows (observing the first, second, and fifth nodes)::
 
     >>> Q = ciw.Simulation(N, tracker=ciw.trackers.NodePopulationSubset([0, 1, 4])) # doctest:+SKIP
 
 
+.. _groupednodepop:
+
+---------------------------------
+The GroupedNodePopulation Tracker
+---------------------------------
+
+The GroupedNodePopulation Tracker, similar to the NodePopulation Tracker, records the number of customers at each node. However this allows users to group nodes together into one state.
+States take the form of list of numbers. An example of tracking a queueing network with three grouped nodes is shown below::
+
+    (2, 0, 5)
+
+This denotes that there are two customers at the first group of nodes, no customers at the second group of nodes, and five customers at the third group of nodes.
+
+The Simulation object takes in the optional argument :code:`tracker`, which takes an argument :code:`groups` a list of groups of nodes (a list of lists, nodes in the same list are in the same group), used as follows (the first group observes the total population in the 1st and 7th nodes, the second group observed the population of the 4th node, and the 3th group observes the population in the 2nd, 3rd, 5th and 6th nodes::
+
+    >>> Q = ciw.Simulation(N, tracker=ciw.trackers.GroupedNodePopulation(groups=[[0, 6], [3], [1, 2, 4, 5]])) # doctest:+SKIP
+
+
 .. _nodeclssmatrix:
 
 ---------------------------
 The NodeClassMatrix Tracker
 ---------------------------
 
 The NodeClassPopulation Tracker records the number of customers at each node, split by customer class.
```

### Comparing `Ciw-3.1.4/docs/Tutorial-I/tutorial_i.rst` & `ciw-3.2.0/docs/Tutorial/GettingStarted/part_1.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.. _tutorial-i:
+.. _tutorial-i-p1:
 
-===========================================
-Tutorial I: Defining & Running a Simulation
-===========================================
+====================================================
+Tutorial I: Part 1 - Defining & Running a Simulation
+====================================================
 
 Assume you are a bank manager and would like to know how long customers wait in your bank.
 Customers arrive randomly, roughly 12 per hour, regardless of the time of day.
 Service time is random, but on average lasts roughly 10 minutes.
 The bank is open 24 hours a day, 7 days a week, and has three servers who are always on duty.
 If all servers are busy, newly arriving customers form a queue and wait for service.
 On average how long do customers wait?
@@ -60,8 +60,8 @@
 
 Let's run the simulation for a day of bank time (don't worry, this won't take a day of real time!).
 As we parametrised the system with time units of minutes, a day will be 1440 time units::
 
     >>> Q.simulate_until_max_time(1440)
 
 Well done! We've now defined and simulated the bank for a day.
-In the next tutorial, we will explore the :code:`Simulation` object some more.
+In the next part, we will explore the :code:`Simulation` object some more.
```

### Comparing `Ciw-3.1.4/docs/Tutorial-I/tutorial_ii.rst` & `ciw-3.2.0/docs/Tutorial/GettingStarted/part_2.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-.. _tutorial-ii:
+.. _tutorial-i-p2:
 
-============================================
-Tutorial II: Exploring the Simulation Object
-============================================
+====================================================
+Tutorial I: Part 2 - Exploring the Simulation Object
+====================================================
 
-In the previous tutorial, we defined and simulated our bank for a week::
+In the previous part, we defined and simulated our bank for a week::
 
     >>> import ciw
     >>> N = ciw.create_network(
     ...     arrival_distributions=[ciw.dists.Exponential(rate=0.2)],
     ...     service_distributions=[ciw.dists.Exponential(rate=0.1)],
     ...     number_of_servers=[3]
     ... )
@@ -19,15 +19,15 @@
 Let's explore the Simulation object :code:`Q`.
 Although our queueing system consisted of one node (the bank), the object :code:`Q` is made up of three, accessed using::
 
     >>> Q.nodes
     [Arrival Node, Node 1, Exit Node]
 
 + **The Arrival Node:**
-  This is where customers are created. They are spawned here, and can :ref:`baulk <baulking-functions>`, :ref:`be rejected <tutorial-vi>` or sent to a service node. Accessed using::
+  This is where customers are created. They are spawned here, and can :ref:`baulk <baulking-functions>`, :ref:`be rejected <tutorial-iii>` or sent to a service node. Accessed using::
 
     >>> Q.nodes[0]
     Arrival Node
 
 + **Service Node:**
   This is where customers queue up and receive service. This can be thought of as the bank itself. Accessed using::
 
@@ -72,8 +72,8 @@
     2.944637...
     >>> ind.data_records[0].service_end_date
     10.88093...
     >>> ind.data_records[0].exit_date
     10.88093...
 
 This isn't a very efficient way to look at results.
-In the next tutorial we will look at generating lists of records to gain some summary statistics.
+In the next part we will look at generating lists of records to gain some summary statistics.
```

### Comparing `Ciw-3.1.4/docs/Tutorial-I/tutorial_iv.rst` & `ciw-3.2.0/docs/Tutorial/GettingStarted/part_4.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-.. _tutorial-iv:
+.. _tutorial-i-p4:
 
-========================================
-Tutorial IV: Trials, Warm-up & Cool-down
-========================================
+================================================
+Tutorial I: Part 4 - Trials, Warm-up & Cool-down
+================================================
 
-In Tutorials I-III we investigated one run of a simulation of a bank.
+In parts 1-3 we investigated one run of a simulation of a bank.
 Before we draw any conclusions about the behaviour of the bank, there are three things we should consider:
 
 1. Our original description of the bank described it as open 24/7. This means the bank would never start from an empty state, as our simulation does.
 2. Those customers left inside the system at the end of the run: their records were not collected, despite spending time in the system during the observation period.
 3. Does that single run of our simulation really reflect reality? Were our results simply a fluke? An extreme case?
 
 These three concerns can be addressed with warm-up, cool-down, and trials respectively.
@@ -41,15 +41,15 @@
     ...     mean_wait = sum(waits) / len(waits)
     ...     average_waits.append(mean_wait)
 
 The list :code:`average_waits` will now contain ten numbers denoting the mean waiting time from each of the trials.
 Notice that we set a different seed every time, so each trial will yield different results::
 
     >>> average_waits
-    [3.91950..., 4.34163..., 4.61779..., 5.33537..., 5.06224..., 2.90274..., 4.93209..., 17.95093128538666, 4.06136..., 3.14126...]
+    [3.91950..., 4.34163..., 4.61779..., 5.33537..., 5.06224..., 2.90274..., 4.93209..., 17.95093..., 4.06136..., 3.14126...]
 
 We can see that the range of waits are quite high, between 1.6 and 7.5.
 This shows that running a single trial wouldn't have given us a very confident answer.
 We can take the mean result over the trials to get a more confident answer::
 
     >>> sum(average_waits) / len(average_waits)
     5.62649...
```

### Comparing `Ciw-3.1.4/docs/Tutorial-II/tutorial_v.rst` & `ciw-3.2.0/docs/Tutorial/tutorial_ii.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.. _tutorial-v:
+.. _tutorial-ii:
 
-===============================
-Tutorial V: A Network of Queues
-===============================
+================================
+Tutorial II: A Network of Queues
+================================
 
 Ciw's real power comes when modelling networks of queues.
 That is many service nodes, such that when customers finish service, there is a probability of joining another node, rejoining the current node, or leaving the system.
 
 Imagine a café that sells both hot and cold food.
 Customers arrive and can take a few routes:
```

### Comparing `Ciw-3.1.4/docs/Tutorial-II/tutorial_vi.rst` & `ciw-3.2.0/docs/Tutorial/tutorial_iii.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.. _tutorial-vi:
+.. _tutorial-iii:
 
-================================
-Tutorial VI: Restricted Networks
-================================
+=================================
+Tutorial III: Restricted Networks
+=================================
 
 Imagine a manufacturing plant that produces stools:
 
 + Every 4 seconds a seat arrives on a conveyor-belt.
 + The belt contains three workstations.
 + At the each workstation a leg is connected.
 + Connecting a leg takes a random amount of time between 3 seconds and 5 seconds.
```

### Comparing `Ciw-3.1.4/docs/Tutorial-II/tutorial_vii.rst` & `ciw-3.2.0/docs/Tutorial/tutorial_iv.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.. _tutorial-vii:
+.. _tutorial-iv:
 
-==========================================
-Tutorial VII: Multiple Classes of Customer
-==========================================
+=========================================
+Tutorial IV: Multiple Classes of Customer
+=========================================
 
 Imagine a 24 hour paediatricians clinic:
 
 + Two types of patient arrive, babies and children.
 + When patients arrive they must register at the reception desk.
 + Registration time is random, but for babies lasts an average of 15 minutes, and for children and average of 10 minutes.
 + After registration the two types of patients go to separate waiting rooms where they wait to be seen by separate specialists.
```

### Comparing `Ciw-3.1.4/docs/_static/2nodes.svg` & `ciw-3.2.0/docs/_static/2nodes.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/2nodesindeadlock.svg` & `ciw-3.2.0/docs/_static/2nodesindeadlock.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/cafe.svg` & `ciw-3.2.0/docs/_static/cafe.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/codestructure.svg` & `ciw-3.2.0/docs/_static/codestructure.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/codestructure.tex` & `ciw-3.2.0/docs/_static/codestructure.tex`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/coxian.svg` & `ciw-3.2.0/docs/_static/coxian.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/custom_number_servers_with.svg` & `ciw-3.2.0/docs/_static/custom_number_servers_with.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/custom_number_servers_without.svg` & `ciw-3.2.0/docs/_static/custom_number_servers_without.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/des+sd_hybrid.svg` & `ciw-3.2.0/docs/_static/des+sd_hybrid.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/erlang.svg` & `ciw-3.2.0/docs/_static/erlang.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/favicon.ico` & `ciw-3.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/hybrid.png` & `ciw-3.2.0/docs/_static/hybrid.png`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/hypererlang.svg` & `ciw-3.2.0/docs/_static/hypererlang.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/hyperexponential.svg` & `ciw-3.2.0/docs/_static/hyperexponential.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/logo.pdf` & `ciw-3.2.0/docs/_static/logo.pdf`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/logo.png` & `ciw-3.2.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/logo.svg` & `ciw-3.2.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/logo_small.png` & `ciw-3.2.0/docs/_static/logo_small.png`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/phasetype.svg` & `ciw-3.2.0/docs/_static/phasetype.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/progress_bar_customers.png` & `ciw-3.2.0/docs/_static/progress_bar_customers.png`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/progress_bar_time.png` & `ciw-3.2.0/docs/_static/progress_bar_time.png`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/ps_capacitated_verification.svg` & `ciw-3.2.0/docs/_static/ps_capacitated_verification.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/script_for_parallel_processing/main.py` & `ciw-3.2.0/docs/_static/script_for_parallel_processing/main.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/server_dependent_dist_with.svg` & `ciw-3.2.0/docs/_static/server_dependent_dist_with.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/server_dependent_dist_without.svg` & `ciw-3.2.0/docs/_static/server_dependent_dist_without.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/_static/tutorial_iii_waitshist.svg` & `ciw-3.2.0/docs/_static/tutorial_iii_waitshist.svg`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/conf.py` & `ciw-3.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Ciw-3.1.4/docs/index.rst` & `ciw-3.2.0/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -7,26 +7,25 @@
 restricted networks.
 A number of other features are also implemented, including priorities,
 baulking, reneging, schedules, slotted services, batch arrivals, service
 disciplines, dynamic customer classes, and deadlock detection.
 
 The name **Ciw** is the Welsh word for a queue.
 
-Ciw is currently supported for and regularly tested on Python versions 3.7,
-3.8, 3.9, 3.10 and 3.11.
+Ciw is currently supported for and regularly tested on Python versions 3.8,
+3.9, 3.10, 3.11 and 3.12.
 
 Contents:
 
 .. toctree::
-   :maxdepth: 2
+   :maxdepth: 3
    :titlesonly:
    
    installation.rst
-   Tutorial-I/index.rst
-   Tutorial-II/index.rst
+   Tutorial/index.rst
    Guides/index.rst
    Reference/index.rst
    Background/index.rst
 
 
 - :ref:`genindex`
 - :ref:`search`
```

### Comparing `Ciw-3.1.4/setup.py` & `ciw-3.2.0/setup.py`

 * *Files identical despite different names*

