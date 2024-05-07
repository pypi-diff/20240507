# Comparing `tmp/pyupgrader-2.5.13b2.tar.gz` & `tmp/pyupgrader-2.5.16b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyupgrader-2.5.13b2.tar", last modified: Mon Apr  1 04:39:44 2024, max compression
+gzip compressed data, was "pyupgrader-2.5.16b2.tar", last modified: Tue May  7 00:23:22 2024, max compression
```

## Comparing `pyupgrader-2.5.13b2.tar` & `pyupgrader-2.5.16b2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:39:44.545202 pyupgrader-2.5.13b2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-01 04:39:44.545202 pyupgrader-2.5.13b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:39:44.541202 pyupgrader-2.5.13b2/pyupgrader/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/pyupgrader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/pyupgrader/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    19507 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/pyupgrader/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:39:44.541202 pyupgrader-2.5.13b2/pyupgrader/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/pyupgrader/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/pyupgrader/utilities/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/pyupgrader/utilities/file_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)    20745 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/pyupgrader/utilities/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/pyupgrader/utilities/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:39:44.545202 pyupgrader-2.5.13b2/pyupgrader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-01 04:39:44.000000 pyupgrader-2.5.13b2/pyupgrader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-01 04:39:44.000000 pyupgrader-2.5.13b2/pyupgrader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 04:39:44.000000 pyupgrader-2.5.13b2/pyupgrader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 04:39:44.000000 pyupgrader-2.5.13b2/pyupgrader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 04:39:44.000000 pyupgrader-2.5.13b2/pyupgrader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 04:39:44.000000 pyupgrader-2.5.13b2/pyupgrader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 04:39:44.545202 pyupgrader-2.5.13b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:39:44.545202 pyupgrader-2.5.13b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/tests/test_file_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-01 04:39:36.000000 pyupgrader-2.5.13b2/tests/test_main_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:23:22.477376 pyupgrader-2.5.16b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-07 00:23:22.477376 pyupgrader-2.5.16b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:23:22.473376 pyupgrader-2.5.16b2/pyupgrader/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/pyupgrader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/pyupgrader/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19830 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/pyupgrader/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:23:22.477376 pyupgrader-2.5.16b2/pyupgrader/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/pyupgrader/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/pyupgrader/utilities/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/pyupgrader/utilities/file_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20745 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/pyupgrader/utilities/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/pyupgrader/utilities/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:23:22.477376 pyupgrader-2.5.16b2/pyupgrader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-07 00:23:22.000000 pyupgrader-2.5.16b2/pyupgrader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-07 00:23:22.000000 pyupgrader-2.5.16b2/pyupgrader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 00:23:22.000000 pyupgrader-2.5.16b2/pyupgrader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 00:23:22.000000 pyupgrader-2.5.16b2/pyupgrader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 00:23:22.000000 pyupgrader-2.5.16b2/pyupgrader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 00:23:22.000000 pyupgrader-2.5.16b2/pyupgrader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 00:23:22.477376 pyupgrader-2.5.16b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:23:22.477376 pyupgrader-2.5.16b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/tests/test_file_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-07 00:23:16.000000 pyupgrader-2.5.16b2/tests/test_main_cli.py
```

### Comparing `pyupgrader-2.5.13b2/LICENSE` & `pyupgrader-2.5.16b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyupgrader-2.5.13b2/PKG-INFO` & `pyupgrader-2.5.16b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyupgrader
-Version: 2.5.13b2
+Version: 2.5.16b2
 Summary: Keep your Python code up to date on client machines.
 Author: Noah Blaszak
 Author-email: technology.misc@gmail.com
 Project-URL: Homepage, https://pypi.org/project/pyupgrader
 Project-URL: Documentation, https://github.com/Trogiken/PyUpgrader/wiki
 Project-URL: Release Notes, https://github.com/Trogiken/PyUpgrader/wiki/Release-Notes
 Project-URL: Source, https://github.com/Trogiken/PyUpgrader
```

### Comparing `pyupgrader-2.5.13b2/README.md` & `pyupgrader-2.5.16b2/README.md`

 * *Files identical despite different names*

### Comparing `pyupgrader-2.5.13b2/pyupgrader/main_cli.py` & `pyupgrader-2.5.16b2/pyupgrader/main_cli.py`

 * *Files identical despite different names*

### Comparing `pyupgrader-2.5.13b2/pyupgrader/update.py` & `pyupgrader-2.5.16b2/pyupgrader/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 - GetFilesError: Raised when there is an error in retrieving file paths from the cloud.
 - DownloadFilesError: Raised when there is an error in downloading files from the cloud.
 - NoUpdateError: Raised when there is no files downloaded during an update.
 - URLNotValidError: Raised when the URL is not valid.
 """
 
 import os
+import sys
+import subprocess
 import tempfile
 import shutil
 import pickle
-import sys
 import logging
 import requests
 from packaging.version import Version
 from pyupgrader.utilities import helper, hashing
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.addHandler(logging.NullHandler())
@@ -153,14 +154,24 @@
             self._local_hash_db_path = None  # Set in _validate_attributes
             self._validate_attributes()
         except Exception as e:
             LOGGER.exception("Error occurred while setting project path")
             raise e
 
     @property
+    def pyupgrader_path(self) -> str:
+        """
+        Get the path to the .pyupgrader folder.
+
+        Returns:
+        - str: The path to the .pyupgrader folder.
+        """
+        return self._pyupgrader_path
+
+    @property
     def config_path(self) -> str:
         """
         Get the path to the config file.
 
         Returns:
         - str: The path to the config file.
         """
@@ -500,15 +511,16 @@
             return action_pkl
         except Exception as e:
             LOGGER.exception("Error occurred while preparing update")
             raise e
 
     def update(self, actions_path: str) -> None:
         """
-        Start the application update process. This function will replace the current process.
+        Start the application update process. This function will start a new process.
+        It is advised to unlink all file descriptors before calling this function.
 
         Args:
         - actions_path (str): The path to the actions file.
 
         Raises:
         - FileNotFoundError: If the actions file does not exist.
         """
@@ -519,15 +531,15 @@
 
             LOGGER.debug("Actions Path: '%s'", actions_path)
 
             updater_path = os.path.join(os.path.dirname(__file__), "utilities", "file_updater.py")
 
             LOGGER.debug("Updater Path: '%s'", updater_path)
 
-            args = ["-a", actions_path]
+            args = [sys.executable, updater_path, "-a", actions_path]
 
             LOGGER.debug("Args: '%s'", args)
 
-            os.execv(sys.executable, [sys.executable, updater_path] + args)
+            subprocess.run(args, check=True)
         except Exception as e:
             LOGGER.exception("Error occurred during update process")
             raise e
```

### Comparing `pyupgrader-2.5.13b2/pyupgrader/utilities/build.py` & `pyupgrader-2.5.16b2/pyupgrader/utilities/build.py`

 * *Files identical despite different names*

### Comparing `pyupgrader-2.5.13b2/pyupgrader/utilities/file_updater.py` & `pyupgrader-2.5.16b2/pyupgrader/utilities/file_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module is a utility for the update process."""
 
 import argparse
 import os
+import sys
+import subprocess
 import pickle
 import shutil
-import sys
 import datetime
 import logging
 from time import sleep
 
 dump_dir = os.path.join(os.path.dirname(__file__), "Update_Logs")
 os.makedirs(dump_dir, exist_ok=True)
 
@@ -245,18 +246,23 @@
 
     if cleanup:
         shutil.rmtree(downloads_dir)
         LOGGER.info("Cleaned up downloads directory at %s", downloads_dir)
     else:
         LOGGER.info("Downloads directory left at %s", downloads_dir)
 
-    LOGGER.info("Update completed successfully. Restarting application...")
+    LOGGER.info("Update completed successfully")
 
     # Start the application
-    os.execv(sys.executable, [sys.executable, startup_path])
+    if os.path.exists(startup_path):
+        LOGGER.info("Starting application...")
+        args = [sys.executable, startup_path]
+        subprocess.run(args, check=True)
+    else:
+        LOGGER.warning("Startup path not found at %s", startup_path)
 
 
 if __name__ == "__main__":
     try:
         main()
     except Exception as e:
         LOGGER.exception("Update failed")
```

### Comparing `pyupgrader-2.5.13b2/pyupgrader/utilities/hashing.py` & `pyupgrader-2.5.16b2/pyupgrader/utilities/hashing.py`

 * *Files identical despite different names*

### Comparing `pyupgrader-2.5.13b2/pyupgrader/utilities/helper.py` & `pyupgrader-2.5.16b2/pyupgrader/utilities/helper.py`

 * *Files identical despite different names*

### Comparing `pyupgrader-2.5.13b2/pyupgrader.egg-info/PKG-INFO` & `pyupgrader-2.5.16b2/pyupgrader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyupgrader
-Version: 2.5.13b2
+Version: 2.5.16b2
 Summary: Keep your Python code up to date on client machines.
 Author: Noah Blaszak
 Author-email: technology.misc@gmail.com
 Project-URL: Homepage, https://pypi.org/project/pyupgrader
 Project-URL: Documentation, https://github.com/Trogiken/PyUpgrader/wiki
 Project-URL: Release Notes, https://github.com/Trogiken/PyUpgrader/wiki/Release-Notes
 Project-URL: Source, https://github.com/Trogiken/PyUpgrader
```

### Comparing `pyupgrader-2.5.13b2/pyupgrader.egg-info/SOURCES.txt` & `pyupgrader-2.5.16b2/pyupgrader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyupgrader-2.5.13b2/setup.py` & `pyupgrader-2.5.16b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', encoding="utf-8") as f:
     readme = f.read()
 
 
 setup(
     name='pyupgrader',
-    version='2.5.13b2',
+    version='2.5.16b2',
     author='Noah Blaszak',
     author_email='technology.misc@gmail.com',
     description='Keep your Python code up to date on client machines.',
     long_description=readme,
     long_description_content_type='text/markdown',
     project_urls={
         'Homepage': 'https://pypi.org/project/pyupgrader',
```

### Comparing `pyupgrader-2.5.13b2/tests/test_build.py` & `pyupgrader-2.5.16b2/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `pyupgrader-2.5.13b2/tests/test_file_updater.py` & `pyupgrader-2.5.16b2/tests/test_file_updater.py`

 * *Files identical despite different names*

### Comparing `pyupgrader-2.5.13b2/tests/test_hashing.py` & `pyupgrader-2.5.16b2/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `pyupgrader-2.5.13b2/tests/test_helper.py` & `pyupgrader-2.5.16b2/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pyupgrader-2.5.13b2/tests/test_main_cli.py` & `pyupgrader-2.5.16b2/tests/test_main_cli.py`

 * *Files identical despite different names*

