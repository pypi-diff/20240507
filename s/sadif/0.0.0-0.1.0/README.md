# Comparing `tmp/sadif-0.0.0.tar.gz` & `tmp/sadif-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sadif-0.0.0.tar", max compression
+gzip compressed data, was "sadif-0.1.0.tar", max compression
```

## Comparing `sadif-0.0.0.tar` & `sadif-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,74 @@
--rw-r--r--   0        0        0        5 2024-04-19 21:15:58.199986 sadif-0.0.0/README.md
--rwxr-xr-x   0        0        0     4538 2024-04-19 21:15:58.203986 sadif-0.0.0/pyproject.toml
--rwxr-xr-x   0        0        0       14 2024-04-19 21:15:58.203986 sadif-0.0.0/src/sadif/__init__.py
--rwxr-xr-x   0        0        0        0 2024-04-19 21:15:58.203986 sadif-0.0.0/src/sadif/py.typed
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 sadif-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-05-07 17:21:45.448671 sadif-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1008 2024-05-07 17:21:45.448671 sadif-0.1.0/README.md
+-rw-r--r--   0        0        0     5377 2024-05-07 17:21:45.456671 sadif-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/__init__.py
+-rw-r--r--   0        0        0     1034 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/cli.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/clientmanager/__init__.py
+-rw-r--r--   0        0        0     3525 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/clientmanager/client_data_export.py
+-rw-r--r--   0        0        0     5694 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/clientmanager/client_data_import.py
+-rw-r--r--   0        0        0    11633 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/clientmanager/client_data_manager.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/config/__init__.py
+-rw-r--r--   0        0        0     2530 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/config/soar_config.py
+-rw-r--r--   0        0        0      120 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/dataconfig/__init__.py
+-rw-r--r--   0        0        0     2473 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/dataconfig/variables.json
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/crawler/__init__.py
+-rw-r--r--   0        0        0     7920 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/crawler/base_crawler/__init__.py
+-rw-r--r--   0        0        0    21705 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/crawler/crawler_manager.py
+-rw-r--r--   0        0        0     6749 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/gitmanager/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/log_manager/__init__.py
+-rw-r--r--   0        0        0     7575 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/log_manager/soar_log.py
+-rw-r--r--   0        0        0    11492 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/modules_manager/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/notification/__init__.py
+-rw-r--r--   0        0        0     6489 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/notification/webhook.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/soar_yara/__init__.py
+-rw-r--r--   0        0        0     3381 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/soar_yara/yara_compiler.py
+-rw-r--r--   0        0        0     3799 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/soar_yara/yara_crud.py
+-rw-r--r--   0        0        0     2499 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/soar_yara/yara_export.py
+-rw-r--r--   0        0        0     7573 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/soar_yara/yara_import.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/caso_de_uso/__init__.py
+-rw-r--r--   0        0        0     1697 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/caso_de_uso/caselist.py
+-rw-r--r--   0        0        0     3364 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_datatype/__init__.py
+-rw-r--r--   0        0        0     4796 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_alert/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_case/__init__.py
+-rw-r--r--   0        0        0     4785 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_case/case_response.py
+-rw-r--r--   0        0        0     6142 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_case/create_case.py
+-rw-r--r--   0        0        0     1950 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_case/delete_case.py
+-rw-r--r--   0        0        0     2299 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_case/get_case.py
+-rw-r--r--   0        0        0     2228 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_case/list_case.py
+-rw-r--r--   0        0        0      383 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_case/save_case.py
+-rw-r--r--   0        0        0     2425 2024-05-07 17:21:45.456671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_case/update_case.py
+-rw-r--r--   0        0        0     1855 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_case_comment_template/__init__.py
+-rw-r--r--   0        0        0     1094 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_case_comment_template/template_render.py
+-rw-r--r--   0        0        0     3152 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_comment/__init__.py
+-rw-r--r--   0        0        0     1911 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_markdown/__init__.py
+-rw-r--r--   0        0        0    12029 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_observable/__init__.py
+-rw-r--r--   0        0        0     6396 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_manager_tasks/__init__.py
+-rw-r--r--   0        0        0     2880 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_internal_mods_api/thehive_session/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/ticket_system/thehive/thehive_ticket_template/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/web/__init__.py
+-rw-r--r--   0        0        0      366 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/web/authenticator/__init__.py
+-rw-r--r--   0        0        0      438 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/web/authenticator/basic_auth_strategy.py
+-rw-r--r--   0        0        0      404 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/web/authenticator/bearer_auth_strategy.py
+-rw-r--r--   0        0        0      493 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/web/authenticator/digest_auth_strategy.py
+-rw-r--r--   0        0        0     1394 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/frameworks_drivers/web/session_manager/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/interfaces/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/interfaces/base_modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/interfaces/web/__init__.py
+-rw-r--r--   0        0        0     1103 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/interfaces/web/authenticator/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/modules/crawler/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/modules/crawler/generic/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/modules/crawler/targeted_crawler/__init__.py
+-rw-r--r--   0        0        0     6302 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/modules/crawler/targeted_crawler/pastebin.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/modules/populate/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/modules/populate/url_to_dbs/__init__.py
+-rw-r--r--   0        0        0    14335 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/modules/populate/url_to_dbs/ransomwhatimport.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/utils/generete_string/__init__.py
+-rw-r--r--   0        0        0     7214 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/utils/generete_string/markdown_string_generator.py
+-rw-r--r--   0        0        0     3117 2024-05-07 17:21:45.460671 sadif-0.1.0/src/sadif/utils/generete_string/random_string_generator.py
+-rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 sadif-0.1.0/PKG-INFO
```

### Comparing `sadif-0.0.0/pyproject.toml` & `sadif-0.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "sadif"
-version = "0.0.0"
+version = "0.1.0"
 description = "Secure Asses Data Insight Framework - SADIF"
 authors = ["CorrêaLabs <lcorrea@florestleaks.com>"]
 readme = "README.md"
 repository = "https://github.com/florestleaks/SADIF"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 update_changelog_on_bump = true
 version_provider = "poetry"
 
 [tool.poetry.dependencies]  # https://python-poetry.org/docs/dependency-specification/
 python = ">=3.10,<4.0"
+pymongo = "^4.6.3"
+sentry-sdk = "^1.45.0"
+toml = "^0.10.2"
+bs4 = "^0.0.2"
+yara-python = "^4.5.0"
+mongomock = "^4.1.2"
+pymdown-extensions = "^10.8.1"
+mdx-include = "^1.4.2"
+mkdocs-rss-plugin = "^1.12.2"
+mkdocstrings = "^0.25.0"
+mkdocstrings-python = "^1.10.0"
+griffe-typingdoc = "^0.2.5"
 
 [tool.poetry.group.test.dependencies]  # https://python-poetry.org/docs/master/managing-dependencies/
 commitizen = ">=3.21.3"
 coverage = { extras = ["toml"], version = ">=7.4.4" }
 mypy = ">=1.9.0"
 poethepoet = ">=0.25.0"
 pre-commit = ">=3.7.0"
@@ -35,14 +47,25 @@
 
 [tool.poetry.group.dev.dependencies]  # https://python-poetry.org/docs/master/managing-dependencies/
 cruft = ">=2.15.0"
 ipykernel = ">=6.29.4"
 ipywidgets = ">=8.1.2"
 pdoc = ">=14.4.0"
 
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.5.3"
+mkdocs-material = "^9.5.18"
+mkdocs-git-authors-plugin = "^0.8.0"
+mkdocs-git-committers-plugin-2 = "^2.3.0"
+mkdocs-git-revision-date-localized-plugin = "^1.2.4"
+mkdocs-glightbox = "^0.3.7"
+mike = {git = "https://github.com/jimporter/mike"}
+lxml = "^5.2.1"
+
 [tool.coverage.report]  # https://coverage.readthedocs.io/en/latest/config.html#report
 fail_under = 0
 precision = 1
 show_missing = true
 skip_covered = true
 
 [tool.coverage.run]  # https://coverage.readthedocs.io/en/latest/config.html#run
@@ -76,17 +99,17 @@
 fix = true
 line-length = 100
 src = ["src", "tests"]
 target-version = "py310"
 
 [tool.ruff.lint]
 ignore-init-module-imports = true
-select = ["A", "ASYNC", "B", "BLE", "C4", "C90", "D", "DTZ", "E", "EM", "ERA", "F", "FBT", "FLY", "FURB", "G", "I", "ICN", "INP", "INT", "ISC", "LOG", "N", "NPY", "PERF", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "Q", "RET", "RSE", "RUF", "S", "SIM", "SLF", "SLOT", "T10", "T20", "TCH", "TID", "TRY", "UP", "W", "YTT"]
-ignore = ["D203", "D213", "E501", "RET504", "S101", "S307"]
-unfixable = ["ERA001", "F401", "F841", "T201", "T203"]
+select = ["A", "ASYNC", "B", "BLE", "C4", "C90", "D", "DTZ", "E", "EM", "ERA", "F", "FBT", "FLY", "FURB", "G", "I", "ICN", "INP", "INT", "ISC", "LOG", "N", "NPY", "PERF", "PGH", "PIE", "PLC", "PLE", "PLR", "PLW", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "S", "SIM", "SLF", "SLOT", "T10", "T20", "TCH", "TID", "TRY", "UP", "W", "YTT"]
+ignore = ["E501","S311",'TRY301','TCH002','PERF203','PLR0912','TRY004','N806','RUF013','TRY002','PLR2004','ERA001','FBT002','N815','N803','PLR0913','C901','W','B007','BLE001','RET505','TRY300','T203','F811','SIM117','T201','UP008','TRY401',"D205","G004","D",'PT',"SLF","ISC001","N999","PGH001", "RET504", "S101"]
+
 
 [tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.lint.pycodestyle]
 max-doc-length = 100
```

