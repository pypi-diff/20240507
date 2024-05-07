# Comparing `tmp/siibra-1.0a8.tar.gz` & `tmp/siibra-1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siibra-1.0a8.tar", last modified: Tue Mar 12 14:13:05 2024, max compression
+gzip compressed data, was "siibra-1.0a9.tar", last modified: Mon Mar 18 10:17:23 2024, max compression
```

## Comparing `siibra-1.0a8.tar` & `siibra-1.0a9.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.581079 siibra-1.0a8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-12 14:06:21.000000 siibra-1.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-12 14:06:21.000000 siibra-1.0a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-03-12 14:13:05.581079 siibra-1.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-03-12 14:06:21.000000 siibra-1.0a8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 14:13:05.581079 siibra-1.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-12 14:06:21.000000 siibra-1.0a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.565079 siibra-1.0a8/siibra/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27532 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.565079 siibra-1.0a8/siibra/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    21109 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/configuration/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.569079 siibra-1.0a8/siibra/core/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/core/assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/core/atlas.py
--rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/core/concept.py
--rw-r--r--   0 runner    (1001) docker     (127)    13873 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/core/parcellation.py
--rw-r--r--   0 runner    (1001) docker     (127)    38663 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/core/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/core/space.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/core/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.569079 siibra-1.0a8/siibra/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/experimental/contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/experimental/cortical_profile_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/experimental/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/experimental/plane3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.569079 siibra-1.0a8/siibra/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/explorer/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/explorer/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.569079 siibra-1.0a8/siibra/features/
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/anchor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.569079 siibra-1.0a8/siibra/features/connectivity/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/connectivity/functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)    16736 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/connectivity/regional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/connectivity/streamline_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/connectivity/streamline_lengths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/connectivity/tracing_connectivity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.573079 siibra-1.0a8/siibra/features/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/dataset/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (127)    32572 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.573079 siibra-1.0a8/siibra/features/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/image/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/image/sections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/image/volume_of_interest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.573079 siibra-1.0a8/siibra/features/tabular/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/tabular/bigbrain_intensity_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/tabular/cell_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/tabular/cortical_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/tabular/gene_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/tabular/layerwise_bigbrain_intensities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/tabular/layerwise_cell_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     7186 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/tabular/receptor_density_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/tabular/receptor_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/tabular/regional_timeseries_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/features/tabular/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.573079 siibra-1.0a8/siibra/livequeries/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/livequeries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/livequeries/allen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/livequeries/bigbrain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/livequeries/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/livequeries/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.577079 siibra-1.0a8/siibra/locations/
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15298 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/locations/boundingbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/locations/location.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/locations/point.py
--rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/locations/pointset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.577079 siibra-1.0a8/siibra/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/retrieval/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/retrieval/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.577079 siibra-1.0a8/siibra/retrieval/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/retrieval/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30441 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/retrieval/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/retrieval/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.581079 siibra-1.0a8/siibra/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/vocabularies/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)  1647972 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/vocabularies/gene_names.json
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/vocabularies/receptor_symbols.json
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/vocabularies/region_aliases.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.581079 siibra-1.0a8/siibra/volumes/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48644 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/volumes/parcellationmap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.581079 siibra-1.0a8/siibra/volumes/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/volumes/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/volumes/providers/gifti.py
--rw-r--r--   0 runner    (1001) docker     (127)    26936 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/volumes/providers/neuroglancer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/volumes/providers/nifti.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/volumes/providers/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    22274 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/volumes/sparsemap.py
--rw-r--r--   0 runner    (1001) docker     (127)    25771 2024-03-12 14:06:21.000000 siibra-1.0a8/siibra/volumes/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.581079 siibra-1.0a8/siibra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-03-12 14:13:05.000000 siibra-1.0a8/siibra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-12 14:13:05.000000 siibra-1.0a8/siibra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 14:13:05.000000 siibra-1.0a8/siibra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-12 14:13:05.000000 siibra-1.0a8/siibra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-12 14:13:05.000000 siibra-1.0a8/siibra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:13:05.581079 siibra-1.0a8/test/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-12 14:06:21.000000 siibra-1.0a8/test/test_siibra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.406697 siibra-1.0a9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-18 10:12:31.000000 siibra-1.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-18 10:12:31.000000 siibra-1.0a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-03-18 10:17:23.406697 siibra-1.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-03-18 10:12:31.000000 siibra-1.0a9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 10:17:23.406697 siibra-1.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-18 10:12:31.000000 siibra-1.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.386697 siibra-1.0a9/siibra/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28449 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.390697 siibra-1.0a9/siibra/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21110 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/configuration/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.390697 siibra-1.0a9/siibra/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/core/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/core/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/core/concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13873 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/core/parcellation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38661 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/core/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/core/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/core/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.390697 siibra-1.0a9/siibra/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/experimental/contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/experimental/cortical_profile_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/experimental/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/experimental/plane3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.390697 siibra-1.0a9/siibra/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/explorer/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/explorer/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.394697 siibra-1.0a9/siibra/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/anchor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.394697 siibra-1.0a9/siibra/features/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/connectivity/functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16736 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/connectivity/regional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/connectivity/streamline_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/connectivity/streamline_lengths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/connectivity/tracing_connectivity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.394697 siibra-1.0a9/siibra/features/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/dataset/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32573 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.394697 siibra-1.0a9/siibra/features/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/image/sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/image/volume_of_interest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.398697 siibra-1.0a9/siibra/features/tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/tabular/bigbrain_intensity_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/tabular/cell_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/tabular/cortical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/tabular/gene_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/tabular/layerwise_bigbrain_intensities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/tabular/layerwise_cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7186 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/tabular/receptor_density_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/tabular/receptor_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/tabular/regional_timeseries_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/features/tabular/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.398697 siibra-1.0a9/siibra/livequeries/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/livequeries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/livequeries/allen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/livequeries/bigbrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/livequeries/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/livequeries/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.398697 siibra-1.0a9/siibra/locations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15298 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/locations/boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/locations/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/locations/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/locations/pointset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.398697 siibra-1.0a9/siibra/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/retrieval/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/retrieval/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.398697 siibra-1.0a9/siibra/retrieval/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/retrieval/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30443 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/retrieval/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/retrieval/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.402697 siibra-1.0a9/siibra/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/vocabularies/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1647972 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/vocabularies/gene_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/vocabularies/receptor_symbols.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/vocabularies/region_aliases.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.402697 siibra-1.0a9/siibra/volumes/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48646 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/volumes/parcellationmap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.402697 siibra-1.0a9/siibra/volumes/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/volumes/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/volumes/providers/gifti.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26940 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/volumes/providers/neuroglancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/volumes/providers/nifti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/volumes/providers/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22274 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/volumes/sparsemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25771 2024-03-18 10:12:31.000000 siibra-1.0a9/siibra/volumes/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.402697 siibra-1.0a9/siibra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-03-18 10:17:23.000000 siibra-1.0a9/siibra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-18 10:17:23.000000 siibra-1.0a9/siibra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 10:17:23.000000 siibra-1.0a9/siibra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-18 10:17:23.000000 siibra-1.0a9/siibra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-18 10:17:23.000000 siibra-1.0a9/siibra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:23.402697 siibra-1.0a9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-18 10:12:31.000000 siibra-1.0a9/test/test_siibra.py
```

### Comparing `siibra-1.0a8/LICENSE` & `siibra-1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/PKG-INFO` & `siibra-1.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 1.0a8
+Version: 1.0a9
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `siibra-1.0a8/README.rst` & `siibra-1.0a9/README.rst`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/setup.py` & `siibra-1.0a9/setup.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/__init__.py` & `siibra-1.0a9/siibra/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/commons.py` & `siibra-1.0a9/siibra/commons.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import re
 from enum import Enum
 from nibabel import Nifti1Image
 import logging
 from tqdm import tqdm
 import numpy as np
 import pandas as pd
-from typing import Generic, Iterable, Iterator, List, TypeVar, Union, Dict
+from typing import Generic, Iterable, Iterator, List, TypeVar, Union, Dict, Generator, Tuple
 from skimage.filters import gaussian
 from dataclasses import dataclass
 from hashlib import md5
 from uuid import UUID
 import math
 try:
     from typing import TypedDict
@@ -526,20 +526,48 @@
         Nifti1Image(source_data, source_affine),
         Nifti1Image(target_data, target_affine),
         interpolation=interp
     )
     return np.asanyarray(resampled_img.dataobj)
 
 
-def connected_components(imgdata: np.ndarray):
-    """
-    Provide an iterator over connected components in the array
+def connected_components(
+    imgdata: np.ndarray,
+    background: int = 0,
+    connectivity: int = 2,
+    threshold: float = 0.0,
+) -> Generator[Tuple[int, np.ndarray], None, None]:
+    """
+    Provide an iterator over connected components in the array. If the image
+    data is float (such as probability maps), it will convert to a mask and
+    then find the connected components.
+
+    Note
+    ----
+    `Uses skimage.measure.label()` to determine foreground compenents.
+
+    Parameters
+    ----------
+    imgdata : np.ndarray
+    background_value : int, Default: 0
+    connectivity : int, Default: 2
+    threshold: float, Default: 0.0
+        The threshold used to create mask from probability maps, i.e, anything
+        below set to 0 and rest to 1.
+
+    Yields
+    ------
+    Generator[Tuple[int, np.ndarray], None, None]
+        tuple of integer label of the component and component as an nd.array in
+        the shape of the original image.
     """
     from skimage import measure
-    components = measure.label(imgdata, connectivity=2, background=0)
+
+    mask = (imgdata > threshold).astype('uint8')
+    components = measure.label(mask, connectivity=connectivity, background=background)
     component_labels = np.unique(components)
     return (
         (label, (components == label).astype('uint8'))
         for label in component_labels
         if label > 0
     )
```

### Comparing `siibra-1.0a8/siibra/configuration/__init__.py` & `siibra-1.0a9/siibra/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/configuration/configuration.py` & `siibra-1.0a9/siibra/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/configuration/factory.py` & `siibra-1.0a9/siibra/configuration/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
     @classmethod
     @build_type("siibra/map/v0.0.1")
     def build_map(cls, spec):
         # maps have no configured identifier - we require the spec filename to build one
         assert "filename" in spec
         basename = path.splitext(path.basename(spec['filename']))[0]
         name = basename.replace('-', ' ').replace('_', ' ').replace('continuous', 'statistical')
-        identifier = f"{spec['@type'].replace('/','-')}_{basename}"
+        identifier = f"{spec['@type'].replace('/', '-')}_{basename}"
         volumes = cls.extract_volumes(spec, space_id=spec["space"].get("@id"), name_prefix=basename)
 
         if spec.get("sparsemap", {}).get("is_sparsemap"):
             Maptype = sparsemap.SparseMap
         else:
             Maptype = parcellationmap.Map
         return Maptype(
```

### Comparing `siibra-1.0a8/siibra/core/__init__.py` & `siibra-1.0a9/siibra/core/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/core/assignment.py` & `siibra-1.0a9/siibra/core/assignment.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/core/atlas.py` & `siibra-1.0a9/siibra/core/atlas.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/core/concept.py` & `siibra-1.0a9/siibra/core/concept.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/core/parcellation.py` & `siibra-1.0a9/siibra/core/parcellation.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/core/region.py` & `siibra-1.0a9/siibra/core/region.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
             regex_match = self._regex_re.match(regionspec)
             if regex_match:
                 flags = regex_match.group('flags')
                 expression = regex_match.group('expression')
 
                 for flag in flags or []:  # catch if flags is nullish
                     if flag not in self._accepted_flags:
-                        raise Exception(f"only accepted flag are in { self._accepted_flags }. {flag} is not within them")
+                        raise Exception(f"only accepted flag are in {self._accepted_flags}. {flag} is not within them")
                 search_regex = (f"(?{flags})" if flags else "") + expression
                 regionspec = re.compile(search_regex)
 
         candidates = list(
             anytree.search.findall(self, lambda node: node.matches(regionspec))
         )
```

### Comparing `siibra-1.0a8/siibra/core/space.py` & `siibra-1.0a9/siibra/core/space.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/core/structure.py` & `siibra-1.0a9/siibra/core/structure.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/exceptions.py` & `siibra-1.0a9/siibra/exceptions.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/experimental/__init__.py` & `siibra-1.0a9/siibra/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/experimental/contour.py` & `siibra-1.0a9/siibra/experimental/contour.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/experimental/cortical_profile_sampler.py` & `siibra-1.0a9/siibra/experimental/cortical_profile_sampler.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/experimental/patch.py` & `siibra-1.0a9/siibra/experimental/patch.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/experimental/plane3d.py` & `siibra-1.0a9/siibra/experimental/plane3d.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/explorer/__init__.py` & `siibra-1.0a9/siibra/explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/explorer/url.py` & `siibra-1.0a9/siibra/explorer/url.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/explorer/util.py` & `siibra-1.0a9/siibra/explorer/util.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/__init__.py` & `siibra-1.0a9/siibra/features/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/anchor.py` & `siibra-1.0a9/siibra/features/anchor.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/connectivity/__init__.py` & `siibra-1.0a9/siibra/features/connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/connectivity/functional_connectivity.py` & `siibra-1.0a9/siibra/features/connectivity/functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/connectivity/regional_connectivity.py` & `siibra-1.0a9/siibra/features/connectivity/regional_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/connectivity/streamline_counts.py` & `siibra-1.0a9/siibra/features/connectivity/streamline_counts.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/connectivity/streamline_lengths.py` & `siibra-1.0a9/siibra/features/connectivity/streamline_lengths.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/connectivity/tracing_connectivity.py` & `siibra-1.0a9/siibra/features/connectivity/tracing_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/dataset/__init__.py` & `siibra-1.0a9/siibra/features/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/dataset/ebrains.py` & `siibra-1.0a9/siibra/features/dataset/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/feature.py` & `siibra-1.0a9/siibra/features/feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
     @classmethod
     def _livequery(cls, concept: Union[region.Region, parcellation.Parcellation, space.Space], **kwargs) -> List['Feature']:
         if not hasattr(cls, "_live_queries"):
             return []
 
         live_instances = []
         for QueryType in cls._live_queries:
-            argstr = f" ({', '.join('='.join(map(str,_)) for _ in kwargs.items())})" \
+            argstr = f" ({', '.join('='.join(map(str, _)) for _ in kwargs.items())})" \
                 if len(kwargs) > 0 else ""
             logger.debug(
                 f"Running live query for {QueryType.feature_type.__name__} "
                 f"objects linked to {str(concept)}{argstr}"
             )
             q = QueryType(**kwargs)
             features = q.query(concept)
```

### Comparing `siibra-1.0a8/siibra/features/image/__init__.py` & `siibra-1.0a9/siibra/features/image/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/image/image.py` & `siibra-1.0a9/siibra/features/image/image.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/image/sections.py` & `siibra-1.0a9/siibra/features/image/sections.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/image/volume_of_interest.py` & `siibra-1.0a9/siibra/features/image/volume_of_interest.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/tabular/__init__.py` & `siibra-1.0a9/siibra/features/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/tabular/bigbrain_intensity_profile.py` & `siibra-1.0a9/siibra/features/tabular/bigbrain_intensity_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/tabular/cell_density_profile.py` & `siibra-1.0a9/siibra/features/tabular/cell_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/tabular/cortical_profile.py` & `siibra-1.0a9/siibra/features/tabular/cortical_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/tabular/gene_expression.py` & `siibra-1.0a9/siibra/features/tabular/gene_expression.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/tabular/layerwise_bigbrain_intensities.py` & `siibra-1.0a9/siibra/features/tabular/layerwise_bigbrain_intensities.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/tabular/layerwise_cell_density.py` & `siibra-1.0a9/siibra/features/tabular/layerwise_cell_density.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/tabular/receptor_density_fingerprint.py` & `siibra-1.0a9/siibra/features/tabular/receptor_density_fingerprint.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/tabular/receptor_density_profile.py` & `siibra-1.0a9/siibra/features/tabular/receptor_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/tabular/regional_timeseries_activity.py` & `siibra-1.0a9/siibra/features/tabular/regional_timeseries_activity.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/features/tabular/tabular.py` & `siibra-1.0a9/siibra/features/tabular/tabular.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/livequeries/__init__.py` & `siibra-1.0a9/siibra/livequeries/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/livequeries/allen.py` & `siibra-1.0a9/siibra/livequeries/allen.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/livequeries/bigbrain.py` & `siibra-1.0a9/siibra/livequeries/bigbrain.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/livequeries/ebrains.py` & `siibra-1.0a9/siibra/livequeries/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/livequeries/query.py` & `siibra-1.0a9/siibra/livequeries/query.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/locations/__init__.py` & `siibra-1.0a9/siibra/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/locations/boundingbox.py` & `siibra-1.0a9/siibra/locations/boundingbox.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/locations/location.py` & `siibra-1.0a9/siibra/locations/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     @property
     def species(self):
         return None if self.space is None else self.space.species
 
     def __str__(self):
         space_str = "" if self.space is None else f" in {self.space.name}"
-        coord_str = "" if len(self) == 0 else f" [{','.join(str(l) for l in iter(self))}]"
+        coord_str = "" if len(self) == 0 else f" [{','.join(str(pt) for pt in iter(self))}]"
         return f"{self.__class__.__name__}{space_str}{coord_str}"
 
     def __repr__(self):
         spacespec = f"'{self.space.id}'" if self.space else None
         return f"<{self.__class__.__name__}({[point.__repr__() for point in self]}), space={spacespec}>"
 
     def __hash__(self) -> int:
```

### Comparing `siibra-1.0a8/siibra/locations/point.py` & `siibra-1.0a9/siibra/locations/point.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/locations/pointset.py` & `siibra-1.0a9/siibra/locations/pointset.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/retrieval/__init__.py` & `siibra-1.0a9/siibra/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/retrieval/cache.py` & `siibra-1.0a9/siibra/retrieval/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         index = 0
         for index, (fn, st) in enumerate(sfiles):
             if targetsize <= self.SIZE_GIB:
                 break
             targetsize -= st.st_size / 1024**3
 
         if index > 0:
-            logger.debug(f"Removing the {index+1} oldest files to keep cache size below {targetsize:.2f} GiB.")
+            logger.debug(f"Removing the {index + 1} oldest files to keep cache size below {targetsize:.2f} GiB.")
             for fn, st in sfiles[:index + 1]:
                 if os.path.isdir(fn):
                     import shutil
                     size = sum(os.path.getsize(f) for f in os.listdir(fn) if os.path.isfile(f))
                     shutil.rmtree(fn)
                 else:
                     size = st.st_size
```

### Comparing `siibra-1.0a8/siibra/retrieval/datasets.py` & `siibra-1.0a9/siibra/retrieval/datasets.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/retrieval/exceptions/__init__.py` & `siibra-1.0a9/siibra/retrieval/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/retrieval/repositories.py` & `siibra-1.0a9/siibra/retrieval/repositories.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
     @property
     def branches(self):
         return self._branchloader.data
 
     def _build_url(self, folder="", filename=None, recursive=False, page=1):
         ref = self.reftag if self.want_commit is None else self.want_commit["short_id"]
         if filename is None:
-            pathstr = "" if len(folder) == 0 else f"&path={quote(folder,safe='')}"
+            pathstr = "" if len(folder) == 0 else f"&path={quote(folder, safe='')}"
             return f"{self.base_url}/tree?ref={ref}{pathstr}&per_page={self._per_page}&page={page}&recursive={recursive}"
         else:
             pathstr = filename if folder == "" else f"{folder}/{filename}"
             filepath = quote(pathstr, safe="")
             return f"{self.base_url}/files/{filepath}/raw?ref={ref}"
 
     def search_files(self, folder="", suffix=None, recursive=False):
@@ -460,15 +460,15 @@
 
     def search_files(self, folder="", suffix=None, recursive=False):
         raise NotImplementedError(
             f"File search in folders not implemented for {self.__class__.__name__}."
         )
 
     def _build_url(self, folder, filename):
-        fpath = "" if folder == "" else f"path={quote(folder,safe='')}&"
+        fpath = "" if folder == "" else f"path={quote(folder, safe='')}&"
         fpath += f"files={quote(filename)}"
         url = f"{self.base_url}/download?{fpath}"
         return url
 
 
 class EbrainsHdgConnector(RepositoryConnector):
     """Download sensitive files from EBRAINS using
```

### Comparing `siibra-1.0a8/siibra/retrieval/requests.py` & `siibra-1.0a9/siibra/retrieval/requests.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/vocabularies/__init__.py` & `siibra-1.0a9/siibra/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/vocabularies/gene_names.json` & `siibra-1.0a9/siibra/vocabularies/gene_names.json`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/vocabularies/receptor_symbols.json` & `siibra-1.0a9/siibra/vocabularies/receptor_symbols.json`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/vocabularies/region_aliases.json` & `siibra-1.0a9/siibra/vocabularies/region_aliases.json`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/volumes/__init__.py` & `siibra-1.0a9/siibra/volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/volumes/parcellationmap.py` & `siibra-1.0a9/siibra/volumes/parcellationmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1198,15 +1198,15 @@
                 indices[regionname] = [{'volume': vol_idx, 'label': label}]
 
         # check for any remaining labels in the NIfTI volume
         unnamed_labels = list(set(labels_in_volume) - set(regionlabels))
         if unnamed_labels:
             logger.warning(
                 f"The following labels appear in the NIfTI volume {vol_idx}, but not in "
-                f"the specified regions: {', '.join(str(l) for l in unnamed_labels)}. "
+                f"the specified regions: {', '.join(str(lb) for lb in unnamed_labels)}. "
                 "They will be removed from the nifti volume."
             )
             for label in unnamed_labels:
                 arr[arr == label] = 0
         providers.extend(vol._providers.values())
 
     # parcellation
```

### Comparing `siibra-1.0a8/siibra/volumes/providers/__init__.py` & `siibra-1.0a9/siibra/volumes/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/volumes/providers/gifti.py` & `siibra-1.0a9/siibra/volumes/providers/gifti.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/volumes/providers/neuroglancer.py` & `siibra-1.0a9/siibra/volumes/providers/neuroglancer.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                 4, axis=0
             )
             num_conflicts += np.count_nonzero(result_arr[Xt, Yt, Zt])
             result_arr[Xt, Yt, Zt] = arr[Xs, Ys, Zs]
 
         if num_conflicts > 0:
             num_voxels = np.count_nonzero(result_arr)
-            logger.warning(f"Merging fragments required to overwrite {num_conflicts} conflicting voxels ({num_conflicts/num_voxels*100.:2.1f}%).")
+            logger.warning(f"Merging fragments required to overwrite {num_conflicts} conflicting voxels ({num_conflicts / num_voxels * 100.:2.1f}%).")
 
         return result
 
 
 class NeuroglancerVolume:
 
     USE_CACHE = False  # Whether to keep fetched data in local cache
```

### Comparing `siibra-1.0a8/siibra/volumes/providers/nifti.py` & `siibra-1.0a9/siibra/volumes/providers/nifti.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                 4, axis=0
             )
             num_conflicts += np.count_nonzero(result_arr[Xt, Yt, Zt])
             result_arr[Xt, Yt, Zt] = arr[Xs, Ys, Zs]
 
         if num_conflicts > 0:
             num_voxels = np.count_nonzero(result_arr)
-            logger.warning(f"Merging fragments required to overwrite {num_conflicts} conflicting voxels ({num_conflicts/num_voxels*100.:2.1f}%).")
+            logger.warning(f"Merging fragments required to overwrite {num_conflicts} conflicting voxels ({num_conflicts / num_voxels * 100.:2.1f}%).")
 
         return result
 
     def fetch(
         self,
         fragment: str = None,
         voi: _boundingbox.BoundingBox = None,
```

### Comparing `siibra-1.0a8/siibra/volumes/providers/provider.py` & `siibra-1.0a9/siibra/volumes/providers/provider.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/volumes/sparsemap.py` & `siibra-1.0a9/siibra/volumes/sparsemap.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra/volumes/volume.py` & `siibra-1.0a9/siibra/volumes/volume.py`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/siibra.egg-info/PKG-INFO` & `siibra-1.0a9/siibra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 1.0a8
+Version: 1.0a9
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `siibra-1.0a8/siibra.egg-info/SOURCES.txt` & `siibra-1.0a9/siibra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `siibra-1.0a8/test/test_siibra.py` & `siibra-1.0a9/test/test_siibra.py`

 * *Files identical despite different names*

