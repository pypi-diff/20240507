# Comparing `tmp/proboscis_async_events-0.1.4.tar.gz` & `tmp/proboscis_async_events-0.1.5.tar.gz`

## Comparing `proboscis_async_events-0.1.4.tar` & `proboscis_async_events-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.python-version
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/requirements-dev.lock
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/requirements.lock
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/.gitignore
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/modules.xml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/proboscis-async-events.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/vcs.xml
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/workspace.xml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/codeStyles/Project.xml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/src/proboscis_async_events/__init__.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/src/proboscis_async_events/messaging.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/test/test_messaging.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/.gitignore
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/README.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.python-version
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/requirements-dev.lock
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/requirements.lock
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/.gitignore
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/modules.xml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/proboscis-async-events.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/codeStyles/Project.xml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/src/proboscis_async_events/__init__.py
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/src/proboscis_async_events/messaging.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/test/test_messaging.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/.gitignore
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/README.md
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.5/PKG-INFO
```

### Comparing `proboscis_async_events-0.1.4/.idea/proboscis-async-events.iml` & `proboscis_async_events-0.1.5/.idea/proboscis-async-events.iml`

 * *Files identical despite different names*

### Comparing `proboscis_async_events-0.1.4/.idea/workspace.xml` & `proboscis_async_events-0.1.5/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `proboscis_async_events-0.1.4/.idea/inspectionProfiles/Project_Default.xml` & `proboscis_async_events-0.1.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `proboscis_async_events-0.1.4/pyproject.toml` & `proboscis_async_events-0.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "proboscis-async-events"
-version = "0.1.4"
+version = "0.1.5"
 description = "Add your description here"
 authors = [
     { name = "proboscis", email = "nameissoap@gmail.com" }
 ]
 dependencies = [
     "pampy>=0.3.0",
     "pytest>=8.2.0",
@@ -18,10 +18,9 @@
 
 [tool.rye]
 managed = true
 dev-dependencies = []
 
 [tool.hatch.metadata]
 allow-direct-references = true
-
 [tool.hatch.build.targets.wheel]
 packages = ["src/proboscis_async_events"]
```

