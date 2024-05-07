# Comparing `tmp/revhubinterface-1.3.0.tar.gz` & `tmp/revhubinterface-1.3.1.dev25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.0.tar", last modified: Tue May  7 04:11:03 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.1.dev25.tar", last modified: Tue May  7 20:23:06 2024, max compression
```

## Comparing `revhubinterface-1.3.0.tar` & `revhubinterface-1.3.1.dev25.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-07 04:11:03.161022 revhubinterface-1.3.0/
--rw-rw-r--   0 james     (1000) james     (1000)       80 2024-05-07 01:41:32.000000 revhubinterface-1.3.0/.gitignore
--rw-rw-r--   0 james     (1000) james     (1000)     2592 2024-05-02 23:56:52.000000 revhubinterface-1.3.0/LICENSE.txt
--rw-r--r--   0 james     (1000) james     (1000)      172 2024-05-07 04:11:03.161022 revhubinterface-1.3.0/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)     3685 2024-05-07 01:41:32.000000 revhubinterface-1.3.0/README.md
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-07 04:11:03.161022 revhubinterface-1.3.0/REVHubInterface/
--rw-rw-r--   0 james     (1000) james     (1000)    20812 2024-05-07 02:39:40.000000 revhubinterface-1.3.0/REVHubInterface/REV2mSensor.py
--rw-rw-r--   0 james     (1000) james     (1000)     1154 2024-05-07 04:01:09.000000 revhubinterface-1.3.0/REVHubInterface/REVADC.py
--rw-rw-r--   0 james     (1000) james     (1000)     5165 2024-05-07 02:39:55.000000 revhubinterface-1.3.0/REVHubInterface/REVColorSensorV3.py
--rw-rw-r--   0 james     (1000) james     (1000)     1176 2024-05-07 04:01:09.000000 revhubinterface-1.3.0/REVHubInterface/REVComPorts.py
--rw-rw-r--   0 james     (1000) james     (1000)     2552 2024-05-07 02:38:41.000000 revhubinterface-1.3.0/REVHubInterface/REVDIO.py
--rw-rw-r--   0 james     (1000) james     (1000)    15925 2024-05-07 02:38:58.000000 revhubinterface-1.3.0/REVHubInterface/REVI2C.py
--rw-rw-r--   0 james     (1000) james     (1000)     4757 2024-05-07 02:37:17.000000 revhubinterface-1.3.0/REVHubInterface/REVModule.py
--rw-rw-r--   0 james     (1000) james     (1000)    11713 2024-05-07 02:37:40.000000 revhubinterface-1.3.0/REVHubInterface/REVMotor.py
--rw-rw-r--   0 james     (1000) james     (1000)     3184 2024-05-07 02:38:11.000000 revhubinterface-1.3.0/REVHubInterface/REVServo.py
--rw-rw-r--   0 james     (1000) james     (1000)    16892 2024-05-07 04:01:09.000000 revhubinterface-1.3.0/REVHubInterface/REVcomm.py
--rw-rw-r--   0 james     (1000) james     (1000)    73523 2024-05-07 01:41:32.000000 revhubinterface-1.3.0/REVHubInterface/REVmessages.py
--rw-rw-r--   0 james     (1000) james     (1000)        0 2024-05-07 02:11:41.000000 revhubinterface-1.3.0/REVHubInterface/__init__.py
--rw-rw-r--   0 james     (1000) james     (1000)    73418 2024-05-07 04:01:09.000000 revhubinterface-1.3.0/REVHubInterface/__main__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-07 04:11:03.161022 revhubinterface-1.3.0/REVHubInterface.egg-info/
--rw-r--r--   0 james     (1000) james     (1000)      172 2024-05-07 04:11:03.000000 revhubinterface-1.3.0/REVHubInterface.egg-info/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)      829 2024-05-07 04:11:03.000000 revhubinterface-1.3.0/REVHubInterface.egg-info/SOURCES.txt
--rw-rw-r--   0 james     (1000) james     (1000)        1 2024-05-07 04:11:03.000000 revhubinterface-1.3.0/REVHubInterface.egg-info/dependency_links.txt
--rw-rw-r--   0 james     (1000) james     (1000)       68 2024-05-07 04:11:03.000000 revhubinterface-1.3.0/REVHubInterface.egg-info/entry_points.txt
--rw-rw-r--   0 james     (1000) james     (1000)       42 2024-05-07 04:11:03.000000 revhubinterface-1.3.0/REVHubInterface.egg-info/requires.txt
--rw-rw-r--   0 james     (1000) james     (1000)       16 2024-05-07 04:11:03.000000 revhubinterface-1.3.0/REVHubInterface.egg-info/top_level.txt
--rwxrwxr-x   0 james     (1000) james     (1000)       39 2024-05-07 01:41:32.000000 revhubinterface-1.3.0/REVHubInterface.sh
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2024-05-07 04:11:03.161022 revhubinterface-1.3.0/flatpak/
--rw-rw-r--   0 james     (1000) james     (1000)    17481 2024-05-07 01:41:32.000000 revhubinterface-1.3.0/flatpak/flatpak-pip-generator
--rw-rw-r--   0 james     (1000) james     (1000)     2274 2024-05-07 01:41:32.000000 revhubinterface-1.3.0/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-rw-r--   0 james     (1000) james     (1000)     2839 2024-05-07 01:41:32.000000 revhubinterface-1.3.0/flatpak/python3-requirements.json
--rw-rw-r--   0 james     (1000) james     (1000)     1094 2024-05-07 01:41:32.000000 revhubinterface-1.3.0/flatpak/tkinter.json
--rw-rw-r--   0 james     (1000) james     (1000)      460 2024-05-07 04:04:56.000000 revhubinterface-1.3.0/pyproject.toml
--rw-rw-r--   0 james     (1000) james     (1000)       41 2024-05-06 22:12:48.000000 revhubinterface-1.3.0/requirements.txt
--rw-rw-r--   0 james     (1000) james     (1000)       38 2024-05-07 04:11:03.161022 revhubinterface-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:06.761077 revhubinterface-1.3.1.dev25/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:06.753077 revhubinterface-1.3.1.dev25/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:06.757077 revhubinterface-1.3.1.dev25/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-07 20:23:06.761077 revhubinterface-1.3.1.dev25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:06.757077 revhubinterface-1.3.1.dev25/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73547 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:06.761077 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-07 20:23:06.000000 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-07 20:23:06.000000 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:23:06.000000 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 20:23:06.000000 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 20:23:06.000000 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 20:23:06.000000 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:06.761077 revhubinterface-1.3.1.dev25/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/flatpak/flatpak-pip-generator
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:23:06.761077 revhubinterface-1.3.1.dev25/setup.cfg
```

### Comparing `revhubinterface-1.3.0/LICENSE.txt` & `revhubinterface-1.3.1.dev25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/README.md` & `revhubinterface-1.3.1.dev25/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.1.dev25/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/REVHubInterface/REVADC.py` & `revhubinterface-1.3.1.dev25/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.1.dev25/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.1.dev25/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.1.dev25/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.1.dev25/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/REVHubInterface/REVModule.py` & `revhubinterface-1.3.1.dev25/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.1.dev25/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/REVHubInterface/REVServo.py` & `revhubinterface-1.3.1.dev25/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.1.dev25/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.1.dev25/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/REVHubInterface/__main__.py` & `revhubinterface-1.3.1.dev25/REVHubInterface/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from . import REVcomm
-from .REV2mSensor import REV2mSensor
-from .REVColorSensorV3 import REVColorSensorV3
-from .REVcomm import *
+from REVHubInterface import REVcomm # relative imports don't work here due to pyinstaller issue
+from REVHubInterface.REV2mSensor import REV2mSensor
+from REVHubInterface.REVColorSensorV3 import REVColorSensorV3
+from REVHubInterface.REVcomm import *
 from functools import partial
 from sys import platform
 import tkinter as tk, tkinter.ttk, tkinter.filedialog, tkinter.messagebox, os, subprocess, time, platform
 
 try:
     import ft232
 except Exception as e: 
@@ -1425,15 +1425,15 @@
         try:
             import sv_ttk
             print('Loaded Tk theme: Sun Valley')
             sv_ttk.set_theme("dark")
         except:
             pass
 
-    xroot.title('Crossplatform Hub Interface')
+    xroot.title('REV Hub Interface - Community Edition')
     try:
         xroot.iconbitmap('resource\\\\favicon.ico')
     except:
         try:
             xroot.iconbitmap('favicon.ico')
         except:
             pass
```

### Comparing `revhubinterface-1.3.0/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 .gitignore
 LICENSE.txt
 README.md
 REVHubInterface.sh
+REVHubInterface.spec
 pyproject.toml
 requirements.txt
+.github/workflows/pyinstaller.yml
+.github/workflows/python-publish.yml
 REVHubInterface/REV2mSensor.py
 REVHubInterface/REVADC.py
 REVHubInterface/REVColorSensorV3.py
 REVHubInterface/REVComPorts.py
 REVHubInterface/REVDIO.py
 REVHubInterface/REVI2C.py
 REVHubInterface/REVModule.py
@@ -21,9 +24,8 @@
 REVHubInterface.egg-info/SOURCES.txt
 REVHubInterface.egg-info/dependency_links.txt
 REVHubInterface.egg-info/entry_points.txt
 REVHubInterface.egg-info/requires.txt
 REVHubInterface.egg-info/top_level.txt
 flatpak/flatpak-pip-generator
 flatpak/org.unofficialrevport.REVHubInterface.yml
-flatpak/python3-requirements.json
-flatpak/tkinter.json
+flatpak/python3-requirements.json
```

### Comparing `revhubinterface-1.3.0/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.1.dev25/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.0/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.1.dev25/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 runtime: org.freedesktop.Platform
 runtime-version: '23.08'
 sdk: org.freedesktop.Sdk
 command: REVHubInterface.sh
 finish-args:
   - --device=all
   - --share=ipc
-  - --socket=fallback-x11
-  - --socket=wayland
+  - --socket=x11
   - --device=dri
-  - --socket=pulseaudio
+  - --talk-name=org.freedesktop.Flatpak 
 modules:
   - python3-requirements.json
   - name: tkinter
     buildsystem: simple
     build-commands:
       - pip3 install --prefix=${FLATPAK_DEST} .
     sources:
       - type: git
         url: https://github.com/iwalton3/tkinter-standalone
-        commit: ba946536054f9d27a08aafde21aa18330ce05729
+        commit: 88aa05075d90d393a29a484bce676e237d311082
     modules:
       - name: tcl
         buildsystem: autotools
         subdir: unix
         post-install:
           - chmod 755 /app/lib/libtcl*.so
         cleanup:
@@ -62,8 +61,8 @@
     builddir: true
     build-commands:
       - pip3 install --verbose --exists-action=i --no-index --find-links="file://${PWD}" --prefix=${FLATPAK_DEST} . --no-build-isolation
       - install -D REVHubInterface.sh /app/bin/REVHubInterface.sh
     sources:
       - type: git
         url: https://github.com/unofficial-rev-port/REVHubInterface.git
-        branch: package-atomic
+        branch: main
```

### Comparing `revhubinterface-1.3.0/flatpak/python3-requirements.json` & `revhubinterface-1.3.1.dev25/flatpak/python3-requirements.json`

 * *Files identical despite different names*

