# Comparing `tmp/solidwrap-2.1.1.tar.gz` & `tmp/solidwrap-2.1.2.tar.gz`

## Comparing `solidwrap-2.1.1.tar` & `solidwrap-2.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     8020 2020-02-02 00:00:00.000000 solidwrap-2.1.1/info/API Reference.rst
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 solidwrap-2.1.1/solidwrap/__init__.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 solidwrap-2.1.1/solidwrap/containers.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 solidwrap-2.1.1/solidwrap/logger.py
--rw-r--r--   0        0        0    16870 2020-02-02 00:00:00.000000 solidwrap-2.1.1/solidwrap/solidwrap.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 solidwrap-2.1.1/solidwrap/utilities.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 solidwrap-2.1.1/tests/tests.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 solidwrap-2.1.1/LICENSE
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 solidwrap-2.1.1/README.rst
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 solidwrap-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 solidwrap-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     8020 2020-02-02 00:00:00.000000 solidwrap-2.1.2/info/API Reference.rst
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 solidwrap-2.1.2/solidwrap/__init__.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 solidwrap-2.1.2/solidwrap/containers.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 solidwrap-2.1.2/solidwrap/logger.py
+-rw-r--r--   0        0        0    19209 2020-02-02 00:00:00.000000 solidwrap-2.1.2/solidwrap/solidwrap.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 solidwrap-2.1.2/solidwrap/utilities.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 solidwrap-2.1.2/tests/tests.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 solidwrap-2.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 solidwrap-2.1.2/README.rst
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 solidwrap-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 solidwrap-2.1.2/PKG-INFO
```

### Comparing `solidwrap-2.1.1/info/API Reference.rst` & `solidwrap-2.1.2/info/API Reference.rst`

 * *Files identical despite different names*

### Comparing `solidwrap-2.1.1/solidwrap/containers.py` & `solidwrap-2.1.2/solidwrap/containers.py`

 * *Files identical despite different names*

### Comparing `solidwrap-2.1.1/solidwrap/logger.py` & `solidwrap-2.1.2/solidwrap/logger.py`

 * *Files identical despite different names*

### Comparing `solidwrap-2.1.1/solidwrap/solidwrap.py` & `solidwrap-2.1.2/solidwrap/solidwrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self.version = version
 
     # LIFETIME MANAGEMENT METHODS
     def connect(self, headless: bool = False) -> bool:
         '''Creates a connection to the SolidWorks client.'''
         log.critical(f"connecting to SolidWorks client ( {self.version} )")
         client_key = compute_client_key(self.version)
-        
+
         # Attempt client dispatch
         log.info('establishing connection...')
         try:
             pycom.CoInitialize()
             if (com_object := win.Dispatch(client_key)):
                 SolidWorks.client = com_object
                 SolidWorks.client.visible = not headless
@@ -332,15 +332,15 @@
         # Format a check in comment
         message = AUTOMATION_MESSAGE
         if comment:
             message = message + ': ' + comment
 
         # Check current document state         
         if not file.IsLocked:
-            log.warning(f"file is already checked in: '{filepath.name}'")
+            log.info(f"file is already checked in: '{filepath.name}'")
             return None
         
         # Execute PDM-API method    
         file.UnlockFile(0, message)
             
     def checkout(self, filepath: Filepath) -> None:
         """
@@ -353,15 +353,15 @@
 
         # Get PDM-API objects
         directory = Vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder
         file = directory.GetFile(filepath.name)                         # IEdmFile
 
         # Check current document state
         if file.IsLocked:
-            log.warning(f"file is already checked out: '{filepath.name}'")
+            log.info(f"file is already checked out: '{filepath.name}'")
             return None
         
         # Execute PDM-API method
         file.LockFile(directory.ID, 0)
 
     def undo_checkout(self, filepath: Filepath) -> None:
         """
@@ -374,38 +374,95 @@
 
         # Get PDM-API objects
         directory = Vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder
         file = directory.GetFile(filepath.name)                         # IEdmFile
 
         # Check current document state
         if not file.IsLocked:
-            log.warning(f"file is not checked out: '{filepath.name}'")
+            log.info(f"file is not checked out: '{filepath.name}'")
             return None
         
         # Execute PDM-API method
         file.UndoLockFile(0)
 
     # WORKFLOW STATE METHODS
-    # WIP
-    # def change_state(self, filepath: Filepath, state: str,
-    #     comment: str = None) -> None:
-    #     log.info(f"changing workflow state: '{filepath.name}'")
-    #     # GET FILE WORKFLOW DATA
-    #     log.debug(f"current state: '{asdf}'")
-    #     log.debug(f"new state: '{ghjk}'")
+    def change_state(self, filepath: Filepath, transition: str, comment: str = None) -> None:
+        '''Changes the PDM state of a file using a provided transition.'''
+
+        # Get PDM-API objects
+        directory = Vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder
+        file = directory.GetFile(filepath.name)                         # IEdmFile
+        
+        # Get all possible transitions
+        index: int = 0
+        transitions: List = []
+        current = file.CurrentState
+        position = current.GetFirstTransitionPosition()
+        while not position.IsNull:
+            possibility = current.GetNextTransition(position)
+            transitions.append(possibility)
+            index += 1
+        
+        # Get next state by checking against possible transitions
+        found: bool = False
+        for test in transitions:
+            if test.Name == transition:
+                next_state = test.ToState
+                log.info(fr"transitioning file ( '{filepath.name}' ) to state: {next_state.Name}")
+                found = True
+        if not found:
+            log.warning(f"failed to execute transition: '{transition.Name}'")
+            return
+        
+        # Format a default comment
+        if comment is None:
+            comment = AUTOMATION_MESSAGE
+
+        # Define COM VARIANT args
+        arg1 = win.VARIANT(pycom.VT_I4, int(directory.ID))
+        arg2 = win.VARIANT(pycom.VT_BSTR, comment)
+
+        # SolidWorks API call
+        file.ChangeState(next_state, arg1.value, arg2.value, 0)
 
     # DATA RETRIEVAL METHODS
     def get_revision(self, filepath: Filepath) -> str:
         '''Gets a file's release version.'''
         log.debug('release revision')
 
         # Get PDM-API objects
-        directory = Vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
-        file = directory.GetFile(filepath.name)                         # IEdmFile5
+        directory = Vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder
+        file = directory.GetFile(filepath.name)                         # IEdmFile
         return file.CurrentRevision
+    
+    def get_state(self, filepath: Filepath) -> str:
+        '''Gets a file's current PDM state.'''
+        
+        # Get PDM-API objects
+        directory = Vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder
+        file = directory.GetFile(filepath.name)                         # IEdmFile
+        return file.CurrentState.Name
+
+    def get_transitions(self, filepath: Filepath) -> List[str]:
+        '''Gets all of the possible state transitions for a file's current
+        PDM state.'''
+        
+        # Get PDM-API objects
+        directory = Vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder
+        file = directory.GetFile(filepath.name)                         # IEdmFile
+        
+        index: int = 0
+        transitions: List = []
+        current = file.CurrentState
+        position = current.GetFirstTransitionPosition()
+        while not position.IsNull:
+            transition = current.GetNextTransition(position)
+            transitions.append(transition.Name)
+            index += 1
+        return transitions
 
 
 # FUNCTIONS
 def prepare_export(document: SWDocument, target_format: SWExportFormat,
         destination: Filepath = None) -> Filepath:
     '''Prepares a document for an export operation.'''
     log.debug(f"preparing document for export: '{document.source.name}'")
@@ -432,15 +489,15 @@
     root = document.source.root
     extension = target_format.value
     return Filepath(fr"{destination.complete}\{root}.{extension}")
 
 
 # OBJECTS
 # Which document types are compatible with which export formats?
-export_matrix: Dict[SWDocType, List[Type[SWExportFormat]]] = {
+export_matrix: Dict[SWDocType, List[SWExportFormat]] = {
     SWDocType.PART: [
         SWExportFormat.IMAGE,
         SWExportFormat.PARASOLID,
         SWExportFormat.STEP,
         SWExportFormat.STL
     ],
     SWDocType.ASSEMBLY: [
```

### Comparing `solidwrap-2.1.1/solidwrap/utilities.py` & `solidwrap-2.1.2/solidwrap/utilities.py`

 * *Files identical despite different names*

### Comparing `solidwrap-2.1.1/tests/tests.py` & `solidwrap-2.1.2/tests/tests.py`

 * *Files identical despite different names*

### Comparing `solidwrap-2.1.1/LICENSE` & `solidwrap-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `solidwrap-2.1.1/README.rst` & `solidwrap-2.1.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -104,11 +104,11 @@
 
 **For a local installation**
 
 Extract the contents of this module to a safe location. Open a new terminal and navigate to the top level directory of your project. Run the following command:
 
 .. code:: sh
 
-  py -m pip install "DIRECTORY_HERE\solidwrap\dist\solidwrap-2.0.0.tar.gz"
+  py -m pip install "DIRECTORY_HERE\solidwrap\dist\solidwrap-2.1.2.tar.gz"
 
 - ``DIRECTORY_HERE`` should be replaced with the complete filepath to the folder where you saved the SolidWrap module contents.
-- Depending on the release of SolidWrap you've chosen, you may have to change ``2.0.0`` to reflect your specific version.
+- Depending on the release of SolidWrap you've chosen, you may have to change ``2.1.2`` to reflect your specific version.
```

### Comparing `solidwrap-2.1.1/pyproject.toml` & `solidwrap-2.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "solidwrap"
-version = "2.1.1"
+version = "2.1.2"
 authors = [
   { name="Sean Yeatts" },
 ]
 license = {text = "MIT License"}
 description = "Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow."
 readme = "README.rst"
 requires-python = ">=3.7"
```

### Comparing `solidwrap-2.1.1/PKG-INFO` & `solidwrap-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: solidwrap
-Version: 2.1.1
+Version: 2.1.2
 Summary: Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow.
 Project-URL: Homepage, https://github.com/SeanYeatts/SolidWrap/tree/main
 Project-URL: Bug Tracker, https://github.com/users/SeanYeatts/projects/6/views/1
 Author: Sean Yeatts
 License: MIT License
-License-File: LICENSE
+License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 
 SolidWrap
@@ -119,11 +119,11 @@
 
 **For a local installation**
 
 Extract the contents of this module to a safe location. Open a new terminal and navigate to the top level directory of your project. Run the following command:
 
 .. code:: sh
 
-  py -m pip install "DIRECTORY_HERE\solidwrap\dist\solidwrap-2.0.0.tar.gz"
+  py -m pip install "DIRECTORY_HERE\solidwrap\dist\solidwrap-2.1.2.tar.gz"
 
 - ``DIRECTORY_HERE`` should be replaced with the complete filepath to the folder where you saved the SolidWrap module contents.
-- Depending on the release of SolidWrap you've chosen, you may have to change ``2.0.0`` to reflect your specific version.
+- Depending on the release of SolidWrap you've chosen, you may have to change ``2.1.2`` to reflect your specific version.
```

