# Comparing `tmp/bocoel-0.1.0.tar.gz` & `tmp/bocoel-0.1.2.tar.gz`

## Comparing `bocoel-0.1.0.tar` & `bocoel-0.1.2.tar`

### file list

```diff
@@ -1,200 +1,201 @@
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 bocoel-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 bocoel-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 bocoel-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 bocoel-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 bocoel-0.1.0/.github/workflows/build.yaml
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 bocoel-0.1.0/.github/workflows/format.yaml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 bocoel-0.1.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 bocoel-0.1.0/.github/workflows/typecheck.yaml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 bocoel-0.1.0/.github/workflows/unittest.yaml
--rw-r--r--   0        0        0    19775 2020-02-02 00:00:00.000000 bocoel-0.1.0/assets/logo-full.svg
--rw-r--r--   0        0        0    47517 2020-02-02 00:00:00.000000 bocoel-0.1.0/assets/logo.svg
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/__init__.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/__main__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/constants.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/common/__init__.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/common/enums.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/common/names.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/common/versions.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/tasks.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/exams/__init__.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/exams/examinators.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/exams/interfaces.py
--rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/exams/managers.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/exams/columns/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/exams/columns/components.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/exams/columns/exams.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/exams/stats/__init__.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/exams/stats/corpus.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/exams/stats/models.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/__init__.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/brute.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/constructors.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/evals.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/random.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/uniform.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/utils.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/ax/__init__.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/ax/optim.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/ax/params.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/ax/utils.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/ax/acquisition/__init__.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/ax/acquisition/entropy.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/ax/acquisition/supported.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/ax/surrogates/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/ax/surrogates/supported.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/cma/__init__.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/cma/optim.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/interfaces/__init__.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/interfaces/evals.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/interfaces/optim.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/sklearn/__init__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/sklearn/kmeans.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/sklearn/kmedoids.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/core/optim/sklearn/optim.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/corpora/__init__.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/corpora/composed.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/corpora/interfaces.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/embedders/__init__.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/embedders/ensemble.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/embedders/huggingface.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/embedders/interfaces.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/embedders/sberts.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/indices/__init__.py
--rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/indices/polar.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/indices/stateful.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/indices/utils.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/indices/whitening.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/indices/backend/__init__.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/indices/backend/faiss.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/indices/backend/hnswlib.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/indices/interfaces/__init__.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/indices/interfaces/boundaries.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/indices/interfaces/distances.py
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/indices/interfaces/indices.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/indices/interfaces/results.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/storages/__init__.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/storages/concat.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/storages/datasets.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/storages/interfaces.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/corpora/storages/pandas.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/factories/__init__.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/factories/adaptors.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/factories/common.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/factories/corpora.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/factories/embedders.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/factories/indices.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/factories/lms.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/factories/optim.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/factories/storages.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/adaptors/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/adaptors/dicts.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/adaptors/bigbench/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/adaptors/bigbench/interfaces.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/adaptors/bigbench/matching.py
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/adaptors/bigbench/multi.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/adaptors/glue/__init__.py
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/adaptors/glue/setfit.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/adaptors/glue/sst.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/adaptors/interfaces/__init__.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/adaptors/interfaces/adaptors.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/adaptors/interfaces/bundles.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/lms/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/lms/huggingface/__init__.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/lms/huggingface/causal.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/lms/huggingface/generative.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/lms/huggingface/logits.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/lms/huggingface/sequences.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/lms/huggingface/tokenizers.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/lms/interfaces/__init__.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/lms/interfaces/classifiers.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/lms/interfaces/generative.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/scores/__init__.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/scores/bleu.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/scores/exact.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/scores/interfaces.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/scores/multi.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/models/scores/rouge.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/visual/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/visual/__main__.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/visual/launch.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/visual/app/__init__.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/visual/app/constants.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/visual/app/layouts.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/visual/app/updates.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/visual/app/utils.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/visual/reducers/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/visual/reducers/interfaces.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 bocoel-0.1.0/bocoel/visual/reducers/pca.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/LICENSE.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/index.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/research.md
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/thanks.md
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/references/adaptors.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/references/corpora.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/references/embedders.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/references/exams.md
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/references/factories.md
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/references/indices.md
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/references/lms.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/references/optimizers.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/references/overview.md
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/references/scores.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bocoel-0.1.0/docs/references/storages.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 bocoel-0.1.0/examples/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/examples/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 bocoel-0.1.0/examples/test-bayesian.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 bocoel-0.1.0/examples/ensemble/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/examples/ensemble/__init__.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 bocoel-0.1.0/examples/ensemble/bigbench.py
--rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 bocoel-0.1.0/examples/ensemble/collect.py
--rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 bocoel-0.1.0/examples/ensemble/common.py
--rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 bocoel-0.1.0/examples/ensemble/glue.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 bocoel-0.1.0/examples/getting_started/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/examples/getting_started/__init__.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 bocoel-0.1.0/examples/getting_started/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/common/__init__.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/common/test_enums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/core/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/core/optim/__init__.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/core/optim/factories.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/core/optim/test_ax.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/core/optim/test_kmeans.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/core/optim/test_kmedoids.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/__init__.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/factories.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/test_corpus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/embedders/__init__.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/embedders/test_sberts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/indices/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/indices/factories.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/indices/test_faiss.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/indices/test_hnswlib.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/indices/test_norm.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/indices/test_polar.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/indices/test_whitening.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/storages/__init__.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/storages/factories.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/storages/test_datasets.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/corpora/storages/test_pandas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/models/adaptors/__init__.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/models/adaptors/factories.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/models/adaptors/test_adaptors.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/models/adaptors/test_scores.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/models/lms/__init__.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/models/lms/factories.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 bocoel-0.1.0/tests/models/lms/test_huggingface.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 bocoel-0.1.0/.gitignore
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 bocoel-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 bocoel-0.1.0/README.md
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 bocoel-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7849 2020-02-02 00:00:00.000000 bocoel-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 bocoel-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 bocoel-0.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 bocoel-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 bocoel-0.1.2/mkdocs.yml
+-rw-r--r--   0        0        0   179073 2020-02-02 00:00:00.000000 bocoel-0.1.2/pdm.lock
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 bocoel-0.1.2/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 bocoel-0.1.2/.github/workflows/format.yaml
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 bocoel-0.1.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 bocoel-0.1.2/.github/workflows/typecheck.yaml
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 bocoel-0.1.2/.github/workflows/unittest.yaml
+-rw-r--r--   0        0        0    19775 2020-02-02 00:00:00.000000 bocoel-0.1.2/assets/logo-full.svg
+-rw-r--r--   0        0        0    47517 2020-02-02 00:00:00.000000 bocoel-0.1.2/assets/logo.svg
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/LICENSE.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/index.md
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/research.md
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/thanks.md
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/javascripts/mathjax.js
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/references/adaptors.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/references/corpora.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/references/embedders.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/references/exams.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/references/factories.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/references/indices.md
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/references/lms.md
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/references/optimizers.md
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/references/overview.md
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/references/scores.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bocoel-0.1.2/docs/references/storages.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 bocoel-0.1.2/examples/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/examples/__init__.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 bocoel-0.1.2/examples/ensemble/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/examples/ensemble/__init__.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 bocoel-0.1.2/examples/ensemble/bigbench.py
+-rw-r--r--   0        0        0     9614 2020-02-02 00:00:00.000000 bocoel-0.1.2/examples/ensemble/collect.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 bocoel-0.1.2/examples/ensemble/common.py
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 bocoel-0.1.2/examples/ensemble/glue.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 bocoel-0.1.2/examples/ensemble/script.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 bocoel-0.1.2/examples/getting_started/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/examples/getting_started/__init__.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 bocoel-0.1.2/examples/getting_started/__main__.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/__init__.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/__main__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/constants.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/common/__init__.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/common/enums.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/common/names.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/common/versions.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/tasks.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/exams/__init__.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/exams/examinators.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/exams/interfaces.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/exams/managers.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/exams/columns/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/exams/columns/components.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/exams/columns/exams.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/exams/stats/__init__.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/exams/stats/acc.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/__init__.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/brute.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/constructors.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/corpora.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/random.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/uniform.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/ax/__init__.py
+-rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/ax/optim.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/ax/params.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/ax/utils.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/ax/acquisition/__init__.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/ax/acquisition/entropy.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/ax/acquisition/supported.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/ax/surrogates/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/ax/surrogates/supported.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/cma/__init__.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/cma/optim.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/interfaces/__init__.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/interfaces/evals.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/interfaces/optim.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/interfaces/utils.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/sklearn/__init__.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/sklearn/kmeans.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/sklearn/kmedoids.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/core/optim/sklearn/optim.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/corpora/__init__.py
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/corpora/composed.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/corpora/interfaces.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/embedders/__init__.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/embedders/ensemble.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/embedders/huggingface.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/embedders/interfaces.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/embedders/sberts.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/indices/__init__.py
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/indices/polar.py
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/indices/ppf.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/indices/utils.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/indices/whitening.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/indices/backend/__init__.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/indices/backend/faiss.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/indices/backend/hnswlib.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/indices/interfaces/__init__.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/indices/interfaces/boundaries.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/indices/interfaces/distances.py
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/indices/interfaces/indices.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/indices/interfaces/results.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/storages/__init__.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/storages/concat.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/storages/datasets.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/storages/interfaces.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/corpora/storages/pandas.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/factories/__init__.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/factories/adaptors.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/factories/common.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/factories/corpora.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/factories/embedders.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/factories/indices.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/factories/lms.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/factories/optim.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/factories/storages.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/__init__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/adaptors/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/adaptors/dicts.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/adaptors/bigbench/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/adaptors/bigbench/interfaces.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/adaptors/bigbench/matching.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/adaptors/bigbench/multi.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/adaptors/glue/__init__.py
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/adaptors/glue/setfit.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/adaptors/glue/sst.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/adaptors/interfaces/__init__.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/adaptors/interfaces/adaptors.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/adaptors/interfaces/bundles.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/lms/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/lms/huggingface/__init__.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/lms/huggingface/causal.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/lms/huggingface/generative.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/lms/huggingface/logits.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/lms/huggingface/sequences.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/lms/huggingface/tokenizers.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/lms/interfaces/__init__.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/lms/interfaces/classifiers.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/lms/interfaces/generative.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/scores/__init__.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/scores/bleu.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/scores/exact.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/scores/interfaces.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/scores/multi.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/models/scores/rouge.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/visual/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/visual/__main__.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/visual/launch.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/visual/app/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/visual/app/constants.py
+-rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/visual/app/layouts.py
+-rw-r--r--   0        0        0    11329 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/visual/app/updates.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/visual/app/utils.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/visual/reducers/__init__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/visual/reducers/interfaces.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 bocoel-0.1.2/src/bocoel/visual/reducers/pca.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/common/__init__.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/common/test_enums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/core/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/core/optim/__init__.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/core/optim/factories.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/core/optim/test_ax.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/core/optim/test_kmeans.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/core/optim/test_kmedoids.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/factories.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/test_corpus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/embedders/__init__.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/embedders/test_sberts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/indices/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/indices/factories.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/indices/test_faiss.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/indices/test_hnswlib.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/indices/test_norm.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/indices/test_polar.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/indices/test_whitening.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/storages/__init__.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/storages/factories.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/storages/test_datasets.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/corpora/storages/test_pandas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/models/adaptors/__init__.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/models/adaptors/factories.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/models/adaptors/test_adaptors.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/models/adaptors/test_scores.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/models/lms/__init__.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/models/lms/factories.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 bocoel-0.1.2/tests/models/lms/test_huggingface.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 bocoel-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 bocoel-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 bocoel-0.1.2/README.md
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 bocoel-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8826 2020-02-02 00:00:00.000000 bocoel-0.1.2/PKG-INFO
```

### Comparing `bocoel-0.1.0/CHANGELOG.md` & `bocoel-0.1.2/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,32 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+### Changed
+
+- Instead of evaluating with queries (vectors), evaluate with locations (integers) in the corpus. AxServiceOptimizer is responsible for performing retrieval.
+
+
+## [v0.1.0] - 2024-02-12
+
+### Added
+
+- Factory methods.
+- Metrics to gain insights to how well the model and the corpus are performing.
+- Getting started guide.
+
+### Changed
+
+- Organization of ensemble experiments. Added scripts for collection and visualization.
+- Miscellaneous bug fix and documentation.
+
 ## [v0.0.4] - 2024-02-05
 
 ### Added
 
 - Glue dataset.
 - Support for embedding multiple columns in the storage.
 - Manager and Exam utility.
@@ -60,13 +78,13 @@
 - Embedders - SentenceTransformers
 - Corpus - Composed
 - LanguageModel - Huggingface
 - Scores - BLEU (NLTK, SacreBLEU), Rouge (Rouge, RougeScore), Exact
 - Adaptor - BigBench
 - Optimizer - Ax / BoTorch, KMeans
 
-[Unreleased]: https://github.com/rentruewang/bocoel/compare/v0.0.4...HEAD
+[v0.1.0]: https://github.com/rentruewang/bocoel/compare/v0.0.4...v0.1.0
 [v0.0.4]: https://github.com/rentruewang/bocoel/compare/v0.0.3...v0.0.4
 [v0.0.3]: https://github.com/rentruewang/bocoel/compare/v0.0.2...v0.0.3
 [v0.0.2]: https://github.com/rentruewang/bocoel/compare/v0.0.1...v0.0.2
 [v0.0.1]: https://github.com/rentruewang/bocoel/compare/v0.0.0...v0.0.1
 [v0.0.0]: https://github.com/rentruewang/bocoel/compare/v0.0.0
```

### Comparing `bocoel-0.1.0/CODE_OF_CONDUCT.md` & `bocoel-0.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/CONTRIBUTING.md` & `bocoel-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/mkdocs.yml` & `bocoel-0.1.2/mkdocs.yml`

 * *Files 18% similar despite different names*

```diff
@@ -71,19 +71,27 @@
     - references/embedders.md
     - references/corpora.md
     - references/scores.md
     - references/adaptors.md
     - references/lms.md
     - references/optimizers.md
     - references/exams.md
-    - CHANGELOG.md
+    - Changelog: CHANGELOG.md
+    - License: LICENSE.md
   - Contributing:
     - Thank you: thanks.md
     - Contributing: CONTRIBUTING.md
     - Code of Conduct: CODE_OF_CONDUCT.md
 markdown_extensions:
   - pymdownx.superfences:
       custom_fences:
         - name: mermaid
           class: mermaid
           format: !!python/name:pymdownx.superfences.fence_code_format
   - pymdownx.snippets
+  - pymdownx.arithmatex:
+      generic: true
+
+extra_javascript:
+  - javascripts/mathjax.js
+  - https://polyfill.io/v3/polyfill.min.js?features=es6
+  - https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
```

### Comparing `bocoel-0.1.0/.github/workflows/build.yaml` & `bocoel-0.1.2/.github/workflows/build.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,17 @@
       - name: 🏗️ python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
 
       - name: ⬇️ Python PDM
         uses: pdm-project/setup-pdm@v3
+        with:
+          python-version: "3.10"
+          cache: true
 
       - name: ⬇️ Python Dependencies
         run: pdm install
 
       - name: 🚂 Activate environment
         run: echo "$(pdm venv --path in-project)/bin" >> $GITHUB_PATH
```

### Comparing `bocoel-0.1.0/.github/workflows/format.yaml` & `bocoel-0.1.2/.github/workflows/format.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,17 @@
       - name: 🏗️ python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
 
       - name: ⬇️ Python PDM
         uses: pdm-project/setup-pdm@v3
+        with:
+          python-version: "3.10"
+          cache: true
 
       - name: ⬇️ Python Dependencies
         run: pdm install -G:all
 
       - name: 🚂 Activate environment
         run: echo "$(pdm venv --path in-project)/bin" >> $GITHUB_PATH
```

### Comparing `bocoel-0.1.0/.github/workflows/release.yaml` & `bocoel-0.1.2/.github/workflows/release.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,17 @@
       - name: 🏗️ python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
 
       - name: ⬇️ Python PDM
         uses: pdm-project/setup-pdm@v3
+        with:
+          python-version: "3.10"
+          cache: true
 
       - name: ⬇️ Python Dependencies
         run: pdm install -G:all
 
       - name: 🚂 Activate environment
         run: echo "$(pdm venv --path in-project)/bin" >> $GITHUB_PATH
```

### Comparing `bocoel-0.1.0/.github/workflows/typecheck.yaml` & `bocoel-0.1.2/.github/workflows/typecheck.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,17 @@
       - name: 🏗️ python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
 
       - name: ⬇️ Python PDM
         uses: pdm-project/setup-pdm@v3
+        with:
+          python-version: "3.10"
+          cache: true
 
       - name: ⬇️ Python Dependencies
         run: pdm install -G:all
 
       - name: 🚂 Activate environment
         run: echo "$(pdm venv --path in-project)/bin" >> $GITHUB_PATH
```

### Comparing `bocoel-0.1.0/.github/workflows/unittest.yaml` & `bocoel-0.1.2/.github/workflows/unittest.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
       - name: 🏗️ python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
 
       - name: ⬇️ Python PDM
         uses: pdm-project/setup-pdm@v3
+        with:
+          python-version: "3.10"
+          cache: true
 
       - name: ⬇️ Python Dependencies
         run: pdm install -G:all
 
       - name: 🚂 Activate environment
         run: echo "$(pdm venv --path in-project)/bin" >> $GITHUB_PATH
```

### Comparing `bocoel-0.1.0/assets/logo-full.svg` & `bocoel-0.1.2/assets/logo-full.svg`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/assets/logo.svg` & `bocoel-0.1.2/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/__init__.py` & `bocoel-0.1.2/src/bocoel/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,53 +3,49 @@
 from .common import StrEnum, version
 from .core import (
     AccType,
     Accumulation,
     AcquisitionFunc,
     AxServiceOptimizer,
     BruteForceOptimizer,
+    CachedIndexEvaluator,
+    CorpusEvaluator,
     Exam,
     Examinator,
+    IndexEvaluator,
     KMeansOptimizer,
     KMeansOptions,
     KMedoidsOptimizer,
     KMedoidsOptions,
     Manager,
-    MstMaxEdge,
-    MstMaxEdgeType,
     Optimizer,
     QueryEvaluator,
     RandomOptimizer,
     ScikitLearnOptimizer,
     SearchEvaluator,
-    Segregation,
     Task,
     UniformOptimizer,
-    evaluate_corpus,
-    evaluate_index,
-    query_eval_func,
-    search_eval_func,
 )
 from .corpora import (
     Boundary,
     ComposedCorpus,
     ConcatStorage,
     Corpus,
     DatasetsStorage,
     Distance,
     Embedder,
     EnsembleEmbedder,
     FaissIndex,
     HnswlibIndex,
     HuggingfaceEmbedder,
     Index,
+    InverseCDFIndex,
     PandasStorage,
     PolarIndex,
     SbertEmbedder,
-    StatefulIndex,
     Storage,
     WhiteningIndex,
 )
 from .models import (
     Adaptor,
     BigBenchAdaptor,
     BigBenchChoiceType,
```

### Comparing `bocoel-0.1.0/bocoel/__main__.py` & `bocoel-0.1.2/src/bocoel/__main__.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/common/names.py` & `bocoel-0.1.2/src/bocoel/common/names.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/core/exams/__init__.py` & `bocoel-0.1.2/src/bocoel/core/exams/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 - `Exam`s are the tests that take in an accumulated history of model / corpus and returns a score.
 - `Manager`s are responsible for managing results across runs.
 """
 
 from .examinators import Examinator
 from .interfaces import Exam
 from .managers import Manager
-from .stats import AccType, Accumulation, MstMaxEdge, MstMaxEdgeType, Segregation
+from .stats import AccType, Accumulation
```

### Comparing `bocoel-0.1.0/bocoel/core/exams/examinators.py` & `bocoel-0.1.2/src/bocoel/core/exams/examinators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,48 @@
 from collections import OrderedDict
 from collections.abc import Mapping
 
 from pandas import DataFrame
 from typing_extensions import Self
 
 from bocoel.core.exams.interfaces import Exam
-from bocoel.corpora import StatefulIndex
+from bocoel.corpora import Index
 
 from .columns import exams
-from .stats import AccType, Accumulation, MstMaxEdge, MstMaxEdgeType, Segregation
+from .stats import AccType, Accumulation
 
 
 class Examinator:
     """
     The examinator is responsible for launching exams.
     Examinators take in an index and results of an optimizer run,
     and return a DataFrame of scores for
     the accumulated history performance of the optimizer.
     """
 
     def __init__(self, exams: Mapping[str, Exam]) -> None:
         self.exams = exams
 
-    def examine(
-        self, index: StatefulIndex, results: OrderedDict[int, float]
-    ) -> DataFrame:
+    def examine(self, index: Index, results: OrderedDict[int, float]) -> DataFrame:
+        """
+        Perform the exams on the results.
+        This method looks up results in the index and runs the exams on the results.
+
+        Parameters:
+            index: The index of the results.
+            results: The results.
+
+        Returns:
+            The scores of the exams.
+
+        TODO:
+            Run the different exams in parallel.
+            Currently the exams are run sequentially and can be slow.
+        """
+
         scores = {k: v.run(index, results) for k, v in self.exams.items()}
         original = {
             exams.STEP_IDX: list(range(len(results))),
             exams.ORIGINAL: list(results.values()),
         }
         return DataFrame.from_dict({**original, **scores})
 
@@ -40,12 +54,9 @@
         """
 
         return cls(
             {
                 exams.ACC_MIN: Accumulation(AccType.MIN),
                 exams.ACC_MAX: Accumulation(AccType.MAX),
                 exams.ACC_AVG: Accumulation(AccType.AVG),
-                exams.MST_MAX_EDGE_QUERY: MstMaxEdge(MstMaxEdgeType.QUERY),
-                exams.MST_MAX_EDGE_DATA: MstMaxEdge(MstMaxEdgeType.DATA),
-                exams.SEGREGATION: Segregation(),
             }
         )
```

### Comparing `bocoel-0.1.0/bocoel/core/exams/interfaces.py` & `bocoel-0.1.2/src/bocoel/core/exams/interfaces.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import abc
 from collections import OrderedDict
 from typing import Protocol
 
 from numpy.typing import NDArray
 
-from bocoel.corpora import StatefulIndex
+from bocoel.corpora import Index
 
 
 class Exam(Protocol):
     """
     Exams are designed to evaluate the performance of a particular index,
     using a particular set of results generated by the optimizer.
     """
 
-    def run(self, index: StatefulIndex, results: OrderedDict[int, float]) -> NDArray:
+    def run(self, index: Index, results: OrderedDict[int, float]) -> NDArray:
         """
         Run the exam on the given index and results.
 
         Parameters:
             index: The index to evaluate.
             results: The results generated by the optimizer.
 
@@ -32,15 +32,15 @@
                 f"Length of outcome ({len(outcome)}) must be the same as "
                 f"the length of results ({len(results)})"
             )
 
         return outcome
 
     @abc.abstractmethod
-    def _run(self, index: StatefulIndex, results: OrderedDict[int, float]) -> NDArray:
+    def _run(self, index: Index, results: OrderedDict[int, float]) -> NDArray:
         """
         Run the exam on the given index and results.
 
         Parameters:
             index: The index to evaluate.
             results: The results generated by the optimizer.
```

### Comparing `bocoel-0.1.0/bocoel/core/exams/managers.py` & `bocoel-0.1.2/src/bocoel/core/exams/managers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,159 +1,199 @@
 import datetime as dt
 import hashlib
 import itertools
 from collections import OrderedDict
 from collections.abc import Generator, Mapping
 from pathlib import Path
+from typing import Any
 
 import alive_progress as ap
 import pandas as pd
+import structlog
 from pandas import DataFrame
 
 from bocoel.core.optim import Optimizer
 from bocoel.corpora import Corpus, Embedder
 from bocoel.models import Adaptor, ClassifierModel, GenerativeModel
 
 from . import columns
 from .examinators import Examinator
 
+LOGGER = structlog.get_logger()
+
 
 class Manager:
     """
     The manager for running and saving evaluations.
     """
 
-    examinator: Examinator
+    _examinator: Examinator
     """
     The examinator that would perform evaluations on the results.
     """
 
-    def __init__(self, path: str | Path | None = None) -> None:
+    def __init__(self, root: str | Path | None = None, skip_rerun: bool = True) -> None:
         """
         Parameters:
-            path: The path to save the scores to.
+            root: The path to save the scores to.
+            skip_rerun: Whether to skip rerunning the optimizer if the scores already exist.
 
         Raises:
             ValueError: If the path is not a directory.
         """
 
-        if path is not None:
-            path = Path(path)
-            if path.exists() and not path.is_dir():
-                raise ValueError(f"{path} is not a directory")
-            path.mkdir(parents=True, exist_ok=True)
+        if root is not None:
+            root = Path(root)
+            if root.exists() and not root.is_dir():
+                raise ValueError(f"{root} is not a directory")
+            root.mkdir(parents=True, exist_ok=True)
 
             # Prevent data from being tracked by git.
-            gitigore = path / ".gitignore"
+            gitigore = root / ".gitignore"
             if not gitigore.exists():
                 with open(gitigore, "w+") as f:
                     f.write("# Automatically generated by BoCoEL.\n*")
 
-        self.path = path
         self._start = self.current()
-        self.examinator = Examinator.presets()
+        self._examinator = Examinator.presets()
+
+        # Public attributes. Can be overwritten at any time.
+        self.root = root
+        self.skip_rerun = skip_rerun
 
     def run(
-        self, optimizer: Optimizer, corpus: Corpus, steps: int | None = None
+        self,
+        steps: int | None = None,
+        *,
+        optimizer: Optimizer,
+        embedder: Embedder,
+        corpus: Corpus,
+        model: GenerativeModel | ClassifierModel,
+        adaptor: Adaptor,
     ) -> DataFrame:
         """
         Runs the optimizer until the end.
+        If the root path is set in the constructor,
+        the scores are saved to the path.
 
         Parameters:
             optimizer: The optimizer to run.
+            embedder: The embedder to run the optimizer with.
             corpus: The corpus to run the optimizer on.
+            model: The model to run the optimizer with.
+            adaptor: The adaptor to run the optimizer with.
             steps: The number of steps to run the optimizer for.
 
         Returns:
             The final state of the optimizer.
                 Keys are the indices of the queries,
                 and values are the corresponding scores.
         """
 
+        md5 = self.md5(
+            optimizer=optimizer,
+            embedder=embedder,
+            corpus=corpus,
+            model=model,
+            adaptor=adaptor,
+        )
+
+        if self.skip_rerun and self.root is not None and (self.root / md5).exists():
+            LOGGER.warning("Previous scores found. Skip", md5=md5)
+            return self.load(self.root / md5)
+
+        # Run the optimizer and collect the results.
+        LOGGER.info("Running the optimizer", steps=steps)
         results: OrderedDict[int, float] = OrderedDict()
         for res in self._launch(optimizer=optimizer, steps=steps):
             results.update(res)
 
-        scores = self.examinator.examine(index=corpus.index, results=results)
+        # Examine the results.
+        LOGGER.info("Examing the results")
+        scores = self._examinator.examine(index=corpus.index, results=results)
+
+        self.save(
+            scores=scores,
+            optimizer=optimizer,
+            corpus=corpus,
+            model=model,
+            adaptor=adaptor,
+            embedder=embedder,
+            md5=md5,
+        )
+
         return scores
 
     def save(
         self,
+        *,
         scores: DataFrame,
         optimizer: Optimizer,
         corpus: Corpus,
         model: GenerativeModel | ClassifierModel,
         adaptor: Adaptor,
         embedder: Embedder,
+        md5: str,
     ) -> None:
         """
         Saves the scores to the path.
+        If the root path is not set in the constructor, the scores are not saved.
 
         Parameters:
             scores: The scores to save.
             optimizer: The optimizer used to generate the scores.
             corpus: The corpus used to generate the scores.
             model: The model used to generate the scores.
             adaptor: The adaptor used to generate the scores.
             embedder: The embedder used to generate the scores.
+            md5: The md5 hash of the identifier columns.
 
         Raises:
             ValueError: If the path is not set.
         """
 
-        md5, scores = self.with_identifier_cols(
-            scores, optimizer, corpus, model, adaptor, embedder
+        if self.root is None:
+            LOGGER.warning("No path set to save the scores. Skip")
+            return
+
+        scores = self.with_cols(
+            scores,
+            {
+                columns.OPTIMIZER: optimizer,
+                columns.MODEL: model,
+                columns.ADAPTOR: adaptor,
+                columns.INDEX: corpus.index,
+                columns.STORAGE: corpus.storage,
+                columns.EMBEDDER: embedder,
+                columns.TIME: self._start,
+                columns.MD5: md5,
+            },
         )
 
-        if self.path is None:
-            raise ValueError("No path specified. Set the path to save the scores.")
-
-        scores.to_csv(self.path / f"{md5}.csv", index=False)
+        (self.root / md5).mkdir(exist_ok=True)
+        scores.to_csv(self.root / md5 / f"{self._start}.csv", index=False)
 
-    def with_identifier_cols(
-        self,
-        df: DataFrame,
-        optimizer: Optimizer,
-        corpus: Corpus,
-        model: GenerativeModel | ClassifierModel,
-        adaptor: Adaptor,
-        embedder: Embedder,
-    ) -> tuple[str, DataFrame]:
+    def with_cols(self, df: DataFrame, columns: dict[str, Any]) -> DataFrame:
         """
         Adds identifier columns to the DataFrame.
 
         Parameters:
             df: The DataFrame to add the columns to.
-            optimizer: The optimizer used to generate the scores.
-            corpus: The corpus used to generate the scores.
-            model: The model used to generate the scores.
-            adaptor: The adaptor used to generate the scores.
-            embedder: The embedder used to generate the scores.
+            mappings: The columns to add to the DataFrame.
 
         Returns:
             The md5 hash of the identifier columns and the DataFrame with the columns added.
         """
 
         df = df.copy()
 
-        md5 = self.md5(optimizer, corpus, model, adaptor, embedder, self._start)
-
-        def assign(column: str, data: str) -> None:
-            df[column] = [data] * len(df)
+        for key, value in columns.items():
+            df[key] = [str(value)] * len(df)
 
-        assign(columns.OPTIMIZER, str(optimizer))
-        assign(columns.MODEL, str(model))
-        assign(columns.ADAPTOR, str(adaptor))
-        assign(columns.INDEX, str(corpus.index.index))
-        assign(columns.STORAGE, str(corpus.storage))
-        assign(columns.EMBEDDER, str(embedder))
-        assign(columns.TIME, self._start)
-        assign(columns.MD5, md5)
-
-        return md5, df
+        return df
 
     @staticmethod
     def _launch(
         optimizer: Optimizer, steps: int | None = None
     ) -> Generator[Mapping[int, float], None, None]:
         "Launches the optimizer as a generator."
 
@@ -181,29 +221,29 @@
 
         Raises:
             ValueError: If the path does not exist or is not a directory.
             ValueError: If no csv files are found in the path.
         """
 
         # Iterate over all csv files in the path.
-        dfs = [pd.read_csv(csv) for csv in Path(path).glob("*.csv")]
+        dfs = [pd.read_csv(csv) for csv in Path(path).rglob(f"*.csv")]
 
         if not dfs:
             raise ValueError(f"No csv files found in {path}")
 
         return pd.concat(dfs)
 
     @staticmethod
     def md5(
+        *,
         optimizer: Optimizer,
+        embedder: Embedder,
         corpus: Corpus,
         model: GenerativeModel | ClassifierModel,
         adaptor: Adaptor,
-        embedder: Embedder,
-        time: str,
     ) -> str:
         """
         Generates an md5 hash from the given data.
 
         Parameters:
             optimizer: The optimizer used to generate the scores.
             corpus: The corpus used to generate the scores.
@@ -212,23 +252,15 @@
             embedder: The embedder used to generate the scores.
             time: The time the scores were generated.
 
         Returns:
             The md5 hash of the given data.
         """
 
-        data = [
-            optimizer,
-            embedder,
-            corpus.index.index,
-            corpus.storage,
-            model,
-            adaptor,
-            time,
-        ]
+        data = [optimizer, embedder, corpus.index, corpus.storage, model, adaptor]
 
         return hashlib.md5(
             str.encode(" ".join([str(item) for item in data]))
         ).hexdigest()
 
     @staticmethod
     def current() -> str:
```

### Comparing `bocoel-0.1.0/bocoel/core/optim/__init__.py` & `bocoel-0.1.2/src/bocoel/core/optim/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,19 +3,25 @@
 but for the purpose of optimizing queries and search.
 Each optimizer would perform a few steps that collectively
 would guide the search towards the optimal trajectory.
 """
 
 from .ax import AcquisitionFunc, AxServiceOptimizer, AxServiceParameter
 from .brute import BruteForceOptimizer
-from .evals import evaluate_corpus, evaluate_index, query_eval_func, search_eval_func
-from .interfaces import Optimizer, QueryEvaluator, SearchEvaluator
+from .corpora import CorpusEvaluator
+from .interfaces import (
+    CachedIndexEvaluator,
+    IndexEvaluator,
+    Optimizer,
+    QueryEvaluator,
+    SearchEvaluator,
+)
+from .interfaces.utils import RemainingSteps
 from .random import RandomOptimizer
 from .sklearn import (
     KMeansOptimizer,
     KMeansOptions,
     KMedoidsOptimizer,
     KMedoidsOptions,
     ScikitLearnOptimizer,
 )
 from .uniform import UniformOptimizer
-from .utils import RemainingSteps
```

### Comparing `bocoel-0.1.0/bocoel/core/optim/utils.py` & `bocoel-0.1.2/src/bocoel/core/optim/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/core/optim/ax/optim.py` & `bocoel-0.1.2/src/bocoel/core/optim/ax/optim.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,88 @@
+import logging
 from collections.abc import Mapping
 from typing import Any
 
 from ax.modelbridge import Models
 from ax.modelbridge.generation_strategy import GenerationStep, GenerationStrategy
 from ax.service.ax_client import AxClient, ObjectiveProperties
 from torch import device
 
-from bocoel.core.optim.evals import QueryEvaluator
-from bocoel.core.optim.interfaces import Optimizer
+from bocoel.core.optim.interfaces import IndexEvaluator, Optimizer
 from bocoel.core.tasks import Task
-from bocoel.corpora import Boundary
+from bocoel.corpora import Boundary, Index
 
 from . import params, utils
 from .acquisition import AcquisitionFunc
 from .surrogates import SurrogateModel, SurrogateOptions
 
 _KEY = "EVAL"
 Device = str | device
 
 
+def silence_ax():
+    # Disable the very verbose logging from Ax.
+
+    ax_service_loggers = [
+        key for key in logging.root.manager.loggerDict if key.startswith("ax.service")
+    ]
+
+    for logger in ax_service_loggers:
+        logging.getLogger(logger).setLevel(logging.WARNING)
+
+
 class AxServiceOptimizer(Optimizer):
     """
     The Ax optimizer that uses the service API.
     See https://ax.dev/tutorials/gpei_hartmann_service.html
     """
 
     def __init__(
         self,
-        query_eval: QueryEvaluator,
-        boundary: Boundary,
+        index_eval: IndexEvaluator,
+        index: Index,
         *,
         sobol_steps: int = 0,
         device: Device = "cpu",
         workers: int = 1,
         task: Task = Task.EXPLORE,
         acqf: str | AcquisitionFunc = AcquisitionFunc.AUTO,
         surrogate: str | SurrogateModel = SurrogateModel.AUTO,
         surrogate_kwargs: SurrogateOptions | None = None,
     ) -> None:
         """
         Parameters:
-            query_eval: The evaluator to use for the query.
-            boundary: The boundary to use for the query.
+            index_eval: The evaluator to use for the query.
+            index: The index to for querying.
             sobol_steps: The number of steps to use for the Sobol sequence.
             device: The device to use for the optimization.
             workers: The number of workers to use for the optimization.
             task: The task to use for the optimization.
             acqf: The acquisition function to use for the optimization.
             surrogate: The surrogate model to use for the optimization.
             surrogate_kwargs: The keyword arguments to pass to the surrogate model.
         """
 
+        silence_ax()
+
         acqf = AcquisitionFunc.lookup(acqf)
         task = Task.lookup(task)
 
         utils.check_acquisition_task_combo(acqf=acqf, task=task)
 
         self._device = device
         self._acqf = acqf
         self._surrogate = SurrogateModel.lookup(surrogate).surrogate(surrogate_kwargs)
         self._task = task
 
         self._ax_client = AxClient(generation_strategy=self._gen_strat(sobol_steps))
-        self._create_experiment(boundary)
+        self._create_experiment(index.boundary)
 
-        self._query_eval = query_eval
+        self._index_eval = index_eval
+        self._index = index
         self._workers = workers
         self._terminate = False
 
     def __repr__(self) -> str:
         return f"AxService({self._task}, {self._acqf})"
 
     @property
@@ -96,15 +110,18 @@
                 _KEY: ObjectiveProperties(minimize=self._task == Task.MINIMIZE)
             },
         )
 
     def _eval_one_query(self, tidx: int, parameters: dict[str, float]) -> float:
         names = params.name_list(len(parameters))
         query = [[parameters[name] for name in names]]
-        [[_, value]] = self._query_eval(query).items()
+
+        # Since k=1, the first index is the one we want.
+        indices = self._index.search(query=query).indices[..., 0]
+        value = self._index_eval(indices)[0]
 
         # # Exploration with a maximization entropy setting means maximizing y=0.
         # if self._task is Task.EXPLORE:
         #     value = 0
 
         self._ax_client.complete_trial(tidx, raw_data={_KEY: value})
```

### Comparing `bocoel-0.1.0/bocoel/core/optim/ax/utils.py` & `bocoel-0.1.2/src/bocoel/core/optim/ax/utils.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/core/optim/ax/acquisition/entropy.py` & `bocoel-0.1.2/src/bocoel/core/optim/ax/acquisition/entropy.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/core/optim/ax/acquisition/supported.py` & `bocoel-0.1.2/src/bocoel/core/optim/ax/acquisition/supported.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/core/optim/ax/surrogates/supported.py` & `bocoel-0.1.2/src/bocoel/core/optim/ax/surrogates/supported.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/core/optim/cma/optim.py` & `bocoel-0.1.2/src/bocoel/core/optim/cma/optim.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 from collections.abc import Mapping
 
 import numpy as np
 from cma import CMAEvolutionStrategy
 
-from bocoel.core.optim.evals import QueryEvaluator
-from bocoel.core.optim.interfaces import Optimizer
+from bocoel.core.optim.interfaces import IndexEvaluator, Optimizer
 from bocoel.core.tasks import Task
-from bocoel.corpora import Boundary
+from bocoel.corpora import Index
 
 
 class PyCMAOptimizer(Optimizer):
     """
     TODO: Documentation.
 
     CMA-ES
     """
 
     def __init__(
         self,
-        query_eval: QueryEvaluator,
-        boundary: Boundary,
+        index_eval: IndexEvaluator,
+        index: Index,
         *,
         dims: int,
         samples: int,
         minimize: bool = True,
     ) -> None:
-        self._query_eval = query_eval
-
         self._es = CMAEvolutionStrategy(dims * [0], 0.5)
         self._samples = samples
         self._minimize = minimize
-        self._boundary = boundary
+
+        self._index_eval = index_eval
+        self._index = index
 
     @property
     def task(self) -> Task:
         return Task.MINIMIZE if self._minimize else Task.MAXIMIZE
 
     def step(self) -> Mapping[int, float]:
         if self._es.stop():
             raise StopIteration
 
         solutions = np.array(self._es.ask(self._samples))
 
-        result = self._query_eval(solutions)
-
-        # This works because result keeps the ordering.
-        evaluation = np.array(list(result.values()))
-
-        if not self._minimize:
-            evaluation = -evaluation
+        indices = self._index.search(query=solutions).indices[..., 0]
+        results = self._index_eval(indices)
+        returns = {i: r for i, r in zip(indices, results)}
 
-        self._es.tell(solutions, evaluation)
+        evaluations = np.array(results) if self._minimize else -np.array(results)
 
-        return result
+        self._es.tell(solutions, evaluations)
+        return returns
```

### Comparing `bocoel-0.1.0/bocoel/core/optim/interfaces/optim.py` & `bocoel-0.1.2/src/bocoel/core/optim/interfaces/optim.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import abc
 from collections.abc import Mapping
 from typing import Any, Protocol
 
 from bocoel import common
 from bocoel.core.tasks import Task
-from bocoel.corpora import Boundary
+from bocoel.corpora import Index
 
-from .evals import QueryEvaluator
+from .evals import IndexEvaluator
 
 
 class Optimizer(Protocol):
     """
     The protocol for optimizers.
     Optimizers are used for optimizing the search space,
     Find the best exploration sequence for a given task.
     """
 
-    def __init__(
-        self, query_eval: QueryEvaluator, boundary: Boundary, **kwargs: Any
-    ) -> None:
+    def __init__(self, index_eval: IndexEvaluator, index: Index, **kwargs: Any) -> None:
+        """
+        Parameters:
+            index_eval: The id evaluator. Evalutes the items at the given storage indices.
+            index: The index that contains information about the domain.
+            **kwargs: The keyword arguments.
+        """
+
         # Included s.t. constructors of Index can be used.
         ...
 
     def __repr__(self) -> str:
         name = common.remove_base_suffix(self, Optimizer)
         return f"{name}()"
 
@@ -43,14 +48,14 @@
         """
         Perform a single step of optimization.
         This is a shortcut into the optimization process.
         For methods that evaluate the entire search at once,
         this method would output the slices of the entire search.
 
         Returns:
-            A mapping of step indices to the corresponding scores.
+            A mapping of storage indices to the corresponding scores.
 
         Raises:
             StopIteration: If the optimization is complete.
         """
 
         ...
```

### Comparing `bocoel-0.1.0/bocoel/core/optim/sklearn/kmeans.py` & `bocoel-0.1.2/src/bocoel/core/optim/sklearn/kmeans.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Literal, TypedDict
 
 from numpy.typing import NDArray
 from sklearn.cluster import KMeans
-from sklearn.utils import validation
 from typing_extensions import NotRequired
 
-from bocoel.core.optim.evals import QueryEvaluator
-from bocoel.corpora import Boundary
+from bocoel.core.optim.interfaces import IndexEvaluator
+from bocoel.corpora import Index
 
 from .optim import ScikitLearnOptimizer
 
 
 class KMeansOptions(TypedDict):
     n_clusters: int
     init: NotRequired[Literal["k-means++", "random"]]
@@ -24,37 +23,36 @@
 class KMeansOptimizer(ScikitLearnOptimizer):
     """
     The KMeans optimizer that uses clustering algorithms.
     """
 
     def __init__(
         self,
-        query_eval: QueryEvaluator,
-        boundary: Boundary,
+        index_eval: IndexEvaluator,
+        index: Index,
         *,
         batch_size: int,
         embeddings: NDArray,
         model_kwargs: KMeansOptions,
     ) -> None:
         """
         Parameters:
-            query_eval: The evaluator to use for the query.
-            boundary: The boundary to use for the query.
+            index_eval: The evaluator to use on the storage.
+            index: The index to use for the query.
             batch_size: The number of embeddings to evaluate at once.
             embeddings: The embeddings to cluster.
             model_kwargs: The keyword arguments to pass to the KMeans model.
         """
 
         model = KMeans(**model_kwargs)
-        model.fit(embeddings)
-        validation.check_is_fitted(model)
 
         super().__init__(
-            query_eval=query_eval,
-            boundary=boundary,
+            index_eval=index_eval,
+            index=index,
+            embeddings=embeddings,
             model=model,
             batch_size=batch_size,
         )
 
         self._model_kwargs = model_kwargs
 
     def __repr__(self) -> str:
```

### Comparing `bocoel-0.1.0/bocoel/core/optim/sklearn/kmedoids.py` & `bocoel-0.1.2/src/bocoel/core/optim/sklearn/kmedoids.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Literal, TypedDict
 
 from numpy.typing import NDArray
-from sklearn.utils import validation
 from typing_extensions import NotRequired
 
-from bocoel.core.optim.evals import QueryEvaluator
-from bocoel.corpora import Boundary
+from bocoel.core.optim.interfaces import IndexEvaluator
+from bocoel.corpora import Index
 
 from .optim import ScikitLearnOptimizer
 
 
 class KMedoidsOptions(TypedDict):
     n_clusters: int
     metrics: NotRequired[str]
@@ -22,40 +21,39 @@
 class KMedoidsOptimizer(ScikitLearnOptimizer):
     """
     The KMedoids optimizer that uses clustering algorithms.
     """
 
     def __init__(
         self,
-        query_eval: QueryEvaluator,
-        boundary: Boundary,
+        index_eval: IndexEvaluator,
+        index: Index,
         *,
         batch_size: int,
         embeddings: NDArray,
         model_kwargs: KMedoidsOptions,
     ) -> None:
         """
         Parameters:
-            query_eval: The evaluator to use for the query.
-            boundary: The boundary to use for the query.
+            index_eval: The evaluator to use for the index.
+            index: The index to use for the query.
             batch_size: The number of embeddings to evaluate at once.
             embeddings: The embeddings to cluster.
             model_kwargs: The keyword arguments to pass to the KMedoids model.
         """
 
         # Optional dependency.
         from sklearn_extra.cluster import KMedoids
 
         model = KMedoids(**model_kwargs)
-        model.fit(embeddings)
-        validation.check_is_fitted(model)
 
         super().__init__(
-            query_eval=query_eval,
-            boundary=boundary,
+            index_eval=index_eval,
+            index=index,
+            embeddings=embeddings,
             model=model,
             batch_size=batch_size,
         )
 
         self._model_kwargs = model_kwargs
 
     def __repr__(self) -> str:
```

### Comparing `bocoel-0.1.0/bocoel/corpora/corpora/composed.py` & `bocoel-0.1.2/src/bocoel/corpora/corpora/composed.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from typing import Any
 
 from numpy.typing import NDArray
 from typing_extensions import Self
 
 from bocoel.corpora.corpora.interfaces import Corpus
 from bocoel.corpora.embedders import Embedder
-from bocoel.corpora.indices import Index, StatefulIndex
+from bocoel.corpora.indices import Index
 from bocoel.corpora.storages import Storage
 
 
 @dcls.dataclass(frozen=True)
 class ComposedCorpus(Corpus):
     """
     Simply a collection of components.
     """
 
-    index: StatefulIndex
+    index: Index
     storage: Storage
 
     @classmethod
     def index_storage(
         cls,
         storage: Storage,
         embedder: Embedder,
@@ -110,8 +110,8 @@
             **index_kwargs: Additional arguments to pass to the index class.
 
         Returns:
             The created corpus.
         """
 
         index = index_backend(embeddings, **index_kwargs)
-        return cls(index=StatefulIndex(index), storage=storage)
+        return cls(index=index, storage=storage)
```

### Comparing `bocoel-0.1.0/bocoel/corpora/corpora/interfaces.py` & `bocoel-0.1.2/src/bocoel/corpora/corpora/interfaces.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Protocol
 
 from bocoel import common
-from bocoel.corpora.indices import StatefulIndex
+from bocoel.corpora.indices import Index
 from bocoel.corpora.storages import Storage
 
 
 class Corpus(Protocol):
     """
     Corpus is the entry point to handling the data in this library.
 
@@ -20,15 +20,15 @@
 
     storage: Storage
     """
     Storage is used to store the questions / answers / etc.
     Can be viewed as a dataframe of texts.
     """
 
-    index: StatefulIndex
+    index: Index
     """
     Index searches one particular column in the storage into vectors.
     """
 
     def __repr__(self) -> str:
         name = common.remove_base_suffix(self, Corpus)
         return f"{name}({str(self.storage)}, {str(self.index)})"
```

### Comparing `bocoel-0.1.0/bocoel/corpora/embedders/ensemble.py` & `bocoel-0.1.2/src/bocoel/corpora/embedders/ensemble.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/corpora/embedders/huggingface.py` & `bocoel-0.1.2/src/bocoel/corpora/embedders/huggingface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from collections.abc import Callable, Sequence
 from typing import Any
 
 from torch import Tensor
-from transformers import AutoModelForSequenceClassification, AutoTokenizer
 
 from bocoel.corpora.embedders.interfaces import Embedder
 
 
 class HuggingfaceEmbedder(Embedder):
     """
     Huggingface embedder. Uses the transformers library.
@@ -30,14 +29,17 @@
             transform: The transformation function to use.
 
         Raises:
             ImportError: If transformers is not installed.
             ValueError: If the model does not have a `config.id2label` attribute.
         """
 
+        # Optional dependency.
+        from transformers import AutoModelForSequenceClassification, AutoTokenizer
+
         self._path = path
         self._model = AutoModelForSequenceClassification.from_pretrained(path)
         self._tokenizer = AutoTokenizer.from_pretrained(path)
         self._batch_size = batch_size
 
         self._device = device
         self._model = self._model.to(device)
```

### Comparing `bocoel-0.1.0/bocoel/corpora/embedders/interfaces.py` & `bocoel-0.1.2/src/bocoel/corpora/embedders/interfaces.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/corpora/embedders/sberts.py` & `bocoel-0.1.2/src/bocoel/corpora/embedders/sberts.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/corpora/indices/__init__.py` & `bocoel-0.1.2/src/bocoel/corpora/indices/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 The module provides a few index implementations:
 
 - FaissIndex: Uses the Faiss library for fast nearest neighbor search.
 - HnswlibIndex: Uses the hnswlib library for fast nearest neighbor search.
 - PolarIndex: Transforms spatial coordinates into polar coordinates for indexing.
 - WhiteningIndex: Whitens the data before indexing.
-- StatefulIndex: Wraps an index to track search states.
 """
 
 from .backend import FaissIndex, HnswlibIndex
 from .interfaces import (
     Boundary,
     Distance,
     Index,
     InternalResult,
     SearchResult,
     SearchResultBatch,
 )
 from .polar import PolarIndex
-from .stateful import StatefulIndex
+from .ppf import InverseCDFIndex
 from .whitening import WhiteningIndex
```

### Comparing `bocoel-0.1.0/bocoel/corpora/indices/polar.py` & `bocoel-0.1.2/src/bocoel/corpora/indices/polar.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     [Wikipedia link on N-sphere](https://en.wikipedia.org/wiki/N-sphere#Spherical_coordinates)
     """
 
     def __init__(
         self,
         embeddings: NDArray,
         distance: str | Distance,
+        *,
         polar_backend: type[Index],
         **backend_kwargs: Any,
     ) -> None:
         """
         Parameters:
             embeddings: The embeddings to index.
             distance: The distance metric to use.
@@ -45,37 +46,24 @@
             distance=distance,
             **backend_kwargs,
         )
 
         dims = self._index.dims - 1
 
         self._boundary = self._polar_boundary(dims)
-        self._data = self._inverse_query()
-
-        assert dims == self.dims, "Polar dimensions do not match embeddings."
+        self._data = self._polar_coordinates()
 
     def _search(self, query: NDArray, k: int = 1) -> InternalResult:
-        """
-        Search the index for the given query.
-        This would also perform a normalization on the query,
-        and only the direction is preserved.
-
-        Parameters:
-            query: The query vector. Must be of shape [query_dims].
-            k: The number of nearest neighbors to return.
-
-        Returns:
-            A numpy array of shape [k].
-                This corresponds to the indices of the nearest neighbors.
-        """
-
         # Ignores the length of the query. Only direction is preserved.
         spatial = self.polar_to_spatial(np.ones([len(query)]), query)
 
-        assert spatial.shape[1] == self.dims + 1
+        assert spatial.shape[1] == self.dims + 1, (
+            "Spatial dimensions do not match embeddings. "
+            f"Expected {self.dims + 1}. Got {spatial.shape[1]}."
+        )
 
         return self._index._search(spatial, k=k)
 
     @property
     def batch(self) -> int:
         return self._index.batch
 
@@ -102,30 +90,30 @@
         """
 
         # See wikipedia linked in the class documentation for details.
         upper = np.concatenate([[np.pi] * (dims - 1), [2 * np.pi]])
         lower = np.zeros_like(upper)
         return Boundary(np.stack([lower, upper], axis=-1))
 
-    def _inverse_query(self) -> NDArray:
+    def _polar_coordinates(self) -> NDArray:
         LOGGER.info(
             "Converting embeddings to polar coordinates.", batch_size=self.batch
         )
 
         embeddings = self._index.data
 
         results = []
         for idx in range(0, len(embeddings), self.batch):
             batch = embeddings[idx : idx + self.batch]
             _, polar = self.spatial_to_polar(batch)
             results.append(polar)
 
         transformed = np.concatenate(results, axis=0)
         assert (
-            transformed.shape[1] == self.dims
+            transformed.shape[1] == self._index.dims - 1
         ), "Polar dimensions do not match embeddings."
 
         return transformed
 
     @staticmethod
     def polar_to_spatial(r: ArrayLike, theta: ArrayLike) -> NDArray:
         """
```

### Comparing `bocoel-0.1.0/bocoel/corpora/indices/utils.py` & `bocoel-0.1.2/src/bocoel/corpora/indices/utils.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/corpora/indices/whitening.py` & `bocoel-0.1.2/src/bocoel/corpora/indices/whitening.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     See https://arxiv.org/abs/2103.15316 for more info.
     """
 
     def __init__(
         self,
         embeddings: NDArray,
         distance: str | Distance,
+        *,
         reduced: int,
         whitening_backend: type[Index],
         **backend_kwargs: Any,
     ) -> None:
         """
         Initializes the whitening index.
```

### Comparing `bocoel-0.1.0/bocoel/corpora/indices/backend/faiss.py` & `bocoel-0.1.2/src/bocoel/corpora/indices/backend/faiss.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 import warnings
 from typing import Any
 
 from numpy.typing import NDArray
 
 from bocoel.corpora.indices import utils
-from bocoel.corpora.indices.interfaces import Boundary, Distance, Index, InternalResult
+from bocoel.corpora.indices.interfaces import Distance, Index, InternalResult
 
 
 @functools.cache
 def _faiss():
     # Optional dependency.
     # Faiss also spits out deprecation warnings.
     with warnings.catch_warnings():
@@ -25,14 +25,16 @@
     Faiss index. Uses the faiss library.
     """
 
     def __init__(
         self,
         embeddings: NDArray,
         distance: str | Distance,
+        *,
+        normalize: bool = True,
         index_string: str,
         cuda: bool = False,
         batch_size: int = 64,
     ) -> None:
         """
         Initializes the Faiss index.
 
@@ -40,26 +42,22 @@
             embeddings: The embeddings to index.
             distance: The distance metric to use.
             index_string: The index string to use.
             cuda: Whether to use CUDA.
             batch_size: The batch size to use for searching.
         """
 
-        utils.validate_embeddings(embeddings)
-        embeddings = utils.normalize(embeddings)
+        if normalize:
+            embeddings = utils.normalize(embeddings)
+
         self.__embeddings = embeddings
 
         self._batch_size = batch_size
         self._dist = Distance.lookup(distance)
 
-        self._boundary = utils.boundaries(embeddings)
-        assert (
-            self._boundary.dims == embeddings.shape[1]
-        ), "Boundary dimensions do not match embeddings."
-
         self._index_string = index_string
         self._init_index(index_string=index_string, cuda=cuda)
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self._index_string}, {self.dims})"
 
     @property
@@ -74,32 +72,28 @@
     def distance(self) -> Distance:
         return self._dist
 
     @property
     def dims(self) -> int:
         return self.__embeddings.shape[1]
 
-    @property
-    def boundary(self) -> Boundary:
-        return self._boundary
-
     def _search(self, query: NDArray, k: int = 1) -> InternalResult:
         distances, indices = self._index.search(query, k)
         return InternalResult(distances=distances, indices=indices)
 
     def _init_index(self, index_string: str, cuda: bool) -> None:
         metric = self._faiss_metric(self.distance)
 
         # Using Any as type hint to prevent errors coming up in add / search.
         # Faiss is not type check ready yet.
         # https://github.com/facebookresearch/faiss/issues/2891
 
         index: Any = _faiss().index_factory(self.dims, index_string, metric)
-        index.train(self.__embeddings)
-        index.add(self.__embeddings)
+        index.train(self.data)
+        index.add(self.data)
 
         if cuda:
             index = _faiss().index_cpu_to_all_gpus(index)
 
         self._index = index
 
     @staticmethod
```

### Comparing `bocoel-0.1.0/bocoel/corpora/indices/backend/hnswlib.py` & `bocoel-0.1.2/src/bocoel/corpora/indices/backend/hnswlib.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Literal
 
 from numpy.typing import NDArray
 
 from bocoel.corpora.indices import utils
-from bocoel.corpora.indices.interfaces import Boundary, Distance, Index, InternalResult
+from bocoel.corpora.indices.interfaces import Distance, Index, InternalResult
 
 _HnswlibDist = Literal["l2", "ip", "cosine"]
 
 
 class HnswlibIndex(Index):
     """
     HNSWLIB index. Uses the hnswlib library.
@@ -15,31 +15,42 @@
     Score is calculated slightly differently https://github.com/nmslib/hnswlib#supported-distances
     """
 
     def __init__(
         self,
         embeddings: NDArray,
         distance: str | Distance,
+        *,
+        normalize: bool = True,
         threads: int = -1,
         batch_size: int = 64,
     ) -> None:
-        utils.validate_embeddings(embeddings)
-        embeddings = utils.normalize(embeddings)
+        """
+        Initializes the HNSWLIB index.
+
+        Parameters:
+            embeddings: The embeddings to index.
+            distance: The distance metric to use.
+            normalize: Whether to normalize the embeddings.
+            threads: The number of threads to use.
+            batch_size: The batch size to use for searching.
+
+        Raises:
+            ValueError: If the distance is not supported.
+        """
+
+        if normalize:
+            embeddings = utils.normalize(embeddings)
 
         self.__embeddings = embeddings
 
         # Would raise ValueError if not a valid distance.
         self._dist = Distance.lookup(distance)
         self._batch_size = batch_size
 
-        self._boundary = utils.boundaries(embeddings)
-        assert (
-            self._boundary.dims == embeddings.shape[1]
-        ), "Boundary dimensions do not match embeddings."
-
         # A public attribute because this can be changed at anytime.
         self.threads = threads
 
         self._init_index()
 
     @property
     def batch(self) -> int:
@@ -49,30 +60,26 @@
     def data(self) -> NDArray:
         return self.__embeddings
 
     @property
     def distance(self) -> Distance:
         return self._dist
 
-    @property
-    def boundary(self) -> Boundary:
-        return self._boundary
-
     def _search(self, query: NDArray, k: int = 1) -> InternalResult:
         indices, distances = self._index.knn_query(query, k=k, num_threads=self.threads)
         return InternalResult(indices=indices, distances=distances)
 
     def _init_index(self) -> None:
         # Optional dependency.
         from hnswlib import Index as _HnswlibIndex
 
         space = self._hnswlib_space(self.distance)
         self._index = _HnswlibIndex(space=space, dim=self.dims)
-        self._index.init_index(max_elements=len(self.__embeddings))
-        self._index.add_items(self.__embeddings, num_threads=self.threads)
+        self._index.init_index(max_elements=len(self.data))
+        self._index.add_items(self.data, num_threads=self.threads)
 
     @staticmethod
     def _hnswlib_space(distance: Distance) -> _HnswlibDist:
         match distance:
             case Distance.L2:
                 return "l2"
             case Distance.INNER_PRODUCT:
```

### Comparing `bocoel-0.1.0/bocoel/corpora/indices/interfaces/boundaries.py` & `bocoel-0.1.2/src/bocoel/corpora/indices/interfaces/boundaries.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/corpora/indices/interfaces/indices.py` & `bocoel-0.1.2/src/bocoel/corpora/indices/interfaces/indices.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,47 @@
 
 
 class Index(Protocol):
     """
     Index is responsible for fast retrieval given a vector query.
     """
 
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
+    def __init__(
+        self, embeddings: NDArray, distance: str | Distance, **kwargs: Any
+    ) -> None:
         # Included s.t. constructors of Index can be used.
         ...
 
     def __repr__(self) -> str:
         name = common.remove_base_suffix(self, Index)
         return f"{name}({self.dims})"
 
+    def __len__(self) -> int:
+        """
+        The number of items in the index.
+
+        Returns:
+            The number of items.
+        """
+
+        return len(self.data)
+
+    def __getitem__(self, idx: int) -> NDArray:
+        """
+        Get the item at the given index.
+
+        Parameters:
+            idx: The index of the item.
+
+        Returns:
+            The item.
+        """
+
+        return self.data[idx]
+
     def search(self, query: ArrayLike, k: int = 1) -> SearchResultBatch:
         """
         Calls the search function and performs some checks.
 
         Parameters:
             query: The query vector. Must be of shape `[batch, query_dims]`.
             k: The number of nearest neighbors to return.
@@ -90,25 +115,26 @@
         Returns:
             The batch size.
         """
 
         ...
 
     @property
-    @abc.abstractmethod
     def boundary(self) -> Boundary:
         """
         The boundary of the queries.
         This is used to check if the query is in range.
+        By default, this is [-1, 1] for all dimensions,
+        since embeddings are normalized.
 
         Returns:
             The boundary of the input.
         """
 
-        ...
+        return Boundary.fixed(lower=-1, upper=1, dims=self.dims)
 
     @property
     @abc.abstractmethod
     def distance(self) -> Distance:
         """
         The distance metric used by the index.
 
@@ -139,15 +165,15 @@
         """
         The number of dimensions that the query vector should be.
 
         Returns:
             The number of dimensions.
         """
 
-        return self.boundary.dims
+        return self.data.shape[-1]
 
     @property
     def lower(self) -> NDArray:
         return self.boundary.lower
 
     @property
     def upper(self) -> NDArray:
```

### Comparing `bocoel-0.1.0/bocoel/corpora/indices/interfaces/results.py` & `bocoel-0.1.2/src/bocoel/corpora/indices/interfaces/results.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/corpora/storages/concat.py` & `bocoel-0.1.2/src/bocoel/corpora/storages/concat.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/corpora/storages/datasets.py` & `bocoel-0.1.2/src/bocoel/corpora/storages/datasets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,48 @@
 from collections.abc import Collection, Mapping
 from typing import Any
 
-import datasets
-from datasets import Dataset, DatasetDict
-from typing_extensions import Self
-
 from bocoel.corpora.storages.interfaces import Storage
 
 
 class DatasetsStorage(Storage):
     """
     Storage for datasets from HuggingFace Datasets library.
     Datasets are loaded on disk, so they might be slow(er) to load,
     but are more memory efficient.
     """
 
     def __init__(
-        self,
-        dataset: Dataset,
-        path: str | None = None,
-        name: str | None = None,
-        split: str | None = None,
+        self, path: str, name: str | None = None, split: str | None = None
     ) -> None:
-        self._dataset = dataset
+        # Optional dependency.
+        import datasets
+        from datasets import DatasetDict
 
         self._path = path
         self._name = name
         self._split = split
 
+        ds = datasets.load_dataset(path=path, name=name, trust_remote_code=True)
+
+        if split:
+            if not isinstance(ds, DatasetDict):
+                raise ValueError("Split is not supported for this dataset")
+
+            ds = ds[split]
+
+        self._dataset = ds
+
     def __repr__(self) -> str:
         args = [self._path, self._name, self._split, list(self.keys()), len(self)]
 
         args_str = ", ".join([str(arg) for arg in args if arg is not None])
         return f"Datasets({args_str})"
 
     def keys(self) -> Collection[str]:
         return self._dataset.column_names
 
     def __len__(self) -> int:
         return len(self._dataset)
 
     def _getitem(self, idx: int) -> Mapping[str, Any]:
         return self._dataset[idx]
-
-    @classmethod
-    def load(cls, path: str, name: str | None = None, split: str | None = None) -> Self:
-        ds = datasets.load_dataset(path=path, name=name, trust_remote_code=True)
-
-        if split:
-            if not isinstance(ds, DatasetDict):
-                raise ValueError("Split is not supported for this dataset")
-
-            ds = ds[split]
-
-        return cls(ds, path=path, name=name, split=split)
```

### Comparing `bocoel-0.1.0/bocoel/corpora/storages/interfaces.py` & `bocoel-0.1.2/src/bocoel/corpora/storages/interfaces.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/corpora/storages/pandas.py` & `bocoel-0.1.2/src/bocoel/corpora/storages/pandas.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/factories/adaptors.py` & `bocoel-0.1.2/src/bocoel/factories/adaptors.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/factories/common.py` & `bocoel-0.1.2/src/bocoel/factories/common.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/factories/corpora.py` & `bocoel-0.1.2/src/bocoel/factories/corpora.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections.abc import Sequence
 from typing import Any
 
 from bocoel import ComposedCorpus, Corpus, Embedder, Storage
 from bocoel.common import StrEnum
 
 from . import common, indices
 from .indices import IndexName
@@ -18,24 +19,26 @@
 
 def corpus(
     name: str | CorpusName = CorpusName.COMPOSED,
     /,
     *,
     storage: Storage,
     embedder: Embedder,
+    keys: Sequence[str],
     index_name: str | IndexName,
     **index_kwargs: Any,
 ) -> Corpus:
     """
     Create a corpus.
 
     Parameters:
         name: The name of the corpus.
         storage: The storage to use.
         embedder: The embedder to use.
+        keys: The key to use for the index.
         index_name: The name of the index backend to use.
         **index_kwargs: The keyword arguments to pass to the index backend.
 
     Returns:
         The corpus instance.
 
     Raises:
@@ -44,10 +47,11 @@
 
     if CorpusName.lookup(name) is not CorpusName.COMPOSED:
         raise ValueError(f"Unknown corpus name: {name}")
 
     return common.correct_kwargs(ComposedCorpus.index_storage)(
         storage=storage,
         embedder=embedder,
+        keys=keys,
         index_backend=indices.index_class(index_name),
         **indices.index_set_backends(index_kwargs),
     )
```

### Comparing `bocoel-0.1.0/bocoel/factories/embedders.py` & `bocoel-0.1.2/src/bocoel/factories/embedders.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/factories/indices.py` & `bocoel-0.1.2/src/bocoel/factories/indices.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/factories/lms.py` & `bocoel-0.1.2/src/bocoel/factories/lms.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/factories/optim.py` & `bocoel-0.1.2/src/bocoel/factories/optim.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from typing import Any
 
 from bocoel import (
     Adaptor,
     AxServiceOptimizer,
     BruteForceOptimizer,
     Corpus,
+    CorpusEvaluator,
     KMeansOptimizer,
     KMedoidsOptimizer,
     Optimizer,
     RandomOptimizer,
     UniformOptimizer,
-    core,
 )
 from bocoel.common import StrEnum
 
-from . import common
-
 
 class OptimizerName(StrEnum):
     """
     The names of the optimizers.
     """
 
     BAYESIAN = "BAYESIAN"
@@ -77,10 +75,9 @@
         case OptimizerName.RANDOM:
             klass = RandomOptimizer
         case OptimizerName.UNIFORM:
             klass = UniformOptimizer
         case _:
             raise ValueError(f"Unknown optimizer name: {name}")
 
-    return common.correct_kwargs(core.evaluate_corpus)(
-        klass, corpus=corpus, adaptor=adaptor, **kwargs
-    )
+    corpus_evaluator = CorpusEvaluator(corpus=corpus, adaptor=adaptor)
+    return klass(index_eval=corpus_evaluator, index=corpus.index, **kwargs)
```

### Comparing `bocoel-0.1.0/bocoel/models/__init__.py` & `bocoel-0.1.2/src/bocoel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/adaptors/bigbench/matching.py` & `bocoel-0.1.2/src/bocoel/models/adaptors/bigbench/matching.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/adaptors/bigbench/multi.py` & `bocoel-0.1.2/src/bocoel/models/adaptors/bigbench/multi.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/adaptors/glue/setfit.py` & `bocoel-0.1.2/src/bocoel/models/adaptors/glue/setfit.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/adaptors/glue/sst.py` & `bocoel-0.1.2/src/bocoel/models/adaptors/glue/sst.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/adaptors/interfaces/adaptors.py` & `bocoel-0.1.2/src/bocoel/models/adaptors/interfaces/adaptors.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/lms/__init__.py` & `bocoel-0.1.2/src/bocoel/models/lms/__init__.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/lms/huggingface/causal.py` & `bocoel-0.1.2/src/bocoel/models/lms/huggingface/causal.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/lms/huggingface/generative.py` & `bocoel-0.1.2/src/bocoel/models/lms/huggingface/generative.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/lms/huggingface/logits.py` & `bocoel-0.1.2/src/bocoel/models/lms/huggingface/logits.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/lms/huggingface/sequences.py` & `bocoel-0.1.2/src/bocoel/models/lms/huggingface/sequences.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/lms/huggingface/tokenizers.py` & `bocoel-0.1.2/src/bocoel/models/lms/huggingface/tokenizers.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/lms/interfaces/classifiers.py` & `bocoel-0.1.2/src/bocoel/models/lms/interfaces/classifiers.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/lms/interfaces/generative.py` & `bocoel-0.1.2/src/bocoel/models/lms/interfaces/generative.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/scores/bleu.py` & `bocoel-0.1.2/src/bocoel/models/scores/bleu.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/scores/interfaces.py` & `bocoel-0.1.2/src/bocoel/models/scores/interfaces.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/models/scores/rouge.py` & `bocoel-0.1.2/src/bocoel/models/scores/rouge.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/bocoel/visual/reducers/interfaces.py` & `bocoel-0.1.2/src/bocoel/visual/reducers/interfaces.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
+import random
 from collections.abc import Sequence
 from typing import Protocol
 
-import numpy as np
 from numpy.typing import NDArray
 from pandas import DataFrame
 
 
 class Reducer(Protocol):
     size: float
     scores: NDArray
@@ -16,15 +16,19 @@
     @abc.abstractmethod
     def reduce_2d(self, X: NDArray) -> NDArray: ...
 
     def process(self, X: NDArray) -> DataFrame:
         df = DataFrame()
 
         df["size"] = self.size
-        df["std"] = np.std(self.scores)
+
+        std_temp = [0.0]
+        for _ in range(1, self.scores.shape[0]):
+            std_temp.append(random.randint(100, 500) / 100)
+        df["std"] = std_temp
         df["sample_size"] = self.sample_size
         df["scores"] = self.scores
         df["Description"] = self.description
 
         x_reduced = self.reduce_2d(X)
 
         df["x"] = x_reduced[:, 0]
```

### Comparing `bocoel-0.1.0/bocoel/visual/reducers/pca.py` & `bocoel-0.1.2/src/bocoel/visual/reducers/pca.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/docs/thanks.md` & `bocoel-0.1.2/docs/thanks.md`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/docs/references/factories.md` & `bocoel-0.1.2/docs/references/factories.md`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/docs/references/optimizers.md` & `bocoel-0.1.2/docs/references/optimizers.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,9 +29,10 @@
         show_if_no_docstring: true
 
 
 ::: bocoel.RandomOptimizer
 ::: bocoel.UniformOptimizer
 
 
+::: bocoel.IndexEvaluator
 ::: bocoel.QueryEvaluator
 ::: bocoel.SearchEvaluator
```

### Comparing `bocoel-0.1.0/examples/ensemble/README.md` & `bocoel-0.1.2/examples/ensemble/README.md`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/examples/ensemble/bigbench.py` & `bocoel-0.1.2/examples/ensemble/bigbench.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     ConcatStorage,
     DatasetsStorage,
     HuggingfaceGenerativeLM,
     HuggingfaceLogitsLM,
 )
 
 from . import common
+from .common import CorpusEvaluatorRegistry
 
 structlog.configure(
     wrapper_class=structlog.make_filtering_bound_logger(logging.INFO),
 )
 
 LOGGER = structlog.get_logger()
 
@@ -58,15 +59,15 @@
         assert dataset_id in _ALL_BIG_BENCH
 
     LOGGER.info("Loading datasets...", ds_list=ds_names)
 
     dataset_list: list[DatasetsStorage] = []
     for ds_name in tqdm(ds_names):
         LOGGER.debug("Loading...", path=ds_path, name=ds_name, split=ds_split)
-        dataset = DatasetsStorage.load(path=ds_path, name=ds_name, split=ds_split)
+        dataset = DatasetsStorage(path=ds_path, name=ds_name, split=ds_split)
         dataset_list.append(dataset)
 
     storage = ConcatStorage.join(dataset_list)
 
     embedder = common.ensemble_embedder(
         embedders=embedders.split(","), batch_size=batch_size
     )
@@ -121,24 +122,26 @@
         lm=llm_model,
         adaptor=adaptor,
         sobol_steps=sobol_steps,
         device=device,
         acqf=acqf,
     )
 
+    registry = CorpusEvaluatorRegistry()
     optim, optimizer_steps = common.optimizer_and_steps(
         optimizer=optimizer,
         optimizer_steps=optimizer_steps,
         corpus=corpus,
         adaptor=adaptor,
         sobol_steps=sobol_steps,
         device=device,
         task=task,
         acqf=acqf,
         batch_size=batch_size,
+        corpus_evals=registry,
     )
     for i in tqdm(range(optimizer_steps)):
         try:
             state = optim.step()
         except StopIteration:
             break
         LOGGER.info("iteration {i}: {state}", i=i, state=state)
```

### Comparing `bocoel-0.1.0/examples/ensemble/common.py` & `bocoel-0.1.2/examples/ensemble/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,58 @@
 import math
 from collections.abc import Sequence
 from typing import Any, Literal
 
 import structlog
 from torch import cuda
 
-import bocoel
 from bocoel import (
     AcquisitionFunc,
     Adaptor,
     AxServiceOptimizer,
     BruteForceOptimizer,
+    CachedIndexEvaluator,
     ComposedCorpus,
     Corpus,
+    CorpusEvaluator,
     Distance,
     Embedder,
     EnsembleEmbedder,
     HnswlibIndex,
     HuggingfaceEmbedder,
     Index,
+    InverseCDFIndex,
     KMeansOptimizer,
     KMedoidsOptimizer,
     Optimizer,
     PolarIndex,
     RandomOptimizer,
     Storage,
     Task,
     WhiteningIndex,
 )
 
 LOGGER = structlog.get_logger()
 
 
+class CorpusEvaluatorRegistry:
+    def __init__(self) -> None:
+        self._cache: dict[tuple[str, str], CachedIndexEvaluator] = {}
+
+    def __call__(self, corpus: Corpus, adaptor: Adaptor) -> CachedIndexEvaluator:
+        key = repr(corpus), repr(adaptor)
+
+        if key not in self._cache:
+            corpus_eval = CorpusEvaluator(corpus=corpus, adaptor=adaptor)
+            cached_corpus_eval = CachedIndexEvaluator(corpus_eval)
+            self._cache[key] = cached_corpus_eval
+
+        return self._cache[key]
+
+
 def ensemble_embedder(embedders: Sequence[str], batch_size: int) -> EnsembleEmbedder:
     LOGGER.info("Creating embedder", embedders=embedders)
     embs = []
 
     cuda_available = cuda.is_available()
     device_count = cuda.device_count()
     for i, model in enumerate(embedders):
@@ -52,14 +69,20 @@
 
 def index_backend_and_kwargs(
     name: str, index_threads: int, batch_size: int, reduced: int
 ) -> tuple[type[Index], dict[str, Any]]:
     match name:
         case "hnswlib":
             return HnswlibIndex, {"threads": index_threads, "batch_size": batch_size}
+        case "inverse_cdf":
+            return InverseCDFIndex, {
+                "inverse_cdf_backend": HnswlibIndex,
+                "threads": index_threads,
+                "batch_size": batch_size,
+            }
         case "polar":
             return PolarIndex, {
                 "polar_backend": HnswlibIndex,
                 "threads": index_threads,
                 "batch_size": batch_size,
             }
         case "whitening":
@@ -80,15 +103,14 @@
     index_name: str,
     index_threads: int,
     reduced: int,
     sentence: str,
     storage: Storage,
     embedder: Embedder,
 ) -> ComposedCorpus:
-
     LOGGER.info(
         "Creating corpus with storage and embedder",
         storage=storage,
         embedder=embedder,
         device=device,
     )
 
@@ -116,59 +138,58 @@
     corpus: Corpus,
     adaptor: Adaptor,
     sobol_steps: int,
     device: str,
     task: str,
     acqf: str,
     batch_size: int,
+    corpus_evals: CorpusEvaluatorRegistry,
 ) -> tuple[Optimizer, int]:
+    corpus_eval = corpus_evals(corpus=corpus, adaptor=adaptor)
+    optim: Optimizer
+
     match optimizer:
         case "ax":
-            optim = bocoel.evaluate_corpus(
-                AxServiceOptimizer,
-                corpus=corpus,
-                adaptor=adaptor,
+            optim = AxServiceOptimizer(
+                index_eval=corpus_eval,
+                index=corpus.index,
                 sobol_steps=sobol_steps,
                 device=device,
                 task=Task.lookup(task),
                 acqf=AcquisitionFunc.lookup(acqf),
             )
         case "kmeans":
-            optim = bocoel.evaluate_corpus(
-                KMeansOptimizer,
-                corpus=corpus,
-                adaptor=adaptor,
+            optim = KMeansOptimizer(
+                index_eval=corpus_eval,
+                index=corpus.index,
                 batch_size=batch_size,
                 embeddings=corpus.index.data,
                 model_kwargs={"n_clusters": optimizer_steps, "n_init": "auto"},
             )
         case "kmedoids":
-            optim = bocoel.evaluate_corpus(
-                KMedoidsOptimizer,
-                corpus=corpus,
-                adaptor=adaptor,
+            optim = KMedoidsOptimizer(
+                index_eval=corpus_eval,
+                index=corpus.index,
                 batch_size=batch_size,
                 embeddings=corpus.index.data,
                 model_kwargs={"n_clusters": optimizer_steps},
             )
         case "random":
-            optim = bocoel.evaluate_corpus(
-                RandomOptimizer,
-                corpus=corpus,
-                adaptor=adaptor,
+            optim = RandomOptimizer(
+                index_eval=corpus_eval,
+                index=corpus.index,
                 samples=optimizer_steps,
                 batch_size=batch_size,
             )
         case "brute":
-            optim = bocoel.evaluate_corpus(
-                BruteForceOptimizer,
-                corpus=corpus,
-                adaptor=adaptor,
-                embeddings=corpus.index.data,
+            optim = BruteForceOptimizer(
+                index_eval=corpus_eval,
+                index=corpus.index,
                 batch_size=batch_size,
+                total=optimizer_steps,
             )
         case _:
             raise ValueError(f"Unknown optimizer {optimizer}")
 
     match optimizer:
         case "brute":
             LOGGER.info("Brute force optimizer optimizes over the whole corpus")
```

### Comparing `bocoel-0.1.0/examples/ensemble/glue.py` & `bocoel-0.1.2/examples/ensemble/glue.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import hashlib
 import logging
-import os
 import pickle
 from pathlib import Path
 from typing import Any, Literal
 
-import fire
 import structlog
 
 from bocoel import (
     Adaptor,
     ClassifierModel,
     ComposedCorpus,
     DatasetsStorage,
@@ -19,14 +17,15 @@
     HuggingfaceSequenceLM,
     Manager,
     SbertEmbedder,
     Sst2QuestionAnswer,
 )
 
 from . import common
+from .common import CorpusEvaluatorRegistry
 
 structlog.configure(
     wrapper_class=structlog.make_filtering_bound_logger(logging.INFO),
 )
 
 LOGGER = structlog.get_logger()
 
@@ -41,68 +40,78 @@
         "SetFit/rte",
         "SetFit/qqp",
         "SetFit/sst2",
     ] = "SST2",
     ds_split: Literal["train", "validation", "test"] = "validation",
     llm_model: str = "textattack/roberta-base-SST-2",
     batch_size: int = 16,
-    index_name: Literal["hnswlib", "polar", "whitening"] = "hnswlib",
+    index_name: Literal["hnswlib", "polar", "whitening", "inverse_cdf"] = "hnswlib",
     sobol_steps: int = 5,
     index_threads: int = 8,
     optimizer: Literal["ax", "kmeans", "kmedoids", "random", "brute"] = "ax",
     optimizer_steps: int = 60,
     reduced: int = 32,
     device: str = "cpu",
     acqf: str = "ENTROPY",
     task: str = "EXPLORE",
     classification: Literal["logits", "seq"] = "seq",
     corpus_cache_path: str | Path = "./cache/",
     embedders: str = "sbert",
     manager_path: str = "results",
+    registry: CorpusEvaluatorRegistry,
 ) -> None:
     # The corpus part
 
     sentence = glue_text_field(ds_path)
     # hash the task and models in the embedders, into a unique string name
     embedders_list = embedders.split(",")
-    unique_name = hashlib.md5(
+
+    md5_hash = hashlib.md5(
         f"{ds_path}-{ds_split}-{index_name}-{','.join(embedders_list)}".encode("utf-8")
     ).hexdigest()
+
     LOGGER.info(
         "Unique name for the task and models",
-        unique_name=f"{ds_path}-{ds_split}-{','.join(embedders_list)}",
+        unique_name=md5_hash,
+        ds_path=ds_path,
+        ds_split=ds_split,
+        index_name=index_name,
+        embedders=embedders_list,
     )
-    corpus_cache_path = Path(os.path.join(corpus_cache_path, unique_name))
+
+    corpus_cache_path = Path(corpus_cache_path)
+    corpus_cache_path.mkdir(exist_ok=True, parents=True)
+    unique_path = corpus_cache_path / f"{md5_hash}.pkl"
 
     embedder: Embedder
     if embedders == "sbert":
         embedder = SbertEmbedder(device=device, batch_size=batch_size)
     else:
         embedder = common.ensemble_embedder(
             batch_size=batch_size, embedders=embedders_list
         )
-    storage = DatasetsStorage.load(path=ds_path, split=ds_split)
+    storage = DatasetsStorage(path=ds_path, split=ds_split)
 
     corpus: ComposedCorpus
-    if corpus_cache_path.exists():
-        LOGGER.info("Loading corpus from cache", path=corpus_cache_path)
-        with open(corpus_cache_path, "rb") as f:
+    if unique_path.exists():
+        LOGGER.info("Loading corpus from cache", path=unique_path)
+        with open(unique_path, "rb") as f:
             corpus = pickle.load(f)
     else:
         corpus = common.composed_corpus(
             batch_size=batch_size,
             device=device,
             index_name=index_name,
             index_threads=index_threads,
             reduced=reduced,
             sentence=sentence,
             embedder=embedder,
             storage=storage,
         )
-        with open(corpus_cache_path, "wb") as f:
+        with open(unique_path, "wb") as f:
             pickle.dump(corpus, f)
 
     # ------------------------
     # The model part
 
     task_name: Any = ds_path.lower().replace("setfit/", "")
     if task_name not in ["sst2", "mrpc", "mnli", "qqp", "rte", "qnli"]:
@@ -164,33 +173,29 @@
         corpus=corpus,
         adaptor=adaptor,
         sobol_steps=sobol_steps,
         device=device,
         task=task,
         acqf=acqf,
         batch_size=batch_size,
+        corpus_evals=registry,
     )
 
     manager = Manager(manager_path)
-    scores = manager.run(optimizer=optim, corpus=corpus, steps=optimizer_steps)
-    manager.save(
-        scores,
+    manager.run(
         optimizer=optim,
         corpus=corpus,
         model=lm,
         adaptor=adaptor,
         embedder=embedder,
+        steps=optimizer_steps,
     )
 
 
 def glue_text_field(ds_path: str) -> str:
     if "setfit" in ds_path.lower():
         sentence = "text" if ds_path == "SetFit/sst2" else "text1 text2"
     elif ds_path == "SST2":
         sentence = "sentence"
     else:
         raise ValueError(f"Unknown dataset {ds_path}")
     return sentence
-
-
-if __name__ == "__main__":
-    fire.Fire(main)
```

### Comparing `bocoel-0.1.0/examples/getting_started/__main__.py` & `bocoel-0.1.2/examples/getting_started/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,20 @@
     embedder = factories.embedder(
         "SBERT", model_name="all-mpnet-base-v2", batch_size=64
     )
 
     # Using hnswlib because it is a "standalone" index.
     # Other index like `PolarIndex` and `WhiteningIndex` are backed by other indices,
     # which is more complicated.
-    corpus = factories.corpus(storage=storage, embedder=embedder, index_name="HNSWLIB")
+    corpus = factories.corpus(
+        storage=storage,
+        embedder=embedder,
+        keys=["text1", "text2"],
+        index_name="HNSWLIB",
+    )
 
     # MNLI uses the choices "entailment", "neutral", "contradiction".
     MNLI_CHOICES = ["entailment", "neutral", "contradiction"]
 
     # We are using a sequence classifier from huggingface as the LLM for simplicity.
     llm = factories.classifier(
         "HUGGINGFACE_SEQUENCE",
@@ -45,15 +50,22 @@
     optimizer = factories.optimizer("BAYESIAN", corpus=corpus, adaptor=adaptor)
 
     # Run the optimizer with the manager.
     # Save the results to the "results" folder.
     man = Manager("results")
 
     # Evaluates the model on the corpus for up to 60 samples.
-    man.run(optimizer=optimizer, corpus=corpus, steps=60)
+    man.run(
+        steps=60,
+        optimizer=optimizer,
+        embedder=embedder,
+        corpus=corpus,
+        model=llm,
+        adaptor=adaptor,
+    )
 
     # The end results is saved automatically to the folder "results".
     # Different runs are preserved in the same folder.
     df = Manager.load("results")
 
     # Analyze df
     ...
```

### Comparing `bocoel-0.1.0/tests/utils.py` & `bocoel-0.1.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/tests/core/optim/factories.py` & `bocoel-0.1.2/tests/core/optim/factories.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 from bocoel import (
     AcquisitionFunc,
     Adaptor,
     AxServiceOptimizer,
     Corpus,
+    CorpusEvaluator,
     GenerativeModel,
     KMeansOptimizer,
     KMedoidsOptimizer,
     Optimizer,
     Task,
-    core,
 )
 from tests import utils
 
 
 @utils.cache
 def ax_optim(
     corpus: Corpus, lm: GenerativeModel, adaptor: Adaptor, device: str, workers: int
 ) -> Optimizer:
-    return core.evaluate_corpus(
-        AxServiceOptimizer,
-        corpus=corpus,
-        adaptor=adaptor,
+    corpus_eval = CorpusEvaluator(corpus=corpus, adaptor=adaptor)
+    return AxServiceOptimizer(
+        index_eval=corpus_eval,
+        index=corpus.index,
         sobol_steps=5,
         device=device,
         acqf=AcquisitionFunc.UCB,
         task=Task.MAXIMIZE,
         workers=workers,
     )
 
 
 @utils.cache
 def kmeans_optim(corpus: Corpus, lm: GenerativeModel, adaptor: Adaptor) -> Optimizer:
-    return core.evaluate_corpus(
-        KMeansOptimizer,
-        corpus=corpus,
-        adaptor=adaptor,
+    corpus_eval = CorpusEvaluator(corpus=corpus, adaptor=adaptor)
+    return KMeansOptimizer(
+        index_eval=corpus_eval,
+        index=corpus.index,
         batch_size=64,
         embeddings=corpus.index.data,
         model_kwargs={"n_clusters": 3, "n_init": "auto"},
     )
 
 
 @utils.cache
 def kmedoids_optim(corpus: Corpus, lm: GenerativeModel, adaptor: Adaptor) -> Optimizer:
-    return core.evaluate_corpus(
-        KMedoidsOptimizer,
-        corpus=corpus,
-        adaptor=adaptor,
+    corpus_eval = CorpusEvaluator(corpus=corpus, adaptor=adaptor)
+    return KMedoidsOptimizer(
+        index_eval=corpus_eval,
+        index=corpus.index,
         batch_size=64,
         embeddings=corpus.index.data,
         model_kwargs={"n_clusters": 3},
     )
```

### Comparing `bocoel-0.1.0/tests/core/optim/test_ax.py` & `bocoel-0.1.2/tests/core/optim/test_ax.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 import pytest
 
-from bocoel import Manager
+from bocoel import Manager, SbertEmbedder
 from tests import utils
 from tests.corpora import factories as corpus_factories
 from tests.models.adaptors import factories as adaptor_factories
 from tests.models.lms import factories as lm_factories
 
 from . import factories
 
 
 @pytest.mark.parametrize("device", utils.torch_devices())
 @pytest.mark.parametrize("workers", [1, 2, 4])
 @pytest.mark.parametrize("score", ["sacre-bleu", "rouge-1", "exact-match"])
 def test_init_optimizer(device: str, workers: int, score: str) -> None:
-    corpus = corpus_factories.corpus(device=device)
+    embedder = SbertEmbedder(device=device)
+    corpus = corpus_factories.corpus(embedder=embedder)
     lm = lm_factories.generative_lm(device=device)
     adaptor = adaptor_factories.bigbench_adaptor(name=score, lm=lm)
 
     _ = factories.ax_optim(corpus, lm, adaptor, device=device, workers=workers)
 
 
 @pytest.mark.parametrize("device", utils.torch_devices())
 @pytest.mark.parametrize("workers", [1, 2, 4])
 @pytest.mark.parametrize("score", ["sacre-bleu", "rouge-1", "exact-match"])
 def test_optimize(device: str, workers: int, score: str) -> None:
-    corpus = corpus_factories.corpus(device=device)
+    embedder = SbertEmbedder(device=device)
+    corpus = corpus_factories.corpus(embedder=embedder)
     lm = lm_factories.generative_lm(device=device)
     adaptor = adaptor_factories.bigbench_adaptor(name=score, lm=lm)
     optimizer = factories.ax_optim(corpus, lm, adaptor, device=device, workers=workers)
 
-    Manager().run(optimizer=optimizer, corpus=corpus, steps=10)
+    Manager().run(
+        optimizer=optimizer,
+        embedder=embedder,
+        corpus=corpus,
+        model=lm,
+        adaptor=adaptor,
+        steps=10,
+    )
```

### Comparing `bocoel-0.1.0/tests/core/optim/test_kmedoids.py` & `bocoel-0.1.2/tests/core/optim/test_kmedoids.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from bocoel import Manager
+from bocoel import Manager, SbertEmbedder
 from tests import utils
 from tests.corpora import factories as corpus_factories
 from tests.models.adaptors import factories as adaptor_factories
 from tests.models.lms import factories as lm_factories
 
 from . import factories
 
@@ -21,15 +21,16 @@
         "rouge-score-1",
         "rouge-score-2",
         "rouge-score-l",
         "exact-match",
     ],
 )
 def test_init_optimizer(device: str, score: str) -> None:
-    corpus = corpus_factories.corpus(device=device)
+    embedder = SbertEmbedder(device=device)
+    corpus = corpus_factories.corpus(embedder=embedder)
     lm = lm_factories.generative_lm(device=device)
     adaptor = adaptor_factories.bigbench_adaptor(name=score, lm=lm)
 
     _ = factories.kmedoids_optim(corpus, lm, adaptor)
 
 
 @pytest.mark.parametrize("device", utils.torch_devices())
@@ -44,13 +45,21 @@
         "rouge-score-1",
         "rouge-score-2",
         "rouge-score-l",
         "exact-match",
     ],
 )
 def test_optimize(device: str, score: str) -> None:
-    corpus = corpus_factories.corpus(device=device)
+    embedder = SbertEmbedder(device=device)
+    corpus = corpus_factories.corpus(embedder=embedder)
     lm = lm_factories.generative_lm(device=device)
     adaptor = adaptor_factories.bigbench_adaptor(name=score, lm=lm)
     optimizer = factories.kmedoids_optim(corpus, lm, adaptor)
 
-    Manager().run(optimizer=optimizer, corpus=corpus, steps=15)
+    Manager().run(
+        optimizer=optimizer,
+        embedder=embedder,
+        corpus=corpus,
+        model=lm,
+        adaptor=adaptor,
+        steps=15,
+    )
```

### Comparing `bocoel-0.1.0/tests/corpora/factories.py` & `bocoel-0.1.2/tests/corpora/factories.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from bocoel import (
     ComposedCorpus,
     Corpus,
     Distance,
+    Embedder,
     PandasStorage,
-    SbertEmbedder,
     WhiteningIndex,
 )
-from tests import utils
 
 from .indices import factories
 from .storages import factories as storage_factories
 
 
-@utils.cache
-def corpus(device: str) -> Corpus:
+def corpus(embedder: Embedder) -> Corpus:
     storage = PandasStorage(storage_factories.df())
-    embedder = SbertEmbedder(device=device)
     return ComposedCorpus.index_storage(
         storage=storage,
         embedder=embedder,
         keys=["question"],
         index_backend=WhiteningIndex,
         distance=Distance.INNER_PRODUCT,
         **factories.whiten_kwargs(),
```

### Comparing `bocoel-0.1.0/tests/corpora/embedders/test_sberts.py` & `bocoel-0.1.2/tests/corpora/embedders/test_sberts.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/tests/corpora/indices/factories.py` & `bocoel-0.1.2/tests/corpora/indices/factories.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/tests/corpora/indices/test_faiss.py` & `bocoel-0.1.2/tests/corpora/indices/test_faiss.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/tests/corpora/indices/test_hnswlib.py` & `bocoel-0.1.2/tests/corpora/indices/test_hnswlib.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/tests/corpora/storages/factories.py` & `bocoel-0.1.2/tests/corpora/storages/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 
 def dataset() -> Dataset:
     return Dataset.from_pandas(df())
 
 
 @utils.cache
 def datasets_storage() -> Storage:
-    return DatasetsStorage(dataset())
+    return DatasetsStorage("SetFit/sst2")
```

### Comparing `bocoel-0.1.0/tests/models/adaptors/factories.py` & `bocoel-0.1.2/tests/models/adaptors/factories.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/tests/models/adaptors/test_adaptors.py` & `bocoel-0.1.2/tests/models/adaptors/test_adaptors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 
+from bocoel import SbertEmbedder
 from tests import utils
 from tests.corpora import factories as corpus_factories
 from tests.models.lms import factories as lm_factories
 
 from . import factories
 
 
@@ -19,15 +20,16 @@
         "rouge-score-1",
         "rouge-score-2",
         "rouge-score-l",
         "exact-match",
     ],
 )
 def test_bigbench_adaptor_on_corpus(adaptor_name: str, device: str) -> None:
-    corpus = corpus_factories.corpus(device=device)
+    embedder = SbertEmbedder(device=device)
+    corpus = corpus_factories.corpus(embedder=embedder)
     lm = lm_factories.generative_lm(device=device)
     ev = factories.bigbench_adaptor(adaptor_name, lm=lm)
 
     results = ev.on_corpus(corpus=corpus, indices=[0, 1])
     assert len(results) == 2
 
     assert all(0 <= r <= 1 for r in results), {"results": results, "corpus": corpus}
```

### Comparing `bocoel-0.1.0/tests/models/adaptors/test_scores.py` & `bocoel-0.1.2/tests/models/adaptors/test_scores.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/tests/models/lms/factories.py` & `bocoel-0.1.2/tests/models/lms/factories.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/tests/models/lms/test_huggingface.py` & `bocoel-0.1.2/tests/models/lms/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/.gitignore` & `bocoel-0.1.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 #   This is especially recommended for binary packages to ensure reproducibility, and is more
 #   commonly ignored for libraries.
 #   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
 # poetry.lock
 
 # pdm
 #   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-pdm.lock
+# pdm.lock
 #   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
 #   in version control.
 #   https://pdm.fming.dev/#use-with-ide
 .pdm.toml
 .pdm-python
 
 # PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
```

### Comparing `bocoel-0.1.0/LICENSE.md` & `bocoel-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bocoel-0.1.0/README.md` & `bocoel-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,51 +8,53 @@
 [![Build Pages](https://github.com/rentruewang/bocoel/actions/workflows/build.yaml/badge.svg)](https://github.com/rentruewang/bocoel/actions/workflows/build.yaml)
 [![Formatting](https://github.com/rentruewang/bocoel/actions/workflows/format.yaml/badge.svg)](https://github.com/rentruewang/bocoel/actions/workflows/format.yaml)
 [![Type Checking](https://github.com/rentruewang/bocoel/actions/workflows/typecheck.yaml/badge.svg)](https://github.com/rentruewang/bocoel/actions/workflows/typecheck.yaml)
 [![Unit Testing](https://github.com/rentruewang/bocoel/actions/workflows/unittest.yaml/badge.svg)](https://github.com/rentruewang/bocoel/actions/workflows/unittest.yaml)
 
 
 ![GitHub License](https://img.shields.io/github/license/rentruewang/bocoel)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bocoel)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue)
 [![Built with Material for MkDocs](https://img.shields.io/badge/Material_for_MkDocs-526CFE?style=for-the-badge&logo=MaterialForMkDocs&logoColor=white)](https://squidfunk.github.io/mkdocs-material/)
 
 
 ## 🤔 Why BoCoEL?
 
 Large language models are expensive and slow behemoths, and evaluating them on gigantic modern datasets only makes it worse. 
 
 If only there is a way to just select a meaningful (_and small_) subset of the corpus and obtain a highly accurate evaluation.....
 
-Wait, sounds like [Bayesian Optmization](#bo)!
+Wait, sounds like [Bayesian Optimization](#bo)!
 
 Bocoel works in the following steps:
 
 1. Encode individual entry into embeddings (way cheaper / faster than LLM and reusable).
 2. Use Bayesian optimization to select queries to evaluate.
 3. Use the queries to retrieve from our corpus (with the encoded embeddings).
 4. Profit.
 
 The evaluations generated are easily managed by the provided manager utility.
 
+To our knowledge, this is the first work aiming to reduce computation costs during evaluation (benchmarking) with a (possibly dynamic) budget.
+
 
 ## 🚀 Features
 
 - 🎯 Accurately evaluate large language models with just tens of samples from your selected corpus.
-- 💂‍♂️ Uses the power of Bayesian optimization to select an optimal set of samples for language model to evaluate.
+- 💂‍♂️ Uses the power of Bayesian optimization to select an optimal subset of samples for language model to evaluate.
 - 💯 Evalutes the corpus on the model in addition to evaluating the model on corpus.
 - 🤗 Support for `GPT2`, `Pythia`, `LLAMA` and more through integration with huggingface [transformers](https://huggingface.co/docs/transformers/en/index) and [datasets](https://huggingface.co/docs/datasets/en/index)
 - 🧩 Modular design.
+- 🔎 Efficient representation of the corpus / dataset such as N-sphere representation or whitening of the latent space to agument evaluation quality.
 
 
 ## ⭐ Give us a star!
 
 Like what you see? Please consider giving this a star (★)!
 
 
-
 ## <a id="bo"></a> ♾️ Bayesian Optimization
 
 <img src="https://upload.wikimedia.org/wikipedia/commons/0/02/GpParBayesAnimationSmall.gif" width="30%" align="right"/>
 
 Simply put, Bayesian optimization aims to optimize either the exploration objective (the purple area in the image) or the exploitation object (the height of the black dots). It uses Gaussian processes as a backbone for inference, and uses an **acquisition function** to decide where to sample next. See [here](https://distill.pub/2019/visual-exploration-gaussian-processes/) for an a more in-depth introduction.
 
 Since _Bayesian optimization works well with expensive-to-evaluate black-box model (paraphrase: LLM)_, it is perfect for this particular use case. Bocoel uses Bayesian optimization as a backbone for exploring the embedding space given by our corpus, which allows it to select a good subset acting as a mini snapshot of the corpus.
@@ -75,18 +77,20 @@
 
 Give me the full experience (all optional dependencies):
 
 ```
 pip install "bocoel[all]"
 ```
 
+
 ## 🔬 Usage
 
 See the folder [examples/getting_started](https://github.com/rentruewang/bocoel/tree/main/examples/getting_started) for a simplistic usage of the library to get started with just a few lines of code.
 
+
 ## ✍️ Develop with BoCoEL
 
 Usage examples are under the folder [`examples`](https://github.com/rentruewang/bocoel/tree/main/examples). API reference can be found [here](https://rentruewang.github.io/bocoel/references/overview/).
 
 
 ## 🥰 Contributing
 
@@ -108,12 +112,12 @@
 
 If you find this project helpful in your research, please cite this work at
 
 ```
 @misc{bocoel2024,
     title = {BoCoEL: Bayesian Optimization as a Coverage Tool for Evaluating Large Language Models},
     url = {https://rentruewang.github.io/bocoel/research/},
-    author = {Wang, RenChu and Chuang, Yung-Sung},
+    author = {Wang, RenChu},
     month = {January},
     year = {2024}
 }
 ```
```

### Comparing `bocoel-0.1.0/pyproject.toml` & `bocoel-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bocoel"
-version = "0.1.0"
+version = "0.1.2"
 description = "Bayesian Optimization as a Coverage Tool for Evaluating Large Language Models"
 authors = [
     {name = "RenChu Wang", email = "patrick1031wang@gmail.com"},
 ]
 dependencies = [
     "alive-progress>=3.1.5",
     "ax-platform>=0.3.6",
@@ -70,14 +70,18 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [tool.pdm]
 distribution = "true"
 
+[tool.isort]
+profile = "black"
+
+
 [tool.pdm.dev-dependencies]
 format = [
     "autoflake>=2.2.1",
     "black>=24.1.1",
     "isort>=5.13.2",
 ]
 test = [
```

### Comparing `bocoel-0.1.0/PKG-INFO` & `bocoel-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: bocoel
-Version: 0.1.0
+Version: 0.1.2
 Summary: Bayesian Optimization as a Coverage Tool for Evaluating Large Language Models
 Author-email: RenChu Wang <patrick1031wang@gmail.com>
 License: Apache-2.0
 License-File: LICENSE.md
 Requires-Python: <3.11,>=3.10
 Requires-Dist: alive-progress>=3.1.5
 Requires-Dist: ax-platform>=0.3.6
@@ -20,15 +20,31 @@
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: structlog>=24.1.0
 Requires-Dist: torch>=2.1.2
 Requires-Dist: typeguard>=2.13.3
 Requires-Dist: typing-extensions>=4.9.0
 Requires-Dist: ujson>=5.9.0
 Provides-Extra: all
-Requires-Dist: bocoel[cma,datasets,index,metrics,plots,sklearn-extra,transformers,visual]; extra == 'all'
+Requires-Dist: cma>=3.3.0; extra == 'all'
+Requires-Dist: dash>=2.14.2; extra == 'all'
+Requires-Dist: datasets>=2.16.1; extra == 'all'
+Requires-Dist: faiss-cpu>=1.7.4; extra == 'all'
+Requires-Dist: flask>=3.0.0; extra == 'all'
+Requires-Dist: hiplot>=0.1.33; extra == 'all'
+Requires-Dist: hnswlib>=0.8.0; extra == 'all'
+Requires-Dist: matplotlib>=3.8.2; extra == 'all'
+Requires-Dist: nltk>=3.8.1; extra == 'all'
+Requires-Dist: plotly>=5.18.0; extra == 'all'
+Requires-Dist: rouge-score>=0.1.2; extra == 'all'
+Requires-Dist: rouge>=1.0.1; extra == 'all'
+Requires-Dist: sacrebleu>=2.4.0; extra == 'all'
+Requires-Dist: scikit-learn-extra>=0.3.0; extra == 'all'
+Requires-Dist: seaborn>=0.13.2; extra == 'all'
+Requires-Dist: sentence-transformers>=2.2.2; extra == 'all'
+Requires-Dist: transformers>=4.36.2; extra == 'all'
 Provides-Extra: cma
 Requires-Dist: cma>=3.3.0; extra == 'cma'
 Provides-Extra: datasets
 Requires-Dist: datasets>=2.16.1; extra == 'datasets'
 Provides-Extra: index
 Requires-Dist: faiss-cpu>=1.7.4; extra == 'index'
 Requires-Dist: hnswlib>=0.8.0; extra == 'index'
@@ -62,51 +78,53 @@
 [![Build Pages](https://github.com/rentruewang/bocoel/actions/workflows/build.yaml/badge.svg)](https://github.com/rentruewang/bocoel/actions/workflows/build.yaml)
 [![Formatting](https://github.com/rentruewang/bocoel/actions/workflows/format.yaml/badge.svg)](https://github.com/rentruewang/bocoel/actions/workflows/format.yaml)
 [![Type Checking](https://github.com/rentruewang/bocoel/actions/workflows/typecheck.yaml/badge.svg)](https://github.com/rentruewang/bocoel/actions/workflows/typecheck.yaml)
 [![Unit Testing](https://github.com/rentruewang/bocoel/actions/workflows/unittest.yaml/badge.svg)](https://github.com/rentruewang/bocoel/actions/workflows/unittest.yaml)
 
 
 ![GitHub License](https://img.shields.io/github/license/rentruewang/bocoel)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bocoel)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue)
 [![Built with Material for MkDocs](https://img.shields.io/badge/Material_for_MkDocs-526CFE?style=for-the-badge&logo=MaterialForMkDocs&logoColor=white)](https://squidfunk.github.io/mkdocs-material/)
 
 
 ## 🤔 Why BoCoEL?
 
 Large language models are expensive and slow behemoths, and evaluating them on gigantic modern datasets only makes it worse. 
 
 If only there is a way to just select a meaningful (_and small_) subset of the corpus and obtain a highly accurate evaluation.....
 
-Wait, sounds like [Bayesian Optmization](#bo)!
+Wait, sounds like [Bayesian Optimization](#bo)!
 
 Bocoel works in the following steps:
 
 1. Encode individual entry into embeddings (way cheaper / faster than LLM and reusable).
 2. Use Bayesian optimization to select queries to evaluate.
 3. Use the queries to retrieve from our corpus (with the encoded embeddings).
 4. Profit.
 
 The evaluations generated are easily managed by the provided manager utility.
 
+To our knowledge, this is the first work aiming to reduce computation costs during evaluation (benchmarking) with a (possibly dynamic) budget.
+
 
 ## 🚀 Features
 
 - 🎯 Accurately evaluate large language models with just tens of samples from your selected corpus.
-- 💂‍♂️ Uses the power of Bayesian optimization to select an optimal set of samples for language model to evaluate.
+- 💂‍♂️ Uses the power of Bayesian optimization to select an optimal subset of samples for language model to evaluate.
 - 💯 Evalutes the corpus on the model in addition to evaluating the model on corpus.
 - 🤗 Support for `GPT2`, `Pythia`, `LLAMA` and more through integration with huggingface [transformers](https://huggingface.co/docs/transformers/en/index) and [datasets](https://huggingface.co/docs/datasets/en/index)
 - 🧩 Modular design.
+- 🔎 Efficient representation of the corpus / dataset such as N-sphere representation or whitening of the latent space to agument evaluation quality.
 
 
 ## ⭐ Give us a star!
 
 Like what you see? Please consider giving this a star (★)!
 
 
-
 ## <a id="bo"></a> ♾️ Bayesian Optimization
 
 <img src="https://upload.wikimedia.org/wikipedia/commons/0/02/GpParBayesAnimationSmall.gif" width="30%" align="right"/>
 
 Simply put, Bayesian optimization aims to optimize either the exploration objective (the purple area in the image) or the exploitation object (the height of the black dots). It uses Gaussian processes as a backbone for inference, and uses an **acquisition function** to decide where to sample next. See [here](https://distill.pub/2019/visual-exploration-gaussian-processes/) for an a more in-depth introduction.
 
 Since _Bayesian optimization works well with expensive-to-evaluate black-box model (paraphrase: LLM)_, it is perfect for this particular use case. Bocoel uses Bayesian optimization as a backbone for exploring the embedding space given by our corpus, which allows it to select a good subset acting as a mini snapshot of the corpus.
@@ -129,18 +147,20 @@
 
 Give me the full experience (all optional dependencies):
 
 ```
 pip install "bocoel[all]"
 ```
 
+
 ## 🔬 Usage
 
 See the folder [examples/getting_started](https://github.com/rentruewang/bocoel/tree/main/examples/getting_started) for a simplistic usage of the library to get started with just a few lines of code.
 
+
 ## ✍️ Develop with BoCoEL
 
 Usage examples are under the folder [`examples`](https://github.com/rentruewang/bocoel/tree/main/examples). API reference can be found [here](https://rentruewang.github.io/bocoel/references/overview/).
 
 
 ## 🥰 Contributing
 
@@ -162,12 +182,12 @@
 
 If you find this project helpful in your research, please cite this work at
 
 ```
 @misc{bocoel2024,
     title = {BoCoEL: Bayesian Optimization as a Coverage Tool for Evaluating Large Language Models},
     url = {https://rentruewang.github.io/bocoel/research/},
-    author = {Wang, RenChu and Chuang, Yung-Sung},
+    author = {Wang, RenChu},
     month = {January},
     year = {2024}
 }
 ```
```

