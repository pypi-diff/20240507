# Comparing `tmp/mkdocs_techdocs_diamond-1.0.1.tar.gz` & `tmp/mkdocs_techdocs_diamond-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_techdocs_diamond-1.0.1.tar", last modified: Tue May  7 09:18:36 2024, max compression
+gzip compressed data, was "mkdocs_techdocs_diamond-1.0.2.tar", last modified: Tue May  7 13:36:33 2024, max compression
```

## Comparing `mkdocs_techdocs_diamond-1.0.1.tar` & `mkdocs_techdocs_diamond-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.782673 mkdocs_techdocs_diamond-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.778673 mkdocs_techdocs_diamond-1.0.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.778673 mkdocs_techdocs_diamond-1.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.778673 mkdocs_techdocs_diamond-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14639 2024-05-07 09:18:36.782673 mkdocs_techdocs_diamond-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/catalog-info.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:18:36.782673 mkdocs_techdocs_diamond-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.778673 mkdocs_techdocs_diamond-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.778673 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.782673 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14639 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.782673 mkdocs_techdocs_diamond-1.0.1/test-site/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/test-site/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.782673 mkdocs_techdocs_diamond-1.0.1/test-site/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/test-site/docs/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/test-site/docs/include.md
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/test-site/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/test-site/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:36:33.866215 mkdocs_techdocs_diamond-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:36:33.862215 mkdocs_techdocs_diamond-1.0.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:36:33.862215 mkdocs_techdocs_diamond-1.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:36:33.862215 mkdocs_techdocs_diamond-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14688 2024-05-07 13:36:33.866215 mkdocs_techdocs_diamond-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/catalog-info.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:36:33.866215 mkdocs_techdocs_diamond-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:36:33.862215 mkdocs_techdocs_diamond-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:36:33.862215 mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 13:36:33.000000 mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:36:33.866215 mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14688 2024-05-07 13:36:33.000000 mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 13:36:33.000000 mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:36:33.000000 mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 13:36:33.000000 mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 13:36:33.000000 mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 13:36:33.000000 mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:36:33.862215 mkdocs_techdocs_diamond-1.0.2/test-site/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/test-site/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:36:33.866215 mkdocs_techdocs_diamond-1.0.2/test-site/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/test-site/docs/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/test-site/docs/include.md
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/test-site/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 13:36:28.000000 mkdocs_techdocs_diamond-1.0.2/test-site/mkdocs.yml
```

### Comparing `mkdocs_techdocs_diamond-1.0.1/.devcontainer/devcontainer.json` & `mkdocs_techdocs_diamond-1.0.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `mkdocs_techdocs_diamond-1.0.1/.github/workflows/code.yml` & `mkdocs_techdocs_diamond-1.0.2/.github/workflows/code.yml`

 * *Files 6% similar despite different names*

```diff
@@ -7,71 +7,71 @@
 jobs:
   lint:
     # Deduplicate jobs from pull requests and branch pushes within the same repo.
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10", "3.11", "3.12"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: Checkout
-        uses: actions/checkout@v4.1.2
+        uses: actions/checkout@v4.1.5
 
       - name: Setup Python
         uses: actions/setup-python@v5.1.0
         with:
-          python-version: ${{ matrix.python-version }} 
+          python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: pip install -e .[dev]
 
       - name: Lint
         run: tox -e pre-commit,mypy
 
   canary:
     # Deduplicate jobs from pull requests and branch pushes within the same repo.
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.10", "3.11", "3.12"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: Checkout
-        uses: actions/checkout@v4.1.2
+        uses: actions/checkout@v4.1.5
 
       - name: Setup Python
         uses: actions/setup-python@v5.1.0
         with:
-          python-version: ${{ matrix.python-version }} 
+          python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: pip install .
 
       - name: Build Test Site
         run: mkdocs build
         working-directory: test-site
 
   dist:
     # Deduplicate jobs from pull requests and branch pushes within the same repo.
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     runs-on: "ubuntu-latest"
     steps:
       - name: Checkout
-        uses: actions/checkout@v4.1.2
+        uses: actions/checkout@v4.1.5
 
       - name: Build sdist and wheel
         run: |
           export SOURCE_DATE_EPOCH=$(git log -1 --pretty=%ct) && \
           pipx run build
 
       - name: Check for packaging errors
         run: pipx run twine check --strict dist/*
 
       - name: Upload sdist and wheel as artifacts
-        uses: actions/upload-artifact@v4.3.1
+        uses: actions/upload-artifact@v4.3.3
         with:
           name: dist
           path: dist
 
   release:
     # pull requests are a duplicate of a branch push if within the same repo.
     needs: [lint, canary, dist]
@@ -79,15 +79,15 @@
     runs-on: ubuntu-latest
     permissions:
       id-token: write
       contents: write
     environment: release
     steps:
       - name: Download wheel and lockfiles
-        uses: actions/download-artifact@v4.1.4
+        uses: actions/download-artifact@v4.1.7
         with:
           name: dist
           path: dist
 
       - name: Github Release
         uses: softprops/action-gh-release@v2.0.4
         with:
```

### Comparing `mkdocs_techdocs_diamond-1.0.1/.pre-commit-config.yaml` & `mkdocs_techdocs_diamond-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mkdocs_techdocs_diamond-1.0.1/LICENSE` & `mkdocs_techdocs_diamond-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_techdocs_diamond-1.0.1/PKG-INFO` & `mkdocs_techdocs_diamond-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-techdocs-diamond
-Version: 1.0.1
+Version: 1.0.2
 Summary: An Mkdocs plugin for configuring Diamond Techdocs sites
 Author-email: Garry O'Donnell <garry.o'donnell@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -203,18 +203,19 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
 Project-URL: GitHub, https://github.com/DiamondLightSource/mkdocs-techdocs-diamond
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs<1.6.0
 Requires-Dist: mkdocs-awesome-pages-plugin
 Requires-Dist: mkdocs-include-markdown-plugin
 Requires-Dist: mkdocs-material
 Requires-Dist: mdx_truly_sane_lists
```

### Comparing `mkdocs_techdocs_diamond-1.0.1/pyproject.toml` & `mkdocs_techdocs_diamond-1.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mkdocs-techdocs-diamond"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 description = "An Mkdocs plugin for configuring Diamond Techdocs sites"
 dependencies = [
     "mkdocs<1.6.0",
@@ -20,15 +21,15 @@
     "mdx_truly_sane_lists",
     "pymdown-extensions",
     "pygments",
 ]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 
 [tool.setuptools]
 include-package-data = true
 
 [project.optional-dependencies]
 dev = [
     "black",
```

### Comparing `mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/config.yml` & `mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond/config.yml`

 * *Files identical despite different names*

### Comparing `mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/plugin.py` & `mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/PKG-INFO` & `mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-techdocs-diamond
-Version: 1.0.1
+Version: 1.0.2
 Summary: An Mkdocs plugin for configuring Diamond Techdocs sites
 Author-email: Garry O'Donnell <garry.o'donnell@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -203,18 +203,19 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
 Project-URL: GitHub, https://github.com/DiamondLightSource/mkdocs-techdocs-diamond
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs<1.6.0
 Requires-Dist: mkdocs-awesome-pages-plugin
 Requires-Dist: mkdocs-include-markdown-plugin
 Requires-Dist: mkdocs-material
 Requires-Dist: mdx_truly_sane_lists
```

### Comparing `mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/SOURCES.txt` & `mkdocs_techdocs_diamond-1.0.2/src/mkdocs_techdocs_diamond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

