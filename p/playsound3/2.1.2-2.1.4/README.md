# Comparing `tmp/playsound3-2.1.2.tar.gz` & `tmp/playsound3-2.1.4.tar.gz`

## Comparing `playsound3-2.1.2.tar` & `playsound3-2.1.4.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 playsound3-2.1.2/script_release.sh
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/.gitignore
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/modules.xml
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/playsound3.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/vcs.xml
--rw-r--r--   0        0        0    16353 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/workspace.xml
--rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 playsound3-2.1.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 playsound3-2.1.2/playsound3/__init__.py
--rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 playsound3-2.1.2/playsound3/playsound3.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 playsound3-2.1.2/.gitignore
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 playsound3-2.1.2/LICENSE
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 playsound3-2.1.2/README.md
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 playsound3-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 playsound3-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 playsound3-2.1.4/.github/workflows/check-code-quality.yaml
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 playsound3-2.1.4/.github/workflows/check-with-pytest-linux.yaml
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 playsound3-2.1.4/.github/workflows/check-with-pytest-macos.yaml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 playsound3-2.1.4/.github/workflows/check-with-pytest-windows.yaml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 playsound3-2.1.4/.idea/.gitignore
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 playsound3-2.1.4/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 playsound3-2.1.4/.idea/modules.xml
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 playsound3-2.1.4/.idea/playsound3.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 playsound3-2.1.4/.idea/vcs.xml
+-rw-r--r--   0        0        0    23758 2020-02-02 00:00:00.000000 playsound3-2.1.4/.idea/workspace.xml
+-rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 playsound3-2.1.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 playsound3-2.1.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 playsound3-2.1.4/playsound3/__init__.py
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 playsound3-2.1.4/playsound3/playsound3.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 playsound3-2.1.4/tests/test_playsound.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 playsound3-2.1.4/.gitignore
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 playsound3-2.1.4/LICENSE
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 playsound3-2.1.4/README.md
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 playsound3-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 playsound3-2.1.4/PKG-INFO
```

### Comparing `playsound3-2.1.2/.idea/workspace.xml` & `playsound3-2.1.4/.idea/workspace.xml`

 * *Files 24% similar despite different names*

#### Comparing `playsound3-2.1.2/.idea/workspace.xml` & `playsound3-2.1.4/.idea/workspace.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="4fbee7df-bfbf-4326-aa56-dc3a718f551b" name="Changes" comment="Fix missing certificates for download"/>
+    <list default="true" id="4fbee7df-bfbf-4326-aa56-dc3a718f551b" name="Changes" comment="Change backend naming"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
@@ -18,28 +18,28 @@
 }</component>
   <component name="ProjectId" id="2g5sXLf8F18eSiUiNloeaQqPaCM"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
     <option name="sortKey" value="BY_TIME_DESCENDING"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "git-widget-placeholder": "main",
-    "last_opened_file_path": "/home/gaha/workspace/python/playsound3",
-    "node.js.detected.package.eslint": "true",
-    "node.js.detected.package.tslint": "true",
-    "node.js.selected.package.eslint": "(autodetect)",
-    "node.js.selected.package.tslint": "(autodetect)",
-    "nodejs_package_manager_path": "npm",
-    "settings.editor.selected.configurable": "preferences.sourceCode",
-    "vue.rearranger.settings.migration": "true"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;git-widget-placeholder&quot;: &quot;main&quot;,
+    &quot;last_opened_file_path&quot;: &quot;/home/gaha/workspace/python/playsound3/.github/workflows&quot;,
+    &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
+    &quot;node.js.detected.package.tslint&quot;: &quot;true&quot;,
+    &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
+    &quot;node.js.selected.package.tslint&quot;: &quot;(autodetect)&quot;,
+    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;preferences.sourceCode&quot;,
+    &quot;vue.rearranger.settings.migration&quot;: &quot;true&quot;
   }
-}]]></component>
+}</component>
   <component name="PyConsoleOptionsProvider">
     <option name="myPythonConsoleState">
       <console-settings custom-start-script="%load_ext autoreload
 %autoreload 2
 
 import sys; print('Python %s on %s' % (sys.version, sys.platform))
 sys.path.extend([WORKING_DIR_AND_PYTHON_PATHS])
@@ -54,14 +54,15 @@
         <option name="myModuleName" value="playsound3"/>
       </console-settings>
     </option>
     <option name="myShowVariablesByDefault" value="false"/>
   </component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
+      <recent name="$PROJECT_DIR$/.github/workflows"/>
       <recent name="$PROJECT_DIR$"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/devel"/>
       <recent name="$PROJECT_DIR$/playsound2"/>
     </key>
   </component>
@@ -86,257 +87,410 @@
       <workItem from="1715014531807" duration="3424000"/>
       <workItem from="1715028902191" duration="292000"/>
       <workItem from="1715029948125" duration="587000"/>
       <workItem from="1715030546044" duration="41000"/>
       <workItem from="1715030697321" duration="9000"/>
       <workItem from="1715035744281" duration="106000"/>
       <workItem from="1715035857578" duration="3880000"/>
-      <workItem from="1715073679361" duration="4093000"/>
+      <workItem from="1715073679361" duration="15313000"/>
+      <workItem from="1715089410611" duration="769000"/>
+    </task>
+    <task id="LOCAL-00034" summary="Install gstreamer for test">
+      <option name="closed" value="true"/>
+      <created>1715080824378</created>
+      <option name="number" value="00034"/>
+      <option name="presentableId" value="LOCAL-00034"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715080824378</updated>
+    </task>
+    <task id="LOCAL-00035" summary="Install gstreamer for test">
+      <option name="closed" value="true"/>
+      <created>1715081249487</created>
+      <option name="number" value="00035"/>
+      <option name="presentableId" value="LOCAL-00035"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715081249487</updated>
+    </task>
+    <task id="LOCAL-00036" summary="Install gstreamer for test">
+      <option name="closed" value="true"/>
+      <created>1715081492014</created>
+      <option name="number" value="00036"/>
+      <option name="presentableId" value="LOCAL-00036"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715081492014</updated>
+    </task>
+    <task id="LOCAL-00037" summary="Install gstreamer for test">
+      <option name="closed" value="true"/>
+      <created>1715081543799</created>
+      <option name="number" value="00037"/>
+      <option name="presentableId" value="LOCAL-00037"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715081543799</updated>
+    </task>
+    <task id="LOCAL-00038" summary="Install gstreamer for test">
+      <option name="closed" value="true"/>
+      <created>1715081784901</created>
+      <option name="number" value="00038"/>
+      <option name="presentableId" value="LOCAL-00038"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715081784901</updated>
+    </task>
+    <task id="LOCAL-00039" summary="Add separate tests for Windows and Mac OS">
+      <option name="closed" value="true"/>
+      <created>1715082103842</created>
+      <option name="number" value="00039"/>
+      <option name="presentableId" value="LOCAL-00039"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715082103842</updated>
+    </task>
+    <task id="LOCAL-00040" summary="Remove 3.7 runner from Mac OS">
+      <option name="closed" value="true"/>
+      <created>1715082277170</created>
+      <option name="number" value="00040"/>
+      <option name="presentableId" value="LOCAL-00040"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715082277170</updated>
+    </task>
+    <task id="LOCAL-00041" summary="Update workflows">
+      <option name="closed" value="true"/>
+      <created>1715083003371</created>
+      <option name="number" value="00041"/>
+      <option name="presentableId" value="LOCAL-00041"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715083003371</updated>
+    </task>
+    <task id="LOCAL-00042" summary="Update workflows">
+      <option name="closed" value="true"/>
+      <created>1715083188627</created>
+      <option name="number" value="00042"/>
+      <option name="presentableId" value="LOCAL-00042"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715083188627</updated>
+    </task>
+    <task id="LOCAL-00043" summary="Update workflows">
+      <option name="closed" value="true"/>
+      <created>1715083251898</created>
+      <option name="number" value="00043"/>
+      <option name="presentableId" value="LOCAL-00043"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715083251898</updated>
+    </task>
+    <task id="LOCAL-00044" summary="Update workflows">
+      <option name="closed" value="true"/>
+      <created>1715083304184</created>
+      <option name="number" value="00044"/>
+      <option name="presentableId" value="LOCAL-00044"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715083304184</updated>
+    </task>
+    <task id="LOCAL-00045" summary="Update workflows">
+      <option name="closed" value="true"/>
+      <created>1715083337529</created>
+      <option name="number" value="00045"/>
+      <option name="presentableId" value="LOCAL-00045"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715083337529</updated>
+    </task>
+    <task id="LOCAL-00046" summary="Update workflows">
+      <option name="closed" value="true"/>
+      <created>1715083408493</created>
+      <option name="number" value="00046"/>
+      <option name="presentableId" value="LOCAL-00046"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715083408493</updated>
+    </task>
+    <task id="LOCAL-00047" summary="Update workflows - force install">
+      <option name="closed" value="true"/>
+      <created>1715083498513</created>
+      <option name="number" value="00047"/>
+      <option name="presentableId" value="LOCAL-00047"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715083498513</updated>
+    </task>
+    <task id="LOCAL-00048" summary="Update workflows - force install">
+      <option name="closed" value="true"/>
+      <created>1715083564971</created>
+      <option name="number" value="00048"/>
+      <option name="presentableId" value="LOCAL-00048"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715083564971</updated>
+    </task>
+    <task id="LOCAL-00049" summary="Revert to setup-gstreamer action">
+      <option name="closed" value="true"/>
+      <created>1715083667376</created>
+      <option name="number" value="00049"/>
+      <option name="presentableId" value="LOCAL-00049"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715083667376</updated>
+    </task>
+    <task id="LOCAL-00050" summary="Revert to setup-gstreamer action">
+      <option name="closed" value="true"/>
+      <created>1715083883233</created>
+      <option name="number" value="00050"/>
+      <option name="presentableId" value="LOCAL-00050"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715083883233</updated>
+    </task>
+    <task id="LOCAL-00051" summary="Revert to setup-gstreamer action">
+      <option name="closed" value="true"/>
+      <created>1715083949015</created>
+      <option name="number" value="00051"/>
+      <option name="presentableId" value="LOCAL-00051"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715083949015</updated>
+    </task>
+    <task id="LOCAL-00052" summary="Revert to setup-gstreamer action">
+      <option name="closed" value="true"/>
+      <created>1715084012716</created>
+      <option name="number" value="00052"/>
+      <option name="presentableId" value="LOCAL-00052"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715084012716</updated>
     </task>
-    <task id="LOCAL-00001" summary="Clearing up the structure">
+    <task id="LOCAL-00053" summary="Revert to setup-gstreamer action">
       <option name="closed" value="true"/>
-      <created>1714999313464</created>
-      <option name="number" value="00001"/>
-      <option name="presentableId" value="LOCAL-00001"/>
+      <created>1715084136253</created>
+      <option name="number" value="00053"/>
+      <option name="presentableId" value="LOCAL-00053"/>
       <option name="project" value="LOCAL"/>
-      <updated>1714999313464</updated>
+      <updated>1715084136253</updated>
     </task>
-    <task id="LOCAL-00002" summary="Remove some README sections">
+    <task id="LOCAL-00054" summary="Revert to setup-gstreamer action">
       <option name="closed" value="true"/>
-      <created>1714999377033</created>
-      <option name="number" value="00002"/>
-      <option name="presentableId" value="LOCAL-00002"/>
+      <created>1715084367717</created>
+      <option name="number" value="00054"/>
+      <option name="presentableId" value="LOCAL-00054"/>
       <option name="project" value="LOCAL"/>
-      <updated>1714999377033</updated>
+      <updated>1715084367717</updated>
     </task>
-    <task id="LOCAL-00003" summary="Separate source code">
+    <task id="LOCAL-00055" summary="Github actions - add dummy output device for linux">
       <option name="closed" value="true"/>
-      <created>1714999976248</created>
-      <option name="number" value="00003"/>
-      <option name="presentableId" value="LOCAL-00003"/>
+      <created>1715084519162</created>
+      <option name="number" value="00055"/>
+      <option name="presentableId" value="LOCAL-00055"/>
       <option name="project" value="LOCAL"/>
-      <updated>1714999976248</updated>
+      <updated>1715084519162</updated>
     </task>
-    <task id="LOCAL-00004" summary="Refactoring the main file">
+    <task id="LOCAL-00056" summary="Github actions - add timeout and verbosity">
       <option name="closed" value="true"/>
-      <created>1715001862807</created>
-      <option name="number" value="00004"/>
-      <option name="presentableId" value="LOCAL-00004"/>
+      <created>1715084686654</created>
+      <option name="number" value="00056"/>
+      <option name="presentableId" value="LOCAL-00056"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715001862807</updated>
+      <updated>1715084686654</updated>
     </task>
-    <task id="LOCAL-00005" summary="Update requirements">
+    <task id="LOCAL-00057" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715003173317</created>
-      <option name="number" value="00005"/>
-      <option name="presentableId" value="LOCAL-00005"/>
+      <created>1715084997443</created>
+      <option name="number" value="00057"/>
+      <option name="presentableId" value="LOCAL-00057"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715003173317</updated>
+      <updated>1715084997443</updated>
     </task>
-    <task id="LOCAL-00006" summary="Add back Windows support">
+    <task id="LOCAL-00058" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715004151981</created>
-      <option name="number" value="00006"/>
-      <option name="presentableId" value="LOCAL-00006"/>
+      <created>1715085139085</created>
+      <option name="number" value="00058"/>
+      <option name="presentableId" value="LOCAL-00058"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715004151982</updated>
+      <updated>1715085139085</updated>
     </task>
-    <task id="LOCAL-00007" summary="Typo">
+    <task id="LOCAL-00059" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715004758764</created>
-      <option name="number" value="00007"/>
-      <option name="presentableId" value="LOCAL-00007"/>
+      <created>1715085346728</created>
+      <option name="number" value="00059"/>
+      <option name="presentableId" value="LOCAL-00059"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715004758764</updated>
+      <updated>1715085346728</updated>
     </task>
-    <task id="LOCAL-00008" summary="Remove licensing information from README">
+    <task id="LOCAL-00060" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715004972498</created>
-      <option name="number" value="00008"/>
-      <option name="presentableId" value="LOCAL-00008"/>
+      <created>1715085443292</created>
+      <option name="number" value="00060"/>
+      <option name="presentableId" value="LOCAL-00060"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715004972498</updated>
+      <updated>1715085443292</updated>
     </task>
-    <task id="LOCAL-00009" summary="Fix import">
+    <task id="LOCAL-00061" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715006555283</created>
-      <option name="number" value="00009"/>
-      <option name="presentableId" value="LOCAL-00009"/>
+      <created>1715085629196</created>
+      <option name="number" value="00061"/>
+      <option name="presentableId" value="LOCAL-00061"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715006555283</updated>
+      <updated>1715085629196</updated>
     </task>
-    <task id="LOCAL-00010" summary="Fix OSX version">
+    <task id="LOCAL-00062" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715015970445</created>
-      <option name="number" value="00010"/>
-      <option name="presentableId" value="LOCAL-00010"/>
+      <created>1715085788467</created>
+      <option name="number" value="00062"/>
+      <option name="presentableId" value="LOCAL-00062"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715015970445</updated>
+      <updated>1715085788467</updated>
     </task>
-    <task id="LOCAL-00011" summary="Remove additional files">
+    <task id="LOCAL-00063" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715015982231</created>
-      <option name="number" value="00011"/>
-      <option name="presentableId" value="LOCAL-00011"/>
+      <created>1715085868822</created>
+      <option name="number" value="00063"/>
+      <option name="presentableId" value="LOCAL-00063"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715015982231</updated>
+      <updated>1715085868822</updated>
     </task>
-    <task id="LOCAL-00012" summary="Fix setup.py">
+    <task id="LOCAL-00064" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715016251549</created>
-      <option name="number" value="00012"/>
-      <option name="presentableId" value="LOCAL-00012"/>
+      <created>1715085940716</created>
+      <option name="number" value="00064"/>
+      <option name="presentableId" value="LOCAL-00064"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715016251549</updated>
+      <updated>1715085940716</updated>
     </task>
-    <task id="LOCAL-00013" summary="Update documentation">
+    <task id="LOCAL-00065" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715016926338</created>
-      <option name="number" value="00013"/>
-      <option name="presentableId" value="LOCAL-00013"/>
+      <created>1715086197671</created>
+      <option name="number" value="00065"/>
+      <option name="presentableId" value="LOCAL-00065"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715016926338</updated>
+      <updated>1715086197671</updated>
     </task>
-    <task id="LOCAL-00014" summary="Release 2.0.0">
+    <task id="LOCAL-00066" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715017032333</created>
-      <option name="number" value="00014"/>
-      <option name="presentableId" value="LOCAL-00014"/>
+      <created>1715086565429</created>
+      <option name="number" value="00066"/>
+      <option name="presentableId" value="LOCAL-00066"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715017032333</updated>
+      <updated>1715086565429</updated>
     </task>
-    <task id="LOCAL-00015" summary="Add badges">
+    <task id="LOCAL-00067" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715017178649</created>
-      <option name="number" value="00015"/>
-      <option name="presentableId" value="LOCAL-00015"/>
+      <created>1715086781691</created>
+      <option name="number" value="00067"/>
+      <option name="presentableId" value="LOCAL-00067"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715017178649</updated>
+      <updated>1715086781691</updated>
     </task>
-    <task id="LOCAL-00016" summary="Bump version for release">
+    <task id="LOCAL-00068" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715017208426</created>
-      <option name="number" value="00016"/>
-      <option name="presentableId" value="LOCAL-00016"/>
+      <created>1715087004454</created>
+      <option name="number" value="00068"/>
+      <option name="presentableId" value="LOCAL-00068"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715017208426</updated>
+      <updated>1715087004454</updated>
     </task>
-    <task id="LOCAL-00017" summary="README typo">
+    <task id="LOCAL-00069" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715017344053</created>
-      <option name="number" value="00017"/>
-      <option name="presentableId" value="LOCAL-00017"/>
+      <created>1715087496389</created>
+      <option name="number" value="00069"/>
+      <option name="presentableId" value="LOCAL-00069"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715017344053</updated>
+      <updated>1715087496389</updated>
     </task>
-    <task id="LOCAL-00018" summary="Importing changes">
+    <task id="LOCAL-00070" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715017614283</created>
-      <option name="number" value="00018"/>
-      <option name="presentableId" value="LOCAL-00018"/>
+      <created>1715087591063</created>
+      <option name="number" value="00070"/>
+      <option name="presentableId" value="LOCAL-00070"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715017614283</updated>
+      <updated>1715087591063</updated>
     </task>
-    <task id="LOCAL-00019" summary="Remove mentions of supporting web files">
+    <task id="LOCAL-00071" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
-      <created>1715017778386</created>
-      <option name="number" value="00019"/>
-      <option name="presentableId" value="LOCAL-00019"/>
+      <created>1715087761324</created>
+      <option name="number" value="00071"/>
+      <option name="presentableId" value="LOCAL-00071"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715017778386</updated>
+      <updated>1715087761324</updated>
     </task>
-    <task id="LOCAL-00020" summary="Fix typing error">
+    <task id="LOCAL-00072" summary="Github actions - other fixes">
       <option name="closed" value="true"/>
-      <created>1715029081242</created>
-      <option name="number" value="00020"/>
-      <option name="presentableId" value="LOCAL-00020"/>
+      <created>1715088071361</created>
+      <option name="number" value="00072"/>
+      <option name="presentableId" value="LOCAL-00072"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715029081242</updated>
+      <updated>1715088071361</updated>
     </task>
-    <task id="LOCAL-00021" summary="Clear up the license">
+    <task id="LOCAL-00073" summary="Github actions - other fixes">
       <option name="closed" value="true"/>
-      <created>1715030476646</created>
-      <option name="number" value="00021"/>
-      <option name="presentableId" value="LOCAL-00021"/>
+      <created>1715088182515</created>
+      <option name="number" value="00073"/>
+      <option name="presentableId" value="LOCAL-00073"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715030476646</updated>
+      <updated>1715088182515</updated>
     </task>
-    <task id="LOCAL-00022" summary="Add short description">
+    <task id="LOCAL-00074" summary="Github actions - other fixes">
       <option name="closed" value="true"/>
-      <created>1715035847548</created>
-      <option name="number" value="00022"/>
-      <option name="presentableId" value="LOCAL-00022"/>
+      <created>1715088453532</created>
+      <option name="number" value="00074"/>
+      <option name="presentableId" value="LOCAL-00074"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715035847548</updated>
+      <updated>1715088453532</updated>
     </task>
-    <task id="LOCAL-00023" summary="Change case">
+    <task id="LOCAL-00075" summary="Github actions - other fixes">
       <option name="closed" value="true"/>
-      <created>1715035904774</created>
-      <option name="number" value="00023"/>
-      <option name="presentableId" value="LOCAL-00023"/>
+      <created>1715088568535</created>
+      <option name="number" value="00075"/>
+      <option name="presentableId" value="LOCAL-00075"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715035904774</updated>
+      <updated>1715088568535</updated>
     </task>
-    <task id="LOCAL-00024" summary="Add support for URL files">
+    <task id="LOCAL-00076" summary="Skip windows test">
       <option name="closed" value="true"/>
-      <created>1715038575990</created>
-      <option name="number" value="00024"/>
-      <option name="presentableId" value="LOCAL-00024"/>
+      <created>1715088709633</created>
+      <option name="number" value="00076"/>
+      <option name="presentableId" value="LOCAL-00076"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715038575990</updated>
+      <updated>1715088709633</updated>
     </task>
-    <task id="LOCAL-00025" summary="Add support for URL files">
+    <task id="LOCAL-00077" summary="Update README">
       <option name="closed" value="true"/>
-      <created>1715038598510</created>
-      <option name="number" value="00025"/>
-      <option name="presentableId" value="LOCAL-00025"/>
+      <created>1715088969893</created>
+      <option name="number" value="00077"/>
+      <option name="presentableId" value="LOCAL-00077"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715038598510</updated>
+      <updated>1715088969893</updated>
     </task>
-    <task id="LOCAL-00026" summary="isort and black formatting">
+    <task id="LOCAL-00078" summary="Use URLs in blocking test">
       <option name="closed" value="true"/>
-      <created>1715038636110</created>
-      <option name="number" value="00026"/>
-      <option name="presentableId" value="LOCAL-00026"/>
+      <created>1715089442965</created>
+      <option name="number" value="00078"/>
+      <option name="presentableId" value="LOCAL-00078"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715038636110</updated>
+      <updated>1715089442965</updated>
     </task>
-    <task id="LOCAL-00027" summary="Restore python 3.7 compatibility">
+    <task id="LOCAL-00079" summary="Remove audio samples">
       <option name="closed" value="true"/>
-      <created>1715039900731</created>
-      <option name="number" value="00027"/>
-      <option name="presentableId" value="LOCAL-00027"/>
+      <created>1715089800126</created>
+      <option name="number" value="00079"/>
+      <option name="presentableId" value="LOCAL-00079"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715039900731</updated>
+      <updated>1715089800126</updated>
     </task>
-    <task id="LOCAL-00028" summary="Change to packaging system to pyproject.toml">
+    <task id="LOCAL-00080" summary="Modify Linux backend">
       <option name="closed" value="true"/>
-      <created>1715075015844</created>
-      <option name="number" value="00028"/>
-      <option name="presentableId" value="LOCAL-00028"/>
+      <created>1715089812786</created>
+      <option name="number" value="00080"/>
+      <option name="presentableId" value="LOCAL-00080"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715075015844</updated>
+      <updated>1715089812786</updated>
     </task>
-    <task id="LOCAL-00029" summary="Updating legacy download function">
+    <task id="LOCAL-00081" summary="Remove unsued dependency">
       <option name="closed" value="true"/>
-      <created>1715076338617</created>
-      <option name="number" value="00029"/>
-      <option name="presentableId" value="LOCAL-00029"/>
+      <created>1715090132556</created>
+      <option name="number" value="00081"/>
+      <option name="presentableId" value="LOCAL-00081"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715076338617</updated>
+      <updated>1715090132556</updated>
     </task>
-    <task id="LOCAL-00030" summary="Fix missing certificates for download">
+    <task id="LOCAL-00082" summary="Change backend naming">
       <option name="closed" value="true"/>
-      <created>1715077928155</created>
-      <option name="number" value="00030"/>
-      <option name="presentableId" value="LOCAL-00030"/>
+      <created>1715090141200</created>
+      <option name="number" value="00082"/>
+      <option name="presentableId" value="LOCAL-00082"/>
       <option name="project" value="LOCAL"/>
-      <updated>1715077928155</updated>
+      <updated>1715090141200</updated>
     </task>
-    <option name="localTasksCounter" value="31"/>
+    <option name="localTasksCounter" value="83"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -346,35 +500,35 @@
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="Update requirements"/>
-    <MESSAGE value="Add back Windows support"/>
-    <MESSAGE value="Typo"/>
-    <MESSAGE value="Remove licensing information from README"/>
-    <MESSAGE value="Fix import"/>
-    <MESSAGE value="Fix OSX version"/>
-    <MESSAGE value="Remove additional files"/>
-    <MESSAGE value="Fix setup.py"/>
-    <MESSAGE value="Update documentation"/>
-    <MESSAGE value="Release 2.0.0"/>
-    <MESSAGE value="Add badges"/>
-    <MESSAGE value="Bump version for release"/>
-    <MESSAGE value="README typo"/>
-    <MESSAGE value="Importing changes"/>
-    <MESSAGE value="Remove mentions of supporting web files"/>
-    <MESSAGE value="Fix typing error"/>
-    <MESSAGE value="Clear up the license"/>
-    <MESSAGE value="Add short description"/>
-    <MESSAGE value="Change case"/>
-    <MESSAGE value="Add support for URL files"/>
     <MESSAGE value="isort and black formatting"/>
     <MESSAGE value="Restore python 3.7 compatibility"/>
     <MESSAGE value="Change to packaging system to pyproject.toml"/>
     <MESSAGE value="Updating legacy download function"/>
     <MESSAGE value="Fix missing certificates for download"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Fix missing certificates for download"/>
+    <MESSAGE value="Install and use certifi by default"/>
+    <MESSAGE value="Add tests and github workflows"/>
+    <MESSAGE value="Isort and Black formatting"/>
+    <MESSAGE value="Install gstreamer for test"/>
+    <MESSAGE value="Add separate tests for Windows and Mac OS"/>
+    <MESSAGE value="Remove 3.7 runner from Mac OS"/>
+    <MESSAGE value="Update workflows"/>
+    <MESSAGE value="Update workflows - force install"/>
+    <MESSAGE value="Revert to setup-gstreamer action"/>
+    <MESSAGE value="Github actions - add dummy output device for linux"/>
+    <MESSAGE value="Github actions - add timeout and verbosity"/>
+    <MESSAGE value="Github actions - add local sound files"/>
+    <MESSAGE value="Github actions - other fixes"/>
+    <MESSAGE value="Skip windows test"/>
+    <MESSAGE value="Update README"/>
+    <MESSAGE value="Use URLs in blocking test"/>
+    <MESSAGE value="Remove audio samples"/>
+    <MESSAGE value="Modify Linux backend"/>
+    <MESSAGE value="Remove unsued dependency"/>
+    <MESSAGE value="Change backend naming"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Change backend naming"/>
   </component>
 </project>
```

### Comparing `playsound3-2.1.2/.idea/inspectionProfiles/Project_Default.xml` & `playsound3-2.1.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.2/playsound3/playsound3.py` & `playsound3-2.1.4/playsound3/playsound3.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,64 @@
 import atexit
 import ctypes
 import logging
 import platform
+import ssl
 import subprocess
 import tempfile
-import urllib.request
 import urllib.error
+import urllib.request
 import uuid
 from pathlib import Path
 from threading import Thread
 
+import certifi
+
 logger = logging.getLogger(__name__)
 
 SYSTEM = platform.system()
 DOWNLOAD_CACHE = dict()
 
 
 class PlaysoundException(Exception):
     pass
 
 
 def playsound(sound, block: bool = True) -> None:
     """Play a sound file using an audio backend availabile in your system.
 
     Args:
-        sound: Path to the sound file. Can be either an str or pathlib.Path.
+        sound: Path or URL to the sound file. Can be a string or pathlib.Path.
         block: If True, the function will block execution until the sound finishes playing.
+               If False, sound will play in a background thread.
     """
     sound = _prepare_path(sound)
 
     if SYSTEM == "Linux":
-        func = _playsound_gstreamer
+        func = _playsound_gst_play
     elif SYSTEM == "Windows":
-        func = _playsound_winmm
+        func = _playsound_mci_winmm
     elif SYSTEM == "Darwin":
         func = _playsound_afplay
     else:
         raise PlaysoundException(f"Platform '{SYSTEM}' is not supported")
 
     if block:
         func(sound)
     else:
-        t = Thread(target=func, args=(sound,), daemon=True).start()
+        Thread(target=func, args=(sound,), daemon=True).start()
 
 
 def _download_sound_from_web(link, destination):
     # Identifies itself as a browser to avoid HTTP 403 errors
     headers = {"User-Agent": "Mozilla/5.0 (Windows NT 6.1; Win64; x64)"}
     request = urllib.request.Request(link, headers=headers)
-
-    try:
-        import ssl
-        import certifi
-
-        context = ssl.create_default_context(cafile=certifi.where())
-    except ImportError:
-        context = None
-
-    try:
-        with urllib.request.urlopen(request, context=context) as response, open(destination, "wb") as out_file:
-            out_file.write(response.read())
-    except urllib.error.HTTPError as e:
-        msg = f"Failed to download sound from {link}: {e}\nTry running 'pip install certifi'"
-        raise PlaysoundException(msg)
+    context = ssl.create_default_context(cafile=certifi.where())
+    with urllib.request.urlopen(request, context=context) as response, open(destination, "wb") as out_file:
+        out_file.write(response.read())
 
 
 def _prepare_path(sound):
     if sound.startswith(("http://", "https://")):
         # To play file from URL, we download the file first to a temporary location and cache it
         if sound not in DOWNLOAD_CACHE:
             with tempfile.NamedTemporaryFile(delete=False, prefix="playsound3-") as f:
@@ -77,15 +69,25 @@
     path = Path(sound)
 
     if not path.exists():
         raise PlaysoundException(f"File not found: {sound}")
     return path.absolute().as_posix()
 
 
-def _playsound_gstreamer(sound):
+def _playsound_gst_play(sound):
+    """Uses gst-play-1.0 utility (built-in Linux)."""
+    logger.debug("gst-play-1.0: starting playing %s", sound)
+    try:
+        subprocess.run(["gst-play-1.0", "--no-interactive", "--quiet", sound], check=True)
+    except subprocess.CalledProcessError as e:
+        raise PlaysoundException(f"gst-play-1.0 failed to play sound: {e}")
+    logger.debug("gst-play-1.0: finishing play %s", sound)
+
+
+def _playsound_gstreamer_legacy(sound):
     """Play a sound using gstreamer (built-in Linux)."""
 
     if not sound.startswith("file://"):
         sound = "file://" + urllib.request.pathname2url(sound)
 
     import gi
 
@@ -113,19 +115,19 @@
 
 
 def _send_winmm_mci_command(command):
     winmm = ctypes.WinDLL("winmm.dll")
     buffer = ctypes.create_string_buffer(255)
     error_code = winmm.mciSendStringA(ctypes.c_char_p(command.encode()), buffer, 254, 0)
     if error_code:
-        logger.error("Error code: %s", error_code)
+        logger.error("MCI error code: %s", error_code)
     return buffer.value
 
 
-def _playsound_winmm(sound):
+def _playsound_mci_winmm(sound):
     """Play a sound utilizing windll.winmm."""
 
     # Select a unique alias for the sound
     alias = str(uuid.uuid4())
     logger.debug("winmm: starting playing %s", sound)
     _send_winmm_mci_command(f'open "{sound}" type mpegvideo alias {alias}')
     _send_winmm_mci_command(f"play {alias} wait")
```

### Comparing `playsound3-2.1.2/.gitignore` & `playsound3-2.1.4/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -56,7 +56,8 @@
 docs/_build/
 
 # PyBuilder
 target/
 
 # Custom
 devel/
+**/script*
```

### Comparing `playsound3-2.1.2/LICENSE` & `playsound3-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.2/README.md` & `playsound3-2.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -33,17 +33,19 @@
 The playsound module contains only one thing - the function (also named) playsound:
 
 ```python
 def playsound(sound, block: bool = True) -> None:
     """Play a sound file using an audio backend availabile in your system.
 
     Args:
-        sound: Path to the sound file. Can be either an str or pathlib.Path.
+        sound: Path or URL to the sound file. Can be a string or pathlib.Path.
         block: If True, the function will block execution until the sound finishes playing.
+               If False, sound will play in a background thread.
     """
+    ...
 ```
 
 It requires one argument - the path to the file with the sound you'd like to play.
 This should be a local file or a URL.
 There's an optional second argument, block, which is set to True by default.
 Setting it to False makes the function run asynchronously.
```

### Comparing `playsound3-2.1.2/pyproject.toml` & `playsound3-2.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "playsound3"
-version = "2.1.2"
+version = "2.1.4"
 requires-python = ">=3.7"
 authors = [
     { name = "Szymon Mikler", email = "sjmikler@gmail.com" },
     { name = "Taylor Marks", email = "taylor@marksfam.com" },
 ]
 maintainers = [
     { name = "Szymon Mikler", email = "sjmikler@gmail.com" },
@@ -29,26 +29,30 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Multimedia :: Sound/Audio :: MIDI",
     "Topic :: Multimedia :: Sound/Audio :: Players",
     "Topic :: Multimedia :: Sound/Audio :: Players :: MP3",
     "Operating System :: OS Independent",
 ]
-dependencies = [
-    "pygobject; platform_system=='Linux'",
-]
+dependencies = ["certifi"]
 
 [project.urls]
 Repository = "https://github.com/sjmikler/playsound3"
 Issues = "https://github.com/sjmikler/playsound3/issues"
 Documentation = "https://github.com/sjmikler/playsound3?tab=readme-ov-file#documentation"
 
 ##################################
 ## Formatting and testing tools ##
 ##################################
 
+[tool.mypy]
+ignore_missing_imports = true
+
+[tool.flake8]
+max-line-length = 120
+
 [tool.isort]
 profile = "black"
 line_length = 120
 
 [tool.black]
 line_length = 120
```

### Comparing `playsound3-2.1.2/PKG-INFO` & `playsound3-2.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: playsound3
-Version: 2.1.2
+Version: 2.1.4
 Summary: Cross-platform library to play audio files
 Project-URL: Repository, https://github.com/sjmikler/playsound3
 Project-URL: Issues, https://github.com/sjmikler/playsound3/issues
 Project-URL: Documentation, https://github.com/sjmikler/playsound3?tab=readme-ov-file#documentation
 Author-email: Szymon Mikler <sjmikler@gmail.com>, Taylor Marks <taylor@marksfam.com>
 Maintainer-email: Szymon Mikler <sjmikler@gmail.com>
 License: MIT License
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players :: MP3
 Requires-Python: >=3.7
-Requires-Dist: pygobject; platform_system == 'Linux'
+Requires-Dist: certifi
 Description-Content-Type: text/markdown
 
 > This repository was forked from [TaylorSMarks/playsound](https://github.com/TaylorSMarks/playsound)
 
 # playsound3
 
 [![PyPi version](https://img.shields.io/badge/dynamic/json?label=latest&query=info.version&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fplaysound3%2Fjson)](https://pypi.org/project/playsound3)
@@ -63,17 +63,19 @@
 The playsound module contains only one thing - the function (also named) playsound:
 
 ```python
 def playsound(sound, block: bool = True) -> None:
     """Play a sound file using an audio backend availabile in your system.
 
     Args:
-        sound: Path to the sound file. Can be either an str or pathlib.Path.
+        sound: Path or URL to the sound file. Can be a string or pathlib.Path.
         block: If True, the function will block execution until the sound finishes playing.
+               If False, sound will play in a background thread.
     """
+    ...
 ```
 
 It requires one argument - the path to the file with the sound you'd like to play.
 This should be a local file or a URL.
 There's an optional second argument, block, which is set to True by default.
 Setting it to False makes the function run asynchronously.
```

