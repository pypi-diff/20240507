# Comparing `tmp/ipynbname-2023.2.0.0.tar.gz` & `tmp/ipynbname-2024.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipynbname-2023.2.0.0.tar", last modified: Tue Jul 25 06:44:58 2023, max compression
+gzip compressed data, was "ipynbname-2024.1.0.0.tar", last modified: Tue May  7 07:44:55 2024, max compression
```

## Comparing `ipynbname-2023.2.0.0.tar` & `ipynbname-2024.1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 06:44:58.229221 ipynbname-2023.2.0.0/
--rw-rw-rw-   0        0        0     1092 2023-04-09 11:23:56.000000 ipynbname-2023.2.0.0/LICENSE
--rw-rw-rw-   0        0        0       19 2023-04-09 11:23:56.000000 ipynbname-2023.2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1891 2023-07-25 06:44:58.229221 ipynbname-2023.2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2023-07-25 06:32:44.000000 ipynbname-2023.2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 06:44:58.213135 ipynbname-2023.2.0.0/ipynbname/
--rw-rw-rw-   0        0        0     3749 2023-04-09 11:23:56.000000 ipynbname-2023.2.0.0/ipynbname/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:44:58.229221 ipynbname-2023.2.0.0/ipynbname.egg-info/
--rw-rw-rw-   0        0        0     1891 2023-07-25 06:44:58.000000 ipynbname-2023.2.0.0/ipynbname.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-25 06:44:58.000000 ipynbname-2023.2.0.0/ipynbname.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 06:44:58.000000 ipynbname-2023.2.0.0/ipynbname.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 06:44:58.000000 ipynbname-2023.2.0.0/ipynbname.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 06:44:58.000000 ipynbname-2023.2.0.0/ipynbname.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-25 06:44:58.244925 ipynbname-2023.2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-07-25 06:37:20.000000 ipynbname-2023.2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:44:55.241832 ipynbname-2024.1.0.0/
+-rw-rw-rw-   0        0        0     1092 2023-04-09 11:23:56.000000 ipynbname-2024.1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       19 2023-04-09 11:23:56.000000 ipynbname-2024.1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1921 2024-05-07 07:44:55.241832 ipynbname-2024.1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2023-07-25 06:32:44.000000 ipynbname-2024.1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 07:44:55.210975 ipynbname-2024.1.0.0/ipynbname/
+-rw-rw-rw-   0        0        0     3737 2024-05-07 07:41:24.000000 ipynbname-2024.1.0.0/ipynbname/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:44:55.240619 ipynbname-2024.1.0.0/ipynbname.egg-info/
+-rw-rw-rw-   0        0        0     1921 2024-05-07 07:44:55.000000 ipynbname-2024.1.0.0/ipynbname.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-05-07 07:44:55.000000 ipynbname-2024.1.0.0/ipynbname.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 07:44:55.000000 ipynbname-2024.1.0.0/ipynbname.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-07 07:44:55.000000 ipynbname-2024.1.0.0/ipynbname.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-07 07:44:55.000000 ipynbname-2024.1.0.0/ipynbname.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-07 07:44:55.246386 ipynbname-2024.1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      988 2024-05-07 07:42:22.000000 ipynbname-2024.1.0.0/setup.py
```

### Comparing `ipynbname-2023.2.0.0/LICENSE` & `ipynbname-2024.1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipynbname-2023.2.0.0/PKG-INFO` & `ipynbname-2024.1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ipynbname
-Version: 2023.2.0.0
+Version: 2024.1.0.0
 Summary: Simply returns either notebook filename or the full path to the notebook when run from Jupyter notebook in browser.
 Home-page: https://github.com/msm1089/ipynbname
 Author: Mark McPherson
 Author-email: msm1089@yahoo.co.uk
 License: MIT
 Keywords: jupyter,notebook,filename
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.4
+Requires-Python: >=3.4, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ipykernel
 
 # ipynbname
 
 When run in a Jupyter notebook, simply returns the notebook filename or the full path to the notebook.
 I created this to help with automating posting blog posts written in Jupyter notebooks directly to
 GitHub Pages.
```

### Comparing `ipynbname-2023.2.0.0/README.md` & `ipynbname-2024.1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ipynbname-2023.2.0.0/ipynbname/__init__.py` & `ipynbname-2024.1.0.0/ipynbname/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     except (MultipleInstanceError, RuntimeError):
         return None, None  # Could not determine
     for srv in _list_maybe_running_servers():
         try:
             sessions = _get_sessions(srv)
             for sess in sessions:
                 if sess['kernel']['id'] == kernel_id:
-                    return srv, PurePath(sess['notebook']['path'])
+                    return srv, PurePath(sess['path'])
         except Exception:
             pass  # There may be stale entries in the runtime directory
     return None, None
 
 
 def name() -> str:
     """ Returns the short name of the notebook w/o the .ipynb extension,
```

### Comparing `ipynbname-2023.2.0.0/ipynbname.egg-info/PKG-INFO` & `ipynbname-2024.1.0.0/ipynbname.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ipynbname
-Version: 2023.2.0.0
+Version: 2024.1.0.0
 Summary: Simply returns either notebook filename or the full path to the notebook when run from Jupyter notebook in browser.
 Home-page: https://github.com/msm1089/ipynbname
 Author: Mark McPherson
 Author-email: msm1089@yahoo.co.uk
 License: MIT
 Keywords: jupyter,notebook,filename
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.4
+Requires-Python: >=3.4, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ipykernel
 
 # ipynbname
 
 When run in a Jupyter notebook, simply returns the notebook filename or the full path to the notebook.
 I created this to help with automating posting blog posts written in Jupyter notebooks directly to
 GitHub Pages.
```

### Comparing `ipynbname-2023.2.0.0/setup.py` & `ipynbname-2024.1.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 from pathlib import Path
 
 here = Path(__file__).parent
 long_description = (here / 'README.md').read_text()
 
 setuptools.setup(
     name='ipynbname',
-    version='2023.2.0.0',
+    version='2024.1.0.0',
     author='Mark McPherson',
     author_email='msm1089@yahoo.co.uk',
     description='Simply returns either notebook filename or the full path to the notebook when run from Jupyter notebook in browser.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     keywords='jupyter notebook filename'.split(),
     url='https://github.com/msm1089/ipynbname',
     packages=setuptools.find_packages(),
     package_data={},
     install_requires=['ipykernel'],
-    python_requires='>=3.4',
+    python_requires='>=3.4, <4',
     classifiers=[
         'Operating System :: OS Independent',
         'Development Status :: 4 - Beta',
         'Framework :: Jupyter',
         'Topic :: Utilities',
         'License :: OSI Approved :: MIT License'
     ]
```

