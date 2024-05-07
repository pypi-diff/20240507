# Comparing `tmp/behaverse-0.0.2.dev4.tar.gz` & `tmp/behaverse-0.0.3.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behaverse-0.0.2.dev4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "behaverse-0.0.3.dev5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `behaverse-0.0.2.dev4.tar` & `behaverse-0.0.3.dev5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1240 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      100 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/.gitignore
--rw-r--r--   0        0        0      158 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/.pypirc
--rw-r--r--   0        0        0      375 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/.vscode/settings.json
--rw-r--r--   0        0        0     1071 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/LICENSE
--rw-r--r--   0        0        0      890 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/README.md
--rw-r--r--   0        0        0       54 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/docs/.gitignore
--rw-r--r--   0        0        0       22 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/docs/_extensions/machow/interlinks/.gitignore
--rw-r--r--   0        0        0      126 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/docs/_extensions/machow/interlinks/_extension.yml
--rw-r--r--   0        0        0     6853 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/docs/_extensions/machow/interlinks/interlinks.lua
--rw-r--r--   0        0        0     1392 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/docs/_quarto.yml
--rw-r--r--   0        0        0     1172 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/docs/getting_started.qmd
--rw-r--r--   0        0        0      176 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/docs/index.qmd
--rw-r--r--   0        0        0      209 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/environment.yml
--rw-r--r--   0        0        0     1627 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/pyproject.toml
--rw-r--r--   0        0        0      487 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/__init__.py
--rw-r--r--   0        0        0       27 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/conftest.py
--rw-r--r--   0        0        0     6773 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/dataset.py
--rw-r--r--   0        0        0      238 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/dataset_description.py
--rw-r--r--   0        0        0     1369 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/dataset_test.py
--rw-r--r--   0        0        0     2487 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/functional.py
--rw-r--r--   0        0        0       28 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/functions_test.py
--rw-r--r--   0        0        0     3722 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/utils.py
--rw-r--r--   0        0        0      178 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/utils_test.py
--rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 behaverse-0.0.2.dev4/PKG-INFO
+-rw-r--r--   0        0        0     1654 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/.github/workflows/docs-publish.yml
+-rw-r--r--   0        0        0     1243 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      100 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/.gitignore
+-rw-r--r--   0        0        0      158 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/.pypirc
+-rw-r--r--   0        0        0      375 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/.vscode/settings.json
+-rw-r--r--   0        0        0     1071 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/LICENSE
+-rw-r--r--   0        0        0      890 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/README.md
+-rw-r--r--   0        0        0       54 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/docs/.gitignore
+-rw-r--r--   0        0        0       22 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/docs/_extensions/machow/interlinks/.gitignore
+-rw-r--r--   0        0        0      126 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/docs/_extensions/machow/interlinks/_extension.yml
+-rw-r--r--   0        0        0     6853 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/docs/_extensions/machow/interlinks/interlinks.lua
+-rw-r--r--   0        0        0     1392 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/docs/_quarto.yml
+-rw-r--r--   0        0        0     1147 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/docs/getting_started.qmd
+-rw-r--r--   0        0        0      176 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/docs/index.qmd
+-rw-r--r--   0        0        0      209 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/environment.yml
+-rw-r--r--   0        0        0     1627 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/src/behaverse/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/src/behaverse/conftest.py
+-rw-r--r--   0        0        0     6773 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/src/behaverse/dataset.py
+-rw-r--r--   0        0        0      238 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/src/behaverse/dataset_description.py
+-rw-r--r--   0        0        0     1369 2024-05-07 05:00:25.477647 behaverse-0.0.3.dev5/src/behaverse/dataset_test.py
+-rw-r--r--   0        0        0     2487 2024-05-07 05:00:25.481648 behaverse-0.0.3.dev5/src/behaverse/functional.py
+-rw-r--r--   0        0        0       28 2024-05-07 05:00:25.481648 behaverse-0.0.3.dev5/src/behaverse/functions_test.py
+-rw-r--r--   0        0        0     3722 2024-05-07 05:00:25.481648 behaverse-0.0.3.dev5/src/behaverse/utils.py
+-rw-r--r--   0        0        0      178 2024-05-07 05:00:25.481648 behaverse-0.0.3.dev5/src/behaverse/utils_test.py
+-rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 behaverse-0.0.3.dev5/PKG-INFO
```

### Comparing `behaverse-0.0.2.dev4/.github/workflows/pypi-publish.yml` & `behaverse-0.0.3.dev5/.github/workflows/pypi-publish.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Publish Python Package
+name: 📦 Publish Python Package
 
 on:
   release:
     types: [published]
   # push:
   #   branches:
   #     - python
@@ -43,9 +43,9 @@
       id-token: write  # for trusted publishing
     steps:
     - name: ⬇️ Download the distribution packages
       uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
-    - name: ⬆️ Publish distribution to PyPI
+    - name: 🚀 Publish distribution to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `behaverse-0.0.2.dev4/LICENSE` & `behaverse-0.0.3.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.2.dev4/README.md` & `behaverse-0.0.3.dev5/README.md`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.2.dev4/docs/_extensions/machow/interlinks/interlinks.lua` & `behaverse-0.0.3.dev5/docs/_extensions/machow/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.2.dev4/docs/_quarto.yml` & `behaverse-0.0.3.dev5/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.2.dev4/docs/getting_started.qmd` & `behaverse-0.0.3.dev5/docs/getting_started.qmd`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 ---
-title: "Getting Started"
 execute:
   echo: true
 jupyter: python3
 ---
 
 # Getting Started
```

### Comparing `behaverse-0.0.2.dev4/pyproject.toml` & `behaverse-0.0.3.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.2.dev4/src/behaverse/dataset.py` & `behaverse-0.0.3.dev5/src/behaverse/dataset.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.2.dev4/src/behaverse/dataset_test.py` & `behaverse-0.0.3.dev5/src/behaverse/dataset_test.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.2.dev4/src/behaverse/functional.py` & `behaverse-0.0.3.dev5/src/behaverse/functional.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.2.dev4/src/behaverse/utils.py` & `behaverse-0.0.3.dev5/src/behaverse/utils.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.2.dev4/PKG-INFO` & `behaverse-0.0.3.dev5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behaverse
-Version: 0.0.2.dev4
+Version: 0.0.3.dev5
 Summary: Behaverse Python Package.
 Author-email: xCIT Development Team <contact@xcit.org>
 Maintainer-email: Morteza Ansarinia <ansarinia@me.com>, Hoorieh Afkari <hoorieh.afkari@uni.lu>, Pedro Cardoso-Leite <pedro.cardosoleite@uni.lu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

