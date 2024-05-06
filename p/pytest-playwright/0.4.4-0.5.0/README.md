# Comparing `tmp/pytest-playwright-0.4.4.tar.gz` & `tmp/pytest-playwright-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-playwright-0.4.4.tar", last modified: Fri Feb  2 13:01:18 2024, max compression
+gzip compressed data, was "pytest-playwright-0.5.0.tar", last modified: Mon May  6 22:49:34 2024, max compression
```

## Comparing `pytest-playwright-0.4.4.tar` & `pytest-playwright-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:01:18.049026 pytest-playwright-0.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:01:18.045026 pytest-playwright-0.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:01:18.045026 pytest-playwright-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-02 13:01:18.049026 pytest-playwright-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/conda_build_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/local-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:01:18.045026 pytest-playwright-0.4.4/pytest_playwright/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/pytest_playwright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-02 13:01:17.000000 pytest-playwright-0.4.4/pytest_playwright/_repo_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13336 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/pytest_playwright/pytest_playwright.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:01:18.049026 pytest-playwright-0.4.4/pytest_playwright.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-02 13:01:17.000000 pytest-playwright-0.4.4/pytest_playwright.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-02-02 13:01:18.000000 pytest-playwright-0.4.4/pytest_playwright.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 13:01:17.000000 pytest-playwright-0.4.4/pytest_playwright.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-02 13:01:17.000000 pytest-playwright-0.4.4/pytest_playwright.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-02 13:01:17.000000 pytest-playwright-0.4.4/pytest_playwright.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-02 13:01:17.000000 pytest-playwright-0.4.4/pytest_playwright.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-02 13:01:18.049026 pytest-playwright-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:01:18.049026 pytest-playwright-0.4.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:01:18.045026 pytest-playwright-0.4.4/tests/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:01:18.049026 pytest-playwright-0.4.4/tests/assets/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/tests/assets/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/tests/assets/django/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/tests/assets/django/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    22249 2024-02-02 13:01:01.000000 pytest-playwright-0.4.4/tests/test_playwright.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 22:49:34.746647 pytest-playwright-0.5.0/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 22:49:34.742647 pytest-playwright-0.5.0/.azure-pipelines/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2042 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/.azure-pipelines/publish.yml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 22:49:34.742647 pytest-playwright-0.5.0/.github/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 22:49:34.746647 pytest-playwright-0.5.0/.github/workflows/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1977 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/.github/workflows/ci.yml
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      905 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/.github/workflows/python-publish.yml
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2135 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/.gitignore
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      648 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/.pre-commit-config.yaml
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      444 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      933 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/CONTRIBUTING.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11399 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1362 2024-05-06 22:49:34.750647 pytest-playwright-0.5.0/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      632 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2780 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/SECURITY.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      158 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/local-requirements.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      728 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/meta.yaml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 22:49:34.746647 pytest-playwright-0.5.0/pytest_playwright/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/pytest_playwright/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       18 2024-05-06 22:49:34.000000 pytest-playwright-0.5.0/pytest_playwright/_repo_version.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19874 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/pytest_playwright/pytest_playwright.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 22:49:34.746647 pytest-playwright-0.5.0/pytest_playwright.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1362 2024-05-06 22:49:34.000000 pytest-playwright-0.5.0/pytest_playwright.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      729 2024-05-06 22:49:34.000000 pytest-playwright-0.5.0/pytest_playwright.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-06 22:49:34.000000 pytest-playwright-0.5.0/pytest_playwright.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       60 2024-05-06 22:49:34.000000 pytest-playwright-0.5.0/pytest_playwright.egg-info/entry_points.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       97 2024-05-06 22:49:34.000000 pytest-playwright-0.5.0/pytest_playwright.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       18 2024-05-06 22:49:34.000000 pytest-playwright-0.5.0/pytest_playwright.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      422 2024-05-06 22:49:34.750647 pytest-playwright-0.5.0/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1450 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 22:49:34.746647 pytest-playwright-0.5.0/tests/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 22:49:34.742647 pytest-playwright-0.5.0/tests/assets/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 22:49:34.746647 pytest-playwright-0.5.0/tests/assets/django/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/tests/assets/django/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2664 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/tests/assets/django/settings.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      133 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/tests/assets/django/urls.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1418 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/tests/conftest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26517 2024-05-06 22:48:42.000000 pytest-playwright-0.5.0/tests/test_playwright.py
```

### Comparing `pytest-playwright-0.4.4/.github/workflows/ci.yml` & `pytest-playwright-0.5.0/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,37 +4,37 @@
     branches: [ main ]
   pull_request:
     branches: [ main ]
 jobs:
   lint:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: 3.11
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -r local-requirements.txt
     - name: Lint
       run: pre-commit run --show-diff-on-failure --color=always --all-files
   build:
     timeout-minutes: 30
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-latest, windows-latest, macos-latest]
+        os: [ubuntu-latest, windows-latest, macos-13]
         python-version: [3.8, 3.9, '3.10', 3.11]
     runs-on: ${{ matrix.os }}
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -r local-requirements.txt
         pip install -e .
@@ -50,19 +50,19 @@
     name: Conda Build
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-latest, macos-latest, windows-latest ]
     runs-on: ${{ matrix.os }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Get conda
-        uses: conda-incubator/setup-miniconda@v2
+        uses: conda-incubator/setup-miniconda@v3
         with:
           python-version: 3.9
           channels: conda-forge
       - name: Prepare
         run: conda install conda-build conda-verify
       - name: Build
         run: conda build . -c microsoft -c conda-forge
```

### Comparing `pytest-playwright-0.4.4/.gitignore` & `pytest-playwright-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.4/.pre-commit-config.yaml` & `pytest-playwright-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.4/CONTRIBUTING.md` & `pytest-playwright-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.4/LICENSE` & `pytest-playwright-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.4/PKG-INFO` & `pytest-playwright-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-playwright
-Version: 0.4.4
+Version: 0.5.0
 Summary: A pytest wrapper with fixtures for Playwright to automate web browsers
 Home-page: https://github.com/microsoft/playwright-pytest
 Author: Microsoft
 Author-email: 
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pytest-playwright-0.4.4/README.md` & `pytest-playwright-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.4/SECURITY.md` & `pytest-playwright-0.5.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.4/meta.yaml` & `pytest-playwright-0.5.0/meta.yaml`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.4/pytest_playwright.egg-info/PKG-INFO` & `pytest-playwright-0.5.0/pytest_playwright.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-playwright
-Version: 0.4.4
+Version: 0.5.0
 Summary: A pytest wrapper with fixtures for Playwright to automate web browsers
 Home-page: https://github.com/microsoft/playwright-pytest
 Author: Microsoft
 Author-email: 
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pytest-playwright-0.4.4/pytest_playwright.egg-info/SOURCES.txt` & `pytest-playwright-0.5.0/pytest_playwright.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .gitignore
 .pre-commit-config.yaml
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 README.md
 SECURITY.md
-conda_build_config.yaml
 local-requirements.txt
 meta.yaml
 setup.cfg
 setup.py
+.azure-pipelines/publish.yml
 .github/workflows/ci.yml
 .github/workflows/python-publish.yml
 pytest_playwright/__init__.py
 pytest_playwright/_repo_version.py
 pytest_playwright/pytest_playwright.py
 pytest_playwright.egg-info/PKG-INFO
 pytest_playwright.egg-info/SOURCES.txt
```

### Comparing `pytest-playwright-0.4.4/setup.py` & `pytest-playwright-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.4/tests/assets/django/settings.py` & `pytest-playwright-0.5.0/tests/assets/django/settings.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.4/tests/conftest.py` & `pytest-playwright-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.4.4/tests/test_playwright.py` & `pytest-playwright-0.5.0/tests/test_playwright.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-import re
 import sys
-from typing import Any, List
 
 import pytest
 
 
 def test_default(testdir: pytest.Testdir) -> None:
     testdir.makepyfile(
         """
@@ -387,14 +385,39 @@
         "2",
     )
     result.assert_outcomes(passed=12)
     assert "gw0" in "\n".join(result.outlines)
     assert "gw1" in "\n".join(result.outlines)
 
 
+def test_xdist_should_not_print_any_warnings(testdir: pytest.Testdir) -> None:
+    original = os.environ.get("PYTHONWARNINGS")
+    os.environ["PYTHONWARNINGS"] = "always"
+    try:
+        testdir.makepyfile(
+            """
+            import pytest
+
+            def test_default(page):
+                pass
+        """
+        )
+        result = testdir.runpytest(
+            "--numprocesses",
+            "2",
+        )
+        result.assert_outcomes(passed=1)
+        assert "ResourceWarning" not in "".join(result.stderr.lines)
+    finally:
+        if original is not None:
+            os.environ["PYTHONWARNINGS"] = original
+        else:
+            del os.environ["PYTHONWARNINGS"]
+
+
 def test_headed(testdir: pytest.Testdir) -> None:
     testdir.makepyfile(
         """
         def test_base_url(page, browser_name):
             user_agent = page.evaluate("window.navigator.userAgent")
             assert "HeadlessChrome" not in user_agent
     """
@@ -627,45 +650,27 @@
         def test_failing(page):
             raise Exception("Failed")
     """
     )
     result = testdir.runpytest("--screenshot", "on", "--video", "on", "--tracing", "on")
     result.assert_outcomes(passed=1, failed=1)
     test_results_dir = os.path.join(testdir.tmpdir, "test-results")
-    expected = [
-        {
-            "name": "test-artifacts-should-store-everything-if-on-py-test-failing-chromium",
-            "children": [
-                {
-                    "name": re.compile(r".*webm"),
-                },
-                {
-                    "name": "test-failed-1.png",
-                },
-                {
-                    "name": "trace.zip",
-                },
-            ],
-        },
-        {
-            "name": "test-artifacts-should-store-everything-if-on-py-test-passing-chromium",
-            "children": [
-                {
-                    "name": re.compile(r".*webm"),
-                },
-                {
-                    "name": "test-finished-1.png",
-                },
-                {
-                    "name": "trace.zip",
-                },
-            ],
-        },
-    ]
-    _assert_folder_tree(test_results_dir, expected)
+    _assert_folder_structure(
+        test_results_dir,
+        """
+- test-artifacts-should-store-everything-if-on-py-test-failing-chromium:
+  - test-failed-1.png
+  - trace.zip
+  - video.webm
+- test-artifacts-should-store-everything-if-on-py-test-passing-chromium:
+  - test-finished-1.png
+  - trace.zip
+  - video.webm
+""",
+    )
 
 
 def test_artifacts_retain_on_failure(testdir: pytest.Testdir) -> None:
     testdir.makepyfile(
         """
         def test_passing(page):
             assert 2 == page.evaluate("1 + 1")
@@ -680,31 +685,23 @@
         "--video",
         "retain-on-failure",
         "--tracing",
         "retain-on-failure",
     )
     result.assert_outcomes(passed=1, failed=1)
     test_results_dir = os.path.join(testdir.tmpdir, "test-results")
-    expected = [
-        {
-            "name": "test-artifacts-retain-on-failure-py-test-failing-chromium",
-            "children": [
-                {
-                    "name": re.compile(r".*webm"),
-                },
-                {
-                    "name": "test-failed-1.png",
-                },
-                {
-                    "name": "trace.zip",
-                },
-            ],
-        }
-    ]
-    _assert_folder_tree(test_results_dir, expected)
+    _assert_folder_structure(
+        test_results_dir,
+        """
+- test-artifacts-retain-on-failure-py-test-failing-chromium:
+  - test-failed-1.png
+  - trace.zip
+  - video.webm
+""",
+    )
 
 
 def test_should_work_with_test_names_which_exceeds_256_characters(
     testdir: pytest.Testdir,
 ) -> None:
     long_test_name = "abcdefghijklmnopqrstuvwxyz" * 100
     testdir.makepyfile(
@@ -712,40 +709,46 @@
         def test_{long_test_name}(page):
             pass
     """
     )
     result = testdir.runpytest("--tracing", "on")
     result.assert_outcomes(passed=1, failed=0)
     test_results_dir = os.path.join(testdir.tmpdir, "test-results")
-    expected = [
-        {
-            "name": "test-should-work-with-test-names-which-exceeds-256-characters-py-test-abcdefghijklmnopqrstuvwxyzabcd-23f2441-nopqrstuvwxyzabcdefghijklmnopqrstuvwxyzabcdefghijklmnopqrstuvwxyzabcdefghijklmnopqrstuvwxyz-chromium/",
-            "children": [
-                {
-                    "name": "trace.zip",
-                },
-            ],
-        },
-    ]
-    _assert_folder_tree(test_results_dir, expected)
-
-
-def _assert_folder_tree(root: str, expected_tree: List[Any]) -> None:
-    assert len(os.listdir(root)) == len(expected_tree)
-    for file in expected_tree:
-        if isinstance(file["name"], str):
-            if "children" in file:
-                assert os.path.isdir(os.path.join(root, file["name"]))
-            else:
-                assert os.path.isfile(os.path.join(root, file["name"]))
-        if isinstance(file["name"], re.Pattern):
-            assert any([file["name"].match(item) for item in os.listdir(root)])
-            assert "children" not in file
-        if "children" in file:
-            _assert_folder_tree(os.path.join(root, file["name"]), file["children"])
+    _assert_folder_structure(
+        test_results_dir,
+        """
+- test-should-work-with-test-names-which-exceeds-256-characters-py-test-abcdefghijklmnopqrstuvwxyzabcd-23f2441-nopqrstuvwxyzabcdefghijklmnopqrstuvwxyzabcdefghijklmnopqrstuvwxyzabcdefghijklmnopqrstuvwxyz-chromium:
+  - trace.zip
+""",
+    )
+
+
+def _make_folder_list(root: str, level: int = 0) -> str:
+    if not os.path.exists(root):
+        return ""
+    tree = []
+    for entry in sorted(os.scandir(root), key=lambda e: e.name):
+        prefix = f"{'  ' * level}- "
+        if entry.is_dir():
+            tree.append(f"{prefix}{entry.name}:\n")
+            tree.append(_make_folder_list(entry.path, level + 1))
+        else:
+            tree.append(f"{prefix}{entry.name}\n")
+    return "".join(tree)
+
+
+def _assert_folder_structure(root: str, expected: str) -> None:
+    __tracebackhide__ = True
+    actual = _make_folder_list(root)
+    if actual.strip() != expected.strip():
+        print("Actual:")
+        print(actual)
+        print("Expected:")
+        print(expected)
+        raise AssertionError("Actual tree does not match expected tree")
 
 
 def test_is_able_to_set_expect_timeout_via_conftest(testdir: pytest.Testdir) -> None:
     testdir.makeconftest(
         """
         from playwright.sync_api import expect
         expect.set_options(timeout=1111)
@@ -760,7 +763,150 @@
             expect(page.locator("#A")).to_be_visible()
     """
     )
     result = testdir.runpytest()
     result.assert_outcomes(passed=0, failed=1, skipped=0)
     result.stdout.fnmatch_lines("*AssertionError: Locator expected to be visible*")
     result.stdout.fnmatch_lines("*LocatorAssertions.to_be_visible with timeout 1111ms*")
+
+
+def test_artifact_collection_should_work_for_manually_created_contexts_keep_open(
+    testdir: pytest.Testdir,
+) -> None:
+    testdir.makepyfile(
+        """
+        import pytest
+
+        def test_artifact_collection(browser, page, new_context):
+            page.goto("data:text/html,<div>hello</div>")
+
+            other_context = new_context()
+            other_context_page = other_context.new_page()
+            other_context_page.goto("data:text/html,<div>hello</div>")
+        """
+    )
+    result = testdir.runpytest("--screenshot", "on", "--video", "on", "--tracing", "on")
+    result.assert_outcomes(passed=1)
+    test_results_dir = os.path.join(testdir.tmpdir, "test-results")
+    _assert_folder_structure(
+        test_results_dir,
+        """
+- test-artifact-collection-should-work-for-manually-created-contexts-keep-open-py-test-artifact-collection-chromium:
+  - test-finished-1.png
+  - test-finished-2.png
+  - trace-1.zip
+  - trace-2.zip
+  - video-1.webm
+  - video-2.webm
+""",
+    )
+
+
+def test_artifact_collection_should_work_for_manually_created_contexts_get_closed(
+    testdir: pytest.Testdir,
+) -> None:
+    testdir.makepyfile(
+        """
+        import pytest
+
+        def test_artifact_collection(browser, page, new_context):
+            page.goto("data:text/html,<div>hello</div>")
+
+            other_context = new_context()
+            other_context_page = other_context.new_page()
+            other_context_page.goto("data:text/html,<div>hello</div>")
+            other_context.close()
+        """
+    )
+    result = testdir.runpytest("--video", "on", "--tracing", "on")
+    result.assert_outcomes(passed=1)
+    test_results_dir = os.path.join(testdir.tmpdir, "test-results")
+    _assert_folder_structure(
+        test_results_dir,
+        """
+- test-artifact-collection-should-work-for-manually-created-contexts-get-closed-py-test-artifact-collection-chromium:
+  - trace-1.zip
+  - trace-2.zip
+  - video-1.webm
+  - video-2.webm
+""",
+    )
+
+
+def test_artifact_collection_should_work_for_manually_created_contexts_retain_on_failure_failed(
+    testdir: pytest.Testdir,
+) -> None:
+    testdir.makepyfile(
+        """
+        import pytest
+
+        def test_artifact_collection(browser, page, new_context):
+            page.goto("data:text/html,<div>hello</div>")
+
+            other_context = new_context()
+            other_context_page = other_context.new_page()
+            other_context_page.goto("data:text/html,<div>hello</div>")
+
+            raise Exception("Failed")
+        """
+    )
+    result = testdir.runpytest(
+        "--video", "retain-on-failure", "--tracing", "retain-on-failure"
+    )
+    result.assert_outcomes(failed=1)
+    test_results_dir = os.path.join(testdir.tmpdir, "test-results")
+    _assert_folder_structure(
+        test_results_dir,
+        """
+- test-artifact-collection-should-work-for-manually-created-contexts-retain-on-failure-failed-py-test-artifact-collection-chromium:
+  - trace-1.zip
+  - trace-2.zip
+  - video-1.webm
+  - video-2.webm
+""",
+    )
+
+
+def test_artifact_collection_should_work_for_manually_created_contexts_retain_on_failure_pass(
+    testdir: pytest.Testdir,
+) -> None:
+    testdir.makepyfile(
+        """
+        import pytest
+
+        def test_artifact_collection(browser, page, new_context):
+            page.goto("data:text/html,<div>hello</div>")
+
+            other_context = new_context()
+            other_context_page = other_context.new_page()
+            other_context_page.goto("data:text/html,<div>hello</div>")
+        """
+    )
+    result = testdir.runpytest(
+        "--video", "retain-on-failure", "--tracing", "retain-on-failure"
+    )
+    result.assert_outcomes(passed=1)
+    test_results_dir = os.path.join(testdir.tmpdir, "test-results")
+    _assert_folder_structure(test_results_dir, "")
+
+
+def test_new_context_allow_passing_args(
+    testdir: pytest.Testdir,
+) -> None:
+    testdir.makepyfile(
+        """
+        import pytest
+
+        def test_artifact_collection(new_context):
+            context1 = new_context(user_agent="agent1")
+            page1 = context1.new_page()
+            assert page1.evaluate("window.navigator.userAgent") == "agent1"
+            context1.close()
+
+            context2 = new_context(user_agent="agent2")
+            page2 = context2.new_page()
+            assert page2.evaluate("window.navigator.userAgent") == "agent2"
+            context2.close()
+            """
+    )
+    result = testdir.runpytest()
+    result.assert_outcomes(passed=1)
```

