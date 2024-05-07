# Comparing `tmp/test_behavior_curriculum-0.0.6.tar.gz` & `tmp/test_behavior_curriculum-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_behavior_curriculum-0.0.6.tar", last modified: Mon May  6 16:47:46 2024, max compression
+gzip compressed data, was "test_behavior_curriculum-0.0.7.tar", last modified: Tue May  7 17:37:55 2024, max compression
```

## Comparing `test_behavior_curriculum-0.0.6.tar` & `test_behavior_curriculum-0.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:47:46.801839 test_behavior_curriculum-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:47:46.793839 test_behavior_curriculum-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:47:46.793839 test_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:47:46.793839 test_behavior_curriculum-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/.github/workflows/init.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/.github/workflows/tag_publish_upload.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-06 16:47:46.797839 test_behavior_curriculum-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:47:46.797839 test_behavior_curriculum-0.0.6/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:47:46.797839 test_behavior_curriculum-0.0.6/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:47:46.797839 test_behavior_curriculum-0.0.6/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:47:46.801839 test_behavior_curriculum-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:47:46.793839 test_behavior_curriculum-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:47:46.797839 test_behavior_curriculum-0.0.6/src/test_behavior_curriculum/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 16:47:37.000000 test_behavior_curriculum-0.0.6/src/test_behavior_curriculum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/src/test_behavior_curriculum/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:47:46.797839 test_behavior_curriculum-0.0.6/src/test_behavior_curriculum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-06 16:47:46.000000 test_behavior_curriculum-0.0.6/src/test_behavior_curriculum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-06 16:47:46.000000 test_behavior_curriculum-0.0.6/src/test_behavior_curriculum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:47:46.000000 test_behavior_curriculum-0.0.6/src/test_behavior_curriculum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 16:47:46.000000 test_behavior_curriculum-0.0.6/src/test_behavior_curriculum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 16:47:46.000000 test_behavior_curriculum-0.0.6/src/test_behavior_curriculum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:47:46.797839 test_behavior_curriculum-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-06 16:47:36.000000 test_behavior_curriculum-0.0.6/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:55.240825 test_behavior_curriculum-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:55.232825 test_behavior_curriculum-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:55.232825 test_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:55.236825 test_behavior_curriculum-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/.github/workflows/init.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/.github/workflows/tag_publish_upload.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-07 17:37:55.240825 test_behavior_curriculum-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:55.236825 test_behavior_curriculum-0.0.7/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:55.236825 test_behavior_curriculum-0.0.7/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:55.236825 test_behavior_curriculum-0.0.7/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:37:55.240825 test_behavior_curriculum-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:55.232825 test_behavior_curriculum-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:55.236825 test_behavior_curriculum-0.0.7/src/test_behavior_curriculum/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 17:37:46.000000 test_behavior_curriculum-0.0.7/src/test_behavior_curriculum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/src/test_behavior_curriculum/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:55.236825 test_behavior_curriculum-0.0.7/src/test_behavior_curriculum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-07 17:37:55.000000 test_behavior_curriculum-0.0.7/src/test_behavior_curriculum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-07 17:37:55.000000 test_behavior_curriculum-0.0.7/src/test_behavior_curriculum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:37:55.000000 test_behavior_curriculum-0.0.7/src/test_behavior_curriculum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 17:37:55.000000 test_behavior_curriculum-0.0.7/src/test_behavior_curriculum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 17:37:55.000000 test_behavior_curriculum-0.0.7/src/test_behavior_curriculum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:37:55.236825 test_behavior_curriculum-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-07 17:37:45.000000 test_behavior_curriculum-0.0.7/tests/test_example.py
```

### Comparing `test_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md` & `test_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/feature_request.md` & `test_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/user-story.md` & `test_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/.github/workflows/init.yml` & `test_behavior_curriculum-0.0.7/.github/workflows/init.yml`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/.github/workflows/tag_publish_upload.yml` & `test_behavior_curriculum-0.0.7/.github/workflows/tag_publish_upload.yml`

 * *Files 0% similar despite different names*

```diff
@@ -123,8 +123,8 @@
           python -m pip install awscli
       - name: Upload curriculum and curriculum diagram
         # Upload curriculum if TEMP_DIR is not empty.
         run: |
           python -m $REPO_NAME.upload $TEMP_DIR
           if [ -z "$(ls -A $TEMP_DIR)" ]; then
             aws s3 sync $TEMP_DIR s3://$AWS_BEHAVIOR_CURRICULUM_BUCKET/$S3_PREFIX/$REPO_NAME/$VERSION
-          fi
+          fi
```

### Comparing `test_behavior_curriculum-0.0.6/.github/workflows/test_and_lint.yml` & `test_behavior_curriculum-0.0.7/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/.gitignore` & `test_behavior_curriculum-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/LICENSE` & `test_behavior_curriculum-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/PKG-INFO` & `test_behavior_curriculum-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-behavior-curriculum
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generated from aind-behavior-curriculum-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `test_behavior_curriculum-0.0.6/README.md` & `test_behavior_curriculum-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/doc_template/Makefile` & `test_behavior_curriculum-0.0.7/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/doc_template/make.bat` & `test_behavior_curriculum-0.0.7/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/doc_template/source/_static/dark-logo.svg` & `test_behavior_curriculum-0.0.7/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/doc_template/source/_static/favicon.ico` & `test_behavior_curriculum-0.0.7/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/doc_template/source/_static/light-logo.svg` & `test_behavior_curriculum-0.0.7/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/doc_template/source/conf.py` & `test_behavior_curriculum-0.0.7/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/pyproject.toml` & `test_behavior_curriculum-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.6/src/test_behavior_curriculum.egg-info/PKG-INFO` & `test_behavior_curriculum-0.0.7/src/test_behavior_curriculum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-behavior-curriculum
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generated from aind-behavior-curriculum-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `test_behavior_curriculum-0.0.6/src/test_behavior_curriculum.egg-info/SOURCES.txt` & `test_behavior_curriculum-0.0.7/src/test_behavior_curriculum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

