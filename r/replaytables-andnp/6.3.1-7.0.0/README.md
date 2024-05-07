# Comparing `tmp/ReplayTables_andnp-6.3.1.tar.gz` & `tmp/ReplayTables_andnp-7.0.0.tar.gz`

## Comparing `ReplayTables_andnp-6.3.1.tar` & `ReplayTables_andnp-7.0.0.tar`

### file list

```diff
@@ -1,83 +1,82 @@
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 ReplayTables_andnp-6.3.1/Cargo.toml
--rw-r--r--   0     1001      127      888 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/.github/dependabot.yml
--rw-r--r--   0     1001      127     1003 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/.github/workflows/benchmark.yml
--rw-r--r--   0     1001      127     1099 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/.github/workflows/pr_benchmark.yml
--rw-r--r--   0     1001      127     2233 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/.github/workflows/publish.yml
--rw-r--r--   0     1001      127      834 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/.github/workflows/tag.yml
--rw-r--r--   0     1001      127      861 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/.github/workflows/test.yml
--rw-r--r--   0     1001      127      148 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/.gitignore
--rw-r--r--   0     1001      127      265 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     2350 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/README.md
--rw-r--r--   0     1001      127      748 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/BackwardsReplay.py
--rw-r--r--   0     1001      127     6094 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/Distributions.py
--rw-r--r--   0     1001      127     2476 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/PER.py
--rw-r--r--   0     1001      127     2582 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/PSER.py
--rw-r--r--   0     1001      127      803 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/PrototypeBuffer.py
--rw-r--r--   0     1001      127     4358 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/ReplayBuffer.py
--rw-r--r--   0     1001      127     6193 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/_utils/MinMaxHeap.py
--rw-r--r--   0     1001      127     1772 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/_utils/RandDict.py
--rw-r--r--   0     1001      127     2679 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/_utils/SamplableSet.py
--rw-r--r--   0     1001      127     2024 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/_utils/SumTree.py
--rw-r--r--   0     1001      127        0 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/_utils/__init__.py
--rw-r--r--   0     1001      127     1523 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/_utils/jit.py
--rw-r--r--   0     1001      127       58 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/_utils/logger.py
--rw-r--r--   0     1001      127      502 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/_utils/np.py
--rw-r--r--   0     1001      127      850 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/ingress/CircularMapper.py
--rw-r--r--   0     1001      127      599 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/ingress/IndexMapper.py
--rw-r--r--   0     1001      127     3193 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/ingress/LagBuffer.py
--rw-r--r--   0     1001      127     1788 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/ingress/MinHeapMapper.py
--rw-r--r--   0     1001      127     1295 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/ingress/RandomIndexer.py
--rw-r--r--   0     1001      127      956 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/ingress/Trackers.py
--rw-r--r--   0     1001      127     1509 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/interface.py
--rw-r--r--   0     1001      127     1255 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/registry.py
--rw-r--r--   0     1001      127     2190 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/sampling/BackwardsSampler.py
--rw-r--r--   0     1001      127     1292 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/sampling/IndexSampler.py
--rw-r--r--   0     1001      127     1996 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/sampling/PrioritySampler.py
--rw-r--r--   0     1001      127     5388 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/sampling/PrioritySequenceSampler.py
--rw-r--r--   0     1001      127      947 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/sampling/UniformSampler.py
--rw-r--r--   0     1001      127      460 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/sampling/tools.py
--rw-r--r--   0     1001      127     4804 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/storage/BasicStorage.py
--rw-r--r--   0     1001      127     2045 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/storage/CompressedStorage.py
--rw-r--r--   0     1001      127      951 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/storage/MetadataStorage.py
--rw-r--r--   0     1001      127      969 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/storage/NonArrayStorage.py
--rw-r--r--   0     1001      127      974 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/ReplayTables/storage/Storage.py
--rwxr-xr-x   0     1001      127      105 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/dev-setup.sh
--rw-r--r--   0     1001      127     1534 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/requirements.txt
--rwxr-xr-x   0     1001      127      511 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/scripts/publish.sh
--rwxr-xr-x   0     1001      127       47 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/scripts/run_tests.sh
--rw-r--r--   0     1001      127      119 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/setup.cfg
--rw-r--r--   0     1001      127      395 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/src/lib.rs
--rw-r--r--   0     1001      127     5019 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/src/storage/metadata_storage.rs
--rw-r--r--   0     1001      127       26 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/src/storage.rs
--rw-r--r--   0     1001      127     3087 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/src/utils/ref_count.rs
--rw-r--r--   0     1001      127     5400 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/src/utils/sumtree.rs
--rw-r--r--   0     1001      127       36 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/src/utils.rs
--rw-r--r--   0     1001      127      247 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/test.py
--rw-r--r--   0     1001      127        0 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/__init__.py
--rw-r--r--   0     1001      127     4137 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/_utils/fake_data.py
--rw-r--r--   0     1001      127     1219 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/ingress/test_RandomIndexer.py
--rw-r--r--   0     1001      127      998 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/rust/test_RefCount.py
--rw-r--r--   0     1001      127        0 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/sampling/__init__.py
--rw-r--r--   0     1001      127     2584 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/sampling/test_PrioritizedSequenceSampler.py
--rw-r--r--   0     1001      127     1216 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/storage/test_BasicStorage.py
--rw-r--r--   0     1001      127     6419 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/storage/test_Storage.py
--rw-r--r--   0     1001      127     2947 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/test_LagBuffer.py
--rw-r--r--   0     1001      127     4955 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/test_PER.py
--rw-r--r--   0     1001      127     2174 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/test_PrototypeBuffer.py
--rw-r--r--   0     1001      127     5158 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/test_ReplayBuffer.py
--rw-r--r--   0     1001      127     2392 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/test_fuzz.py
--rw-r--r--   0     1001      127     1657 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/test_integration.py
--rw-r--r--   0     1001      127        0 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/utils/__init__.py
--rw-r--r--   0     1001      127      981 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/utils/test_MinMaxHeap.py
--rw-r--r--   0     1001      127     3285 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/tests/utils/test_SumTree.py
--rw-r--r--   0     1001      127        0 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/typings/ReplayTables/__init__.pyi
--rw-r--r--   0     1001      127     1489 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/typings/ReplayTables/rust/__init__.pyi
--rw-r--r--   0     1001      127      108 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/typings/lz4/frame/__init__.pyi
--rw-r--r--   0     1001      127      491 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/typings/numba/__init__.pyi
--rw-r--r--   0     1001      127       55 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/typings/numba/core/errors/__init__.pyi
--rw-r--r--   0     1001      127       38 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/typings/numba/experimental/__init__.pyi
--rw-r--r--   0     1001      127      153 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/typings/numba/typed/__init__.pyi
--rw-r--r--   0     1001      127       34 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/typings/numba/types/__init__.pyi
--rw-r--r--   0     1001      127    12392 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/Cargo.lock
--rw-r--r--   0     1001      127     1152 2024-05-05 19:07:37.000000 ReplayTables_andnp-6.3.1/pyproject.toml
--rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 ReplayTables_andnp-6.3.1/PKG-INFO
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 ReplayTables_andnp-7.0.0/Cargo.toml
+-rw-r--r--   0     1001      127      888 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/.github/dependabot.yml
+-rw-r--r--   0     1001      127     1003 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/.github/workflows/benchmark.yml
+-rw-r--r--   0     1001      127     1099 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/.github/workflows/pr_benchmark.yml
+-rw-r--r--   0     1001      127     2233 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/.github/workflows/publish.yml
+-rw-r--r--   0     1001      127      834 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/.github/workflows/tag.yml
+-rw-r--r--   0     1001      127      861 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      148 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/.gitignore
+-rw-r--r--   0     1001      127      265 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     2350 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/README.md
+-rw-r--r--   0     1001      127      730 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/BackwardsReplay.py
+-rw-r--r--   0     1001      127     6094 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/Distributions.py
+-rw-r--r--   0     1001      127     2635 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/PER.py
+-rw-r--r--   0     1001      127     2749 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/PSER.py
+-rw-r--r--   0     1001      127      795 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/PrototypeBuffer.py
+-rw-r--r--   0     1001      127     4294 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/ReplayBuffer.py
+-rw-r--r--   0     1001      127     6193 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/_utils/MinMaxHeap.py
+-rw-r--r--   0     1001      127     1772 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/_utils/RandDict.py
+-rw-r--r--   0     1001      127     2679 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/_utils/SamplableSet.py
+-rw-r--r--   0     1001      127     2024 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/_utils/SumTree.py
+-rw-r--r--   0     1001      127        0 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/_utils/__init__.py
+-rw-r--r--   0     1001      127     1523 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/_utils/jit.py
+-rw-r--r--   0     1001      127       58 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/_utils/logger.py
+-rw-r--r--   0     1001      127      502 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/_utils/np.py
+-rw-r--r--   0     1001      127     1011 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/ingress/CircularMapper.py
+-rw-r--r--   0     1001      127      724 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/ingress/IndexMapper.py
+-rw-r--r--   0     1001      127     3211 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/ingress/LagBuffer.py
+-rw-r--r--   0     1001      127     1975 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/ingress/MinHeapMapper.py
+-rw-r--r--   0     1001      127     1468 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/ingress/RandomIndexer.py
+-rw-r--r--   0     1001      127      956 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/ingress/Trackers.py
+-rw-r--r--   0     1001      127     1619 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/interface.py
+-rw-r--r--   0     1001      127     1255 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/registry.py
+-rw-r--r--   0     1001      127     2266 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/sampling/BackwardsSampler.py
+-rw-r--r--   0     1001      127     1341 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/sampling/IndexSampler.py
+-rw-r--r--   0     1001      127     2052 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/sampling/PrioritySampler.py
+-rw-r--r--   0     1001      127     5478 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/sampling/PrioritySequenceSampler.py
+-rw-r--r--   0     1001      127      996 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/sampling/UniformSampler.py
+-rw-r--r--   0     1001      127      460 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/sampling/tools.py
+-rw-r--r--   0     1001      127     4901 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/storage/BasicStorage.py
+-rw-r--r--   0     1001      127     2045 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/storage/CompressedStorage.py
+-rw-r--r--   0     1001      127      994 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/storage/MetadataStorage.py
+-rw-r--r--   0     1001      127      969 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/storage/NonArrayStorage.py
+-rw-r--r--   0     1001      127     1023 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/ReplayTables/storage/Storage.py
+-rwxr-xr-x   0     1001      127      105 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/dev-setup.sh
+-rw-r--r--   0     1001      127     1484 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/requirements.txt
+-rwxr-xr-x   0     1001      127      511 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/scripts/publish.sh
+-rwxr-xr-x   0     1001      127       34 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/scripts/run_tests.sh
+-rw-r--r--   0     1001      127      119 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/setup.cfg
+-rw-r--r--   0     1001      127      395 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/src/lib.rs
+-rw-r--r--   0     1001      127     5129 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/src/storage/metadata_storage.rs
+-rw-r--r--   0     1001      127       26 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/src/storage.rs
+-rw-r--r--   0     1001      127     3087 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/src/utils/ref_count.rs
+-rw-r--r--   0     1001      127     5400 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/src/utils/sumtree.rs
+-rw-r--r--   0     1001      127       36 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/src/utils.rs
+-rw-r--r--   0     1001      127        0 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/__init__.py
+-rw-r--r--   0     1001      127     4185 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/_utils/fake_data.py
+-rw-r--r--   0     1001      127     1437 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/ingress/test_RandomIndexer.py
+-rw-r--r--   0     1001      127      998 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/rust/test_RefCount.py
+-rw-r--r--   0     1001      127        0 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/sampling/__init__.py
+-rw-r--r--   0     1001      127     2587 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/sampling/test_PrioritizedSequenceSampler.py
+-rw-r--r--   0     1001      127     1238 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/storage/test_BasicStorage.py
+-rw-r--r--   0     1001      127     6532 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/storage/test_Storage.py
+-rw-r--r--   0     1001      127     2947 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/test_LagBuffer.py
+-rw-r--r--   0     1001      127     4973 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/test_PER.py
+-rw-r--r--   0     1001      127     2072 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/test_PrototypeBuffer.py
+-rw-r--r--   0     1001      127     5168 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/test_ReplayBuffer.py
+-rw-r--r--   0     1001      127     2429 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/test_fuzz.py
+-rw-r--r--   0     1001      127     1657 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/test_integration.py
+-rw-r--r--   0     1001      127        0 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/utils/__init__.py
+-rw-r--r--   0     1001      127      981 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/utils/test_MinMaxHeap.py
+-rw-r--r--   0     1001      127     3285 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/tests/utils/test_SumTree.py
+-rw-r--r--   0     1001      127        0 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/typings/ReplayTables/__init__.pyi
+-rw-r--r--   0     1001      127     1540 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/typings/ReplayTables/rust/__init__.pyi
+-rw-r--r--   0     1001      127      108 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/typings/lz4/frame/__init__.pyi
+-rw-r--r--   0     1001      127      491 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/typings/numba/__init__.pyi
+-rw-r--r--   0     1001      127       55 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/typings/numba/core/errors/__init__.pyi
+-rw-r--r--   0     1001      127       38 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/typings/numba/experimental/__init__.pyi
+-rw-r--r--   0     1001      127      153 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/typings/numba/typed/__init__.pyi
+-rw-r--r--   0     1001      127       34 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/typings/numba/types/__init__.pyi
+-rw-r--r--   0     1001      127    12392 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/Cargo.lock
+-rw-r--r--   0     1001      127     1318 2024-05-07 03:32:56.000000 ReplayTables_andnp-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3340 1970-01-01 00:00:00.000000 ReplayTables_andnp-7.0.0/PKG-INFO
```

### Comparing `ReplayTables_andnp-6.3.1/Cargo.toml` & `ReplayTables_andnp-7.0.0/Cargo.toml`

 * *Files 23% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
 [dependencies]
 bincode = "1.3.3"
 hashbrown = { version = "0.14.5", features = ["serde"] }
 ndarray = { version = "0.15.6", features = ["serde"] }
 numpy = "0.21.0"
 pyo3 = { version = "0.21.2", features = ["extension-module", "generate-import-lib"] }
-serde = { version = "1.0.199", features = ["derive"] }
+serde = { version = "1.0.200", features = ["derive"] }
```

### Comparing `ReplayTables_andnp-6.3.1/.github/dependabot.yml` & `ReplayTables_andnp-7.0.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/.github/workflows/benchmark.yml` & `ReplayTables_andnp-7.0.0/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/.github/workflows/pr_benchmark.yml` & `ReplayTables_andnp-7.0.0/.github/workflows/pr_benchmark.yml`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/.github/workflows/publish.yml` & `ReplayTables_andnp-7.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/.github/workflows/tag.yml` & `ReplayTables_andnp-7.0.0/.github/workflows/tag.yml`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/.github/workflows/test.yml` & `ReplayTables_andnp-7.0.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/README.md` & `ReplayTables_andnp-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/BackwardsReplay.py` & `ReplayTables_andnp-7.0.0/ReplayTables/BackwardsReplay.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,13 +10,13 @@
     jump: int = 1
 
 class BackwardsReplay(ReplayBuffer):
     def __init__(self, max_size: int, lag: int, rng: np.random.Generator, config: BackwardsReplayConfig | None = None):
         super().__init__(max_size, lag, rng)
 
         self._c = config or BackwardsReplayConfig()
-        self._sampler: BackwardsSampler = BackwardsSampler(
+        self._sampler = BackwardsSampler(
             rng=rng,
             max_size=self._storage.max_size,
             reset_probability=self._c.reset_probability,
             jump=self._c.jump,
         )
```

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/Distributions.py` & `ReplayTables_andnp-7.0.0/ReplayTables/Distributions.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/PER.py` & `ReplayTables_andnp-7.0.0/ReplayTables/PER.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from dataclasses import dataclass
 from typing import Any
-from ReplayTables.interface import EID, LaggedTimestep, Batch, Item
+from ReplayTables.interface import LaggedTimestep, Batch, Item, TransId
 from ReplayTables.ReplayBuffer import ReplayBuffer
 from ReplayTables.sampling.PrioritySampler import PrioritySampler
 from ReplayTables.ingress.IndexMapper import IndexMapper
 from ReplayTables.storage.Storage import Storage
 
 @dataclass
 class PERConfig:
@@ -23,48 +23,54 @@
         config: PERConfig | None = None,
         idx_mapper: IndexMapper | None = None,
         storage: Storage | None = None,
     ):
         super().__init__(max_size, lag, rng, idx_mapper=idx_mapper, storage=storage)
 
         self._c = config or PERConfig()
-        self._sampler: PrioritySampler = PrioritySampler(
+        self._sampler = PrioritySampler(
             rng=self._rng,
             max_size=self._storage.max_size,
             uniform_probability=self._c.uniform_probability,
         )
 
         self._max_priority = 1e-16
 
     def _on_add(self, item: Item, transition: LaggedTimestep):
         if transition.extra is not None and 'priority' in transition.extra:
             priority = transition.extra['priority']
+
         elif self._c.new_priority_mode == 'max':
             priority = self._max_priority
+
         elif self._c.new_priority_mode == 'mean':
+            assert isinstance(self._sampler, PrioritySampler)
             total_priority = self._sampler.total_priority()
             priority = total_priority / self.size()
             if priority == 0:
                 priority = 1e-16
+
         else:
             raise NotImplementedError()
 
-        self._sampler.replace(item.idx, transition, priority=priority)
+        self._sampler.replace(item.storage_idx, transition, priority=priority)
 
     def update_batch(self, batch: Batch, **kwargs: Any):
         priorities = kwargs['priorities']
         return self.update_priorities(batch, priorities)
 
     def update_priorities(self, batch: Batch, priorities: np.ndarray):
-        idxs = self._idx_mapper.eids2idxs(batch.eid)
+        idxs = self._idx_mapper.get_storage_idxs(batch.trans_id)
 
         priorities = np.abs(priorities) ** self._c.priority_exponent
         self._sampler.update(idxs, batch, priorities=priorities)
 
         self._max_priority = max(
             self._c.max_decay * self._max_priority,
             priorities.max(),
         )
 
-    def delete_sample(self, eid: EID):
-        idx = self._idx_mapper.eid2idx(eid)
-        self._sampler.mask_sample(idx)
+    def delete_sample(self, tid: TransId):
+        storage_idx = self._idx_mapper.get_storage_idx(tid)
+
+        assert isinstance(self._sampler, PrioritySampler)
+        self._sampler.mask_sample(storage_idx)
```

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/PSER.py` & `ReplayTables_andnp-7.0.0/ReplayTables/PSER.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from dataclasses import dataclass
 from typing import Any
-from ReplayTables.interface import Batch, Item, LaggedTimestep, EID
+from ReplayTables.interface import Batch, Item, LaggedTimestep, TransId
 from ReplayTables.ReplayBuffer import ReplayBuffer
 from ReplayTables.PER import PERConfig
 from ReplayTables.sampling.PrioritySequenceSampler import PrioritySequenceSampler
 from ReplayTables.ingress.IndexMapper import IndexMapper
 from ReplayTables.storage.Storage import Storage
 
 @dataclass
@@ -23,51 +23,57 @@
         config: PSERConfig | None = None,
         idx_mapper: IndexMapper | None = None,
         storage: Storage | None = None,
     ):
         super().__init__(max_size, lag, rng, idx_mapper=idx_mapper, storage=storage)
 
         self._c = config or PSERConfig()
-        self._sampler: PrioritySequenceSampler = PrioritySequenceSampler(
+        self._sampler = PrioritySequenceSampler(
             self._rng,
             self._storage.max_size,
             self._c.uniform_probability,
             self._c.trace_decay,
             self._c.trace_depth,
             self._c.combinator,
         )
 
         self._max_priority = 1e-16
 
     def _on_add(self, item: Item, transition: LaggedTimestep):
         if transition.extra is not None and 'priority' in transition.extra:
             priority = transition.extra['priority']
+
         elif self._c.new_priority_mode == 'max':
             priority = self._max_priority
+
         elif self._c.new_priority_mode == 'mean':
+            assert isinstance(self._sampler, PrioritySequenceSampler)
             total_priority = self._sampler.total_priority()
             priority = total_priority / self.size()
             if priority == 0:
                 priority = 1e-16
+
         else:
             raise NotImplementedError()
 
-        self._sampler.replace(item.idx, transition, priority=priority)
+        self._sampler.replace(item.storage_idx, transition, priority=priority)
 
     def update_batch(self, batch: Batch, **kwargs: Any):
         priorities = kwargs['priorities']
         return self.update_priorities(batch, priorities)
 
     def update_priorities(self, batch: Batch, priorities: np.ndarray):
-        idxs = self._idx_mapper.eids2idxs(batch.eid)
+        idxs = self._idx_mapper.get_storage_idxs(batch.trans_id)
 
         priorities = np.abs(priorities) ** self._c.priority_exponent
         self._sampler.update(idxs, batch, priorities=priorities)
 
         self._max_priority = max(
             self._c.max_decay * self._max_priority,
             priorities.max(),
         )
 
-    def delete_sample(self, eid: EID):
-        idx = self._idx_mapper.eid2idx(eid)
-        self._sampler.mask_sample(idx)
+    def delete_sample(self, tid: TransId):
+        storage_idx = self._idx_mapper.get_storage_idx(tid)
+
+        assert isinstance(self._sampler, PrioritySequenceSampler)
+        self._sampler.mask_sample(storage_idx)
```

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/PrototypeBuffer.py` & `ReplayTables_andnp-7.0.0/ReplayTables/PrototypeBuffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,7 @@
             rng: np.random.Generator,
             idx_mapper: IndexMapper | None = None,
             storage: Storage | None = None,
             sampler: IndexSampler | None = None,
     ):
         super().__init__(max_size, lag, rng, idx_mapper=idx_mapper, storage=storage, sampler=sampler)
         self._idx_mapper: IndexMapper = RandomIndexer(max_size, rng=self._rng)
-
```

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/ReplayBuffer.py` & `ReplayTables_andnp-7.0.0/ReplayTables/ReplayBuffer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from abc import abstractmethod
 from typing import Any
 from ReplayTables._utils.logger import logger
-from ReplayTables.interface import Timestep, LaggedTimestep, Batch, EID, EIDs, Item
+from ReplayTables.interface import Timestep, LaggedTimestep, Batch, Item, TransIds
 from ReplayTables.ingress.IndexMapper import IndexMapper
 from ReplayTables.ingress.CircularMapper import CircularMapper
 from ReplayTables.ingress.LagBuffer import LagBuffer
 from ReplayTables.sampling.IndexSampler import IndexSampler
 from ReplayTables.sampling.UniformSampler import UniformSampler
 from ReplayTables.storage.BasicStorage import BasicStorage
 from ReplayTables.storage.Storage import Storage
@@ -36,15 +36,21 @@
 
     def size(self) -> int:
         return max(0, len(self._storage))
 
     def add(self, transition: LaggedTimestep):
         if not self._built: self._deferred_init()
 
-        idx = self._idx_mapper.add_eid(transition.eid)
+        idx = self._idx_mapper.add_transition(transition)
+
+        # if the mapper does not assign an IDX
+        # then don't store the transition
+        if idx is None:
+            return
+
         item = self._storage.add(idx, transition)
         self._on_add(item, transition)
 
     def sample(self, n: int) -> Batch:
         idxs = self._sampler.sample(n)
         samples = self._storage.get(idxs)
         return samples
@@ -72,33 +78,23 @@
 
         if len(idx_list) > n:
             idx_list = idx_list[:n]
 
         idxs: Any = np.asarray(idx_list, dtype=np.int64)
         return self._storage.get(idxs)
 
-    def isr_weights(self, eids: EIDs) -> np.ndarray:
-        idxs = self._idx_mapper.eids2idxs(eids)
+    def isr_weights(self, tids: TransIds) -> np.ndarray:
+        idxs = self._idx_mapper.get_storage_idxs(tids)
         weights = self._sampler.isr_weights(idxs)
         return weights
 
-    def get(self, eids: EIDs):
-        idxs = self._idx_mapper.eids2idxs(eids)
+    def get(self, tids: TransIds):
+        idxs = self._idx_mapper.get_storage_idxs(tids)
         return self._storage.get(idxs)
 
-    def next_eid(self) -> EID:
-        eid: Any = self._t
-        self._t += 1
-        return eid
-
-    def last_eid(self) -> EID:
-        assert self._t > 0, "No previous EID!"
-        last: Any = self._t - 1
-        return last
-
     def use_storage(self, storage: Storage):
         assert self._max_size <= storage.max_size
         self._storage = storage
 
     def update_batch(self, batch: Batch, **kwargs: Any): ...
 
     @abstractmethod
@@ -125,8 +121,8 @@
 
         return out
 
     def flush(self):
         self._lag_buffer.flush()
 
     def _on_add(self, item: Item, transition: LaggedTimestep):
-        self._sampler.replace(item.idx, transition)
+        self._sampler.replace(item.storage_idx, transition)
```

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/_utils/MinMaxHeap.py` & `ReplayTables_andnp-7.0.0/ReplayTables/_utils/MinMaxHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/_utils/RandDict.py` & `ReplayTables_andnp-7.0.0/ReplayTables/_utils/RandDict.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/_utils/SamplableSet.py` & `ReplayTables_andnp-7.0.0/ReplayTables/_utils/SamplableSet.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/_utils/SumTree.py` & `ReplayTables_andnp-7.0.0/ReplayTables/_utils/SumTree.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/_utils/jit.py` & `ReplayTables_andnp-7.0.0/ReplayTables/_utils/jit.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/ingress/LagBuffer.py` & `ReplayTables_andnp-7.0.0/ReplayTables/ingress/LagBuffer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import numpy as np
 from ReplayTables._utils.jit import try2jit
 from typing import Any, Dict, List, Tuple
-from ReplayTables.interface import Timestep, LaggedTimestep, EID, XID
+from ReplayTables.interface import Timestep, LaggedTimestep, XID, TransId
 
 class LagBuffer:
     def __init__(self, lag: int):
         self._lag = lag
         self._max_len = lag + 1
 
         self._idx = 0
         self._xid: Any = 0
-        self._eid: Any = 0
+        self._tid: Any = 0
 
         self._buffer: Dict[int, Tuple[XID | None, Timestep]] = {}
         self._r = np.zeros(self._max_len, dtype=np.float_)
         self._g = np.zeros(self._max_len, dtype=np.float_)
 
     def add(self, experience: Timestep):
         self._idx = (self._idx + 1) % self._max_len
@@ -34,15 +34,15 @@
         f_idx = (idx - self._lag) % self._max_len
         f_xid, f = self._buffer[f_idx]
         r, g = _accumulate_return(self._r, self._g, f_idx, self._lag, self._max_len)
 
         assert f.x is not None
         assert f_xid is not None
         out.append(LaggedTimestep(
-            eid=self._next_eid(),
+            trans_id=self._next_tid(),
             xid=f_xid,
             x=f.x,
             a=f.a,
             r=r,
             gamma=g,
             extra=f.extra or {},
             terminal=experience.terminal,
@@ -57,15 +57,15 @@
             start = (f_idx + i) % self._max_len
             f_xid, f = self._buffer[start]
             r, g = _accumulate_return(self._r, self._g, start, self._lag - i, self._max_len)
 
             assert f.x is not None
             assert f_xid is not None
             out.append(LaggedTimestep(
-                eid=self._next_eid(),
+                trans_id=self._next_tid(),
                 xid=f_xid,
                 x=f.x,
                 a=f.a,
                 r=r,
                 gamma=g,
                 extra=f.extra or {},
                 terminal=experience.terminal,
@@ -86,18 +86,18 @@
 
     def flush(self):
         self._buffer = {}
         self._idx = 0
         self._r = np.zeros(self._max_len, dtype=np.float_)
         self._g = np.zeros(self._max_len, dtype=np.float_)
 
-    def _next_eid(self) -> EID:
-        eid = self._eid
-        self._eid += 1
-        return eid
+    def _next_tid(self) -> TransId:
+        tid = self._tid
+        self._tid += 1
+        return tid
 
     def _next_xid(self) -> XID:
         xid = self._xid
         self._xid += 1
         return xid
```

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/ingress/MinHeapMapper.py` & `ReplayTables_andnp-7.0.0/ReplayTables/ingress/MinHeapMapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 import numpy as np
 from typing import Any, Dict
 from ReplayTables.ingress.IndexMapper import IndexMapper
-from ReplayTables.interface import EID, IDX, EIDs, IDXs
+from ReplayTables.interface import LaggedTimestep, StorageIdx, StorageIdxs, TransId, TransIds
 from ReplayTables._utils.MinMaxHeap import MinMaxHeap
 
 class MinHeapMapper(IndexMapper):
     def __init__(self, max_size: int):
         super().__init__(max_size)
 
         self._heap = MinMaxHeap()
-        self._eid2idx: Dict[EID, IDX] = {}
+        self._eid2idx: Dict[TransId, StorageIdx] = {}
         self._idx2eid = np.zeros(max_size, dtype=np.int64)
 
-    def eid2idx(self, eid: EID) -> IDX:
+    def get_storage_idx(self, tid: TransId) -> StorageIdx:
         default: Any = -1
-        return self._eid2idx.get(eid, default)
+        return self._eid2idx.get(tid, default)
 
-    def eids2idxs(self, eids: EIDs) -> IDXs:
-        f = np.vectorize(self.eid2idx, otypes=[np.int64])
-        return f(eids)
+    def get_storage_idxs(self, tids: TransIds) -> StorageIdxs:
+        f = np.vectorize(self.get_storage_idx, otypes=[np.int64])
+        return f(tids)
 
-    def add_eid(self, eid: EID, /, **kwargs: Any) -> IDX:
+    def add_transition(self, transition: LaggedTimestep, /, **kwargs: Any) -> StorageIdx:
         # check if priority is given, else assume max
         if 'priority' in kwargs:
             p = kwargs['priority']
         else:
             p, _ = self._heap.max()
 
         # when not full, next index is just the current size
         idx: Any = self._size
 
         # when full, delete lowest priority
         if self._size == self._max_size:
             _, idx = self._heap.min()
             self._heap.update(p, idx)
 
-            last_eid = self._idx2eid[idx]
-            del self._eid2idx[last_eid]
+            last_tid: Any = self._idx2eid[idx]
+            del self._eid2idx[last_tid]
 
         else:
             self._heap.add(p, idx)
 
-        self._eid2idx[eid] = idx
-        self._idx2eid[idx] = eid
+        tid = transition.trans_id
+        self._eid2idx[tid] = idx
+        self._idx2eid[idx] = tid
 
         self._size = min(self._size + 1, self._max_size)
         return idx
 
-    def update_eid(self, eid: EID, /, **kwargs: Any):
+    def update_transition(self, tid: TransId, /, **kwargs: Any):
         assert 'priority' in kwargs
         p = kwargs['priority']
 
-        idx = self._eid2idx[eid]
+        idx = self._eid2idx[tid]
         self._heap.update(p, idx)
 
-    def has_eids(self, eids: EIDs):
+    def has_transitions(self, tids: TransIds):
         f = np.vectorize(lambda e: e in self._eid2idx, otypes=[np.bool_])
-        return f(eids)
+        return f(tids)
```

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/ingress/Trackers.py` & `ReplayTables_andnp-7.0.0/ReplayTables/ingress/Trackers.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/registry.py` & `ReplayTables_andnp-7.0.0/ReplayTables/registry.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/sampling/BackwardsSampler.py` & `ReplayTables_andnp-7.0.0/ReplayTables/sampling/BackwardsSampler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from typing import Any
 from ReplayTables.sampling.IndexSampler import IndexSampler
-from ReplayTables.interface import IDX, IDXs, EIDs, LaggedTimestep, Batch
+from ReplayTables.interface import LaggedTimestep, Batch, StorageIdx, StorageIdxs, TransIds
 from ReplayTables.sampling.tools import back_sequence, in_set
 
 
 class BackwardsSampler(IndexSampler):
     def __init__(
         self,
         rng: np.random.Generator,
@@ -13,53 +13,53 @@
         jump: int,
         reset_probability: float,
     ) -> None:
         super().__init__(rng, max_size)
         self._reset = reset_probability
         self._jump = jump
         self._batch_size: int | None = None
-        self._prior_eids: EIDs | None = None
+        self._prior_tids: TransIds | None = None
 
         self._terminal = set[int]()
         # numba needs help with type inference
         # so add a dummy value to the set
         self._terminal.add(-1)
 
-    def replace(self, idx: IDX, transition: LaggedTimestep, /, **kwargs: Any) -> None:
+    def replace(self, idx: StorageIdx, transition: LaggedTimestep, /, **kwargs: Any) -> None:
         self._terminal.discard(idx)
         if transition.terminal:
             self._terminal.add(idx)
 
-    def update(self, idxs: IDXs, batch: Batch, /, **kwargs: Any) -> None:
+    def update(self, idxs: StorageIdxs, batch: Batch, /, **kwargs: Any) -> None:
         ...
 
-    def isr_weights(self, idxs: IDXs):
+    def isr_weights(self, idxs: StorageIdxs):
         return np.ones(len(idxs))
 
-    def sample(self, n: int) -> IDXs:
+    def sample(self, n: int) -> StorageIdxs:
         idxs: Any = self._rng.integers(0, self._mapper.size, size=n, dtype=np.int64)
-        reset_eids = self._storage.meta.get_items_by_idx(idxs).eids
+        reset_tids = self._storage.meta.get_items_by_idx(idxs).trans_ids
 
-        if self._prior_eids is None or self._batch_size != n:
-            self._prior_eids = reset_eids
+        if self._prior_tids is None or self._batch_size != n:
+            self._prior_tids = reset_tids
             self._batch_size = n
             return idxs
 
-        eids: Any = self._prior_eids - self._jump
+        tids: Any = self._prior_tids - self._jump
 
-        back_seq = back_sequence(self._prior_eids, self._jump)
+        back_seq = back_sequence(self._prior_tids, self._jump)
         back_seq = back_seq.reshape(n * self._jump)
 
         is_term = in_set(back_seq, self._terminal)
         is_term = is_term.reshape((n, self._jump))
         is_term = np.any(is_term, axis=1)
 
-        is_valid = self._mapper.has_eids(eids)
+        is_valid = self._mapper.has_transitions(tids)
         should_reset = is_term | (1 - is_valid) | (self._rng.random(size=n) < self._reset)
 
-        new_eids = (1 - should_reset) * eids + should_reset * reset_eids
-        self._prior_eids = new_eids
+        new_eids = (1 - should_reset) * tids + should_reset * reset_tids
+        self._prior_tids = new_eids
 
-        return self._mapper.eids2idxs(new_eids)
+        return self._mapper.get_storage_idxs(new_eids)
 
-    def stratified_sample(self, n: int) -> IDXs:
+    def stratified_sample(self, n: int) -> StorageIdxs:
         raise NotImplementedError()
```

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/sampling/IndexSampler.py` & `ReplayTables_andnp-7.0.0/ReplayTables/sampling/IndexSampler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from abc import abstractmethod
 from typing import Any
-from ReplayTables.interface import IDX, IDXs, LaggedTimestep, Batch
+from ReplayTables.interface import LaggedTimestep, Batch, StorageIdx, StorageIdxs
 from ReplayTables.Distributions import UniformDistribution
 from ReplayTables.storage.Storage import Storage
 from ReplayTables.ingress.IndexMapper import IndexMapper
 
 _tmp: Any = None
 
 class IndexSampler:
@@ -21,25 +21,25 @@
     def deferred_init(self, storage: Storage, mapper: IndexMapper):
         assert not self._built
         self._storage = storage
         self._mapper = mapper
         self._built = True
 
     @abstractmethod
-    def replace(self, idx: IDX, transition: LaggedTimestep, /, **kwargs: Any) -> None:
+    def replace(self, idx: StorageIdx, transition: LaggedTimestep, /, **kwargs: Any) -> None:
         ...
 
     @abstractmethod
-    def update(self, idxs: IDXs, batch: Batch, /, **kwargs: Any) -> None:
+    def update(self, idxs: StorageIdxs, batch: Batch, /, **kwargs: Any) -> None:
         ...
 
     @abstractmethod
-    def isr_weights(self, idxs: IDXs) -> np.ndarray:
+    def isr_weights(self, idxs: StorageIdxs) -> np.ndarray:
         ...
 
     @abstractmethod
-    def sample(self, n: int) -> IDXs:
+    def sample(self, n: int) -> StorageIdxs:
         ...
 
     @abstractmethod
-    def stratified_sample(self, n: int) -> IDXs:
+    def stratified_sample(self, n: int) -> StorageIdxs:
         ...
```

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/sampling/PrioritySampler.py` & `ReplayTables_andnp-7.0.0/ReplayTables/sampling/PrioritySampler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from typing import Any
 from ReplayTables.Distributions import MixinUniformDistribution, SubDistribution, PrioritizedDistribution, MixtureDistribution
-from ReplayTables.interface import IDX, IDXs, LaggedTimestep, Batch
+from ReplayTables.interface import LaggedTimestep, Batch, StorageIdx, StorageIdxs
 from ReplayTables.sampling.IndexSampler import IndexSampler
 
 class PrioritySampler(IndexSampler):
     def __init__(
         self,
         rng: np.random.Generator,
         max_size: int,
@@ -18,39 +18,39 @@
         self._uniform = MixinUniformDistribution()
         self._p_dist = PrioritizedDistribution()
         self._dist = MixtureDistribution(self._max_size, dists=[
             SubDistribution(d=self._p_dist, p=1 - uniform_probability),
             SubDistribution(d=self._uniform, p=uniform_probability)
         ])
 
-    def replace(self, idx: IDX, transition: LaggedTimestep, /, **kwargs: Any) -> None:
+    def replace(self, idx: StorageIdx, transition: LaggedTimestep, /, **kwargs: Any) -> None:
         idxs = np.array([idx], dtype=np.int64)
 
         priority: float = kwargs['priority']
         priorities = np.array([priority])
         self._uniform.update(idxs)
         self._p_dist.update(idxs, priorities)
 
-    def update(self, idxs: IDXs, batch: Batch, /, **kwargs: Any) -> None:
+    def update(self, idxs: StorageIdxs, batch: Batch, /, **kwargs: Any) -> None:
         priorities = kwargs['priorities']
         self._uniform.update(idxs)
         self._p_dist.update(idxs, priorities)
 
-    def isr_weights(self, idxs: IDXs):
+    def isr_weights(self, idxs: StorageIdxs):
         return self._dist.isr(self._target, idxs)
 
-    def sample(self, n: int) -> IDXs:
+    def sample(self, n: int) -> StorageIdxs:
         idxs: Any = self._dist.sample(self._rng, n)
         return idxs
 
-    def stratified_sample(self, n: int) -> IDXs:
+    def stratified_sample(self, n: int) -> StorageIdxs:
         idxs: Any = self._dist.stratified_sample(self._rng, n)
         return idxs
 
-    def mask_sample(self, idx: IDX):
+    def mask_sample(self, idx: StorageIdx):
         idxs = np.array([idx], dtype=np.int64)
         zero = np.zeros(1)
 
         self._p_dist.update(idxs, zero)
         self._uniform.set(idxs, zero)
 
     def total_priority(self):
```

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/sampling/PrioritySequenceSampler.py` & `ReplayTables_andnp-7.0.0/ReplayTables/sampling/PrioritySequenceSampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Set
 
 from ReplayTables.Distributions import PrioritizedDistribution, SubDistribution, MixtureDistribution, MixinUniformDistribution
 from ReplayTables._utils.SumTree import SumTree
 from ReplayTables.sampling.IndexSampler import IndexSampler
 from ReplayTables.storage.Storage import Storage
 from ReplayTables.ingress.IndexMapper import IndexMapper
-from ReplayTables.interface import IDX, Batch, IDXs, EIDs, LaggedTimestep
+from ReplayTables.interface import Batch, LaggedTimestep, StorageIdx, StorageIdxs, TransIds
 from ReplayTables._utils.jit import try2jit
 from ReplayTables.sampling.tools import back_sequence
 
 class PrioritySequenceSampler(IndexSampler):
     def __init__(
         self,
         rng: np.random.Generator,
@@ -45,40 +45,40 @@
 
         self._uniform = MixinUniformDistribution()
         self._dist = MixtureDistribution(self._max_size, dists=[
             SubDistribution(d=self._ps_dist, p=1 - self._uniform_prob),
             SubDistribution(d=self._uniform, p=self._uniform_prob)
         ])
 
-    def replace(self, idx: IDX, transition: LaggedTimestep, /, **kwargs: Any) -> None:
+    def replace(self, idx: StorageIdx, transition: LaggedTimestep, /, **kwargs: Any) -> None:
         self._terminal.discard(int(idx))
         if transition.terminal:
             self._terminal.add(int(idx))
 
         priority: float = kwargs['priority']
         self._uniform.update_single(idx)
         self._ps_dist.update_single(idx, priority)
 
-    def update(self, idxs: IDXs, batch: Batch, /, **kwargs: Any) -> None:
+    def update(self, idxs: StorageIdxs, batch: Batch, /, **kwargs: Any) -> None:
         priorities = kwargs['priorities']
         self._uniform.update(idxs)
-        self._ps_dist.update_seq(batch.eid, idxs, priorities, terminal=self._terminal)
+        self._ps_dist.update_seq(batch.trans_id, idxs, priorities, terminal=self._terminal)
 
-    def isr_weights(self, idxs: IDXs):
+    def isr_weights(self, idxs: StorageIdxs):
         return self._dist.isr(self._target, idxs)
 
-    def sample(self, n: int) -> IDXs:
+    def sample(self, n: int) -> StorageIdxs:
         idxs: Any = self._dist.sample(self._rng, n)
         return idxs
 
-    def stratified_sample(self, n: int) -> IDXs:
+    def stratified_sample(self, n: int) -> StorageIdxs:
         idxs: Any = self._dist.stratified_sample(self._rng, n)
         return idxs
 
-    def mask_sample(self, idx: IDX):
+    def mask_sample(self, idx: StorageIdx):
         idxs = np.array([idx], dtype=np.int64)
         zero = np.zeros(1)
 
         self._ps_dist.update(idxs, zero)
         self._uniform.set(idxs, zero)
 
     def total_priority(self):
@@ -99,19 +99,19 @@
 
         self._storage = storage
         self._mapper = mapper
 
         # pre-compute and cache this
         self._trace = np.cumprod(np.ones(self._c.trace_depth) * self._c.trace_decay)
 
-    def update_seq(self, eids: EIDs, idxs: IDXs, priorities: np.ndarray, terminal: Set[int]):
-        b_eids: Any = back_sequence(eids, self._c.trace_depth)
+    def update_seq(self, tids: TransIds, idxs: StorageIdxs, priorities: np.ndarray, terminal: Set[int]):
+        b_eids: Any = back_sequence(tids, self._c.trace_depth)
 
-        b_idxs = self._mapper.eids2idxs(b_eids)
-        idx_mask = _term_sequence(b_idxs, terminal) | (~self._mapper.has_eids(b_eids))
+        b_idxs = self._mapper.get_storage_idxs(b_eids)
+        idx_mask = _term_sequence(b_idxs, terminal) | (~self._mapper.has_transitions(b_eids))
 
         u_idx, u_priorities = _get_priorities(
             self.tree,
             self.dim,
             b_idxs,
             idx_mask,
             self._trace,
```

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/storage/BasicStorage.py` & `ReplayTables_andnp-7.0.0/ReplayTables/storage/BasicStorage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import numpy as np
 import ReplayTables._utils.np as npu
 
 from typing import Any, Dict
-from ReplayTables.interface import Batch, LaggedTimestep, IDX, IDXs, SIDX, SIDXs, Item
+from ReplayTables.interface import Batch, LaggedTimestep, SIDX, SIDXs, Item, StorageIdx, StorageIdxs
 from ReplayTables.storage.Storage import Storage
 
 
 class BasicStorage(Storage):
     def __init__(self, max_size: int):
         super().__init__(max_size)
 
         self._built = False
 
-        self._extras: Dict[IDX, Any] = {}
+        self._extras: Dict[StorageIdx, Any] = {}
         self._r = np.ones(max_size, dtype=np.float_) * np.nan
         self._term = np.empty(max_size, dtype=np.bool_)
         self._gamma = np.ones(max_size, dtype=np.float_) * np.nan
 
         # building dummy values here for type inference
         self._state_store: Any = np.empty(0)
         self._a = np.zeros(0)
@@ -26,20 +26,20 @@
 
         shape = transition.x.shape
         self._state_store = np.empty((self._max_size + 1, ) + shape, dtype=transition.x.dtype)
         self._a = np.empty(self._max_size, dtype=npu.get_dtype(transition.a))
 
         self._state_store[-1] = 0
 
-    def add(self, idx: IDX, transition: LaggedTimestep, /, **kwargs: Any):
+    def add(self, idx: StorageIdx, transition: LaggedTimestep, /, **kwargs: Any):
         if not self._built: self._deferred_init(transition)
 
         # stash metadata
         item, last_item = self.meta.add_item(
-            eid=transition.eid,
+            eid=transition.trans_id,
             idx=idx,
             xid=transition.xid,
             n_xid=transition.n_xid,
         )
 
         # make room in state storage
         if last_item is not None:
@@ -57,15 +57,15 @@
         # if there is a bootstrap state, then store that too
         if item.n_sidx is not None:
             assert transition.n_x is not None
             self._store_state(item.n_sidx, transition.n_x)
 
         return item
 
-    def set(self, idx: IDX, transition: LaggedTimestep):
+    def set(self, idx: StorageIdx, transition: LaggedTimestep):
         if not self._built: self._deferred_init(transition)
 
         item = self.meta.get_item_by_idx(idx)
 
         self._r[idx] = transition.r
         self._a[idx] = transition.a
         self._term[idx] = transition.terminal
@@ -76,61 +76,61 @@
 
         if item.n_sidx is not None:
             assert transition.n_x is not None
             self._store_state(item.n_sidx, transition.n_x)
 
         return item
 
-    def get(self, idxs: IDXs) -> Batch:
+    def get(self, idxs: StorageIdxs) -> Batch:
         items = self.meta.get_items_by_idx(idxs)
 
         x = self._load_states(items.sidxs)
         xp = self._load_states(items.n_sidxs)
 
         return Batch(
             x=x,
             a=self._a[idxs],
             r=self._r[idxs],
             gamma=self._gamma[idxs],
             terminal=self._term[idxs],
-            eid=items.eids,
+            trans_id=items.trans_ids,
             xp=xp,
         )
 
-    def get_item(self, idx: IDX) -> LaggedTimestep:
+    def get_item(self, idx: StorageIdx) -> LaggedTimestep:
         item = self.meta.get_item_by_idx(idx)
         n_x = None
 
         if item.n_xid is not None:
             assert item.n_sidx is not None
             n_x = self._load_state(item.n_sidx)
 
         return LaggedTimestep(
             x=self._load_state(item.sidx),
             a=self._a[idx],
             r=self._r[idx],
             gamma=self._gamma[idx],
             terminal=self._term[idx],
-            eid=item.eid,
+            trans_id=item.trans_id,
             xid=item.xid,
             extra=self._extras[idx],
             n_xid=item.n_xid,
             n_x=n_x,
         )
 
-    def delete(self, idx: IDX):
+    def delete(self, idx: StorageIdx):
         item = self.meta.get_item_by_idx(idx)
         self.delete_item(item)
 
     def delete_item(self, item: Item):
         if not self.meta.has_xid(item.xid):
             self._remove_state(item.sidx)
 
-        if item.idx in self._extras:
-            del self._extras[item.idx]
+        if item.storage_idx in self._extras:
+            del self._extras[item.storage_idx]
 
         if item.n_xid is not None and not self.meta.has_xid(item.n_xid):
             assert item.n_sidx is not None
             self._remove_state(item.n_sidx)
 
     def __len__(self):
         return len(self._extras)
```

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/storage/CompressedStorage.py` & `ReplayTables_andnp-7.0.0/ReplayTables/storage/CompressedStorage.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/storage/MetadataStorage.py` & `ReplayTables_andnp-7.0.0/ReplayTables/storage/MetadataStorage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Tuple
-from ReplayTables.interface import Item, Items, EID, IDX, IDXs, XID
+from ReplayTables.interface import Item, Items, XID, StorageIdx, StorageIdxs, TransId
 import ReplayTables.rust as ru
 
 _EID_C = 0
 _XID_C = 1
 _NXID_C = 2
 _SIDX_C = 3
 _NSIDX_C = 4
 
 class MetadataStorage:
     def __init__(self, max_size: int, null_idx: int):
         self._m = ru.MetadataStorage(max_size, null_idx)
 
-    def get_item_by_idx(self, idx: IDX) -> Item:
+    def get_item_by_idx(self, idx: StorageIdx) -> Item:
         return self._m.get_item_by_idx(idx)
 
-    def get_items_by_idx(self, idxs: IDXs) -> Items:
+    def get_items_by_idx(self, idxs: StorageIdxs) -> Items:
         return self._m.get_items_by_idx(idxs)
 
-    def add_item(self, eid: EID, idx: IDX, xid: XID, n_xid: XID | None) -> Tuple[Item, Item | None]:
+    def add_item(self, eid: TransId, idx: StorageIdx, xid: XID, n_xid: XID | None) -> Tuple[Item, Item | None]:
         return self._m.add_item(eid, idx, xid, n_xid)
 
     def has_xid(self, xid: XID):
         return self._m.has_xid(xid)
 
     def __getstate__(self):
         return {
```

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/storage/NonArrayStorage.py` & `ReplayTables_andnp-7.0.0/ReplayTables/storage/NonArrayStorage.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/ReplayTables/storage/Storage.py` & `ReplayTables_andnp-7.0.0/ReplayTables/storage/Storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from abc import abstractmethod
 from typing import Any
-from ReplayTables.interface import Batch, LaggedTimestep, IDX, IDXs, Item
+from ReplayTables.interface import Batch, LaggedTimestep, Item, StorageIdx, StorageIdxs
 from ReplayTables.storage.MetadataStorage import MetadataStorage
 
 class Storage:
     def __init__(self, max_size: int):
         self._max_size = max_size
         self._max_i = np.iinfo(np.int64).max
         self.meta = MetadataStorage(max_size, self._max_i)
@@ -15,25 +15,25 @@
         return self._max_size
 
     @abstractmethod
     def __len__(self) -> int:
         ...
 
     @abstractmethod
-    def get(self, idxs: IDXs) -> Batch:
+    def get(self, idxs: StorageIdxs) -> Batch:
         ...
 
     @abstractmethod
-    def get_item(self, idx: IDX) -> LaggedTimestep:
+    def get_item(self, idx: StorageIdx) -> LaggedTimestep:
         ...
 
     @abstractmethod
-    def set(self, idx: IDX, transition: LaggedTimestep) -> Item:
+    def set(self, idx: StorageIdx, transition: LaggedTimestep) -> Item:
         ...
 
     @abstractmethod
-    def add(self, idx: IDX, transition: LaggedTimestep, /, **kwargs: Any) -> Item:
+    def add(self, idx: StorageIdx, transition: LaggedTimestep, /, **kwargs: Any) -> Item:
         ...
 
     @abstractmethod
-    def delete(self, idx: IDX):
+    def delete(self, idx: StorageIdx):
         ...
```

### Comparing `ReplayTables_andnp-6.3.1/requirements.txt` & `ReplayTables_andnp-7.0.0/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -25,19 +25,18 @@
     # via commitizen
 llvmlite==0.42.0
     # via numba
 lz4==4.3.3
 markupsafe==2.1.5
     # via jinja2
 maturin==1.5.0
-mypy==1.9.0
-mypy-extensions==1.0.0
-    # via mypy
 nodeenv==1.8.0
-    # via pre-commit
+    # via
+    #   pre-commit
+    #   pyright
 numba==0.59.1
 numpy==1.26.4
     # via
     #   numba
     #   scipy
 packaging==24.0
     # via
@@ -49,14 +48,15 @@
 pluggy==1.4.0
     # via pytest
 pre-commit==3.7.0
 prompt-toolkit==3.0.36
     # via questionary
 py-cpuinfo==9.0.0
     # via pytest-benchmark
+pyright==1.1.361
 pytest==8.1.1
     # via pytest-benchmark
 pytest-benchmark==4.0.0
 pyyaml==6.0.1
     # via
     #   commitizen
     #   pre-commit
@@ -66,15 +66,13 @@
 scipy==1.12.0
 setuptools==69.2.0
     # via nodeenv
 termcolor==2.4.0
     # via commitizen
 tomlkit==0.12.4
     # via commitizen
-typing-extensions==4.10.0
-    # via mypy
 virtualenv==20.25.1
     # via pre-commit
 wcwidth==0.2.13
     # via prompt-toolkit
 zipp==3.18.1
     # via importlib-metadata
```

### Comparing `ReplayTables_andnp-6.3.1/src/storage/metadata_storage.rs` & `ReplayTables_andnp-7.0.0/src/storage/metadata_storage.rs`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 use serde::{Deserialize, Serialize};
 
 
 #[pyclass(module = "rust", frozen)]
 #[derive(Serialize, Deserialize, Clone, Copy)]
 pub struct Item {
     #[pyo3(get)]
-    pub eid: i64,
+    pub trans_id: i64,
     #[pyo3(get)]
-    pub idx: usize,
+    pub storage_idx: usize,
     #[pyo3(get)]
     pub xid: i64,
     #[pyo3(get)]
     pub n_xid: Option<i64>,
     #[pyo3(get)]
     pub sidx: i64,
     #[pyo3(get)]
@@ -22,30 +22,30 @@
 }
 
 #[pymethods]
 impl Item {
     #[staticmethod]
     pub fn default(null_idx: i64) -> Self {
         Item {
-            eid: null_idx,
-            idx: 0,
+            trans_id: null_idx,
+            storage_idx: 0,
             xid: 0,
             n_xid: None,
             sidx: 0,
             n_sidx: None,
         }
     }
 }
 
 #[pyclass(module = "rust")]
 pub struct Items {
     #[pyo3(get)]
-    pub idxs: Py<PyArray1<i64>>,
+    pub storage_idxs: Py<PyArray1<i64>>,
     #[pyo3(get)]
-    pub eids: Py<PyArray1<i64>>,
+    pub trans_ids: Py<PyArray1<i64>>,
     #[pyo3(get)]
     pub xids: Py<PyArray1<i64>>,
     #[pyo3(get)]
     pub n_xids: Py<PyArray1<i64>>,
     #[pyo3(get)]
     pub sidxs: Py<PyArray1<i64>>,
     #[pyo3(get)]
@@ -103,73 +103,73 @@
             .expect("Item not found for index")
     }
 
     pub fn get_items_by_idx(&mut self, idxs: PyReadonlyArray1<i64>) -> Items {
         let idxs = idxs.as_array();
         let size = idxs.len();
 
-        let mut eids = vec![0; size];
+        let mut trans_ids = vec![0; size];
         let mut xids = vec![0; size];
         let mut n_xids = vec![0; size];
         let mut sidxs = vec![0; size];
         let mut n_sidxs = vec![0; size];
 
 
         for i in 0..size {
             let idx = *idxs.get(i).expect("");
             let item = self._ids.get(idx as usize).expect("");
-            eids[i] = item.eid;
+            trans_ids[i] = item.trans_id;
             xids[i] = item.xid;
             sidxs[i] = item.sidx;
 
             n_xids[i] = item.n_xid.unwrap_or(self._null_idx);
             n_sidxs[i] = item.n_sidx.unwrap_or(-1);
         }
 
         Python::with_gil(|py| {
             Items {
-                idxs: idxs.to_pyarray_bound(py).into(),
-                eids: eids.to_pyarray_bound(py).into(),
+                storage_idxs: idxs.to_pyarray_bound(py).into(),
+                trans_ids: trans_ids.to_pyarray_bound(py).into(),
                 xids: xids.to_pyarray_bound(py).into(),
                 sidxs: sidxs.to_pyarray_bound(py).into(),
                 n_xids: n_xids.to_pyarray_bound(py).into(),
                 n_sidxs: n_sidxs.to_pyarray_bound(py).into(),
             }
         })
     }
 
     pub fn add_item(
         &mut self,
-        eid: i64,
+        trans_id: i64,
         idx: i64,
         xid: i64,
         n_xid: Option<i64>,
     ) -> (Item, Option<Item>) {
         // first check if there was already an item
         let item = &self._ids[idx as usize];
         let mut last_item = None;
-        if item.eid != self._null_idx {
-            self._ref.remove_transition(item.eid);
+        if item.trans_id != self._null_idx {
+            self._ref.remove_transition(item.trans_id);
             last_item = Some(item.clone());
         }
 
         let sidx = self._ref
-            .add_state(eid, xid)
+            .add_state(trans_id, xid)
             .expect("");
 
         let mut n_sidx = None;
         if n_xid.is_some() {
             n_sidx = self._ref
-                .add_state(eid, n_xid.expect(""))
+                .add_state(trans_id, n_xid.expect(""))
                 .ok();
         }
 
         let item = Item {
-            idx: idx as usize,
-            eid,
+            storage_idx: idx as usize,
+            trans_id,
             xid,
             sidx,
             n_xid,
             n_sidx,
         };
         self._ids[idx as usize] = item;
```

### Comparing `ReplayTables_andnp-6.3.1/src/utils/ref_count.rs` & `ReplayTables_andnp-7.0.0/src/utils/ref_count.rs`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/src/utils/sumtree.rs` & `ReplayTables_andnp-7.0.0/src/utils/sumtree.rs`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/tests/_utils/fake_data.py` & `ReplayTables_andnp-7.0.0/tests/_utils/fake_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from typing import cast, Any, Dict, Hashable, Sequence, Tuple
-from ReplayTables.interface import Batch, Timestep, LaggedTimestep, EID, XID
+from ReplayTables.interface import Batch, Timestep, LaggedTimestep, XID, TransId
 from ReplayTables.ingress.LagBuffer import LagBuffer
 
 _zero = np.zeros(8)
 def fake_timestep(
     x: np.ndarray | None = _zero,
     a: int = 0,
     r: float | None = 0.0,
@@ -24,40 +24,40 @@
 _zero_b = np.zeros((1, 8))
 def fake_batch(
     x: np.ndarray = _zero_b,
     a: np.ndarray = _zero_b,
     r: np.ndarray = _zero_b,
     xp: np.ndarray = _zero_b,
 ):
-    eids: Any = np.array([0], dtype=np.int64)
+    tids: Any = np.array([0], dtype=np.int64)
     return Batch(
         x=x,
         a=a,
         r=r,
         gamma=np.array([0.99]),
         terminal=np.array([False]),
-        eid=eids,
+        trans_id=tids,
         xp=xp
     )
 
 
 def fake_lagged_timestep(
-    eid: int,
+    trans_id: int,
     xid: int,
     n_xid: int,
     x: np.ndarray = _zero,
     a: int | float = 0,
     r: float = 0,
     gamma: float = 0.99,
     terminal: bool = False,
     extra: Dict = {},
     n_x: np.ndarray = _zero,
 ):
     return LaggedTimestep(
-        eid=cast(EID, eid),
+        trans_id=cast(TransId, trans_id),
         xid=cast(XID, xid),
         x=x,
         a=a,
         r=r,
         gamma=gamma,
         terminal=terminal,
         extra=extra,
@@ -80,15 +80,15 @@
         and l1.xid == l2.xid and l1.n_xid == l2.n_xid
 
 
 def batch_equal(b1: Batch, b2: Batch):
     return obs_equal(b1.x, b2.x) \
         and obs_equal(b1.xp, b2.xp) \
         and np.all(b1.a == b2.a) \
-        and np.all(b1.eid == b2.eid) \
+        and np.all(b1.trans_id == b2.trans_id) \
         and np.all(b1.r == b2.r) \
         and np.all(b1.gamma == b2.gamma) \
         and np.all(b1.terminal == b2.terminal)
 
 
 def lags_to_batch(lagged: Sequence[LaggedTimestep]) -> Batch:
     zero = np.zeros_like(lagged[0].x)
@@ -96,17 +96,17 @@
 
     for lag in lagged:
         if lag.n_x is None:
             xps.append(zero)
         else:
             xps.append(lag.n_x)
 
-    eids: Any = np.array([lag.eid for lag in lagged])
+    tids: Any = np.array([lag.trans_id for lag in lagged])
     return Batch(
-        eid=eids,
+        trans_id=tids,
         x=np.stack([d.x for d in lagged], axis=0),
         a=np.array([d.a for d in lagged]),
         r=np.array([d.r for d in lagged]),
         gamma=np.array([d.gamma for d in lagged]),
         terminal=np.array([d.terminal for d in lagged]),
         xp=np.stack(xps, axis=0),
     )
```

### Comparing `ReplayTables_andnp-6.3.1/tests/rust/test_RefCount.py` & `ReplayTables_andnp-7.0.0/tests/rust/test_RefCount.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/tests/sampling/test_PrioritizedSequenceSampler.py` & `ReplayTables_andnp-7.0.0/tests/sampling/test_PrioritizedSequenceSampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     dist.init()
 
     data = LaggedDataStream(lag=1)
     data.next()
     for _ in range(10):
         d = data.next_single()
 
-        idx = mapper.add_eid(d.eid)
+        idx = mapper.add_transition(d)
         storage.add(idx, d)
 
     tree = dist.tree
     dim = dist.dim
 
     assert tree.dim_total(dim) == 0.
```

### Comparing `ReplayTables_andnp-6.3.1/tests/storage/test_BasicStorage.py` & `ReplayTables_andnp-7.0.0/tests/storage/test_BasicStorage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import numpy as np
 from typing import cast, Any
 from ReplayTables.storage.BasicStorage import BasicStorage
-from ReplayTables.interface import LaggedTimestep, EID, XID
+from ReplayTables.interface import LaggedTimestep, XID, TransId
 
 def test_inferred_types1():
     storage = BasicStorage(10)
 
     x = np.zeros((32, 32), dtype=np.uint8)
     a = 1.0
 
     d = LaggedTimestep(
-        eid=cast(EID, 32),
+        trans_id=cast(TransId, 32),
         xid=cast(XID, 0),
         x=x,
         a=a,
         r=1.0,
         gamma=0.99,
         terminal=False,
         extra={},
@@ -32,15 +32,15 @@
 def test_inferred_types2():
     storage = BasicStorage(10)
 
     x = np.zeros(15, dtype=np.float32)
     a = 1
 
     d = LaggedTimestep(
-        eid=cast(EID, 32),
+        trans_id=cast(TransId, 32),
         xid=cast(XID, 0),
         x=x,
         a=a,
         r=1.0,
         gamma=0.99,
         terminal=False,
         extra={},
```

### Comparing `ReplayTables_andnp-6.3.1/tests/storage/test_Storage.py` & `ReplayTables_andnp-7.0.0/tests/storage/test_Storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 
 from collections import deque
 from typing import Any, Sequence, Type
 from ReplayTables.storage.BasicStorage import Storage, BasicStorage
 from ReplayTables.storage.CompressedStorage import CompressedStorage
 from ReplayTables.storage.NonArrayStorage import NonArrayStorage
-from ReplayTables.interface import LaggedTimestep, IDX, IDXs
+from ReplayTables.interface import LaggedTimestep, StorageIdx, StorageIdxs
 
 from tests._utils.fake_data import fake_lagged_timestep, LaggedDataStream, lagged_equal, batch_equal, lags_to_batch
 
 
 STORAGES = [
     BasicStorage,
     CompressedStorage,
@@ -23,54 +23,54 @@
 ]
 
 @pytest.mark.parametrize('Store', STORAGES)
 def test_add1(Store: Type[Storage]):
     storage = Store(10)
     storage.add(
         as_idx(0),
-        fake_lagged_timestep(eid=32, xid=32, n_xid=34),
+        fake_lagged_timestep(trans_id=32, xid=32, n_xid=34),
     )
 
     storage.add(
         as_idx(1),
-        fake_lagged_timestep(eid=34, xid=34, n_xid=36),
+        fake_lagged_timestep(trans_id=34, xid=34, n_xid=36),
     )
 
     assert len(storage) == 2
 
     for i in range(10):
         storage.add(
             as_idx(i),
-            fake_lagged_timestep(eid=36 + i, xid=i, n_xid=i),
+            fake_lagged_timestep(trans_id=36 + i, xid=i, n_xid=i),
         )
 
     assert len(storage) == 10
 
 
 @pytest.mark.parametrize('Store', STORAGES)
 def test_integration1(Store: Type[Storage]):
     storage = Store(10)
     data = LaggedDataStream(lag=1)
     past = deque(maxlen=5)
 
     def add_and_check(exp: LaggedTimestep, expected_len: int):
         past.append(exp)
         storage.add(
-            as_idx(exp.eid % 10),
+            as_idx(exp.trans_id % 10),
             exp,
         )
         assert len(storage) == expected_len
 
         got = storage.get_item(
-            as_idx(exp.eid % 10),
+            as_idx(exp.trans_id % 10),
         )
         assert lagged_equal(got, exp)
 
         for past_exp in past:
-            got = storage.get_item(as_idx(past_exp.eid % 10))
+            got = storage.get_item(as_idx(past_exp.trans_id % 10))
             assert lagged_equal(got, past_exp)
 
     # can maintain partial storage
     # ----------------------------
     exps = data.next()
     assert len(exps) == 0
     assert len(storage) == 0
@@ -125,61 +125,61 @@
     storage = Store(10)
     data = LaggedDataStream(lag=1)
     data.next()
 
     samples = []
     for _ in range(10):
         d = data.next_single()
-        storage.add(as_idx(d.eid % 10), d)
+        storage.add(as_idx(d.trans_id % 10), d)
         samples.append(d)
 
     assert len(storage) == 10
 
     got = storage.get(as_idxs(np.arange(10)))
     expected = lags_to_batch(samples)
     assert batch_equal(got, expected)
 
     # can handle soft termination
     # ---------------------------
     samples = []
     exps = data.next(soft_term=True)
     samples.append(exps[0])
-    storage.add(as_idx(exps[0].eid % 10), exps[0])
+    storage.add(as_idx(exps[0].trans_id % 10), exps[0])
 
     data.next()
 
     for _ in range(5):
         d = data.next_single()
         samples.append(d)
-        storage.add(as_idx(d.eid % 10), d)
+        storage.add(as_idx(d.trans_id % 10), d)
 
     expected = lags_to_batch(samples)
-    eids: Any = expected.eid
+    eids: Any = expected.trans_id
     got = storage.get(as_idxs(eids % 10))
 
     assert batch_equal(got, expected)
     assert np.all(got.xp[0] != 0)
     assert got.terminal[0]
 
     # can handle hard termination
     # ---------------------------
     samples = []
     exps = data.next(hard_term=True)
     samples.append(exps[0])
-    storage.add(as_idx(exps[0].eid % 10), exps[0])
+    storage.add(as_idx(exps[0].trans_id % 10), exps[0])
 
     data.next()
 
     for _ in range(5):
         d = data.next_single()
         samples.append(d)
-        storage.add(as_idx(d.eid % 10), d)
+        storage.add(as_idx(d.trans_id % 10), d)
 
     expected = lags_to_batch(samples)
-    eids: Any = expected.eid
+    eids: Any = expected.trans_id
     got = storage.get(as_idxs(eids % 10))
 
     assert batch_equal(got, expected)
     assert np.all(got.xp[0] == 0)
     assert got.terminal[0]
 
 # ------------------------------
@@ -190,62 +190,62 @@
 def test_small_data(benchmark, Store: Type[Storage]):
     benchmark.name = Store.__name__
     benchmark.group = 'storage | small data'
 
     def add_and_get(storage: Storage, timesteps, eids):
         for i in range(100):
             storage.add(
-                as_idx(timesteps[i].eid % 10_000),
+                as_idx(timesteps[i].trans_id % 10_000),
                 timesteps[i],
             )
 
         for i in range(100):
             storage.get(eids % 10_000)
 
     storage = Store(10_000)
     eids = np.arange(32, dtype=np.int64)
     data = [
-        fake_lagged_timestep(eid=i, xid=2 * i, n_xid=2 * i + 1, x=np.ones(10), n_x=np.ones(10))
+        fake_lagged_timestep(trans_id=i, xid=2 * i, n_xid=2 * i + 1, x=np.ones(10), n_x=np.ones(10))
         for i in range(100)
     ]
 
     benchmark(add_and_get, storage, data, eids)
 
 
 @pytest.mark.parametrize('Store', STORAGES)
 def test_big_data(benchmark, Store: Type[Storage]):
     benchmark.name = Store.__name__
     benchmark.group = 'storage | big data'
 
     def add_and_get(storage: Storage, timesteps, eids):
         for i in range(100):
             storage.add(
-                as_idx(timesteps[i].eid % 10_000),
+                as_idx(timesteps[i].trans_id % 10_000),
                 timesteps[i],
             )
 
         for i in range(100):
             storage.get(eids % 10_000)
 
     storage = Store(10_000)
     eids = np.arange(32, dtype=np.int64)
     x = np.ones((64, 64, 3), dtype=np.uint8)
     data = [
-        fake_lagged_timestep(eid=i, xid=2 * i, n_xid=2 * i + 1, x=x, n_x=x)
+        fake_lagged_timestep(trans_id=i, xid=2 * i, n_xid=2 * i + 1, x=x, n_x=x)
         for i in range(100)
     ]
 
     benchmark(add_and_get, storage, data, eids)
 
 
 # --------------------
 # -- Internal Utils --
 # --------------------
 
-def as_idx(i: int) -> IDX:
+def as_idx(i: int) -> StorageIdx:
     idx: Any = i
     return idx
 
 
-def as_idxs(i: Sequence[int] | np.ndarray) -> IDXs:
+def as_idxs(i: Sequence[int] | np.ndarray) -> StorageIdxs:
     idxs: Any = np.asarray(i, dtype=np.int64)
     return idxs
```

### Comparing `ReplayTables_andnp-6.3.1/tests/test_LagBuffer.py` & `ReplayTables_andnp-7.0.0/tests/test_LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/tests/test_PER.py` & `ReplayTables_andnp-7.0.0/tests/test_PER.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pickle
 import numpy as np
 from typing import cast, Any
 
-from ReplayTables.interface import EID, Timestep
+from ReplayTables.interface import Timestep, TransId
 from ReplayTables.PER import PrioritizedReplay, PERConfig
 
 from tests._utils.fake_data import fake_timestep
 
 class TestPER:
     def test_simple_buffer(self):
         rng = np.random.default_rng(0)
@@ -21,17 +21,17 @@
         assert buffer.size() == 0
 
         d = fake_timestep(a=2)
         buffer.add_step(d)
         assert buffer.size() == 1
 
         samples = buffer.sample(10)
-        weights = buffer.isr_weights(samples.eid)
+        weights = buffer.isr_weights(samples.trans_id)
         assert np.all(samples.a == 1)
-        assert np.all(samples.eid == 0)
+        assert np.all(samples.trans_id == 0)
         assert np.all(weights == 0.2)
 
         # should be able to add a few more points
         for i in range(4):
             x = i + 3
             buffer.add_step(fake_timestep(a=x))
 
@@ -132,15 +132,15 @@
         for i in range(5):
             buffer.add_step(fake_timestep(a=i, r=2 * i))
 
         buffer.add_step(fake_timestep())
         batch = buffer.sample(512)
         assert np.unique(batch.a).shape == (5,)
 
-        buffer.delete_sample(cast(EID, 2))
+        buffer.delete_sample(cast(TransId, 2))
         batch = buffer.sample(512)
         assert np.unique(batch.a).shape == (4,)
         assert 2 not in batch.a
 
 # ----------------
 # -- Benchmarks --
 # ----------------
```

### Comparing `ReplayTables_andnp-6.3.1/tests/test_PrototypeBuffer.py` & `ReplayTables_andnp-7.0.0/tests/test_PrototypeBuffer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Any
 import numpy as np
 
 from ReplayTables.PrototypeBuffer import RandomEgressBuffer
 
 from tests._utils.fake_data import fake_timestep
 
 
@@ -11,75 +12,63 @@
         lag = 1
         seed = 42
 
         sampler_rng = np.random.default_rng(seed)
         indexer_rng = np.random.default_rng(seed)
 
         buffer = RandomEgressBuffer(max_size, lag, sampler_rng)
-        buffer._idx_mapper._rng = indexer_rng
 
         assert buffer.size() == 0
 
         # should be able to simply add and sample a single data point
         d = fake_timestep(a=1)
         buffer.add_step(d)
         assert buffer.size() == 0
 
         d = fake_timestep(a=2)
         buffer.add_step(d)
         assert buffer.size() == 1
 
         samples = buffer.sample(10)
-        weights = buffer.isr_weights(samples.eid)
+        weights = buffer.isr_weights(samples.trans_id)
         assert np.all(samples.a == 1)
-        assert np.all(samples.eid == 0)
+        assert np.all(samples.trans_id == 0)
         assert np.all(weights == 1.0)
 
-
         # should be able to add a few more points
         for i in range(4):
             x = i + 3
             buffer.add_step(fake_timestep(a=x))
 
         assert buffer.size() == 5
 
-
         # should remove random elements when over max size
         control_as = np.array([1, 2, 3, 4, 5])
         for i in range(100):
             x = i + 7
             buffer.add_step(fake_timestep(a=x))
             swap_idx = indexer_rng.integers(0, 5)
             control_as[swap_idx] = x - 1
 
-        assert np.all(buffer._storage.get(np.array([0, 1, 2 , 3, 4])).a == control_as)
-
+        idxs: Any = np.array([0, 1, 2, 3, 4])
+        assert np.all(buffer._storage.get(idxs).a == control_as)
 
     def test_sampling(self):
         max_size = 5
         lag = 1
         seed = 0
 
         sampler_rng = np.random.default_rng(seed)
-        indexer_rng = np.random.default_rng(seed)
 
         buffer = RandomEgressBuffer(max_size, lag, sampler_rng)
-        buffer._idx_mapper._rng = indexer_rng
-
 
         # should be able to sample all data points
         for i in range(6):
             x = i + 1
             buffer.add_step(fake_timestep(a=x))
 
         assert buffer.size() == 5
 
         samples = buffer.sample(1000)
         unique = np.unique(samples.a)
         unique.sort()
         assert np.all(unique == np.array([1, 2, 3, 4, 5]))
-
-
-
-
-
-
```

### Comparing `ReplayTables_andnp-6.3.1/tests/test_ReplayBuffer.py` & `ReplayTables_andnp-7.0.0/tests/test_ReplayBuffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
         assert buffer.size() == 0
 
         d = fake_timestep(a=2)
         buffer.add_step(d)
         assert buffer.size() == 1
 
         samples = buffer.sample(10)
-        weights = buffer.isr_weights(samples.eid)
+        weights = buffer.isr_weights(samples.trans_id)
         assert np.all(samples.a == 1)
-        assert np.all(samples.eid == 0)
+        assert np.all(samples.trans_id == 0)
         assert np.all(weights == 1)
 
         # should be able to add a few more points
         for i in range(4):
             x = i + 3
             d = fake_timestep(a=x)
             buffer.add_step(d)
```

### Comparing `ReplayTables_andnp-6.3.1/tests/test_fuzz.py` & `ReplayTables_andnp-7.0.0/tests/test_fuzz.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 from typing import Any
-from ReplayTables.interface import Batch, IDXs, Item, LaggedTimestep, Timestep
+from ReplayTables.interface import Batch, Item, LaggedTimestep, StorageIdxs, Timestep
 from ReplayTables.ReplayBuffer import ReplayBufferInterface
 from ReplayTables.ingress.LagBuffer import LagBuffer
 
 from tests._utils.fake_data import batch_equal
 
 # ---------------
 # -- Baselines --
@@ -20,23 +20,23 @@
     def add(self, e):
         self.storage[self._i] = Batch(
             x=e.x,
             a=e.a,
             r=e.r,
             gamma=e.gamma,
             terminal=e.terminal,
-            eid=e.eid,
+            trans_id=e.trans_id,
             xp=e.n_x,
         )
         self._i = (self._i + 1) % self._max
 
     def size(self):
         return len(self.storage)
 
-    def get(self, idxs: IDXs) -> Batch:
+    def get(self, idxs: StorageIdxs) -> Batch:
         x, a, r, g, t, e, xp = zip(*[self.storage[idx] for idx in idxs])
 
         xps = []
         for _xp in xp:
             if _xp is None:
                 xps.append(np.zeros(8))
             else:
@@ -45,21 +45,21 @@
         eid: Any = np.array(e)
         return Batch(
             x=np.array(x),
             a=np.array(a),
             r=np.array(r),
             gamma=np.array(g),
             terminal=np.array(t),
-            eid=eid,
+            trans_id=eid,
             xp=np.array(xps),
         )
 
 class ReplayBuffer(ReplayBufferInterface):
     def _on_add(self, item: Item, transition: LaggedTimestep):
-        self._sampler.replace(item.idx, transition)
+        self._sampler.replace(item.storage_idx, transition)
 
 # -----------
 # -- Tests --
 # -----------
 
 def test_1():
     rng = np.random.default_rng(0)
```

### Comparing `ReplayTables_andnp-6.3.1/tests/test_integration.py` & `ReplayTables_andnp-7.0.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/tests/utils/test_MinMaxHeap.py` & `ReplayTables_andnp-7.0.0/tests/utils/test_MinMaxHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/tests/utils/test_SumTree.py` & `ReplayTables_andnp-7.0.0/tests/utils/test_SumTree.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.3.1/typings/ReplayTables/rust/__init__.pyi` & `ReplayTables_andnp-7.0.0/typings/ReplayTables/rust/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import numpy as np
 from typing import Tuple
-from ReplayTables.interface import EID, IDX, SIDX, XID, IDXs, Item, Items
+from ReplayTables.interface import SIDX, XID, Item, Items, StorageIdx, StorageIdxs, TransId
 
 class RefCount:
-    def add_state(self, eid: EID, xid: XID) -> SIDX: ...
+    def add_state(self, tid: TransId, xid: XID) -> SIDX: ...
     def load_state(self, xid: XID) -> int: ...
     def has_xid(self, xid: XID) -> bool: ...
-    def remove_transition(self, eid: EID) -> None: ...
+    def remove_transition(self, tid: TransId) -> None: ...
 
 
 class MetadataStorage:
     def __init__(self, *args): ...
-    def get_item_by_idx(self, idx: IDX) -> Item: ...
-    def get_items_by_idx(self, idxs: IDXs) -> Items: ...
-    def add_item(self, eid: EID, idx: IDX, xid: XID, n_xid: XID | None) -> Tuple[Item, Item | None]: ...
+    def get_item_by_idx(self, idx: StorageIdx) -> Item: ...
+    def get_items_by_idx(self, idxs: StorageIdxs) -> Items: ...
+    def add_item(self, tid: TransId, idx: StorageIdx, xid: XID, n_xid: XID | None) -> Tuple[Item, Item | None]: ...
     def has_xid(self, xid: XID) -> bool: ...
     def __getstate__(self): ...
     def __setstate__(self, state): ...
 
 class SumTree:
     size: int
     dims: int
```

### Comparing `ReplayTables_andnp-6.3.1/Cargo.lock` & `ReplayTables_andnp-7.0.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -333,26 +333,26 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `ReplayTables_andnp-6.3.1/pyproject.toml` & `ReplayTables_andnp-7.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 [tool]
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "6.3.1"
+version = "7.0.0"
 tag_format = "$version"
 version_files = ["pyproject.toml"]
 
-[tool.mypy]
-mypy_path = "typings"
-
 [tool.maturin]
 features = ["pyo3/extension-module"]
 module-name = "ReplayTables.rust"
 
 [tool.ruff.lint]
-ignore = ['E701']
+select = ['F', 'E', 'W']
+ignore = ['E501', 'E701']
+
+[tool.pyright]
+include = ["ReplayTables", "tests"]
+stubPath = "./typings"
+venvPath = "."
+venv = ".venv"
+typeCheckingMode = "standard"
+useLibraryCodeForTypes = true
 
 [project]
 name = "ReplayTables-andnp"
-version = "6.3.1"
+version = "7.0.0"
 description = "A simple replay buffer implementation in python for sampling n-step trajectories"
 authors = [
     {name = "Andy Patterson", email = "andnpatterson@gmail.com"},
 ]
 dependencies = [
     "numba~=0.57",
     "numpy~=1.23",
@@ -37,16 +43,16 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pip",
-    "mypy",
     "ruff",
+    "pyright",
     "commitizen",
     "pre-commit",
     "pytest>=7.3,<9.0",
     "pytest-benchmark~=4.0",
     "maturin>=1.4,<1.6",
 ]
```

### Comparing `ReplayTables_andnp-6.3.1/PKG-INFO` & `ReplayTables_andnp-7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.3
 Name: ReplayTables-andnp
-Version: 6.3.1
+Version: 7.0.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numba ~=0.57
 Requires-Dist: numpy ~=1.23
 Requires-Dist: scipy ~=1.9
 Requires-Dist: lz4 ~=4.3.2
 Requires-Dist: pip ; extra == 'dev'
-Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: ruff ; extra == 'dev'
+Requires-Dist: pyright ; extra == 'dev'
 Requires-Dist: commitizen ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
 Requires-Dist: pytest >=7.3, <9.0 ; extra == 'dev'
 Requires-Dist: pytest-benchmark ~=4.0 ; extra == 'dev'
 Requires-Dist: maturin >=1.4, <1.6 ; extra == 'dev'
 Provides-Extra: dev
 Summary: A simple replay buffer implementation in python for sampling n-step trajectories
```

