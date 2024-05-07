# Comparing `tmp/eth_gtd_cli-0.0.2.tar.gz` & `tmp/eth_gtd_cli-0.0.3.tar.gz`

## Comparing `eth_gtd_cli-0.0.2.tar` & `eth_gtd_cli-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/CLI.iml
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/LICENSE
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/.idea/CLI.iml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/LICENSE
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.3/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.2/.idea/workspace.xml` & `eth_gtd_cli-0.0.3/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `eth_gtd_cli-0.0.2/.idea/workspace.xml` & `eth_gtd_cli-0.0.3/.idea/workspace.xml`

```diff
@@ -125,15 +125,15 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="d43fb52d-49ac-4abd-b19d-bb5a37435ca0" name="Changes" comment=""/>
       <created>1714725291835</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1714725291835</updated>
       <workItem from="1714725292898" duration="18885000"/>
-      <workItem from="1715072837883" duration="5101000"/>
+      <workItem from="1715072837883" duration="5559000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
```

### Comparing `eth_gtd_cli-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `eth_gtd_cli-0.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.2/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.3/src/ETH_GTD_cli/helper.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.2/src/ETH_GTD_cli/main.py` & `eth_gtd_cli-0.0.3/src/ETH_GTD_cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         data = response.json()
         if not full:
             for topic in data["topics"]:
                 print(f" - {topic['name']}")
         else:
             table = Table("UUID", "name", "type", "nrMessages", "frequency")
             for topic in data["topics"]:
-                table.add_row(topic["uuid"], topic["name"], topic["type"], topic["nrMessages"], f"{topic["frequency"]}")
+                table.add_row(topic["uuid"], topic["name"], topic["type"], topic["nrMessages"], f"{topic['frequency']}")
             print(table)
 
     except httpx.HTTPError as e:
         print(f"Failed")
 
 @projects.command("create")
 def create_project(name: Annotated[str, typer.Option()]):
```

### Comparing `eth_gtd_cli-0.0.2/LICENSE` & `eth_gtd_cli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.2/pyproject.toml` & `eth_gtd_cli-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
 description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `eth_gtd_cli-0.0.2/PKG-INFO` & `eth_gtd_cli-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ETH_GTD_cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: A CLI for the ETH project Grand Tour
 Project-URL: Homepage, https://github.com/leggedrobotics/GrandTourDatasets
 Project-URL: Issues, https://github.com/leggedrobotics/GrandTourDatasets/issues
 Author-email: Johann Schwabe <jschwab@ethz.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

