# Comparing `tmp/mkdocs-techdocs-diamond-1.0.0.tar.gz` & `tmp/mkdocs_techdocs_diamond-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-techdocs-diamond-1.0.0.tar", last modified: Fri Jan 19 12:06:39 2024, max compression
+gzip compressed data, was "mkdocs_techdocs_diamond-1.0.1.tar", last modified: Tue May  7 09:18:36 2024, max compression
```

## Comparing `mkdocs-techdocs-diamond-1.0.0.tar` & `mkdocs_techdocs_diamond-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 12:06:39.556087 mkdocs-techdocs-diamond-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 12:06:39.552087 mkdocs-techdocs-diamond-1.0.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 12:06:39.552087 mkdocs-techdocs-diamond-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 12:06:39.552087 mkdocs-techdocs-diamond-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14633 2024-01-19 12:06:39.556087 mkdocs-techdocs-diamond-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/catalog-info.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 12:06:39.556087 mkdocs-techdocs-diamond-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 12:06:39.552087 mkdocs-techdocs-diamond-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 12:06:39.556087 mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-19 12:06:39.000000 mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 12:06:39.556087 mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14633 2024-01-19 12:06:39.000000 mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-01-19 12:06:39.000000 mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 12:06:39.000000 mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-19 12:06:39.000000 mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-01-19 12:06:39.000000 mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-19 12:06:39.000000 mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 12:06:39.556087 mkdocs-techdocs-diamond-1.0.0/test-site/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/test-site/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 12:06:39.556087 mkdocs-techdocs-diamond-1.0.0/test-site/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/test-site/docs/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/test-site/docs/include.md
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/test-site/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-19 12:06:33.000000 mkdocs-techdocs-diamond-1.0.0/test-site/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.782673 mkdocs_techdocs_diamond-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.778673 mkdocs_techdocs_diamond-1.0.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.778673 mkdocs_techdocs_diamond-1.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.778673 mkdocs_techdocs_diamond-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14639 2024-05-07 09:18:36.782673 mkdocs_techdocs_diamond-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/catalog-info.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:18:36.782673 mkdocs_techdocs_diamond-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.778673 mkdocs_techdocs_diamond-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.778673 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.782673 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14639 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 09:18:36.000000 mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.782673 mkdocs_techdocs_diamond-1.0.1/test-site/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/test-site/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:18:36.782673 mkdocs_techdocs_diamond-1.0.1/test-site/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/test-site/docs/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/test-site/docs/include.md
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/test-site/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 09:18:33.000000 mkdocs_techdocs_diamond-1.0.1/test-site/mkdocs.yml
```

### Comparing `mkdocs-techdocs-diamond-1.0.0/.devcontainer/devcontainer.json` & `mkdocs_techdocs_diamond-1.0.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `mkdocs-techdocs-diamond-1.0.0/.github/workflows/code.yml` & `mkdocs_techdocs_diamond-1.0.1/.github/workflows/code.yml`

 * *Files 15% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.10", "3.11", "3.12"]
     steps:
       - name: Checkout
-        uses: actions/checkout@v4.1.1
+        uses: actions/checkout@v4.1.2
 
       - name: Setup Python
-        uses: actions/setup-python@v5.0.0
+        uses: actions/setup-python@v5.1.0
         with:
           python-version: ${{ matrix.python-version }} 
 
       - name: Install dependencies
         run: pip install -e .[dev]
 
       - name: Lint
@@ -32,18 +32,18 @@
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.10", "3.11", "3.12"]
     steps:
       - name: Checkout
-        uses: actions/checkout@v4.1.1
+        uses: actions/checkout@v4.1.2
 
       - name: Setup Python
-        uses: actions/setup-python@v5.0.0
+        uses: actions/setup-python@v5.1.0
         with:
           python-version: ${{ matrix.python-version }} 
 
       - name: Install dependencies
         run: pip install .
 
       - name: Build Test Site
@@ -52,26 +52,26 @@
 
   dist:
     # Deduplicate jobs from pull requests and branch pushes within the same repo.
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     runs-on: "ubuntu-latest"
     steps:
       - name: Checkout
-        uses: actions/checkout@v4.1.1
+        uses: actions/checkout@v4.1.2
 
       - name: Build sdist and wheel
         run: |
           export SOURCE_DATE_EPOCH=$(git log -1 --pretty=%ct) && \
           pipx run build
 
       - name: Check for packaging errors
         run: pipx run twine check --strict dist/*
 
       - name: Upload sdist and wheel as artifacts
-        uses: actions/upload-artifact@v4.0.0
+        uses: actions/upload-artifact@v4.3.1
         with:
           name: dist
           path: dist
 
   release:
     # pull requests are a duplicate of a branch push if within the same repo.
     needs: [lint, canary, dist]
@@ -79,25 +79,23 @@
     runs-on: ubuntu-latest
     permissions:
       id-token: write
       contents: write
     environment: release
     steps:
       - name: Download wheel and lockfiles
-        uses: actions/download-artifact@v4.1.0
+        uses: actions/download-artifact@v4.1.4
         with:
           name: dist
           path: dist
 
       - name: Github Release
-        # We pin to the SHA, not the tag, for security reasons.
-        # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
-        uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844 # v0.1.15
+        uses: softprops/action-gh-release@v2.0.4
         with:
           prerelease: ${{ contains(github.ref_name, 'a') || contains(github.ref_name, 'b') || contains(github.ref_name, 'rc') }}
           files: dist/*
           generate_release_notes: true
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.11
+        uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `mkdocs-techdocs-diamond-1.0.0/.pre-commit-config.yaml` & `mkdocs_techdocs_diamond-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mkdocs-techdocs-diamond-1.0.0/LICENSE` & `mkdocs_techdocs_diamond-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-techdocs-diamond-1.0.0/PKG-INFO` & `mkdocs_techdocs_diamond-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-techdocs-diamond
-Version: 1.0.0
+Version: 1.0.1
 Summary: An Mkdocs plugin for configuring Diamond Techdocs sites
 Author-email: Garry O'Donnell <garry.o'donnell@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,15 +209,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mkdocs
+Requires-Dist: mkdocs<1.6.0
 Requires-Dist: mkdocs-awesome-pages-plugin
 Requires-Dist: mkdocs-include-markdown-plugin
 Requires-Dist: mkdocs-material
 Requires-Dist: mdx_truly_sane_lists
 Requires-Dist: pymdown-extensions
 Requires-Dist: pygments
 Provides-Extra: dev
```

### Comparing `mkdocs-techdocs-diamond-1.0.0/pyproject.toml` & `mkdocs_techdocs_diamond-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 description = "An Mkdocs plugin for configuring Diamond Techdocs sites"
 dependencies = [
-    "mkdocs",
+    "mkdocs<1.6.0",
     "mkdocs-awesome-pages-plugin",
     "mkdocs-include-markdown-plugin",
     "mkdocs-material",
     "mdx_truly_sane_lists",
     "pymdown-extensions",
     "pygments",
 ]
```

### Comparing `mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond/config.yml` & `mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/config.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond/plugin.py` & `mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond.egg-info/PKG-INFO` & `mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-techdocs-diamond
-Version: 1.0.0
+Version: 1.0.1
 Summary: An Mkdocs plugin for configuring Diamond Techdocs sites
 Author-email: Garry O'Donnell <garry.o'donnell@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,15 +209,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mkdocs
+Requires-Dist: mkdocs<1.6.0
 Requires-Dist: mkdocs-awesome-pages-plugin
 Requires-Dist: mkdocs-include-markdown-plugin
 Requires-Dist: mkdocs-material
 Requires-Dist: mdx_truly_sane_lists
 Requires-Dist: pymdown-extensions
 Requires-Dist: pygments
 Provides-Extra: dev
```

### Comparing `mkdocs-techdocs-diamond-1.0.0/src/mkdocs_techdocs_diamond.egg-info/SOURCES.txt` & `mkdocs_techdocs_diamond-1.0.1/src/mkdocs_techdocs_diamond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

