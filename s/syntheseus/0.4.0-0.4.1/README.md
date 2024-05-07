# Comparing `tmp/syntheseus-0.4.0.tar.gz` & `tmp/syntheseus-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntheseus-0.4.0.tar", last modified: Thu Apr 11 11:14:44 2024, max compression
+gzip compressed data, was "syntheseus-0.4.1.tar", last modified: Tue May  7 15:55:30 2024, max compression
```

## Comparing `syntheseus-0.4.0.tar` & `syntheseus-0.4.1.tar`

### file list

```diff
@@ -1,203 +1,204 @@
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.921803 syntheseus-0.4.0/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      509 2024-04-11 11:13:34.000000 syntheseus-0.4.0/.coveragerc
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.897803 syntheseus-0.4.0/.github/
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.901803 syntheseus-0.4.0/.github/azure_pipelines/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      528 2024-04-11 11:13:34.000000 syntheseus-0.4.0/.github/azure_pipelines/code-security-analysis.yml
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.901803 syntheseus-0.4.0/.github/workflows/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2618 2024-04-11 11:13:34.000000 syntheseus-0.4.0/.github/workflows/ci.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      991 2024-04-11 11:13:34.000000 syntheseus-0.4.0/.github/workflows/docs.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      701 2024-04-11 11:13:41.000000 syntheseus-0.4.0/.github/workflows/release.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      382 2024-04-11 11:13:34.000000 syntheseus-0.4.0/.gitignore
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1643 2024-04-11 11:13:34.000000 syntheseus-0.4.0/.pre-commit-config.yaml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7228 2024-04-11 11:13:34.000000 syntheseus-0.4.0/CHANGELOG.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      444 2024-04-11 11:13:34.000000 syntheseus-0.4.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1141 2024-04-11 11:13:34.000000 syntheseus-0.4.0/LICENSE
--rw-r--r--   0 krmaziar  (1001) krmaziar  (1002)     6793 2024-04-11 11:14:44.921803 syntheseus-0.4.0/PKG-INFO
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3747 2024-04-11 11:13:34.000000 syntheseus-0.4.0/README.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2756 2024-04-11 11:13:34.000000 syntheseus-0.4.0/SECURITY.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      504 2024-04-11 11:13:34.000000 syntheseus-0.4.0/SUPPORT.md
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.901803 syntheseus-0.4.0/docs/
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/docs/cli/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2662 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/cli/eval_single_step.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1579 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/cli/search.md
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/docs/images/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    95644 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/images/logo.png
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2201 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/images/logo.svg
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1242 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/index.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3157 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/installation.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2381 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/single_step.md
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/docs/tutorials/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       65 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/tutorials/.gitignore
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    11918 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/tutorials/custom_model.ipynb
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    44305 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/tutorials/paroutes_benchmark.ipynb
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     8296 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/tutorials/quick_start.ipynb
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      130 2024-04-11 11:13:34.000000 syntheseus-0.4.0/environment.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      341 2024-04-11 11:13:34.000000 syntheseus-0.4.0/environment_full.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1290 2024-04-11 11:13:34.000000 syntheseus-0.4.0/mkdocs.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2794 2024-04-11 11:13:34.000000 syntheseus-0.4.0/pyproject.toml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       38 2024-04-11 11:14:44.921803 syntheseus-0.4.0/setup.cfg
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      430 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/cli/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/cli/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    17900 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/cli/eval_single_step.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      714 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/cli/main.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    15167 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/cli/search.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1247 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/cli/search_config.yml
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/interface/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/interface/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1174 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/interface/bag.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7054 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/interface/models.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3186 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/interface/molecule.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2933 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/interface/reaction.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      372 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/interface/typed_dict.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/py.typed
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/reaction_prediction/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/reaction_prediction/chem/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/chem/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1192 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/chem/utils.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/reaction_prediction/cli/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/cli/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/reaction_prediction/data/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/data/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5378 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/data/dataset.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2858 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/data/reaction_sample.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.909803 syntheseus-0.4.0/syntheseus/reaction_prediction/environment_gln/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1321 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/environment_gln/Dockerfile
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      455 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/environment_gln/environment.yml
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.909803 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      988 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1491 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/base.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6156 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/chemformer.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1198 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/config.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      563 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/default_checkpoint_links.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3265 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/gln.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3862 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/graph2edits.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5742 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/local_retro.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7142 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/megan.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7138 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/mhnreact.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4882 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/retro_knn.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    11041 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/root_aligned.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3943 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/toy_models.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.909803 syntheseus-0.4.0/syntheseus/reaction_prediction/models/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/models/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2363 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/models/retro_knn.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.909803 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2246 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/config.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2378 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/downloading.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3281 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/inference.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1618 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/metrics.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3968 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/misc.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1644 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/model_loading.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1855 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/parallel.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      737 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/testing.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.909803 syntheseus-0.4.0/syntheseus/search/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       95 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.909803 syntheseus-0.4.0/syntheseus/search/algorithms/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    15847 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/base.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/algorithms/best_first/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/best_first/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     8108 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/best_first/base.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    11974 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/best_first/retro_star.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2103 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/breadth_first.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/algorithms/mcts/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/mcts/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    12737 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/mcts/base.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      299 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/mcts/molset.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      895 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/mixins.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    18103 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/pdvn.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2133 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/random.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/analysis/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/analysis/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    10226 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/analysis/diversity.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     9772 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/analysis/route_extraction.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2622 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/analysis/solution_time.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/graph/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     9079 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/and_or.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4892 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/base_graph.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/graph/message_passing/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      266 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/message_passing/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6413 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/message_passing/run.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      834 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/message_passing/update_functions.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7558 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/molset.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3984 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/node.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2897 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/route.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6861 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/standardization.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1901 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/mol_inventory.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/node_evaluation/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      102 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/node_evaluation/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6048 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/node_evaluation/base.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2201 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/node_evaluation/common.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/utils/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/utils/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       69 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/utils/misc.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6477 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/visualization.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/tests/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/tests/cli/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/cli/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5562 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/cli/test_cli.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6166 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/cli/test_eval_single_step.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      925 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/conftest.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/tests/interface/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/interface/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      556 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/interface/test_bag.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5867 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/interface/test_models.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4595 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/interface/test_molecule.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3146 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/interface/test_reaction.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1331 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/interface/test_toy_models.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/chem/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/chem/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      561 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/chem/test_utils.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/data/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/data/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5288 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/data/test_dataset.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/inference/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/inference/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1773 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/inference/test_models.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/utils/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/utils/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      573 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/utils/test_misc.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/search/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/search/algorithms/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    25001 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_base.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    13331 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_best_first.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    10793 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_breadth_first.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    13280 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_mcts.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    15592 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_pdvn.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1703 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_random.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/search/analysis/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/analysis/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1691 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/analysis/conftest.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4029 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/analysis/test_diversity.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     9974 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/analysis/test_route_extraction.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      109 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/analysis/test_solution_time.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    14701 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/conftest.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/search/graph/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7208 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/test_andor.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      541 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/test_base.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4587 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/test_message_passing.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5132 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/test_molset.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      292 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/test_route.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      776 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/test_standardization.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/search/node_evaluation/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/node_evaluation/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5848 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/node_evaluation/test_common.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2321 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/test_mol_inventory.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2094 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/test_visualization.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus.egg-info/
--rw-r--r--   0 krmaziar  (1001) krmaziar  (1002)     6793 2024-04-11 11:14:44.000000 syntheseus-0.4.0/syntheseus.egg-info/PKG-INFO
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6416 2024-04-11 11:14:44.000000 syntheseus-0.4.0/syntheseus.egg-info/SOURCES.txt
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        1 2024-04-11 11:14:44.000000 syntheseus-0.4.0/syntheseus.egg-info/dependency_links.txt
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       56 2024-04-11 11:14:44.000000 syntheseus-0.4.0/syntheseus.egg-info/entry_points.txt
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      562 2024-04-11 11:14:44.000000 syntheseus-0.4.0/syntheseus.egg-info/requires.txt
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       11 2024-04-11 11:14:44.000000 syntheseus-0.4.0/syntheseus.egg-info/top_level.txt
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.779495 syntheseus-0.4.1/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      509 2024-04-15 12:52:06.000000 syntheseus-0.4.1/.coveragerc
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.751495 syntheseus-0.4.1/.github/
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.755495 syntheseus-0.4.1/.github/azure_pipelines/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      528 2024-04-15 12:52:06.000000 syntheseus-0.4.1/.github/azure_pipelines/code-security-analysis.yml
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.755495 syntheseus-0.4.1/.github/workflows/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2618 2024-04-15 12:52:06.000000 syntheseus-0.4.1/.github/workflows/ci.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      991 2024-04-15 12:52:06.000000 syntheseus-0.4.1/.github/workflows/docs.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      701 2024-04-15 12:52:06.000000 syntheseus-0.4.1/.github/workflows/release.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      382 2024-04-15 12:52:06.000000 syntheseus-0.4.1/.gitignore
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1643 2024-04-15 12:52:06.000000 syntheseus-0.4.1/.pre-commit-config.yaml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7571 2024-05-07 15:54:40.000000 syntheseus-0.4.1/CHANGELOG.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      444 2024-04-11 11:13:34.000000 syntheseus-0.4.1/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1397 2024-04-15 12:52:06.000000 syntheseus-0.4.1/DEVELOPMENT.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1141 2024-04-11 11:13:34.000000 syntheseus-0.4.1/LICENSE
+-rw-r--r--   0 krmaziar  (1001) krmaziar  (1002)     6793 2024-05-07 15:55:30.779495 syntheseus-0.4.1/PKG-INFO
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3747 2024-04-15 12:52:06.000000 syntheseus-0.4.1/README.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2756 2024-04-11 11:13:34.000000 syntheseus-0.4.1/SECURITY.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      504 2024-04-11 11:13:34.000000 syntheseus-0.4.1/SUPPORT.md
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.755495 syntheseus-0.4.1/docs/
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.755495 syntheseus-0.4.1/docs/cli/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2662 2024-04-15 12:52:06.000000 syntheseus-0.4.1/docs/cli/eval_single_step.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1579 2024-04-15 12:52:06.000000 syntheseus-0.4.1/docs/cli/search.md
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.759495 syntheseus-0.4.1/docs/images/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    95644 2024-04-15 12:52:06.000000 syntheseus-0.4.1/docs/images/logo.png
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2201 2024-04-15 12:52:06.000000 syntheseus-0.4.1/docs/images/logo.svg
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1242 2024-04-15 12:52:06.000000 syntheseus-0.4.1/docs/index.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3157 2024-04-15 12:52:06.000000 syntheseus-0.4.1/docs/installation.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2381 2024-04-29 11:41:42.000000 syntheseus-0.4.1/docs/single_step.md
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.759495 syntheseus-0.4.1/docs/tutorials/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       65 2024-04-15 12:52:06.000000 syntheseus-0.4.1/docs/tutorials/.gitignore
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    11918 2024-04-15 12:52:06.000000 syntheseus-0.4.1/docs/tutorials/custom_model.ipynb
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    44305 2024-04-15 12:52:06.000000 syntheseus-0.4.1/docs/tutorials/paroutes_benchmark.ipynb
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     8296 2024-04-15 12:52:06.000000 syntheseus-0.4.1/docs/tutorials/quick_start.ipynb
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      130 2024-04-15 12:52:06.000000 syntheseus-0.4.1/environment.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      341 2024-04-15 12:52:06.000000 syntheseus-0.4.1/environment_full.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1290 2024-04-15 12:52:06.000000 syntheseus-0.4.1/mkdocs.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2794 2024-04-15 12:52:06.000000 syntheseus-0.4.1/pyproject.toml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       38 2024-05-07 15:55:30.779495 syntheseus-0.4.1/setup.cfg
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.763495 syntheseus-0.4.1/syntheseus/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      430 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.763495 syntheseus-0.4.1/syntheseus/cli/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/cli/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    17900 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/cli/eval_single_step.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      714 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/cli/main.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    15167 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/cli/search.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1247 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/cli/search_config.yml
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.763495 syntheseus-0.4.1/syntheseus/interface/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/interface/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1174 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/interface/bag.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7054 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/interface/models.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3186 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/interface/molecule.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2933 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/interface/reaction.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      372 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/interface/typed_dict.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/py.typed
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.763495 syntheseus-0.4.1/syntheseus/reaction_prediction/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.763495 syntheseus-0.4.1/syntheseus/reaction_prediction/chem/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/chem/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1192 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/chem/utils.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.763495 syntheseus-0.4.1/syntheseus/reaction_prediction/cli/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/cli/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.763495 syntheseus-0.4.1/syntheseus/reaction_prediction/data/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/data/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5378 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/data/dataset.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2858 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/data/reaction_sample.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.763495 syntheseus-0.4.1/syntheseus/reaction_prediction/environment_gln/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1321 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/environment_gln/Dockerfile
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      455 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/environment_gln/environment.yml
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.767495 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      988 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1491 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/base.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6156 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/chemformer.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1198 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/config.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      563 2024-04-29 11:41:42.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/default_checkpoint_links.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3373 2024-04-29 11:41:42.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/gln.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3862 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/graph2edits.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5742 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/local_retro.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7142 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/megan.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7138 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/mhnreact.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4882 2024-04-15 15:52:01.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/retro_knn.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    11041 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/root_aligned.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3943 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/inference/toy_models.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.767495 syntheseus-0.4.1/syntheseus/reaction_prediction/models/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/models/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2363 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/models/retro_knn.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.767495 syntheseus-0.4.1/syntheseus/reaction_prediction/utils/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/utils/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2246 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/utils/config.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2378 2024-04-15 14:13:22.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/utils/downloading.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3281 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/utils/inference.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1618 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/utils/metrics.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3968 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/utils/misc.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1644 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/utils/model_loading.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1855 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/utils/parallel.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      737 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/reaction_prediction/utils/testing.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.767495 syntheseus-0.4.1/syntheseus/search/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       95 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.767495 syntheseus-0.4.1/syntheseus/search/algorithms/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/algorithms/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    15847 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/algorithms/base.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.767495 syntheseus-0.4.1/syntheseus/search/algorithms/best_first/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/algorithms/best_first/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     8108 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/algorithms/best_first/base.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    11974 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/algorithms/best_first/retro_star.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2103 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/algorithms/breadth_first.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.767495 syntheseus-0.4.1/syntheseus/search/algorithms/mcts/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/algorithms/mcts/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    12737 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/algorithms/mcts/base.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      299 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/algorithms/mcts/molset.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      895 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/algorithms/mixins.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    18103 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/algorithms/pdvn.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2133 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/algorithms/random.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.767495 syntheseus-0.4.1/syntheseus/search/analysis/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/analysis/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    10226 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/analysis/diversity.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     9772 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/analysis/route_extraction.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2622 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/analysis/solution_time.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.771495 syntheseus-0.4.1/syntheseus/search/graph/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/graph/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     9079 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/graph/and_or.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4892 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/graph/base_graph.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.771495 syntheseus-0.4.1/syntheseus/search/graph/message_passing/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      266 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/graph/message_passing/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6413 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/graph/message_passing/run.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      834 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/graph/message_passing/update_functions.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7558 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/graph/molset.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3984 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/graph/node.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2897 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/graph/route.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6861 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/graph/standardization.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1901 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/mol_inventory.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.771495 syntheseus-0.4.1/syntheseus/search/node_evaluation/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      102 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/node_evaluation/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6048 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/node_evaluation/base.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2201 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/search/node_evaluation/common.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.771495 syntheseus-0.4.1/syntheseus/search/utils/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/utils/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       69 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/utils/misc.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6477 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/search/visualization.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.771495 syntheseus-0.4.1/syntheseus/tests/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.771495 syntheseus-0.4.1/syntheseus/tests/cli/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/cli/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5562 2024-04-15 15:52:01.000000 syntheseus-0.4.1/syntheseus/tests/cli/test_cli.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6166 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/cli/test_eval_single_step.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      925 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/conftest.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.771495 syntheseus-0.4.1/syntheseus/tests/interface/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/interface/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      556 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/interface/test_bag.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5867 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/interface/test_models.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4595 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/interface/test_molecule.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3146 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/interface/test_reaction.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1331 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/interface/test_toy_models.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.771495 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.771495 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/chem/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/chem/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      561 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/chem/test_utils.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.771495 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/data/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/data/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5288 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/data/test_dataset.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.771495 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/inference/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/inference/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1773 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/inference/test_models.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.771495 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/utils/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/utils/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      573 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/reaction_prediction/utils/test_misc.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.771495 syntheseus-0.4.1/syntheseus/tests/search/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.775495 syntheseus-0.4.1/syntheseus/tests/search/algorithms/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/algorithms/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    25001 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/search/algorithms/test_base.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    13331 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/search/algorithms/test_best_first.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    10793 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/algorithms/test_breadth_first.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    13280 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/algorithms/test_mcts.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    15592 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/search/algorithms/test_pdvn.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1703 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/search/algorithms/test_random.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.775495 syntheseus-0.4.1/syntheseus/tests/search/analysis/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/analysis/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1691 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/analysis/conftest.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4029 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/analysis/test_diversity.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     9974 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/analysis/test_route_extraction.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      109 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/analysis/test_solution_time.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    14701 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/search/conftest.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.775495 syntheseus-0.4.1/syntheseus/tests/search/graph/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/graph/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7208 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/search/graph/test_andor.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      541 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/graph/test_base.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4587 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/graph/test_message_passing.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5132 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/search/graph/test_molset.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      292 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/search/graph/test_route.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      776 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/graph/test_standardization.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.775495 syntheseus-0.4.1/syntheseus/tests/search/node_evaluation/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/node_evaluation/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5848 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/node_evaluation/test_common.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2321 2024-04-15 12:52:06.000000 syntheseus-0.4.1/syntheseus/tests/search/test_mol_inventory.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2094 2024-04-11 11:13:34.000000 syntheseus-0.4.1/syntheseus/tests/search/test_visualization.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-05-07 15:55:30.775495 syntheseus-0.4.1/syntheseus.egg-info/
+-rw-r--r--   0 krmaziar  (1001) krmaziar  (1002)     6793 2024-05-07 15:55:30.000000 syntheseus-0.4.1/syntheseus.egg-info/PKG-INFO
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6431 2024-05-07 15:55:30.000000 syntheseus-0.4.1/syntheseus.egg-info/SOURCES.txt
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        1 2024-05-07 15:55:30.000000 syntheseus-0.4.1/syntheseus.egg-info/dependency_links.txt
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       56 2024-05-07 15:55:30.000000 syntheseus-0.4.1/syntheseus.egg-info/entry_points.txt
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      562 2024-05-07 15:55:30.000000 syntheseus-0.4.1/syntheseus.egg-info/requires.txt
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       11 2024-05-07 15:55:30.000000 syntheseus-0.4.1/syntheseus.egg-info/top_level.txt
```

### Comparing `syntheseus-0.4.0/.github/azure_pipelines/code-security-analysis.yml` & `syntheseus-0.4.1/.github/azure_pipelines/code-security-analysis.yml`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/.github/workflows/ci.yml` & `syntheseus-0.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/.github/workflows/docs.yml` & `syntheseus-0.4.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/.github/workflows/release.yml` & `syntheseus-0.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/.pre-commit-config.yaml` & `syntheseus-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/CHANGELOG.md` & `syntheseus-0.4.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,26 @@
 All notable changes to the project are documented in this file.
 
 The format follows [Common Changelog](https://common-changelog.org/),
 and the project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.4.1] - 2024-05-04
+
+### Fixed
+
+- Fix incorrectly uploaded RetroKNN weights ([#91](https://github.com/microsoft/syntheseus/pull/91)) ([@kmaziarz])
+- Fix GLN weights and issues in its model wrapper ([#92](https://github.com/microsoft/syntheseus/pull/92)) ([@kmaziarz])
+
 ## [0.4.0] - 2024-04-10
 
 ### Changed
 
-- Merge reaction and reaction model base classes in `search` and `reaction_predction` ([#63](https://github.com/microsoft/syntheseus/pull/63), [#67](https://github.com/microsoft/syntheseus/pull/67), [#73](https://github.com/microsoft/syntheseus/pull/73), [#74](https://github.com/microsoft/syntheseus/pull/74), [#76](https://github.com/microsoft/syntheseus/pull/76), [#84](https://github.com/microsoft/syntheseus/pull/84)) ([@austint], [@kmaziarz])
+- Merge reaction and reaction model base classes in `search` and `reaction_prediction` ([#63](https://github.com/microsoft/syntheseus/pull/63), [#67](https://github.com/microsoft/syntheseus/pull/67), [#73](https://github.com/microsoft/syntheseus/pull/73), [#74](https://github.com/microsoft/syntheseus/pull/74), [#76](https://github.com/microsoft/syntheseus/pull/76), [#84](https://github.com/microsoft/syntheseus/pull/84)) ([@austint], [@kmaziarz])
 - Make reaction models return `Sequence[Reaction]` instead of `PredictionList` objects ([#61](https://github.com/microsoft/syntheseus/pull/61)) ([@austint])
 - Suppress the remaining noisy logs and warnings coming from single-step models ([#53](https://github.com/microsoft/syntheseus/pull/53)) ([@kmaziarz])
 - Improve efficiency and logging of retro* algorithm ([#62](https://github.com/microsoft/syntheseus/pull/62)) ([@austint])
 - Improve error handling in single-step evaluation and allow CLI to use the default checkpoints ([#75](https://github.com/microsoft/syntheseus/pull/75)) ([@kmaziarz])
 - Make basic classes from `interface` importable from top-level ([#81](https://github.com/microsoft/syntheseus/pull/81)) ([@austint])
 
 ### Added
@@ -76,17 +83,18 @@
 - Fix compatibility with Python 3.7 ([#5](https://github.com/microsoft/syntheseus/pull/5)) ([@kmaziarz])
 - Correct some typos and unclear error messages ([#39](https://github.com/microsoft/syntheseus/pull/39)) ([@austint])
 
 ## [0.1.0] - 2023-05-25
 
 :seedling: Initial public release, containing several multi-step search algorithms and a minimal interface for single-step models.
 
-[Unreleased]: https://github.com/microsoft/syntheseus/compare/v0.4.0...HEAD
+[Unreleased]: https://github.com/microsoft/syntheseus/compare/v0.4.1...HEAD
 [0.1.0]: https://github.com/microsoft/syntheseus/releases/tag/v0.1.0
 [0.2.0]: https://github.com/microsoft/syntheseus/releases/tag/v0.2.0
 [0.3.0]: https://github.com/microsoft/syntheseus/releases/tag/v0.3.0
 [0.4.0]: https://github.com/microsoft/syntheseus/releases/tag/v0.4.0
+[0.4.1]: https://github.com/microsoft/syntheseus/releases/tag/v0.4.1
 
 [@austint]: https://github.com/AustinT
 [@kmaziarz]: https://github.com/kmaziarz
 [@jagarridotorres]: https://github.com/jagarridotorres
 [@fiberleif]: https://github.com/fiberleif
```

### Comparing `syntheseus-0.4.0/LICENSE` & `syntheseus-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/PKG-INFO` & `syntheseus-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntheseus
-Version: 0.4.0
+Version: 0.4.1
 Summary: A package for retrosynthetic planning.
 Author: Austin Tripp, Krzysztof Maziarz, Guoqing Liu, Megan Stanley, Marwin Segler
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syntheseus Version: 0.4.0 Summary: A package for
+Metadata-Version: 2.1 Name: syntheseus Version: 0.4.1 Summary: A package for
 retrosynthetic planning. Author: Austin Tripp, Krzysztof Maziarz, Guoqing Liu,
 Megan Stanley, Marwin Segler License: MIT License Copyright (c) Microsoft
 Corporation. Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
```

### Comparing `syntheseus-0.4.0/README.md` & `syntheseus-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/SECURITY.md` & `syntheseus-0.4.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/docs/cli/eval_single_step.md` & `syntheseus-0.4.1/docs/cli/eval_single_step.md`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/docs/cli/search.md` & `syntheseus-0.4.1/docs/cli/search.md`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/docs/images/logo.png` & `syntheseus-0.4.1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/docs/images/logo.svg` & `syntheseus-0.4.1/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/docs/index.md` & `syntheseus-0.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/docs/installation.md` & `syntheseus-0.4.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/docs/single_step.md` & `syntheseus-0.4.1/docs/single_step.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 If no checkpoint directory is provided during model loading, `syntheseus` will automatically download a default checkpoint and cache it on disk for future use.
 The default path for the cache is `$HOME/.cache/torch/syntheseus`, but it can be overriden by setting the `SYNTHESEUS_CACHE_DIR` environment variable.
 See table below for the links to the default checkpoints.
 
 | Model checkpoint link                                          | Source |
 |----------------------------------------------------------------|--------|
 | [Chemformer](https://figshare.com/ndownloader/files/42009888)  | finetuned by us starting from checkpoint released by authors |
-| [GLN](https://figshare.com/ndownloader/files/42012720)         | released by authors |
+| [GLN](https://figshare.com/ndownloader/files/45882867)         | released by authors |
 | [Graph2Edits](https://figshare.com/ndownloader/files/44194301) | released by authors |
 | [LocalRetro](https://figshare.com/ndownloader/files/42287319)  | trained by us |
 | [MEGAN](https://figshare.com/ndownloader/files/42012732)       | trained by us |
 | [MHNreact](https://figshare.com/ndownloader/files/42012777)    | trained by us |
-| [RetroKNN](https://figshare.com/ndownloader/files/43636584)    | trained by us |
+| [RetroKNN](https://figshare.com/ndownloader/files/45662430)    | trained by us |
 | [RootAligned](https://figshare.com/ndownloader/files/42012792) | released by authors |
 
 ??? note "More advanced datasets"
 
     The USPTO-50K dataset is well-established but relatively small. Advanced users may prefer to retrain their models of interest on a larger dataset, such as USPTO-FULL or Pistachio. To do that, please follow the instructions in the original model repositories.
 
 In `reaction_prediction/cli/eval.py` a forward model can be used for computing back-translation (round-trip) accuracy.
```

### Comparing `syntheseus-0.4.0/docs/tutorials/custom_model.ipynb` & `syntheseus-0.4.1/docs/tutorials/custom_model.ipynb`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/docs/tutorials/paroutes_benchmark.ipynb` & `syntheseus-0.4.1/docs/tutorials/paroutes_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/docs/tutorials/quick_start.ipynb` & `syntheseus-0.4.1/docs/tutorials/quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/mkdocs.yml` & `syntheseus-0.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/pyproject.toml` & `syntheseus-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/cli/eval_single_step.py` & `syntheseus-0.4.1/syntheseus/cli/eval_single_step.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/cli/main.py` & `syntheseus-0.4.1/syntheseus/cli/main.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/cli/search.py` & `syntheseus-0.4.1/syntheseus/cli/search.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/cli/search_config.yml` & `syntheseus-0.4.1/syntheseus/cli/search_config.yml`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/interface/bag.py` & `syntheseus-0.4.1/syntheseus/interface/bag.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/interface/models.py` & `syntheseus-0.4.1/syntheseus/interface/models.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/interface/molecule.py` & `syntheseus-0.4.1/syntheseus/interface/molecule.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/interface/reaction.py` & `syntheseus-0.4.1/syntheseus/interface/reaction.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/chem/utils.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/chem/utils.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/data/dataset.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/data/dataset.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/data/reaction_sample.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/data/reaction_sample.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/environment_gln/Dockerfile` & `syntheseus-0.4.1/syntheseus/reaction_prediction/environment_gln/Dockerfile`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/__init__.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/base.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/inference/base.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/chemformer.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/inference/chemformer.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/config.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/inference/config.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/default_checkpoint_links.yml` & `syntheseus-0.4.1/syntheseus/reaction_prediction/inference/default_checkpoint_links.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 backward:
   Chemformer: https://figshare.com/ndownloader/files/42009888
-  GLN: https://figshare.com/ndownloader/files/42012720
+  GLN: https://figshare.com/ndownloader/files/45882867
   Graph2Edits: https://figshare.com/ndownloader/files/44194301
   LocalRetro: https://figshare.com/ndownloader/files/42287319
   MEGAN: https://figshare.com/ndownloader/files/42012732
   MHNreact: https://figshare.com/ndownloader/files/42012777
-  RetroKNN: https://figshare.com/ndownloader/files/43636584
+  RetroKNN: https://figshare.com/ndownloader/files/45662430
   RootAligned: https://figshare.com/ndownloader/files/42012792
 forward:
   Chemformer: https://figshare.com/ndownloader/files/42012708
```

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/gln.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/inference/gln.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,18 @@
                 sys.argv += [f"-{name}", str(value)]
 
             # The global state hackery has to happen before this.
             from gln.test.model_inference import RetroGLN
 
             self.model = RetroGLN(self.model_dir, chkpt_path)
 
+    @property
+    def name(self) -> str:
+        return "GLN"
+
     def get_parameters(self):
         return self.model.gln.parameters()
 
     def _get_model_predictions(
         self, input: Molecule, num_results: int
     ) -> Sequence[SingleProductReaction]:
         with suppress_outputs():
@@ -69,14 +73,16 @@
         if result is None:
             return []
         else:
             # `scores` are actually probabilities (produced by running `softmax`).
             return process_raw_smiles_outputs_backwards(
                 input=input,
                 output_list=result["reactants"],
-                metadata_list=[{"probability": probability} for probability in result["scores"]],
+                metadata_list=[
+                    {"probability": probability.item()} for probability in result["scores"]
+                ],
             )
 
     def _get_reactions(
         self, inputs: List[Molecule], num_results: int
     ) -> List[Sequence[SingleProductReaction]]:
         return [self._get_model_predictions(input, num_results=num_results) for input in inputs]
```

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/graph2edits.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/inference/graph2edits.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/local_retro.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/inference/local_retro.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/megan.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/inference/megan.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/mhnreact.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/inference/mhnreact.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/retro_knn.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/inference/retro_knn.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/root_aligned.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/inference/root_aligned.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/toy_models.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/inference/toy_models.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/models/retro_knn.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/models/retro_knn.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/config.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/utils/config.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/downloading.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/utils/downloading.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/inference.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/utils/inference.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/metrics.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/misc.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/utils/misc.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/model_loading.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/utils/model_loading.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/parallel.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/testing.py` & `syntheseus-0.4.1/syntheseus/reaction_prediction/utils/testing.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/algorithms/base.py` & `syntheseus-0.4.1/syntheseus/search/algorithms/base.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/algorithms/best_first/base.py` & `syntheseus-0.4.1/syntheseus/search/algorithms/best_first/base.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/algorithms/best_first/retro_star.py` & `syntheseus-0.4.1/syntheseus/search/algorithms/best_first/retro_star.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/algorithms/breadth_first.py` & `syntheseus-0.4.1/syntheseus/search/algorithms/breadth_first.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/algorithms/mcts/base.py` & `syntheseus-0.4.1/syntheseus/search/algorithms/mcts/base.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/algorithms/mixins.py` & `syntheseus-0.4.1/syntheseus/search/algorithms/mixins.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/algorithms/pdvn.py` & `syntheseus-0.4.1/syntheseus/search/algorithms/pdvn.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/algorithms/random.py` & `syntheseus-0.4.1/syntheseus/search/algorithms/random.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/analysis/diversity.py` & `syntheseus-0.4.1/syntheseus/search/analysis/diversity.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/analysis/route_extraction.py` & `syntheseus-0.4.1/syntheseus/search/analysis/route_extraction.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/analysis/solution_time.py` & `syntheseus-0.4.1/syntheseus/search/analysis/solution_time.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/graph/and_or.py` & `syntheseus-0.4.1/syntheseus/search/graph/and_or.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/graph/base_graph.py` & `syntheseus-0.4.1/syntheseus/search/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/graph/message_passing/run.py` & `syntheseus-0.4.1/syntheseus/search/graph/message_passing/run.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/graph/message_passing/update_functions.py` & `syntheseus-0.4.1/syntheseus/search/graph/message_passing/update_functions.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/graph/molset.py` & `syntheseus-0.4.1/syntheseus/search/graph/molset.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/graph/node.py` & `syntheseus-0.4.1/syntheseus/search/graph/node.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/graph/route.py` & `syntheseus-0.4.1/syntheseus/search/graph/route.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/graph/standardization.py` & `syntheseus-0.4.1/syntheseus/search/graph/standardization.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/mol_inventory.py` & `syntheseus-0.4.1/syntheseus/search/mol_inventory.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/node_evaluation/base.py` & `syntheseus-0.4.1/syntheseus/search/node_evaluation/base.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/node_evaluation/common.py` & `syntheseus-0.4.1/syntheseus/search/node_evaluation/common.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/search/visualization.py` & `syntheseus-0.4.1/syntheseus/search/visualization.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/cli/test_cli.py` & `syntheseus-0.4.1/syntheseus/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/cli/test_eval_single_step.py` & `syntheseus-0.4.1/syntheseus/tests/cli/test_eval_single_step.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/conftest.py` & `syntheseus-0.4.1/syntheseus/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/interface/test_bag.py` & `syntheseus-0.4.1/syntheseus/tests/interface/test_bag.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/interface/test_models.py` & `syntheseus-0.4.1/syntheseus/tests/interface/test_models.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/interface/test_molecule.py` & `syntheseus-0.4.1/syntheseus/tests/interface/test_molecule.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/interface/test_reaction.py` & `syntheseus-0.4.1/syntheseus/tests/interface/test_reaction.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/interface/test_toy_models.py` & `syntheseus-0.4.1/syntheseus/tests/interface/test_toy_models.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/reaction_prediction/chem/test_utils.py` & `syntheseus-0.4.1/syntheseus/tests/reaction_prediction/chem/test_utils.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/reaction_prediction/data/test_dataset.py` & `syntheseus-0.4.1/syntheseus/tests/reaction_prediction/data/test_dataset.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/reaction_prediction/inference/test_models.py` & `syntheseus-0.4.1/syntheseus/tests/reaction_prediction/inference/test_models.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/reaction_prediction/utils/test_misc.py` & `syntheseus-0.4.1/syntheseus/tests/reaction_prediction/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_base.py` & `syntheseus-0.4.1/syntheseus/tests/search/algorithms/test_base.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_best_first.py` & `syntheseus-0.4.1/syntheseus/tests/search/algorithms/test_best_first.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_breadth_first.py` & `syntheseus-0.4.1/syntheseus/tests/search/algorithms/test_breadth_first.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_mcts.py` & `syntheseus-0.4.1/syntheseus/tests/search/algorithms/test_mcts.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_pdvn.py` & `syntheseus-0.4.1/syntheseus/tests/search/algorithms/test_pdvn.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_random.py` & `syntheseus-0.4.1/syntheseus/tests/search/algorithms/test_random.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/analysis/conftest.py` & `syntheseus-0.4.1/syntheseus/tests/search/analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/analysis/test_diversity.py` & `syntheseus-0.4.1/syntheseus/tests/search/analysis/test_diversity.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/analysis/test_route_extraction.py` & `syntheseus-0.4.1/syntheseus/tests/search/analysis/test_route_extraction.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/conftest.py` & `syntheseus-0.4.1/syntheseus/tests/search/conftest.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/graph/test_andor.py` & `syntheseus-0.4.1/syntheseus/tests/search/graph/test_andor.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/graph/test_base.py` & `syntheseus-0.4.1/syntheseus/tests/search/graph/test_base.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/graph/test_message_passing.py` & `syntheseus-0.4.1/syntheseus/tests/search/graph/test_message_passing.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/graph/test_molset.py` & `syntheseus-0.4.1/syntheseus/tests/search/graph/test_molset.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/graph/test_standardization.py` & `syntheseus-0.4.1/syntheseus/tests/search/graph/test_standardization.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/node_evaluation/test_common.py` & `syntheseus-0.4.1/syntheseus/tests/search/node_evaluation/test_common.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/test_mol_inventory.py` & `syntheseus-0.4.1/syntheseus/tests/search/test_mol_inventory.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus/tests/search/test_visualization.py` & `syntheseus-0.4.1/syntheseus/tests/search/test_visualization.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.4.0/syntheseus.egg-info/PKG-INFO` & `syntheseus-0.4.1/syntheseus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntheseus
-Version: 0.4.0
+Version: 0.4.1
 Summary: A package for retrosynthetic planning.
 Author: Austin Tripp, Krzysztof Maziarz, Guoqing Liu, Megan Stanley, Marwin Segler
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syntheseus Version: 0.4.0 Summary: A package for
+Metadata-Version: 2.1 Name: syntheseus Version: 0.4.1 Summary: A package for
 retrosynthetic planning. Author: Austin Tripp, Krzysztof Maziarz, Guoqing Liu,
 Megan Stanley, Marwin Segler License: MIT License Copyright (c) Microsoft
 Corporation. Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
```

### Comparing `syntheseus-0.4.0/syntheseus.egg-info/SOURCES.txt` & `syntheseus-0.4.1/syntheseus.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .coveragerc
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
 CODE_OF_CONDUCT.md
+DEVELOPMENT.md
 LICENSE
 README.md
 SECURITY.md
 SUPPORT.md
 environment.yml
 environment_full.yml
 mkdocs.yml
```

### Comparing `syntheseus-0.4.0/syntheseus.egg-info/requires.txt` & `syntheseus-0.4.1/syntheseus.egg-info/requires.txt`

 * *Files identical despite different names*

