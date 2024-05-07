# Comparing `tmp/cae_cli-0.1.5.tar.gz` & `tmp/cae_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.1.5.tar", last modified: Tue May  7 20:59:15 2024, max compression
+gzip compressed data, was "cae_cli-0.1.6.tar", last modified: Tue May  7 21:04:24 2024, max compression
```

## Comparing `cae_cli-0.1.5.tar` & `cae_cli-0.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 20:59:15.956954 cae_cli-0.1.5/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      415 2024-05-07 20:59:15.955953 cae_cli-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 20:59:15.916621 cae_cli-0.1.5/cae/
--rw-rw-rw-   0        0        0     7644 2024-05-07 20:56:41.000000 cae_cli-0.1.5/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.1.5/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.1.5/cae/__init__.py
--rw-rw-rw-   0        0        0     8078 2024-05-07 02:25:43.000000 cae_cli-0.1.5/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-07 20:59:15.934929 cae_cli-0.1.5/cae/templates/
--rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.1.5/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.1.5/cae/templates/dependency_wrapper.txt
--rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.1.5/cae/templates/entity.txt
--rw-rw-rw-   0        0        0      581 2024-05-07 20:50:41.000000 cae_cli-0.1.5/cae/templates/entityFactory.txt
--rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.1.5/cae/templates/entityImplementation.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.1.5/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.1.5/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1717 2024-05-07 01:56:38.000000 cae_cli-0.1.5/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1789 2024-05-07 01:56:38.000000 cae_cli-0.1.5/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1944 2024-05-07 01:56:38.000000 cae_cli-0.1.5/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.1.5/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.1.5/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.1.5/cae/templates/use_case_factory.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.1.5/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.1.5/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      397 2024-05-04 04:16:15.000000 cae_cli-0.1.5/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.1.5/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 20:59:15.954955 cae_cli-0.1.5/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      415 2024-05-07 20:59:15.000000 cae_cli-0.1.5/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      801 2024-05-07 20:59:15.000000 cae_cli-0.1.5/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 20:59:15.000000 cae_cli-0.1.5/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-07 20:59:15.000000 cae_cli-0.1.5/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-07 20:59:15.000000 cae_cli-0.1.5/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 20:59:15.956954 cae_cli-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      610 2024-05-07 20:56:41.000000 cae_cli-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:04:24.811388 cae_cli-0.1.6/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      415 2024-05-07 21:04:24.809879 cae_cli-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 21:04:24.777447 cae_cli-0.1.6/cae/
+-rw-rw-rw-   0        0        0     7644 2024-05-07 20:56:41.000000 cae_cli-0.1.6/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.1.6/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.1.6/cae/__init__.py
+-rw-rw-rw-   0        0        0     8078 2024-05-07 02:25:43.000000 cae_cli-0.1.6/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-07 21:04:24.795674 cae_cli-0.1.6/cae/templates/
+-rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.1.6/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.1.6/cae/templates/dependency_wrapper.txt
+-rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.1.6/cae/templates/entity.txt
+-rw-rw-rw-   0        0        0      584 2024-05-07 21:04:05.000000 cae_cli-0.1.6/cae/templates/entityFactory.txt
+-rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.1.6/cae/templates/entityImplementation.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.1.6/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.1.6/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1717 2024-05-07 01:56:38.000000 cae_cli-0.1.6/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1789 2024-05-07 01:56:38.000000 cae_cli-0.1.6/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1944 2024-05-07 01:56:38.000000 cae_cli-0.1.6/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.1.6/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.1.6/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.1.6/cae/templates/use_case_factory.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.1.6/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.1.6/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      397 2024-05-04 04:16:15.000000 cae_cli-0.1.6/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.1.6/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 21:04:24.808878 cae_cli-0.1.6/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-05-07 21:04:24.000000 cae_cli-0.1.6/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      801 2024-05-07 21:04:24.000000 cae_cli-0.1.6/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 21:04:24.000000 cae_cli-0.1.6/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-07 21:04:24.000000 cae_cli-0.1.6/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-07 21:04:24.000000 cae_cli-0.1.6/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 21:04:24.811388 cae_cli-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      610 2024-05-07 21:04:23.000000 cae_cli-0.1.6/setup.py
```

### Comparing `cae_cli-0.1.5/LICENSE` & `cae_cli-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/README.md` & `cae_cli-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/cae/ArchFlowJavaWeb.py` & `cae_cli-0.1.6/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/cae/db.json` & `cae_cli-0.1.6/cae/db.json`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/cae/templates/assembler.txt` & `cae_cli-0.1.6/cae/templates/assembler.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/cae/templates/entityFactory.txt` & `cae_cli-0.1.6/cae/templates/entityFactory.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-package <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.entities.factory;
+package <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.entities.factories;
 
-import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>entities.<pc>args[0]</pc>;
+import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.entities.<pc>args[0]</pc>;
 import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.entities.implementations.<pc>args[0]</pc>Implementation;
 import lombok.AccessLevel;
 import lombok.NoArgsConstructor;
 
 @NoArgsConstructor(access = AccessLevel.PRIVATE)
 public class <pc>args[0]</pc>Factory {
```

### Comparing `cae_cli-0.1.5/cae/templates/implementation_cuc.txt` & `cae_cli-0.1.6/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/cae/templates/implementation_suc.txt` & `cae_cli-0.1.6/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/cae/templates/pom-adapters.txt` & `cae_cli-0.1.6/cae/templates/pom-adapters.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/cae/templates/pom-assemblers.txt` & `cae_cli-0.1.6/cae/templates/pom-assemblers.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/cae/templates/pom-core.txt` & `cae_cli-0.1.6/cae/templates/pom-core.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/cae/templates/use_case.txt` & `cae_cli-0.1.6/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/cae/templates/use_case_factory.txt` & `cae_cli-0.1.6/cae/templates/use_case_factory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/cae/templates/use_case_implementation.txt` & `cae_cli-0.1.6/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.1.6/cae_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.5/setup.py` & `cae_cli-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.1.5',
+    version='0.1.6',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
```

