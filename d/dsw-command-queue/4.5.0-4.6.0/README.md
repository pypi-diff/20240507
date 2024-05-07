# Comparing `tmp/dsw-command-queue-4.5.0.tar.gz` & `tmp/dsw_command_queue-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-command-queue-4.5.0.tar", last modified: Tue Apr  2 10:28:57 2024, max compression
+gzip compressed data, was "dsw_command_queue-4.6.0.tar", last modified: Tue May  7 07:13:03 2024, max compression
```

## Comparing `dsw-command-queue-4.5.0.tar` & `dsw_command_queue-4.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:57.871791 dsw-command-queue-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-02 10:28:57.871791 dsw-command-queue-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:57.867790 dsw-command-queue-4.5.0/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:57.867790 dsw-command-queue-4.5.0/dsw/command_queue/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/dsw/command_queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw/command_queue/build_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/dsw/command_queue/command_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/dsw/command_queue/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:57.871791 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 10:28:57.000000 dsw-command-queue-4.5.0/dsw_command_queue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:28:57.871791 dsw-command-queue-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:28:53.000000 dsw-command-queue-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:13:03.596029 dsw_command_queue-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-07 07:12:52.000000 dsw_command_queue-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-07 07:13:03.596029 dsw_command_queue-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-07 07:12:52.000000 dsw_command_queue-4.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:13:03.592029 dsw_command_queue-4.6.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:13:03.596029 dsw_command_queue-4.6.0/dsw/command_queue/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 07:12:52.000000 dsw_command_queue-4.6.0/dsw/command_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 07:13:02.000000 dsw_command_queue-4.6.0/dsw/command_queue/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-05-07 07:12:52.000000 dsw_command_queue-4.6.0/dsw/command_queue/command_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-07 07:12:52.000000 dsw_command_queue-4.6.0/dsw/command_queue/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:13:03.596029 dsw_command_queue-4.6.0/dsw_command_queue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-07 07:13:03.000000 dsw_command_queue-4.6.0/dsw_command_queue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-07 07:13:03.000000 dsw_command_queue-4.6.0/dsw_command_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:13:03.000000 dsw_command_queue-4.6.0/dsw_command_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:13:03.000000 dsw_command_queue-4.6.0/dsw_command_queue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 07:13:03.000000 dsw_command_queue-4.6.0/dsw_command_queue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 07:13:03.000000 dsw_command_queue-4.6.0/dsw_command_queue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-07 07:12:52.000000 dsw_command_queue-4.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:13:03.596029 dsw_command_queue-4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:12:52.000000 dsw_command_queue-4.6.0/setup.py
```

### Comparing `dsw-command-queue-4.5.0/LICENSE` & `dsw_command_queue-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-command-queue-4.5.0/PKG-INFO` & `dsw_command_queue-4.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-command-queue
-Version: 4.5.0
+Version: 4.6.0
 Summary: Library for working with command queue and persistent commands
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,subscriber,publisher,database,queue,processing
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dsw-database==4.5.0
+Requires-Dist: dsw-database==4.6.0
 
 # Data Stewardship Wizard: Command Queue
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-command-queue)](https://pypi.org/project/dsw-command-queue/)
 [![LICENSE](https://img.shields.io/github/license/ds-wizard/engine-tools)](LICENSE)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4975/badge)](https://bestpractices.coreinfrastructure.org/projects/4975)
```

### Comparing `dsw-command-queue-4.5.0/README.md` & `dsw_command_queue-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-command-queue-4.5.0/dsw/command_queue/command_queue.py` & `dsw_command_queue-4.6.0/dsw/command_queue/command_queue.py`

 * *Files 18% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         LOG.debug('Trying to fetch a new job')
         return self.fetch_and_process()
 
     def fetch_and_process(self) -> bool:
         cursor = self.db.conn_query.new_cursor(use_dict=True)
         cursor.execute(
             query=self.queries.query_get_command(),
-            params={'now': datetime.datetime.utcnow()},
+            params={'now': datetime.datetime.now(tz=datetime.UTC)},
         )
         result = cursor.fetchall()
         if len(result) != 1:
             LOG.debug(f'Fetched {len(result)} persistent commands')
             return False
 
         command = PersistentCommand.from_dict_row(result[0])
@@ -144,26 +144,26 @@
 
         try:
             self.worker.work(command)
 
             self.db.execute_query(
                 query=self.queries.query_command_done(),
                 attempts=command.attempts + 1,
-                updated_at=datetime.datetime.utcnow(),
+                updated_at=datetime.datetime.now(tz=datetime.UTC),
                 uuid=command.uuid,
             )
         except Exception as e:
             msg = f'Failed with exception: {str(e)} ({type(e).__name__})'
             LOG.warning(msg)
             self.worker.process_exception(e)
             self.db.execute_query(
                 query=self.queries.query_command_error(),
                 attempts=command.attempts + 1,
                 error_message=msg,
-                updated_at=datetime.datetime.utcnow(),
+                updated_at=datetime.datetime.now(tz=datetime.UTC),
                 uuid=command.uuid,
             )
 
         LOG.debug('Committing transaction')
         self.db.conn_query.connection.commit()
         cursor.close()
         LOG.info('Notification processing finished')
```

### Comparing `dsw-command-queue-4.5.0/dsw/command_queue/query.py` & `dsw_command_queue-4.6.0/dsw/command_queue/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         return f"""
             SELECT *
             FROM persistent_command
             WHERE component = '{self.component}'
               AND attempts < max_attempts
               AND state != '{CommandState.DONE}'
               AND state != '{CommandState.IGNORE}'
-              AND updated_at < (%(now)s - ({exp} ^ attempts - 1) * INTERVAL '{interval}')
+              AND (updated_at AT TIME ZONE 'UTC') < (%(now)s - ({exp} ^ attempts - 1) * INTERVAL '{interval}')
             ORDER BY attempts ASC, updated_at DESC
             LIMIT 1 FOR UPDATE SKIP LOCKED;
         """
 
     @staticmethod
     def query_command_error() -> str:
         return f"""
```

### Comparing `dsw-command-queue-4.5.0/dsw_command_queue.egg-info/PKG-INFO` & `dsw_command_queue-4.6.0/dsw_command_queue.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-command-queue
-Version: 4.5.0
+Version: 4.6.0
 Summary: Library for working with command queue and persistent commands
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,subscriber,publisher,database,queue,processing
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dsw-database==4.5.0
+Requires-Dist: dsw-database==4.6.0
 
 # Data Stewardship Wizard: Command Queue
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-command-queue)](https://pypi.org/project/dsw-command-queue/)
 [![LICENSE](https://img.shields.io/github/license/ds-wizard/engine-tools)](LICENSE)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4975/badge)](https://bestpractices.coreinfrastructure.org/projects/4975)
```

### Comparing `dsw-command-queue-4.5.0/pyproject.toml` & `dsw_command_queue-4.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-command-queue'
-version = "4.5.0"
+version = "4.6.0"
 description = 'Library for working with command queue and persistent commands'
 readme = 'README.md'
 keywords = ['dsw', 'subscriber', 'publisher', 'database', 'queue', 'processing']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
@@ -21,15 +21,15 @@
     'Topic :: Database',
     'Topic :: Text Processing',
     'Topic :: Utilities',
 ]
 requires-python = '>=3.10, <4'
 dependencies = [
     # DSW
-    "dsw-database==4.5.0",
+    "dsw-database==4.6.0",
 ]
 
 [project.urls]
 Homepage = 'https://ds-wizard.org'
 Repository = 'https://github.com/ds-wizard/engine-tools'
 Documentation = 'https://guide.ds-wizard.org'
```

