# Comparing `tmp/sinaraml_jupyter-2024.4.22.tar.gz` & `tmp/sinaraml_jupyter-2024.5.7.tar.gz`

## Comparing `sinaraml_jupyter-2024.4.22.tar` & `sinaraml_jupyter-2024.5.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/sinaraml_jupyter/__init__.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/sinaraml_jupyter/_version.py
--rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/sinaraml_jupyter/org_manager.py
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/sinaraml_jupyter/sinaraml_jupyter.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/LICENSE
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/README.md
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/pyproject.toml
--rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/sinaraml_jupyter/__init__.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/sinaraml_jupyter/_version.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/sinaraml_jupyter/org_manager.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/sinaraml_jupyter/sinaraml_jupyter.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/LICENSE
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/README.md
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/pyproject.toml
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.5.7/PKG-INFO
```

### Comparing `sinaraml_jupyter-2024.4.22/sinaraml_jupyter/org_manager.py` & `sinaraml_jupyter-2024.5.7/sinaraml_jupyter/org_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,18 @@
     @staticmethod
     def add_list_handler(root_parser):
         list_parser = root_parser.add_parser('list', help='list all installed organization cli and platforms')
         list_parser.set_defaults(func=SinaraOrgManager.list_platforms)
 
     @staticmethod
     def get_orgs_dir(org_name = None):
-        #dir = Path(Path.home(), '.sinaraml', 'orgs')
-        dir = Path(Path.home(), 'work', 'orgs')
+        if os.environ.get('SINARA_DEBUG') == '1':
+            dir = Path(Path.home(), 'work', 'orgs')
+        else:
+            dir = Path(Path.home(), '.sinaraml', 'orgs')
         if org_name:
             dir = Path(dir, org_name)
         return dir
 
     @staticmethod
     def get_orgs():
         result = []
```

### Comparing `sinaraml_jupyter-2024.4.22/sinaraml_jupyter/sinaraml_jupyter.py` & `sinaraml_jupyter-2024.5.7/sinaraml_jupyter/sinaraml_jupyter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 #!/usr/bin/env python3
 
 import argparse
+import json
 import logging
+import os
 import sys
 from dataclasses import dataclass
 from .org_manager import SinaraOrgManager
 
 
 @dataclass
 class Gitref:
     gitref: str
 
 def check_any_org_exists():
     if not SinaraOrgManager.check_last_update():
-        args = Gitref(gitref = "https://github.com/4-DS/mlops_jupyter_organization.git")
+        jupyter_cli_org = "https://github.com/4-DS/mlops_jupyter_organization.git"
+        if os.environ.get('SINARA_ORG'):
+            platform = os.environ.get('SINARA_PLATFORM')
+            sinara_org = json.loads(os.environ.get('SINARA_ORG').replace("'", '"'))
+            body = [body for body in sinara_org["cli_bodies"] if platform in body["platform_names"]]
+            if body and "mlops_jupyter_organization" in body[0].keys():
+                jupyter_cli_org = body[0]["mlops_jupyter_organization"]
+            
+        args = Gitref(gitref = jupyter_cli_org)
         SinaraOrgManager.install_from_git(args)
 
 def init_cli(root_parser, subject_parser, platform=None):
     root_parser.subjects = []
 
     SinaraOrgManager.add_command_handlers(root_parser, subject_parser)
```

### Comparing `sinaraml_jupyter-2024.4.22/.gitignore` & `sinaraml_jupyter-2024.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `sinaraml_jupyter-2024.4.22/LICENSE` & `sinaraml_jupyter-2024.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sinaraml_jupyter-2024.4.22/README.md` & `sinaraml_jupyter-2024.5.7/README.md`

 * *Files identical despite different names*

### Comparing `sinaraml_jupyter-2024.4.22/pyproject.toml` & `sinaraml_jupyter-2024.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sinaraml_jupyter-2024.4.22/PKG-INFO` & `sinaraml_jupyter-2024.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sinaraml_jupyter
-Version: 2024.4.22
+Version: 2024.5.7
 Summary: SinaraML Jupyter CLI
 Project-URL: Homepage, https://github.com/4-DS/sinaraml_jupyter
 Author-email: sinaraml <sinaraml.official@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 SinaraML
```

