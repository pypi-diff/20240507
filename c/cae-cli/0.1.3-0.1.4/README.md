# Comparing `tmp/cae_cli-0.1.3.tar.gz` & `tmp/cae_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.1.3.tar", last modified: Tue May  7 02:16:44 2024, max compression
+gzip compressed data, was "cae_cli-0.1.4.tar", last modified: Tue May  7 14:37:12 2024, max compression
```

## Comparing `cae_cli-0.1.3.tar` & `cae_cli-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 02:16:44.784125 cae_cli-0.1.3/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      415 2024-05-07 02:16:44.783124 cae_cli-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 02:16:44.753480 cae_cli-0.1.3/cae/
--rw-rw-rw-   0        0        0     7618 2024-05-05 04:35:29.000000 cae_cli-0.1.3/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.1.3/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.1.3/cae/__init__.py
--rw-rw-rw-   0        0        0     8072 2024-05-07 02:16:32.000000 cae_cli-0.1.3/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-07 02:16:44.768961 cae_cli-0.1.3/cae/templates/
--rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.1.3/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.1.3/cae/templates/dependency_wrapper.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.1.3/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.1.3/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1717 2024-05-07 01:56:38.000000 cae_cli-0.1.3/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1789 2024-05-07 01:56:38.000000 cae_cli-0.1.3/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1944 2024-05-07 01:56:38.000000 cae_cli-0.1.3/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.1.3/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.1.3/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.1.3/cae/templates/use_case_factory.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.1.3/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.1.3/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      397 2024-05-04 04:16:15.000000 cae_cli-0.1.3/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.1.3/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 02:16:44.782123 cae_cli-0.1.3/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      415 2024-05-07 02:16:44.000000 cae_cli-0.1.3/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      705 2024-05-07 02:16:44.000000 cae_cli-0.1.3/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 02:16:44.000000 cae_cli-0.1.3/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-07 02:16:44.000000 cae_cli-0.1.3/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-07 02:16:44.000000 cae_cli-0.1.3/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 02:16:44.784125 cae_cli-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      610 2024-05-07 02:16:32.000000 cae_cli-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:37:12.418935 cae_cli-0.1.4/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      415 2024-05-07 14:37:12.417936 cae_cli-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 14:37:12.305205 cae_cli-0.1.4/cae/
+-rw-rw-rw-   0        0        0     7618 2024-05-05 04:35:29.000000 cae_cli-0.1.4/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.1.4/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.1.4/cae/__init__.py
+-rw-rw-rw-   0        0        0     8078 2024-05-07 02:25:43.000000 cae_cli-0.1.4/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-07 14:37:12.393538 cae_cli-0.1.4/cae/templates/
+-rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.1.4/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.1.4/cae/templates/dependency_wrapper.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.1.4/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.1.4/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1717 2024-05-07 01:56:38.000000 cae_cli-0.1.4/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1789 2024-05-07 01:56:38.000000 cae_cli-0.1.4/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1944 2024-05-07 01:56:38.000000 cae_cli-0.1.4/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.1.4/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.1.4/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.1.4/cae/templates/use_case_factory.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.1.4/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.1.4/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      397 2024-05-04 04:16:15.000000 cae_cli-0.1.4/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.1.4/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 14:37:12.416620 cae_cli-0.1.4/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-05-07 14:37:11.000000 cae_cli-0.1.4/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2024-05-07 14:37:12.000000 cae_cli-0.1.4/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:37:11.000000 cae_cli-0.1.4/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-07 14:37:11.000000 cae_cli-0.1.4/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-07 14:37:11.000000 cae_cli-0.1.4/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 14:37:12.418935 cae_cli-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      610 2024-05-07 14:37:09.000000 cae_cli-0.1.4/setup.py
```

### Comparing `cae_cli-0.1.3/LICENSE` & `cae_cli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.3/README.md` & `cae_cli-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.3/cae/ArchFlowJavaWeb.py` & `cae_cli-0.1.4/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.3/cae/db.json` & `cae_cli-0.1.4/cae/db.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940476190476191%*

 * *Differences: {"'functions'": "{'install': {'steps': [OrderedDict([('install_layer', ['core'])]), "*

 * *                "OrderedDict([('install_layer', ['adapters'])]), OrderedDict([('install_layer', "*

 * *                "['assemblers'])])]}}"}*

```diff
@@ -174,25 +174,25 @@
                     ]
                 }
             ]
         },
         "install": {
             "steps": [
                 {
-                    "clear_layer": [
+                    "install_layer": [
                         "core"
                     ]
                 },
                 {
-                    "clear_layer": [
+                    "install_layer": [
                         "adapters"
                     ]
                 },
                 {
-                    "clear_layer": [
+                    "install_layer": [
                         "assemblers"
                     ]
                 }
             ]
         },
         "install_all": {
             "steps": [
```

### Comparing `cae_cli-0.1.3/cae/templates/assembler.txt` & `cae_cli-0.1.4/cae/templates/assembler.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.3/cae/templates/implementation_cuc.txt` & `cae_cli-0.1.4/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.3/cae/templates/implementation_suc.txt` & `cae_cli-0.1.4/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.3/cae/templates/pom-adapters.txt` & `cae_cli-0.1.4/cae/templates/pom-adapters.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.3/cae/templates/pom-assemblers.txt` & `cae_cli-0.1.4/cae/templates/pom-assemblers.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.3/cae/templates/pom-core.txt` & `cae_cli-0.1.4/cae/templates/pom-core.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.3/cae/templates/use_case.txt` & `cae_cli-0.1.4/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.3/cae/templates/use_case_factory.txt` & `cae_cli-0.1.4/cae/templates/use_case_factory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.3/cae/templates/use_case_implementation.txt` & `cae_cli-0.1.4/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.3/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.1.4/cae_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.3/setup.py` & `cae_cli-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.1.3',
+    version='0.1.4',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
     packages=['cae'],
     package_data={
           'cae': ['templates/*.txt', '*.json']
     },
     install_requires=[
-        'arch-flow>=0.1.5',
+        'arch-flow>=0.1.6',
         'colorama'
       ],
 )
```

