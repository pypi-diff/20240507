# Comparing `tmp/lakefs-spec-0.8.0.post0.tar.gz` & `tmp/lakefs_spec-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakefs-spec-0.8.0.post0.tar", last modified: Wed Apr  3 10:23:13 2024, max compression
+gzip compressed data, was "lakefs_spec-0.9.0.tar", last modified: Tue May  7 08:38:06 2024, max compression
```

## Comparing `lakefs-spec-0.8.0.post0.tar` & `lakefs_spec-0.9.0.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.792932 lakefs-spec-0.8.0.post0/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.772932 lakefs-spec-0.8.0.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/ISSUE_TEMPLATE/bug-report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/ISSUE_TEMPLATE/feature-request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.772932 lakefs-spec-0.8.0.post0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/.github/actions/mike-docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/actions/mike-docs/action.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/.github/actions/python-deps/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/actions/python-deps/action.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/pull-request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/workflows/python.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-03 10:23:13.792932 lakefs-spec-0.8.0.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    14056 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/assets/lakefs-spec-logo-all.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/docs/_code/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_code/duckdb_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_code/hf_datasets_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_code/pandas_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_code/polars_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_code/pyarrow_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_code/quickstart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/aai-favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    26004 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/aai-logo-cropped.png
--rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/lakefs-spec-favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/lakefs-spec-logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    31995 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/lakefs-spec-logo-light.png
--rw-r--r--   0 runner    (1001) docker     (127)    40636 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/quickstart-lakefs-repositories.png
--rw-r--r--   0 runner    (1001) docker     (127)   123174 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/quickstart-lakefs-sample-repo.png
--rw-r--r--   0 runner    (1001) docker     (127)    32617 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/quickstart-lakefs-ui.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_scripts/gen_api_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_scripts/jupytext_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/_styles/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_styles/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)    41136 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_styles/neoteroi-mkdocs.css
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_styles/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/_theme_overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_theme_overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/_theme_overrides/partials/
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_theme_overrides/partials/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/guides/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/guides/filesystem-usage.md
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/guides/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/guides/integrations.md
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/guides/transactions.md
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/tutorials/.lakectl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/tutorials/demo_data_science_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/tutorials/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.784932 lakefs-spec-0.8.0.post0/hack/
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/hack/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.784932 lakefs-spec-0.8.0.post0/hack/config/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/hack/config/s3.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/hack/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/hack/lakefs-s3-local.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      429 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/hack/lock-deps.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:23:13.792932 lakefs-spec-0.8.0.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.772932 lakefs-spec-0.8.0.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.784932 lakefs-spec-0.8.0.post0/src/lakefs_spec/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    30309 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.788932 lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-03 10:23:13.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-03 10:23:13.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:23:13.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-03 10:23:13.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 10:23:13.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.788932 lakefs-spec-0.8.0.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.788932 lakefs-spec-0.8.0.post0/tests/smoke_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/smoke_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/smoke_tests/test_abstractfilesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/smoke_tests/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_get_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_internals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_lakefs_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_put_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_spec_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.708164 lakefs_spec-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.692164 lakefs_spec-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.692164 lakefs_spec-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/.github/ISSUE_TEMPLATE/bug-report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/.github/ISSUE_TEMPLATE/feature-request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.688164 lakefs_spec-0.9.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.692164 lakefs_spec-0.9.0/.github/actions/mike-docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/.github/actions/mike-docs/action.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.692164 lakefs_spec-0.9.0/.github/actions/python-deps/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/.github/actions/python-deps/action.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/.github/pull-request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.692164 lakefs_spec-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/.github/workflows/python.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-07 08:38:06.704164 lakefs_spec-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.692164 lakefs_spec-0.9.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    14056 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/assets/lakefs-spec-logo-all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.692164 lakefs_spec-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.692164 lakefs_spec-0.9.0/docs/_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_code/duckdb_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_code/hf_datasets_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_code/pandas_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_code/polars_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_code/pyarrow_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_code/quickstart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.696164 lakefs_spec-0.9.0/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_images/aai-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26004 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_images/aai-logo-cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_images/lakefs-spec-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_images/lakefs-spec-logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31995 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_images/lakefs-spec-logo-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40636 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_images/quickstart-lakefs-repositories.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123174 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_images/quickstart-lakefs-sample-repo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32617 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_images/quickstart-lakefs-ui.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.696164 lakefs_spec-0.9.0/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_scripts/gen_api_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_scripts/jupytext_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.696164 lakefs_spec-0.9.0/docs/_styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_styles/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)    41136 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_styles/neoteroi-mkdocs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_styles/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.696164 lakefs_spec-0.9.0/docs/_theme_overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_theme_overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.696164 lakefs_spec-0.9.0/docs/_theme_overrides/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/_theme_overrides/partials/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.696164 lakefs_spec-0.9.0/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/guides/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/guides/filesystem-usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/guides/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/guides/integrations.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/guides/transactions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.696164 lakefs_spec-0.9.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/tutorials/.lakectl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/tutorials/demo_data_science_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/docs/tutorials/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.700164 lakefs_spec-0.9.0/hack/
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/hack/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.700164 lakefs_spec-0.9.0/hack/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/hack/config/s3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/hack/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/hack/lakefs-s3-local.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      453 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/hack/lock-deps.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:38:06.708164 lakefs_spec-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.688164 lakefs_spec-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.700164 lakefs_spec-0.9.0/src/lakefs_spec/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/src/lakefs_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/src/lakefs_spec/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/src/lakefs_spec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    29593 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/src/lakefs_spec/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/src/lakefs_spec/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/src/lakefs_spec/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.704164 lakefs_spec-0.9.0/src/lakefs_spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-07 08:38:06.000000 lakefs_spec-0.9.0/src/lakefs_spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-07 08:38:06.000000 lakefs_spec-0.9.0/src/lakefs_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:38:06.000000 lakefs_spec-0.9.0/src/lakefs_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-07 08:38:06.000000 lakefs_spec-0.9.0/src/lakefs_spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 08:38:06.000000 lakefs_spec-0.9.0/src/lakefs_spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.704164 lakefs_spec-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:38:06.704164 lakefs_spec-0.9.0/tests/smoke_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/smoke_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/smoke_tests/test_abstractfilesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/smoke_tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_get_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_lakefs_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_put_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_spec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-07 08:37:09.000000 lakefs_spec-0.9.0/tests/util.py
```

### Comparing `lakefs-spec-0.8.0.post0/.github/ISSUE_TEMPLATE/bug-report.yaml` & `lakefs_spec-0.9.0/.github/ISSUE_TEMPLATE/bug-report.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/.github/ISSUE_TEMPLATE/feature-request.yaml` & `lakefs_spec-0.9.0/.github/ISSUE_TEMPLATE/feature-request.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/.github/actions/mike-docs/action.yaml` & `lakefs_spec-0.9.0/.github/actions/mike-docs/action.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/.github/actions/python-deps/action.yaml` & `lakefs_spec-0.9.0/.github/actions/python-deps/action.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/.github/workflows/python.yaml` & `lakefs_spec-0.9.0/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/.github/workflows/release.yaml` & `lakefs_spec-0.9.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/.gitignore` & `lakefs_spec-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/.pre-commit-config.yaml` & `lakefs_spec-0.9.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 default_language_version:
   python: python3.11
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-json
       - id: check-toml
       - id: check-yaml
         exclude: "mkdocs.yml"
       - id: end-of-file-fixer
       - id: mixed-line-ending
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       # See https://github.com/pre-commit/mirrors-mypy/blob/main/.pre-commit-hooks.yaml
       - id: mypy
         types_or: [python, pyi]
         args: [--ignore-missing-imports, --scripts-are-modules]
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.4.3
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
   - repo: https://github.com/PyCQA/bandit
     rev: 1.7.8
     hooks:
       - id: bandit
         args: [-c, pyproject.toml]
         additional_dependencies: ["bandit[toml]"]
   - repo: https://github.com/jsh9/pydoclint
     rev: 0.4.1
     hooks:
       - id: pydoclint
-  - repo: https://github.com/jazzband/pip-tools
-    rev: 7.4.1
+  - repo: https://github.com/astral-sh/uv-pre-commit
+    rev: 0.1.39
     hooks:
       - id: pip-compile
         name: pip-compile requirements-dev.txt
         args:
           - --no-annotate
+          - --no-strip-extras
           - --extra=dev
           - --output-file=requirements-dev.txt
           - pyproject.toml
         files: ^(pyproject\.toml|requirements-dev\.txt)$
       - id: pip-compile
         name: pip-compile requirements-docs.txt
         args:
           - --no-annotate
+          - --no-strip-extras
           - --extra=docs
           - --output-file=requirements-docs.txt
           - pyproject.toml
         files: ^(pyproject\.toml|requirements-docs\.txt)$
```

### Comparing `lakefs-spec-0.8.0.post0/CONTRIBUTING.md` & `lakefs_spec-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/LICENSE` & `lakefs_spec-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/PKG-INFO` & `lakefs_spec-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs-spec
-Version: 0.8.0.post0
+Version: 0.9.0
 Summary: An fsspec implementation for lakeFS.
 Author-email: appliedAI Institute for Europe <lakefs-spec@appliedai-institute.de>
 Maintainer-email: Nicholas Junge <n.junge@appliedai-institute.de>, Max Mynter <m.mynter@appliedai-institute.de>, Adrian Rumpold <a.rumpold@appliedai-institute.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/aai-institute/lakefs-spec
 Project-URL: Repository, https://github.com/aai-institute/lakefs-spec.git
 Project-URL: Issues, https://github.com/aai-institute/lakefs-spec/issues
@@ -24,25 +24,25 @@
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fsspec>=2023.6.0
+Requires-Dist: fsspec>=2023.12.0
 Requires-Dist: lakefs>=0.2.0
 Provides-Extra: dev
 Requires-Dist: build>=0.10.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.3; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: pydoclint; extra == "dev"
 Requires-Dist: pandas[parquet]; extra == "dev"
 Requires-Dist: polars; extra == "dev"
-Requires-Dist: duckdb; extra == "dev"
+Requires-Dist: duckdb<=0.10.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-callouts; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
 Requires-Dist: mkdocs-literate-nav; extra == "docs"
 Requires-Dist: mkdocs-section-index; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
```

### Comparing `lakefs-spec-0.8.0.post0/README.md` & `lakefs_spec-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/assets/lakefs-spec-logo-all.svg` & `lakefs_spec-0.9.0/assets/lakefs-spec-logo-all.svg`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/CONTRIBUTING.md` & `lakefs_spec-0.9.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_code/pyarrow_example.py` & `lakefs_spec-0.9.0/docs/_code/pyarrow_example.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_code/quickstart.py` & `lakefs_spec-0.9.0/docs/_code/quickstart.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_images/aai-favicon.png` & `lakefs_spec-0.9.0/docs/_images/aai-favicon.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_images/aai-logo-cropped.png` & `lakefs_spec-0.9.0/docs/_images/aai-logo-cropped.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_images/lakefs-spec-favicon.png` & `lakefs_spec-0.9.0/docs/_images/lakefs-spec-favicon.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_images/lakefs-spec-logo-dark.png` & `lakefs_spec-0.9.0/docs/_images/lakefs-spec-logo-dark.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_images/lakefs-spec-logo-light.png` & `lakefs_spec-0.9.0/docs/_images/lakefs-spec-logo-light.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_images/quickstart-lakefs-repositories.png` & `lakefs_spec-0.9.0/docs/_images/quickstart-lakefs-repositories.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_images/quickstart-lakefs-sample-repo.png` & `lakefs_spec-0.9.0/docs/_images/quickstart-lakefs-sample-repo.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_images/quickstart-lakefs-ui.png` & `lakefs_spec-0.9.0/docs/_images/quickstart-lakefs-ui.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_scripts/gen_api_ref_pages.py` & `lakefs_spec-0.9.0/docs/_scripts/gen_api_ref_pages.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_scripts/jupytext_convert.py` & `lakefs_spec-0.9.0/docs/_scripts/jupytext_convert.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_styles/extra.css` & `lakefs_spec-0.9.0/docs/_styles/extra.css`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_styles/neoteroi-mkdocs.css` & `lakefs_spec-0.9.0/docs/_styles/neoteroi-mkdocs.css`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_styles/theme.css` & `lakefs_spec-0.9.0/docs/_styles/theme.css`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/_theme_overrides/partials/header.html` & `lakefs_spec-0.9.0/docs/_theme_overrides/partials/header.html`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/guides/configuration.md` & `lakefs_spec-0.9.0/docs/guides/configuration.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/guides/filesystem-usage.md` & `lakefs_spec-0.9.0/docs/guides/filesystem-usage.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/guides/index.md` & `lakefs_spec-0.9.0/docs/guides/index.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/guides/integrations.md` & `lakefs_spec-0.9.0/docs/guides/integrations.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/guides/transactions.md` & `lakefs_spec-0.9.0/docs/guides/transactions.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/index.md` & `lakefs_spec-0.9.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/docs/quickstart.md` & `lakefs_spec-0.9.0/docs/quickstart.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Quickstart
 
 Welcome! This quickstart guide will get you up and running with lakeFS-spec by showing you how to
 
-1. [install the `lakefs-spec` package](#installing),
+1. [install the `lakefs-spec` package](#installing-lakefs-spec),
 1. [spin up a local lakeFS server](#spinning-up-a-local-lakefs-instance),
 1. [create a lakeFS repository for experimentation](#create-a-lakefs-repository), and
-1. [perform basic file system operations](#using-the-lakefs-fsspec-file-system)
+1. [perform basic file system operations](#using-the-lakefs-file-system)
 in a lakeFS repository using lakeFS-spec.
 
 ??? info "Prerequisites"
 
     To follow along with this guide, you will need a few prerequisites ready on your machine:
 
     - lakeFS-spec supports Windows, macOS, or Linux
```

### Comparing `lakefs-spec-0.8.0.post0/docs/tutorials/demo_data_science_project.py` & `lakefs_spec-0.9.0/docs/tutorials/demo_data_science_project.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/hack/README.md` & `lakefs_spec-0.9.0/hack/README.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/hack/docker-compose.yml` & `lakefs_spec-0.9.0/hack/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/hack/lakefs-s3-local.yml` & `lakefs_spec-0.9.0/hack/lakefs-s3-local.yml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/mkdocs.yml` & `lakefs_spec-0.9.0/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,16 @@
           - Remove_input
   - mike:
       canonical_version: latest
   - privacy
   - search:
   - git-revision-date-localized:
       type: iso_date
+      strict: false
+      fallback_to_build_date: true
   - include_dir_to_nav:
       file_pattern: '.*\.(md|ipynb)$'
 
 markdown_extensions:
   - neoteroi.cards  # https://www.neoteroi.dev/mkdocs-plugins/cards/
   # python-markdown extensions: https://python-markdown.github.io/extensions/
   - admonition
```

#### html2text {}

```diff
@@ -21,35 +21,36 @@
 mknotebooks: execute: true # https://github.com/greenape/mknotebooks/blob/
 master/examples/cell_tag_remove/mkdocs.yml # See the following for how to add
 the tags to cells: https://jupyterbook.org/en/stable/content/
 metadata.html#jupyter-cell-tags tag_remove_configs: remove_cell_tags: -
 Remove_cell remove_all_outputs_tags: - Remove_all_output
 remove_single_output_tags: - Remove_single_output remove_input_tags: -
 Remove_input - mike: canonical_version: latest - privacy - search: - git-
-revision-date-localized: type: iso_date - include_dir_to_nav: file_pattern:
-'.*\.(md|ipynb)$' markdown_extensions: - neoteroi.cards # https://
-www.neoteroi.dev/mkdocs-plugins/cards/ # python-markdown extensions: https://
-python-markdown.github.io/extensions/ - admonition - attr_list - sane_lists -
-toc: permalink: true toc_depth: 3 # pymdown-extensions: https://
-facelessuser.github.io/pymdown-extensions/ - pymdownx.details - pymdownx.emoji:
-emoji_index: !!python/name:material.extensions.emoji.twemoji emoji_generator:
-!!python/name:material.extensions.emoji.to_svg - pymdownx.highlight:
-anchor_linenums: true line_spans: __span pygments_lang_class: true -
-pymdownx.inlinehilite - pymdownx.snippets: url_download: true -
-pymdownx.superfences - pymdownx.tabbed: alternate_style: true theme: name:
-"material" custom_dir: docs/_theme_overrides logo: _images/aai-logo-cropped.png
-favicon: _images/lakefs-spec-favicon.png font: text: IBM Plex Sans # Arial
-replacement code: Source Code Pro icon: logo: _images/aai-favicon.png repo:
-fontawesome/brands/github features: - content.tabs.link - content.code.copy -
-content.code.annotate - content.action.edit palette: # Palette toggle for light
-mode - scheme: aai-light toggle: icon: material/brightness-7 name: Switch to
-dark mode # Palette toggle for dark mode - scheme: slate toggle: icon:
-material/brightness-4 name: Switch to light mode extra: copyright_link: https:/
-/appliedai-institute.de homepage: https://lakefs-spec.org generator: false
-pre_release: !ENV [DOCS_PRERELEASE, false] version: provider: mike default:
-latest social: - icon: fontawesome/brands/github link: https://github.com/aai-
-institute/lakefs-spec - icon: fontawesome/brands/python link: https://pypi.org/
-project/lakefs-spec - icon: fontawesome/brands/linkedin link: https://
-www.linkedin.com/company/appliedai-institute-for-europe-ggmbh/ - icon:
-fontawesome/solid/section link: https://appliedai-institute.de/impressum name:
-Impressum / Imprint extra_css: - _styles/extra.css - _styles/theme.css -
-_styles/neoteroi-mkdocs.css
+revision-date-localized: type: iso_date strict: false fallback_to_build_date:
+true - include_dir_to_nav: file_pattern: '.*\.(md|ipynb)$' markdown_extensions:
+- neoteroi.cards # https://www.neoteroi.dev/mkdocs-plugins/cards/ # python-
+markdown extensions: https://python-markdown.github.io/extensions/ - admonition
+- attr_list - sane_lists - toc: permalink: true toc_depth: 3 # pymdown-
+extensions: https://facelessuser.github.io/pymdown-extensions/ -
+pymdownx.details - pymdownx.emoji: emoji_index: !!python/name:
+material.extensions.emoji.twemoji emoji_generator: !!python/name:
+material.extensions.emoji.to_svg - pymdownx.highlight: anchor_linenums: true
+line_spans: __span pygments_lang_class: true - pymdownx.inlinehilite -
+pymdownx.snippets: url_download: true - pymdownx.superfences - pymdownx.tabbed:
+alternate_style: true theme: name: "material" custom_dir: docs/_theme_overrides
+logo: _images/aai-logo-cropped.png favicon: _images/lakefs-spec-favicon.png
+font: text: IBM Plex Sans # Arial replacement code: Source Code Pro icon: logo:
+_images/aai-favicon.png repo: fontawesome/brands/github features: -
+content.tabs.link - content.code.copy - content.code.annotate -
+content.action.edit palette: # Palette toggle for light mode - scheme: aai-
+light toggle: icon: material/brightness-7 name: Switch to dark mode # Palette
+toggle for dark mode - scheme: slate toggle: icon: material/brightness-4 name:
+Switch to light mode extra: copyright_link: https://appliedai-institute.de
+homepage: https://lakefs-spec.org generator: false pre_release: !ENV
+[DOCS_PRERELEASE, false] version: provider: mike default: latest social: -
+icon: fontawesome/brands/github link: https://github.com/aai-institute/lakefs-
+spec - icon: fontawesome/brands/python link: https://pypi.org/project/lakefs-
+spec - icon: fontawesome/brands/linkedin link: https://www.linkedin.com/
+company/appliedai-institute-for-europe-ggmbh/ - icon: fontawesome/solid/section
+link: https://appliedai-institute.de/impressum name: Impressum / Imprint
+extra_css: - _styles/extra.css - _styles/theme.css - _styles/neoteroi-
+mkdocs.css
```

### Comparing `lakefs-spec-0.8.0.post0/pyproject.toml` & `lakefs_spec-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Version Control",
     "Topic :: System :: Filesystems",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 
-dependencies = ["fsspec>=2023.6.0", "lakefs>=0.2.0"]
+dependencies = ["fsspec>=2023.12.0", "lakefs>=0.2.0"]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/aai-institute/lakefs-spec"
 Repository = "https://github.com/aai-institute/lakefs-spec.git"
 Issues = "https://github.com/aai-institute/lakefs-spec/issues"
@@ -51,15 +51,15 @@
     "pre-commit>=3.3.3",
     "pytest>=7.4.0",
     "pytest-cov>=4.1.0",
     "pydoclint",
     # for integration tests.
     "pandas[parquet]",
     "polars",
-    "duckdb",
+    "duckdb<=0.10.0",  # due to https://github.com/duckdb/duckdb/issues/11875
 ]
 docs = [
     "mkdocs",
     "mkdocs-callouts",
     "mkdocs-gen-files",
     "mkdocs-literate-nav",
     "mkdocs-section-index",
```

### Comparing `lakefs-spec-0.8.0.post0/requirements-dev.txt` & `lakefs_spec-0.9.0/requirements-dev.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,41 @@
-#
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
-#
-#    pip-compile --extra=dev --no-annotate --output-file=requirements-dev.txt pyproject.toml
-#
+# This file was autogenerated by uv via the following command:
+#    uv pip compile --no-annotate --no-strip-extras --extra=dev --output-file=requirements-dev.txt pyproject.toml
 aenum==3.1.15
-build==1.0.3
+annotated-types==0.6.0
+build==1.2.1
 cfgv==3.4.0
 click==8.1.7
-coverage[toml]==7.4.1
+coverage[toml]==7.5.1
 distlib==0.3.8
 docstring-parser-fork==0.0.5
-duckdb==0.9.2
-filelock==3.13.1
-fsspec==2024.2.0
-identify==2.5.33
+duckdb==0.10.0
+filelock==3.14.0
+fsspec==2024.3.1
+identify==2.5.36
 iniconfig==2.0.0
-lakefs==0.3.0
-lakefs-sdk==1.9.1
+lakefs==0.6.0
+lakefs-sdk==1.21.0
 nodeenv==1.8.0
-numpy==1.26.3
-packaging==23.2
-pandas[parquet]==2.2.0
-platformdirs==4.2.0
-pluggy==1.4.0
-polars==0.20.7
-pre-commit==3.6.0
-pyarrow==15.0.0
-pydantic==1.10.14
-pydoclint==0.3.9
-pyproject-hooks==1.0.0
-pytest==8.0.0
-pytest-cov==4.1.0
-python-dateutil==2.8.2
+numpy==1.26.4
+packaging==24.0
+pandas[parquet]==2.2.2
+platformdirs==4.2.1
+pluggy==1.5.0
+polars==0.20.23
+pre-commit==3.7.0
+pyarrow==16.0.0
+pydantic==2.7.1
+pydantic-core==2.18.2
+pydoclint==0.4.1
+pyproject-hooks==1.1.0
+pytest==8.2.0
+pytest-cov==5.0.0
+python-dateutil==2.9.0.post0
 pytz==2024.1
 pyyaml==6.0.1
+setuptools==68.2.2
 six==1.16.0
-typing-extensions==4.9.0
-tzdata==2023.4
+typing-extensions==4.11.0
+tzdata==2024.1
 urllib3==2.0.7
-virtualenv==20.25.0
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
+virtualenv==20.26.1
```

### Comparing `lakefs-spec-0.8.0.post0/requirements-docs.txt` & `lakefs_spec-0.9.0/requirements-docs.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,159 +1,155 @@
-#
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
-#
-#    pip-compile --extra=docs --no-annotate --output-file=requirements-docs.txt pyproject.toml
-#
+# This file was autogenerated by uv via the following command:
+#    uv pip compile --no-annotate --no-strip-extras --extra=docs --output-file=requirements-docs.txt pyproject.toml
 aenum==3.1.15
-anyio==4.2.0
-appnope==0.1.3
+annotated-types==0.6.0
+anyio==4.3.0
+appnope==0.1.4
 argon2-cffi==23.1.0
 argon2-cffi-bindings==21.2.0
 arrow==1.3.0
 asttokens==2.4.1
 async-lru==2.0.4
 attrs==23.2.0
-babel==2.14.0
+babel==2.15.0
 beautifulsoup4==4.12.3
-black==24.3.0
+black==24.4.2
 bleach==6.1.0
 certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
-comm==0.2.1
-debugpy==1.8.0
+comm==0.2.2
+debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
 docstring-parser==0.16
 essentials==1.1.5
 essentials-openapi==1.0.9
 executing==2.0.1
 fastjsonschema==2.19.1
 fqdn==1.5.1
-fsspec==2024.2.0
+fsspec==2024.3.1
 ghp-import==2.1.0
 gitdb==4.0.11
-gitpython==3.1.41
-griffe==0.40.0
+gitpython==3.1.43
+griffe==0.44.0
 h11==0.14.0
-httpcore==1.0.2
-httpx==0.26.0
-idna==3.6
-importlib-metadata==7.0.1
-importlib-resources==6.1.1
-ipykernel==6.29.0
-ipython==8.21.0
-ipywidgets==8.1.1
+httpcore==1.0.5
+httpx==0.27.0
+idna==3.7
+importlib-metadata==7.1.0
+importlib-resources==6.4.0
+ipykernel==6.29.4
+ipython==8.24.0
+ipywidgets==8.1.2
 isoduration==20.11.0
 jedi==0.19.1
-jinja2==3.1.3
-json5==0.9.14
+jinja2==3.1.4
+json5==0.9.25
 jsonpointer==2.4
-jsonschema[format-nongpl]==4.21.1
+jsonschema[format-nongpl]==4.22.0
 jsonschema-specifications==2023.12.1
 jupyter==1.0.0
-jupyter-client==8.6.0
+jupyter-client==8.6.1
 jupyter-console==6.6.3
-jupyter-core==5.7.1
-jupyter-events==0.9.0
-jupyter-lsp==2.2.2
-jupyter-server==2.12.5
-jupyter-server-terminals==0.5.2
-jupyterlab==4.1.0
+jupyter-core==5.7.2
+jupyter-events==0.10.0
+jupyter-lsp==2.2.5
+jupyter-server==2.14.0
+jupyter-server-terminals==0.5.3
+jupyterlab==4.1.8
 jupyterlab-pygments==0.3.0
-jupyterlab-server==2.25.2
-jupyterlab-widgets==3.0.9
-jupytext==1.16.1
-lakefs==0.3.0
-lakefs-sdk==1.9.1
-markdown==3.5.2
+jupyterlab-server==2.27.1
+jupyterlab-widgets==3.0.10
+jupytext==1.16.2
+lakefs==0.6.0
+lakefs-sdk==1.21.0
+markdown==3.6
 markdown-it-py==3.0.0
 markupsafe==2.1.5
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
 mdit-py-plugins==0.4.0
 mdurl==0.1.2
 mergedeep==1.3.4
-mike==2.0.0
+mike==2.1.1
 mistune==3.0.2
-mkdocs==1.5.3
-mkdocs-autorefs==0.5.0
-mkdocs-callouts==1.10.0
+mkdocs==1.6.0
+mkdocs-autorefs==1.0.1
+mkdocs-callouts==1.13.2
 mkdocs-gen-files==0.5.0
-mkdocs-git-revision-date-localized-plugin==1.2.4
+mkdocs-get-deps==0.2.0
+mkdocs-git-revision-date-localized-plugin==1.2.5
 mkdocs-include-dir-to-nav==1.2.0
 mkdocs-literate-nav==0.6.1
-mkdocs-material==9.5.7
+mkdocs-material==9.5.21
 mkdocs-material-extensions==1.3.1
-mkdocs-section-index==0.3.8
-mkdocstrings[python]==0.24.0
-mkdocstrings-python==1.8.0
+mkdocs-section-index==0.3.9
+mkdocstrings[python]==0.25.1
+mkdocstrings-python==1.10.0
 mknotebooks==0.8.0
 mypy-extensions==1.0.0
-nbclient==0.9.0
-nbconvert==7.14.2
-nbformat==5.9.2
+nbclient==0.10.0
+nbconvert==7.16.4
+nbformat==5.10.4
 neoteroi-mkdocs==1.0.5
 nest-asyncio==1.6.0
-notebook==7.0.7
-notebook-shim==0.2.3
+notebook==7.1.3
+notebook-shim==0.2.4
 overrides==7.7.0
-packaging==23.2
+packaging==24.0
 paginate==0.5.6
 pandocfilters==1.5.1
-parso==0.8.3
+parso==0.8.4
 pathspec==0.12.1
 pexpect==4.9.0
-platformdirs==4.2.0
-prometheus-client==0.19.0
+platformdirs==4.2.1
+prometheus-client==0.20.0
 prompt-toolkit==3.0.43
 psutil==5.9.8
 ptyprocess==0.7.0
 pure-eval==0.2.2
-pycparser==2.21
-pydantic==1.10.14
-pygments==2.17.2
-pymdown-extensions==10.7
-pyparsing==3.1.1
-python-dateutil==2.8.2
+pycparser==2.22
+pydantic==2.7.1
+pydantic-core==2.18.2
+pygments==2.18.0
+pymdown-extensions==10.8.1
+pyparsing==3.1.2
+python-dateutil==2.9.0.post0
 python-json-logger==2.0.7
 pytz==2024.1
 pyyaml==6.0.1
 pyyaml-env-tag==0.1
-pyzmq==25.1.2
-qtconsole==5.5.1
+pyzmq==26.0.3
+qtconsole==5.5.2
 qtpy==2.4.1
-referencing==0.33.0
-regex==2023.12.25
+referencing==0.35.1
+regex==2024.4.28
 requests==2.31.0
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
-rich==13.7.0
-rpds-py==0.17.1
-send2trash==1.8.2
+rich==13.7.1
+rpds-py==0.18.1
+send2trash==1.8.3
+setuptools==68.2.2
 six==1.16.0
 smmap==5.0.1
-sniffio==1.3.0
+sniffio==1.3.1
 soupsieve==2.5
 stack-data==0.6.3
-terminado==0.18.0
-tinycss2==1.2.1
-toml==0.10.2
+terminado==0.18.1
+tinycss2==1.3.0
 tornado==6.4
-traitlets==5.14.1
-types-python-dateutil==2.8.19.20240106
-typing-extensions==4.9.0
+traitlets==5.14.3
+types-python-dateutil==2.9.0.20240316
+typing-extensions==4.11.0
 uri-template==1.3.0
 urllib3==2.0.7
 verspec==0.1.0
-watchdog==3.0.0
+watchdog==4.0.0
 wcwidth==0.2.13
 webcolors==1.13
 webencodings==0.5.1
-websocket-client==1.7.0
-widgetsnbextension==4.0.9
-zipp==3.17.0
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
+websocket-client==1.8.0
+widgetsnbextension==4.0.10
+zipp==3.18.1
```

### Comparing `lakefs-spec-0.8.0.post0/src/lakefs_spec/errors.py` & `lakefs_spec-0.9.0/src/lakefs_spec/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,19 @@
     OSError
         A builtin Python exception ready to be thrown.
     """
     status = error.status_code
 
     if hasattr(error, "body"):
         # error has a JSON response body attached
-        reason = error.body["message"]
+        reason = error.body.get("message", "")
     else:
         reason = error.reason
 
-    emsg = f"{status} {reason}"
+    emsg = f"{status} {reason}".rstrip()
     if rpath:
         emsg += f": {rpath!r}"
 
     constructor = HTTP_CODE_TO_ERROR.get(status, partial(IOError, errno.EIO))
     custom_exc = constructor(message or emsg)
 
     if set_cause:
```

### Comparing `lakefs-spec-0.8.0.post0/src/lakefs_spec/spec.py` & `lakefs_spec-0.9.0/src/lakefs_spec/spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     source_branch: str
         Source branch set as origin when a new branch is implicitly created.
     **storage_options: Any
         Configuration options to pass to the file system's directory cache.
     """
 
     protocol = "lakefs"
+    transaction_type = LakeFSTransaction
 
     def __init__(
         self,
         host: str | None = None,
         username: str | None = None,
         password: str | None = None,
         api_key: str | None = None,
@@ -131,33 +132,14 @@
         if isinstance(path, list):
             return [cls._strip_protocol(p) for p in path]
         spath = super()._strip_protocol(path)
         if stringify_path(path).endswith("/"):
             return spath + "/"
         return spath
 
-    @property
-    def transaction(self) -> LakeFSTransaction:
-        """
-        A context manager within which file uploads and versioning operations are deferred to a
-        queue, and carried out during when exiting the context.
-
-        Requires the file class to implement ``.commit()`` and ``.discard()`` for the normal and exception cases.
-        """
-        self._transaction: LakeFSTransaction | None
-        if self._transaction is None:
-            self._transaction = LakeFSTransaction(self)
-        return self._transaction
-
-    def start_transaction(self):
-        raise NotImplementedError(
-            "lakeFS transactions should only be used as a context manager via"
-            " `with LakeFSFileSystem.transaction as tx:`"
-        )
-
     @contextmanager
     def wrapped_api_call(
         self, rpath: str | None = None, message: str | None = None, set_cause: bool = True
     ) -> Generator[None, None, None]:
         """
         A context manager to wrap lakeFS API calls, translating any API errors to Python-native OS errors.
```

### Comparing `lakefs-spec-0.8.0.post0/src/lakefs_spec/transaction.py` & `lakefs_spec-0.9.0/src/lakefs_spec/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,15 @@
 
     Parameters
     ----------
     fs: LakeFSFileSystem
         The lakeFS file system associated with the transaction.
     """
 
-    def __init__(
-        self,
-        fs: "LakeFSFileSystem",
-    ):
+    def __init__(self, fs: "LakeFSFileSystem"):
         super().__init__(fs=fs)
         self.fs: "LakeFSFileSystem"
         self.files: deque[ObjectWriter] = deque(self.files)
 
         self.repository: str | None = None
         self.base_branch: Branch | None = None
         self.automerge: bool = False
```

### Comparing `lakefs-spec-0.8.0.post0/src/lakefs_spec/util.py` & `lakefs_spec-0.9.0/src/lakefs_spec/util.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/PKG-INFO` & `lakefs_spec-0.9.0/src/lakefs_spec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs-spec
-Version: 0.8.0.post0
+Version: 0.9.0
 Summary: An fsspec implementation for lakeFS.
 Author-email: appliedAI Institute for Europe <lakefs-spec@appliedai-institute.de>
 Maintainer-email: Nicholas Junge <n.junge@appliedai-institute.de>, Max Mynter <m.mynter@appliedai-institute.de>, Adrian Rumpold <a.rumpold@appliedai-institute.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/aai-institute/lakefs-spec
 Project-URL: Repository, https://github.com/aai-institute/lakefs-spec.git
 Project-URL: Issues, https://github.com/aai-institute/lakefs-spec/issues
@@ -24,25 +24,25 @@
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fsspec>=2023.6.0
+Requires-Dist: fsspec>=2023.12.0
 Requires-Dist: lakefs>=0.2.0
 Provides-Extra: dev
 Requires-Dist: build>=0.10.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.3; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: pydoclint; extra == "dev"
 Requires-Dist: pandas[parquet]; extra == "dev"
 Requires-Dist: polars; extra == "dev"
-Requires-Dist: duckdb; extra == "dev"
+Requires-Dist: duckdb<=0.10.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-callouts; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
 Requires-Dist: mkdocs-literate-nav; extra == "docs"
 Requires-Dist: mkdocs-section-index; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
```

### Comparing `lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/SOURCES.txt` & `lakefs_spec-0.9.0/src/lakefs_spec.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .editorconfig
 .git-blame-ignore-revs
 .gitignore
 .pre-commit-config.yaml
 CONTRIBUTING.md
 LICENSE
 README.md
+codecov.yml
 mkdocs.yml
 pyproject.toml
 requirements-dev.txt
 requirements-docs.txt
 .github/pull-request.md
 .github/ISSUE_TEMPLATE/bug-report.yaml
 .github/ISSUE_TEMPLATE/config.yml
```

### Comparing `lakefs-spec-0.8.0.post0/tests/conftest.py` & `lakefs_spec-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/smoke_tests/test_abstractfilesystem.py` & `lakefs_spec-0.9.0/tests/smoke_tests/test_abstractfilesystem.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/smoke_tests/test_integrations.py` & `lakefs_spec-0.9.0/tests/smoke_tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/test_checksum.py` & `lakefs_spec-0.9.0/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/test_copy.py` & `lakefs_spec-0.9.0/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/test_errors.py` & `lakefs_spec-0.9.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/test_exists.py` & `lakefs_spec-0.9.0/tests/test_exists.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/test_fs.py` & `lakefs_spec-0.9.0/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/test_get_file.py` & `lakefs_spec-0.9.0/tests/test_get_file.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/test_info.py` & `lakefs_spec-0.9.0/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/test_internals.py` & `lakefs_spec-0.9.0/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/test_lakefs_file.py` & `lakefs_spec-0.9.0/tests/test_lakefs_file.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/test_ls.py` & `lakefs_spec-0.9.0/tests/test_ls.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/test_put_file.py` & `lakefs_spec-0.9.0/tests/test_put_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     assert non_existing_branch in list_branchnames(repository)
     # branch has been created at this point
     repository.branch(non_existing_branch).delete()
 
     fs.create_branch_ok = False
     another_non_existing_branch = "non-existing-" + "".join(random.choices(string.digits, k=8))
-    with pytest.raises(FileNotFoundError, match="Not Found: .*"):
+    with pytest.raises(FileNotFoundError):
         put_random_file_on_branch(random_file_factory, fs, repository, another_non_existing_branch)
 
 
 def test_put_client_caching(
     random_file_factory: RandomFileFactory,
     fs: LakeFSFileSystem,
     repository: Repository,
```

### Comparing `lakefs-spec-0.8.0.post0/tests/test_rm.py` & `lakefs_spec-0.9.0/tests/test_rm.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/test_spec_utils.py` & `lakefs_spec-0.9.0/tests/test_spec_utils.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/test_transactions.py` & `lakefs_spec-0.9.0/tests/test_transactions.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0.post0/tests/util.py` & `lakefs_spec-0.9.0/tests/util.py`

 * *Files identical despite different names*

