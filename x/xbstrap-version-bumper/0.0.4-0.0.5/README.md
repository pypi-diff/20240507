# Comparing `tmp/xbstrap_version_bumper-0.0.4.tar.gz` & `tmp/xbstrap_version_bumper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbstrap_version_bumper-0.0.4.tar", last modified: Sun May  5 23:13:27 2024, max compression
+gzip compressed data, was "xbstrap_version_bumper-0.0.5.tar", last modified: Tue May  7 14:07:32 2024, max compression
```

## Comparing `xbstrap_version_bumper-0.0.4.tar` & `xbstrap_version_bumper-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 23:13:27.793629 xbstrap_version_bumper-0.0.4/
--rw-r--r--   0 alexander  (1000) wheel      (998)     1075 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.4/LICENSE
--rw-r--r--   0 alexander  (1000) wheel      (998)      873 2024-05-05 23:13:27.793629 xbstrap_version_bumper-0.0.4/PKG-INFO
--rw-r--r--   0 alexander  (1000) wheel      (998)      181 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.4/README.md
--rw-r--r--   0 alexander  (1000) wheel      (998)      834 2024-05-05 23:13:10.000000 xbstrap_version_bumper-0.0.4/pyproject.toml
--rw-r--r--   0 alexander  (1000) wheel      (998)       38 2024-05-05 23:13:27.793629 xbstrap_version_bumper-0.0.4/setup.cfg
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 23:13:27.792629 xbstrap_version_bumper-0.0.4/src/
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 23:13:27.792629 xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper/
--rw-r--r--   0 alexander  (1000) wheel      (998)        0 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper/__init__.py
--rw-r--r--   0 alexander  (1000) wheel      (998)      102 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper/__main__.py
--rw-r--r--   0 alexander  (1000) wheel      (998)     8430 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper/linecounted_yaml.py
--rw-r--r--   0 alexander  (1000) wheel      (998)    13455 2024-05-05 23:10:50.000000 xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper/main.py
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 23:13:27.793629 xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper.egg-info/
--rw-r--r--   0 alexander  (1000) wheel      (998)      873 2024-05-05 23:13:27.000000 xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper.egg-info/PKG-INFO
--rw-r--r--   0 alexander  (1000) wheel      (998)      494 2024-05-05 23:13:27.000000 xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper.egg-info/SOURCES.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)        1 2024-05-05 23:13:27.000000 xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper.egg-info/dependency_links.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)       76 2024-05-05 23:13:27.000000 xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper.egg-info/entry_points.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)       73 2024-05-05 23:13:27.000000 xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper.egg-info/requires.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)       23 2024-05-05 23:13:27.000000 xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper.egg-info/top_level.txt
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-07 14:07:32.516481 xbstrap_version_bumper-0.0.5/
+-rw-r--r--   0 alexander  (1000) wheel      (998)     1075 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.5/LICENSE
+-rw-r--r--   0 alexander  (1000) wheel      (998)      873 2024-05-07 14:07:32.516481 xbstrap_version_bumper-0.0.5/PKG-INFO
+-rw-r--r--   0 alexander  (1000) wheel      (998)      181 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.5/README.md
+-rw-r--r--   0 alexander  (1000) wheel      (998)      834 2024-05-07 14:07:13.000000 xbstrap_version_bumper-0.0.5/pyproject.toml
+-rw-r--r--   0 alexander  (1000) wheel      (998)       38 2024-05-07 14:07:32.516481 xbstrap_version_bumper-0.0.5/setup.cfg
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-07 14:07:32.514481 xbstrap_version_bumper-0.0.5/src/
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-07 14:07:32.515481 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/
+-rw-r--r--   0 alexander  (1000) wheel      (998)        0 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/__init__.py
+-rw-r--r--   0 alexander  (1000) wheel      (998)      102 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/__main__.py
+-rw-r--r--   0 alexander  (1000) wheel      (998)     8430 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/linecounted_yaml.py
+-rw-r--r--   0 alexander  (1000) wheel      (998)    14538 2024-05-07 14:06:27.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/main.py
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-07 14:07:32.515481 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/
+-rw-r--r--   0 alexander  (1000) wheel      (998)      873 2024-05-07 14:07:32.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/PKG-INFO
+-rw-r--r--   0 alexander  (1000) wheel      (998)      494 2024-05-07 14:07:32.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)        1 2024-05-07 14:07:32.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)       76 2024-05-07 14:07:32.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/entry_points.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)       73 2024-05-07 14:07:32.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/requires.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)       23 2024-05-07 14:07:32.000000 xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/top_level.txt
```

### Comparing `xbstrap_version_bumper-0.0.4/LICENSE` & `xbstrap_version_bumper-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xbstrap_version_bumper-0.0.4/PKG-INFO` & `xbstrap_version_bumper-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbstrap_version_bumper
-Version: 0.0.4
+Version: 0.0.5
 Summary: xbstrap distro auto version bumper
 Author-email: Alexander Richards <electrodeyt@gmail.com>
 Project-URL: Homepage, https://github.com/ElectrodeYT/xbstrap_version_bumper
 Project-URL: Issues, https://github.com/ElectrodeYT/xbstrap_version_bumper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xbstrap_version_bumper-0.0.4/pyproject.toml` & `xbstrap_version_bumper-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xbstrap_version_bumper"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="Alexander Richards", email="electrodeyt@gmail.com" },
 ]
 requires-python = ">=3.8"
 description="xbstrap distro auto version bumper"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper/linecounted_yaml.py` & `xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/linecounted_yaml.py`

 * *Files identical despite different names*

### Comparing `xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper/main.py` & `xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,24 +32,39 @@
             cur_count / (max_count or 100.0),
             message or "NO MESSAGE",
         )
 
 
 class Change:
     def __init__(self, line: int, base_str: str = "", to_str: str = "",
-                 delete_line: bool = False, insert_line: bool = False, insert_auto_indent: bool = True):
+                 delete_line: bool = False, insert_line: bool = False, insert_auto_indent: bool = True,
+                 update_is_version=False):
         self.line = line
         self.base_str = base_str
         self.to_str = to_str
         self.delete_line = delete_line
         self.insert_line = insert_line
         self.insert_auto_indent = insert_auto_indent
+        self.update_is_version = update_is_version
 
     def apply(self, line):
-        return line.replace(self.base_str, self.to_str)
+        if not self.update_is_version:
+            return line.replace(self.base_str, self.to_str)
+
+        # This is a version, there are several ways these are commonly encoded in tags,
+        # try to support all of them
+        current_line = line
+        if self.base_str.replace('.', '_') in line:
+            current_line = current_line.replace(self.base_str.replace('.', '_'), self.to_str.replace('.', '_'))
+        if self.base_str.replace('.', '-') in line:
+            current_line = current_line.replace(self.base_str.replace('.', '-'), self.to_str.replace('.', '-'))
+        if self.base_str in line:
+            current_line = current_line.replace(self.base_str, self.to_str)
+
+        return current_line
 
 
 class StrapFile:
     def __init__(self, path):
         self.path = path
         self.yaml = global_yaml.load(pathlib.Path(path))
         self.changes = []
@@ -156,49 +171,47 @@
         changes = []
 
         old_version = source['version']
         print(f'--> Changing version of {source_name} from {old_version} to {new_version}')
         changes.append(Change(source['version'].lc.line, old_version, new_version))
 
         if 'url' in source:
-            new_url = source['url'].replace(old_version, new_version)
-            changes.append(Change(source['url'].lc.line, str(source['url']), new_url))
+            url_change = Change(source['url'].lc.line, old_version, new_version, update_is_version=True)
+            new_url = url_change.apply(source['url'])
+            changes.append(url_change)
 
         if 'checksum' in source:
             assert 'url' in source
             print(f'---> Attempting to download "{new_url}" to make new checksum')
             r = requests.get(new_url)
             new_checksum = hashlib.blake2b(r.content).hexdigest()
             changes.append(Change(source['checksum'].lc.line, str(source['checksum']), f'blake2b:{new_checksum}'))
             print(f'---> Updated checksum to blake2b:{new_checksum}')
 
         if 'filename' in source:
-            new_filename = source['filename'].replace(old_version, new_version)
-            changes.append(Change(source['filename'].lc.line, str(source['filename']), new_filename))
+            changes.append(Change(source['filename'].lc.line, old_version, new_version, update_is_version=True))
 
         if 'tag' in source:
-            new_tag = source['tag'].replace(old_version, new_version)
-            changes.append(Change(source['tag'].lc.line, str(source['tag']), new_tag))
+            changes.append(Change(source['tag'].lc.line, old_version, new_version, update_is_version=True))
 
         if 'extract_path' in source:
-            new_extract_path = source['extract_path'].replace(old_version, new_version)
-            changes.append(Change(source['extract_path'].lc.line, str(source['extract_path']), new_extract_path))
+            changes.append(Change(source['extract_path'].lc.line, old_version, new_version, update_is_version=True))
 
         self.__add_changes_to_stapfile(strapfile, changes)
 
     def modify_source_version(self, source_name, new_version):
         # Locate the source
         strapfile, source_in_package, source = self.__locate_source(source_name)
         self.__modify_source_impl(source, strapfile, source_name, new_version)
 
-    def __args_to_changes(self, args, from_str, to_str):
+    def __args_to_changes(self, args, from_str, to_str, update_is_version=False):
         changes = []
         for arg in args:
             if from_str in arg:
-                changes.append(Change(arg.lc.line, from_str, to_str))
+                changes.append(Change(arg.lc.line, from_str, to_str, update_is_version=update_is_version))
 
         return changes
 
     def modify_package_version(self, package_name, new_version):
         strapfile, package = self.__locate_package(package_name)
         changes = []
         if 'source' in package:
@@ -221,19 +234,19 @@
                 revision_insert_line_num = package['build'].lc.line - 1
             else:
                 raise Exception('Could not find a suitable place to insert revision tag')
             changes.append(Change(revision_insert_line_num, 'revision: 1', insert_line=True))
 
         if 'configure' in package:
             for configure in package['configure']:
-                changes += self.__args_to_changes(configure['args'], old_version, new_version)
+                changes += self.__args_to_changes(configure['args'], old_version, new_version, update_is_version=True)
 
         if 'build' in package:
             for build in package['build']:
-                changes += self.__args_to_changes(build['args'], old_version, new_version)
+                changes += self.__args_to_changes(build['args'], old_version, new_version, update_is_version=True)
 
         self.__add_changes_to_stapfile(strapfile, changes)
 
     def __get_latest_git_version(self, source):
         if 'git' not in source:
             return False
         g = git.cmd.Git()
@@ -280,33 +293,40 @@
     parser.add_argument('--set-version')
     parser.add_argument('--bootstrap-dir', required=True)
     parser.add_argument('--pull-from-master', action='store_true')
     parser.add_argument('--create-branch', action='store_true')
     parser.add_argument('--commiter-name')
     parser.add_argument('--commiter-email')
     parser.add_argument('--attempt-latest-version-autodetect', action='store_true')
+    parser.add_argument('--try-global-update', action='store_true')
     args = parser.parse_args()
 
     pprint(args)
 
+    if not args.try_global_update and args.to_modify is None:
+        parser.error('to_modify is needed if --try-global-update is not given')
+
+    if args.try_global_update and not args.attempt_latest_version_autodetect:
+        parser.error('--try-global-update requires --attempt-latest-version-autodetect')
+
     if not (args.set_version or args.attempt_latest_version_autodetect):
         parser.error('--set-version or --attempt-latest-version-autodetect is required')
 
     if args.create_branch and (args.commiter_name is None or args.commiter_email is None):
         parser.error('--commiter-name and --commiter-email is required when creating a branch')
 
     repo = Repo(args.bootstrap_dir)
     assert not repo.bare
 
     if args.pull_from_master:
         for remote in repo.remotes:
             if remote.name == 'origin':
                 # Pull master from origin
                 print(f'--> Pulling from origin ({remote.url})')
-                #remote.pull(progress=ProgressPrinter())
+                remote.pull(progress=ProgressPrinter())
 
     print('-> Reading bootstrap files')
     distro = Distro(args.bootstrap_dir)
 
     version_to_set = args.set_version
     if args.attempt_latest_version_autodetect:
         if not args.is_source:
```

### Comparing `xbstrap_version_bumper-0.0.4/src/xbstrap_version_bumper.egg-info/PKG-INFO` & `xbstrap_version_bumper-0.0.5/src/xbstrap_version_bumper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbstrap_version_bumper
-Version: 0.0.4
+Version: 0.0.5
 Summary: xbstrap distro auto version bumper
 Author-email: Alexander Richards <electrodeyt@gmail.com>
 Project-URL: Homepage, https://github.com/ElectrodeYT/xbstrap_version_bumper
 Project-URL: Issues, https://github.com/ElectrodeYT/xbstrap_version_bumper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

