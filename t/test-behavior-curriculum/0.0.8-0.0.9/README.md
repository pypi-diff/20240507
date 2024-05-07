# Comparing `tmp/test_behavior_curriculum-0.0.8.tar.gz` & `tmp/test_behavior_curriculum-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_behavior_curriculum-0.0.8.tar", last modified: Tue May  7 17:59:08 2024, max compression
+gzip compressed data, was "test_behavior_curriculum-0.0.9.tar", last modified: Tue May  7 18:18:30 2024, max compression
```

## Comparing `test_behavior_curriculum-0.0.8.tar` & `test_behavior_curriculum-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:08.521131 test_behavior_curriculum-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:08.509131 test_behavior_curriculum-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:08.513131 test_behavior_curriculum-0.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:08.517131 test_behavior_curriculum-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/.github/workflows/init.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/.github/workflows/tag_publish_upload.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-07 17:59:08.521131 test_behavior_curriculum-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:08.517131 test_behavior_curriculum-0.0.8/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:08.517131 test_behavior_curriculum-0.0.8/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:08.517131 test_behavior_curriculum-0.0.8/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:59:08.521131 test_behavior_curriculum-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:08.513131 test_behavior_curriculum-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:08.517131 test_behavior_curriculum-0.0.8/src/test_behavior_curriculum/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 17:58:58.000000 test_behavior_curriculum-0.0.8/src/test_behavior_curriculum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/src/test_behavior_curriculum/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:08.517131 test_behavior_curriculum-0.0.8/src/test_behavior_curriculum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-07 17:59:08.000000 test_behavior_curriculum-0.0.8/src/test_behavior_curriculum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-07 17:59:08.000000 test_behavior_curriculum-0.0.8/src/test_behavior_curriculum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:59:08.000000 test_behavior_curriculum-0.0.8/src/test_behavior_curriculum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 17:59:08.000000 test_behavior_curriculum-0.0.8/src/test_behavior_curriculum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 17:59:08.000000 test_behavior_curriculum-0.0.8/src/test_behavior_curriculum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:08.517131 test_behavior_curriculum-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-07 17:58:57.000000 test_behavior_curriculum-0.0.8/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:30.184497 test_behavior_curriculum-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:30.172497 test_behavior_curriculum-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:30.176497 test_behavior_curriculum-0.0.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:30.176497 test_behavior_curriculum-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/.github/workflows/init.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/.github/workflows/tag_publish_upload.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-07 18:18:30.184497 test_behavior_curriculum-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:30.176497 test_behavior_curriculum-0.0.9/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:30.180497 test_behavior_curriculum-0.0.9/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:30.180497 test_behavior_curriculum-0.0.9/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 18:18:30.184497 test_behavior_curriculum-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:30.172497 test_behavior_curriculum-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:30.180497 test_behavior_curriculum-0.0.9/src/test_behavior_curriculum/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/src/test_behavior_curriculum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/src/test_behavior_curriculum/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:30.180497 test_behavior_curriculum-0.0.9/src/test_behavior_curriculum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-07 18:18:30.000000 test_behavior_curriculum-0.0.9/src/test_behavior_curriculum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-07 18:18:30.000000 test_behavior_curriculum-0.0.9/src/test_behavior_curriculum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:18:30.000000 test_behavior_curriculum-0.0.9/src/test_behavior_curriculum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 18:18:30.000000 test_behavior_curriculum-0.0.9/src/test_behavior_curriculum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 18:18:30.000000 test_behavior_curriculum-0.0.9/src/test_behavior_curriculum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:18:30.180497 test_behavior_curriculum-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-07 18:18:19.000000 test_behavior_curriculum-0.0.9/tests/test_example.py
```

### Comparing `test_behavior_curriculum-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md` & `test_behavior_curriculum-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md` & `test_behavior_curriculum-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/.github/ISSUE_TEMPLATE/user-story.md` & `test_behavior_curriculum-0.0.9/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/.github/workflows/init.yml` & `test_behavior_curriculum-0.0.9/.github/workflows/init.yml`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/.github/workflows/tag_publish_upload.yml` & `test_behavior_curriculum-0.0.9/.github/workflows/tag_publish_upload.yml`

 * *Files 1% similar despite different names*

```diff
@@ -120,13 +120,13 @@
         run: |
           sudo apt install graphviz libgraphviz-dev -y
           python -m pip install -e .
           python -m pip install awscli
       - name: Upload curriculum and curriculum diagram
         # Upload curriculum if TEMP_DIR is not empty.
         run: |
-          module_name=$(echo "$REPO_NAME" | awk -F '/' '{print $2}')
+          module_name=$(echo "$REPO_NAME" | awk -F '/' '{print $2}' | tr '-' '_')
           python -m $module_name.upload $TEMP_DIR
 
           if [ -z "$(ls -A $TEMP_DIR)" ]; then
             aws s3 sync $TEMP_DIR s3://$AWS_BEHAVIOR_CURRICULUM_BUCKET/$S3_PREFIX/$REPO_NAME/$VERSION
           fi
```

### Comparing `test_behavior_curriculum-0.0.8/.github/workflows/test_and_lint.yml` & `test_behavior_curriculum-0.0.9/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/.gitignore` & `test_behavior_curriculum-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/LICENSE` & `test_behavior_curriculum-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/PKG-INFO` & `test_behavior_curriculum-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-behavior-curriculum
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generated from aind-behavior-curriculum-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `test_behavior_curriculum-0.0.8/README.md` & `test_behavior_curriculum-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/doc_template/Makefile` & `test_behavior_curriculum-0.0.9/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/doc_template/make.bat` & `test_behavior_curriculum-0.0.9/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/doc_template/source/_static/dark-logo.svg` & `test_behavior_curriculum-0.0.9/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/doc_template/source/_static/favicon.ico` & `test_behavior_curriculum-0.0.9/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/doc_template/source/_static/light-logo.svg` & `test_behavior_curriculum-0.0.9/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/doc_template/source/conf.py` & `test_behavior_curriculum-0.0.9/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/pyproject.toml` & `test_behavior_curriculum-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.8/src/test_behavior_curriculum.egg-info/PKG-INFO` & `test_behavior_curriculum-0.0.9/src/test_behavior_curriculum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-behavior-curriculum
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generated from aind-behavior-curriculum-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `test_behavior_curriculum-0.0.8/src/test_behavior_curriculum.egg-info/SOURCES.txt` & `test_behavior_curriculum-0.0.9/src/test_behavior_curriculum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

