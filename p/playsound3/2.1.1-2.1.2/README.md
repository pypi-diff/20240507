# Comparing `tmp/playsound3-2.1.1.tar.gz` & `tmp/playsound3-2.1.2.tar.gz`

## Comparing `playsound3-2.1.1.tar` & `playsound3-2.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 playsound3-2.1.1/script_release.sh
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/.gitignore
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/playsound3.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0    15985 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/workspace.xml
--rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 playsound3-2.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 playsound3-2.1.1/playsound3/__init__.py
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 playsound3-2.1.1/playsound3/playsound3.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 playsound3-2.1.1/.gitignore
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 playsound3-2.1.1/LICENSE
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 playsound3-2.1.1/README.md
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 playsound3-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 playsound3-2.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 playsound3-2.1.2/script_release.sh
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/.gitignore
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/playsound3.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    16353 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/workspace.xml
+-rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 playsound3-2.1.2/playsound3/__init__.py
+-rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 playsound3-2.1.2/playsound3/playsound3.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 playsound3-2.1.2/.gitignore
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 playsound3-2.1.2/LICENSE
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 playsound3-2.1.2/README.md
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 playsound3-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 playsound3-2.1.2/PKG-INFO
```

### Comparing `playsound3-2.1.1/.idea/workspace.xml` & `playsound3-2.1.2/.idea/workspace.xml`

 * *Files 9% similar despite different names*

#### Comparing `playsound3-2.1.1/.idea/workspace.xml` & `playsound3-2.1.2/.idea/workspace.xml`

```diff
@@ -1,16 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="4fbee7df-bfbf-4326-aa56-dc3a718f551b" name="Changes" comment="Change to packaging system to pyproject.toml">
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-    </list>
+    <list default="true" id="4fbee7df-bfbf-4326-aa56-dc3a718f551b" name="Changes" comment="Fix missing certificates for download"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
@@ -20,28 +18,28 @@
 }</component>
   <component name="ProjectId" id="2g5sXLf8F18eSiUiNloeaQqPaCM"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
     <option name="sortKey" value="BY_TIME_DESCENDING"/>
   </component>
-  <component name="PropertiesComponent">{
-  &quot;keyToString&quot;: {
-    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
-    &quot;git-widget-placeholder&quot;: &quot;main&quot;,
-    &quot;last_opened_file_path&quot;: &quot;/home/gaha/workspace/python/playsound3&quot;,
-    &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
-    &quot;node.js.detected.package.tslint&quot;: &quot;true&quot;,
-    &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
-    &quot;node.js.selected.package.tslint&quot;: &quot;(autodetect)&quot;,
-    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
-    &quot;settings.editor.selected.configurable&quot;: &quot;PyConsoleConfigurable.Python Console&quot;,
-    &quot;vue.rearranger.settings.migration&quot;: &quot;true&quot;
+  <component name="PropertiesComponent"><![CDATA[{
+  "keyToString": {
+    "RunOnceActivity.ShowReadmeOnStart": "true",
+    "git-widget-placeholder": "main",
+    "last_opened_file_path": "/home/gaha/workspace/python/playsound3",
+    "node.js.detected.package.eslint": "true",
+    "node.js.detected.package.tslint": "true",
+    "node.js.selected.package.eslint": "(autodetect)",
+    "node.js.selected.package.tslint": "(autodetect)",
+    "nodejs_package_manager_path": "npm",
+    "settings.editor.selected.configurable": "preferences.sourceCode",
+    "vue.rearranger.settings.migration": "true"
   }
-}</component>
+}]]></component>
   <component name="PyConsoleOptionsProvider">
     <option name="myPythonConsoleState">
       <console-settings custom-start-script="%load_ext autoreload
 %autoreload 2
 
 import sys; print('Python %s on %s' % (sys.version, sys.platform))
 sys.path.extend([WORKING_DIR_AND_PYTHON_PATHS])
@@ -88,15 +86,15 @@
       <workItem from="1715014531807" duration="3424000"/>
       <workItem from="1715028902191" duration="292000"/>
       <workItem from="1715029948125" duration="587000"/>
       <workItem from="1715030546044" duration="41000"/>
       <workItem from="1715030697321" duration="9000"/>
       <workItem from="1715035744281" duration="106000"/>
       <workItem from="1715035857578" duration="3880000"/>
-      <workItem from="1715073679361" duration="1499000"/>
+      <workItem from="1715073679361" duration="4093000"/>
     </task>
     <task id="LOCAL-00001" summary="Clearing up the structure">
       <option name="closed" value="true"/>
       <created>1714999313464</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
@@ -314,15 +312,31 @@
       <option name="closed" value="true"/>
       <created>1715075015844</created>
       <option name="number" value="00028"/>
       <option name="presentableId" value="LOCAL-00028"/>
       <option name="project" value="LOCAL"/>
       <updated>1715075015844</updated>
     </task>
-    <option name="localTasksCounter" value="29"/>
+    <task id="LOCAL-00029" summary="Updating legacy download function">
+      <option name="closed" value="true"/>
+      <created>1715076338617</created>
+      <option name="number" value="00029"/>
+      <option name="presentableId" value="LOCAL-00029"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715076338617</updated>
+    </task>
+    <task id="LOCAL-00030" summary="Fix missing certificates for download">
+      <option name="closed" value="true"/>
+      <created>1715077928155</created>
+      <option name="number" value="00030"/>
+      <option name="presentableId" value="LOCAL-00030"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715077928155</updated>
+    </task>
+    <option name="localTasksCounter" value="31"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -332,16 +346,14 @@
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="Separate source code"/>
-    <MESSAGE value="Refactoring the main file"/>
     <MESSAGE value="Update requirements"/>
     <MESSAGE value="Add back Windows support"/>
     <MESSAGE value="Typo"/>
     <MESSAGE value="Remove licensing information from README"/>
     <MESSAGE value="Fix import"/>
     <MESSAGE value="Fix OSX version"/>
     <MESSAGE value="Remove additional files"/>
@@ -357,10 +369,12 @@
     <MESSAGE value="Clear up the license"/>
     <MESSAGE value="Add short description"/>
     <MESSAGE value="Change case"/>
     <MESSAGE value="Add support for URL files"/>
     <MESSAGE value="isort and black formatting"/>
     <MESSAGE value="Restore python 3.7 compatibility"/>
     <MESSAGE value="Change to packaging system to pyproject.toml"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Change to packaging system to pyproject.toml"/>
+    <MESSAGE value="Updating legacy download function"/>
+    <MESSAGE value="Fix missing certificates for download"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Fix missing certificates for download"/>
   </component>
 </project>
```

### Comparing `playsound3-2.1.1/.idea/inspectionProfiles/Project_Default.xml` & `playsound3-2.1.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.1/playsound3/playsound3.py` & `playsound3-2.1.2/playsound3/playsound3.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import atexit
 import ctypes
 import logging
 import platform
 import subprocess
 import tempfile
 import urllib.request
+import urllib.error
 import uuid
 from pathlib import Path
 from threading import Thread
 
 logger = logging.getLogger(__name__)
 
 SYSTEM = platform.system()
@@ -39,20 +40,41 @@
 
     if block:
         func(sound)
     else:
         t = Thread(target=func, args=(sound,), daemon=True).start()
 
 
+def _download_sound_from_web(link, destination):
+    # Identifies itself as a browser to avoid HTTP 403 errors
+    headers = {"User-Agent": "Mozilla/5.0 (Windows NT 6.1; Win64; x64)"}
+    request = urllib.request.Request(link, headers=headers)
+
+    try:
+        import ssl
+        import certifi
+
+        context = ssl.create_default_context(cafile=certifi.where())
+    except ImportError:
+        context = None
+
+    try:
+        with urllib.request.urlopen(request, context=context) as response, open(destination, "wb") as out_file:
+            out_file.write(response.read())
+    except urllib.error.HTTPError as e:
+        msg = f"Failed to download sound from {link}: {e}\nTry running 'pip install certifi'"
+        raise PlaysoundException(msg)
+
+
 def _prepare_path(sound):
     if sound.startswith(("http://", "https://")):
-        # To play file from URL, we download the file first to a temporary location
+        # To play file from URL, we download the file first to a temporary location and cache it
         if sound not in DOWNLOAD_CACHE:
             with tempfile.NamedTemporaryFile(delete=False, prefix="playsound3-") as f:
-                urllib.request.urlretrieve(sound, f.name)
+                _download_sound_from_web(sound, f.name)
                 DOWNLOAD_CACHE[sound] = f.name
         sound = DOWNLOAD_CACHE[sound]
 
     path = Path(sound)
 
     if not path.exists():
         raise PlaysoundException(f"File not found: {sound}")
```

### Comparing `playsound3-2.1.1/.gitignore` & `playsound3-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.1/LICENSE` & `playsound3-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.1/README.md` & `playsound3-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.1/pyproject.toml` & `playsound3-2.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "playsound3"
-version = "2.1.1"
+version = "2.1.2"
 requires-python = ">=3.7"
 authors = [
     { name = "Szymon Mikler", email = "sjmikler@gmail.com" },
     { name = "Taylor Marks", email = "taylor@marksfam.com" },
 ]
 maintainers = [
     { name = "Szymon Mikler", email = "sjmikler@gmail.com" },
```

### Comparing `playsound3-2.1.1/PKG-INFO` & `playsound3-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: playsound3
-Version: 2.1.1
+Version: 2.1.2
 Summary: Cross-platform library to play audio files
 Project-URL: Repository, https://github.com/sjmikler/playsound3
 Project-URL: Issues, https://github.com/sjmikler/playsound3/issues
 Project-URL: Documentation, https://github.com/sjmikler/playsound3?tab=readme-ov-file#documentation
 Author-email: Szymon Mikler <sjmikler@gmail.com>, Taylor Marks <taylor@marksfam.com>
 Maintainer-email: Szymon Mikler <sjmikler@gmail.com>
 License: MIT License
```

