# Comparing `tmp/tenacity-8.2.3.tar.gz` & `tmp/tenacity-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenacity-8.2.3.tar", last modified: Mon Aug 14 13:22:48 2023, max compression
+gzip compressed data, was "tenacity-8.3.0.tar", last modified: Tue May  7 08:48:14 2024, max compression
```

## Comparing `tenacity-8.2.3.tar` & `tenacity-8.3.0.tar`

### file list

```diff
@@ -1,79 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-14 13:22:48.214220 tenacity-8.2.3/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-08-14 13:22:23.000000 tenacity-8.2.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-14 13:22:48.202221 tenacity-8.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-14 13:22:48.202221 tenacity-8.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-08-14 13:22:23.000000 tenacity-8.2.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-08-14 13:22:23.000000 tenacity-8.2.3/.github/workflows/deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-08-14 13:22:23.000000 tenacity-8.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1712 2023-08-14 13:22:23.000000 tenacity-8.2.3/.mergify.yml
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-08-14 13:22:23.000000 tenacity-8.2.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-08-14 13:22:23.000000 tenacity-8.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-08-14 13:22:48.214220 tenacity-8.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17335 2023-08-14 13:22:23.000000 tenacity-8.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-14 13:22:48.202221 tenacity-8.2.3/doc/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-14 13:22:48.206220 tenacity-8.2.3/doc/source/
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-08-14 13:22:23.000000 tenacity-8.2.3/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-08-14 13:22:23.000000 tenacity-8.2.3/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-08-14 13:22:23.000000 tenacity-8.2.3/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)    17335 2023-08-14 13:22:23.000000 tenacity-8.2.3/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-08-14 13:22:23.000000 tenacity-8.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-14 13:22:48.202221 tenacity-8.2.3/releasenotes/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-14 13:22:48.210220 tenacity-8.2.3/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/Fix-tests-for-typeguard-3.x-6eebfea546b6207e.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/Use--for-formatting-and-validate-using-black-39ec9d57d4691778.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/add-reno-d1ab5710f272650a.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/add-retry_except_exception_type-31b31da1924d55f4.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/add_omitted_modules_to_import_all-2ab282f20a2c22f7.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/add_retry_if_exception_cause_type-d16b918ace4ae0ad.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/added_a_link_to_documentation-eefaf8f074b539f8.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/after_log-50f4d73b24ce9203.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/allow-mocking-of-nap-sleep-6679c50e702446f1.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/annotate_code-197b93130df14042.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/before_sleep_log-improvements-d8149274dfb37d7c.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/clarify-reraise-option-6829667eacf4f599.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/do_not_package_tests-fe5ac61940b0a5ed.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/drop-deprecated-python-versions-69a05cb2e0f1034c.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/drop_deprecated-7ea90b212509b082.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/export-convenience-symbols-981d9611c8b754f3.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/fix-async-loop-with-result-f68e913ccb425aca.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/fix-wait-typing-b26eecdb6cc0a1de.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/fix_async-52b6594c8e75c4bc.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/make-logger-more-compatible-5da1ddf1bab77047.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/no-async-iter-6132a42e52348a75.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/pr320-py3-only-wheel-tag.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/py36_plus-c425fb3aa17c6682.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/remove-py36-876c0416cf279d15.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/retrycallstate-repr-94947f7b00ee15e1.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/sphinx_define_error-642c9cd5c165d39a.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/support-timedelta-wait-unit-type-5ba1e9fc0fe45523.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/timedelta-for-stop-ef6bf71b88ce9988.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-08-14 13:22:23.000000 tenacity-8.2.3/releasenotes/notes/wait_exponential_jitter-6ffc81dddcbaa6d3.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-08-14 13:22:23.000000 tenacity-8.2.3/reno.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1109 2023-08-14 13:22:48.214220 tenacity-8.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-08-14 13:22:23.000000 tenacity-8.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-14 13:22:48.210220 tenacity-8.2.3/tenacity/
--rw-r--r--   0 runner    (1001) docker     (122)    20214 2023-08-14 13:22:23.000000 tenacity-8.2.3/tenacity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3491 2023-08-14 13:22:23.000000 tenacity-8.2.3/tenacity/_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-08-14 13:22:23.000000 tenacity-8.2.3/tenacity/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-08-14 13:22:23.000000 tenacity-8.2.3/tenacity/after.py
--rw-r--r--   0 runner    (1001) docker     (122)     1538 2023-08-14 13:22:23.000000 tenacity-8.2.3/tenacity/before.py
--rw-r--r--   0 runner    (1001) docker     (122)     2348 2023-08-14 13:22:23.000000 tenacity-8.2.3/tenacity/before_sleep.py
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-08-14 13:22:23.000000 tenacity-8.2.3/tenacity/nap.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-14 13:22:23.000000 tenacity-8.2.3/tenacity/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     8734 2023-08-14 13:22:23.000000 tenacity-8.2.3/tenacity/retry.py
--rw-r--r--   0 runner    (1001) docker     (122)     3062 2023-08-14 13:22:23.000000 tenacity-8.2.3/tenacity/stop.py
--rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-08-14 13:22:23.000000 tenacity-8.2.3/tenacity/tornadoweb.py
--rw-r--r--   0 runner    (1001) docker     (122)     8000 2023-08-14 13:22:23.000000 tenacity-8.2.3/tenacity/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-14 13:22:48.210220 tenacity-8.2.3/tenacity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-08-14 13:22:48.000000 tenacity-8.2.3/tenacity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2603 2023-08-14 13:22:48.000000 tenacity-8.2.3/tenacity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-14 13:22:48.000000 tenacity-8.2.3/tenacity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-08-14 13:22:48.000000 tenacity-8.2.3/tenacity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-08-14 13:22:48.000000 tenacity-8.2.3/tenacity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-14 13:22:48.214220 tenacity-8.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-14 13:22:23.000000 tenacity-8.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2217 2023-08-14 13:22:23.000000 tenacity-8.2.3/tests/test_after.py
--rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-08-14 13:22:23.000000 tenacity-8.2.3/tests/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (122)    55976 2023-08-14 13:22:23.000000 tenacity-8.2.3/tests/test_tenacity.py
--rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-08-14 13:22:23.000000 tenacity-8.2.3/tests/test_tornado.py
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-08-14 13:22:23.000000 tenacity-8.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:13.999645 tenacity-8.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-07 08:48:00.000000 tenacity-8.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:13.991645 tenacity-8.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-07 08:48:00.000000 tenacity-8.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:13.991645 tenacity-8.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-07 08:48:00.000000 tenacity-8.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-07 08:48:00.000000 tenacity-8.3.0/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-07 08:48:00.000000 tenacity-8.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-07 08:48:00.000000 tenacity-8.3.0/.mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 08:48:00.000000 tenacity-8.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 08:48:00.000000 tenacity-8.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-07 08:48:13.999645 tenacity-8.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-07 08:48:00.000000 tenacity-8.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:13.987645 tenacity-8.3.0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:13.991645 tenacity-8.3.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-07 08:48:00.000000 tenacity-8.3.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 08:48:00.000000 tenacity-8.3.0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-07 08:48:00.000000 tenacity-8.3.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-07 08:48:00.000000 tenacity-8.3.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-07 08:48:00.000000 tenacity-8.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:13.987645 tenacity-8.3.0/releasenotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:13.995645 tenacity-8.3.0/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/Fix-tests-for-typeguard-3.x-6eebfea546b6207e.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/Use--for-formatting-and-validate-using-black-39ec9d57d4691778.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/add-reno-d1ab5710f272650a.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/add-retry_except_exception_type-31b31da1924d55f4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/add-stop-before-delay-a775f88ac872c923.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/add-test-extra-55e869261b03e56d.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/add_omitted_modules_to_import_all-2ab282f20a2c22f7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/add_retry_if_exception_cause_type-d16b918ace4ae0ad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/added_a_link_to_documentation-eefaf8f074b539f8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/after_log-50f4d73b24ce9203.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/allow-mocking-of-nap-sleep-6679c50e702446f1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/annotate_code-197b93130df14042.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/before_sleep_log-improvements-d8149274dfb37d7c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/clarify-reraise-option-6829667eacf4f599.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/dependabot-for-github-actions-4d2464f3c0928463.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/do_not_package_tests-fe5ac61940b0a5ed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/drop-deprecated-python-versions-69a05cb2e0f1034c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/drop_deprecated-7ea90b212509b082.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/export-convenience-symbols-981d9611c8b754f3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/fix-async-loop-with-result-f68e913ccb425aca.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/fix-wait-typing-b26eecdb6cc0a1de.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/fix_async-52b6594c8e75c4bc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/make-logger-more-compatible-5da1ddf1bab77047.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/no-async-iter-6132a42e52348a75.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/pr320-py3-only-wheel-tag.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/py36_plus-c425fb3aa17c6682.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/remove-py36-876c0416cf279d15.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/retrycallstate-repr-94947f7b00ee15e1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/some-slug-for-preserve-defaults-86682846dfa18005.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/sphinx_define_error-642c9cd5c165d39a.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/support-timedelta-wait-unit-type-5ba1e9fc0fe45523.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/timedelta-for-stop-ef6bf71b88ce9988.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-07 08:48:00.000000 tenacity-8.3.0/releasenotes/notes/wait_exponential_jitter-6ffc81dddcbaa6d3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 08:48:00.000000 tenacity-8.3.0/reno.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-07 08:48:13.999645 tenacity-8.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-07 08:48:00.000000 tenacity-8.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:13.999645 tenacity-8.3.0/tenacity/
+-rw-r--r--   0 runner    (1001) docker     (127)    23415 2024-05-07 08:48:00.000000 tenacity-8.3.0/tenacity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-07 08:48:00.000000 tenacity-8.3.0/tenacity/_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-07 08:48:00.000000 tenacity-8.3.0/tenacity/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-07 08:48:00.000000 tenacity-8.3.0/tenacity/after.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-07 08:48:00.000000 tenacity-8.3.0/tenacity/before.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-07 08:48:00.000000 tenacity-8.3.0/tenacity/before_sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-07 08:48:00.000000 tenacity-8.3.0/tenacity/nap.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:00.000000 tenacity-8.3.0/tenacity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-07 08:48:00.000000 tenacity-8.3.0/tenacity/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-07 08:48:00.000000 tenacity-8.3.0/tenacity/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-07 08:48:00.000000 tenacity-8.3.0/tenacity/tornadoweb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-05-07 08:48:00.000000 tenacity-8.3.0/tenacity/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:13.999645 tenacity-8.3.0/tenacity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-07 08:48:13.000000 tenacity-8.3.0/tenacity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-07 08:48:13.000000 tenacity-8.3.0/tenacity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:48:13.000000 tenacity-8.3.0/tenacity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 08:48:13.000000 tenacity-8.3.0/tenacity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 08:48:13.000000 tenacity-8.3.0/tenacity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:13.999645 tenacity-8.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 08:48:00.000000 tenacity-8.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-07 08:48:00.000000 tenacity-8.3.0/tests/test_after.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-07 08:48:00.000000 tenacity-8.3.0/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58948 2024-05-07 08:48:00.000000 tenacity-8.3.0/tests/test_tenacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-07 08:48:00.000000 tenacity-8.3.0/tests/test_tornado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-07 08:48:00.000000 tenacity-8.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-07 08:48:00.000000 tenacity-8.3.0/tox.ini
```

### Comparing `tenacity-8.2.3/.github/workflows/ci.yaml` & `tenacity-8.3.0/.github/workflows/ci.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -14,38 +14,37 @@
 jobs:
   test:
     timeout-minutes: 20
     runs-on: ubuntu-20.04
     strategy:
       matrix:
         include:
-          - python: "3.7"
-            tox: py37
           - python: "3.8"
             tox: py38
           - python: "3.9"
             tox: py39
           - python: "3.10"
             tox: py310
           - python: "3.11"
             tox: py311
-          - python: "3.11"
+          - python: "3.12"
+            tox: py312
+          - python: "3.12"
             tox: pep8
           - python: "3.11"
-            tox: black-ci
-          - python: "3.11"
             tox: mypy
     steps:
       - name: Checkout 🛎️
-        uses: actions/checkout@v3.3.0
+        uses: actions/checkout@v4.1.1
         with:
           fetch-depth: 0
 
       - name: Setup Python 🔧
-        uses: actions/setup-python@v4.5.0
+        uses: actions/setup-python@v5.0.0
         with:
-          python-version: ${{ matrix.python }}
+          python-version: ${{ matrix.python }}
+          allow-prereleases: true
 
       - name: Build 🔧 & Test 🔍
         run: |
           pip install tox
           tox -e ${{ matrix.tox }}
```

### Comparing `tenacity-8.2.3/LICENSE` & `tenacity-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tenacity-8.2.3/PKG-INFO` & `tenacity-8.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: tenacity
-Version: 8.2.3
+Version: 8.3.0
 Summary: Retry code until it succeeds
 Home-page: https://github.com/jd/tenacity
 Author: Julien Danjou
 Author-email: julien@danjou.info
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: doc
+Provides-Extra: test
 License-File: LICENSE
 
 Tenacity is a general-purpose retrying library to simplify the task of adding retry behavior to just about anything.
```

### Comparing `tenacity-8.2.3/README.rst` & `tenacity-8.3.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -120,14 +120,24 @@
 .. testcode::
 
     @retry(stop=stop_after_delay(10))
     def stop_after_10_s():
         print("Stopping after 10 seconds")
         raise Exception
 
+If you're on a tight deadline, and exceeding your delay time isn't ok, 
+then you can give up on retries one attempt before you would exceed the delay. 
+
+.. testcode::
+
+    @retry(stop=stop_before_delay(10))
+    def stop_before_10_s():
+        print("Stopping 1 attempt before 10 seconds")
+        raise Exception
+
 You can combine several stop conditions by using the `|` operator:
 
 .. testcode::
 
     @retry(stop=(stop_after_delay(10) | stop_after_attempt(5)))
     def stop_after_10_s_or_5_retries():
         print("Stopping after 10 seconds or 5 retries")
@@ -398,86 +408,50 @@
            retry=retry_if_result(is_false))
     def eventually_return_false():
         return False
 
 RetryCallState
 ~~~~~~~~~~~~~~
 
-``retry_state`` argument is an object of `RetryCallState` class:
-
-.. autoclass:: tenacity.RetryCallState
-
-   Constant attributes:
-
-   .. autoattribute:: start_time(float)
-      :annotation:
-
-   .. autoattribute:: retry_object(BaseRetrying)
-      :annotation:
-
-   .. autoattribute:: fn(callable)
-      :annotation:
-
-   .. autoattribute:: args(tuple)
-      :annotation:
-
-   .. autoattribute:: kwargs(dict)
-      :annotation:
-
-   Variable attributes:
-
-   .. autoattribute:: attempt_number(int)
-      :annotation:
-
-   .. autoattribute:: outcome(tenacity.Future or None)
-      :annotation:
-
-   .. autoattribute:: outcome_timestamp(float or None)
-      :annotation:
-
-   .. autoattribute:: idle_for(float)
-      :annotation:
-
-   .. autoattribute:: next_action(tenacity.RetryAction or None)
-      :annotation:
+``retry_state`` argument is an object of :class:`~tenacity.RetryCallState` class.
 
 Other Custom Callbacks
 ~~~~~~~~~~~~~~~~~~~~~~
 
 It's also possible to define custom callbacks for other keyword arguments.
 
 .. function:: my_stop(retry_state)
 
-   :param RetryState retry_state: info about current retry invocation
+   :param RetryCallState retry_state: info about current retry invocation
    :return: whether or not retrying should stop
    :rtype: bool
 
 .. function:: my_wait(retry_state)
 
-   :param RetryState retry_state: info about current retry invocation
+   :param RetryCallState retry_state: info about current retry invocation
    :return: number of seconds to wait before next retry
    :rtype: float
 
 .. function:: my_retry(retry_state)
 
-   :param RetryState retry_state: info about current retry invocation
+   :param RetryCallState retry_state: info about current retry invocation
    :return: whether or not retrying should continue
    :rtype: bool
 
 .. function:: my_before(retry_state)
 
-   :param RetryState retry_state: info about current retry invocation
+   :param RetryCallState retry_state: info about current retry invocation
 
 .. function:: my_after(retry_state)
 
-   :param RetryState retry_state: info about current retry invocation
+   :param RetryCallState retry_state: info about current retry invocation
 
 .. function:: my_before_sleep(retry_state)
 
-   :param RetryState retry_state: info about current retry invocation
+   :param RetryCallState retry_state: info about current retry invocation
 
 Here's an example with a custom ``before_sleep`` function:
 
 .. testcode::
 
     import logging
```

### Comparing `tenacity-8.2.3/doc/source/api.rst` & `tenacity-8.3.0/doc/source/api.rst`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 .. autoclass:: tenacity.AsyncRetrying
    :members:
 
 .. autoclass:: tenacity.tornadoweb.TornadoRetrying
    :members:
 
+.. autoclass:: tenacity.RetryCallState
+   :members:
+
 After Functions
 ---------------
 
 Those functions can be used as the `after` keyword argument of
 :py:func:`tenacity.retry`.
 
 .. automodule:: tenacity.after
```

### Comparing `tenacity-8.2.3/doc/source/conf.py` & `tenacity-8.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `tenacity-8.2.3/doc/source/index.rst` & `tenacity-8.3.0/doc/source/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -120,14 +120,24 @@
 .. testcode::
 
     @retry(stop=stop_after_delay(10))
     def stop_after_10_s():
         print("Stopping after 10 seconds")
         raise Exception
 
+If you're on a tight deadline, and exceeding your delay time isn't ok, 
+then you can give up on retries one attempt before you would exceed the delay. 
+
+.. testcode::
+
+    @retry(stop=stop_before_delay(10))
+    def stop_before_10_s():
+        print("Stopping 1 attempt before 10 seconds")
+        raise Exception
+
 You can combine several stop conditions by using the `|` operator:
 
 .. testcode::
 
     @retry(stop=(stop_after_delay(10) | stop_after_attempt(5)))
     def stop_after_10_s_or_5_retries():
         print("Stopping after 10 seconds or 5 retries")
@@ -398,86 +408,50 @@
            retry=retry_if_result(is_false))
     def eventually_return_false():
         return False
 
 RetryCallState
 ~~~~~~~~~~~~~~
 
-``retry_state`` argument is an object of `RetryCallState` class:
-
-.. autoclass:: tenacity.RetryCallState
-
-   Constant attributes:
-
-   .. autoattribute:: start_time(float)
-      :annotation:
-
-   .. autoattribute:: retry_object(BaseRetrying)
-      :annotation:
-
-   .. autoattribute:: fn(callable)
-      :annotation:
-
-   .. autoattribute:: args(tuple)
-      :annotation:
-
-   .. autoattribute:: kwargs(dict)
-      :annotation:
-
-   Variable attributes:
-
-   .. autoattribute:: attempt_number(int)
-      :annotation:
-
-   .. autoattribute:: outcome(tenacity.Future or None)
-      :annotation:
-
-   .. autoattribute:: outcome_timestamp(float or None)
-      :annotation:
-
-   .. autoattribute:: idle_for(float)
-      :annotation:
-
-   .. autoattribute:: next_action(tenacity.RetryAction or None)
-      :annotation:
+``retry_state`` argument is an object of :class:`~tenacity.RetryCallState` class.
 
 Other Custom Callbacks
 ~~~~~~~~~~~~~~~~~~~~~~
 
 It's also possible to define custom callbacks for other keyword arguments.
 
 .. function:: my_stop(retry_state)
 
-   :param RetryState retry_state: info about current retry invocation
+   :param RetryCallState retry_state: info about current retry invocation
    :return: whether or not retrying should stop
    :rtype: bool
 
 .. function:: my_wait(retry_state)
 
-   :param RetryState retry_state: info about current retry invocation
+   :param RetryCallState retry_state: info about current retry invocation
    :return: number of seconds to wait before next retry
    :rtype: float
 
 .. function:: my_retry(retry_state)
 
-   :param RetryState retry_state: info about current retry invocation
+   :param RetryCallState retry_state: info about current retry invocation
    :return: whether or not retrying should continue
    :rtype: bool
 
 .. function:: my_before(retry_state)
 
-   :param RetryState retry_state: info about current retry invocation
+   :param RetryCallState retry_state: info about current retry invocation
 
 .. function:: my_after(retry_state)
 
-   :param RetryState retry_state: info about current retry invocation
+   :param RetryCallState retry_state: info about current retry invocation
 
 .. function:: my_before_sleep(retry_state)
 
-   :param RetryState retry_state: info about current retry invocation
+   :param RetryCallState retry_state: info about current retry invocation
 
 Here's an example with a custom ``before_sleep`` function:
 
 .. testcode::
 
     import logging
```

### Comparing `tenacity-8.2.3/setup.cfg` & `tenacity-8.3.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -9,37 +9,40 @@
 home_page = https://github.com/jd/tenacity
 classifier = 
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Utilities
 
 [options]
 install_requires = 
-python_requires = >=3.7
+python_requires = >=3.8
 packages = tenacity
 
 [options.packages.find]
 exclude = tests
 
 [options.package_data]
 tenacity = py.typed
 
 [options.extras_require]
 doc = 
 	reno
 	sphinx
+test = 
+	pytest
 	tornado>=4.5
+	typeguard
 
 [tool:pytest]
 filterwarnings = 
 	once::DeprecationWarning
 
 [egg_info]
 tag_build =
```

### Comparing `tenacity-8.2.3/setup.py` & `tenacity-8.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `tenacity-8.2.3/tenacity/__init__.py` & `tenacity-8.3.0/tenacity/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-
+import dataclasses
 import functools
 import sys
 import threading
 import time
 import typing as t
 import warnings
 from abc import ABC, abstractmethod
@@ -46,14 +45,15 @@
 # Import all nap strategies for easier usage.
 from .nap import sleep  # noqa
 from .nap import sleep_using_event  # noqa
 
 # Import all built-in stop strategies for easier usage.
 from .stop import stop_after_attempt  # noqa
 from .stop import stop_after_delay  # noqa
+from .stop import stop_before_delay  # noqa
 from .stop import stop_all  # noqa
 from .stop import stop_any  # noqa
 from .stop import stop_never  # noqa
 from .stop import stop_when_event_set  # noqa
 
 # Import all built-in wait strategies for easier usage.
 from .wait import wait_chain  # noqa
@@ -92,14 +92,37 @@
     from .wait import WaitBaseT
 
 
 WrappedFnReturnT = t.TypeVar("WrappedFnReturnT")
 WrappedFn = t.TypeVar("WrappedFn", bound=t.Callable[..., t.Any])
 
 
+dataclass_kwargs = {}
+if sys.version_info >= (3, 10):
+    dataclass_kwargs.update({"slots": True})
+
+
+@dataclasses.dataclass(**dataclass_kwargs)
+class IterState:
+    actions: t.List[t.Callable[["RetryCallState"], t.Any]] = dataclasses.field(
+        default_factory=list
+    )
+    retry_run_result: bool = False
+    delay_since_first_attempt: int = 0
+    stop_run_result: bool = False
+    is_explicit_retry: bool = False
+
+    def reset(self) -> None:
+        self.actions = []
+        self.retry_run_result = False
+        self.delay_since_first_attempt = 0
+        self.stop_run_result = False
+        self.is_explicit_retry = False
+
+
 class TryAgain(Exception):
     """Always retry the executed function when raised."""
 
 
 NO_RESULT = object()
 
 
@@ -120,15 +143,17 @@
     - NAME: for identification in retry object methods and callbacks
     """
 
     REPR_FIELDS: t.Sequence[str] = ()
     NAME: t.Optional[str] = None
 
     def __repr__(self) -> str:
-        state_str = ", ".join(f"{field}={getattr(self, field)!r}" for field in self.REPR_FIELDS)
+        state_str = ", ".join(
+            f"{field}={getattr(self, field)!r}" for field in self.REPR_FIELDS
+        )
         return f"{self.__class__.__name__}({state_str})"
 
     def __str__(self) -> str:
         return repr(self)
 
 
 class RetryAction(BaseAction):
@@ -216,31 +241,37 @@
         self,
         sleep: t.Union[t.Callable[[t.Union[int, float]], None], object] = _unset,
         stop: t.Union["StopBaseT", object] = _unset,
         wait: t.Union["WaitBaseT", object] = _unset,
         retry: t.Union[retry_base, object] = _unset,
         before: t.Union[t.Callable[["RetryCallState"], None], object] = _unset,
         after: t.Union[t.Callable[["RetryCallState"], None], object] = _unset,
-        before_sleep: t.Union[t.Optional[t.Callable[["RetryCallState"], None]], object] = _unset,
+        before_sleep: t.Union[
+            t.Optional[t.Callable[["RetryCallState"], None]], object
+        ] = _unset,
         reraise: t.Union[bool, object] = _unset,
         retry_error_cls: t.Union[t.Type[RetryError], object] = _unset,
-        retry_error_callback: t.Union[t.Optional[t.Callable[["RetryCallState"], t.Any]], object] = _unset,
+        retry_error_callback: t.Union[
+            t.Optional[t.Callable[["RetryCallState"], t.Any]], object
+        ] = _unset,
     ) -> "BaseRetrying":
         """Copy this object with some parameters changed if needed."""
         return self.__class__(
             sleep=_first_set(sleep, self.sleep),
             stop=_first_set(stop, self.stop),
             wait=_first_set(wait, self.wait),
             retry=_first_set(retry, self.retry),
             before=_first_set(before, self.before),
             after=_first_set(after, self.after),
             before_sleep=_first_set(before_sleep, self.before_sleep),
             reraise=_first_set(reraise, self.reraise),
             retry_error_cls=_first_set(retry_error_cls, self.retry_error_cls),
-            retry_error_callback=_first_set(retry_error_callback, self.retry_error_callback),
+            retry_error_callback=_first_set(
+                retry_error_callback, self.retry_error_callback
+            ),
         )
 
     def __repr__(self) -> str:
         return (
             f"<{self.__class__.__name__} object at 0x{id(self):x} ("
             f"stop={self.stop}, "
             f"wait={self.wait}, "
@@ -274,21 +305,31 @@
         """
         try:
             return self._local.statistics  # type: ignore[no-any-return]
         except AttributeError:
             self._local.statistics = t.cast(t.Dict[str, t.Any], {})
             return self._local.statistics
 
+    @property
+    def iter_state(self) -> IterState:
+        try:
+            return self._local.iter_state  # type: ignore[no-any-return]
+        except AttributeError:
+            self._local.iter_state = IterState()
+            return self._local.iter_state
+
     def wraps(self, f: WrappedFn) -> WrappedFn:
         """Wrap a function for retrying.
 
         :param f: A function to wraps for retrying.
         """
 
-        @functools.wraps(f)
+        @functools.wraps(
+            f, functools.WRAPPER_ASSIGNMENTS + ("__defaults__", "__kwdefaults__")
+        )
         def wrapped_f(*args: t.Any, **kw: t.Any) -> t.Any:
             return self(f, *args, **kw)
 
         def retry_with(*args: t.Any, **kwargs: t.Any) -> WrappedFn:
             return self.copy(*args, **kwargs).wraps(f)
 
         wrapped_f.retry = self  # type: ignore[attr-defined]
@@ -298,50 +339,97 @@
 
     def begin(self) -> None:
         self.statistics.clear()
         self.statistics["start_time"] = time.monotonic()
         self.statistics["attempt_number"] = 1
         self.statistics["idle_for"] = 0
 
+    def _add_action_func(self, fn: t.Callable[..., t.Any]) -> None:
+        self.iter_state.actions.append(fn)
+
+    def _run_retry(self, retry_state: "RetryCallState") -> None:
+        self.iter_state.retry_run_result = self.retry(retry_state)
+
+    def _run_wait(self, retry_state: "RetryCallState") -> None:
+        if self.wait:
+            sleep = self.wait(retry_state)
+        else:
+            sleep = 0.0
+
+        retry_state.upcoming_sleep = sleep
+
+    def _run_stop(self, retry_state: "RetryCallState") -> None:
+        self.statistics["delay_since_first_attempt"] = retry_state.seconds_since_start
+        self.iter_state.stop_run_result = self.stop(retry_state)
+
     def iter(self, retry_state: "RetryCallState") -> t.Union[DoAttempt, DoSleep, t.Any]:  # noqa
+        self._begin_iter(retry_state)
+        result = None
+        for action in self.iter_state.actions:
+            result = action(retry_state)
+        return result
+
+    def _begin_iter(self, retry_state: "RetryCallState") -> None:  # noqa
+        self.iter_state.reset()
+
         fut = retry_state.outcome
         if fut is None:
             if self.before is not None:
-                self.before(retry_state)
-            return DoAttempt()
+                self._add_action_func(self.before)
+            self._add_action_func(lambda rs: DoAttempt())
+            return
 
-        is_explicit_retry = fut.failed and isinstance(fut.exception(), TryAgain)
-        if not (is_explicit_retry or self.retry(retry_state)):
-            return fut.result()
+        self.iter_state.is_explicit_retry = fut.failed and isinstance(
+            fut.exception(), TryAgain
+        )
+        if not self.iter_state.is_explicit_retry:
+            self._add_action_func(self._run_retry)
+        self._add_action_func(self._post_retry_check_actions)
+
+    def _post_retry_check_actions(self, retry_state: "RetryCallState") -> None:
+        if not (self.iter_state.is_explicit_retry or self.iter_state.retry_run_result):
+            self._add_action_func(lambda rs: rs.outcome.result())
+            return
 
         if self.after is not None:
-            self.after(retry_state)
+            self._add_action_func(self.after)
 
-        self.statistics["delay_since_first_attempt"] = retry_state.seconds_since_start
-        if self.stop(retry_state):
+        self._add_action_func(self._run_wait)
+        self._add_action_func(self._run_stop)
+        self._add_action_func(self._post_stop_check_actions)
+
+    def _post_stop_check_actions(self, retry_state: "RetryCallState") -> None:
+        if self.iter_state.stop_run_result:
             if self.retry_error_callback:
-                return self.retry_error_callback(retry_state)
-            retry_exc = self.retry_error_cls(fut)
-            if self.reraise:
-                raise retry_exc.reraise()
-            raise retry_exc from fut.exception()
+                self._add_action_func(self.retry_error_callback)
+                return
 
-        if self.wait:
-            sleep = self.wait(retry_state)
-        else:
-            sleep = 0.0
-        retry_state.next_action = RetryAction(sleep)
-        retry_state.idle_for += sleep
-        self.statistics["idle_for"] += sleep
-        self.statistics["attempt_number"] += 1
+            def exc_check(rs: "RetryCallState") -> None:
+                fut = t.cast(Future, rs.outcome)
+                retry_exc = self.retry_error_cls(fut)
+                if self.reraise:
+                    raise retry_exc.reraise()
+                raise retry_exc from fut.exception()
+
+            self._add_action_func(exc_check)
+            return
+
+        def next_action(rs: "RetryCallState") -> None:
+            sleep = rs.upcoming_sleep
+            rs.next_action = RetryAction(sleep)
+            rs.idle_for += sleep
+            self.statistics["idle_for"] += sleep
+            self.statistics["attempt_number"] += 1
+
+        self._add_action_func(next_action)
 
         if self.before_sleep is not None:
-            self.before_sleep(retry_state)
+            self._add_action_func(self.before_sleep)
 
-        return DoSleep(sleep)
+        self._add_action_func(lambda rs: DoSleep(rs.upcoming_sleep))
 
     def __iter__(self) -> t.Generator[AttemptManager, None, None]:
         self.begin()
 
         retry_state = RetryCallState(self, fn=None, args=(), kwargs={})
         while True:
             do = self.iter(retry_state=retry_state)
@@ -387,15 +475,15 @@
             elif isinstance(do, DoSleep):
                 retry_state.prepare_for_next_attempt()
                 self.sleep(do)
             else:
                 return do  # type: ignore[no-any-return]
 
 
-if sys.version_info[1] >= 9:
+if sys.version_info >= (3, 9):
     FutureGenericT = futures.Future[t.Any]
 else:
     FutureGenericT = futures.Future
 
 
 class Future(FutureGenericT):
     """Encapsulates a (future or past) attempted call to a target function."""
@@ -406,15 +494,17 @@
 
     @property
     def failed(self) -> bool:
         """Return whether a exception is being held in this future."""
         return self.exception() is not None
 
     @classmethod
-    def construct(cls, attempt_number: int, value: t.Any, has_exception: bool) -> "Future":
+    def construct(
+        cls, attempt_number: int, value: t.Any, has_exception: bool
+    ) -> "Future":
         """Construct a new Future object."""
         fut = cls(attempt_number)
         if has_exception:
             fut.set_exception(value)
         else:
             fut.set_result(value)
         return fut
@@ -447,14 +537,16 @@
         self.outcome: t.Optional[Future] = None
         #: Timestamp of the last outcome
         self.outcome_timestamp: t.Optional[float] = None
         #: Time spent sleeping in retries
         self.idle_for: float = 0.0
         #: Next action as decided by the retry manager
         self.next_action: t.Optional[RetryAction] = None
+        #: Next sleep time as decided by the retry manager.
+        self.upcoming_sleep: float = 0.0
 
     @property
     def seconds_since_start(self) -> t.Optional[float]:
         if self.outcome_timestamp is None:
             return None
         return self.outcome_timestamp - self.start_time
 
@@ -467,15 +559,18 @@
     def set_result(self, val: t.Any) -> None:
         ts = time.monotonic()
         fut = Future(self.attempt_number)
         fut.set_result(val)
         self.outcome, self.outcome_timestamp = fut, ts
 
     def set_exception(
-        self, exc_info: t.Tuple[t.Type[BaseException], BaseException, "types.TracebackType| None"]
+        self,
+        exc_info: t.Tuple[
+            t.Type[BaseException], BaseException, "types.TracebackType| None"
+        ],
     ) -> None:
         ts = time.monotonic()
         fut = Future(self.attempt_number)
         fut.set_exception(exc_info[1])
         self.outcome, self.outcome_timestamp = fut, ts
 
     def __repr__(self) -> str:
@@ -489,32 +584,30 @@
 
         slept = float(round(self.idle_for, 2))
         clsname = self.__class__.__name__
         return f"<{clsname} {id(self)}: attempt #{self.attempt_number}; slept for {slept}; last result: {result}>"
 
 
 @t.overload
-def retry(func: WrappedFn) -> WrappedFn:
-    ...
+def retry(func: WrappedFn) -> WrappedFn: ...
 
 
 @t.overload
 def retry(
     sleep: t.Callable[[t.Union[int, float]], t.Optional[t.Awaitable[None]]] = sleep,
     stop: "StopBaseT" = stop_never,
     wait: "WaitBaseT" = wait_none(),
     retry: "RetryBaseT" = retry_if_exception_type(),
     before: t.Callable[["RetryCallState"], None] = before_nothing,
     after: t.Callable[["RetryCallState"], None] = after_nothing,
     before_sleep: t.Optional[t.Callable[["RetryCallState"], None]] = None,
     reraise: bool = False,
     retry_error_cls: t.Type["RetryError"] = RetryError,
     retry_error_callback: t.Optional[t.Callable[["RetryCallState"], t.Any]] = None,
-) -> t.Callable[[WrappedFn], WrappedFn]:
-    ...
+) -> t.Callable[[WrappedFn], WrappedFn]: ...
 
 
 def retry(*dargs: t.Any, **dkw: t.Any) -> t.Any:
     """Wrap a function with a new `Retrying` object.
 
     :param dargs: positional arguments passed to Retrying object
     :param dkw: keyword arguments passed to the Retrying object
@@ -529,15 +622,19 @@
                 warnings.warn(
                     f"Got retry_base instance ({f.__class__.__name__}) as callable argument, "
                     f"this will probably hang indefinitely (did you mean retry={f.__class__.__name__}(...)?)"
                 )
             r: "BaseRetrying"
             if iscoroutinefunction(f):
                 r = AsyncRetrying(*dargs, **dkw)
-            elif tornado and hasattr(tornado.gen, "is_coroutine_function") and tornado.gen.is_coroutine_function(f):
+            elif (
+                tornado
+                and hasattr(tornado.gen, "is_coroutine_function")
+                and tornado.gen.is_coroutine_function(f)
+            ):
                 r = TornadoRetrying(*dargs, **dkw)
             else:
                 r = Retrying(*dargs, **dkw)
 
             return r.wraps(f)
 
         return wrap
@@ -564,14 +661,15 @@
     "retry_unless_exception_type",
     "retry_if_exception_message",
     "retry_if_not_exception_message",
     "sleep",
     "sleep_using_event",
     "stop_after_attempt",
     "stop_after_delay",
+    "stop_before_delay",
     "stop_all",
     "stop_any",
     "stop_never",
     "stop_when_event_set",
     "wait_chain",
     "wait_combine",
     "wait_exponential",
```

### Comparing `tenacity-8.2.3/tenacity/_asyncio.py` & `tenacity-8.3.0/tenacity/_asyncio.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,80 +14,134 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import functools
 import sys
 import typing as t
-from asyncio import sleep
 
 from tenacity import AttemptManager
 from tenacity import BaseRetrying
 from tenacity import DoAttempt
 from tenacity import DoSleep
 from tenacity import RetryCallState
+from tenacity import _utils
 
 WrappedFnReturnT = t.TypeVar("WrappedFnReturnT")
 WrappedFn = t.TypeVar("WrappedFn", bound=t.Callable[..., t.Awaitable[t.Any]])
 
 
+def asyncio_sleep(duration: float) -> t.Awaitable[None]:
+    # Lazy import asyncio as it's expensive (responsible for 25-50% of total import overhead).
+    import asyncio
+
+    return asyncio.sleep(duration)
+
+
 class AsyncRetrying(BaseRetrying):
     sleep: t.Callable[[float], t.Awaitable[t.Any]]
 
-    def __init__(self, sleep: t.Callable[[float], t.Awaitable[t.Any]] = sleep, **kwargs: t.Any) -> None:
+    def __init__(
+        self,
+        sleep: t.Callable[[float], t.Awaitable[t.Any]] = asyncio_sleep,
+        **kwargs: t.Any,
+    ) -> None:
         super().__init__(**kwargs)
         self.sleep = sleep
 
     async def __call__(  # type: ignore[override]
         self, fn: WrappedFn, *args: t.Any, **kwargs: t.Any
     ) -> WrappedFnReturnT:
         self.begin()
 
         retry_state = RetryCallState(retry_object=self, fn=fn, args=args, kwargs=kwargs)
         while True:
-            do = self.iter(retry_state=retry_state)
+            do = await self.iter(retry_state=retry_state)
             if isinstance(do, DoAttempt):
                 try:
                     result = await fn(*args, **kwargs)
                 except BaseException:  # noqa: B902
                     retry_state.set_exception(sys.exc_info())  # type: ignore[arg-type]
                 else:
                     retry_state.set_result(result)
             elif isinstance(do, DoSleep):
                 retry_state.prepare_for_next_attempt()
                 await self.sleep(do)
             else:
                 return do  # type: ignore[no-any-return]
 
+    @classmethod
+    def _wrap_action_func(cls, fn: t.Callable[..., t.Any]) -> t.Callable[..., t.Any]:
+        if _utils.is_coroutine_callable(fn):
+            return fn
+
+        async def inner(*args: t.Any, **kwargs: t.Any) -> t.Any:
+            return fn(*args, **kwargs)
+
+        return inner
+
+    def _add_action_func(self, fn: t.Callable[..., t.Any]) -> None:
+        self.iter_state.actions.append(self._wrap_action_func(fn))
+
+    async def _run_retry(self, retry_state: "RetryCallState") -> None:  # type: ignore[override]
+        self.iter_state.retry_run_result = await self._wrap_action_func(self.retry)(
+            retry_state
+        )
+
+    async def _run_wait(self, retry_state: "RetryCallState") -> None:  # type: ignore[override]
+        if self.wait:
+            sleep = await self._wrap_action_func(self.wait)(retry_state)
+        else:
+            sleep = 0.0
+
+        retry_state.upcoming_sleep = sleep
+
+    async def _run_stop(self, retry_state: "RetryCallState") -> None:  # type: ignore[override]
+        self.statistics["delay_since_first_attempt"] = retry_state.seconds_since_start
+        self.iter_state.stop_run_result = await self._wrap_action_func(self.stop)(
+            retry_state
+        )
+
+    async def iter(
+        self, retry_state: "RetryCallState"
+    ) -> t.Union[DoAttempt, DoSleep, t.Any]:  # noqa: A003
+        self._begin_iter(retry_state)
+        result = None
+        for action in self.iter_state.actions:
+            result = await action(retry_state)
+        return result
+
     def __iter__(self) -> t.Generator[AttemptManager, None, None]:
         raise TypeError("AsyncRetrying object is not iterable")
 
     def __aiter__(self) -> "AsyncRetrying":
         self.begin()
         self._retry_state = RetryCallState(self, fn=None, args=(), kwargs={})
         return self
 
     async def __anext__(self) -> AttemptManager:
         while True:
-            do = self.iter(retry_state=self._retry_state)
+            do = await self.iter(retry_state=self._retry_state)
             if do is None:
                 raise StopAsyncIteration
             elif isinstance(do, DoAttempt):
                 return AttemptManager(retry_state=self._retry_state)
             elif isinstance(do, DoSleep):
                 self._retry_state.prepare_for_next_attempt()
                 await self.sleep(do)
             else:
                 raise StopAsyncIteration
 
     def wraps(self, fn: WrappedFn) -> WrappedFn:
         fn = super().wraps(fn)
         # Ensure wrapper is recognized as a coroutine function.
 
-        @functools.wraps(fn)
+        @functools.wraps(
+            fn, functools.WRAPPER_ASSIGNMENTS + ("__defaults__", "__kwdefaults__")
+        )
         async def async_wrapped(*args: t.Any, **kwargs: t.Any) -> t.Any:
             return await fn(*args, **kwargs)
 
         # Preserve attributes
         async_wrapped.retry = fn.retry  # type: ignore[attr-defined]
         async_wrapped.retry_with = fn.retry_with  # type: ignore[attr-defined]
```

### Comparing `tenacity-8.2.3/tenacity/_utils.py` & `tenacity-8.3.0/tenacity/_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import functools
+import inspect
 import sys
 import typing
 from datetime import timedelta
 
 
 # sys.maxsize:
 # An integer giving the maximum value a variable of type Py_ssize_t can take.
@@ -69,8 +70,20 @@
         return ".".join(segments)
 
 
 time_unit_type = typing.Union[int, float, timedelta]
 
 
 def to_seconds(time_unit: time_unit_type) -> float:
-    return float(time_unit.total_seconds() if isinstance(time_unit, timedelta) else time_unit)
+    return float(
+        time_unit.total_seconds() if isinstance(time_unit, timedelta) else time_unit
+    )
+
+
+def is_coroutine_callable(call: typing.Callable[..., typing.Any]) -> bool:
+    if inspect.isclass(call):
+        return False
+    if inspect.iscoroutinefunction(call):
+        return True
+    partial_call = isinstance(call, functools.partial) and call.func
+    dunder_call = partial_call or getattr(call, "__call__", None)
+    return inspect.iscoroutinefunction(dunder_call)
```

### Comparing `tenacity-8.2.3/tenacity/after.py` & `tenacity-8.3.0/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `tenacity-8.2.3/tenacity/before.py` & `tenacity-8.3.0/tenacity/before.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     from tenacity import RetryCallState
 
 
 def before_nothing(retry_state: "RetryCallState") -> None:
     """Before call strategy that does nothing."""
 
 
-def before_log(logger: "logging.Logger", log_level: int) -> typing.Callable[["RetryCallState"], None]:
+def before_log(
+    logger: "logging.Logger", log_level: int
+) -> typing.Callable[["RetryCallState"], None]:
     """Before call strategy that logs to some logger the attempt."""
 
     def log_it(retry_state: "RetryCallState") -> None:
         if retry_state.fn is None:
             # NOTE(sileht): can't really happen, but we must please mypy
             fn_name = "<unknown>"
         else:
```

### Comparing `tenacity-8.2.3/tenacity/before_sleep.py` & `tenacity-8.3.0/tenacity/before_sleep.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,12 +60,13 @@
             # NOTE(sileht): can't really happen, but we must please mypy
             fn_name = "<unknown>"
         else:
             fn_name = _utils.get_callback_name(retry_state.fn)
 
         logger.log(
             log_level,
-            f"Retrying {fn_name} " f"in {retry_state.next_action.sleep} seconds as it {verb} {value}.",
+            f"Retrying {fn_name} "
+            f"in {retry_state.next_action.sleep} seconds as it {verb} {value}.",
             exc_info=local_exc_info,
         )
 
     return log_it
```

### Comparing `tenacity-8.2.3/tenacity/nap.py` & `tenacity-8.3.0/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `tenacity-8.2.3/tenacity/retry.py` & `tenacity-8.3.0/tenacity/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,17 @@
 
     def __init__(
         self,
         message: typing.Optional[str] = None,
         match: typing.Optional[str] = None,
     ) -> None:
         if message and match:
-            raise TypeError(f"{self.__class__.__name__}() takes either 'message' or 'match', not both")
+            raise TypeError(
+                f"{self.__class__.__name__}() takes either 'message' or 'match', not both"
+            )
 
         # set predicate
         if message:
 
             def message_fnc(exception: BaseException) -> bool:
                 return message == str(exception)
 
@@ -217,15 +219,17 @@
             prog = re.compile(match)
 
             def match_fnc(exception: BaseException) -> bool:
                 return bool(prog.match(str(exception)))
 
             predicate = match_fnc
         else:
-            raise TypeError(f"{self.__class__.__name__}() missing 1 required argument 'message' or 'match'")
+            raise TypeError(
+                f"{self.__class__.__name__}() missing 1 required argument 'message' or 'match'"
+            )
 
         super().__init__(predicate)
 
 
 class retry_if_not_exception_message(retry_if_exception_message):
     """Retries until an exception message equals or matches."""
```

### Comparing `tenacity-8.2.3/tenacity/stop.py` & `tenacity-8.3.0/tenacity/stop.py`

 * *Files 20% similar despite different names*

```diff
@@ -88,16 +88,43 @@
         self.max_attempt_number = max_attempt_number
 
     def __call__(self, retry_state: "RetryCallState") -> bool:
         return retry_state.attempt_number >= self.max_attempt_number
 
 
 class stop_after_delay(stop_base):
-    """Stop when the time from the first attempt >= limit."""
+    """
+    Stop when the time from the first attempt >= limit.
+
+    Note: `max_delay` will be exceeded, so when used with a `wait`, the actual total delay will be greater
+    than `max_delay` by some of the final sleep period before `max_delay` is exceeded.
+
+    If you need stricter timing with waits, consider `stop_before_delay` instead.
+    """
 
     def __init__(self, max_delay: _utils.time_unit_type) -> None:
         self.max_delay = _utils.to_seconds(max_delay)
 
     def __call__(self, retry_state: "RetryCallState") -> bool:
         if retry_state.seconds_since_start is None:
             raise RuntimeError("__call__() called but seconds_since_start is not set")
         return retry_state.seconds_since_start >= self.max_delay
+
+
+class stop_before_delay(stop_base):
+    """
+    Stop right before the next attempt would take place after the time from the first attempt >= limit.
+
+    Most useful when you are using with a `wait` function like wait_random_exponential, but need to make
+    sure that the max_delay is not exceeded.
+    """
+
+    def __init__(self, max_delay: _utils.time_unit_type) -> None:
+        self.max_delay = _utils.to_seconds(max_delay)
+
+    def __call__(self, retry_state: "RetryCallState") -> bool:
+        if retry_state.seconds_since_start is None:
+            raise RuntimeError("__call__() called but seconds_since_start is not set")
+        return (
+            retry_state.seconds_since_start + retry_state.upcoming_sleep
+            >= self.max_delay
+        )
```

### Comparing `tenacity-8.2.3/tenacity/tornadoweb.py` & `tenacity-8.3.0/tenacity/tornadoweb.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 if typing.TYPE_CHECKING:
     from tornado.concurrent import Future
 
 _RetValT = typing.TypeVar("_RetValT")
 
 
 class TornadoRetrying(BaseRetrying):
-    def __init__(self, sleep: "typing.Callable[[float], Future[None]]" = gen.sleep, **kwargs: typing.Any) -> None:
+    def __init__(
+        self,
+        sleep: "typing.Callable[[float], Future[None]]" = gen.sleep,
+        **kwargs: typing.Any,
+    ) -> None:
         super().__init__(**kwargs)
         self.sleep = sleep
 
     @gen.coroutine  # type: ignore[misc]
     def __call__(
         self,
         fn: "typing.Callable[..., typing.Union[typing.Generator[typing.Any, typing.Any, _RetValT], Future[_RetValT]]]",
```

### Comparing `tenacity-8.2.3/tenacity/wait.py` & `tenacity-8.3.0/tenacity/wait.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,17 @@
     def __radd__(self, other: "wait_base") -> typing.Union["wait_combine", "wait_base"]:
         # make it possible to use multiple waits with the built-in sum function
         if other == 0:  # type: ignore[comparison-overlap]
             return self
         return self.__add__(other)
 
 
-WaitBaseT = typing.Union[wait_base, typing.Callable[["RetryCallState"], typing.Union[float, int]]]
+WaitBaseT = typing.Union[
+    wait_base, typing.Callable[["RetryCallState"], typing.Union[float, int]]
+]
 
 
 class wait_fixed(wait_base):
     """Wait strategy that waits a fixed amount of time between each retry."""
 
     def __init__(self, wait: _utils.time_unit_type) -> None:
         self.wait_fixed = _utils.to_seconds(wait)
@@ -60,20 +62,24 @@
     def __init__(self) -> None:
         super().__init__(0)
 
 
 class wait_random(wait_base):
     """Wait strategy that waits a random amount of time between min/max."""
 
-    def __init__(self, min: _utils.time_unit_type = 0, max: _utils.time_unit_type = 1) -> None:  # noqa
+    def __init__(
+        self, min: _utils.time_unit_type = 0, max: _utils.time_unit_type = 1
+    ) -> None:  # noqa
         self.wait_random_min = _utils.to_seconds(min)
         self.wait_random_max = _utils.to_seconds(max)
 
     def __call__(self, retry_state: "RetryCallState") -> float:
-        return self.wait_random_min + (random.random() * (self.wait_random_max - self.wait_random_min))
+        return self.wait_random_min + (
+            random.random() * (self.wait_random_max - self.wait_random_min)
+        )
 
 
 class wait_combine(wait_base):
     """Combine several waiting strategies."""
 
     def __init__(self, *strategies: wait_base) -> None:
         self.wait_funcs = strategies
```

### Comparing `tenacity-8.2.3/tenacity.egg-info/PKG-INFO` & `tenacity-8.3.0/tenacity.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: tenacity
-Version: 8.2.3
+Version: 8.3.0
 Summary: Retry code until it succeeds
 Home-page: https://github.com/jd/tenacity
 Author: Julien Danjou
 Author-email: julien@danjou.info
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: doc
+Provides-Extra: test
 License-File: LICENSE
 
 Tenacity is a general-purpose retrying library to simplify the task of adding retry behavior to just about anything.
```

### Comparing `tenacity-8.2.3/tenacity.egg-info/SOURCES.txt` & `tenacity-8.3.0/tenacity.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,45 +5,50 @@
 LICENSE
 README.rst
 pyproject.toml
 reno.yaml
 setup.cfg
 setup.py
 tox.ini
+.github/dependabot.yml
 .github/workflows/ci.yaml
 .github/workflows/deploy.yaml
 doc/source/api.rst
 doc/source/changelog.rst
 doc/source/conf.py
 doc/source/index.rst
 releasenotes/notes/Fix-tests-for-typeguard-3.x-6eebfea546b6207e.yaml
 releasenotes/notes/Use--for-formatting-and-validate-using-black-39ec9d57d4691778.yaml
 releasenotes/notes/add-reno-d1ab5710f272650a.yaml
 releasenotes/notes/add-retry_except_exception_type-31b31da1924d55f4.yaml
+releasenotes/notes/add-stop-before-delay-a775f88ac872c923.yaml
+releasenotes/notes/add-test-extra-55e869261b03e56d.yaml
 releasenotes/notes/add_omitted_modules_to_import_all-2ab282f20a2c22f7.yaml
 releasenotes/notes/add_retry_if_exception_cause_type-d16b918ace4ae0ad.yaml
 releasenotes/notes/added_a_link_to_documentation-eefaf8f074b539f8.yaml
 releasenotes/notes/after_log-50f4d73b24ce9203.yaml
 releasenotes/notes/allow-mocking-of-nap-sleep-6679c50e702446f1.yaml
 releasenotes/notes/annotate_code-197b93130df14042.yaml
 releasenotes/notes/before_sleep_log-improvements-d8149274dfb37d7c.yaml
 releasenotes/notes/clarify-reraise-option-6829667eacf4f599.yaml
+releasenotes/notes/dependabot-for-github-actions-4d2464f3c0928463.yaml
 releasenotes/notes/do_not_package_tests-fe5ac61940b0a5ed.yaml
 releasenotes/notes/drop-deprecated-python-versions-69a05cb2e0f1034c.yaml
 releasenotes/notes/drop_deprecated-7ea90b212509b082.yaml
 releasenotes/notes/export-convenience-symbols-981d9611c8b754f3.yaml
 releasenotes/notes/fix-async-loop-with-result-f68e913ccb425aca.yaml
 releasenotes/notes/fix-wait-typing-b26eecdb6cc0a1de.yaml
 releasenotes/notes/fix_async-52b6594c8e75c4bc.yaml
 releasenotes/notes/make-logger-more-compatible-5da1ddf1bab77047.yaml
 releasenotes/notes/no-async-iter-6132a42e52348a75.yaml
 releasenotes/notes/pr320-py3-only-wheel-tag.yaml
 releasenotes/notes/py36_plus-c425fb3aa17c6682.yaml
 releasenotes/notes/remove-py36-876c0416cf279d15.yaml
 releasenotes/notes/retrycallstate-repr-94947f7b00ee15e1.yaml
+releasenotes/notes/some-slug-for-preserve-defaults-86682846dfa18005.yaml
 releasenotes/notes/sphinx_define_error-642c9cd5c165d39a.yaml
 releasenotes/notes/support-timedelta-wait-unit-type-5ba1e9fc0fe45523.yaml
 releasenotes/notes/timedelta-for-stop-ef6bf71b88ce9988.yaml
 releasenotes/notes/wait_exponential_jitter-6ffc81dddcbaa6d3.yaml
 tenacity/__init__.py
 tenacity/_asyncio.py
 tenacity/_utils.py
@@ -61,8 +66,9 @@
 tenacity.egg-info/dependency_links.txt
 tenacity.egg-info/requires.txt
 tenacity.egg-info/top_level.txt
 tests/__init__.py
 tests/test_after.py
 tests/test_asyncio.py
 tests/test_tenacity.py
-tests/test_tornado.py
+tests/test_tornado.py
+tests/test_utils.py
```

### Comparing `tenacity-8.2.3/tests/test_after.py` & `tenacity-8.3.0/tests/test_after.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,51 @@
+# mypy: disable-error-code="no-untyped-def,no-untyped-call"
 import logging
 import random
 import unittest.mock
 
 from tenacity import _utils  # noqa
 from tenacity import after_log
 
 from . import test_tenacity
 
 
 class TestAfterLogFormat(unittest.TestCase):
     def setUp(self) -> None:
-        self.log_level = random.choice((logging.DEBUG, logging.INFO, logging.WARNING, logging.ERROR, logging.CRITICAL))
+        self.log_level = random.choice(
+            (
+                logging.DEBUG,
+                logging.INFO,
+                logging.WARNING,
+                logging.ERROR,
+                logging.CRITICAL,
+            )
+        )
         self.previous_attempt_number = random.randint(1, 512)
 
     def test_01_default(self):
         """Test log formatting."""
         log = unittest.mock.MagicMock(spec="logging.Logger.log")
         logger = unittest.mock.MagicMock(spec="logging.Logger", log=log)
 
         sec_format = "%0.3f"
         delay_since_first_attempt = 0.1
 
-        retry_state = test_tenacity.make_retry_state(self.previous_attempt_number, delay_since_first_attempt)
-        fun = after_log(logger=logger, log_level=self.log_level)  # use default sec_format
+        retry_state = test_tenacity.make_retry_state(
+            self.previous_attempt_number, delay_since_first_attempt
+        )
+        fun = after_log(
+            logger=logger, log_level=self.log_level
+        )  # use default sec_format
         fun(retry_state)
-        fn_name = "<unknown>" if retry_state.fn is None else _utils.get_callback_name(retry_state.fn)
+        fn_name = (
+            "<unknown>"
+            if retry_state.fn is None
+            else _utils.get_callback_name(retry_state.fn)
+        )
         log.assert_called_once_with(
             self.log_level,
             f"Finished call to '{fn_name}' "
             f"after {sec_format % retry_state.seconds_since_start}(s), "
             f"this was the {_utils.to_ordinal(retry_state.attempt_number)} time calling it.",
         )
 
@@ -36,17 +53,23 @@
         """Test log formatting with custom int format.."""
         log = unittest.mock.MagicMock(spec="logging.Logger.log")
         logger = unittest.mock.MagicMock(spec="logging.Logger", log=log)
 
         sec_format = "%.1f"
         delay_since_first_attempt = 0.1
 
-        retry_state = test_tenacity.make_retry_state(self.previous_attempt_number, delay_since_first_attempt)
+        retry_state = test_tenacity.make_retry_state(
+            self.previous_attempt_number, delay_since_first_attempt
+        )
         fun = after_log(logger=logger, log_level=self.log_level, sec_format=sec_format)
         fun(retry_state)
-        fn_name = "<unknown>" if retry_state.fn is None else _utils.get_callback_name(retry_state.fn)
+        fn_name = (
+            "<unknown>"
+            if retry_state.fn is None
+            else _utils.get_callback_name(retry_state.fn)
+        )
         log.assert_called_once_with(
             self.log_level,
             f"Finished call to '{fn_name}' "
             f"after {sec_format % retry_state.seconds_since_start}(s), "
             f"this was the {_utils.to_ordinal(retry_state.attempt_number)} time calling it.",
         )
```

### Comparing `tenacity-8.2.3/tests/test_asyncio.py` & `tenacity-8.3.0/tests/test_asyncio.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# coding: utf-8
+# mypy: disable-error-code="no-untyped-def,no-untyped-call"
 # Copyright 2016 Étienne Bersac
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
@@ -16,14 +16,15 @@
 import asyncio
 import inspect
 import unittest
 from functools import wraps
 
 import pytest
 
+import tenacity
 from tenacity import AsyncRetrying, RetryError
 from tenacity import _asyncio as tasyncio
 from tenacity import retry, retry_if_result, stop_after_attempt
 from tenacity.wait import wait_fixed
 
 from .test_tenacity import NoIOErrorAfterCount, current_time_ms
 
@@ -84,27 +85,48 @@
     def test_repr(self):
         repr(tasyncio.AsyncRetrying())
 
     def test_retry_attributes(self):
         assert hasattr(_retryable_coroutine, "retry")
         assert hasattr(_retryable_coroutine, "retry_with")
 
+    def test_retry_preserves_argument_defaults(self):
+        async def function_with_defaults(a=1):
+            return a
+
+        async def function_with_kwdefaults(*, a=1):
+            return a
+
+        retrying = AsyncRetrying(
+            wait=tenacity.wait_fixed(0.01), stop=tenacity.stop_after_attempt(3)
+        )
+        wrapped_defaults_function = retrying.wraps(function_with_defaults)
+        wrapped_kwdefaults_function = retrying.wraps(function_with_kwdefaults)
+
+        self.assertEqual(
+            function_with_defaults.__defaults__, wrapped_defaults_function.__defaults__
+        )
+        self.assertEqual(
+            function_with_kwdefaults.__kwdefaults__,
+            wrapped_kwdefaults_function.__kwdefaults__,
+        )
+
     @asynctest
     async def test_attempt_number_is_correct_for_interleaved_coroutines(self):
         attempts = []
 
         def after(retry_state):
             attempts.append((retry_state.args[0], retry_state.attempt_number))
 
         thing1 = NoIOErrorAfterCount(3)
         thing2 = NoIOErrorAfterCount(3)
 
         await asyncio.gather(
-            _retryable_coroutine.retry_with(after=after)(thing1),
-            _retryable_coroutine.retry_with(after=after)(thing2),
+            _retryable_coroutine.retry_with(after=after)(thing1),  # type: ignore[attr-defined]
+            _retryable_coroutine.retry_with(after=after)(thing2),  # type: ignore[attr-defined]
         )
 
         # There's no waiting on retry, only a wait in the coroutine, so the
         # executions should be interleaved.
         even_thing_attempts = attempts[::2]
         things, attempt_nos1 = zip(*even_thing_attempts)
         assert len(set(things)) == 1
@@ -133,39 +155,48 @@
 
     @asynctest
     async def test_reraise(self):
         class CustomError(Exception):
             pass
 
         try:
-            async for attempt in tasyncio.AsyncRetrying(stop=stop_after_attempt(1), reraise=True):
+            async for attempt in tasyncio.AsyncRetrying(
+                stop=stop_after_attempt(1), reraise=True
+            ):
                 with attempt:
                     raise CustomError()
         except CustomError:
             pass
         else:
             raise Exception
 
     @asynctest
     async def test_sleeps(self):
         start = current_time_ms()
         try:
-            async for attempt in tasyncio.AsyncRetrying(stop=stop_after_attempt(1), wait=wait_fixed(1)):
+            async for attempt in tasyncio.AsyncRetrying(
+                stop=stop_after_attempt(1), wait=wait_fixed(1)
+            ):
                 with attempt:
                     raise Exception()
         except RetryError:
             pass
         t = current_time_ms() - start
         self.assertLess(t, 1.1)
 
     @asynctest
     async def test_retry_with_result(self):
         async def test():
             attempts = 0
-            async for attempt in tasyncio.AsyncRetrying(retry=retry_if_result(lambda x: x < 3)):
+
+            # mypy doesn't have great lambda support
+            def lt_3(x: float) -> bool:
+                return x < 3
+
+            async for attempt in tasyncio.AsyncRetrying(retry=retry_if_result(lt_3)):
                 with attempt:
                     attempts += 1
                 attempt.retry_state.set_result(attempts)
             return attempts
 
         result = await test()
 
@@ -176,9 +207,20 @@
         thing = NoIOErrorAfterCount(5)
         with pytest.raises(TypeError):
             for attempts in AsyncRetrying():
                 with attempts:
                     await _async_function(thing)
 
 
+# make sure mypy accepts passing an async sleep function
+# https://github.com/jd/tenacity/issues/399
+async def my_async_sleep(x: float) -> None:
+    await asyncio.sleep(x)
+
+
+@retry(sleep=my_async_sleep)
+async def foo():
+    pass
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `tenacity-8.2.3/tests/test_tenacity.py` & `tenacity-8.3.0/tests/test_tenacity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable_error_code="no-untyped-def,no-untyped-call,attr-defined,arg-type,no-any-return,list-item,var-annotated,import,call-overload"
 # Copyright 2016–2021 Julien Danjou
 # Copyright 2016 Joshua Harlow
 # Copyright 2013 Ray Holder
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
@@ -46,33 +47,43 @@
     # Ensure outcome_timestamp - start_time is *exactly* equal to the delay to
     # avoid complexity in test code.
     retry_state.start_time = Fraction(retry_state.start_time)
     retry_state.outcome_timestamp = retry_state.start_time + Fraction(delay)
     assert retry_state.seconds_since_start == delay
 
 
-def make_retry_state(previous_attempt_number, delay_since_first_attempt, last_result=None):
+def make_retry_state(
+    previous_attempt_number,
+    delay_since_first_attempt,
+    last_result=None,
+    upcoming_sleep=0,
+):
     """Construct RetryCallState for given attempt number & delay.
 
     Only used in testing and thus is extra careful about timestamp arithmetics.
     """
-    required_parameter_unset = previous_attempt_number is _unset or delay_since_first_attempt is _unset
+    required_parameter_unset = (
+        previous_attempt_number is _unset or delay_since_first_attempt is _unset
+    )
     if required_parameter_unset:
         raise _make_unset_exception(
             "wait/stop",
             previous_attempt_number=previous_attempt_number,
             delay_since_first_attempt=delay_since_first_attempt,
         )
 
     retry_state = RetryCallState(None, None, (), {})
     retry_state.attempt_number = previous_attempt_number
     if last_result is not None:
         retry_state.outcome = last_result
     else:
         retry_state.set_result(None)
+
+    retry_state.upcoming_sleep = upcoming_sleep
+
     _set_delay_since_start(retry_state, delay_since_first_attempt)
     return retry_state
 
 
 class TestBase(unittest.TestCase):
     def test_retrying_repr(self):
         class ConcreteRetrying(tenacity.BaseRetrying):
@@ -82,39 +93,49 @@
         repr(ConcreteRetrying())
 
     def test_callstate_repr(self):
         rs = RetryCallState(None, None, (), {})
         rs.idle_for = 1.1111111
         assert repr(rs).endswith("attempt #1; slept for 1.11; last result: none yet>")
         rs = make_retry_state(2, 5)
-        assert repr(rs).endswith("attempt #2; slept for 0.0; last result: returned None>")
-        rs = make_retry_state(0, 0, last_result=tenacity.Future.construct(1, ValueError("aaa"), True))
-        assert repr(rs).endswith("attempt #0; slept for 0.0; last result: failed (ValueError aaa)>")
+        assert repr(rs).endswith(
+            "attempt #2; slept for 0.0; last result: returned None>"
+        )
+        rs = make_retry_state(
+            0, 0, last_result=tenacity.Future.construct(1, ValueError("aaa"), True)
+        )
+        assert repr(rs).endswith(
+            "attempt #0; slept for 0.0; last result: failed (ValueError aaa)>"
+        )
 
 
 class TestStopConditions(unittest.TestCase):
     def test_never_stop(self):
         r = Retrying()
         self.assertFalse(r.stop(make_retry_state(3, 6546)))
 
     def test_stop_any(self):
-        stop = tenacity.stop_any(tenacity.stop_after_delay(1), tenacity.stop_after_attempt(4))
+        stop = tenacity.stop_any(
+            tenacity.stop_after_delay(1), tenacity.stop_after_attempt(4)
+        )
 
         def s(*args):
             return stop(make_retry_state(*args))
 
         self.assertFalse(s(1, 0.1))
         self.assertFalse(s(2, 0.2))
         self.assertFalse(s(2, 0.8))
         self.assertTrue(s(4, 0.8))
         self.assertTrue(s(3, 1.8))
         self.assertTrue(s(4, 1.8))
 
     def test_stop_all(self):
-        stop = tenacity.stop_all(tenacity.stop_after_delay(1), tenacity.stop_after_attempt(4))
+        stop = tenacity.stop_all(
+            tenacity.stop_after_delay(1), tenacity.stop_after_attempt(4)
+        )
 
         def s(*args):
             return stop(make_retry_state(*args))
 
         self.assertFalse(s(1, 0.1))
         self.assertFalse(s(2, 0.2))
         self.assertFalse(s(2, 0.8))
@@ -158,14 +179,29 @@
         for delay in (1, datetime.timedelta(seconds=1)):
             with self.subTest():
                 r = Retrying(stop=tenacity.stop_after_delay(delay))
                 self.assertFalse(r.stop(make_retry_state(2, 0.999)))
                 self.assertTrue(r.stop(make_retry_state(2, 1)))
                 self.assertTrue(r.stop(make_retry_state(2, 1.001)))
 
+    def test_stop_before_delay(self):
+        for delay in (1, datetime.timedelta(seconds=1)):
+            with self.subTest():
+                r = Retrying(stop=tenacity.stop_before_delay(delay))
+                self.assertFalse(
+                    r.stop(make_retry_state(2, 0.999, upcoming_sleep=0.0001))
+                )
+                self.assertTrue(r.stop(make_retry_state(2, 1, upcoming_sleep=0.001)))
+                self.assertTrue(r.stop(make_retry_state(2, 1, upcoming_sleep=1)))
+
+                # It should act the same as stop_after_delay if upcoming sleep is 0
+                self.assertFalse(r.stop(make_retry_state(2, 0.999, upcoming_sleep=0)))
+                self.assertTrue(r.stop(make_retry_state(2, 1, upcoming_sleep=0)))
+                self.assertTrue(r.stop(make_retry_state(2, 1.001, upcoming_sleep=0)))
+
     def test_legacy_explicit_stop_type(self):
         Retrying(stop="stop_after_attempt")
 
     def test_stop_func_with_retry_state(self):
         def stop_func(retry_state):
             rs = retry_state
             return rs.attempt_number == rs.seconds_since_start
@@ -184,23 +220,31 @@
     def test_fixed_sleep(self):
         for wait in (1, datetime.timedelta(seconds=1)):
             with self.subTest():
                 r = Retrying(wait=tenacity.wait_fixed(wait))
                 self.assertEqual(1, r.wait(make_retry_state(12, 6546)))
 
     def test_incrementing_sleep(self):
-        for start, increment in ((500, 100), (datetime.timedelta(seconds=500), datetime.timedelta(seconds=100))):
+        for start, increment in (
+            (500, 100),
+            (datetime.timedelta(seconds=500), datetime.timedelta(seconds=100)),
+        ):
             with self.subTest():
-                r = Retrying(wait=tenacity.wait_incrementing(start=start, increment=increment))
+                r = Retrying(
+                    wait=tenacity.wait_incrementing(start=start, increment=increment)
+                )
                 self.assertEqual(500, r.wait(make_retry_state(1, 6546)))
                 self.assertEqual(600, r.wait(make_retry_state(2, 6546)))
                 self.assertEqual(700, r.wait(make_retry_state(3, 6546)))
 
     def test_random_sleep(self):
-        for min_, max_ in ((1, 20), (datetime.timedelta(seconds=1), datetime.timedelta(seconds=20))):
+        for min_, max_ in (
+            (1, 20),
+            (datetime.timedelta(seconds=1), datetime.timedelta(seconds=20)),
+        ):
             with self.subTest():
                 r = Retrying(wait=tenacity.wait_random(min=min_, max=max_))
                 times = set()
                 for _ in range(1000):
                     times.add(r.wait(make_retry_state(1, 6546)))
 
                 # this is kind of non-deterministic...
@@ -279,15 +323,18 @@
         self.assertEqual(r.wait(make_retry_state(5, 0)), 32)
         self.assertEqual(r.wait(make_retry_state(6, 0)), 64)
         self.assertEqual(r.wait(make_retry_state(7, 0)), 128)
         self.assertEqual(r.wait(make_retry_state(8, 0)), 256)
         self.assertEqual(r.wait(make_retry_state(20, 0)), 1048576)
 
     def test_exponential_with_min_wait_andmax__wait(self):
-        for min_, max_ in ((10, 100), (datetime.timedelta(seconds=10), datetime.timedelta(seconds=100))):
+        for min_, max_ in (
+            (10, 100),
+            (datetime.timedelta(seconds=10), datetime.timedelta(seconds=100)),
+        ):
             with self.subTest():
                 r = Retrying(wait=tenacity.wait_exponential(min=min_, max=max_))
                 self.assertEqual(r.wait(make_retry_state(1, 0)), 10)
                 self.assertEqual(r.wait(make_retry_state(2, 0)), 10)
                 self.assertEqual(r.wait(make_retry_state(3, 0)), 10)
                 self.assertEqual(r.wait(make_retry_state(4, 0)), 10)
                 self.assertEqual(r.wait(make_retry_state(5, 0)), 16)
@@ -306,15 +353,19 @@
 
         r = Retrying(wait=wait_func)
         self.assertEqual(r.wait(make_retry_state(1, 5)), 5)
         self.assertEqual(r.wait(make_retry_state(2, 11)), 22)
         self.assertEqual(r.wait(make_retry_state(10, 100)), 1000)
 
     def test_wait_combine(self):
-        r = Retrying(wait=tenacity.wait_combine(tenacity.wait_random(0, 3), tenacity.wait_fixed(5)))
+        r = Retrying(
+            wait=tenacity.wait_combine(
+                tenacity.wait_random(0, 3), tenacity.wait_fixed(5)
+            )
+        )
         # Test it a few time since it's random
         for i in range(1000):
             w = r.wait(make_retry_state(1, 5))
             self.assertLess(w, 8)
             self.assertGreaterEqual(w, 5)
 
     def test_wait_double_sum(self):
@@ -322,15 +373,19 @@
         # Test it a few time since it's random
         for i in range(1000):
             w = r.wait(make_retry_state(1, 5))
             self.assertLess(w, 8)
             self.assertGreaterEqual(w, 5)
 
     def test_wait_triple_sum(self):
-        r = Retrying(wait=tenacity.wait_fixed(1) + tenacity.wait_random(0, 3) + tenacity.wait_fixed(5))
+        r = Retrying(
+            wait=tenacity.wait_fixed(1)
+            + tenacity.wait_random(0, 3)
+            + tenacity.wait_fixed(5)
+        )
         # Test it a few time since it's random
         for i in range(1000):
             w = r.wait(make_retry_state(1, 5))
             self.assertLess(w, 9)
             self.assertGreaterEqual(w, 6)
 
     def test_wait_arbitrary_sum(self):
@@ -474,15 +529,18 @@
         # retry_state is mutable, so return it as an exception to extract the
         # exact values it has when wait is called and bypass any other logic.
         def waitfunc(retry_state):
             raise ExtractCallState(retry_state)
 
         retrying = Retrying(
             wait=waitfunc,
-            retry=(tenacity.retry_if_exception_type() | tenacity.retry_if_result(lambda result: result == 123)),
+            retry=(
+                tenacity.retry_if_exception_type()
+                | tenacity.retry_if_result(lambda result: result == 123)
+            ),
         )
 
         def returnval():
             return 123
 
         try:
             retrying(returnval)
@@ -558,27 +616,31 @@
 
         self.assertTrue(r(tenacity.Future.construct(1, 1, False)))
         self.assertFalse(r(tenacity.Future.construct(1, 2, False)))
         self.assertFalse(r(tenacity.Future.construct(1, 3, False)))
         self.assertFalse(r(tenacity.Future.construct(1, 1, True)))
 
     def test_retry_and(self):
-        retry = tenacity.retry_if_result(lambda x: x == 1) & tenacity.retry_if_result(lambda x: isinstance(x, int))
+        retry = tenacity.retry_if_result(lambda x: x == 1) & tenacity.retry_if_result(
+            lambda x: isinstance(x, int)
+        )
 
         def r(fut):
             retry_state = make_retry_state(1, 1.0, last_result=fut)
             return retry(retry_state)
 
         self.assertTrue(r(tenacity.Future.construct(1, 1, False)))
         self.assertFalse(r(tenacity.Future.construct(1, 2, False)))
         self.assertFalse(r(tenacity.Future.construct(1, 3, False)))
         self.assertFalse(r(tenacity.Future.construct(1, 1, True)))
 
     def test_retry_or(self):
-        retry = tenacity.retry_if_result(lambda x: x == "foo") | tenacity.retry_if_result(lambda x: isinstance(x, int))
+        retry = tenacity.retry_if_result(
+            lambda x: x == "foo"
+        ) | tenacity.retry_if_result(lambda x: isinstance(x, int))
 
         def r(fut):
             retry_state = make_retry_state(1, 1.0, last_result=fut)
             return retry(retry_state)
 
         self.assertTrue(r(tenacity.Future.construct(1, "foo", False)))
         self.assertFalse(r(tenacity.Future.construct(1, "foobar", False)))
@@ -588,15 +650,17 @@
     def _raise_try_again(self):
         self._attempts += 1
         if self._attempts < 3:
             raise tenacity.TryAgain
 
     def test_retry_try_again(self):
         self._attempts = 0
-        Retrying(stop=tenacity.stop_after_attempt(5), retry=tenacity.retry_never)(self._raise_try_again)
+        Retrying(stop=tenacity.stop_after_attempt(5), retry=tenacity.retry_never)(
+            self._raise_try_again
+        )
         self.assertEqual(3, self._attempts)
 
     def test_retry_try_again_forever(self):
         def _r():
             raise tenacity.TryAgain
 
         r = Retrying(stop=tenacity.stop_after_attempt(5), retry=tenacity.retry_never)
@@ -652,15 +716,15 @@
     def go(self):
         """Raise an IOError until after count threshold has been crossed.
 
         Then return True.
         """
         if self.counter < self.count:
             self.counter += 1
-            raise IOError("Hi there, I'm an IOError")
+            raise OSError("Hi there, I'm an IOError")
         return True
 
 
 class NoNameErrorAfterCount:
     """Holds counter state for invoking a method several times in a row."""
 
     def __init__(self, count):
@@ -694,39 +758,39 @@
         Then return True.
         """
         if self.counter < self.count:
             self.counter += 1
             try:
                 self.go2()
             except NameError as e:
-                raise IOError() from e
+                raise OSError() from e
 
         return True
 
 
 class NoIOErrorCauseAfterCount:
     """Holds counter state for invoking a method several times in a row."""
 
     def __init__(self, count):
         self.counter = 0
         self.count = count
 
     def go2(self):
-        raise IOError("Hi there, I'm an IOError")
+        raise OSError("Hi there, I'm an IOError")
 
     def go(self):
         """Raise a NameError with an IOError as cause until after count threshold has been crossed.
 
         Then return True.
         """
         if self.counter < self.count:
             self.counter += 1
             try:
                 self.go2()
-            except IOError as e:
+            except OSError as e:
                 raise NameError() from e
 
         return True
 
 
 class NameErrorUntilCount:
     """Holds counter state for invoking a method several times in a row."""
@@ -759,15 +823,15 @@
         """Return True until after count threshold has been crossed.
 
         Then raise an IOError.
         """
         if self.counter < self.count:
             self.counter += 1
             return True
-        raise IOError("Hi there, I'm an IOError")
+        raise OSError("Hi there, I'm an IOError")
 
 
 class CustomError(Exception):
     """This is a custom exception class.
 
     Note that For Python 2.x, we don't strictly need to extend BaseException,
     however, Python 3.x will complain. While this test suite won't run
@@ -846,15 +910,17 @@
 
 
 @retry(retry=tenacity.retry_if_not_exception_type(IOError))
 def _retryable_test_if_not_exception_type_io(thing):
     return thing.go()
 
 
-@retry(stop=tenacity.stop_after_attempt(3), retry=tenacity.retry_if_exception_type(IOError))
+@retry(
+    stop=tenacity.stop_after_attempt(3), retry=tenacity.retry_if_exception_type(IOError)
+)
 def _retryable_test_with_exception_type_io_attempt_limit(thing):
     return thing.go()
 
 
 @retry(retry=tenacity.retry_unless_exception_type(NameError))
 def _retryable_test_with_unless_exception_type_name(thing):
     return thing.go()
@@ -871,36 +937,54 @@
 @retry(retry=tenacity.retry_unless_exception_type())
 def _retryable_test_with_unless_exception_type_no_input(thing):
     return thing.go()
 
 
 @retry(
     stop=tenacity.stop_after_attempt(5),
-    retry=tenacity.retry_if_exception_message(message=NoCustomErrorAfterCount.derived_message),
+    retry=tenacity.retry_if_exception_message(
+        message=NoCustomErrorAfterCount.derived_message
+    ),
 )
 def _retryable_test_if_exception_message_message(thing):
     return thing.go()
 
 
-@retry(retry=tenacity.retry_if_not_exception_message(message=NoCustomErrorAfterCount.derived_message))
+@retry(
+    retry=tenacity.retry_if_not_exception_message(
+        message=NoCustomErrorAfterCount.derived_message
+    )
+)
 def _retryable_test_if_not_exception_message_message(thing):
     return thing.go()
 
 
-@retry(retry=tenacity.retry_if_exception_message(match=NoCustomErrorAfterCount.derived_message[:3] + ".*"))
+@retry(
+    retry=tenacity.retry_if_exception_message(
+        match=NoCustomErrorAfterCount.derived_message[:3] + ".*"
+    )
+)
 def _retryable_test_if_exception_message_match(thing):
     return thing.go()
 
 
-@retry(retry=tenacity.retry_if_not_exception_message(match=NoCustomErrorAfterCount.derived_message[:3] + ".*"))
+@retry(
+    retry=tenacity.retry_if_not_exception_message(
+        match=NoCustomErrorAfterCount.derived_message[:3] + ".*"
+    )
+)
 def _retryable_test_if_not_exception_message_match(thing):
     return thing.go()
 
 
-@retry(retry=tenacity.retry_if_not_exception_message(message=NameErrorUntilCount.derived_message))
+@retry(
+    retry=tenacity.retry_if_not_exception_message(
+        message=NameErrorUntilCount.derived_message
+    )
+)
 def _retryable_test_not_exception_message_delay(thing):
     return thing.go()
 
 
 @retry
 def _retryable_default(thing):
     return thing.go()
@@ -942,121 +1026,170 @@
             self.assertTrue(re.last_attempt.result() is None)
             print(re)
 
     def test_with_stop_on_exception(self):
         try:
             _retryable_test_with_stop(NoIOErrorAfterCount(5))
             self.fail("Expected IOError")
-        except IOError as re:
+        except OSError as re:
             self.assertTrue(isinstance(re, IOError))
             print(re)
 
     def test_retry_if_exception_of_type(self):
         self.assertTrue(_retryable_test_with_exception_type_io(NoIOErrorAfterCount(5)))
 
         try:
             _retryable_test_with_exception_type_io(NoNameErrorAfterCount(5))
             self.fail("Expected NameError")
         except NameError as n:
             self.assertTrue(isinstance(n, NameError))
             print(n)
 
-        self.assertTrue(_retryable_test_with_exception_type_custom(NoCustomErrorAfterCount(5)))
+        self.assertTrue(
+            _retryable_test_with_exception_type_custom(NoCustomErrorAfterCount(5))
+        )
 
         try:
             _retryable_test_with_exception_type_custom(NoNameErrorAfterCount(5))
             self.fail("Expected NameError")
         except NameError as n:
             self.assertTrue(isinstance(n, NameError))
             print(n)
 
     def test_retry_except_exception_of_type(self):
-        self.assertTrue(_retryable_test_if_not_exception_type_io(NoNameErrorAfterCount(5)))
+        self.assertTrue(
+            _retryable_test_if_not_exception_type_io(NoNameErrorAfterCount(5))
+        )
 
         try:
             _retryable_test_if_not_exception_type_io(NoIOErrorAfterCount(5))
             self.fail("Expected IOError")
-        except IOError as err:
+        except OSError as err:
             self.assertTrue(isinstance(err, IOError))
             print(err)
 
     def test_retry_until_exception_of_type_attempt_number(self):
         try:
-            self.assertTrue(_retryable_test_with_unless_exception_type_name(NameErrorUntilCount(5)))
+            self.assertTrue(
+                _retryable_test_with_unless_exception_type_name(NameErrorUntilCount(5))
+            )
         except NameError as e:
             s = _retryable_test_with_unless_exception_type_name.retry.statistics
             self.assertTrue(s["attempt_number"] == 6)
             print(e)
         else:
             self.fail("Expected NameError")
 
     def test_retry_until_exception_of_type_no_type(self):
         try:
             # no input should catch all subclasses of Exception
-            self.assertTrue(_retryable_test_with_unless_exception_type_no_input(NameErrorUntilCount(5)))
+            self.assertTrue(
+                _retryable_test_with_unless_exception_type_no_input(
+                    NameErrorUntilCount(5)
+                )
+            )
         except NameError as e:
             s = _retryable_test_with_unless_exception_type_no_input.retry.statistics
             self.assertTrue(s["attempt_number"] == 6)
             print(e)
         else:
             self.fail("Expected NameError")
 
     def test_retry_until_exception_of_type_wrong_exception(self):
         try:
             # two iterations with IOError, one that returns True
-            _retryable_test_with_unless_exception_type_name_attempt_limit(IOErrorUntilCount(2))
+            _retryable_test_with_unless_exception_type_name_attempt_limit(
+                IOErrorUntilCount(2)
+            )
             self.fail("Expected RetryError")
         except RetryError as e:
             self.assertTrue(isinstance(e, RetryError))
             print(e)
 
     def test_retry_if_exception_message(self):
         try:
-            self.assertTrue(_retryable_test_if_exception_message_message(NoCustomErrorAfterCount(3)))
+            self.assertTrue(
+                _retryable_test_if_exception_message_message(NoCustomErrorAfterCount(3))
+            )
         except CustomError:
             print(_retryable_test_if_exception_message_message.retry.statistics)
             self.fail("CustomError should've been retried from errormessage")
 
     def test_retry_if_not_exception_message(self):
         try:
-            self.assertTrue(_retryable_test_if_not_exception_message_message(NoCustomErrorAfterCount(2)))
+            self.assertTrue(
+                _retryable_test_if_not_exception_message_message(
+                    NoCustomErrorAfterCount(2)
+                )
+            )
         except CustomError:
             s = _retryable_test_if_not_exception_message_message.retry.statistics
             self.assertTrue(s["attempt_number"] == 1)
 
     def test_retry_if_not_exception_message_delay(self):
         try:
-            self.assertTrue(_retryable_test_not_exception_message_delay(NameErrorUntilCount(3)))
+            self.assertTrue(
+                _retryable_test_not_exception_message_delay(NameErrorUntilCount(3))
+            )
         except NameError:
             s = _retryable_test_not_exception_message_delay.retry.statistics
             print(s["attempt_number"])
             self.assertTrue(s["attempt_number"] == 4)
 
     def test_retry_if_exception_message_match(self):
         try:
-            self.assertTrue(_retryable_test_if_exception_message_match(NoCustomErrorAfterCount(3)))
+            self.assertTrue(
+                _retryable_test_if_exception_message_match(NoCustomErrorAfterCount(3))
+            )
         except CustomError:
             self.fail("CustomError should've been retried from errormessage")
 
     def test_retry_if_not_exception_message_match(self):
         try:
-            self.assertTrue(_retryable_test_if_not_exception_message_message(NoCustomErrorAfterCount(2)))
+            self.assertTrue(
+                _retryable_test_if_not_exception_message_message(
+                    NoCustomErrorAfterCount(2)
+                )
+            )
         except CustomError:
             s = _retryable_test_if_not_exception_message_message.retry.statistics
             self.assertTrue(s["attempt_number"] == 1)
 
     def test_retry_if_exception_cause_type(self):
-        self.assertTrue(_retryable_test_with_exception_cause_type(NoNameErrorCauseAfterCount(5)))
+        self.assertTrue(
+            _retryable_test_with_exception_cause_type(NoNameErrorCauseAfterCount(5))
+        )
 
         try:
             _retryable_test_with_exception_cause_type(NoIOErrorCauseAfterCount(5))
             self.fail("Expected exception without NameError as cause")
         except NameError:
             pass
 
+    def test_retry_preserves_argument_defaults(self):
+        def function_with_defaults(a=1):
+            return a
+
+        def function_with_kwdefaults(*, a=1):
+            return a
+
+        retrying = Retrying(
+            wait=tenacity.wait_fixed(0.01), stop=tenacity.stop_after_attempt(3)
+        )
+        wrapped_defaults_function = retrying.wraps(function_with_defaults)
+        wrapped_kwdefaults_function = retrying.wraps(function_with_kwdefaults)
+
+        self.assertEqual(
+            function_with_defaults.__defaults__, wrapped_defaults_function.__defaults__
+        )
+        self.assertEqual(
+            function_with_kwdefaults.__kwdefaults__,
+            wrapped_kwdefaults_function.__kwdefaults__,
+        )
+
     def test_defaults(self):
         self.assertTrue(_retryable_default(NoNameErrorAfterCount(5)))
         self.assertTrue(_retryable_default_f(NoNameErrorAfterCount(5)))
         self.assertTrue(_retryable_default(NoCustomErrorAfterCount(5)))
         self.assertTrue(_retryable_default_f(NoCustomErrorAfterCount(5)))
 
     def test_retry_function_object(self):
@@ -1066,44 +1199,50 @@
         attribute is missing. It's fixed in Py3 but was never backported.
         """
 
         class Hello:
             def __call__(self):
                 return "Hello"
 
-        retrying = Retrying(wait=tenacity.wait_fixed(0.01), stop=tenacity.stop_after_attempt(3))
+        retrying = Retrying(
+            wait=tenacity.wait_fixed(0.01), stop=tenacity.stop_after_attempt(3)
+        )
         h = retrying.wraps(Hello())
         self.assertEqual(h(), "Hello")
 
 
 class TestRetryWith:
     def test_redefine_wait(self):
         start = current_time_ms()
-        result = _retryable_test_with_wait.retry_with(wait=tenacity.wait_fixed(0.1))(NoneReturnUntilAfterCount(5))
+        result = _retryable_test_with_wait.retry_with(wait=tenacity.wait_fixed(0.1))(
+            NoneReturnUntilAfterCount(5)
+        )
         t = current_time_ms() - start
         assert t >= 500
         assert result is True
 
     def test_redefine_stop(self):
-        result = _retryable_test_with_stop.retry_with(stop=tenacity.stop_after_attempt(5))(NoneReturnUntilAfterCount(4))
+        result = _retryable_test_with_stop.retry_with(
+            stop=tenacity.stop_after_attempt(5)
+        )(NoneReturnUntilAfterCount(4))
         assert result is True
 
     def test_retry_error_cls_should_be_preserved(self):
         @retry(stop=tenacity.stop_after_attempt(10), retry_error_cls=ValueError)
         def _retryable():
             raise Exception("raised for test purposes")
 
         with pytest.raises(Exception) as exc_ctx:
             _retryable.retry_with(stop=tenacity.stop_after_attempt(2))()
 
         assert exc_ctx.type is ValueError, "Should remap to specific exception type"
 
     def test_retry_error_callback_should_be_preserved(self):
         def return_text(retry_state):
-            return "Calling %s keeps raising errors after %s attempts" % (
+            return "Calling {} keeps raising errors after {} attempts".format(
                 retry_state.fn.__name__,
                 retry_state.attempt_number,
             )
 
         @retry(stop=tenacity.stop_after_attempt(10), retry_error_callback=return_text)
         def _retryable():
             raise Exception("raised for test purposes")
@@ -1185,15 +1324,18 @@
                 stop=tenacity.stop_after_attempt(3),
                 before_sleep=_before_sleep,
             )
             get_call_fn(retrying)(thing.go)
         finally:
             logger.removeHandler(handler)
 
-        etalon_re = r"^Retrying .* in 0\.01 seconds as it raised " r"(IO|OS)Error: Hi there, I'm an IOError\.$"
+        etalon_re = (
+            r"^Retrying .* in 0\.01 seconds as it raised "
+            r"(IO|OS)Error: Hi there, I'm an IOError\.$"
+        )
         self.assertEqual(len(handler.records), 2)
         fmt = logging.Formatter().format
         self.assertRegex(fmt(handler.records[0]), etalon_re)
         self.assertRegex(fmt(handler.records[1]), etalon_re)
 
     def test_before_sleep_log_raises(self):
         self._before_sleep_log_raises(lambda x: x)
@@ -1202,15 +1344,17 @@
         thing = NoIOErrorAfterCount(2)
         logger = logging.getLogger(self.id())
         logger.propagate = False
         logger.setLevel(logging.INFO)
         handler = CapturingHandler()
         logger.addHandler(handler)
         try:
-            _before_sleep = tenacity.before_sleep_log(logger, logging.INFO, exc_info=True)
+            _before_sleep = tenacity.before_sleep_log(
+                logger, logging.INFO, exc_info=True
+            )
             retrying = Retrying(
                 wait=tenacity.wait_fixed(0.01),
                 stop=tenacity.stop_after_attempt(3),
                 before_sleep=_before_sleep,
             )
             retrying(thing.go)
         finally:
@@ -1232,15 +1376,17 @@
         thing = NoneReturnUntilAfterCount(2)
         logger = logging.getLogger(self.id())
         logger.propagate = False
         logger.setLevel(logging.INFO)
         handler = CapturingHandler()
         logger.addHandler(handler)
         try:
-            _before_sleep = tenacity.before_sleep_log(logger, logging.INFO, exc_info=exc_info)
+            _before_sleep = tenacity.before_sleep_log(
+                logger, logging.INFO, exc_info=exc_info
+            )
             _retry = tenacity.retry_if_result(lambda result: result is None)
             retrying = Retrying(
                 wait=tenacity.wait_fixed(0.01),
                 stop=tenacity.stop_after_attempt(3),
                 retry=_retry,
                 before_sleep=_before_sleep,
             )
@@ -1515,15 +1661,17 @@
         expected = RetryError(last_attempt=123)
         pickled = pickle.dumps(expected)
         actual = pickle.loads(pickled)
         self.assertEqual(expected.last_attempt, actual.last_attempt)
 
 
 class TestRetryTyping(unittest.TestCase):
-    @pytest.mark.skipif(sys.version_info < (3, 0), reason="typeguard not supported for python 2")
+    @pytest.mark.skipif(
+        sys.version_info < (3, 0), reason="typeguard not supported for python 2"
+    )
     def test_retry_type_annotations(self):
         """The decorator should maintain types of decorated functions."""
         # Just in case this is run with unit-test, return early for py2
         if sys.version_info < (3, 0):
             return
 
         # Function-level import because we can't install this for python 2.
```

### Comparing `tenacity-8.2.3/tests/test_tornado.py` & `tenacity-8.3.0/tests/test_tornado.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# coding: utf-8
+# mypy: disable-error-code="no-untyped-def,no-untyped-call"
 # Copyright 2017 Elisey Zanko
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
@@ -34,15 +34,15 @@
 @retry(stop=stop_after_attempt(2))
 @gen.coroutine
 def _retryable_coroutine_with_2_attempts(thing):
     yield gen.sleep(0.00001)
     thing.go()
 
 
-class TestTornado(testing.AsyncTestCase):
+class TestTornado(testing.AsyncTestCase):  # type: ignore[misc]
     @testing.gen_test
     def test_retry(self):
         assert gen.is_coroutine_function(_retryable_coroutine)
         thing = NoIOErrorAfterCount(5)
         yield _retryable_coroutine(thing)
         assert thing.counter == thing.count
```

