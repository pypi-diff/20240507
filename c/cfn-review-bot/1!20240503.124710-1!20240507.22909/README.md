# Comparing `tmp/cfn-review-bot-1!20240503.124710.tar.gz` & `tmp/cfn-review-bot-1!20240507.22909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn-review-bot-1!20240503.124710.tar", last modified: Fri May  3 12:47:55 2024, max compression
+gzip compressed data, was "cfn-review-bot-1!20240507.22909.tar", last modified: Tue May  7 02:29:57 2024, max compression
```

## Comparing `cfn-review-bot-1!20240503.124710.tar` & `cfn-review-bot-1!20240507.22909.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:47:55.370378 cfn-review-bot-1!20240503.124710/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-03 12:47:55.370378 cfn-review-bot-1!20240503.124710/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:47:55.366378 cfn-review-bot-1!20240503.124710/cfn_review_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3842 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/canonical.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/cfn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/dirloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/model.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-03 12:47:55.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/package-version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:47:55.370378 cfn-review-bot-1!20240503.124710/cfn_review_bot/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/schema/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/schema/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/schema/target.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/schema/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/schema/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/schema/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:47:55.370378 cfn-review-bot-1!20240503.124710/cfn_review_bot/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/templates/summary.md
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot/test_merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:47:55.366378 cfn-review-bot-1!20240503.124710/cfn_review_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-03 12:47:55.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-03 12:47:55.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:47:55.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 12:47:55.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 12:47:55.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 12:47:55.000000 cfn-review-bot-1!20240503.124710/cfn_review_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:47:55.370378 cfn-review-bot-1!20240503.124710/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-03 12:47:46.000000 cfn-review-bot-1!20240503.124710/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:29:57.514016 cfn-review-bot-1!20240507.22909/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-07 02:29:57.514016 cfn-review-bot-1!20240507.22909/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:29:57.514016 cfn-review-bot-1!20240507.22909/cfn_review_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3842 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/canonical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/cfn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/dirloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 02:29:57.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/package-version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:29:57.514016 cfn-review-bot-1!20240507.22909/cfn_review_bot/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/schema/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/schema/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/schema/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/schema/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/schema/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/schema/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:29:57.514016 cfn-review-bot-1!20240507.22909/cfn_review_bot/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/templates/summary.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot/test_merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:29:57.514016 cfn-review-bot-1!20240507.22909/cfn_review_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-07 02:29:57.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-07 02:29:57.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:29:57.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 02:29:57.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 02:29:57.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 02:29:57.000000 cfn-review-bot-1!20240507.22909/cfn_review_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:29:57.514016 cfn-review-bot-1!20240507.22909/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-07 02:29:45.000000 cfn-review-bot-1!20240507.22909/setup.py
```

### Comparing `cfn-review-bot-1!20240503.124710/LICENSE` & `cfn-review-bot-1!20240507.22909/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/PKG-INFO` & `cfn-review-bot-1!20240507.22909/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-review-bot
-Version: 1!20240503.124710
+Version: 1!20240507.22909
 Summary: CLI to manage CloudFormation stacks
 Home-page: https://github.com/biochimia/cfn-review-bot
 Author: João Abecasis
 Author-email: joao@abecasis.name
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/_version.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/_version.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/aws.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/aws.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/canonical.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/canonical.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/cfn.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/cfn.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/dirloader.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/dirloader.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/loader.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/loader.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/main.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/main.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/markdown.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/markdown.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/merge.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/merge.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/model.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/model.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/schema/stack.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/schema/stack.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/schema/target.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/schema/target.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/schema/template.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/schema/template.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/schema/test_stack.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/schema/test_stack.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/templates/summary.md` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/templates/summary.md`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot/test_merge.py` & `cfn-review-bot-1!20240507.22909/cfn_review_bot/test_merge.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot.egg-info/PKG-INFO` & `cfn-review-bot-1!20240507.22909/cfn_review_bot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-review-bot
-Version: 1!20240503.124710
+Version: 1!20240507.22909
 Summary: CLI to manage CloudFormation stacks
 Home-page: https://github.com/biochimia/cfn-review-bot
 Author: João Abecasis
 Author-email: joao@abecasis.name
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfn-review-bot-1!20240503.124710/cfn_review_bot.egg-info/SOURCES.txt` & `cfn-review-bot-1!20240507.22909/cfn_review_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.124710/setup.py` & `cfn-review-bot-1!20240507.22909/setup.py`

 * *Files identical despite different names*

