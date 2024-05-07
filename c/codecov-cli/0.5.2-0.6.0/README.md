# Comparing `tmp/codecov-cli-0.5.2.tar.gz` & `tmp/codecov-cli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecov-cli-0.5.2.tar", last modified: Wed Apr 17 16:24:37 2024, max compression
+gzip compressed data, was "codecov-cli-0.6.0.tar", last modified: Tue May  7 17:44:16 2024, max compression
```

## Comparing `codecov-cli-0.5.2.tar` & `codecov-cli-0.6.0.tar`

### file list

```diff
@@ -1,124 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.654361 codecov-cli-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-04-17 16:24:37.654361 codecov-cli-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18631 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.630361 codecov-cli-0.5.2/codecov_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.634361 codecov-cli-0.5.2/codecov_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/commands/base_picking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/commands/create_report_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/commands/empty_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/commands/get_report_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/commands/labelanalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/commands/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/commands/send_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/commands/staticanalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/commands/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/commands/upload_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/fallbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.634361 codecov-cli-0.5.2/codecov_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.638361 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/appveyor_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/azure_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/bitbucket_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/bitrise_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/buildkite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/circleci.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/cirrus_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/codebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/droneci.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/heroku.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/local.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/teamcity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/travis_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/woodpeckerci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/folder_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/git.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.638361 codecov-cli-0.5.2/codecov_cli/helpers/git_services/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/git_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/git_services/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/helpers/versioning_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.638361 codecov-cli-0.5.2/codecov_cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/plugins/compress_pycoverage_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/plugins/gcov.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/plugins/pycoverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/plugins/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/plugins/xcode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.638361 codecov-cli-0.5.2/codecov_cli/runners/
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/runners/dan_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/runners/pytest_standard_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/runners/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.638361 codecov-cli-0.5.2/codecov_cli/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.642361 codecov-cli-0.5.2/codecov_cli/services/commit/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/commit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/commit/base_picking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.642361 codecov-cli-0.5.2/codecov_cli/services/empty_upload/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/empty_upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.642361 codecov-cli-0.5.2/codecov_cli/services/report/
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.642361 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/
--rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.642361 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/general.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.642361 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/javascript_es6/
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/javascript_es6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/javascript_es6/node_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.642361 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/python/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/finders.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/staticanalysis/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.642361 codecov-cli-0.5.2/codecov_cli/services/upload/
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/upload/file_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/upload/legacy_upload_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/upload/network_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/upload/upload_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/upload/upload_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.642361 codecov-cli-0.5.2/codecov_cli/services/upload_completion/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/services/upload_completion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/codecov_cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.634361 codecov-cli-0.5.2/codecov_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-04-17 16:24:37.000000 codecov-cli-0.5.2/codecov_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-17 16:24:37.000000 codecov-cli-0.5.2/codecov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:24:37.000000 codecov-cli-0.5.2/codecov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 16:24:37.000000 codecov-cli-0.5.2/codecov_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-17 16:24:37.000000 codecov-cli-0.5.2/codecov_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 16:24:37.000000 codecov-cli-0.5.2/codecov_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.642361 codecov-cli-0.5.2/languages/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/languages/languages.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.630361 codecov-cli-0.5.2/languages/treesitterjavascript/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.646360 codecov-cli-0.5.2/languages/treesitterjavascript/src/
--rw-r--r--   0 runner    (1001) docker     (127)  2277994 2024-04-17 16:24:25.000000 codecov-cli-0.5.2/languages/treesitterjavascript/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-17 16:24:25.000000 codecov-cli-0.5.2/languages/treesitterjavascript/src/scanner.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.646360 codecov-cli-0.5.2/languages/treesitterjavascript/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-17 16:24:25.000000 codecov-cli-0.5.2/languages/treesitterjavascript/src/tree_sitter/parser.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.630361 codecov-cli-0.5.2/languages/treesitterpython/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.650361 codecov-cli-0.5.2/languages/treesitterpython/src/
--rw-r--r--   0 runner    (1001) docker     (127)  2658198 2024-04-17 16:24:26.000000 codecov-cli-0.5.2/languages/treesitterpython/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-17 16:24:26.000000 codecov-cli-0.5.2/languages/treesitterpython/src/scanner.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:24:37.650361 codecov-cli-0.5.2/languages/treesitterpython/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-17 16:24:26.000000 codecov-cli-0.5.2/languages/treesitterpython/src/tree_sitter/parser.h
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:24:37.654361 codecov-cli-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-17 16:24:23.000000 codecov-cli-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.681754 codecov-cli-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-05-07 17:44:16.681754 codecov-cli-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18631 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.657754 codecov-cli-0.6.0/codecov_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.661754 codecov-cli-0.6.0/codecov_cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/commands/base_picking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/commands/create_report_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/commands/empty_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/commands/get_report_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/commands/labelanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/commands/process_test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/commands/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/commands/send_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/commands/staticanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/commands/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/commands/upload_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/fallbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.661754 codecov-cli-0.6.0/codecov_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.665754 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/appveyor_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/azure_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/bitbucket_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/bitrise_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/buildkite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/circleci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/cirrus_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/codebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/droneci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/heroku.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/teamcity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/travis_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/woodpeckerci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/folder_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/git.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.665754 codecov-cli-0.6.0/codecov_cli/helpers/git_services/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/git_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/git_services/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/helpers/versioning_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.669754 codecov-cli-0.6.0/codecov_cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/plugins/compress_pycoverage_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/plugins/gcov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/plugins/pycoverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/plugins/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/plugins/xcode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.669754 codecov-cli-0.6.0/codecov_cli/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/runners/dan_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/runners/pytest_standard_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/runners/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.669754 codecov-cli-0.6.0/codecov_cli/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.669754 codecov-cli-0.6.0/codecov_cli/services/commit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/commit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/commit/base_picking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.669754 codecov-cli-0.6.0/codecov_cli/services/empty_upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/empty_upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.669754 codecov-cli-0.6.0/codecov_cli/services/report/
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.669754 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.669754 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/general.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.669754 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/node_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.669754 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/finders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/staticanalysis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.669754 codecov-cli-0.6.0/codecov_cli/services/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/upload/file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/upload/legacy_upload_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/upload/network_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/upload/upload_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/upload/upload_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.673754 codecov-cli-0.6.0/codecov_cli/services/upload_completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/services/upload_completion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/codecov_cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.661754 codecov-cli-0.6.0/codecov_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-05-07 17:44:16.000000 codecov-cli-0.6.0/codecov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-07 17:44:16.000000 codecov-cli-0.6.0/codecov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:44:16.000000 codecov-cli-0.6.0/codecov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 17:44:16.000000 codecov-cli-0.6.0/codecov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-07 17:44:16.000000 codecov-cli-0.6.0/codecov_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 17:44:16.000000 codecov-cli-0.6.0/codecov_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.673754 codecov-cli-0.6.0/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/languages/languages.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.657754 codecov-cli-0.6.0/languages/treesitterjavascript/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.677754 codecov-cli-0.6.0/languages/treesitterjavascript/src/
+-rw-r--r--   0 runner    (1001) docker     (127)  2277994 2024-05-07 17:44:06.000000 codecov-cli-0.6.0/languages/treesitterjavascript/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-07 17:44:06.000000 codecov-cli-0.6.0/languages/treesitterjavascript/src/scanner.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.677754 codecov-cli-0.6.0/languages/treesitterjavascript/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-07 17:44:06.000000 codecov-cli-0.6.0/languages/treesitterjavascript/src/tree_sitter/parser.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.657754 codecov-cli-0.6.0/languages/treesitterpython/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.677754 codecov-cli-0.6.0/languages/treesitterpython/src/
+-rw-r--r--   0 runner    (1001) docker     (127)  2658198 2024-05-07 17:44:07.000000 codecov-cli-0.6.0/languages/treesitterpython/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-07 17:44:07.000000 codecov-cli-0.6.0/languages/treesitterpython/src/scanner.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:44:16.681754 codecov-cli-0.6.0/languages/treesitterpython/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-07 17:44:07.000000 codecov-cli-0.6.0/languages/treesitterpython/src/tree_sitter/parser.h
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:44:16.681754 codecov-cli-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-07 17:44:05.000000 codecov-cli-0.6.0/setup.py
```

### Comparing `codecov-cli-0.5.2/LICENSE` & `codecov-cli-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/PKG-INFO` & `codecov-cli-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecov-cli
-Version: 0.5.2
+Version: 0.6.0
 Summary: Codecov Command Line Interface
 Author: Codecov
 Author-email: support@codecov.io
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `codecov-cli-0.5.2/README.md` & `codecov-cli-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/commands/base_picking.py` & `codecov-cli-0.6.0/codecov_cli/commands/base_picking.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/commands/commit.py` & `codecov-cli-0.6.0/codecov_cli/commands/commit.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/commands/create_report_result.py` & `codecov-cli-0.6.0/codecov_cli/commands/create_report_result.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/commands/empty_upload.py` & `codecov-cli-0.6.0/codecov_cli/commands/empty_upload.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/commands/get_report_results.py` & `codecov-cli-0.6.0/codecov_cli/commands/get_report_results.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/commands/labelanalysis.py` & `codecov-cli-0.6.0/codecov_cli/commands/labelanalysis.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/commands/report.py` & `codecov-cli-0.6.0/codecov_cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/commands/send_notifications.py` & `codecov-cli-0.6.0/codecov_cli/commands/send_notifications.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/commands/staticanalysis.py` & `codecov-cli-0.6.0/codecov_cli/commands/staticanalysis.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/commands/upload.py` & `codecov-cli-0.6.0/codecov_cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/commands/upload_process.py` & `codecov-cli-0.6.0/codecov_cli/commands/upload_process.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/fallbacks.py` & `codecov-cli-0.6.0/codecov_cli/fallbacks.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/__init__.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/appveyor_ci.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/appveyor_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/azure_pipelines.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/azure_pipelines.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/base.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/base.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/bitbucket_ci.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/bitbucket_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/bitrise_ci.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/bitrise_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/buildkite.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/buildkite.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/circleci.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/circleci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/cirrus_ci.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/cirrus_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/codebuild.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/codebuild.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/droneci.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/droneci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/github_actions.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/github_actions.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/gitlab_ci.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/heroku.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/heroku.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/jenkins.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/jenkins.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/local.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/local.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/teamcity.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/teamcity.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/travis_ci.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/travis_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/ci_adapters/woodpeckerci.py` & `codecov-cli-0.6.0/codecov_cli/helpers/ci_adapters/woodpeckerci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/config.py` & `codecov-cli-0.6.0/codecov_cli/helpers/config.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/encoder.py` & `codecov-cli-0.6.0/codecov_cli/helpers/encoder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/folder_searcher.py` & `codecov-cli-0.6.0/codecov_cli/helpers/folder_searcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """
     this_is_included = functools.partial(
         _is_included, filename_include_regex, multipart_include_regex
     )
     this_is_excluded = functools.partial(
         _is_excluded, filename_exclude_regex, multipart_exclude_regex
     )
-    for (dirpath, dirnames, filenames) in os.walk(folder_to_search):
+    for dirpath, dirnames, filenames in os.walk(folder_to_search):
         dirs_to_remove = set(d for d in dirnames if d in folders_to_ignore)
 
         if multipart_exclude_regex is not None:
             dirs_to_remove.union(
                 directory
                 for directory in dirnames
                 if multipart_exclude_regex.match(str(pathlib.Path(dirpath) / directory))
```

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/git.py` & `codecov-cli-0.6.0/codecov_cli/helpers/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,21 +57,24 @@
 def parse_git_service(remote_repo_url: str):
     """
     Extracts git service from git remote urls. returns None if the url is invalid
 
     Possible cases we're considering:
     - https://github.com/codecov/codecov-cli.git returns github
     - git@github.com:codecov/codecov-cli.git returns github
+    - ssh://git@github.com/gitcodecov/codecov-cli returns github
+    - ssh://git@github.com:gitcodecov/codecov-cli returns github
     - https://user-name@bitbucket.org/namespace-codecov/first_repo.git returns bitbucket
     """
     services = [service.value for service in GitService]
     parsed_url = urlparse(remote_repo_url)
     service = None
 
-    if remote_repo_url.startswith("https://"):
+    scheme = parsed_url.scheme
+    if scheme in ("https", "ssh"):
         netloc = parsed_url.netloc
         if "@" in netloc:
             netloc = netloc.split("@", 1)[1]
         if "." in netloc:
             netloc = netloc.split(".", 1)[0]
         service = netloc
     elif remote_repo_url.startswith("git@"):
```

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/git_services/github.py` & `codecov-cli-0.6.0/codecov_cli/helpers/git_services/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,19 @@
                 "url": res["url"],
                 "head": {
                     "sha": res["head"]["sha"],
                     "label": res["head"]["label"],
                     "ref": res["head"]["ref"],
                     # Through empiric test data it seems that the "repo" key in "head" is set to None
                     # If the PR is from the same repo (e.g. not from a fork)
-                    "slug": res["head"]["repo"]["full_name"]
-                    if res["head"]["repo"]
-                    else res["base"]["repo"]["full_name"],
+                    "slug": (
+                        res["head"]["repo"]["full_name"]
+                        if res["head"]["repo"]
+                        else res["base"]["repo"]["full_name"]
+                    ),
                 },
                 "base": {
                     "sha": res["base"]["sha"],
                     "label": res["base"]["label"],
                     "ref": res["base"]["ref"],
                     "slug": res["base"]["repo"]["full_name"],
                 },
```

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/logging_utils.py` & `codecov-cli-0.6.0/codecov_cli/helpers/logging_utils.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/options.py` & `codecov-cli-0.6.0/codecov_cli/helpers/options.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/request.py` & `codecov-cli-0.6.0/codecov_cli/helpers/request.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/helpers/versioning_systems.py` & `codecov-cli-0.6.0/codecov_cli/helpers/versioning_systems.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,17 +131,19 @@
             raise ValueError("Can't determine root folder")
 
         res = subprocess.run(
             ["git", "-C", str(dir_to_use), "ls-files"], capture_output=True
         )
 
         return [
-            filename[1:-1]
-            if filename.startswith('"') and filename.endswith('"')
-            else filename
+            (
+                filename[1:-1]
+                if filename.startswith('"') and filename.endswith('"')
+                else filename
+            )
             for filename in res.stdout.decode("unicode_escape").strip().split("\n")
         ]
 
 
 class NoVersioningSystem(VersioningSystemInterface):
     @classmethod
     def is_available(cls):
```

### Comparing `codecov-cli-0.5.2/codecov_cli/main.py` & `codecov-cli-0.6.0/codecov_cli/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from codecov_cli import __version__
 from codecov_cli.commands.base_picking import pr_base_picking
 from codecov_cli.commands.commit import create_commit
 from codecov_cli.commands.create_report_result import create_report_results
 from codecov_cli.commands.empty_upload import empty_upload
 from codecov_cli.commands.get_report_results import get_report_results
 from codecov_cli.commands.labelanalysis import label_analysis
+from codecov_cli.commands.process_test_results import process_test_results
 from codecov_cli.commands.report import create_report
 from codecov_cli.commands.send_notifications import send_notifications
 from codecov_cli.commands.staticanalysis import static_analysis
 from codecov_cli.commands.upload import do_upload
 from codecov_cli.commands.upload_process import upload_process
 from codecov_cli.helpers.ci_adapters import get_ci_adapter, get_ci_providers_list
 from codecov_cli.helpers.config import load_cli_config
@@ -67,14 +68,15 @@
 cli.add_command(get_report_results)
 cli.add_command(pr_base_picking)
 cli.add_command(label_analysis)
 cli.add_command(static_analysis)
 cli.add_command(empty_upload)
 cli.add_command(upload_process)
 cli.add_command(send_notifications)
+cli.add_command(process_test_results)
 
 
 def run():
     cli(obj={})
 
 
 if __name__ == "__main__":
```

### Comparing `codecov-cli-0.5.2/codecov_cli/plugins/__init__.py` & `codecov-cli-0.6.0/codecov_cli/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/plugins/compress_pycoverage_contexts.py` & `codecov-cli-0.6.0/codecov_cli/plugins/compress_pycoverage_contexts.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/plugins/gcov.py` & `codecov-cli-0.6.0/codecov_cli/plugins/gcov.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/plugins/pycoverage.py` & `codecov-cli-0.6.0/codecov_cli/plugins/pycoverage.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/plugins/xcode.py` & `codecov-cli-0.6.0/codecov_cli/plugins/xcode.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/runners/__init__.py` & `codecov-cli-0.6.0/codecov_cli/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/runners/dan_runner.py` & `codecov-cli-0.6.0/codecov_cli/runners/dan_runner.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/runners/pytest_standard_runner.py` & `codecov-cli-0.6.0/codecov_cli/runners/pytest_standard_runner.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/runners/types.py` & `codecov-cli-0.6.0/codecov_cli/runners/types.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/commit/__init__.py` & `codecov-cli-0.6.0/codecov_cli/services/commit/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/commit/base_picking.py` & `codecov-cli-0.6.0/codecov_cli/services/commit/base_picking.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/empty_upload/__init__.py` & `codecov-cli-0.6.0/codecov_cli/services/empty_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/report/__init__.py` & `codecov-cli-0.6.0/codecov_cli/services/report/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/staticanalysis/__init__.py` & `codecov-cli-0.6.0/codecov_cli/services/staticanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/__init__.py` & `codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/general.py` & `codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/general.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,21 +81,21 @@
         cur = node.parent
         while cur:
             yield cur
             cur = cur.parent
 
     def get_import_lines(self, root_node, imports_query):
         import_lines = set()
-        for (a, _) in imports_query.captures(root_node):
+        for a, _ in imports_query.captures(root_node):
             import_lines.add((a.start_point[0] + 1, a.end_point[0] - a.start_point[0]))
         return import_lines
 
     def get_definition_lines(self, root_node, definitions_query):
         definition_lines = set()
-        for (a, _) in definitions_query.captures(root_node):
+        for a, _ in definitions_query.captures(root_node):
             definition_lines.add(
                 (a.start_point[0] + 1, a.end_point[0] - a.start_point[0])
             )
         return definition_lines
 
     def _get_code_hash(self, start_byte, end_byte):
         j = hashlib.md5()
```

### Comparing `codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/javascript_es6/__init__.py` & `codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/javascript_es6/node_wrappers.py` & `codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/node_wrappers.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/python/__init__.py` & `codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/python/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py` & `codecov-cli-0.6.0/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/staticanalysis/finders.py` & `codecov-cli-0.6.0/codecov_cli/services/staticanalysis/finders.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/upload/__init__.py` & `codecov-cli-0.6.0/codecov_cli/services/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/upload/file_finder.py` & `codecov-cli-0.6.0/codecov_cli/services/upload/file_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,15 +249,19 @@
                 multipart_include_regex=multipart_include_regex,
             )
         )
         not_found_files = []
         user_files_paths_resolved = [path.resolve() for path in user_files_paths]
         for filepath in self.explicitly_listed_files:
             if filepath.resolve() not in user_files_paths_resolved:
-                not_found_files.append(filepath)
+                ## The file given might be linked or in a parent dir, check to see if it exists
+                if filepath.exists():
+                    user_files_paths.append(filepath)
+                else:
+                    not_found_files.append(filepath)
 
         if not_found_files:
             logger.warning(
                 "Some files were not found",
                 extra=dict(extra_log_attributes=dict(not_found_files=not_found_files)),
             )
```

### Comparing `codecov-cli-0.5.2/codecov_cli/services/upload/legacy_upload_sender.py` & `codecov-cli-0.6.0/codecov_cli/services/upload/legacy_upload_sender.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/upload/network_finder.py` & `codecov-cli-0.6.0/codecov_cli/services/upload/network_finder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/upload/upload_collector.py` & `codecov-cli-0.6.0/codecov_cli/services/upload/upload_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,23 +42,24 @@
         if not files or self.disable_file_fixes:
             return []
         # patterns that we don't need to specify a reason for
         empty_line_regex = re.compile(r"^\s*$")
         comment_regex = re.compile(r"^\s*\/\/.*$")
         bracket_regex = re.compile(r"^\s*[\{\}]\s*(\/\/.*)?$")
         list_regex = re.compile(r"^\s*[\]\[]\s*(\/\/.*)?$")
+        parenthesis_regex = re.compile(r"^\s*[\(\)]\s*(\/\/.*)?$")
         go_function_regex = re.compile(r"^\s*func\s*[\{]\s*(\/\/.*)?$")
         php_end_bracket_regex = re.compile(r"^\s*\);\s*(\/\/.*)?$")
 
         # patterns to specify a reason for
         comment_block_regex = re.compile(r"^\s*(\/\*|\*\/)\s*$")
         lcov_excel_regex = re.compile(r"\/\/ LCOV_EXCL")
 
         kt_patterns_to_apply = fix_patterns_to_apply(
-            [bracket_regex], [comment_block_regex], True
+            [bracket_regex, parenthesis_regex], [comment_block_regex], True
         )
         go_patterns_to_apply = fix_patterns_to_apply(
             [empty_line_regex, comment_regex, bracket_regex, go_function_regex],
             [comment_block_regex],
             False,
         )
         dart_patterns_to_apply = fix_patterns_to_apply(
@@ -67,15 +68,14 @@
             False,
         )
         php_patterns_to_apply = fix_patterns_to_apply(
             [bracket_regex, list_regex, php_end_bracket_regex],
             [],
             False,
         )
-
         cpp_swift_vala_patterns_to_apply = fix_patterns_to_apply(
             [empty_line_regex, bracket_regex],
             [lcov_excel_regex],
             False,
         )
 
         file_regex_patterns = {
@@ -135,14 +135,16 @@
             logger.warning(
                 f"There was an issue decoding: {filename}, file fixes were not applied to this file.",
                 extra=dict(
                     encoding=err.encoding,
                     reason=err.reason,
                 ),
             )
+        except IsADirectoryError as err:
+            logger.info(f"Skipping {filename}, found a directory not a file")
 
         return UploadCollectionResultFileFixer(
             path, fixed_lines_without_reason, fixed_lines_with_reason, eof
         )
 
     def generate_upload_data(self, report_type="coverage") -> UploadCollectionResult:
         for prep in self.preparation_plugins:
```

### Comparing `codecov-cli-0.5.2/codecov_cli/services/upload/upload_sender.py` & `codecov-cli-0.6.0/codecov_cli/services/upload/upload_sender.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/services/upload_completion/__init__.py` & `codecov-cli-0.6.0/codecov_cli/services/upload_completion/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli/types.py` & `codecov-cli-0.6.0/codecov_cli/types.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/codecov_cli.egg-info/PKG-INFO` & `codecov-cli-0.6.0/codecov_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecov-cli
-Version: 0.5.2
+Version: 0.6.0
 Summary: Codecov Command Line Interface
 Author: Codecov
 Author-email: support@codecov.io
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `codecov-cli-0.5.2/codecov_cli.egg-info/SOURCES.txt` & `codecov-cli-0.6.0/codecov_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 codecov_cli/commands/__init__.py
 codecov_cli/commands/base_picking.py
 codecov_cli/commands/commit.py
 codecov_cli/commands/create_report_result.py
 codecov_cli/commands/empty_upload.py
 codecov_cli/commands/get_report_results.py
 codecov_cli/commands/labelanalysis.py
+codecov_cli/commands/process_test_results.py
 codecov_cli/commands/report.py
 codecov_cli/commands/send_notifications.py
 codecov_cli/commands/staticanalysis.py
 codecov_cli/commands/upload.py
 codecov_cli/commands/upload_process.py
 codecov_cli/helpers/__init__.py
 codecov_cli/helpers/config.py
```

### Comparing `codecov-cli-0.5.2/languages/treesitterjavascript/src/parser.c` & `codecov-cli-0.6.0/languages/treesitterjavascript/src/parser.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/languages/treesitterjavascript/src/scanner.c` & `codecov-cli-0.6.0/languages/treesitterjavascript/src/scanner.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/languages/treesitterjavascript/src/tree_sitter/parser.h` & `codecov-cli-0.6.0/languages/treesitterjavascript/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/languages/treesitterpython/src/parser.c` & `codecov-cli-0.6.0/languages/treesitterpython/src/parser.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/languages/treesitterpython/src/scanner.cc` & `codecov-cli-0.6.0/languages/treesitterpython/src/scanner.cc`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/languages/treesitterpython/src/tree_sitter/parser.h` & `codecov-cli-0.6.0/languages/treesitterpython/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.2/setup.py` & `codecov-cli-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="codecov-cli",
-    version="0.5.2",
+    version="0.6.0",
     packages=find_packages(exclude=["contrib", "docs", "tests*"]),
     description="Codecov Command Line Interface",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Codecov",
     author_email="support@codecov.io",
     install_requires=[
         "click==8.*",
         "httpx==0.23.*",
         "ijson==3.*",
         "pyyaml==6.*",
         "responses==0.21.*",
         "tree-sitter==0.20.*",
+        "test-results-parser==0.1.*",
+        "regex",
     ],
     entry_points={
         "console_scripts": [
             "codecovcli = codecov_cli.main:run",
         ],
     },
     python_requires=">=3.8",
```

