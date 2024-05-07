# Comparing `tmp/cleanlab-2.6.3.tar.gz` & `tmp/cleanlab-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-2.6.3.tar", last modified: Tue Mar 19 22:09:19 2024, max compression
+gzip compressed data, was "cleanlab-2.6.4.tar", last modified: Tue May  7 18:24:11 2024, max compression
```

## Comparing `cleanlab-2.6.3.tar` & `cleanlab-2.6.4.tar`

### file list

```diff
@@ -1,118 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.029919 cleanlab-2.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-03-19 22:09:12.000000 cleanlab-2.6.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-19 22:09:12.000000 cleanlab-2.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    21688 2024-03-19 22:09:12.000000 cleanlab-2.6.3/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (127)    34524 2024-03-19 22:09:12.000000 cleanlab-2.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 22:09:12.000000 cleanlab-2.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    63287 2024-03-19 22:09:19.029919 cleanlab-2.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21200 2024-03-19 22:09:12.000000 cleanlab-2.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.013919 cleanlab-2.6.3/cleanlab/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.017919 cleanlab-2.6.3/cleanlab/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17651 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/benchmarking/noise_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    53475 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    69505 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/count.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.017919 cleanlab-2.6.3/cleanlab/datalab/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/datalab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.017919 cleanlab-2.6.3/cleanlab/datalab/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.017919 cleanlab-2.6.3/cleanlab/datalab/internal/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/adapter/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8573 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/adapter/imagelab.py
--rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17301 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/data_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/helper_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    20222 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.021919 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/data_valuation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/imbalance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/issue_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.021919 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/multilabel/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/multilabel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/multilabel/label.py
--rw-r--r--   0 runner    (1001) docker     (127)    20218 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/noniid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/null.py
--rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/outlier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.021919 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/regression/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/regression/label.py
--rw-r--r--   0 runner    (1001) docker     (127)    15594 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/underperforming_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/model_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/datalab/internal/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    23957 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.021919 cleanlab-2.6.3/cleanlab/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/experimental/cifar_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/experimental/coteaching.py
--rw-r--r--   0 runner    (1001) docker     (127)    35575 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/experimental/label_issues_batched.py
--rw-r--r--   0 runner    (1001) docker     (127)    14113 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/experimental/mnist_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/experimental/span_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    43279 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.025919 cleanlab-2.6.3/cleanlab/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/label_quality_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14645 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/latent_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/multiannotator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24061 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/multilabel_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/multilabel_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/numerics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/object_detection_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/outlier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/regression_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/segmentation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/token_classification_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29055 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/internal/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.025919 cleanlab-2.6.3/cleanlab/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/models/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/models/keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    90505 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/multiannotator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.025919 cleanlab-2.6.3/cleanlab/multilabel_classification/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/multilabel_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/multilabel_classification/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    17287 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/multilabel_classification/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/multilabel_classification/rank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.029919 cleanlab-2.6.3/cleanlab/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/object_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19629 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/object_detection/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    48986 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/object_detection/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)    34063 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/object_detection/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    29078 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/outlier.py
--rw-r--r--   0 runner    (1001) docker     (127)    25824 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/rank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.029919 cleanlab-2.6.3/cleanlab/regression/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39296 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/regression/learn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/regression/rank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.029919 cleanlab-2.6.3/cleanlab/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/segmentation/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/segmentation/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/segmentation/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.029919 cleanlab-2.6.3/cleanlab/token_classification/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/token_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/token_classification/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/token_classification/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)    13905 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/token_classification/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9447 2024-03-19 22:09:12.000000 cleanlab-2.6.3/cleanlab/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:09:19.029919 cleanlab-2.6.3/cleanlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    63287 2024-03-19 22:09:18.000000 cleanlab-2.6.3/cleanlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-03-19 22:09:18.000000 cleanlab-2.6.3/cleanlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 22:09:18.000000 cleanlab-2.6.3/cleanlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-19 22:09:18.000000 cleanlab-2.6.3/cleanlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-19 22:09:18.000000 cleanlab-2.6.3/cleanlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-03-19 22:09:12.000000 cleanlab-2.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-19 22:09:19.033919 cleanlab-2.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-19 22:09:12.000000 cleanlab-2.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.791739 cleanlab-2.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-05-07 18:24:04.000000 cleanlab-2.6.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-07 18:24:04.000000 cleanlab-2.6.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21688 2024-05-07 18:24:04.000000 cleanlab-2.6.4/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34524 2024-05-07 18:24:04.000000 cleanlab-2.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 18:24:04.000000 cleanlab-2.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    63287 2024-05-07 18:24:11.791739 cleanlab-2.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21200 2024-05-07 18:24:04.000000 cleanlab-2.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.771739 cleanlab-2.6.4/cleanlab/
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.771739 cleanlab-2.6.4/cleanlab/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17651 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/benchmarking/noise_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53475 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69517 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/data_valuation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.775739 cleanlab-2.6.4/cleanlab/datalab/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/datalab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.775739 cleanlab-2.6.4/cleanlab/datalab/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.775739 cleanlab-2.6.4/cleanlab/datalab/internal/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/adapter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8573 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/adapter/imagelab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14317 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17301 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/data_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/helper_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20222 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.779739 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/data_valuation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/imbalance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.779739 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/multilabel/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/multilabel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/multilabel/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20403 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/noniid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/null.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/outlier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.779739 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/regression/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15788 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/underperforming_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/model_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24156 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.779739 cleanlab-2.6.4/cleanlab/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/cifar_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/coteaching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.779739 cleanlab-2.6.4/cleanlab/experimental/datalab/
+-rw-r--r--   0 runner    (1001) docker     (127)    18095 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/datalab/data_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35575 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/label_issues_batched.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14113 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/mnist_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/span_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43279 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.783738 cleanlab-2.6.4/cleanlab/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/label_quality_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14645 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/latent_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/multiannotator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23533 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/multilabel_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/multilabel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/numerics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/object_detection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/outlier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/regression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/segmentation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/token_classification_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29055 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.783738 cleanlab-2.6.4/cleanlab/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/models/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/models/keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90505 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/multiannotator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.783738 cleanlab-2.6.4/cleanlab/multilabel_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/multilabel_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/multilabel_classification/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17287 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/multilabel_classification/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/multilabel_classification/rank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.787739 cleanlab-2.6.4/cleanlab/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19629 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/object_detection/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49070 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/object_detection/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34427 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/object_detection/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30679 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/outlier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25824 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/rank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.787739 cleanlab-2.6.4/cleanlab/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39296 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/regression/learn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/regression/rank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.787739 cleanlab-2.6.4/cleanlab/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/segmentation/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/segmentation/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14450 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/segmentation/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.787739 cleanlab-2.6.4/cleanlab/token_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/token_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/token_classification/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/token_classification/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13905 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/token_classification/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9447 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.787739 cleanlab-2.6.4/cleanlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    63287 2024-05-07 18:24:11.000000 cleanlab-2.6.4/cleanlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-07 18:24:11.000000 cleanlab-2.6.4/cleanlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:24:11.000000 cleanlab-2.6.4/cleanlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 18:24:11.000000 cleanlab-2.6.4/cleanlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 18:24:11.000000 cleanlab-2.6.4/cleanlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-07 18:24:04.000000 cleanlab-2.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-07 18:24:11.791739 cleanlab-2.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 18:24:04.000000 cleanlab-2.6.4/setup.py
```

### Comparing `cleanlab-2.6.3/CODE_OF_CONDUCT.md` & `cleanlab-2.6.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/CONTRIBUTING.md` & `cleanlab-2.6.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/DEVELOPMENT.md` & `cleanlab-2.6.4/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/LICENSE` & `cleanlab-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/PKG-INFO` & `cleanlab-2.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab
-Version: 2.6.3
+Version: 2.6.4
 Summary: The standard package for data-centric AI, machine learning with label errors, and automatically finding and fixing dataset issues in Python.
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License: 
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -700,17 +700,17 @@
 Requires-Dist: termcolor>=2.4.0
 Provides-Extra: datalab
 Requires-Dist: datasets>=2.7.0; extra == "datalab"
 Provides-Extra: image
 Requires-Dist: datasets>=2.7.0; extra == "image"
 Requires-Dist: cleanvision>=0.3.6; extra == "image"
 Provides-Extra: all
-Requires-Dist: matplotlib>=3.5.1; extra == "all"
 Requires-Dist: cleanvision>=0.3.6; extra == "all"
 Requires-Dist: datasets>=2.7.0; extra == "all"
+Requires-Dist: matplotlib>=3.5.1; extra == "all"
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/cleanlab_logo_open_source.png" width=60% height=60%>
 </p>
 
 
 cleanlab helps you **clean** data and **lab**els by automatically detecting issues in a ML dataset. To facilitate **machine learning with messy, real-world data**, this data-centric AI package uses your *existing* models to estimate dataset problems that can be fixed to train even *better* models.
```

### Comparing `cleanlab-2.6.3/README.md` & `cleanlab-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/__init__.py` & `cleanlab-2.6.4/cleanlab/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/benchmarking/noise_generation.py` & `cleanlab-2.6.4/cleanlab/benchmarking/noise_generation.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/classification.py` & `cleanlab-2.6.4/cleanlab/classification.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/count.py` & `cleanlab-2.6.4/cleanlab/count.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,51 +24,48 @@
 
 These are estimated from a classification dataset. This module considers two types of datasets:
 
 * standard (multi-class) classification where each example is labeled as belonging to exactly one of K classes (e.g. ``labels = np.array([0,0,1,0,2,1])``)
 * multi-label classification where each example can be labeled as belonging to multiple classes (e.g. ``labels = [[1,2],[1],[0],[],...]``)
 """
 
+import warnings
+from typing import Optional, Tuple, Union
+
+import numpy as np
+import sklearn.base
 from sklearn.linear_model import LogisticRegression as LogReg
-from sklearn.model_selection import StratifiedKFold
 from sklearn.metrics import confusion_matrix
-import sklearn.base
-import numpy as np
-import warnings
-from typing import Tuple, Union, Optional
+from sklearn.model_selection import StratifiedKFold
 
-from cleanlab.typing import LabelLike
-from cleanlab.internal.multilabel_utils import stack_complement, get_onehot_num_classes
 from cleanlab.internal.constants import (
-    TINY_VALUE,
     CONFIDENT_THRESHOLDS_LOWER_BOUND,
     FLOATING_POINT_COMPARISON,
+    TINY_VALUE,
 )
-
+from cleanlab.internal.latent_algebra import (
+    compute_inv_noise_matrix,
+    compute_noise_matrix_from_inverse,
+    compute_py,
+)
+from cleanlab.internal.multilabel_utils import get_onehot_num_classes, stack_complement
 from cleanlab.internal.util import (
-    value_counts_fill_missing_classes,
-    clip_values,
-    clip_noise_rates,
-    round_preserving_row_totals,
     append_extra_datapoint,
-    train_val_split,
+    clip_noise_rates,
+    clip_values,
     get_num_classes,
     get_unique_classes,
-    is_torch_dataset,
     is_tensorflow_dataset,
+    is_torch_dataset,
+    round_preserving_row_totals,
+    train_val_split,
+    value_counts_fill_missing_classes,
 )
-from cleanlab.internal.latent_algebra import (
-    compute_inv_noise_matrix,
-    compute_py,
-    compute_noise_matrix_from_inverse,
-)
-from cleanlab.internal.validation import (
-    assert_valid_inputs,
-    labels_to_array,
-)
+from cleanlab.internal.validation import assert_valid_inputs, labels_to_array
+from cleanlab.typing import LabelLike
 
 
 def num_label_issues(
     labels: LabelLike,
     pred_probs: np.ndarray,
     *,
     confident_joint: Optional[np.ndarray] = None,
@@ -1454,15 +1451,15 @@
         # BIG_VALUE such that no valid prob >= BIG_VALUE (no example will be counted in missing classes)
         # REQUIRES: pred_probs.max() >= 1
         # TODO: if you want this to work for arbitrary softmax outputs where pred_probs.max()
         #  may exceed 1, change BIG_VALUE = 2 --> BIG_VALUE = 2 * pred_probs.max(). Downside of
         #  this approach is that there will be no standard value returned for missing classes.
         labels = labels_to_array(labels)
         all_classes = range(pred_probs.shape[1])
-        unique_classes = get_unique_classes(labels)
+        unique_classes = get_unique_classes(labels, multi_label=multi_label)
         BIG_VALUE = 2
         confident_thresholds = [
             np.mean(pred_probs[:, k][labels == k]) if k in unique_classes else BIG_VALUE
             for k in all_classes
         ]
         confident_thresholds = np.clip(
             confident_thresholds, a_min=CONFIDENT_THRESHOLDS_LOWER_BOUND, a_max=None
```

### Comparing `cleanlab-2.6.3/cleanlab/datalab/datalab.py` & `cleanlab-2.6.4/cleanlab/datalab/datalab.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/adapter/imagelab.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/adapter/imagelab.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/data.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,11 +380,11 @@
         if isinstance(label_name_feature, ClassLabel):
             label_map = {
                 label: label_name_feature.str2int(label) for label in label_name_feature.names
             }
             formatted_labels = labels
         else:
             label_map = {label: i for i, label in enumerate(np.unique(labels))}
-            formatted_labels = np.vectorize(label_map.get)(labels)
+            formatted_labels = np.vectorize(label_map.get, otypes=[int])(labels)
         inverse_map = {i: label for label, i in label_map.items()}
 
         return formatted_labels, inverse_map
```

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/data_issues.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/data_issues.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/display.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/display.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/helper_factory.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/helper_factory.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/issue_finder.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/issue_finder.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/data_valuation.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/data_valuation.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,30 +14,33 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from typing import (
     TYPE_CHECKING,
     Any,
+    Callable,
     ClassVar,
     Dict,
     List,
     Optional,
     Union,
 )
 import warnings
 
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import csr_matrix
+from scipy.spatial.distance import euclidean
 from sklearn.exceptions import NotFittedError
 from sklearn.neighbors import NearestNeighbors
 from sklearn.utils.validation import check_is_fitted
 
+from cleanlab.data_valuation import data_shapley_knn
 from cleanlab.datalab.internal.issue_manager import IssueManager
 
 if TYPE_CHECKING:  # pragma: no cover
     import numpy.typing as npt
     import pandas as pd
     from cleanlab.datalab.datalab import Datalab
 
@@ -96,15 +99,15 @@
     }
 
     DEFAULT_THRESHOLD = 0.5
 
     def __init__(
         self,
         datalab: Datalab,
-        metric: Optional[str] = None,
+        metric: Optional[Union[str, Callable]] = None,
         threshold: Optional[float] = None,
         k: int = 10,
         **kwargs,
     ):
         super().__init__(datalab)
         self.metric = metric
         self.k = k
@@ -137,15 +140,19 @@
             raise TypeError(error_msg)
         if knn_graph is None or metric_changes:
             if features is None:
                 raise ValueError(
                     "If a knn_graph is not provided, features must be provided to fit a new knn."
                 )
             if self.metric is None:
-                self.metric = "cosine" if features.shape[1] > 3 else "euclidean"
+                self.metric = (
+                    "cosine"
+                    if features.shape[1] > 3
+                    else "euclidean" if features.shape[0] > 100 else euclidean
+                )
             knn = NearestNeighbors(n_neighbors=self.k, metric=self.metric).fit(features)
 
             if self.metric and self.metric != knn.metric:
                 warnings.warn(
                     f"Metric {self.metric} does not match metric {knn.metric} used to fit knn. "
                     "Most likely an existing NearestNeighbors object was passed in, but a different "
                     "metric was specified."
@@ -154,18 +161,16 @@
 
             try:
                 check_is_fitted(knn)
             except NotFittedError:
                 knn.fit(features)
 
             knn_graph = knn.kneighbors_graph(mode="distance")
-        if labels is None:
-            raise ValueError("labels must be provided to run data valuation")
 
-        scores = _knn_shapley_score(knn_graph, labels, self.k)
+        scores = data_shapley_knn(labels, knn_graph=knn_graph, k=self.k)
 
         self.issues = pd.DataFrame(
             {
                 f"is_{self.issue_name}_issue": scores < self.threshold,
                 self.issue_score_key: scores,
             },
         )
@@ -227,23 +232,7 @@
         )
         if prefer_new_graph:
             statistics_dict["statistics"][graph_key] = knn_graph
             if self.metric is not None:
                 statistics_dict["statistics"]["knn_metric"] = self.metric
 
         return statistics_dict
-
-
-def _knn_shapley_score(knn_graph: csr_matrix, labels: np.ndarray, k: int) -> np.ndarray:
-    """Compute the Shapley values of data points based on a knn graph."""
-    N = labels.shape[0]
-    scores = np.zeros((N, N))
-    dist = knn_graph.indices.reshape(N, -1)
-
-    for y, s, dist_i in zip(labels, scores, dist):
-        idx = dist_i[::-1]
-        ans = labels[idx]
-        s[idx[k - 1]] = float(ans[k - 1] == y)
-        ans_matches = (ans == y).flatten()
-        for j in range(k - 2, -1, -1):
-            s[idx[j]] = s[idx[j + 1]] + float(int(ans_matches[j]) - int(ans_matches[j + 1]))
-    return 0.5 * (np.mean(scores / k, axis=0) + 1)
```

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/duplicate.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/duplicate.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, ClassVar, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Dict, List, Optional, Union
 import warnings
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import csr_matrix
+from scipy.spatial.distance import euclidean
 from sklearn.neighbors import NearestNeighbors
 from sklearn.exceptions import NotFittedError
 from sklearn.utils.validation import check_is_fitted
 
 from cleanlab.datalab.internal.issue_manager import IssueManager
+from cleanlab.internal.constants import EPSILON
 
 if TYPE_CHECKING:  # pragma: no cover
     import numpy.typing as npt
     from cleanlab.datalab.datalab import Datalab
 
 
 class NearDuplicateIssueManager(IssueManager):
@@ -49,15 +51,15 @@
         1: [],
         2: ["threshold"],
     }
 
     def __init__(
         self,
         datalab: Datalab,
-        metric: Optional[str] = None,
+        metric: Optional[Union[str, Callable]] = None,
         threshold: float = 0.13,
         k: int = 10,
         **_,
     ):
         super().__init__(datalab)
         self.metric = metric
         self.threshold = self._set_threshold(threshold)
@@ -75,15 +77,19 @@
 
         if knn_graph is None or metric_changes:
             if features is None:
                 raise ValueError(
                     "If a knn_graph is not provided, features must be provided to fit a new knn."
                 )
             if self.metric is None:
-                self.metric = "cosine" if features.shape[1] > 3 else "euclidean"
+                self.metric = (
+                    "cosine"
+                    if features.shape[1] > 3
+                    else "euclidean" if features.shape[0] > 100 else euclidean
+                )
             knn = NearestNeighbors(n_neighbors=self.k, metric=self.metric)
 
             if self.metric and self.metric != knn.metric:
                 warnings.warn(
                     f"Metric {self.metric} does not match metric {knn.metric} used to fit knn. "
                     "Most likely an existing NearestNeighbors object was passed in, but a different "
                     "metric was specified."
@@ -94,17 +100,15 @@
                 check_is_fitted(knn)
             except NotFittedError:
                 knn.fit(features)
 
             knn_graph = knn.kneighbors_graph(mode="distance")
         N = knn_graph.shape[0]
         nn_distances = knn_graph.data.reshape(N, -1)[:, 0]
-        median_nn_distance = max(
-            np.median(nn_distances), 100 * np.finfo(np.float_).eps
-        )  # avoid threshold = 0
+        median_nn_distance = max(np.median(nn_distances), EPSILON)  # avoid threshold = 0
         self.near_duplicate_sets = self._neighbors_within_radius(
             knn_graph, self.threshold, median_nn_distance
         )
 
         # Flag every example in a near-duplicate set as a near-duplicate issue
         all_near_duplicates = np.unique(np.concatenate(self.near_duplicate_sets))
         is_issue_column = np.zeros(N, dtype=bool)
```

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/imbalance.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/imbalance.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     issue_name: ClassVar[str] = "class_imbalance"
     verbosity_levels = {
         0: ["Rarest Class"],
         1: [],
         2: [],
     }
 
-    def __init__(self, datalab: Datalab, threshold: float = 0.1):
+    def __init__(self, datalab: Datalab, threshold: float = 0.1, **_):
         super().__init__(datalab)
         self.threshold = threshold
 
     def find_issues(
         self,
         **kwargs,
     ) -> None:
```

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/issue_manager.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/label.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/label.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, Optional
 
+import numpy as np
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.preprocessing import OneHotEncoder
 
-import numpy as np
-
 from cleanlab.classification import CleanLearning
+from cleanlab.count import get_confident_thresholds
 from cleanlab.datalab.internal.issue_manager import IssueManager
 from cleanlab.internal.validation import assert_valid_inputs
 
 if TYPE_CHECKING:  # pragma: no cover
-    import pandas as pd
     import numpy.typing as npt
+    import pandas as pd
+
     from cleanlab.datalab.datalab import Datalab
 
 
 class LabelIssueManager(IssueManager):
     """Manages label issues in a Datalab.
 
     Parameters
@@ -75,25 +76,26 @@
     ):
         super().__init__(datalab)
         self.cl = CleanLearning(**(clean_learning_kwargs or {}))
         self.k = k
         self.health_summary_parameters: Dict[str, Any] = (
             health_summary_parameters.copy() if health_summary_parameters else {}
         )
+        self._find_issues_inputs: Dict[str, bool] = {"features": False, "pred_probs": False}
         self._reset()
 
     @staticmethod
-    def _process_find_label_issues_kwargs(kwargs: Dict[str, Any]) -> Dict[str, Any]:
+    def _process_find_label_issues_kwargs(**kwargs) -> Dict[str, Any]:
         """Searches for keyword arguments that are meant for the
         CleanLearning.find_label_issues method call
 
         Examples
         --------
         >>> from cleanlab.datalab.internal.issue_manager.label import LabelIssueManager
-        >>> LabelIssueManager._process_clean_learning_kwargs(thresholds=[0.1, 0.9])
+        >>> LabelIssueManager._process_find_label_issues_kwargs(thresholds=[0.1, 0.9])
         {'thresholds': [0.1, 0.9]}
         """
         accepted_kwargs = [
             "thresholds",
             "noise_matrix",
             "inverse_noise_matrix",
             "save_space",
@@ -137,15 +139,18 @@
         ----------
         pred_probs :
             The predicted probabilities for each example.
 
         features :
             The features for each example.
         """
+        if pred_probs is not None:
+            self._find_issues_inputs.update({"pred_probs": True})
         if pred_probs is None:
+            self._find_issues_inputs.update({"features": True})
             if features is None:
                 raise ValueError(
                     "Either pred_probs or features must be provided to find label issues."
                 )
             # produce out-of-sample pred_probs from features
             labels = self.datalab.labels
             if not isinstance(labels, np.ndarray):
@@ -166,28 +171,34 @@
             # adjust pred_probs so it is out-of-sample
             pred_probs = np.asarray(
                 (pred_probs - 1 / (self.k + 1) * one_hot_label) * (self.k + 1) / self.k
             )
 
         self.health_summary_parameters.update({"pred_probs": pred_probs})
         # Find examples with label issues
+        labels = self.datalab.labels
         self.issues = self.cl.find_label_issues(
-            labels=self.datalab.labels,
+            labels=labels,
             pred_probs=pred_probs,
-            **self._process_find_label_issues_kwargs(kwargs),
+            **self._process_find_label_issues_kwargs(**kwargs),
         )
         self.issues.rename(columns={"label_quality": self.issue_score_key}, inplace=True)
 
         summary_dict = self.get_health_summary(pred_probs=pred_probs)
 
         # Get a summarized dataframe of the label issues
         self.summary = self.make_summary(score=summary_dict["overall_label_health_score"])
 
+        confident_thresholds = get_confident_thresholds(labels=labels, pred_probs=pred_probs)
         # Collect info about the label issues
-        self.info = self.collect_info(issues=self.issues, summary_dict=summary_dict)
+        self.info = self.collect_info(
+            issues=self.issues,
+            summary_dict=summary_dict,
+            confident_thresholds=confident_thresholds,
+        )
 
         # Drop columns from issues that are in the info
         self.issues = self.issues.drop(columns=["given_label", "predicted_label"])
 
     def get_health_summary(self, pred_probs) -> dict:
         """Returns a short summary of the health of this Lab."""
         from cleanlab.dataset import health_summary
@@ -237,15 +248,17 @@
             if k in self.health_summary_parameters:
                 summary_parameters[k] = self.health_summary_parameters[k]
 
         return (
             summary_parameters  # will be called in `dataset.health_summary(**summary_parameters)`
         )
 
-    def collect_info(self, issues: pd.DataFrame, summary_dict: dict) -> dict:
+    def collect_info(
+        self, issues: pd.DataFrame, summary_dict: dict, confident_thresholds: np.ndarray
+    ) -> dict:
         issues_info = {
             "num_label_issues": sum(issues[f"is_{self.issue_name}_issue"]),
             "average_label_quality": issues[self.issue_score_key].mean(),
             "given_label": issues["given_label"].tolist(),
             "predicted_label": issues["predicted_label"].tolist(),
         }
 
@@ -261,13 +274,15 @@
                 continue
             cl_info[k] = self.cl.__dict__[k]
 
         info_dict = {
             **issues_info,
             **health_summary_info,
             **cl_info,
+            "confident_thresholds": confident_thresholds.tolist(),
+            "find_issues_inputs": self._find_issues_inputs,
         }
 
         return info_dict
 
     def _validate_pred_probs(self, pred_probs) -> None:
         assert_valid_inputs(X=None, y=self.datalab.labels, pred_probs=pred_probs)
```

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/multilabel/label.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/multilabel/label.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,22 +15,23 @@
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, List
 
 import pandas as pd
 
-from cleanlab.multilabel_classification.filter import find_label_issues
-from cleanlab.multilabel_classification.rank import get_label_quality_scores
 from cleanlab.datalab.internal.issue_manager import IssueManager
 from cleanlab.internal.multilabel_utils import onehot2int
+from cleanlab.multilabel_classification.filter import find_label_issues
+from cleanlab.multilabel_classification.rank import get_label_quality_scores
 
 if TYPE_CHECKING:  # pragma: no cover
-    import pandas as pd
     import numpy.typing as npt
+    import pandas as pd
+
     from cleanlab.datalab.datalab import Datalab
 
 
 class MultilabelIssueManager(IssueManager):
     """Manages label issues in Datalab for multilabel tasks.
 
     Parameters
@@ -60,50 +61,48 @@
         self,
         datalab: Datalab,
         **_,
     ):
         super().__init__(datalab)
 
     @staticmethod
-    def _process_find_label_issues_kwargs(kwargs: Dict[str, Any]) -> Dict[str, Any]:
+    def _process_find_label_issues_kwargs(**kwargs: Dict[str, Any]) -> Dict[str, Any]:
         """Searches for keyword arguments that are meant for the
         multilabel_classification.filter.find_label_issues method call.
 
         Examples
         --------
         >>> from cleanlab.datalab.internal.issue_manager.multilabel.label import MultilabelIssueManager
         >>> MultilabelIssueManager._process_find_label_issues_kwargs(frac_noise=0.9)
-        {'frac_noise': 0.1}
+        {'frac_noise': 0.9}
         """
-        accepted_kwargs = (
-            [
-                "filter_by",
-                "frac_noise",
-                "num_to_remove_per_class",
-                "min_examples_per_class",
-                "confident_joint",
-                "n_jobs",
-                "verbose",
-                "low_memory",
-            ],
-        )
+        accepted_kwargs = [
+            "filter_by",
+            "frac_noise",
+            "num_to_remove_per_class",
+            "min_examples_per_class",
+            "confident_joint",
+            "n_jobs",
+            "verbose",
+            "low_memory",
+        ]
         return {k: v for k, v in kwargs.items() if k in accepted_kwargs and v is not None}
 
     @staticmethod
-    def _process_get_label_quality_scores_kwargs(kwargs: Dict[str, Any]) -> Dict[str, Any]:
+    def _process_get_label_quality_scores_kwargs(**kwargs: Dict[str, Any]) -> Dict[str, Any]:
         """Searches for keyword arguments that are meant for the
         multilabel_classification.rank.get_label_quality_scores method call.
 
         Examples
         --------
         >>> from cleanlab.datalab.internal.issue_manager.multilabel.label import MultilabelIssueManager
         >>> MultilabelIssueManager._process_get_label_quality_scores_kwargs(method="self_confidence")
-        {'method': "self_confidence"}
+        {'method': 'self_confidence'}
         """
-        accepted_kwargs = (["method", "adjust_pred_probs", "aggregator_kwargs"],)
+        accepted_kwargs = ["method", "adjust_pred_probs", "aggregator_kwargs"]
         return {k: v for k, v in kwargs.items() if k in accepted_kwargs and v is not None}
 
     def find_issues(
         self,
         pred_probs: npt.NDArray,
         **kwargs,
     ) -> None:
@@ -117,20 +116,20 @@
         predicted_labels = onehot2int(pred_probs > self._PREDICTED_LABEL_THRESH)
 
         # Find examples with label issues
         assert isinstance(self.datalab.labels, List)  # Type Narrowing
         is_issue_column = find_label_issues(
             labels=self.datalab.labels,
             pred_probs=pred_probs,
-            **self._process_find_label_issues_kwargs(kwargs),
+            **self._process_find_label_issues_kwargs(**kwargs),
         )
         scores = get_label_quality_scores(
             labels=self.datalab.labels,
             pred_probs=pred_probs,
-            **self._process_get_label_quality_scores_kwargs(kwargs),
+            **self._process_get_label_quality_scores_kwargs(**kwargs),
         )
 
         self.issues = pd.DataFrame(
             {
                 f"is_{self.issue_name}_issue": is_issue_column,
                 self.issue_score_key: scores,
             },
@@ -139,15 +138,13 @@
         self.summary = self.make_summary(score=scores.mean())
 
         # Collect info about the label issues
         self.info = self.collect_info(self.datalab.labels, predicted_labels)
 
     def collect_info(
         self, given_labels: List[List[int]], predicted_labels: List[List[int]]
-    ) -> dict:
+    ) -> Dict[str, Any]:
         issues_info = {
             "given_label": given_labels,
             "predicted_label": predicted_labels,
         }
-        info_dict = {**issues_info}
-
-        return info_dict
+        return issues_info
```

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/noniid.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/noniid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, ClassVar, Dict, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Dict, Optional, Union, cast
 import warnings
 import itertools
 
 from scipy.stats import gaussian_kde
 import numpy as np
 import pandas as pd
 from scipy.sparse import csr_matrix
+from scipy.spatial.distance import euclidean
 from sklearn.neighbors import NearestNeighbors
 from sklearn.exceptions import NotFittedError
 from sklearn.utils.validation import check_is_fitted
 
 from cleanlab.datalab.internal.issue_manager import IssueManager
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -102,15 +103,15 @@
         1: [],
         2: [],
     }
 
     def __init__(
         self,
         datalab: Datalab,
-        metric: Optional[str] = None,
+        metric: Optional[Union[str, Callable]] = None,
         k: int = 10,
         num_permutations: int = 25,
         seed: Optional[int] = 0,
         significance_threshold: float = 0.05,
         **_,
     ):
         super().__init__(datalab)
@@ -199,15 +200,19 @@
             self._skip_storing_knn_graph_for_pred_probs = True
 
         if knn_graph is not None and not metric_changes:
             return None
         features_to_use = self._determine_features(features, pred_probs)
 
         if self.metric is None:
-            self.metric = "cosine" if features_to_use.shape[1] > 3 else "euclidean"
+            self.metric = (
+                "cosine"
+                if features_to_use.shape[1] > 3
+                else "euclidean" if features_to_use.shape[0] > 100 else euclidean
+            )
 
         knn = NearestNeighbors(n_neighbors=self.k, metric=self.metric)
 
         if self.metric != knn.metric:
             warnings.warn(
                 f"Metric {self.metric} does not match metric {knn.metric} used to fit knn. "
                 "Most likely an existing NearestNeighbors object was passed in, but a different "
```

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/null.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/null.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/outlier.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/outlier.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,14 +83,19 @@
             ood_kwargs["params"] = params
 
         self.ood: OutOfDistribution = OutOfDistribution(**ood_kwargs)
 
         self.threshold = threshold
         self._embeddings: Optional[np.ndarray] = None
         self._metric: str = None  # type: ignore
+        self._find_issues_inputs: Dict[str, bool] = {
+            "features": False,
+            "pred_probs": False,
+            "knn_graph": False,
+        }
 
     def find_issues(
         self,
         features: Optional[npt.NDArray] = None,
         pred_probs: Optional[np.ndarray] = None,
         **kwargs,
     ) -> None:
@@ -101,21 +106,24 @@
             N = knn_graph.shape[0]
             k = knn_graph.nnz // N
             t = cast(int, self.ood.params["t"])
             distances = knn_graph.data.reshape(-1, k)
             assert isinstance(distances, np.ndarray)
             avg_distances = distances.mean(axis=1)
             median_avg_distance = np.median(avg_distances)
+            self._find_issues_inputs.update({"knn_graph": True})
             scores = transform_distances_to_scores(
                 avg_distances, t=t, scaling_factor=median_avg_distance
             )
         elif features is not None:
             scores = self._score_with_features(features, **kwargs)
+            self._find_issues_inputs.update({"features": True})
         elif pred_probs is not None:
             scores = self._score_with_pred_probs(pred_probs, **kwargs)
+            self._find_issues_inputs.update({"pred_probs": True})
         else:
             if kwargs.get("knn_graph", None) is not None:
                 raise ValueError(
                     "knn_graph is provided, but not sufficiently large to compute the scores based on the provided hyperparameters."
                 )
             raise ValueError(f"Either features pred_probs must be provided.")
 
@@ -126,36 +134,40 @@
                 ), "features must be provided so that we can compute the knn graph."
                 knn_graph = self._process_knn_graph_from_features(kwargs)
             distances = knn_graph.data.reshape(knn_graph.shape[0], -1)
 
             assert isinstance(distances, np.ndarray)
             (
                 self.threshold,
+                issue_threshold,  # Useful info for detecting issues in test data
                 is_issue_column,
             ) = self._compute_threshold_and_issue_column_from_distances(distances, self.threshold)
 
         else:
             assert pred_probs is not None
             # Threshold based on pred_probs, very small scores are outliers
             if self.threshold is None:
                 self.threshold = self.DEFAULT_THRESHOLDS["pred_probs"]
             if not 0 <= self.threshold:
                 raise ValueError(f"threshold must be non-negative, but got {self.threshold}.")
-            is_issue_column = scores < self.threshold * np.median(scores)
+            issue_threshold = float(
+                self.threshold * np.median(scores)
+            )  # Useful info for detecting issues in test data
+            is_issue_column = scores < issue_threshold
 
         self.issues = pd.DataFrame(
             {
                 f"is_{self.issue_name}_issue": is_issue_column,
                 self.issue_score_key: scores,
             },
         )
 
         self.summary = self.make_summary(score=scores.mean())
 
-        self.info = self.collect_info(knn_graph=knn_graph)
+        self.info = self.collect_info(issue_threshold=issue_threshold, knn_graph=knn_graph)
 
     def _process_knn_graph_from_inputs(self, kwargs: Dict[str, Any]) -> Union[csr_matrix, None]:
         """Determine if a knn_graph is provided in the kwargs or if one is already stored in the associated Datalab instance."""
         knn_graph_kwargs: Optional[csr_matrix] = kwargs.get("knn_graph", None)
         knn_graph_stats = self.datalab.get_info("statistics").get("weighted_knn_graph", None)
 
         knn_graph: Optional[csr_matrix] = None
@@ -170,26 +182,32 @@
             # If the provided knn graph is insufficient, then we need to recompute the knn graph
             # with the provided features
             knn_graph = None
         return knn_graph
 
     def _compute_threshold_and_issue_column_from_distances(
         self, distances: np.ndarray, threshold: Optional[float] = None
-    ) -> Tuple[float, np.ndarray]:
+    ) -> Tuple[float, float, np.ndarray]:
         avg_distances = distances.mean(axis=1)
         if threshold:
             if not (isinstance(threshold, (int, float)) and 0 <= threshold <= 1):
                 raise ValueError(
                     f"threshold must be a number between 0 and 1, got {threshold} of type {type(threshold)}."
                 )
         if threshold is None:
             threshold = OutlierIssueManager.DEFAULT_THRESHOLDS["features"]
-        q3_distance = np.percentile(avg_distances, 75)
-        iqr_scale = 1 / threshold - 1 if threshold != 0 else np.inf
-        return threshold, avg_distances > q3_distance + iqr_scale * iqr(avg_distances)
+
+        def compute_issue_threshold(avg_distances: np.ndarray, threshold: float) -> float:
+            q3_distance = np.percentile(avg_distances, 75)
+            iqr_scale = 1 / threshold - 1 if threshold != 0 else np.inf
+            issue_threshold = q3_distance + iqr_scale * iqr(avg_distances)
+            return float(issue_threshold)
+
+        issue_threshold = compute_issue_threshold(avg_distances, threshold)
+        return threshold, issue_threshold, avg_distances > issue_threshold
 
     def _process_knn_graph_from_features(self, kwargs: Dict) -> csr_matrix:
         # Check if the weighted knn graph exists in info
         knn_graph = self.datalab.get_info("statistics").get("weighted_knn_graph", None)
 
         # Used to check if the knn graph needs to be recomputed, already set in the knn object
         k: int = 0
@@ -202,18 +220,24 @@
             # then we need to recompute the knn graph
             assert knn == self.ood.params["knn"]  # type: ignore[union-attr]
             knn_graph = knn.kneighbors_graph(mode="distance")  # type: ignore[union-attr]
             self._metric = knn.metric  # type: ignore[union-attr]
 
         return knn_graph
 
-    def collect_info(self, *, knn_graph: Optional[csr_matrix] = None) -> dict:
+    def collect_info(
+        self,
+        *,
+        issue_threshold: float,
+        knn_graph: Optional[csr_matrix] = None,
+    ) -> dict:
         issues_dict = {
             "average_ood_score": self.issues[self.issue_score_key].mean(),
             "threshold": self.threshold,
+            "issue_threshold": issue_threshold,
         }
         pred_probs_issues_dict: Dict[str, Any] = {}
         feature_issues_dict = {}
 
         if knn_graph is not None:
             knn = self.ood.params["knn"]  # type: ignore
             N = knn_graph.shape[0]
@@ -231,24 +255,28 @@
             if self.ood.params["knn"] is not None:
                 knn = self.ood.params["knn"]
                 feature_issues_dict.update({"metric": knn.metric})  # type: ignore[union-attr]
 
         if self.ood.params["confident_thresholds"] is not None:
             pass  #
         statistics_dict = self._build_statistics_dictionary(knn_graph=knn_graph)
-        ood_params_dict = self.ood.params
+        ood_params_dict = {
+            "ood": self.ood,
+            **self.ood.params,
+        }
         knn_dict = {
             **pred_probs_issues_dict,
             **feature_issues_dict,
         }
         info_dict: Dict[str, Any] = {
             **issues_dict,
             **ood_params_dict,  # type: ignore[arg-type]
             **knn_dict,
             **statistics_dict,
+            "find_issues_inputs": self._find_issues_inputs,
         }
         return info_dict
 
     def _build_statistics_dictionary(
         self, *, knn_graph: Optional[csr_matrix]
     ) -> Dict[str, Dict[str, Any]]:
         statistics_dict: Dict[str, Dict[str, Any]] = {"statistics": {}}
```

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/regression/label.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/regression/label.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager/underperforming_group.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/underperforming_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, ClassVar, Dict, Optional, Union, Tuple
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Dict, Optional, Union, Tuple
 import warnings
 import inspect
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import csr_matrix
+from scipy.spatial.distance import euclidean
 from sklearn.neighbors import NearestNeighbors
 from sklearn.exceptions import NotFittedError
 from sklearn.utils.validation import check_is_fitted
 from sklearn.cluster import DBSCAN
 
 from cleanlab.datalab.internal.issue_manager import IssueManager
 from cleanlab.rank import get_self_confidence_for_each_label
@@ -75,15 +76,15 @@
     """Specifies labels considered as outliers by the clustering algorithm."""
     NO_UNDERPERFORMING_CLUSTER_ID: ClassVar[int] = min(OUTLIER_CLUSTER_LABELS) - 1
     """Constant to signify absence of any underperforming cluster."""
 
     def __init__(
         self,
         datalab: Datalab,
-        metric: Optional[str] = None,
+        metric: Optional[Union[str, Callable]] = None,
         threshold: float = 0.1,
         k: int = 10,
         clustering_kwargs: Dict[str, Any] = {},
         min_cluster_samples: int = 5,
         **_: Any,
     ):
         super().__init__(datalab)
@@ -153,15 +154,19 @@
 
         if knn_graph is None or metric_changes:
             if features is None:
                 raise ValueError(
                     "If a knn_graph is not provided, features must be provided to fit a new knn."
                 )
             if self.metric is None:
-                self.metric = "cosine" if features.shape[1] > 3 else "euclidean"
+                self.metric = (
+                    "cosine"
+                    if features.shape[1] > 3
+                    else "euclidean" if features.shape[0] > 100 else euclidean
+                )
             knn = NearestNeighbors(n_neighbors=self.k, metric=self.metric)
 
             if self.metric and self.metric != knn.metric:
                 warnings.warn(
                     f"Metric {self.metric} does not match metric {knn.metric} used to fit knn. "
                     "Most likely an existing NearestNeighbors object was passed in, but a different "
                     "metric was specified."
```

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/issue_manager_factory.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager_factory.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/model_outputs.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/model_outputs.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/report.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/report.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/serialize.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/serialize.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/datalab/internal/task.py` & `cleanlab-2.6.4/cleanlab/datalab/internal/task.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/dataset.py` & `cleanlab-2.6.4/cleanlab/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 which classes to remove (see `~cleanlab.dataset.rank_classes_by_label_quality`)
 and which classes to merge (see `~cleanlab.dataset.find_overlapping_classes`).
 """
 
 from typing import Optional, cast
 import numpy as np
 import pandas as pd
+
 from cleanlab.count import estimate_joint, num_label_issues
+from cleanlab.internal.constants import EPSILON
 
 
 def rank_classes_by_label_quality(
     labels=None,
     pred_probs=None,
     *,
     class_names=None,
@@ -96,16 +98,20 @@
             pred_probs=pred_probs,
             confident_joint=confident_joint,
         )
     if num_examples is None:
         num_examples = _get_num_examples(labels=labels)
     given_label_noise = joint.sum(axis=1) - joint.diagonal()  # p(s=k) - p(s=k,y=k) = p(y!=k, s=k)
     true_label_noise = joint.sum(axis=0) - joint.diagonal()  # p(y=k) - p(s=k,y=k) = p(s!=k,y=k)
-    given_conditional_noise = given_label_noise / joint.sum(axis=1)  # p(y!=k, s=k) / p(s=k)
-    true_conditional_noise = true_label_noise / joint.sum(axis=0)  # p(s!=k, y=k) / p(y=k)
+    given_conditional_noise = given_label_noise / np.clip(
+        joint.sum(axis=1), a_min=EPSILON, a_max=None
+    )  # p(y!=k, s=k) / p(s=k) , avoiding division by 0
+    true_conditional_noise = true_label_noise / np.clip(
+        joint.sum(axis=0), a_min=EPSILON, a_max=None
+    )  # p(s!=k, y=k) / p(y=k) , avoiding division by 0
     df = pd.DataFrame(
         {
             "Class Index": np.arange(len(joint)),
             "Label Issues": (given_label_noise * num_examples).round().astype(int),
             "Inverse Label Issues": (true_label_noise * num_examples).round().astype(int),
             "Label Noise": given_conditional_noise,  # p(y!=k | s=k)
             "Inverse Label Noise": true_conditional_noise,  # p(s!=k | y=k)
```

### Comparing `cleanlab-2.6.3/cleanlab/experimental/cifar_cnn.py` & `cleanlab-2.6.4/cleanlab/experimental/cifar_cnn.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/experimental/coteaching.py` & `cleanlab-2.6.4/cleanlab/experimental/coteaching.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/experimental/label_issues_batched.py` & `cleanlab-2.6.4/cleanlab/experimental/label_issues_batched.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/experimental/mnist_pytorch.py` & `cleanlab-2.6.4/cleanlab/experimental/mnist_pytorch.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/experimental/span_classification.py` & `cleanlab-2.6.4/cleanlab/experimental/span_classification.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/filter.py` & `cleanlab-2.6.4/cleanlab/filter.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/internal/constants.py` & `cleanlab-2.6.4/cleanlab/internal/constants.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/internal/label_quality_utils.py` & `cleanlab-2.6.4/cleanlab/internal/label_quality_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/internal/latent_algebra.py` & `cleanlab-2.6.4/cleanlab/internal/latent_algebra.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/internal/multiannotator_utils.py` & `cleanlab-2.6.4/cleanlab/internal/multiannotator_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/internal/multilabel_scorer.py` & `cleanlab-2.6.4/cleanlab/internal/multilabel_scorer.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,21 +18,22 @@
 """
 
 from enum import Enum
 from typing import Callable, Dict, Optional, Union
 
 import numpy as np
 from sklearn.model_selection import cross_val_predict
-from cleanlab.internal.multilabel_utils import _is_multilabel, stack_complement
+
 from cleanlab.internal.label_quality_utils import _subtract_confident_thresholds
+from cleanlab.internal.multilabel_utils import _is_multilabel, stack_complement
 from cleanlab.internal.numerics import softmax
 from cleanlab.rank import (
-    get_self_confidence_for_each_label,
-    get_normalized_margin_for_each_label,
     get_confidence_weighted_entropy_for_each_label,
+    get_normalized_margin_for_each_label,
+    get_self_confidence_for_each_label,
 )
 
 
 class _Wrapper:
     """Helper class for wrapping callable functions as attributes of an Enum instead of
     setting them as methods of the Enum class.
 
@@ -594,35 +595,26 @@
            [0.5, 0.5]])
     >>> y = np.array([[0, 0], [0, 1], [1, 0], [1, 0], [1, 0]])
     >>> multilabel_py(y)
     array([[0.4, 0.6],
            [0.8, 0.2]])
     """
 
-    def compute_class_py(y_slice: np.ndarray) -> np.ndarray:
-        # Should only consider a single class at a time
-        assert y_slice.ndim == 1
-        unique_values, counts = np.unique(y_slice, axis=0, return_counts=True)
-        N = y_slice.shape[0]
-        if len(unique_values) == 1:
-            # Should be 0 and 1, pad with 0 probability if either is missing.
-            counts = np.array([0, N] if unique_values[0] == 1 else [N, 0])
-        return counts / N
-
-    py = np.apply_along_axis(compute_class_py, axis=1, arr=y.T)
+    N, _ = y.shape
+    fraction_0 = np.sum(y == 0, axis=0) / N
+    fraction_1 = 1 - fraction_0
+    py = np.column_stack((fraction_0, fraction_1))
     return py
 
 
 # Cross-validation helpers
 
 
 def _get_split_generator(labels, cv):
-    unique_labels = np.unique(labels, axis=0)
-    label_to_index = {tuple(label): i for i, label in enumerate(unique_labels)}
-    multilabel_ids = np.array([label_to_index[tuple(label)] for label in labels])
+    _, multilabel_ids = np.unique(labels, axis=0, return_inverse=True)
     split_generator = cv.split(X=multilabel_ids, y=multilabel_ids)
     return split_generator
 
 
 def get_cross_validated_multilabel_pred_probs(X, labels: np.ndarray, *, clf, cv) -> np.ndarray:
     """Get predicted probabilities for a multi-label classifier via cross-validation.
```

### Comparing `cleanlab-2.6.3/cleanlab/internal/multilabel_utils.py` & `cleanlab-2.6.4/cleanlab/internal/multilabel_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 Helper functions used internally for multi-label classification tasks.
 """
-from typing import Tuple, Optional, List
+from typing import List, Optional, Tuple
 
 import numpy as np
 
 from cleanlab.internal.util import get_num_classes
 
 
 def _is_multilabel(y: np.ndarray) -> bool:
@@ -98,8 +98,8 @@
 
     Returns
     -------
     labels: list of lists of integers
       e.g. [[0,1], [3], [1,2,3], [1], [2]]
       All integers from 0,1,...,K-1 must be represented."""
 
-    return [list(np.where(row == 1)[0]) for row in onehot_matrix]
+    return [np.where(row)[0].tolist() for row in onehot_matrix]
```

### Comparing `cleanlab-2.6.3/cleanlab/internal/numerics.py` & `cleanlab-2.6.4/cleanlab/internal/numerics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Optional
 import numpy as np
 
+from cleanlab.internal.constants import EPSILON
+
 
 def softmax(
     x: np.ndarray, temperature: float = 1.0, axis: Optional[int] = None, shift: bool = False
 ) -> np.ndarray:
     """Softmax function.
 
     Parameters
@@ -26,12 +28,12 @@
         function.
 
     Returns
     -------
     np.ndarray
         Softmax function applied to the input array.
     """
-    x = x / temperature
+    x = x / max(temperature, EPSILON)
     if shift:
         x = x - np.max(x, axis=axis, keepdims=True)
     exp_x = np.exp(x)
     return exp_x / np.sum(exp_x, axis=axis, keepdims=True)
```

### Comparing `cleanlab-2.6.3/cleanlab/internal/object_detection_utils.py` & `cleanlab-2.6.4/cleanlab/internal/object_detection_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/internal/outlier.py` & `cleanlab-2.6.4/cleanlab/internal/outlier.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 Helper functions used internally for outlier detection tasks.
 """
 
+from typing import Optional
 import numpy as np
 
+from cleanlab.internal.constants import EPSILON
+
 
 def transform_distances_to_scores(
     avg_distances: np.ndarray, t: int, scaling_factor: float
 ) -> np.ndarray:
     """Returns an outlier score for each example based on its average distance to its k nearest neighbors.
 
     The transformation of a distance, :math:`d` , to a score, :math:`o` , is based on the following formula:
@@ -63,13 +66,63 @@
     >>> distances = np.array([[0.0, 0.1, 0.25],
     ...                       [0.15, 0.2, 0.3]])
     >>> avg_distances = np.mean(distances, axis=1)
     >>> transform_distances_to_scores(avg_distances, t=1, scaling_factor=1)
     array([0.88988177, 0.80519832])
     """
     # Map ood_features_scores to range 0-1 with 0 = most concerning
-    ood_features_scores: np.ndarray = np.exp(-1 * avg_distances / scaling_factor * t)
+    return np.exp(-t * avg_distances / max(scaling_factor, EPSILON))
+
+
+def correct_precision_errors(
+    scores: np.ndarray,
+    avg_distances: np.ndarray,
+    metric: str,
+    C: int = 100,
+    p: Optional[int] = None,
+):
+    """
+    Ensure that scores where avg_distances are below the tolerance threshold get a score of one.
+
+    Parameters
+    ----------
+    scores :
+        An array of scores of shape ``(N)``, where N is the number of examples.
+        Each entry represents a score between 0 and 1.
 
-    # Set scores to 1 if the average distance is close to 0
-    inds = np.isclose(avg_distances, 0)
-    ood_features_scores[inds] = 1.0
-    return ood_features_scores
+    avg_distances :
+        An array of distances of shape ``(N)``, where N is the number of examples.
+        Each entry represents an example's average distance to its k nearest neighbors.
+
+    metric :
+        The metric used by the knn algorithm to calculate the distances.
+        It must be 'cosine', 'euclidean' or 'minkowski', otherwise this function does nothing.
+
+    C :
+        Multiplier used to increase the tolerance of the acceptable precision differences.
+        It is a multiplicative factor of the machine epsilon that is used to calculate the tolerance.
+        For the type of values that are used in the distances, a value of 100 should be a sensible
+        default value for small values of the distances, below the order of 1.
+
+    p :
+        This value is only used when metric is 'minkowski'.
+        A ValueError will be raised if metric is 'minkowski' and 'p' was not provided.
+
+    Returns
+    -------
+    fixed_scores :
+        An array of scores of shape ``(N,)`` for N examples with scores between 0 and 1.
+    """
+    if metric == "cosine":
+        tolerance = C * np.finfo(np.float_).epsneg
+    elif metric == "euclidean":
+        tolerance = np.sqrt(C * np.finfo(np.float_).eps)
+    elif metric == "minkowski":
+        if p is None:
+            raise ValueError("When metric is 'minkowski' you must specify the 'p' parameter")
+        tolerance = (C * np.finfo(np.float_).eps) ** (1 / p)
+    else:
+        return scores
+
+    candidates_mask = avg_distances < tolerance
+    scores[candidates_mask] = 1
+    return scores
```

### Comparing `cleanlab-2.6.3/cleanlab/internal/regression_utils.py` & `cleanlab-2.6.4/cleanlab/internal/regression_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/internal/segmentation_utils.py` & `cleanlab-2.6.4/cleanlab/internal/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/internal/token_classification_utils.py` & `cleanlab-2.6.4/cleanlab/internal/token_classification_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/internal/util.py` & `cleanlab-2.6.4/cleanlab/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/internal/validation.py` & `cleanlab-2.6.4/cleanlab/internal/validation.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/models/fasttext.py` & `cleanlab-2.6.4/cleanlab/models/fasttext.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/models/keras.py` & `cleanlab-2.6.4/cleanlab/models/keras.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/multiannotator.py` & `cleanlab-2.6.4/cleanlab/multiannotator.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/multilabel_classification/dataset.py` & `cleanlab-2.6.4/cleanlab/multilabel_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/multilabel_classification/filter.py` & `cleanlab-2.6.4/cleanlab/multilabel_classification/filter.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/multilabel_classification/rank.py` & `cleanlab-2.6.4/cleanlab/multilabel_classification/rank.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/object_detection/filter.py` & `cleanlab-2.6.4/cleanlab/object_detection/filter.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/object_detection/rank.py` & `cleanlab-2.6.4/cleanlab/object_detection/rank.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,41 +13,40 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 
 """Methods to rank and score images in an object detection dataset (object detection data), based on how likely they
 are to contain label errors. """
 
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, TypeVar
 import warnings
+import copy
+import numpy as np
 
 from cleanlab.internal.constants import (
     ALPHA,
     CUSTOM_SCORE_WEIGHT_BADLOC,
     CUSTOM_SCORE_WEIGHT_OVERLOOKED,
     CUSTOM_SCORE_WEIGHT_SWAP,
+    EPSILON,
     EUC_FACTOR,
     HIGH_PROBABILITY_THRESHOLD,
     LOW_PROBABILITY_THRESHOLD,
     MAX_ALLOWED_BOX_PRUNE,
     TINY_VALUE,
     TEMPERATURE,
     LABEL_OVERLAP_THRESHOLD,
 )
-
-
-import copy
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, TypeVar
-
-import numpy as np
 from cleanlab.internal.object_detection_utils import (
     softmin1d,
     assert_valid_aggregation_weights,
     assert_valid_inputs,
 )
 
+
 if TYPE_CHECKING:  # pragma: no cover
     from typing import TypedDict
 
     AuxiliaryTypesDict = TypedDict(
         "AuxiliaryTypesDict",
         {
             "pred_labels": np.ndarray,
@@ -374,15 +373,17 @@
     # compute the area of both AABBs
     bb1_area = (bb1["x2"] - bb1["x1"]) * (bb1["y2"] - bb1["y1"])
     bb2_area = (bb2["x2"] - bb2["x1"]) * (bb2["y2"] - bb2["y1"])
 
     # compute the intersection over union by taking the intersection
     # area and dividing it by the sum of prediction + ground-truth
     # areas - the interesection area
-    iou = intersection_area / float(bb1_area + bb2_area - intersection_area)
+    iou = intersection_area / np.clip(
+        float(bb1_area + bb2_area - intersection_area), a_min=EPSILON, a_max=None
+    )  # avoid division by 0
     # There are some hyper-parameters here like consider tile area/object area
     return iou
 
 
 def _has_overlap(bbox_list, labels):
     """This function determines whether each labeled box overlaps with another box of a different class (i.e. virtually the same box having multiple conflicting annotations). It returns a boolean array."""
     iou_matrix = _get_overlap_matrix(bbox_list, bbox_list)
```

### Comparing `cleanlab-2.6.3/cleanlab/object_detection/summary.py` & `cleanlab-2.6.4/cleanlab/object_detection/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,15 @@
     sorted_lab = sorted(lab_grouped, key=lambda x: x[1], reverse=True)
     sorted_pred = sorted(pred_grouped, key=lambda x: x[1], reverse=True)
 
     return sorted_lab, sorted_pred
 
 
 def plot_class_size_distributions(
-    labels, predictions, class_names=None, class_to_show=MAX_CLASS_TO_SHOW
+    labels, predictions, class_names=None, class_to_show=MAX_CLASS_TO_SHOW, **kwargs
 ):
     """
     Plots the size distributions for bounding boxes for each class.
 
     This plot can help you find annotated/predicted boxes for a particular class that are abnormally big/small.
 
     Parameters
@@ -261,14 +261,17 @@
     class_names: optional
         Optional dictionary mapping one-hot-encoded class labels back to their original class names in the format ``{"integer-label": "original-class-name"}``.
         You can use this argument to control the classes for which the size distribution is plotted.
 
     class_to_show: optional
         The number of classes to show in the plots. Classes over `class_to_show` are hidden. If this argument is provided, then the classes are sorted by the number of instances in the dataset.
         Defaults to `MAX_CLASS_TO_SHOW` which is set to 10.
+
+    kwargs:
+        Additional keyword arguments to pass to ``plt.show()`` (matplotlib.pyplot.show).
     """
     try:
         import matplotlib.pyplot as plt
     except ImportError as e:
         raise ImportError(
             "This functionality requires matplotlib. Install it via: `pip install matplotlib`"
         )
@@ -287,18 +290,18 @@
         fig.suptitle(f"Size distributions for bounding box for class {c}")
         for i, l in enumerate([lab_boxes, pred_boxes]):
             axs[i].hist(l[c], bins="auto")
             axs[i].set_xlabel("box area (pixels)")
             axs[i].set_ylabel("count")
             axs[i].set_title("annotated" if i == 0 else "predicted")
 
-        plt.show()
+        plt.show(**kwargs)
 
 
-def plot_class_distribution(labels, predictions, class_names=None):
+def plot_class_distribution(labels, predictions, class_names=None, **kwargs):
     """
     Plots the distribution of class labels associated with all annotated bounding boxes and predicted bounding boxes in the dataset.
 
     This plot can help you understand which classes are rare or over/under-predicted by the model overall.
 
     Parameters
     ----------
@@ -308,14 +311,17 @@
 
     predictions:
         Predictions output by a trained object detection model.
         Refer to documentation for this argument in :py:func:`object_counts_per_image <cleanlab.object_detection.summary.object_counts_per_image>` for further details.
 
     class_names: optional
         Optional dictionary mapping one-hot-encoded class labels back to their original class names in the format ``{"integer-label": "original-class-name"}``.
+
+    kwargs:
+        Additional keyword arguments to pass to ``plt.show()`` (matplotlib.pyplot.show).
     """
     try:
         import matplotlib.pyplot as plt
     except ImportError as e:
         raise ImportError(
             "This functionality requires matplotlib. Install it via: `pip install matplotlib`"
         )
@@ -323,27 +329,28 @@
     lab_dist, pred_dist = class_label_distribution(labels, predictions, class_names=class_names)
     fig, axs = plt.subplots(1, 2, figsize=(10, 5))
     fig.suptitle(f"Distribution of classes in the dataset")
     for i, d in enumerate([lab_dist, pred_dist]):
         axs[i].pie(d.values(), labels=d.keys(), autopct="%1.1f%%")
         axs[i].set_title("Annotated" if i == 0 else "Predicted")
 
-    plt.show()
+    plt.show(**kwargs)
 
 
 def visualize(
     image: Union[str, np.ndarray, Image],
     *,
     label: Optional[Dict[str, Any]] = None,
     prediction: Optional[np.ndarray] = None,
     prediction_threshold: Optional[float] = None,
     overlay: bool = True,
     class_names: Optional[Dict[Any, Any]] = None,
     figsize: Optional[Tuple[int, int]] = None,
     save_path: Optional[str] = None,
+    **kwargs,
 ) -> None:
     """Display the annotated bounding boxes (given labels) and predicted bounding boxes (model predictions) for a particular image.
     Given labels are shown in red, model predictions in blue.
 
 
     Parameters
     ----------
@@ -376,14 +383,17 @@
 
     save_path:
         Path to save figure at. If a path is provided, the figure is saved. To save in a specific image format, add desired file extension to the end of `save_path`. Allowed file extensions are: 'png', 'pdf', 'ps', 'eps', and 'svg'.
 
     figsize:
         Optional figure size for plotting the image.
         Corresponds to ``matplotlib.figure.figsize``.
+
+    kwargs:
+        Additional keyword arguments to pass to ``plt.show()`` (matplotlib.pyplot.show).
     """
     try:
         import matplotlib.pyplot as plt
     except ImportError as e:
         raise ImportError(
             "This functionality requires matplotlib. Install it via: `pip install matplotlib`"
         )
@@ -447,15 +457,15 @@
             save_path,
             format=image_format,
             bbox_extra_artists=bbox_extra_artists,
             bbox_inches="tight",
             transparent=True,
             pad_inches=0.5,
         )
-    plt.show()
+    plt.show(**kwargs)
 
 
 def _get_per_class_confusion_matrix_dict_(
     labels: List[Dict[str, Any]],
     predictions: List[np.ndarray],
     iou_threshold: Optional[float] = 0.5,
     num_procs: int = 1,
```

### Comparing `cleanlab-2.6.3/cleanlab/outlier.py` & `cleanlab-2.6.4/cleanlab/outlier.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,28 @@
 """
 Methods for finding out-of-distribution examples in a dataset via scores that quantify how atypical each example is compared to the others.
 
 The underlying algorithms are described in `this paper <https://arxiv.org/abs/2207.03061>`_.
 """
 
 import warnings
+from typing import Callable, Dict, Optional, Tuple, Union
+
 import numpy as np
-from cleanlab.count import get_confident_thresholds
-from sklearn.neighbors import NearestNeighbors
+from scipy.spatial.distance import euclidean
 from sklearn.exceptions import NotFittedError
-from typing import Optional, Union, Tuple, Dict
+from sklearn.neighbors import NearestNeighbors
+
+from cleanlab.count import get_confident_thresholds
 from cleanlab.internal.label_quality_utils import (
     _subtract_confident_thresholds,
     get_normalized_entropy,
 )
 from cleanlab.internal.numerics import softmax
-from cleanlab.internal.outlier import transform_distances_to_scores
+from cleanlab.internal.outlier import correct_precision_errors, transform_distances_to_scores
 from cleanlab.internal.validation import assert_valid_inputs, labels_to_array
 from cleanlab.typing import LabelLike
 
 
 class OutOfDistribution:
     """
     Provides scores to detect Out Of Distribution (OOD) examples that are outliers in a dataset.
@@ -54,17 +57,24 @@
      If `features` is passed in during ``fit()``, `params` could contain following keys:
        *  knn: sklearn.neighbors.NearestNeighbors, default = None
              Instantiated ``NearestNeighbors`` object that's been fitted on a dataset in the same feature space.
              Note that the distance metric and `n_neighbors` is specified when instantiating this class.
              You can also pass in a subclass of ``sklearn.neighbors.NearestNeighbors`` which allows you to use faster
              approximate neighbor libraries as long as you wrap them behind the same sklearn API.
              If you specify ``knn`` here, there is no need to later call ``fit()`` before calling ``score()``.
-             If ``knn = None``, then by default: ``knn = sklearn.neighbors.NearestNeighbors(n_neighbors=k, metric=dist_metric).fit(features)``
-             where ``dist_metric == "cosine"`` if ``dim(features) > 3`` or ``dist_metric == "euclidean"`` otherwise.
+             If ``knn is None``, then by default:
+             The knn object is instantiated as ``sklearn.neighbors.NearestNeighbors(n_neighbors=k, metric=dist_metric).fit(features)``.
+             - If ``dim(features) > 3``, the distance metric is set to "cosine".
+             - If ``dim(features) <= 3``, the distance metric is set to "euclidean".
+               The implementation of the euclidean distance metric depends on the number of examples in the features array:
+                - For more than 100 rows, it uses scikit-learn's "euclidean" metric. This is for efficiency reasons reasons.
+                - For 100 or fewer rows, it uses scipy's ``scipy.spatial.distance.euclidean`` metric. This is for numerical stability reasons.
              See: https://scikit-learn.org/stable/modules/neighbors.html
+             See: https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.euclidean_distances.html
+             See: https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.euclidean.html
        *  k : int, default=None
              Optional number of neighbors to use when calculating outlier score (average distance to neighbors).
              If `k` is not provided, then by default ``k = knn.n_neighbors`` or ``k = 10`` if ``knn is None``.
              If an existing ``knn`` object is provided, you can still specify that outlier scores should use
              a different value of `k` than originally used in the ``knn``,
              as long as your specified value of `k` is smaller than the value originally used in ``knn``.
        *  t : int, default=1
@@ -407,34 +417,41 @@
         Returns
         -------
         ood_features_scores : Tuple[np.ndarray, Optional[NearestNeighbors]]
         Return a tuple whose first element is array of `ood_features_scores` and second is a `knn` Estimator object.
         """
         DEFAULT_K = 10
         # fit skip over (if knn is not None) then skipping fit and suggest score else fit.
+        distance_metric = None
         if knn is None:  # setup default KNN estimator
             # Make sure both knn and features are not None
             if features is None:
                 raise ValueError(
                     "Both knn and features arguments cannot be None at the same time. Not enough information to compute outlier scores."
                 )
             if k is None:
                 k = DEFAULT_K  # use default when knn and k are both None
-            if k > len(features):  # Ensure number of neighbors less than number of examples
+            N, M = features.shape
+            if k > N:  # Ensure number of neighbors less than number of examples
                 raise ValueError(
                     f"Number of nearest neighbors k={k} cannot exceed the number of examples N={len(features)} passed into the estimator (knn)."
                 )
 
-            if features.shape[1] > 3:  # use euclidean distance for lower dimensional spaces
+            # strings are used for sklearn metrics, callables are scipy pairwise distance functions
+            metric: Union[str, Callable]
+            if M > 3:  # use euclidean distance for lower dimensional spaces
                 metric = "cosine"
-            else:
+            elif N > 100:  # Use efficient implementation (numerically unstable in edge cases)
                 metric = "euclidean"
+            else:  # Use scipy implementation for precise results
+                metric = euclidean
 
             knn = NearestNeighbors(n_neighbors=k, metric=metric).fit(features)
             features = None  # features should be None in knn.kneighbors(features) to avoid counting duplicate data points
+            distance_metric = metric if isinstance(metric, str) else str(metric.__name__)
 
         elif k is None:
             k = knn.n_neighbors
 
         max_k = knn.n_neighbors  # number of neighbors previously used in NearestNeighbors object
         if k > max_k:  # if k provided is too high, use max possible number of nearest neighbors
             warnings.warn(
@@ -466,14 +483,23 @@
 
         if not isinstance(scaling_factor, float):
             raise ValueError(f"Scaling factor must be a float. Got {type(scaling_factor)} instead.")
 
         ood_features_scores = transform_distances_to_scores(
             avg_knn_distances, t, scaling_factor=scaling_factor
         )
+        distance_metric = distance_metric or (
+            metric if isinstance((metric := knn.metric), str) else metric.__name__
+        )
+        p = None
+        if distance_metric == "minkowski":
+            p = knn.p
+        ood_features_scores = correct_precision_errors(
+            ood_features_scores, avg_knn_distances, distance_metric, p=p
+        )
         return (ood_features_scores, knn)
 
 
 def _get_ood_predictions_scores(
     pred_probs: np.ndarray,
     *,
     labels: Optional[LabelLike] = None,
```

### Comparing `cleanlab-2.6.3/cleanlab/rank.py` & `cleanlab-2.6.4/cleanlab/rank.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/regression/learn.py` & `cleanlab-2.6.4/cleanlab/regression/learn.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/regression/rank.py` & `cleanlab-2.6.4/cleanlab/regression/rank.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,18 @@
 
 Note: Label quality scores are most accurate when they are computed based on out-of-sample `predictions` from your regression model.
 To obtain out-of-sample predictions for every datapoint in your dataset, you can use :ref:`cross-validation <pred_probs_cross_val>`. This is encouraged to get better results.
 
 If you have a sklearn-compatible regression model, consider using `cleanlab.regression.learn.CleanLearning` instead, which can more accurately identify noisy label values.
 """
 
-from typing import Dict, Callable
+from typing import Dict, Callable, Optional, Union
 import numpy as np
 from numpy.typing import ArrayLike
+from scipy.spatial.distance import euclidean
 from sklearn.neighbors import NearestNeighbors
 
 from cleanlab.outlier import OutOfDistribution
 from cleanlab.internal.regression_utils import assert_valid_prediction_inputs
 
 from cleanlab.internal.constants import TINY_VALUE
 
@@ -137,15 +138,15 @@
 
 def _get_outre_score_for_each_label(
     labels: np.ndarray,
     predictions: np.ndarray,
     *,
     residual_scale: float = 5,
     frac_neighbors: float = 0.5,
-    neighbor_metric: str = "euclidean",
+    neighbor_metric: Optional[Union[str, Callable]] = "euclidean",
 ) -> np.ndarray:
     """Returns OUTRE based label-quality scores.
 
     This function computes label-quality scores for regression datasets,
     where a lower score indicates labels that are less likely to be correct.
 
     Parameters
@@ -158,16 +159,17 @@
 
     residual_scale: float, default = 5
         Multiplicative factor to adjust scale (standard deviation) of the residuals relative to the labels.
 
     frac_neighbors: float, default = 0.5
         Fraction of examples in dataset that should be considered as `n_neighbors` in the ``NearestNeighbors`` object used internally to assess outliers.
 
-    neighbor_metric: str, default = "euclidean"
+    neighbor_metric: Optional[str or callable], default = None
         The parameter is passed to sklearn NearestNeighbors. # TODO add reference to sklearn.NearestNeighbor?
+        If None, the metric is chosen based on the number of features in the dataset.
 
     Returns
     -------
     label_quality_scores: np.ndarray
         Contains one score (between 0 and 1) per example.
         Lower scores indicate more likely mislabled examples.
     """
@@ -175,12 +177,17 @@
     labels = (labels - labels.mean()) / (labels.std() + TINY_VALUE)
     residual = residual_scale * ((residual - residual.mean()) / (residual.std() + TINY_VALUE))
 
     # 2D features by combining labels and residual
     features = np.array([labels, residual]).T
 
     neighbors = int(np.ceil(frac_neighbors * labels.shape[0]))
+    if neighbor_metric is None:
+        if features.shape[0] > 100:
+            neighbor_metric = "euclidean"
+        else:
+            neighbor_metric = euclidean
     knn = NearestNeighbors(n_neighbors=neighbors, metric=neighbor_metric).fit(features)
     ood = OutOfDistribution(params={"knn": knn})
 
     label_quality_scores = ood.score(features=features)
     return label_quality_scores
```

### Comparing `cleanlab-2.6.3/cleanlab/segmentation/filter.py` & `cleanlab-2.6.4/cleanlab/segmentation/filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 Methods to find label issues in image semantic segmentation datasets, where each pixel in an image receives its own class label.
 
 """
 
-from cleanlab.experimental.label_issues_batched import LabelInspector
+from typing import Optional, Tuple
+
 import numpy as np
-from typing import Tuple, Optional
 
-from cleanlab.internal.segmentation_utils import _get_valid_optional_params, _check_input
+from cleanlab.experimental.label_issues_batched import LabelInspector
+from cleanlab.internal.segmentation_utils import _check_input, _get_valid_optional_params
 
 
 def find_label_issues(
     labels: np.ndarray,
     pred_probs: np.ndarray,
     *,
     batch_size: Optional[int] = None,
@@ -98,21 +99,19 @@
 
         # Check if possible to downsample
         if h % downsample != 0 or w % downsample != 0:
             raise ValueError(
                 f"Height {h} and width {w} not divisible by downsample value of {downsample}. Set kwarg downsample to 1 to avoid downsampling."
             )
         small_labels = np.round(
-            labels.reshape((num_image, h // factor, factor, w // factor, factor)).mean(4).mean(2)
-        )
-        small_pred_probs = (
-            pred_probs.reshape((num_image, num_classes, h // factor, factor, w // factor, factor))
-            .mean(5)
-            .mean(3)
+            labels.reshape((num_image, h // factor, factor, w // factor, factor)).mean((4, 2))
         )
+        small_pred_probs = pred_probs.reshape(
+            (num_image, num_classes, h // factor, factor, w // factor, factor)
+        ).mean((5, 3))
 
         # We want to make sure that pred_probs are renormalized
         row_sums = small_pred_probs.sum(axis=1)
         renorm_small_pred_probs = small_pred_probs / np.expand_dims(row_sums, 1)
 
         return small_labels, renorm_small_pred_probs
 
@@ -179,39 +178,57 @@
 
     if verbose:
         pbar.close()
 
     ranked_label_issues = lab.get_label_issues()
     ### End find_label_issues_batched() section
 
-    # Finding the right indicies
-    relative_index = ranked_label_issues % (h * w)
-    pixel_coor_i, pixel_coor_j = np.unravel_index(relative_index, (h, w))
-    image_number = ranked_label_issues // (h * w)
-
     # Upsample carefully maintaining indicies
     label_issues = np.full((num_image, h, w), False)
 
-    for num, ii, jj in zip(image_number, pixel_coor_i, pixel_coor_j):
-        # only want to call it an error if pred_probs doesnt match the label at that pixel
-        label_issues[num, ii, jj] = True
+    # only want to call it an error if pred_probs doesnt match the label at those pixels
+    for i in range(0, ranked_label_issues.shape[0], batch_size):
+        issues_batch = ranked_label_issues[i : i + batch_size]
+        # Finding the right indicies
+        image_batch, batch_coor_i, batch_coor_j = _get_indexes_from_ranked_issues(
+            issues_batch, h, w
+        )
+        label_issues[image_batch, batch_coor_i, batch_coor_j] = True
         if downsample == 1:
-            # check if pred_probs matches the label at that pixel
-            if np.argmax(pred_probs[num, :, ii, jj]) == labels[num, ii, jj]:
-                label_issues[num, ii, jj] = False
+            # check if pred_probs matches the label at those pixels
+            pred_argmax = np.argmax(pred_probs[image_batch, :, batch_coor_i, batch_coor_j], axis=1)
+            mask = pred_argmax == labels[image_batch, batch_coor_i, batch_coor_j]
+            label_issues[image_batch[mask], batch_coor_i[mask], batch_coor_j[mask]] = False
 
     if downsample != 1:
         label_issues = label_issues.repeat(downsample, axis=1).repeat(downsample, axis=2)
 
-        for num, ii, jj in zip(image_number, pixel_coor_i, pixel_coor_j):
+        for i in range(0, ranked_label_issues.shape[0], batch_size):
+            issues_batch = ranked_label_issues[i : i + batch_size]
+            image_batch, batch_coor_i, batch_coor_j = _get_indexes_from_ranked_issues(
+                issues_batch, h, w
+            )
             # Upsample the coordinates
-            upsampled_ii = ii * downsample
-            upsampled_jj = jj * downsample
+            upsampled_ii = batch_coor_i * downsample
+            upsampled_jj = batch_coor_j * downsample
             # Iterate over the upsampled region
-            for row in range(upsampled_ii, upsampled_ii + downsample):
-                for col in range(upsampled_jj, upsampled_jj + downsample):
+            for i in range(downsample):
+                for j in range(downsample):
+                    rows = upsampled_ii + i
+                    cols = upsampled_jj + j
+                    pred_argmax = np.argmax(pred_probs[image_batch, :, rows, cols], axis=1)
                     # Check if the predicted class (argmax) at the identified issue location matches the true label
-                    if np.argmax(pred_probs[num, :, row, col]) == labels[num, row, col]:
-                        # If they match, set the corresponding entry in the label_issues array to False
-                        label_issues[num, row, col] = False
+                    mask = pred_argmax == labels[image_batch, rows, cols]
+                    # If they match, set the corresponding entries in the label_issues array to False
+                    label_issues[image_batch[mask], rows[mask], cols[mask]] = False
 
     return label_issues
+
+
+def _get_indexes_from_ranked_issues(
+    ranked_label_issues: np.ndarray, h: int, w: int
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+    hw = h * w
+    relative_index = ranked_label_issues % hw
+    pixel_coor_i, pixel_coor_j = np.unravel_index(relative_index, (h, w))
+    image_batch = ranked_label_issues // hw
+    return image_batch, pixel_coor_i, pixel_coor_j
```

### Comparing `cleanlab-2.6.3/cleanlab/segmentation/rank.py` & `cleanlab-2.6.4/cleanlab/segmentation/rank.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 Methods to rank and score images in a semantic segmentation dataset based on how likely they are to contain mislabeled pixels.
 """
-import numpy as np
 import warnings
-from typing import Optional, Union, Tuple
-from cleanlab.segmentation.filter import find_label_issues
+from typing import Optional, Tuple
+
+import numpy as np
 
-from cleanlab.internal.segmentation_utils import _get_valid_optional_params, _check_input
+from cleanlab.internal.segmentation_utils import _check_input, _get_valid_optional_params
+from cleanlab.segmentation.filter import find_label_issues
 
 
 def get_label_quality_scores(
     labels: np.ndarray,
     pred_probs: np.ndarray,
     *,
     method: str = "softmin",
@@ -115,40 +116,42 @@
 
     if downsample_num_pixel_issues != 1:
         warnings.warn(
             f"image will not downsample for method {method} is only for method: num_pixel_issues"
         )
 
     num_im, num_class, h, w = pred_probs.shape
-    image_scores = []
-    pixel_scores = []
+    image_scores = np.empty((num_im,))
+    pixel_scores = np.empty((num_im, h, w))
     if verbose:
         from tqdm.auto import tqdm
 
         pbar = tqdm(desc=f"images processed using {method}", total=num_im)
+
+    h_array = np.arange(h)[:, None]
+    w_array = np.arange(w)
+
     for image in range(num_im):
         image_probs = pred_probs[image][
             labels[image],
-            np.arange(h)[:, None],
-            np.arange(w),
+            h_array,
+            w_array,
         ]
-        pixel_scores.append(image_probs)
-        image_scores.append(
-            _get_label_quality_per_image(
-                np.array(image_probs.flatten()), method=method, temperature=softmin_temperature
-            )
+        pixel_scores[image, :, :] = image_probs
+        image_scores[image] = _get_label_quality_per_image(
+            image_probs.flatten(), method=method, temperature=softmin_temperature
         )
         if verbose:
             pbar.update(1)
-    return np.array(image_scores), np.array(pixel_scores)
+    return image_scores, pixel_scores
 
 
 def issues_from_scores(
     image_scores: np.ndarray, pixel_scores: Optional[np.ndarray] = None, threshold: float = 0.1
-) -> Union[list, np.ndarray]:
+) -> np.ndarray:
     """
     Converts scores output by `~cleanlab.segmentation.rank.get_label_quality_scores`
     to a list of issues of similar format as output by :py:func:`segmentation.filter.find_label_issues <cleanlab.segmentation.filter.find_label_issues>`.
 
     Only considers as issues those tokens with label quality score lower than `threshold`,
     so this parameter determines the number of issues that are returned.
 
@@ -187,20 +190,19 @@
 
     if image_scores is None:
         raise ValueError("pixel_scores must be provided")
     if threshold < 0 or threshold > 1 or threshold is None:
         raise ValueError("threshold must be between 0 and 1")
 
     if pixel_scores is not None:
-        issues = np.where(pixel_scores < threshold, True, False)
-    else:
-        ranking = np.argsort(image_scores)
-        cutoff = np.searchsorted(image_scores[ranking], threshold)
-        issues = ranking[: cutoff + 1]
-    return issues
+        return pixel_scores < threshold
+
+    ranking = np.argsort(image_scores)
+    cutoff = np.searchsorted(image_scores[ranking], threshold)
+    return ranking[: cutoff + 1]
 
 
 def _get_label_quality_per_image(pixel_scores, method=None, temperature=0.1):
     from cleanlab.internal.multilabel_scorer import softmin
 
     """
     Input pixel scores and get label quality score for that image, currently using the "softmin" method.
```

### Comparing `cleanlab-2.6.3/cleanlab/segmentation/summary.py` & `cleanlab-2.6.4/cleanlab/segmentation/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     issues: np.ndarray,
     *,
     labels: Optional[np.ndarray] = None,
     pred_probs: Optional[np.ndarray] = None,
     class_names: Optional[List[str]] = None,
     exclude: Optional[List[int]] = None,
     top: Optional[int] = None,
+    **kwargs,  # Accepting additional kwargs for plt.show()
 ) -> None:
     """
     Display semantic segmentation label issues, showing images with problematic pixels highlighted.
 
     Can also show given and predicted masks for each image identified to have label issue.
 
     Parameters
@@ -83,28 +84,30 @@
 
     top:
         Optional maximum number of issues to be printed. If not provided, a good default is used.
 
     exclude:
         Optional list of label classes that can be ignored in the errors, each element must be 0, 1, ..., K-1
 
+    kwargs
+        Additional keyword arguments to pass to ``plt.show()`` (matplotlib.pyplot.show).
     """
     class_names, exclude, top = _get_summary_optional_params(class_names, exclude, top)
     if labels is None and len(exclude) > 0:
         raise ValueError("Provide labels to allow class exclusion")
 
     top = min(top, len(issues))
 
     correct_ordering = np.argsort(-np.sum(issues, axis=(1, 2)))[:top]
 
     try:
         import matplotlib.pyplot as plt
         import matplotlib.patches as mpatches
         from matplotlib.colors import ListedColormap
-    except:
+    except ImportError:
         raise ImportError('try "pip install matplotlib"')
 
     output_plots = (pred_probs is not None) + (labels is not None) + 1
 
     # Colormap for errors
     error_cmap = ListedColormap(["none", "red"])
     _, h, w = issues.shape
@@ -124,15 +127,15 @@
             mpatches.Patch(color=cmap[i], label=class_names[i]) for i in range(len(class_names))
         ]
         legend = plt.figure()  # adjust figsize for larger legend
         legend.legend(
             handles=patches, loc="center", ncol=len(class_names), facecolor="white", fontsize=20
         )  # adjust fontsize for larger text
         plt.axis("off")
-        plt.show()
+        plt.show(**kwargs)
 
     for i in correct_ordering:
         # Show images
         fig, axes = plt.subplots(1, output_plots, figsize=(5 * output_plots, 5))
         plot_index = 0
 
         # First image - Given truth labels
@@ -154,15 +157,15 @@
             ax = axes[plot_index]
 
         mask = np.full((h, w), True)
         if labels is not None and len(exclude) != 0:
             mask = ~np.isin(labels[i], exclude)
         ax.imshow(issues[i] & mask, cmap=error_cmap, vmin=0, vmax=1)
         ax.set_title(f"Image {i}: Suggested Errors (in Red)")
-        plt.show()
+        plt.show(**kwargs)
 
     return None
 
 
 def common_label_issues(
     issues: np.ndarray,
     labels: np.ndarray,
```

### Comparing `cleanlab-2.6.3/cleanlab/token_classification/filter.py` & `cleanlab-2.6.4/cleanlab/token_classification/filter.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/token_classification/rank.py` & `cleanlab-2.6.4/cleanlab/token_classification/rank.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/token_classification/summary.py` & `cleanlab-2.6.4/cleanlab/token_classification/summary.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/cleanlab/version.py` & `cleanlab-2.6.4/cleanlab/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 
 
-__version__ = "2.6.3"
+__version__ = "2.6.4"
 
 # 2.6.4 - Not yet released, you are using bleeding-edge developer version. See its documentation at: https://docs.cleanlab.ai/master/
 
 # ------------------------------------------------
 # | PREVIOUS MAJOR VERSION RELEASE NOTES SUMMARY |
 # ------------------------------------------------
```

### Comparing `cleanlab-2.6.3/cleanlab.egg-info/PKG-INFO` & `cleanlab-2.6.4/cleanlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab
-Version: 2.6.3
+Version: 2.6.4
 Summary: The standard package for data-centric AI, machine learning with label errors, and automatically finding and fixing dataset issues in Python.
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License: 
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -700,17 +700,17 @@
 Requires-Dist: termcolor>=2.4.0
 Provides-Extra: datalab
 Requires-Dist: datasets>=2.7.0; extra == "datalab"
 Provides-Extra: image
 Requires-Dist: datasets>=2.7.0; extra == "image"
 Requires-Dist: cleanvision>=0.3.6; extra == "image"
 Provides-Extra: all
-Requires-Dist: matplotlib>=3.5.1; extra == "all"
 Requires-Dist: cleanvision>=0.3.6; extra == "all"
 Requires-Dist: datasets>=2.7.0; extra == "all"
+Requires-Dist: matplotlib>=3.5.1; extra == "all"
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/cleanlab_logo_open_source.png" width=60% height=60%>
 </p>
 
 
 cleanlab helps you **clean** data and **lab**els by automatically detecting issues in a ML dataset. To facilitate **machine learning with messy, real-world data**, this data-centric AI package uses your *existing* models to estimate dataset problems that can be fixed to train even *better* models.
```

### Comparing `cleanlab-2.6.3/cleanlab.egg-info/SOURCES.txt` & `cleanlab-2.6.4/cleanlab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 cleanlab/__init__.py
 cleanlab/classification.py
 cleanlab/count.py
+cleanlab/data_valuation.py
 cleanlab/dataset.py
 cleanlab/filter.py
 cleanlab/multiannotator.py
 cleanlab/outlier.py
 cleanlab/rank.py
 cleanlab/typing.py
 cleanlab/version.py
@@ -56,14 +57,15 @@
 cleanlab/datalab/internal/issue_manager/regression/label.py
 cleanlab/experimental/__init__.py
 cleanlab/experimental/cifar_cnn.py
 cleanlab/experimental/coteaching.py
 cleanlab/experimental/label_issues_batched.py
 cleanlab/experimental/mnist_pytorch.py
 cleanlab/experimental/span_classification.py
+cleanlab/experimental/datalab/data_monitor.py
 cleanlab/internal/__init__.py
 cleanlab/internal/constants.py
 cleanlab/internal/label_quality_utils.py
 cleanlab/internal/latent_algebra.py
 cleanlab/internal/multiannotator_utils.py
 cleanlab/internal/multilabel_scorer.py
 cleanlab/internal/multilabel_utils.py
```

### Comparing `cleanlab-2.6.3/pyproject.toml` & `cleanlab-2.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.3/setup.py` & `cleanlab-2.6.4/setup.py`

 * *Files identical despite different names*

