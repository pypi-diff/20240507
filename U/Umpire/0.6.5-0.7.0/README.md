# Comparing `tmp/Umpire-0.6.5.tar.gz` & `tmp/umpire-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Volumes/vault/git/github/umpire/dist/tmpj5rjhvot/Umpire-0.6.5.tar", last modified: Mon Sep 20 16:53:19 2021, max compression
+gzip compressed data, was "umpire-0.7.0.tar", last modified: Tue May  7 13:17:59 2024, max compression
```

## Comparing `Umpire-0.6.5.tar` & `umpire-0.7.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)        0 2021-09-20 16:53:19.000000 Umpire-0.6.5/
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)     1081 2019-04-25 16:17:36.000000 Umpire-0.6.5/LICENSE
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)      279 2021-09-20 16:53:19.000000 Umpire-0.6.5/PKG-INFO
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)     3266 2021-06-02 14:40:13.000000 Umpire-0.6.5/README.md
-drwxr-xr-x   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)        0 2021-09-20 16:53:19.000000 Umpire-0.6.5/Umpire.egg-info/
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)      279 2021-09-20 16:53:19.000000 Umpire-0.6.5/Umpire.egg-info/PKG-INFO
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)      732 2021-09-20 16:53:19.000000 Umpire-0.6.5/Umpire.egg-info/SOURCES.txt
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)        1 2021-09-20 16:53:19.000000 Umpire-0.6.5/Umpire.egg-info/dependency_links.txt
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)       48 2021-09-20 16:53:19.000000 Umpire-0.6.5/Umpire.egg-info/entry_points.txt
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)       23 2021-09-20 16:53:19.000000 Umpire-0.6.5/Umpire.egg-info/requires.txt
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)        7 2021-09-20 16:53:19.000000 Umpire-0.6.5/Umpire.egg-info/top_level.txt
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)       38 2021-09-20 16:53:19.000000 Umpire-0.6.5/setup.cfg
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)      783 2021-09-20 16:52:57.000000 Umpire-0.6.5/setup.py
-drwxr-xr-x   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)        0 2021-09-20 16:53:19.000000 Umpire-0.6.5/umpire/
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)        0 2019-04-25 16:17:36.000000 Umpire-0.6.5/umpire/__init__.py
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)    14965 2021-06-02 14:40:13.000000 Umpire-0.6.5/umpire/cache.py
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)      703 2021-06-02 14:40:13.000000 Umpire-0.6.5/umpire/config.py
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)     9167 2021-09-20 16:52:57.000000 Umpire-0.6.5/umpire/deploy.py
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)     7919 2021-06-02 14:40:13.000000 Umpire-0.6.5/umpire/fetch.py
-drwxr-xr-x   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)        0 2021-09-20 16:53:19.000000 Umpire-0.6.5/umpire/test/
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)        0 2019-04-25 16:17:36.000000 Umpire-0.6.5/umpire/test/__init__.py
-drwxr-xr-x   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)        0 2021-09-20 16:53:19.000000 Umpire-0.6.5/umpire/test/deploy_tests/
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)        0 2019-04-25 16:17:36.000000 Umpire-0.6.5/umpire/test/deploy_tests/__init__.py
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)     2996 2021-06-02 14:40:13.000000 Umpire-0.6.5/umpire/test/deploy_tests/tc1_full_deploy.py
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)     2674 2021-06-02 14:40:13.000000 Umpire-0.6.5/umpire/test/deploy_tests/tc2_deploy_from_existing_cache.py
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)     2786 2021-06-02 14:40:13.000000 Umpire-0.6.5/umpire/test/deploy_tests/tc3_fresh_deploy_from_cleared_cache.py
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)     2682 2021-06-02 14:40:13.000000 Umpire-0.6.5/umpire/test/deploy_tests/tc4_existing_deploy_from_cleared_cache.py
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)     2047 2021-06-02 14:40:13.000000 Umpire-0.6.5/umpire/test/deploy_tests/tc5_no_extract_copy.py
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)     4696 2021-06-02 14:40:13.000000 Umpire-0.6.5/umpire/test/deploy_tests/tc6_keep_updated.py
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)     3969 2021-06-02 14:40:13.000000 Umpire-0.6.5/umpire/umpire.py
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)     1195 2019-04-25 16:17:36.000000 Umpire-0.6.5/umpire/unpack.py
--rw-r--r--   0 mperttula (1344554453) SIGNIANTOTT\Domain Users (1513040830)     1345 2021-06-02 14:40:13.000000 Umpire-0.6.5/umpire/update.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-07 13:17:59.481830 umpire-0.7.0/
+-rwx------   0 mperttula   (502) staff       (20)     1081 2019-04-25 16:17:36.000000 umpire-0.7.0/LICENSE
+-rw-r--r--   0 mperttula   (502) staff       (20)      310 2024-05-07 13:17:59.477768 umpire-0.7.0/PKG-INFO
+-rwxr-xr-x   0 mperttula   (502) staff       (20)     3267 2024-05-07 13:13:16.000000 umpire-0.7.0/README.md
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-07 13:17:59.476269 umpire-0.7.0/Umpire.egg-info/
+-rw-r--r--   0 mperttula   (502) staff       (20)      310 2024-05-07 13:17:59.000000 umpire-0.7.0/Umpire.egg-info/PKG-INFO
+-rw-r--r--   0 mperttula   (502) staff       (20)      732 2024-05-07 13:17:59.000000 umpire-0.7.0/Umpire.egg-info/SOURCES.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)        1 2024-05-07 13:17:59.000000 umpire-0.7.0/Umpire.egg-info/dependency_links.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)       47 2024-05-07 13:17:59.000000 umpire-0.7.0/Umpire.egg-info/entry_points.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)       29 2024-05-07 13:17:59.000000 umpire-0.7.0/Umpire.egg-info/requires.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)        7 2024-05-07 13:17:59.000000 umpire-0.7.0/Umpire.egg-info/top_level.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)       38 2024-05-07 13:17:59.482244 umpire-0.7.0/setup.cfg
+-rwxr-xr-x   0 mperttula   (502) staff       (20)      820 2024-05-07 13:13:16.000000 umpire-0.7.0/setup.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-07 13:17:59.374060 umpire-0.7.0/umpire/
+-rwx------   0 mperttula   (502) staff       (20)        0 2019-04-25 16:17:36.000000 umpire-0.7.0/umpire/__init__.py
+-rwxr-xr-x   0 mperttula   (502) staff       (20)    15314 2024-05-07 13:13:16.000000 umpire-0.7.0/umpire/cache.py
+-rwx------   0 mperttula   (502) staff       (20)      703 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/config.py
+-rwxr-xr-x   0 mperttula   (502) staff       (20)    12568 2024-05-07 13:13:16.000000 umpire-0.7.0/umpire/deploy.py
+-rwxr-xr-x   0 mperttula   (502) staff       (20)     8459 2024-05-07 13:13:16.000000 umpire-0.7.0/umpire/fetch.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-07 13:17:59.376355 umpire-0.7.0/umpire/test/
+-rwx------   0 mperttula   (502) staff       (20)        0 2019-04-25 16:17:36.000000 umpire-0.7.0/umpire/test/__init__.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-07 13:17:59.475080 umpire-0.7.0/umpire/test/deploy_tests/
+-rwx------   0 mperttula   (502) staff       (20)        0 2019-04-25 16:17:36.000000 umpire-0.7.0/umpire/test/deploy_tests/__init__.py
+-rwx------   0 mperttula   (502) staff       (20)     2996 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/test/deploy_tests/tc1_full_deploy.py
+-rwx------   0 mperttula   (502) staff       (20)     2674 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/test/deploy_tests/tc2_deploy_from_existing_cache.py
+-rwx------   0 mperttula   (502) staff       (20)     2786 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/test/deploy_tests/tc3_fresh_deploy_from_cleared_cache.py
+-rwx------   0 mperttula   (502) staff       (20)     2682 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/test/deploy_tests/tc4_existing_deploy_from_cleared_cache.py
+-rwx------   0 mperttula   (502) staff       (20)     2047 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/test/deploy_tests/tc5_no_extract_copy.py
+-rwx------   0 mperttula   (502) staff       (20)     4696 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/test/deploy_tests/tc6_keep_updated.py
+-rwxr-xr-x   0 mperttula   (502) staff       (20)     5285 2024-05-07 13:13:16.000000 umpire-0.7.0/umpire/umpire.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     1812 2024-05-07 13:13:16.000000 umpire-0.7.0/umpire/unpack.py
+-rwxr-xr-x   0 mperttula   (502) staff       (20)     1436 2024-05-07 13:13:16.000000 umpire-0.7.0/umpire/update.py
```

### Comparing `Umpire-0.6.5/LICENSE` & `umpire-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Umpire-0.6.5/README.md` & `umpire-0.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Umpire was developed as an easy to install command line tool, with it's flexibility being derived from the JSON file options.
 
 Umpire reads a JSON file to retrieve, cache, and link files to their appropriate destination from an Amazon S3 backed repository of compressed packages.
 
 ## Installation
 
-Umpire requires **Python 3.7.1 or above**
+Umpire requires **Python 3.11.6 or above**
 
 Umpire is available as a [pip package](https://pypi.python.org/pypi/pip).
 
 To install Umpire:
 
 1. Download `get-pip.py` from [PyPA](https://pypa.io).
```

### Comparing `Umpire-0.6.5/Umpire.egg-info/SOURCES.txt` & `umpire-0.7.0/Umpire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Umpire-0.6.5/setup.py` & `umpire-0.7.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,23 +3,26 @@
 
 from os import path
 # this_directory = path.abspath(path.dirname(__file__))
 # with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
 #     long_description = f.read()
 
 setup(name='Umpire',
-      version='0.6.5',
+      version='0.7.0',
       description='Generic dependency resolver.',
       long_description='',
       long_description_content_type='text/markdown',
       author='Signiant SRE',
       author_email='sre@signiant.com',
       url='https://www.signiant.com',
       packages=find_packages(),
       license='MIT',
-      install_requires=['MaestroOps>=0.8.8,<0.9'],
+      install_requires=[
+          'MaestroOps>=0.9',
+          'tqdm>=4.64.1'
+      ],
       entry_points = {
           'console_scripts': [
               'umpire = umpire.umpire:entry'
               ]
           }
      )
```

### Comparing `Umpire-0.6.5/umpire/cache.py` & `umpire-0.7.0/umpire/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import configparser
 import maestro.tools.path
 import maestro.tools.file
 import maestro.core.module
 from . import unpack
 from maestro.tools.os_tools import check_pid
 from . import config
+import logging, sys
+logger = logging.getLogger(__name__)
 
 # Cache constants
 CONFIG_FILENAME = config.CONFIG_FILENAME
 CONFIG_REPO_SECTION_NAME = config.CONFIG_REPO_SECTION_NAME
 CONFIG_ENTRY_SECTION_NAME = config.CONFIG_ENTRY_SECTION_NAME
 LOCK_FILENAME = config.LOCK_FILENAME
 CURRENT_ENTRY_CONFIG_VERSION = config.CURRENT_ENTRY_CONFIG_VERSION
@@ -135,14 +137,15 @@
         entry.md5 = None
 
     return entry
 
 def write_entry(entry):
 
         ## Start creating config
+        logging.debug("Creating entry")
         config = configparser.SafeConfigParser()
         config_path = os.path.join(entry.path, CONFIG_FILENAME)
         config.add_section(CONFIG_ENTRY_SECTION_NAME)
 
         config.set(CONFIG_ENTRY_SECTION_NAME, "name", entry.name)
         config.set(CONFIG_ENTRY_SECTION_NAME, "platform", entry.platform)
         config.set(CONFIG_ENTRY_SECTION_NAME, "version", entry.version)
@@ -181,23 +184,30 @@
     config_version = None
     host_id = None
 
     #Lock timeout in seconds
     lock_timeout = None
 
     #Verifies local existance
-    def __init__(self, cache_root, lock_timeout = 1800, host_id="localhost"):
+    def __init__(self, cache_root, lock_timeout = 1800, host_id="localhost", log_level=logging.INFO):
         if not os.path.exists(cache_root):
             raise CacheError("The path '" + str(cache_root) + "' does not contain a valid umpire cache.")
 
         self.local_path = cache_root
         self.lock_timeout = lock_timeout
         self.host_id = host_id
         self.settings_file = os.path.join(cache_root,CONFIG_FILENAME)
 
+        #set logging
+        logger = logging
+        FORMAT = '%(asctime)s - %(levelname)s - %(message)s'
+        logger.basicConfig(format=FORMAT, stream=sys.stdout, level=log_level)
+
+        logging.debug("Running Caching")
+
         if not os.path.exists(self.settings_file):
             raise CacheError("The path '" + str(cache_root) + "' does not appear to be a valid umpire cache")
         config = None
 
         #Get parser
         parser = configparser.SafeConfigParser()
         try:#Read
```

### Comparing `Umpire-0.6.5/umpire/config.py` & `umpire-0.7.0/umpire/config.py`

 * *Files identical despite different names*

### Comparing `Umpire-0.6.5/umpire/fetch.py` & `umpire-0.7.0/umpire/fetch.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """fetch.py"""
 
 import sys, os, urllib, time, traceback
 from . import cache, config
-# from cache import LocalCache
-# from config import default_host_id
 from multiprocessing import Value
 from maestro.core import module
 from maestro.aws import s3
 from maestro.tools import file as mfile
+import logging
+logger = logging.getLogger(__name__)
 
 CACHE_LOCATION_KEYS = ["c", "cache-location"]
 DEPENDENCY_NAME_KEYS = ["n", "name"]
 DEPENDENCY_PLATFORM_KEYS = ["p", "platform"]
 DEPENDENCY_REPOSITORY_KEYS = ["r", "repository"]
 DEPENDENCY_VERSION_KEYS = ["v", "version"]
 HELP_KEYS = ["h", "help"]
@@ -53,99 +53,106 @@
 
     #Is the dependency going to be extracted after the download
     dependency_unpack = None
 
     #Are we going to check if this dependency has changed in the remote?
     keep_updated = None
 
-    def run(self,kwargs):
+    log_level=None
 
+    def run(self,kwargs):
+        logger = logging
+        FORMAT = '%(asctime)s - %(levelname)s - %(message)s'
+        logger.basicConfig(format=FORMAT, stream=sys.stdout, level=self.log_level)
+        logger.debug("Running Fetch")
         #Verify argument validity
         self.__verify_arguments__()
 
         #Get cache name from remote url
         cache_name = self.get_cache_name()
 
         #Get cache path
         cache_path = os.path.join(self.cache_root, cache_name)
 
-        #Get cache object (will raise an exception if it doesn't exist)
-        cache_obj = cache.LocalCache(cache_path, host_id=config.default_host_id)
+        logger.debug(f"Cache path: {cache_path}")
 
-        cache_obj.DEBUG = self.DEBUG
+        #Get cache object (will raise an exception if it doesn't exist)
+        cache_obj = cache.LocalCache(cache_path, host_id=config.default_host_id, log_level=self.log_level)
 
         full_url = s3.join_s3_url(self.dependency_repo, self.dependency_platform, self.dependency_name, self.dependency_version)
 
         cache_obj.lock(os.path.join(cache_path,self.dependency_platform, self.dependency_name, self.dependency_version))
         #Try to get entry from cache
         entry = cache_obj.get(self.dependency_platform, self.dependency_name, self.dependency_version)
 
         #Set state
         if entry is None:
             state = EntryState.DOWNLOADED
         else:
             state = EntryState.CACHE
 
-        #Verify Remote MD5
+        #Verify Remote sha256 if updating
         if self.keep_updated and state == EntryState.CACHE:
-            #TODO: Kinda hacky, but the maestro underlying code needs some refactoring. This will do what I want without changing it
             bucket,prefix = s3.parse_s3_url(full_url)
             checksums = list()
             try:
-                for file in s3.find_files(bucket,prefix,anonymous=False):
+                for file in s3.find_files(bucket, prefix, anonymous=False, sha256=True ):
                     checksums.append(file[1])
             except:
-                if self.DEBUG:
-                    traceback.print_exc()
-                for file in s3.find_files(bucket,prefix,anonymous=True):
+                logger.debug(f"{traceback.print_exc()}")
+                for file in s3.find_files(bucket, prefix, anonymous=True, sha256=True ):
                     checksums.append(file[1])
 
             if entry.md5 not in checksums:
                 state = EntryState.UPDATED
 
         #We need to download the file, it wasn't in the cache
         if state == EntryState.DOWNLOADED or state == EntryState.UPDATED:
 
             if state == EntryState.DOWNLOADED:
-                print (self.format_entry_name() + ": Not in cache")
+                logger.info(self.format_entry_name() + ": Not in cache")
             else:
-                print (self.format_entry_name() + ": Cache is obsolete")
+                logger.info(self.format_entry_name() + ": Cache is obsolete")
 
-            print (self.format_entry_name() + ": Downloading " + full_url)
+            logger.info(self.format_entry_name() + ": Downloading " + full_url)
 
             #Get Downloader
             downloader = s3.AsyncS3Downloader(None)
 
             #Set Downloader arguments
             downloader.source_url = full_url+"/"
+            downloader.sha256 = True
             downloader.destination_path = os.path.join(self.cache_root, "downloading") + os.sep
             downloader.start()
 
             #Wait for downloader to finish #TODO: Do something with the reported progress
-            while downloader.status != module.DONE:
+            while downloader.status != 2:
                 time.sleep(0.5)
 
             #Check for an exception, if so bubble it up
             if downloader.exception is not None:
-                raise downloader.exception
-
-            print(self.format_entry_name() + ": Download complete")
-            print(downloader.result)
+                logger.error(f"Exception!!! {downloader.exception}")
+                # raise downloader.exception
+                sys.exit(1)
+            logger.info(self.format_entry_name() + ": Download complete")
+            logger.debug(f"Result: {downloader.result}")
             if downloader.result is None or len(downloader.result) == 0:
                 raise EntryError(self.format_entry_name() + ": Unable to find remote entry '" + full_url + "'")
 
             #Iterate of the result (downloaded files)
             for item, checksum in downloader.result:
-                local_file_checksum = mfile.md5_checksum(item)
+                local_file_checksum = mfile.sha256_checksum(item, checksum)
+                logging.debug(f"sha 256 checksum local_file: {local_file_checksum} remote: {checksum}")
                 if checksum != local_file_checksum:
-                    print(self.format_entry_name() + ": WARNING: Downloaded file does not match the checksum on the server")
-                    print(self.format_entry_name() + ": WARNING: local:\t" + str(local_file_checksum))
-                    print(self.format_entry_name() + ": WARNING: server:\t" + str(checksum))
+                    logger.warning(self.format_entry_name() + ": WARNING: Downloaded file does not match the checksum on the server")
+                    logger.warning(self.format_entry_name() + ": WARNING: local:\t" + str(local_file_checksum))
+                    logger.warning(self.format_entry_name() + ": WARNING: server:\t" + str(checksum))
                 if self.dependency_unpack:
-                    print (self.format_entry_name() + ": Unpacking...")
+                    print(self.format_entry_name() + ": Unpacking...")
+                    logger.info (self.format_entry_name() + ": Unpacking...")
                 #Put will unlock
                 cache_obj.put(item,self.dependency_platform, self.dependency_name, self.dependency_version, unpack_bol=self.dependency_unpack, checksum=checksum)
             entry = cache_obj.get(self.dependency_platform, self.dependency_name, self.dependency_version)
             if entry is None:
                 raise EntryError(self.format_entry_name() + ": Error retrieving entry from cache.")
         cache_obj.unlock(os.path.join(cache_path,self.dependency_platform, self.dependency_name, self.dependency_version))
         #Entry is not None, return all the files listed in the entry that aren't the configuration files
@@ -166,15 +173,15 @@
             raise ValueError("You must specify a valid version for the dependency.")
         if not self.dependency_is_link:
             # Not used
             pass
         if not self.keep_updated:
             self.keep_updated = False
         if not isinstance(self.dependency_unpack,bool):
-            print(str(self.dependency_unpack))
+            logger.info(str(self.dependency_unpack))
             raise ValueError("You must specify whether the dependency should be unpacked or not")
 
     def get_cache_name(self):
         try:
             bucket, prefix = s3.parse_s3_url(self.dependency_repo)
             return bucket + ".s3"
         except ValueError:
```

### Comparing `Umpire-0.6.5/umpire/test/deploy_tests/tc1_full_deploy.py` & `umpire-0.7.0/umpire/test/deploy_tests/tc1_full_deploy.py`

 * *Files identical despite different names*

### Comparing `Umpire-0.6.5/umpire/test/deploy_tests/tc2_deploy_from_existing_cache.py` & `umpire-0.7.0/umpire/test/deploy_tests/tc2_deploy_from_existing_cache.py`

 * *Files identical despite different names*

### Comparing `Umpire-0.6.5/umpire/test/deploy_tests/tc3_fresh_deploy_from_cleared_cache.py` & `umpire-0.7.0/umpire/test/deploy_tests/tc3_fresh_deploy_from_cleared_cache.py`

 * *Files identical despite different names*

### Comparing `Umpire-0.6.5/umpire/test/deploy_tests/tc4_existing_deploy_from_cleared_cache.py` & `umpire-0.7.0/umpire/test/deploy_tests/tc4_existing_deploy_from_cleared_cache.py`

 * *Files identical despite different names*

### Comparing `Umpire-0.6.5/umpire/test/deploy_tests/tc5_no_extract_copy.py` & `umpire-0.7.0/umpire/test/deploy_tests/tc5_no_extract_copy.py`

 * *Files identical despite different names*

### Comparing `Umpire-0.6.5/umpire/test/deploy_tests/tc6_keep_updated.py` & `umpire-0.7.0/umpire/test/deploy_tests/tc6_keep_updated.py`

 * *Files identical despite different names*

### Comparing `Umpire-0.6.5/umpire/update.py` & `umpire-0.7.0/umpire/update.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import urllib.request, urllib.error, urllib.parse
 import sys
 
 from .umpire import __version__
 from . import config
 import umpire, os
 from maestro.core import module
+import logging
 
 HELP_KEYS = ["h", "help"]
 UPDATE_KEYS = ["u", "update"]
+logger = logging.getLogger(__name__)
 
 def parse_version_string(version):
     """
     Returns a tuple containing the major, minor, revision integers
     """
     nums = version.split(".")
     return int(nums[0]), int(nums[1]), int(nums[2])
@@ -38,13 +40,14 @@
         with open(os.path.join(umpire.get_umpire_root(),"remote_version"), "w+") as f:
             f.write(version)
 
     def get_remote_version(self):
         return urllib.request.urlopen(config.REMOTE_VERSION_URL).read()
 
     def run(self,kwargs):
+        logger.debug("Running update")
         version = self.get_remote_version()
         self.write_remote_version(version)
         for key in UPDATE_KEYS:
             if key in list(kwargs.keys()):
                 __run_pip__()
                 __restart_umpire__()
```

