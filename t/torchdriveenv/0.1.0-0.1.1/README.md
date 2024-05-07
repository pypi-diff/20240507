# Comparing `tmp/torchdriveenv-0.1.0.tar.gz` & `tmp/torchdriveenv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchdriveenv-0.1.0.tar", last modified: Fri Apr 26 01:16:44 2024, max compression
+gzip compressed data, was "torchdriveenv-0.1.1.tar", last modified: Tue May  7 00:56:16 2024, max compression
```

## Comparing `torchdriveenv-0.1.0.tar` & `torchdriveenv-0.1.1.tar`

### file list

```diff
@@ -1,114 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:16:44.291826 torchdriveenv-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:16:44.247826 torchdriveenv-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:16:44.251826 torchdriveenv-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-26 01:16:44.291826 torchdriveenv-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:16:44.251826 torchdriveenv-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/examples/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:16:44.251826 torchdriveenv-0.1.0/examples/env_configs/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/examples/env_configs/rl_training.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/examples/rl_training.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      393 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/examples/train.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/examples/waypoint_suite_env_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/examples/waypoint_suite_evaluation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 01:16:44.291826 torchdriveenv-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:16:44.251826 torchdriveenv-0.1.0/torchdriveenv/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:16:44.251826 torchdriveenv-0.1.0/torchdriveenv/data/
--rw-r--r--   0 runner    (1001) docker     (127)    38777 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/data/training_cases.yml
--rw-r--r--   0 runner    (1001) docker     (127)    34899 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/data/validation_cases.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/env_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/gym_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/iai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:16:44.247826 torchdriveenv-0.1.0/torchdriveenv/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:16:44.287826 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/
--rw-r--r--   0 runner    (1001) docker     (127)   164574 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_10_634.json
--rw-r--r--   0 runner    (1001) docker     (127)   244747 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_15_15.json
--rw-r--r--   0 runner    (1001) docker     (127)   235631 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_15_575.json
--rw-r--r--   0 runner    (1001) docker     (127)   236037 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_15_673.json
--rw-r--r--   0 runner    (1001) docker     (127)   229150 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_15_770.json
--rw-r--r--   0 runner    (1001) docker     (127)   289240 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_18_22.json
--rw-r--r--   0 runner    (1001) docker     (127)   283754 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_18_268.json
--rw-r--r--   0 runner    (1001) docker     (127)   285506 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_18_654.json
--rw-r--r--   0 runner    (1001) docker     (127)    80980 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_5_306.json
--rw-r--r--   0 runner    (1001) docker     (127)    83971 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_5_57.json
--rw-r--r--   0 runner    (1001) docker     (127)   164528 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_10_131.json
--rw-r--r--   0 runner    (1001) docker     (127)   233031 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_142.json
--rw-r--r--   0 runner    (1001) docker     (127)   228878 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_270.json
--rw-r--r--   0 runner    (1001) docker     (127)   232657 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_342.json
--rw-r--r--   0 runner    (1001) docker     (127)   241607 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_568.json
--rw-r--r--   0 runner    (1001) docker     (127)   228907 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_795.json
--rw-r--r--   0 runner    (1001) docker     (127)   242169 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_9.json
--rw-r--r--   0 runner    (1001) docker     (127)   252569 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_920.json
--rw-r--r--   0 runner    (1001) docker     (127)   292355 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_141.json
--rw-r--r--   0 runner    (1001) docker     (127)   297252 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_229.json
--rw-r--r--   0 runner    (1001) docker     (127)   276077 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_345.json
--rw-r--r--   0 runner    (1001) docker     (127)   290439 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_356.json
--rw-r--r--   0 runner    (1001) docker     (127)   285721 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_501.json
--rw-r--r--   0 runner    (1001) docker     (127)   291932 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_515.json
--rw-r--r--   0 runner    (1001) docker     (127)   283201 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_682.json
--rw-r--r--   0 runner    (1001) docker     (127)   292148 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_746.json
--rw-r--r--   0 runner    (1001) docker     (127)   281006 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_749.json
--rw-r--r--   0 runner    (1001) docker     (127)   282515 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_998.json
--rw-r--r--   0 runner    (1001) docker     (127)    84398 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_5_16.json
--rw-r--r--   0 runner    (1001) docker     (127)    84076 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_5_928.json
--rw-r--r--   0 runner    (1001) docker     (127)   154723 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_216.json
--rw-r--r--   0 runner    (1001) docker     (127)   165661 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_271.json
--rw-r--r--   0 runner    (1001) docker     (127)   168352 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_294.json
--rw-r--r--   0 runner    (1001) docker     (127)   168294 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_315.json
--rw-r--r--   0 runner    (1001) docker     (127)   165254 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_378.json
--rw-r--r--   0 runner    (1001) docker     (127)   167515 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_42.json
--rw-r--r--   0 runner    (1001) docker     (127)   168309 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_443.json
--rw-r--r--   0 runner    (1001) docker     (127)   168616 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_522.json
--rw-r--r--   0 runner    (1001) docker     (127)   168448 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_542.json
--rw-r--r--   0 runner    (1001) docker     (127)   161935 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_565.json
--rw-r--r--   0 runner    (1001) docker     (127)   161887 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_663.json
--rw-r--r--   0 runner    (1001) docker     (127)   168553 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_701.json
--rw-r--r--   0 runner    (1001) docker     (127)   164839 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_733.json
--rw-r--r--   0 runner    (1001) docker     (127)   153775 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_757.json
--rw-r--r--   0 runner    (1001) docker     (127)   165044 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_816.json
--rw-r--r--   0 runner    (1001) docker     (127)   168037 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_839.json
--rw-r--r--   0 runner    (1001) docker     (127)   164153 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_932.json
--rw-r--r--   0 runner    (1001) docker     (127)   164917 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_948.json
--rw-r--r--   0 runner    (1001) docker     (127)   168411 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_96.json
--rw-r--r--   0 runner    (1001) docker     (127)   165352 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_993.json
--rw-r--r--   0 runner    (1001) docker     (127)   164127 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_10_31.json
--rw-r--r--   0 runner    (1001) docker     (127)   161910 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_10_760.json
--rw-r--r--   0 runner    (1001) docker     (127)   212721 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_15_103.json
--rw-r--r--   0 runner    (1001) docker     (127)   212766 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_15_205.json
--rw-r--r--   0 runner    (1001) docker     (127)   235880 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_15_447.json
--rw-r--r--   0 runner    (1001) docker     (127)   245696 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_15_863.json
--rw-r--r--   0 runner    (1001) docker     (127)   289503 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_18_416.json
--rw-r--r--   0 runner    (1001) docker     (127)    72724 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_328.json
--rw-r--r--   0 runner    (1001) docker     (127)    84713 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_407.json
--rw-r--r--   0 runner    (1001) docker     (127)    77004 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_564.json
--rw-r--r--   0 runner    (1001) docker     (127)    80235 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_810.json
--rw-r--r--   0 runner    (1001) docker     (127)    68038 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_844.json
--rw-r--r--   0 runner    (1001) docker     (127)    72411 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_925.json
--rw-r--r--   0 runner    (1001) docker     (127)    69370 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_945.json
--rw-r--r--   0 runner    (1001) docker     (127)    84531 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_98.json
--rw-r--r--   0 runner    (1001) docker     (127)   217126 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_15_257.json
--rw-r--r--   0 runner    (1001) docker     (127)   248587 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_15_605.json
--rw-r--r--   0 runner    (1001) docker     (127)   249459 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_15_647.json
--rw-r--r--   0 runner    (1001) docker     (127)   253756 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_15_676.json
--rw-r--r--   0 runner    (1001) docker     (127)   262930 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_18_230.json
--rw-r--r--   0 runner    (1001) docker     (127)   300677 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_18_451.json
--rw-r--r--   0 runner    (1001) docker     (127)   300262 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_18_742.json
--rw-r--r--   0 runner    (1001) docker     (127)    73086 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_5_417.json
--rw-r--r--   0 runner    (1001) docker     (127)    84856 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_5_576.json
--rw-r--r--   0 runner    (1001) docker     (127)    84867 2024-04-26 01:16:39.000000 torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_5_840.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:16:44.291826 torchdriveenv-0.1.0/torchdriveenv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-26 01:16:44.000000 torchdriveenv-0.1.0/torchdriveenv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-26 01:16:44.000000 torchdriveenv-0.1.0/torchdriveenv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:16:44.000000 torchdriveenv-0.1.0/torchdriveenv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-26 01:16:44.000000 torchdriveenv-0.1.0/torchdriveenv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 01:16:44.000000 torchdriveenv-0.1.0/torchdriveenv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:56:16.746903 torchdriveenv-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:56:16.706903 torchdriveenv-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:56:16.710903 torchdriveenv-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-07 00:56:16.746903 torchdriveenv-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:56:16.710903 torchdriveenv-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/examples/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:56:16.706903 torchdriveenv-0.1.1/examples/env_configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:56:16.710903 torchdriveenv-0.1.1/examples/env_configs/multi_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/examples/env_configs/multi_agent/a2c_training.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/examples/env_configs/multi_agent/ppo_training.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/examples/env_configs/multi_agent/sac_training.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/examples/env_configs/multi_agent/td3_training.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:56:16.710903 torchdriveenv-0.1.1/examples/env_configs/single_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/examples/env_configs/single_agent/a2c_training.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/examples/env_configs/single_agent/ppo_training.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/examples/env_configs/single_agent/sac_training.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/examples/env_configs/single_agent/td3_training.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/examples/rl_training.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      393 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/examples/train.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/examples/waypoint_suite_env_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/examples/waypoint_suite_evaluation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 00:56:16.746903 torchdriveenv-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:56:16.714903 torchdriveenv-0.1.1/torchdriveenv/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:56:16.714903 torchdriveenv-0.1.1/torchdriveenv/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    38777 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/data/training_cases.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    34899 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/data/validation_cases.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/env_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21887 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/gym_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/iai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:56:16.706903 torchdriveenv-0.1.1/torchdriveenv/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:56:16.742903 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/
+-rw-r--r--   0 runner    (1001) docker     (127)   164574 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_10_634.json
+-rw-r--r--   0 runner    (1001) docker     (127)   244747 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_15_15.json
+-rw-r--r--   0 runner    (1001) docker     (127)   235631 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_15_575.json
+-rw-r--r--   0 runner    (1001) docker     (127)   236037 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_15_673.json
+-rw-r--r--   0 runner    (1001) docker     (127)   229150 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_15_770.json
+-rw-r--r--   0 runner    (1001) docker     (127)   289240 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_18_22.json
+-rw-r--r--   0 runner    (1001) docker     (127)   283754 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_18_268.json
+-rw-r--r--   0 runner    (1001) docker     (127)   285506 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_18_654.json
+-rw-r--r--   0 runner    (1001) docker     (127)    80980 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_5_306.json
+-rw-r--r--   0 runner    (1001) docker     (127)    83971 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_5_57.json
+-rw-r--r--   0 runner    (1001) docker     (127)   164528 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_10_131.json
+-rw-r--r--   0 runner    (1001) docker     (127)   233031 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_142.json
+-rw-r--r--   0 runner    (1001) docker     (127)   228878 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_270.json
+-rw-r--r--   0 runner    (1001) docker     (127)   232657 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_342.json
+-rw-r--r--   0 runner    (1001) docker     (127)   241607 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_568.json
+-rw-r--r--   0 runner    (1001) docker     (127)   228907 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_795.json
+-rw-r--r--   0 runner    (1001) docker     (127)   242169 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_9.json
+-rw-r--r--   0 runner    (1001) docker     (127)   252569 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_920.json
+-rw-r--r--   0 runner    (1001) docker     (127)   292355 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_141.json
+-rw-r--r--   0 runner    (1001) docker     (127)   297252 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_229.json
+-rw-r--r--   0 runner    (1001) docker     (127)   276077 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_345.json
+-rw-r--r--   0 runner    (1001) docker     (127)   290439 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_356.json
+-rw-r--r--   0 runner    (1001) docker     (127)   285721 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_501.json
+-rw-r--r--   0 runner    (1001) docker     (127)   291932 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_515.json
+-rw-r--r--   0 runner    (1001) docker     (127)   283201 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_682.json
+-rw-r--r--   0 runner    (1001) docker     (127)   292148 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_746.json
+-rw-r--r--   0 runner    (1001) docker     (127)   281006 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_749.json
+-rw-r--r--   0 runner    (1001) docker     (127)   282515 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_998.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84398 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_5_16.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84076 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_5_928.json
+-rw-r--r--   0 runner    (1001) docker     (127)   154723 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_216.json
+-rw-r--r--   0 runner    (1001) docker     (127)   165661 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_271.json
+-rw-r--r--   0 runner    (1001) docker     (127)   168352 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_294.json
+-rw-r--r--   0 runner    (1001) docker     (127)   168294 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_315.json
+-rw-r--r--   0 runner    (1001) docker     (127)   165254 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_378.json
+-rw-r--r--   0 runner    (1001) docker     (127)   167515 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_42.json
+-rw-r--r--   0 runner    (1001) docker     (127)   168309 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_443.json
+-rw-r--r--   0 runner    (1001) docker     (127)   168616 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_522.json
+-rw-r--r--   0 runner    (1001) docker     (127)   168448 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_542.json
+-rw-r--r--   0 runner    (1001) docker     (127)   161935 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_565.json
+-rw-r--r--   0 runner    (1001) docker     (127)   161887 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_663.json
+-rw-r--r--   0 runner    (1001) docker     (127)   168553 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_701.json
+-rw-r--r--   0 runner    (1001) docker     (127)   164839 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_733.json
+-rw-r--r--   0 runner    (1001) docker     (127)   153775 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_757.json
+-rw-r--r--   0 runner    (1001) docker     (127)   165044 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_816.json
+-rw-r--r--   0 runner    (1001) docker     (127)   168037 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_839.json
+-rw-r--r--   0 runner    (1001) docker     (127)   164153 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_932.json
+-rw-r--r--   0 runner    (1001) docker     (127)   164917 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_948.json
+-rw-r--r--   0 runner    (1001) docker     (127)   168411 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_96.json
+-rw-r--r--   0 runner    (1001) docker     (127)   165352 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_993.json
+-rw-r--r--   0 runner    (1001) docker     (127)   164127 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_10_31.json
+-rw-r--r--   0 runner    (1001) docker     (127)   161910 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_10_760.json
+-rw-r--r--   0 runner    (1001) docker     (127)   212721 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_15_103.json
+-rw-r--r--   0 runner    (1001) docker     (127)   212766 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_15_205.json
+-rw-r--r--   0 runner    (1001) docker     (127)   235880 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_15_447.json
+-rw-r--r--   0 runner    (1001) docker     (127)   245696 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_15_863.json
+-rw-r--r--   0 runner    (1001) docker     (127)   289503 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_18_416.json
+-rw-r--r--   0 runner    (1001) docker     (127)    72724 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_328.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84713 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_407.json
+-rw-r--r--   0 runner    (1001) docker     (127)    77004 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_564.json
+-rw-r--r--   0 runner    (1001) docker     (127)    80235 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_810.json
+-rw-r--r--   0 runner    (1001) docker     (127)    68038 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_844.json
+-rw-r--r--   0 runner    (1001) docker     (127)    72411 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_925.json
+-rw-r--r--   0 runner    (1001) docker     (127)    69370 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_945.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84531 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_98.json
+-rw-r--r--   0 runner    (1001) docker     (127)   217126 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_15_257.json
+-rw-r--r--   0 runner    (1001) docker     (127)   248587 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_15_605.json
+-rw-r--r--   0 runner    (1001) docker     (127)   249459 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_15_647.json
+-rw-r--r--   0 runner    (1001) docker     (127)   253756 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_15_676.json
+-rw-r--r--   0 runner    (1001) docker     (127)   262930 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_18_230.json
+-rw-r--r--   0 runner    (1001) docker     (127)   300677 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_18_451.json
+-rw-r--r--   0 runner    (1001) docker     (127)   300262 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_18_742.json
+-rw-r--r--   0 runner    (1001) docker     (127)    73086 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_5_417.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84856 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_5_576.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84867 2024-05-07 00:56:08.000000 torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_5_840.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:56:16.742903 torchdriveenv-0.1.1/torchdriveenv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-07 00:56:16.000000 torchdriveenv-0.1.1/torchdriveenv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-05-07 00:56:16.000000 torchdriveenv-0.1.1/torchdriveenv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 00:56:16.000000 torchdriveenv-0.1.1/torchdriveenv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 00:56:16.000000 torchdriveenv-0.1.1/torchdriveenv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-07 00:56:16.000000 torchdriveenv-0.1.1/torchdriveenv.egg-info/top_level.txt
```

### Comparing `torchdriveenv-0.1.0/.github/workflows/publish-to-pypi.yml` & `torchdriveenv-0.1.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/.github/workflows/publish-to-test-pypi.yml` & `torchdriveenv-0.1.1/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/.gitignore` & `torchdriveenv-0.1.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 *.so
 
 # Logging folders
 examples/runs*
 examples/videos*
 examples/wandb*
 examples/models*
+examples/eval_*
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
```

### Comparing `torchdriveenv-0.1.0/Dockerfile` & `torchdriveenv-0.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/PKG-INFO` & `torchdriveenv-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchdriveenv
-Version: 0.1.0
+Version: 0.1.1
 Summary: TorchDriveEnv is a lightweight 2D driving reinforcement learning environment, supported by a solid simulator and smart non-playable characters
 Author-email: "Inverted AI Ltd." <info@inverted.ai>
 Keywords: reinforcement learning,drive,RL environment,torch-drive-env,torchdriveenv,invertedai,inverted ai
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
```

### Comparing `torchdriveenv-0.1.0/README.md` & `torchdriveenv-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/docker-compose.yml` & `torchdriveenv-0.1.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/examples/common.py` & `torchdriveenv-0.1.1/examples/common.py`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/examples/env_configs/rl_training.yml` & `torchdriveenv-0.1.1/examples/env_configs/single_agent/a2c_training.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-algorithm: sac
-project: "stable_baselines3" 
-total_timesteps: 5e6
+algorithm: a2c
+project: "paper-experiments" 
+total_timesteps: 1e6
 parallel_env_num: 10
 record_training_examples: true  
 
 wandb_callback:
   verbose: true
   gradient_save_freq: -1
   model_save_freq: 1000
```

### Comparing `torchdriveenv-0.1.0/examples/rl_training.py` & `torchdriveenv-0.1.1/examples/rl_training.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import time
 import torch
 import wandb
 import gymnasium as gym
 from typing import Any, Dict
+import argparse
 
 from stable_baselines3 import SAC, PPO, A2C, TD3
 from stable_baselines3.common.monitor import Monitor
 from stable_baselines3.common.vec_env import VecVideoRecorder, VecFrameStack, SubprocVecEnv
 from stable_baselines3.common.callbacks import BaseCallback
 from stable_baselines3.common.evaluation import evaluate_policy
 from wandb.integration.sb3 import WandbCallback
 
 import torchdriveenv
 from torchdriveenv.env_utils import load_default_train_data, load_default_validation_data
 
 from common import BaselineAlgorithm, load_rl_training_config
 
-rl_training_config = load_rl_training_config("env_configs/rl_training.yml")
-env_config = rl_training_config.env
 training_data = load_default_train_data()
 validation_data = load_default_validation_data()
 
-
 class EvalNTimestepsCallback(BaseCallback):
     """
     Trigger a callback every ``n_steps`` timesteps
 
     :param n_steps: Number of timesteps between two trigger.
     :param eval_n_episodes: How many episodes to evaluate each time
     """
@@ -116,28 +114,42 @@
 
     def _on_step(self) -> bool:
         if (self.num_timesteps - self.last_time_trigger) >= self.n_steps:
             self.last_time_trigger = self.num_timesteps
             self._evaluate()
         return True
 
-def make_env():
+def make_env_(env_config):
     env = gym.make('torchdriveenv-v0', args={'cfg': env_config, 'data': training_data})
     env = Monitor(env)
     return env
 
-
-def make_val_env():
+def make_val_env_(env_config):
     env = gym.make('torchdriveenv-v0', args={'cfg': env_config, 'data': validation_data})
     env = Monitor(env, info_keywords=("offroad", "collision", "traffic_light_violation"))
     return env
 
-
 if __name__=='__main__':
-    config = {"policy_type": "CnnPolicy", "total_timesteps": rl_training_config.total_timesteps}
+    
+    parser = argparse.ArgumentParser(
+                    prog='tde_examples',
+                    description='execute benchmarks for tde')
+    parser.add_argument("--config_file", type=str, default="env_configs/single_agent/sac_training.yml")  
+    args = parser.parse_args()
+    
+    rl_training_config = load_rl_training_config(args.config_file)
+    env_config = rl_training_config.env
+
+    make_env = lambda: make_env_(env_config)
+    make_val_env = lambda: make_val_env_(env_config)
+    
+    config = {k:v for (k,v) in vars(rl_training_config).items() if isinstance(v, (float, int, str, list, dict, tuple, bool))}
+    config.update( {'env-'+k:v for (k,v) in vars(rl_training_config.env).items() if isinstance(v, (float, int, str, list, dict, tuple, bool))})
+    config.update( {'tds-'+k:v for (k,v) in vars(rl_training_config.env.simulator).items() if isinstance(v, (float, int, str, list, dict, tuple, bool))})
+     
     experiment_name = f"{rl_training_config.algorithm}_{int(time.time())}"
     wandb.init(
         name=experiment_name,
         project=rl_training_config.project,
         config=config,
         sync_tensorboard=True,
         monitor_gym=True,
@@ -148,28 +160,31 @@
     env = VecFrameStack(env, n_stack=rl_training_config.env.frame_stack, channels_order="first")
     
     if rl_training_config.record_training_examples:
         env = VecVideoRecorder(env, "videos",
             record_video_trigger=lambda x: x % 1000 == 0, video_length=200)  # record videos
 
     if rl_training_config.algorithm == BaselineAlgorithm.sac:
-        model = SAC(config["policy_type"], env, verbose=1, tensorboard_log=f"runs/{experiment_name}",
+        model = SAC("CnnPolicy", env, verbose=1, tensorboard_log=f"runs/{experiment_name}",
                     policy_kwargs={'optimizer_class':torch.optim.Adam})
 
     if rl_training_config.algorithm == BaselineAlgorithm.ppo:
-        model = PPO(config["policy_type"], env, verbose=1, tensorboard_log=f"runs/{experiment_name}",
-                    policy_kwargs={'optimizer_class':torch.optim.Adam})
+        model = PPO("CnnPolicy", env, verbose=1, tensorboard_log=f"runs/{experiment_name}",
+                    policy_kwargs={'optimizer_class':torch.optim.Adam}, 
+                    batch_size=256, n_epochs=5, ent_coef=0.01)
 
     if rl_training_config.algorithm == BaselineAlgorithm.a2c:
-        model = A2C(config["policy_type"], env, verbose=1, tensorboard_log=f"runs/{experiment_name}",
-                    policy_kwargs={'optimizer_class':torch.optim.Adam})
+        model = A2C("CnnPolicy", env, verbose=1, tensorboard_log=f"runs/{experiment_name}",
+                    policy_kwargs={'optimizer_class':torch.optim.Adam}, 
+                    n_steps=int(256/rl_training_config.parallel_env_num), gae_lambda=0.95, ent_coef=0.01)
 
     if rl_training_config.algorithm == BaselineAlgorithm.td3:
-        model = TD3(config["policy_type"], env, verbose=1, tensorboard_log=f"runs/{experiment_name}",
-                    policy_kwargs={'optimizer_class':torch.optim.Adam}, train_freq=1, gradient_steps=1)
+        model = TD3("CnnPolicy", env, verbose=1, tensorboard_log=f"runs/{experiment_name}",
+                    policy_kwargs={'optimizer_class':torch.optim.Adam}, 
+                    train_freq=1, gradient_steps=1)
  
     eval_val_env = SubprocVecEnv([make_val_env])
     eval_val_env = VecFrameStack(eval_val_env, n_stack=rl_training_config.env.frame_stack, channels_order="first")
     eval_val_callback = EvalNTimestepsCallback(eval_val_env, n_steps=rl_training_config.eval_val_callback['n_steps'], 
                                                  eval_n_episodes=rl_training_config.eval_val_callback['eval_n_episodes'], 
                                                  deterministic=rl_training_config.eval_val_callback['deterministic'], log_tab="eval_val")
```

### Comparing `torchdriveenv-0.1.0/examples/waypoint_suite_env_example.ipynb` & `torchdriveenv-0.1.1/examples/waypoint_suite_env_example.ipynb`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/examples/waypoint_suite_evaluation.ipynb` & `torchdriveenv-0.1.1/examples/waypoint_suite_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/pyproject.toml` & `torchdriveenv-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/requirements.txt` & `torchdriveenv-0.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/data/training_cases.yml` & `torchdriveenv-0.1.1/torchdriveenv/data/training_cases.yml`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/data/validation_cases.yml` & `torchdriveenv-0.1.1/torchdriveenv/data/validation_cases.yml`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/env_utils.py` & `torchdriveenv-0.1.1/torchdriveenv/env_utils.py`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/gym_env.py` & `torchdriveenv-0.1.1/torchdriveenv/gym_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,24 +413,29 @@
     def is_terminated(self):
         if self.config.terminated_at_infraction:
             return ((self.simulator.compute_offroad() > 0) or (self.simulator.compute_collision() > 0) or ((self.simulator.compute_traffic_lights_violations()) > 0)).item()
         else:
             return False
 
     def get_info(self):
+        x = self.simulator.get_state()[..., 0]
+        y = self.simulator.get_state()[..., 1]
         psi = self.simulator.get_state()[..., 2]
         speed = self.simulator.get_state()[..., 3]
+        d = math.dist((x, y), (self.last_x, self.last_y)) if (self.last_x is not None) and (self.last_y is not None) else 0
         reached_waypoint_num = self.reached_waypoint_num
         self.info = dict(
             offroad=self.simulator.compute_offroad(),
             collision=self.simulator.compute_collision(),
             traffic_light_violation=self.simulator.compute_traffic_lights_violations(),
             is_success=(self.environment_steps >= self.max_environment_steps),
             reached_waypoint_num=reached_waypoint_num,
             psi_smoothness=((self.last_psi - psi) / 0.1).norm(p=2).item(),
+            psi_reward=(1 - math.cos(psi - self.last_psi)) * (- self.config.heading_penalty),
+            dist_reward=self.config.distance_bonus if d > self.config.distance_cutoff else 0,
             speed_smoothness=((self.last_speed - speed) / 0.1).norm(p=2).item()
         )
         return self.info
 
 
 class SingleAgentWrapper(gym.Wrapper):
     """
```

### Comparing `torchdriveenv-0.1.0/torchdriveenv/helpers.py` & `torchdriveenv-0.1.1/torchdriveenv/helpers.py`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/iai.py` & `torchdriveenv-0.1.1/torchdriveenv/iai.py`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_10_634.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_10_634.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_15_15.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_15_15.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_15_575.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_15_575.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_15_673.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_15_673.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_15_770.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_15_770.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_18_22.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_18_22.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_18_268.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_18_268.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_18_654.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_18_654.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_5_306.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_5_306.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town01_5_57.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town01_5_57.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_10_131.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_10_131.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_142.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_142.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_270.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_270.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_342.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_342.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_568.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_568.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_795.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_795.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_9.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_9.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_15_920.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_15_920.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_141.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_141.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_229.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_229.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_345.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_345.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_356.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_356.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_501.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_501.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_515.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_515.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_682.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_682.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_746.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_746.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_749.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_749.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_18_998.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_18_998.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_5_16.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_5_16.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town02_5_928.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town02_5_928.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_216.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_216.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_271.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_271.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_294.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_294.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_315.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_315.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_378.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_378.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_42.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_42.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_443.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_443.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_522.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_522.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_542.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_542.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_565.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_565.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_663.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_663.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_701.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_701.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_733.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_733.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_757.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_757.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_816.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_816.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_839.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_839.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_932.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_932.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_948.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_948.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_96.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_96.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town03_5_993.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town03_5_993.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_10_31.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_10_31.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_10_760.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_10_760.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_15_103.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_15_103.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_15_205.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_15_205.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_15_447.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_15_447.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_15_863.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_15_863.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_18_416.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_18_416.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_328.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_328.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_407.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_407.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_564.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_564.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_810.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_810.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_844.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_844.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_925.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_925.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_945.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_945.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town07_5_98.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town07_5_98.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_15_257.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_15_257.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_15_605.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_15_605.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_15_647.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_15_647.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_15_676.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_15_676.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_18_230.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_18_230.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_18_451.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_18_451.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_18_742.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_18_742.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_5_417.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_5_417.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_5_576.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_5_576.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv/resources/background_traffic/carla_Town10HD_5_840.json` & `torchdriveenv-0.1.1/torchdriveenv/resources/background_traffic/carla_Town10HD_5_840.json`

 * *Files identical despite different names*

### Comparing `torchdriveenv-0.1.0/torchdriveenv.egg-info/PKG-INFO` & `torchdriveenv-0.1.1/torchdriveenv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchdriveenv
-Version: 0.1.0
+Version: 0.1.1
 Summary: TorchDriveEnv is a lightweight 2D driving reinforcement learning environment, supported by a solid simulator and smart non-playable characters
 Author-email: "Inverted AI Ltd." <info@inverted.ai>
 Keywords: reinforcement learning,drive,RL environment,torch-drive-env,torchdriveenv,invertedai,inverted ai
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
```

### Comparing `torchdriveenv-0.1.0/torchdriveenv.egg-info/SOURCES.txt` & `torchdriveenv-0.1.1/torchdriveenv.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,22 @@
 .github/workflows/publish-to-pypi.yml
 .github/workflows/publish-to-test-pypi.yml
 examples/common.py
 examples/rl_training.py
 examples/train.sh
 examples/waypoint_suite_env_example.ipynb
 examples/waypoint_suite_evaluation.ipynb
-examples/env_configs/rl_training.yml
+examples/env_configs/multi_agent/a2c_training.yml
+examples/env_configs/multi_agent/ppo_training.yml
+examples/env_configs/multi_agent/sac_training.yml
+examples/env_configs/multi_agent/td3_training.yml
+examples/env_configs/single_agent/a2c_training.yml
+examples/env_configs/single_agent/ppo_training.yml
+examples/env_configs/single_agent/sac_training.yml
+examples/env_configs/single_agent/td3_training.yml
 torchdriveenv/__init__.py
 torchdriveenv/env_utils.py
 torchdriveenv/gym_env.py
 torchdriveenv/helpers.py
 torchdriveenv/iai.py
 torchdriveenv.egg-info/PKG-INFO
 torchdriveenv.egg-info/SOURCES.txt
```

