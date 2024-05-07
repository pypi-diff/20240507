# Comparing `tmp/mojo_interfaces-1.3.3.tar.gz` & `tmp/mojo_interfaces-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_interfaces-1.3.3.tar", max compression
+gzip compressed data, was "mojo_interfaces-1.3.4.tar", max compression
```

## Comparing `mojo_interfaces-1.3.3.tar` & `mojo_interfaces-1.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1556 2024-05-02 06:19:49.820698 mojo_interfaces-1.3.3/LICENSE.txt
--rw-r--r--   0        0        0      850 2024-01-26 02:53:59.487659 mojo_interfaces-1.3.3/README.rst
--rw-r--r--   0        0        0      688 2024-05-06 01:44:54.396917 mojo_interfaces-1.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-26 02:53:59.488973 mojo_interfaces-1.3.3/source/packages/mojo/interfaces/__init__.py
--rw-r--r--   0        0        0     1375 2024-05-02 06:18:52.315984 mojo_interfaces-1.3.3/source/packages/mojo/interfaces/iexcludefilter.py
--rw-r--r--   0        0        0     1368 2024-05-02 06:18:57.168205 mojo_interfaces-1.3.3/source/packages/mojo/interfaces/iincludefilter.py
--rw-r--r--   0        0        0      586 2024-05-02 06:19:01.979269 mojo_interfaces-1.3.3/source/packages/mojo/interfaces/iserializable.py
--rw-r--r--   0        0        0     6094 2024-05-02 06:19:10.706809 mojo_interfaces-1.3.3/source/packages/mojo/interfaces/isystemcontext.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 mojo_interfaces-1.3.3/setup.py
--rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 mojo_interfaces-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1556 2024-05-02 06:19:49.820698 mojo_interfaces-1.3.4/LICENSE.txt
+-rw-r--r--   0        0        0      850 2024-01-26 02:53:59.487659 mojo_interfaces-1.3.4/README.rst
+-rw-r--r--   0        0        0      718 2024-05-07 16:00:19.384715 mojo_interfaces-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:59.488973 mojo_interfaces-1.3.4/source/packages/mojo/interfaces/__init__.py
+-rw-r--r--   0        0        0     1375 2024-05-02 06:18:52.315984 mojo_interfaces-1.3.4/source/packages/mojo/interfaces/iexcludefilter.py
+-rw-r--r--   0        0        0     1368 2024-05-02 06:18:57.168205 mojo_interfaces-1.3.4/source/packages/mojo/interfaces/iincludefilter.py
+-rw-r--r--   0        0        0      586 2024-05-02 06:19:01.979269 mojo_interfaces-1.3.4/source/packages/mojo/interfaces/iserializable.py
+-rw-r--r--   0        0        0     6094 2024-05-02 06:19:10.706809 mojo_interfaces-1.3.4/source/packages/mojo/interfaces/isystemcontext.py
+-rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 mojo_interfaces-1.3.4/setup.py
+-rw-r--r--   0        0        0     1518 1970-01-01 00:00:00.000000 mojo_interfaces-1.3.4/PKG-INFO
```

### Comparing `mojo_interfaces-1.3.3/LICENSE.txt` & `mojo_interfaces-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_interfaces-1.3.3/README.rst` & `mojo_interfaces-1.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `mojo_interfaces-1.3.3/source/packages/mojo/interfaces/iexcludefilter.py` & `mojo_interfaces-1.3.4/source/packages/mojo/interfaces/iexcludefilter.py`

 * *Files identical despite different names*

### Comparing `mojo_interfaces-1.3.3/source/packages/mojo/interfaces/iincludefilter.py` & `mojo_interfaces-1.3.4/source/packages/mojo/interfaces/iincludefilter.py`

 * *Files identical despite different names*

### Comparing `mojo_interfaces-1.3.3/source/packages/mojo/interfaces/iserializable.py` & `mojo_interfaces-1.3.4/source/packages/mojo/interfaces/iserializable.py`

 * *Files identical despite different names*

### Comparing `mojo_interfaces-1.3.3/source/packages/mojo/interfaces/isystemcontext.py` & `mojo_interfaces-1.3.4/source/packages/mojo/interfaces/isystemcontext.py`

 * *Files identical despite different names*

### Comparing `mojo_interfaces-1.3.3/setup.py` & `mojo_interfaces-1.3.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,25 +6,29 @@
 
 packages = \
 ['mojo', 'mojo.interfaces']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['typing-extensions>=4.11.0,<5.0.0']
+
 setup_kwargs = {
     'name': 'mojo-interfaces',
-    'version': '1.3.3',
+    'version': '1.3.4',
     'description': 'Automation Mojo Interfaces Package',
     'long_description': "=======================\nmojo-interfaces\n=======================\nThis is a package that contains a collection or library of interfaces that can be shared by other packages.\n\n=================\nCode Organization\n=================\n* .vscode - Common tasks\n* development - This is where the runtime environment scripts are located\n* repository-setup - Scripts for homing your repository and to your checkout and machine setup\n* userguide - Where you put your user guide\n* source/packages - Put your root folder here 'source/packages/(root-module-folder)'\n* source/sphinx - This is the Sphinx documentation folder\n* workspaces - This is where you add VSCode workspaces templates and where workspaces show up when homed.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n",
     'author': 'Myron W Walker',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mojo_interfaces-1.3.3/PKG-INFO` & `mojo_interfaces-1.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: mojo-interfaces
-Version: 1.3.3
+Version: 1.3.4
 Summary: Automation Mojo Interfaces Package
 License: LICENSE.txt
 Keywords: python
 Author: Myron W Walker
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Description-Content-Type: text/x-rst
 
 =======================
 mojo-interfaces
 =======================
 This is a package that contains a collection or library of interfaces that can be shared by other packages.
```

