# Comparing `tmp/eth_gtd_cli-0.0.1.tar.gz` & `tmp/eth_gtd_cli-0.0.2.tar.gz`

## Comparing `eth_gtd_cli-0.0.1.tar` & `eth_gtd_cli-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/.idea/CLI.iml
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/LICENSE
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/README.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/CLI.iml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/LICENSE
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.1/.idea/workspace.xml` & `eth_gtd_cli-0.0.2/.idea/workspace.xml`

 * *Files 1% similar despite different names*

#### Comparing `eth_gtd_cli-0.0.1/.idea/workspace.xml` & `eth_gtd_cli-0.0.2/.idea/workspace.xml`

```diff
@@ -125,15 +125,15 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="d43fb52d-49ac-4abd-b19d-bb5a37435ca0" name="Changes" comment=""/>
       <created>1714725291835</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1714725291835</updated>
       <workItem from="1714725292898" duration="18885000"/>
-      <workItem from="1715072837883" duration="3206000"/>
+      <workItem from="1715072837883" duration="5101000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
```

### Comparing `eth_gtd_cli-0.0.1/.idea/inspectionProfiles/Project_Default.xml` & `eth_gtd_cli-0.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.1/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.2/src/ETH_GTD_cli/helper.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.1/src/ETH_GTD_cli/main.py` & `eth_gtd_cli-0.0.2/src/ETH_GTD_cli/main.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.1/LICENSE` & `eth_gtd_cli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.1/pyproject.toml` & `eth_gtd_cli-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 [build-system]
-requires = ["hatchling", "typer", "httpx"]
+requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
-description = "A CLI for the ETH project"
+description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
 requires-python = ">=3.10"
+dependencies = [
+  "typer",
+  "httpx"
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/leggedrobotics/GrandTourDatasets"
-Issues = "https://github.com/leggedrobotics/GrandTourDatasets/issues"
+Issues = "https://github.com/leggedrobotics/GrandTourDatasets/issues"
+
+[project.scripts]
+GTD = 'ETH_GTD_cli.main:app'
```

### Comparing `eth_gtd_cli-0.0.1/PKG-INFO` & `eth_gtd_cli-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.3
 Name: ETH_GTD_cli
-Version: 0.0.1
-Summary: A CLI for the ETH project
+Version: 0.0.2
+Summary: A CLI for the ETH project Grand Tour
 Project-URL: Homepage, https://github.com/leggedrobotics/GrandTourDatasets
 Project-URL: Issues, https://github.com/leggedrobotics/GrandTourDatasets/issues
 Author-email: Johann Schwabe <jschwab@ethz.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: httpx
+Requires-Dist: typer
 Description-Content-Type: text/markdown
 
 # Grand Tour Datasets: CLI
 
 Used as an alternative to the webtool at https://datasets.leggedrobotics.com/ \
 Use --help to get an overview over available commands.
```

