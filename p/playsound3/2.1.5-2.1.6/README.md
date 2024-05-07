# Comparing `tmp/playsound3-2.1.5.tar.gz` & `tmp/playsound3-2.1.6.tar.gz`

## Comparing `playsound3-2.1.5.tar` & `playsound3-2.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 playsound3-2.1.5/.github/workflows/check-code-quality.yaml
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 playsound3-2.1.5/.github/workflows/check-with-pytest-linux.yaml
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 playsound3-2.1.5/.github/workflows/check-with-pytest-macos.yaml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 playsound3-2.1.5/.github/workflows/check-with-pytest-windows.yaml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 playsound3-2.1.5/.idea/.gitignore
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 playsound3-2.1.5/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 playsound3-2.1.5/.idea/modules.xml
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 playsound3-2.1.5/.idea/playsound3.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 playsound3-2.1.5/.idea/vcs.xml
--rw-r--r--   0        0        0    23891 2020-02-02 00:00:00.000000 playsound3-2.1.5/.idea/workspace.xml
--rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 playsound3-2.1.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 playsound3-2.1.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 playsound3-2.1.5/playsound3/__init__.py
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 playsound3-2.1.5/playsound3/playsound3.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 playsound3-2.1.5/tests/test_playsound.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 playsound3-2.1.5/.gitignore
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 playsound3-2.1.5/LICENSE
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 playsound3-2.1.5/README.md
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 playsound3-2.1.5/pyproject.toml
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 playsound3-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 playsound3-2.1.6/.github/workflows/check-code-quality.yaml
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 playsound3-2.1.6/.github/workflows/check-with-pytest-linux.yaml
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 playsound3-2.1.6/.github/workflows/check-with-pytest-macos.yaml
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 playsound3-2.1.6/.github/workflows/check-with-pytest-windows.yaml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/.gitignore
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/modules.xml
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/playsound3.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/vcs.xml
+-rw-r--r--   0        0        0    23894 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/workspace.xml
+-rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 playsound3-2.1.6/playsound3/__init__.py
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 playsound3-2.1.6/playsound3/playsound3.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 playsound3-2.1.6/tests/test_playsound.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 playsound3-2.1.6/.gitignore
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 playsound3-2.1.6/LICENSE
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 playsound3-2.1.6/README.md
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 playsound3-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 playsound3-2.1.6/PKG-INFO
```

### Comparing `playsound3-2.1.5/.github/workflows/check-code-quality.yaml` & `playsound3-2.1.6/.github/workflows/check-code-quality.yaml`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.5/.github/workflows/check-with-pytest-linux.yaml` & `playsound3-2.1.6/.github/workflows/check-with-pytest-linux.yaml`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.5/.github/workflows/check-with-pytest-macos.yaml` & `playsound3-2.1.6/.github/workflows/check-with-pytest-macos.yaml`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.5/.github/workflows/check-with-pytest-windows.yaml` & `playsound3-2.1.6/.github/workflows/check-with-pytest-windows.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 name: Install locally and run pytest on Windows
 
-# This test fails on Windows device without audio devices
-# We don't run it automatically
+# This test fails on windows server without audio devices
+# So we don't run it automatically
 
 on:
   workflow_dispatch:
 
 #on:
 #  push:
 #    branches: [ "main" ]
```

### Comparing `playsound3-2.1.5/.idea/workspace.xml` & `playsound3-2.1.6/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `playsound3-2.1.5/.idea/workspace.xml` & `playsound3-2.1.6/.idea/workspace.xml`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="4fbee7df-bfbf-4326-aa56-dc3a718f551b" name="Changes" comment="Remove unnecessary note">
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+    <list default="true" id="4fbee7df-bfbf-4326-aa56-dc3a718f551b" name="Changes" comment="Update comments in a test">
+      <change beforePath="$PROJECT_DIR$/playsound3/playsound3.py" beforeDir="false" afterPath="$PROJECT_DIR$/playsound3/playsound3.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
@@ -90,31 +90,15 @@
       <workItem from="1715028902191" duration="292000"/>
       <workItem from="1715029948125" duration="587000"/>
       <workItem from="1715030546044" duration="41000"/>
       <workItem from="1715030697321" duration="9000"/>
       <workItem from="1715035744281" duration="106000"/>
       <workItem from="1715035857578" duration="3880000"/>
       <workItem from="1715073679361" duration="15313000"/>
-      <workItem from="1715089410611" duration="825000"/>
-    </task>
-    <task id="LOCAL-00036" summary="Install gstreamer for test">
-      <option name="closed" value="true"/>
-      <created>1715081492014</created>
-      <option name="number" value="00036"/>
-      <option name="presentableId" value="LOCAL-00036"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715081492014</updated>
-    </task>
-    <task id="LOCAL-00037" summary="Install gstreamer for test">
-      <option name="closed" value="true"/>
-      <created>1715081543799</created>
-      <option name="number" value="00037"/>
-      <option name="presentableId" value="LOCAL-00037"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715081543799</updated>
+      <workItem from="1715089410611" duration="1567000"/>
     </task>
     <task id="LOCAL-00038" summary="Install gstreamer for test">
       <option name="closed" value="true"/>
       <created>1715081784901</created>
       <option name="number" value="00038"/>
       <option name="presentableId" value="LOCAL-00038"/>
       <option name="project" value="LOCAL"/>
@@ -484,15 +468,31 @@
       <option name="closed" value="true"/>
       <created>1715090230713</created>
       <option name="number" value="00084"/>
       <option name="presentableId" value="LOCAL-00084"/>
       <option name="project" value="LOCAL"/>
       <updated>1715090230713</updated>
     </task>
-    <option name="localTasksCounter" value="85"/>
+    <task id="LOCAL-00085" summary="Bump version for release">
+      <option name="closed" value="true"/>
+      <created>1715090244286</created>
+      <option name="number" value="00085"/>
+      <option name="presentableId" value="LOCAL-00085"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715090244286</updated>
+    </task>
+    <task id="LOCAL-00086" summary="Update comments in a test">
+      <option name="closed" value="true"/>
+      <created>1715090571937</created>
+      <option name="number" value="00086"/>
+      <option name="presentableId" value="LOCAL-00086"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715090571937</updated>
+    </task>
+    <option name="localTasksCounter" value="87"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -502,15 +502,14 @@
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="Change to packaging system to pyproject.toml"/>
     <MESSAGE value="Updating legacy download function"/>
     <MESSAGE value="Fix missing certificates for download"/>
     <MESSAGE value="Install and use certifi by default"/>
     <MESSAGE value="Add tests and github workflows"/>
     <MESSAGE value="Isort and Black formatting"/>
     <MESSAGE value="Install gstreamer for test"/>
     <MESSAGE value="Add separate tests for Windows and Mac OS"/>
@@ -525,12 +524,13 @@
     <MESSAGE value="Skip windows test"/>
     <MESSAGE value="Update README"/>
     <MESSAGE value="Use URLs in blocking test"/>
     <MESSAGE value="Remove audio samples"/>
     <MESSAGE value="Modify Linux backend"/>
     <MESSAGE value="Remove unsued dependency"/>
     <MESSAGE value="Change backend naming"/>
-    <MESSAGE value="Bump version for release"/>
     <MESSAGE value="Remove unnecessary note"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Remove unnecessary note"/>
+    <MESSAGE value="Bump version for release"/>
+    <MESSAGE value="Update comments in a test"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Update comments in a test"/>
   </component>
 </project>
```

### Comparing `playsound3-2.1.5/.idea/inspectionProfiles/Project_Default.xml` & `playsound3-2.1.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.5/playsound3/playsound3.py` & `playsound3-2.1.6/playsound3/playsound3.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import atexit
 import ctypes
 import logging
+import os
 import platform
 import ssl
 import subprocess
 import tempfile
 import urllib.error
 import urllib.request
 import uuid
 from pathlib import Path
 from threading import Thread
 
 import certifi
 
+logging.basicConfig(level=os.environ.get("LOGLEVEL", "WARNING"))
 logger = logging.getLogger(__name__)
 
 SYSTEM = platform.system()
 DOWNLOAD_CACHE = dict()
 
 
 class PlaysoundException(Exception):
```

### Comparing `playsound3-2.1.5/tests/test_playsound.py` & `playsound3-2.1.6/tests/test_playsound.py`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.5/.gitignore` & `playsound3-2.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.5/LICENSE` & `playsound3-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.5/README.md` & `playsound3-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.5/pyproject.toml` & `playsound3-2.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "playsound3"
-version = "2.1.5"
+version = "2.1.6"
 requires-python = ">=3.7"
 authors = [
     { name = "Szymon Mikler", email = "sjmikler@gmail.com" },
     { name = "Taylor Marks", email = "taylor@marksfam.com" },
 ]
 maintainers = [
     { name = "Szymon Mikler", email = "sjmikler@gmail.com" },
```

### Comparing `playsound3-2.1.5/PKG-INFO` & `playsound3-2.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: playsound3
-Version: 2.1.5
+Version: 2.1.6
 Summary: Cross-platform library to play audio files
 Project-URL: Repository, https://github.com/sjmikler/playsound3
 Project-URL: Issues, https://github.com/sjmikler/playsound3/issues
 Project-URL: Documentation, https://github.com/sjmikler/playsound3?tab=readme-ov-file#documentation
 Author-email: Szymon Mikler <sjmikler@gmail.com>, Taylor Marks <taylor@marksfam.com>
 Maintainer-email: Szymon Mikler <sjmikler@gmail.com>
 License: MIT License
```

