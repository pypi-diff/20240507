# Comparing `tmp/python_semantic_release-9.7.0.tar.gz` & `tmp/python_semantic_release-9.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_semantic_release-9.7.0.tar", last modified: Mon May  6 03:00:20 2024, max compression
+gzip compressed data, was "python_semantic_release-9.7.1.tar", last modified: Tue May  7 03:29:03 2024, max compression
```

## Comparing `python_semantic_release-9.7.0.tar` & `python_semantic_release-9.7.1.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.107523 python_semantic_release-9.7.0/
--rw-r--r--   0 root         (0) root         (0)      230 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1083 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      225 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5282 2024-05-06 03:00:20.107523 python_semantic_release-9.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2673 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.079522 python_semantic_release-9.7.0/docs/
--rw-r--r--   0 root         (0) root         (0)     6984 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     9656 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/algorithm.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.079522 python_semantic_release-9.7.0/docs/automatic-releases/
--rw-r--r--   0 root         (0) root         (0)     1284 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/automatic-releases/cronjobs.rst
--rw-r--r--   0 root         (0) root         (0)     4046 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/automatic-releases/github-actions.rst
--rw-r--r--   0 root         (0) root         (0)      738 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/automatic-releases/index.rst
--rw-r--r--   0 root         (0) root         (0)     2268 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/automatic-releases/travis.rst
--rw-r--r--   0 root         (0) root         (0)    17609 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/changelog_templates.rst
--rw-r--r--   0 root         (0) root         (0)    16256 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/commands.rst
--rw-r--r--   0 root         (0) root         (0)    15380 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/commit-parsing.rst
--rw-r--r--   0 root         (0) root         (0)     2288 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)    29841 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/configuration.rst
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/contributors.rst
--rw-r--r--   0 root         (0) root         (0)     3644 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/github-action.rst
--rw-r--r--   0 root         (0) root         (0)     6814 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     6735 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)    21218 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/migrating_from_v7.rst
--rw-r--r--   0 root         (0) root         (0)     8869 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/multibranch_releases.rst
--rw-r--r--   0 root         (0) root         (0)     2403 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/strict_mode.rst
--rw-r--r--   0 root         (0) root         (0)     1452 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/docs/troubleshooting.rst
--rw-r--r--   0 root         (0) root         (0)     9237 2024-05-06 03:00:13.000000 python_semantic_release-9.7.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.103522 python_semantic_release-9.7.0/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5282 2024-05-06 03:00:20.000000 python_semantic_release-9.7.0/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5600 2024-05-06 03:00:20.000000 python_semantic_release-9.7.0/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 03:00:20.000000 python_semantic_release-9.7.0/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2024-05-06 03:00:20.000000 python_semantic_release-9.7.0/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      614 2024-05-06 03:00:20.000000 python_semantic_release-9.7.0/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-06 03:00:20.000000 python_semantic_release-9.7.0/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.083522 python_semantic_release-9.7.0/semantic_release/
--rw-r--r--   0 root         (0) root         (0)      870 2024-05-06 03:00:13.000000 python_semantic_release-9.7.0/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.083522 python_semantic_release-9.7.0/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      262 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1051 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6675 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4640 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.083522 python_semantic_release-9.7.0/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      419 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.083522 python_semantic_release-9.7.0/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4197 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     3443 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/commands/cli_context.py
--rw-r--r--   0 root         (0) root         (0)     1699 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     2900 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1958 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    25912 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)     1439 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    20389 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2110 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     3071 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.087523 python_semantic_release-9.7.0/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      615 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3004 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4579 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3452 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5879 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3353 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1505 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      730 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.071523 python_semantic_release-9.7.0/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.087523 python_semantic_release-9.7.0/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     5581 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.087523 python_semantic_release-9.7.0/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2607 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     9216 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/hvcs/bitbucket.py
--rw-r--r--   0 root         (0) root         (0)    11152 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    18287 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     6249 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)     6055 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/hvcs/remote_hvcs_base.py
--rw-r--r--   0 root         (0) root         (0)      663 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2886 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.091523 python_semantic_release-9.7.0/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      270 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16854 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7357 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14175 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 03:00:20.107523 python_semantic_release-9.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.091523 python_semantic_release-9.7.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.091523 python_semantic_release-9.7.0/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2983 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)    11360 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1759 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)     6566 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)     5255 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/command_line/test_publish.py
--rw-r--r--   0 root         (0) root         (0)    31841 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/command_line/test_version.py
--rw-r--r--   0 root         (0) root         (0)     2880 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     7826 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.095522 python_semantic_release-9.7.0/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      197 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1178 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)    12976 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    13342 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/git_repo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.095522 python_semantic_release-9.7.0/tests/fixtures/repos/
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/repos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.095522 python_semantic_release-9.7.0/tests/fixtures/repos/git_flow/
--rw-r--r--   0 root         (0) root         (0)      140 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/repos/git_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21042 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
--rw-r--r--   0 root         (0) root         (0)    21711 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.095522 python_semantic_release-9.7.0/tests/fixtures/repos/github_flow/
--rw-r--r--   0 root         (0) root         (0)       71 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/repos/github_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15712 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/repos/github_flow/repo_w_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.095522 python_semantic_release-9.7.0/tests/fixtures/repos/trunk_based_dev/
--rw-r--r--   0 root         (0) root         (0)      199 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/repos/trunk_based_dev/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10463 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
--rw-r--r--   0 root         (0) root         (0)    13604 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
--rw-r--r--   0 root         (0) root         (0)    10698 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
--rw-r--r--   0 root         (0) root         (0)    14083 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.095522 python_semantic_release-9.7.0/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127286 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12845 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     5074 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.099522 python_semantic_release-9.7.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.099522 python_semantic_release-9.7.0/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.099522 python_semantic_release-9.7.0/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10042 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/changelog/test_changelog_context.py
--rw-r--r--   0 root         (0) root         (0)     6358 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     3560 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2116 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.099522 python_semantic_release-9.7.0/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8907 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     2129 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     6361 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     4344 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/cli/test_util.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.103522 python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6374 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2567 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      778 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/test_parsed_commit.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2203 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      836 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.103522 python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1761 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    10290 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/test_bitbucket.py
--rw-r--r--   0 root         (0) root         (0)    27795 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    36478 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    15576 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      966 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/test_util.py
--rw-r--r--   0 root         (0) root         (0)     4507 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/test_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 03:00:20.103522 python_semantic_release-9.7.0/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9605 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3874 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2951 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9714 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/unit/semantic_release/version/test_version.py
--rw-r--r--   0 root         (0) root         (0)     6271 2024-05-06 02:59:01.000000 python_semantic_release-9.7.0/tests/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.137456 python_semantic_release-9.7.1/
+-rw-r--r--   0 root         (0) root         (0)      230 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      225 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5282 2024-05-07 03:29:03.137456 python_semantic_release-9.7.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2673 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.105455 python_semantic_release-9.7.1/docs/
+-rw-r--r--   0 root         (0) root         (0)     6984 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)     9656 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/algorithm.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.109455 python_semantic_release-9.7.1/docs/automatic-releases/
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/automatic-releases/cronjobs.rst
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/automatic-releases/github-actions.rst
+-rw-r--r--   0 root         (0) root         (0)      738 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/automatic-releases/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/automatic-releases/travis.rst
+-rw-r--r--   0 root         (0) root         (0)    17609 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/changelog_templates.rst
+-rw-r--r--   0 root         (0) root         (0)    16256 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/commands.rst
+-rw-r--r--   0 root         (0) root         (0)    15380 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/commit-parsing.rst
+-rw-r--r--   0 root         (0) root         (0)     2288 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)    29841 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/contributors.rst
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/github-action.rst
+-rw-r--r--   0 root         (0) root         (0)     6814 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     6735 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)    21218 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/migrating_from_v7.rst
+-rw-r--r--   0 root         (0) root         (0)     8869 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/multibranch_releases.rst
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/strict_mode.rst
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/docs/troubleshooting.rst
+-rw-r--r--   0 root         (0) root         (0)     9237 2024-05-07 03:28:56.000000 python_semantic_release-9.7.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.133455 python_semantic_release-9.7.1/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5282 2024-05-07 03:29:03.000000 python_semantic_release-9.7.1/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5600 2024-05-07 03:29:03.000000 python_semantic_release-9.7.1/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 03:29:03.000000 python_semantic_release-9.7.1/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2024-05-07 03:29:03.000000 python_semantic_release-9.7.1/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      614 2024-05-07 03:29:03.000000 python_semantic_release-9.7.1/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 03:29:03.000000 python_semantic_release-9.7.1/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.109455 python_semantic_release-9.7.1/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)      870 2024-05-07 03:28:56.000000 python_semantic_release-9.7.1/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.109455 python_semantic_release-9.7.1/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.113455 python_semantic_release-9.7.1/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      419 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.113455 python_semantic_release-9.7.1/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3443 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/cli_context.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    25912 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    20389 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.117455 python_semantic_release-9.7.1/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      615 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5879 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3353 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      730 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.097455 python_semantic_release-9.7.1/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.117455 python_semantic_release-9.7.1/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5581 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.117455 python_semantic_release-9.7.1/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     9216 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)    11152 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    18287 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     6249 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)     6055 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/remote_hvcs_base.py
+-rw-r--r--   0 root         (0) root         (0)      663 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.121455 python_semantic_release-9.7.1/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16854 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7357 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14175 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 03:29:03.137456 python_semantic_release-9.7.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.121455 python_semantic_release-9.7.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.121455 python_semantic_release-9.7.1/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    11360 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     6566 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     5255 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    31841 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/command_line/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     7826 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)    12976 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    13342 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/git_repo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/fixtures/repos/
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/fixtures/repos/git_flow/
+-rw-r--r--   0 root         (0) root         (0)      140 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/git_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21042 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
+-rw-r--r--   0 root         (0) root         (0)    21711 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/fixtures/repos/github_flow/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/github_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15712 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/github_flow/repo_w_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10463 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
+-rw-r--r--   0 root         (0) root         (0)    10698 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
+-rw-r--r--   0 root         (0) root         (0)    14083 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   127286 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12845 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     5074 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.125455 python_semantic_release-9.7.1/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.129455 python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10042 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_changelog_context.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3560 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.129455 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8907 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     6361 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4344 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_util.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.129455 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6374 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      778 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_parsed_commit.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      836 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.133455 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    10290 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)    27795 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    36478 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    15576 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      966 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_util.py
+-rw-r--r--   0 root         (0) root         (0)     4507 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/test_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 03:29:03.133455 python_semantic_release-9.7.1/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9605 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3874 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9714 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     6271 2024-05-07 03:27:42.000000 python_semantic_release-9.7.1/tests/util.py
```

### Comparing `python_semantic_release-9.7.0/LICENSE` & `python_semantic_release-9.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/PKG-INFO` & `python_semantic_release-9.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.7.0
+Version: 9.7.1
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
@@ -49,15 +49,15 @@
 Requires-Dist: pytest-clarity~=1.0; extra == "test"
 Requires-Dist: responses~=0.25.0; extra == "test"
 Requires-Dist: requests-mock~=1.10; extra == "test"
 Requires-Dist: types-pytest-lazy-fixture~=0.6.3; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pre-commit~=3.5; extra == "dev"
 Requires-Dist: tox~=4.11; extra == "dev"
-Requires-Dist: ruff==0.4.2; extra == "dev"
+Requires-Dist: ruff==0.4.3; extra == "dev"
 Provides-Extra: mypy
 Requires-Dist: mypy==1.10.0; extra == "mypy"
 Requires-Dist: types-requests~=2.31.0; extra == "mypy"
 
 Python Semantic Release
 ***********************
```

### Comparing `python_semantic_release-9.7.0/README.rst` & `python_semantic_release-9.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/Makefile` & `python_semantic_release-9.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/algorithm.rst` & `python_semantic_release-9.7.1/docs/algorithm.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/automatic-releases/cronjobs.rst` & `python_semantic_release-9.7.1/docs/automatic-releases/cronjobs.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/automatic-releases/github-actions.rst` & `python_semantic_release-9.7.1/docs/automatic-releases/github-actions.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/automatic-releases/index.rst` & `python_semantic_release-9.7.1/docs/automatic-releases/index.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/automatic-releases/travis.rst` & `python_semantic_release-9.7.1/docs/automatic-releases/travis.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/changelog_templates.rst` & `python_semantic_release-9.7.1/docs/changelog_templates.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/commands.rst` & `python_semantic_release-9.7.1/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/commit-parsing.rst` & `python_semantic_release-9.7.1/docs/commit-parsing.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/conf.py` & `python_semantic_release-9.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/configuration.rst` & `python_semantic_release-9.7.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/github-action.rst` & `python_semantic_release-9.7.1/docs/github-action.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/index.rst` & `python_semantic_release-9.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/make.bat` & `python_semantic_release-9.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/migrating_from_v7.rst` & `python_semantic_release-9.7.1/docs/migrating_from_v7.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/multibranch_releases.rst` & `python_semantic_release-9.7.1/docs/multibranch_releases.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/strict_mode.rst` & `python_semantic_release-9.7.1/docs/strict_mode.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/docs/troubleshooting.rst` & `python_semantic_release-9.7.1/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/pyproject.toml` & `python_semantic_release-9.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools ~= 69.0", "wheel ~= 0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "9.7.0"
+version = "9.7.1"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
@@ -67,15 +67,15 @@
   "responses ~= 0.25.0",
   "requests-mock ~= 1.10",
   "types-pytest-lazy-fixture ~= 0.6.3",
 ]
 dev = [
   "pre-commit ~= 3.5",
   "tox ~= 4.11",
-  "ruff == 0.4.2"
+  "ruff == 0.4.3"
 ]
 mypy = [
   "mypy == 1.10.0",
   "types-requests ~= 2.31.0"
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `python_semantic_release-9.7.0/python_semantic_release.egg-info/PKG-INFO` & `python_semantic_release-9.7.1/python_semantic_release.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.7.0
+Version: 9.7.1
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
@@ -49,15 +49,15 @@
 Requires-Dist: pytest-clarity~=1.0; extra == "test"
 Requires-Dist: responses~=0.25.0; extra == "test"
 Requires-Dist: requests-mock~=1.10; extra == "test"
 Requires-Dist: types-pytest-lazy-fixture~=0.6.3; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pre-commit~=3.5; extra == "dev"
 Requires-Dist: tox~=4.11; extra == "dev"
-Requires-Dist: ruff==0.4.2; extra == "dev"
+Requires-Dist: ruff==0.4.3; extra == "dev"
 Provides-Extra: mypy
 Requires-Dist: mypy==1.10.0; extra == "mypy"
 Requires-Dist: types-requests~=2.31.0; extra == "mypy"
 
 Python Semantic Release
 ***********************
```

### Comparing `python_semantic_release-9.7.0/python_semantic_release.egg-info/SOURCES.txt` & `python_semantic_release-9.7.1/python_semantic_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/python_semantic_release.egg-info/requires.txt` & `python_semantic_release-9.7.1/python_semantic_release.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 pydantic~=2.0
 rich~=13.0
 shellingham~=1.5
 
 [dev]
 pre-commit~=3.5
 tox~=4.11
-ruff==0.4.2
+ruff==0.4.3
 
 [docs]
 Sphinx~=6.0
 sphinxcontrib-apidoc==0.5.0
 sphinx-autobuild==2024.2.4
 furo~=2024.1
```

### Comparing `python_semantic_release-9.7.0/semantic_release/__init__.py` & `python_semantic_release-9.7.1/semantic_release/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from semantic_release.version import (
     Version,
     VersionTranslator,
     next_version,
     tags_and_versions,
 )
 
-__version__ = "9.7.0"
+__version__ = "9.7.1"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python_semantic_release-9.7.0/semantic_release/changelog/context.py` & `python_semantic_release-9.7.1/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/changelog/release_history.py` & `python_semantic_release-9.7.1/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/changelog/template.py` & `python_semantic_release-9.7.1/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/cli/commands/changelog.py` & `python_semantic_release-9.7.1/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/cli/commands/cli_context.py` & `python_semantic_release-9.7.1/semantic_release/cli/commands/cli_context.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/cli/commands/generate_config.py` & `python_semantic_release-9.7.1/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/cli/commands/main.py` & `python_semantic_release-9.7.1/semantic_release/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/cli/commands/publish.py` & `python_semantic_release-9.7.1/semantic_release/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/cli/commands/version.py` & `python_semantic_release-9.7.1/semantic_release/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/cli/common.py` & `python_semantic_release-9.7.1/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/cli/config.py` & `python_semantic_release-9.7.1/semantic_release/cli/config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/cli/github_actions_output.py` & `python_semantic_release-9.7.1/semantic_release/cli/github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/cli/masking_filter.py` & `python_semantic_release-9.7.1/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/cli/util.py` & `python_semantic_release-9.7.1/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/commit_parser/__init__.py` & `python_semantic_release-9.7.1/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/commit_parser/_base.py` & `python_semantic_release-9.7.1/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/commit_parser/angular.py` & `python_semantic_release-9.7.1/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/commit_parser/emoji.py` & `python_semantic_release-9.7.1/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/commit_parser/scipy.py` & `python_semantic_release-9.7.1/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/commit_parser/tag.py` & `python_semantic_release-9.7.1/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/commit_parser/token.py` & `python_semantic_release-9.7.1/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/commit_parser/util.py` & `python_semantic_release-9.7.1/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/const.py` & `python_semantic_release-9.7.1/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/data/templates/CHANGELOG.md.j2` & `python_semantic_release-9.7.1/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/enums.py` & `python_semantic_release-9.7.1/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/errors.py` & `python_semantic_release-9.7.1/semantic_release/errors.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/helpers.py` & `python_semantic_release-9.7.1/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/hvcs/_base.py` & `python_semantic_release-9.7.1/semantic_release/hvcs/_base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/hvcs/bitbucket.py` & `python_semantic_release-9.7.1/semantic_release/hvcs/bitbucket.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/hvcs/gitea.py` & `python_semantic_release-9.7.1/semantic_release/hvcs/gitea.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/hvcs/github.py` & `python_semantic_release-9.7.1/semantic_release/hvcs/github.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/hvcs/gitlab.py` & `python_semantic_release-9.7.1/semantic_release/hvcs/gitlab.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/hvcs/remote_hvcs_base.py` & `python_semantic_release-9.7.1/semantic_release/hvcs/remote_hvcs_base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/hvcs/token_auth.py` & `python_semantic_release-9.7.1/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/hvcs/util.py` & `python_semantic_release-9.7.1/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/version/algorithm.py` & `python_semantic_release-9.7.1/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/version/declaration.py` & `python_semantic_release-9.7.1/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/version/translator.py` & `python_semantic_release-9.7.1/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/semantic_release/version/version.py` & `python_semantic_release-9.7.1/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/command_line/conftest.py` & `python_semantic_release-9.7.1/tests/command_line/conftest.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/command_line/test_changelog.py` & `python_semantic_release-9.7.1/tests/command_line/test_changelog.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/command_line/test_generate_config.py` & `python_semantic_release-9.7.1/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/command_line/test_help.py` & `python_semantic_release-9.7.1/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/command_line/test_main.py` & `python_semantic_release-9.7.1/tests/command_line/test_main.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/command_line/test_publish.py` & `python_semantic_release-9.7.1/tests/command_line/test_publish.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/command_line/test_version.py` & `python_semantic_release-9.7.1/tests/command_line/test_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/conftest.py` & `python_semantic_release-9.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/const.py` & `python_semantic_release-9.7.1/tests/const.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/fixtures/commit_parsers.py` & `python_semantic_release-9.7.1/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/fixtures/example_project.py` & `python_semantic_release-9.7.1/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/fixtures/git_repo.py` & `python_semantic_release-9.7.1/tests/fixtures/git_repo.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py` & `python_semantic_release-9.7.1/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py` & `python_semantic_release-9.7.1/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/fixtures/repos/github_flow/repo_w_release_channels.py` & `python_semantic_release-9.7.1/tests/fixtures/repos/github_flow/repo_w_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py` & `python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py` & `python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py` & `python_semantic_release-9.7.1/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/fixtures/scipy.py` & `python_semantic_release-9.7.1/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/scenario/test_next_version.py` & `python_semantic_release-9.7.1/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/scenario/test_release_history.py` & `python_semantic_release-9.7.1/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/scenario/test_template_render.py` & `python_semantic_release-9.7.1/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/changelog/test_changelog_context.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_changelog_context.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/changelog/test_release_notes.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/changelog/test_template.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/cli/test_config.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/cli/test_github_actions_output.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/cli/test_masking_filter.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/cli/test_util.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/cli/test_version.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/test_angular.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/test_parsed_commit.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_parsed_commit.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/test_scipy.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_scipy.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/test_tag.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/commit_parser/test_util.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/commit_parser/test_util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/test__base.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/test_bitbucket.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_bitbucket.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/test_gitea.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/test_github.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/test_helpers.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/version/test_algorithm.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/version/test_declaration.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/version/test_translator.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/unit/semantic_release/version/test_version.py` & `python_semantic_release-9.7.1/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.0/tests/util.py` & `python_semantic_release-9.7.1/tests/util.py`

 * *Files identical despite different names*

