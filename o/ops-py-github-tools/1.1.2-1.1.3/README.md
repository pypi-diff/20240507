# Comparing `tmp/ops-py-github-tools-1.1.2.tar.gz` & `tmp/ops_py_github_tools-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-py-github-tools-1.1.2.tar", last modified: Fri Feb 23 14:00:42 2024, max compression
+gzip compressed data, was "ops_py_github_tools-1.1.3.tar", last modified: Tue May  7 09:23:40 2024, max compression
```

## Comparing `ops-py-github-tools-1.1.2.tar` & `ops_py_github_tools-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:00:42.328571 ops-py-github-tools-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-23 14:00:34.000000 ops-py-github-tools-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-23 14:00:42.328571 ops-py-github-tools-1.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:00:42.328571 ops-py-github-tools-1.1.2/github_tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)      124 2024-02-23 14:00:28.000000 ops-py-github-tools-1.1.2/github_tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3570 2024-02-23 14:00:28.000000 ops-py-github-tools-1.1.2/github_tools/gh_create_milestone.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11170 2024-02-23 14:00:28.000000 ops-py-github-tools-1.1.2/github_tools/gh_issue_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4956 2024-02-23 14:00:28.000000 ops-py-github-tools-1.1.2/github_tools/gh_repos.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4583 2024-02-23 14:00:28.000000 ops-py-github-tools-1.1.2/github_tools/github_issue_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1092 2024-02-23 14:00:28.000000 ops-py-github-tools-1.1.2/github_tools/github_tools_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:00:42.328571 ops-py-github-tools-1.1.2/ops_py_github_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-23 14:00:42.000000 ops-py-github-tools-1.1.2/ops_py_github_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-23 14:00:42.000000 ops-py-github-tools-1.1.2/ops_py_github_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 14:00:42.000000 ops-py-github-tools-1.1.2/ops_py_github_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-23 14:00:42.000000 ops-py-github-tools-1.1.2/ops_py_github_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-23 14:00:42.000000 ops-py-github-tools-1.1.2/ops_py_github_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-23 14:00:34.000000 ops-py-github-tools-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-23 14:00:28.000000 ops-py-github-tools-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 14:00:42.328571 ops-py-github-tools-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-23 14:00:34.000000 ops-py-github-tools-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:40.711229 ops_py_github_tools-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-07 09:23:38.000000 ops_py_github_tools-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-07 09:23:40.707229 ops_py_github_tools-1.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:40.707229 ops_py_github_tools-1.1.3/github_tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      124 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/github_tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3570 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/github_tools/gh_create_milestone.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11170 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/github_tools/gh_issue_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4956 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/github_tools/gh_repos.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4584 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/github_tools/github_issue_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1092 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/github_tools/github_tools_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:23:40.707229 ops_py_github_tools-1.1.3/ops_py_github_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-07 09:23:40.000000 ops_py_github_tools-1.1.3/ops_py_github_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 09:23:40.000000 ops_py_github_tools-1.1.3/ops_py_github_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:23:40.000000 ops_py_github_tools-1.1.3/ops_py_github_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 09:23:40.000000 ops_py_github_tools-1.1.3/ops_py_github_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 09:23:40.000000 ops_py_github_tools-1.1.3/ops_py_github_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 09:23:38.000000 ops_py_github_tools-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-07 09:23:38.000000 ops_py_github_tools-1.1.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 09:23:35.000000 ops_py_github_tools-1.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:23:40.711229 ops_py_github_tools-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 09:23:38.000000 ops_py_github_tools-1.1.3/setup.py
```

### Comparing `ops-py-github-tools-1.1.2/LICENSE` & `ops_py_github_tools-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ops-py-github-tools-1.1.2/github_tools/gh_create_milestone.py` & `ops_py_github_tools-1.1.3/github_tools/gh_create_milestone.py`

 * *Files identical despite different names*

### Comparing `ops-py-github-tools-1.1.2/github_tools/gh_issue_templates.py` & `ops_py_github_tools-1.1.3/github_tools/gh_issue_templates.py`

 * *Files identical despite different names*

### Comparing `ops-py-github-tools-1.1.2/github_tools/gh_repos.py` & `ops_py_github_tools-1.1.3/github_tools/gh_repos.py`

 * *Files identical despite different names*

### Comparing `ops-py-github-tools-1.1.2/github_tools/github_issue_templates.py` & `ops_py_github_tools-1.1.3/github_tools/github_issue_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from gh_issue_templates import IssueTemplates
 
 
 ########################################################################################################################
 
 
 def main():
-    """Creates a issue_template object and passes the argparse arguments.
+    """Creates an issue_template object and passes the argparse arguments.
     Prints the output from the issue_template.get_template method"""
     
     logging.basicConfig(format='%(asctime)s - %(levelname)s - %(module)s - %(funcName)s - %(message)s', level=logging.INFO)
 
     # The list of key vaults to check passed as command line arguments
     parser = argparse.ArgumentParser()
     parser.add_argument("-T", "--title", type=str,
```

### Comparing `ops-py-github-tools-1.1.2/github_tools/github_tools_examples.py` & `ops_py_github_tools-1.1.3/github_tools/github_tools_examples.py`

 * *Files identical despite different names*

