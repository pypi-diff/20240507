# Comparing `tmp/vinted_scraper-2.2.1.tar.gz` & `tmp/vinted_scraper-2.3.0.tar.gz`

## Comparing `vinted_scraper-2.2.1.tar` & `vinted_scraper-2.3.0.tar`

### file list

```diff
@@ -1,63 +1,72 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.gitmodules
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/Makefile
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/requirements.txt
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/workflows/linter.yml
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/workflows/update-reminder.yml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.github/workflows/update-user-agents.yml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/.git
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/LICENSE
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/Makefile
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/README.md
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/common.mk
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/common_linters.mk
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/git.mk
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/smtp.mk
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/.github/dependabot.yml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/.github/workflows/linter.yml
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/.github/workflows/update-reminder.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/image/README.md
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/image/docker.mk
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/.dockerignore
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/Dockerfile
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/README.md
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/python.mk
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/requirements.txt
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/hooks/pre-commit.bash
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/test/Dockerfile
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/build-tools/python/test/__init__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/__init__.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/agents.json
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/utils.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/vintedScraper.py
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/vintedWrapper.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/__init__.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedBrand.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedBundleDiscount.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedHighResolution.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedImage.py
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedItem.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedMedia.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedPaymentMethod.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/src/vinted_scraper/models/vintedUser.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/__init__.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/test_models.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/test_quickstart.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/test_utils.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/test_vinted.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/test_vinted_item.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/test_vinted_search.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/utils.py
--rw-r--r--   0        0        0    13533 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/samples/item_dummy.json
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/tests/samples/search_item_dummy.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/LICENSE
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/README.md
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 vinted_scraper-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/.gitmodules
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/Makefile
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/requirements.txt
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/.github/workflows/linter.yml
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/.github/workflows/update-reminder.yml
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/.github/workflows/update-user-agents.yml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/.git
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/LICENSE
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/Makefile
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/README.md
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/common.mk
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/common_linters.mk
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/git.mk
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/smtp.mk
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/.github/dependabot.yml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/.github/workflows/linter.yml
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/.github/workflows/update-reminder.yml
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/dart/README.md
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/dart/dart.mk
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/dart/firebase.mk
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/dart/flutter.mk
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/dart/flutter_launcher_icons.yaml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/dart/.github/dependabot.yml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/dart/.github/workflows/linter.yml
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/dart/.github/workflows/release.yml
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/dart/.github/workflows/test.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/image/README.md
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/image/docker.mk
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/python/.dockerignore
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/python/Dockerfile
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/python/README.md
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/python/python.mk
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/python/requirements.txt
+-rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/python/hooks/pre-commit.bash
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/python/test/Dockerfile
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/build-tools/python/test/__init__.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/__init__.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/agents.json
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/utils.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/vintedScraper.py
+-rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/vintedWrapper.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/models/__init__.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/models/vintedBrand.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/models/vintedBundleDiscount.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/models/vintedHighResolution.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/models/vintedImage.py
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/models/vintedItem.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/models/vintedMedia.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/models/vintedPaymentMethod.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/src/vinted_scraper/models/vintedUser.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/tests/test_models.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/tests/test_quickstart.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/tests/test_vinted.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/tests/test_vinted_item.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/tests/test_vinted_search.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/tests/utils.py
+-rw-r--r--   0        0        0    13533 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/tests/samples/item_dummy.json
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/tests/samples/search_item_dummy.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/LICENSE
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/README.md
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 vinted_scraper-2.3.0/PKG-INFO
```

### Comparing `vinted_scraper-2.2.1/Makefile` & `vinted_scraper-2.3.0/Makefile`

 * *Files 11% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 .PHONY: build
 build: py.build
 
 .PHONY: init
 init: py.init git.hooks.setup
 
 .PHONY: update
-update: py.update git.submodules
+update: git.submodules py.update
 
 .PHONY: update.user.agent
 update.user.agent:
 	curl -s "https://www.useragents.me/#most-common-mobile-useragents-json-csv" | grep -A 20 'id="most-common-mobile-useragents-json-csv"' | grep -A 15 'class="col-lg-6"' | grep -o '<textarea class="form-control" rows="8">.*</textarea>' | sed -E 's/<textarea class="form-control" rows="8">//;s/<\/textarea>//' > $(PROJECT_FOLDER)/$(MODULE_NAME)/agents.json
 
 .PHONY: coverage
 coverage:
```

### Comparing `vinted_scraper-2.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `vinted_scraper-2.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/.github/workflows/coverage.yml` & `vinted_scraper-2.3.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/.github/workflows/linter.yml` & `vinted_scraper-2.3.0/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/.github/workflows/release.yml` & `vinted_scraper-2.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/.github/workflows/test.yml` & `vinted_scraper-2.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/.github/workflows/update-reminder.yml` & `vinted_scraper-2.3.0/.github/workflows/update-reminder.yml`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/.github/workflows/update-user-agents.yml` & `vinted_scraper-2.3.0/.github/workflows/update-user-agents.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 name: Update User Agents
 
 on:
   schedule:
     - cron: 0 6 1 */4 *
 
 permissions:
```

### Comparing `vinted_scraper-2.2.1/build-tools/LICENSE` & `vinted_scraper-2.3.0/build-tools/LICENSE`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/build-tools/README.md` & `vinted_scraper-2.3.0/build-tools/README.md`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/build-tools/common.mk` & `vinted_scraper-2.3.0/build-tools/common.mk`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ====================================================================================
 # Setup Project
 
-# remove default suffixes as we dont use them
+# remove default suffixes as we don't use them
 .SUFFIXES:
 
 # set the shell to bash always
 SHELL := /bin/bash
 
 ROOT := $(shell pwd)
 
@@ -41,14 +41,23 @@
 endif
 
 # set the project technology if not defined
 ifeq ($(origin TECHNOLOGY), undefined)
 TECHNOLOGY := shell
 endif
 
+# Detect the OS
+UNAME_S := $(shell uname -s)
+ifeq ($(UNAME_S),Linux)
+	OS := linux
+endif
+ifeq ($(UNAME_S),Darwin)
+	OS := macos
+endif
+
 # ====================================================================================
 # Version and Tagging
 
 # set the version number if not defined
 ifeq ($(origin VERSION), undefined)
 # check if there are any existing `git tag`
 ifeq ($(shell git -C $(PROJECT_FOLDER) tag),)
```

### Comparing `vinted_scraper-2.2.1/build-tools/common_linters.mk` & `vinted_scraper-2.3.0/build-tools/common_linters.mk`

 * *Files 3% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 RUN_LOCAL=true
 endif
 
 # ====================================================================================
 # Actions
 .PHONY: linter.superlinter
 lint.superlinter: #! Run Super Linter as a static analysis tool to scan the codebase.
-	docker run --rm --name=$(PROJECT_NAME)-$(VERSION)-scanner -e RUN_LOCAL=$(RUN_LOCAL) -e FILTER_REGEX_EXCLUDE="$(AUTOGENERATED_FILE_REGEX)" -v $(ROOT):/tmp/lint/ github/super-linter:v4
+	docker run --rm --name=$(PROJECT_NAME)-$(VERSION)-scanner -e RUN_LOCAL=$(RUN_LOCAL) -e DEFAULT_BRANCH=main -e FILTER_REGEX_EXCLUDE="$(AUTOGENERATED_FILE_REGEX)" -v $(ROOT):/tmp/lint/ ghcr.io/super-linter/super-linter:v5
 
 .PHONY: lint.hadolint
 lint.hadolint: #! Run Hadolint as a static analysis tool to scan the Dockerfile.
-	docker run --rm -i ghcr.io/hadolint/hadolint:v2.8.0-alpine < $(DOCKERFILE)
+	docker run --rm -i ghcr.io/hadolint/hadolint:v2.12.0-alpine < $(DOCKERFILE)
 
 .PHONY: lint.checkmake
 lint.checkmake: #! Run Checkmake as a static analysis tool to scan the Makefile.
 	docker run --rm -v $(MAKEFILE):/Makefile mrtazz/checkmake:latest
 
 .PHONY: lint.clean
 lint.clean: #! Remove file generate by the linters.
```

### Comparing `vinted_scraper-2.2.1/build-tools/git.mk` & `vinted_scraper-2.3.0/build-tools/git.mk`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/build-tools/.github/workflows/linter.yml` & `vinted_scraper-2.3.0/build-tools/.github/workflows/linter.yml`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,16 @@
   push:
     branches:
       - main
     tags:
       - v*
   pull_request:
 
+permissions: read-all
+
 jobs:
   build:
     name: Lint Code Base
     runs-on: ubuntu-latest
 
     steps:
       - name: Checkout Code
```

### Comparing `vinted_scraper-2.2.1/build-tools/image/docker.mk` & `vinted_scraper-2.3.0/build-tools/image/docker.mk`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/build-tools/python/Dockerfile` & `vinted_scraper-2.3.0/build-tools/python/Dockerfile`

 * *Files 23% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 
 RUN useradd -ms /bin/bash app
 USER app
 
 COPY --from=builder /home/installer/.local /home/app/.local
 COPY ./src /usr/src/app/src
 
+#checkov:skip=CKV_DOCKER_2: It is not possible to define a generic health check
 WORKDIR /usr/src/app
```

### Comparing `vinted_scraper-2.2.1/build-tools/python/README.md` & `vinted_scraper-2.3.0/build-tools/python/README.md`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/build-tools/python/python.mk` & `vinted_scraper-2.3.0/build-tools/python/python.mk`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/src/vinted_scraper/agents.json` & `vinted_scraper-2.3.0/src/vinted_scraper/agents.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.375%*

 * *Differences: {'0': "{'ua': 'Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) "*

 * *      "Chrome/124.0.0.0 Mobile Safari/537.3', 'pct': 46.73}",*

 * * '1': "{'ua': 'Mozilla/5.0 (iPhone; CPU iPhone OS 17_4_1 like Mac OS X) AppleWebKit/605.1.15 "*

 * *      "(KHTML, like Gecko) Version/17.4.1 Mobile/15E148 Safari/604.', 'pct': 19.63}",*

 * * '10': "{'ua': 'Mozilla/5.0 (iPhone; CPU iPhone OS 17_4 like Mac OS X) AppleWebKit/605.1.15 "*

 * *       "(KHTML, like Gecko) GSA/313.0.625856595 Mobile/15E148 Safari/604.', 'pct': 0 […]*

```diff
@@ -1,90 +1,66 @@
 [
     {
-        "pct": 32.05,
-        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Mobile Safari/537.3"
+        "pct": 46.73,
+        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 26.92,
-        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Mobile Safari/537.3"
+        "pct": 19.63,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_4_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.4.1 Mobile/15E148 Safari/604."
     },
     {
-        "pct": 10.26,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_3_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.3.1 Mobile/15E148 Safari/604."
+        "pct": 10.28,
+        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/25.0 Chrome/121.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 3.85,
+        "pct": 5.61,
         "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/24.0 Chrome/117.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 2.56,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 12_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/12.0 Mobile/15E148 Safari/604."
-    },
-    {
-        "pct": 2.56,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_2_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.2 Mobile/15E148 Safari/604."
-    },
-    {
-        "pct": 2.56,
-        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Mobile Safari/537.3"
-    },
-    {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) GSA/308.0.615969171 Mobile/15E148 Safari/604."
-    },
-    {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 15_8 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/123.0.6312.52 Mobile/15E148 Safari/604."
-    },
-    {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 16_7 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/123.0.6312.52 Mobile/15E148 Safari/604."
-    },
-    {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_1_2 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.1.2 Mobile/15E148 Safari/604."
+        "pct": 2.8,
+        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Mobile Safari/537.3"
+        "pct": 1.87,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/124.0.6367.88 Mobile/15E148 Safari/604."
     },
     {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (Linux; Android 14; SAMSUNG SM-A546B) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
+        "pct": 1.87,
+        "ua": "Mozilla/5.0 (Linux; Android 5.1.1; SAMSUNG SM-J320FN Build/LMY47V) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/3.5 Chrome/38.0.2125.102 Mobile Safari/537.3"
     },
     {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (Linux; Android 10; Redmi Note 7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.106 Mobile Safari/537.3"
+        "pct": 1.87,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/123.0.6312.52 Mobile/15E148 Safari/604."
     },
     {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (Linux; Android 10; moto e(6i) Build/QOH30.280-26) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.6261.119 Mobile Safari/537.3"
+        "pct": 1.87,
+        "ua": "Mozilla/5.0 (Linux; Android 10; MED-LX9N; HMSCore 6.13.0.321) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.4844.88 HuaweiBrowser/14.0.5.302 Mobile Safari/537.3"
     },
     {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (Linux; Android 11; SAMSUNG SM-A202F) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
+        "pct": 1.87,
+        "ua": "Mozilla/5.0 (Linux; Android 11; moto e20 Build/RONS31.267-94-14) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.6312.118 Mobile Safari/537.3"
     },
     {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (Linux; Android 11; SAMSUNG SM-A705FN) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
+        "pct": 0.93,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) GSA/313.0.625856595 Mobile/15E148 Safari/604."
     },
     {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (Linux; Android 13; SAMSUNG SM-G980F) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
+        "pct": 0.93,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 16_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.1 Mobile/15E148 Safari/604."
     },
     {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (Linux; Android 7.0; SM-G930V Build/NRD90M) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/59.0.3071.125 Mobile Safari/537.36 (compatible; Google-Read-Aloud; +https://support.google.com/webmasters/answer/1061943"
+        "pct": 0.93,
+        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_4_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/21E236"
     },
     {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (Linux; Android 9; SAMSUNG SM-J530F) AppleWebKit/537.36 (KHTML, like Gecko) SamsungBrowser/23.0 Chrome/115.0.0.0 Mobile Safari/537.3"
+        "pct": 0.93,
+        "ua": "Mozilla/5.0 (Linux; Android 14; SM-G991B) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Mobile Safari/537.36 ABB/3.4."
     },
     {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Mobile Safari/537.3"
+        "pct": 0.93,
+        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/121.0.0.0 Mobile Safari/537.3"
     },
     {
-        "pct": 1.28,
-        "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.4 Mobile/15E148 Safari/604."
+        "pct": 0.93,
+        "ua": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Mobile Safari/537.3"
     }
 ]
```

### Comparing `vinted_scraper-2.2.1/src/vinted_scraper/vintedScraper.py` & `vinted_scraper-2.3.0/src/vinted_scraper/vintedScraper.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/src/vinted_scraper/vintedWrapper.py` & `vinted_scraper-2.3.0/src/vinted_scraper/vintedWrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import re
+import time
 from typing import Any, Dict, Optional
 
 import requests
 
 from .utils import get_random_user_agent
 
 
@@ -34,40 +35,39 @@
 
         self.user_agent = agent if agent is not None else get_random_user_agent()
         self.session_cookie = (
             session_cookie if session_cookie is not None else self._fetch_cookie()
         )
         self.proxies = proxies
 
-    def _fetch_cookie(self) -> str:
+    def _fetch_cookie(self, retries: int = 3) -> str:
         """
-        Send an HTTP GET request to the self.base_url to fetch the session cookie.
+        Send an HTTP GET request to the self.base_url to fetch the session cookie with retries.
 
+        :param retries: Number of retries for the HTTP request.
         :return: The session cookie extracted from the HTTP response headers.
         :raises RuntimeError: If the session cookie cannot be fetched or doesn't match the expected format.
-
-        The method performs the following steps:
-        1. Sends an HTTP GET request to the base URL using the provided User-Agent header.
-        2. Retrieves the "Set-Cookie" header from the HTTP response.
-        3. Checks if the "Set-Cookie" header contains the expected session cookie format.
-        4. If a matching session cookie is found, it extracts and returns it.
-        5. If the session cookie cannot be fetched or doesn't match the expected format, it raises a RuntimeError.
         """
-        response = requests.get(self.baseurl, headers={"User-Agent": self.user_agent})
-        if 200 == response.status_code:
-            session_cookie = response.headers.get("Set-Cookie")
-            if session_cookie and "_vinted_fr_session=" in session_cookie:
-                return session_cookie.split("_vinted_fr_session=")[1].split(";")[0]
-        else:
-            raise RuntimeError(
-                f"Cannot fetch session cookie from {self.baseurl}, because of status code: {response.status_code} "
-                f"different from 200."
+        response = None
+        for _ in range(retries):
+            response = requests.get(
+                self.baseurl, headers={"User-Agent": self.user_agent}
             )
-
-        raise RuntimeError(f"Cannot fetch session cookie from {self.baseurl}")
+            if response.status_code == 200:
+                session_cookie = response.headers.get("Set-Cookie")
+                if session_cookie and "_vinted_fr_session=" in session_cookie:
+                    return session_cookie.split("_vinted_fr_session=")[1].split(";")[0]
+            else:
+                # Exponential backoff before retrying
+                time.sleep(2**_)
+
+        raise RuntimeError(
+            f"Cannot fetch session cookie from {self.baseurl}, because of "
+            f"status code: {response.status_code if response is not None else 'none'} different from 200."
+        )
 
     def search(self, params: Optional[Dict] = None) -> Dict[str, Any]:
         """
         Search for items on Vinted.
 
         :param params: an optional Dictionary with all the query parameters to append to the request.
             Vinted supports a search without any parameters, but to perform a search,
```

### Comparing `vinted_scraper-2.2.1/src/vinted_scraper/models/__init__.py` & `vinted_scraper-2.3.0/src/vinted_scraper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/src/vinted_scraper/models/vintedBrand.py` & `vinted_scraper-2.3.0/src/vinted_scraper/models/vintedBrand.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/src/vinted_scraper/models/vintedBundleDiscount.py` & `vinted_scraper-2.3.0/src/vinted_scraper/models/vintedBundleDiscount.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/src/vinted_scraper/models/vintedImage.py` & `vinted_scraper-2.3.0/src/vinted_scraper/models/vintedImage.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/src/vinted_scraper/models/vintedItem.py` & `vinted_scraper-2.3.0/src/vinted_scraper/models/vintedItem.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/src/vinted_scraper/models/vintedPaymentMethod.py` & `vinted_scraper-2.3.0/src/vinted_scraper/models/vintedPaymentMethod.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/src/vinted_scraper/models/vintedUser.py` & `vinted_scraper-2.3.0/src/vinted_scraper/models/vintedUser.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/tests/test_models.py` & `vinted_scraper-2.3.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/tests/test_quickstart.py` & `vinted_scraper-2.3.0/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/tests/test_vinted.py` & `vinted_scraper-2.3.0/tests/test_vinted.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,10 +53,18 @@
         Ensure that the initializer raises an error if it can find the session cookie because of a status code different
          from 200.
         """
         with self.assertRaises(RuntimeError):
             with patch("requests.get", return_value=get_404_response()):
                 VintedWrapper(self.baseurl)
 
+    def test_retry(self):
+        with self.assertRaises(RuntimeError):
+            with patch("requests.get", return_value=get_404_response()) as mock_get:
+                VintedWrapper(self.baseurl)
+
+        # Asserting that requests.get was called 3 times (initial call + 2 retries)
+        self.assertEqual(mock_get.call_count, 3)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `vinted_scraper-2.2.1/tests/test_vinted_item.py` & `vinted_scraper-2.3.0/tests/test_vinted_item.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/tests/test_vinted_search.py` & `vinted_scraper-2.3.0/tests/test_vinted_search.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/tests/utils.py` & `vinted_scraper-2.3.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/tests/samples/item_dummy.json` & `vinted_scraper-2.3.0/tests/samples/item_dummy.json`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/tests/samples/search_item_dummy.json` & `vinted_scraper-2.3.0/tests/samples/search_item_dummy.json`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/.gitignore` & `vinted_scraper-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/LICENSE` & `vinted_scraper-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/README.md` & `vinted_scraper-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vinted_scraper-2.2.1/pyproject.toml` & `vinted_scraper-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vinted_scraper"
-version = "2.2.1"
+version = "2.3.0"
 description = "A very simple Python package that scrapes the Vinted website to retrieve information about its items."
 readme = "README.md"
 requires-python = ">= 3.6"
 license = { file = "LICENSE" }
 authors = [
     { name = "Giglium" }
 ]
```

### Comparing `vinted_scraper-2.2.1/PKG-INFO` & `vinted_scraper-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: vinted_scraper
-Version: 2.2.1
+Version: 2.3.0
 Summary: A very simple Python package that scrapes the Vinted website to retrieve information about its items.
 Project-URL: Changelog, https://github.com/Giglium/vinted_scraper/releases
 Project-URL: Documentation, https://github.com/Giglium/vinted_scraper
 Project-URL: Homepage, https://github.com/Giglium/vinted_scraper
 Project-URL: Issues, https://github.com/Giglium/vinted_scraper/issues
 Project-URL: Source, https://github.com/Giglium/vinted_scraper
 Author: Giglium
```

