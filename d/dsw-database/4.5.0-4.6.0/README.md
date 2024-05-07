# Comparing `tmp/dsw-database-4.5.0.tar.gz` & `tmp/dsw_database-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-database-4.5.0.tar", last modified: Tue Apr  2 10:28:59 2024, max compression
+gzip compressed data, was "dsw_database-4.6.0.tar", last modified: Tue May  7 07:12:51 2024, max compression
```

## Comparing `dsw-database-4.5.0.tar` & `dsw_database-4.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:59.916200 dsw-database-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-02 10:28:55.000000 dsw-database-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-02 10:28:59.916200 dsw-database-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-02 10:28:55.000000 dsw-database-4.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:59.912200 dsw-database-4.5.0/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:59.912200 dsw-database-4.5.0/dsw/database/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 10:28:55.000000 dsw-database-4.5.0/dsw/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 10:28:59.000000 dsw-database-4.5.0/dsw/database/build_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    22515 2024-04-02 10:28:55.000000 dsw-database-4.5.0/dsw/database/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    13055 2024-04-02 10:28:55.000000 dsw-database-4.5.0/dsw/database/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:28:59.916200 dsw-database-4.5.0/dsw_database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-02 10:28:59.000000 dsw-database-4.5.0/dsw_database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-02 10:28:59.000000 dsw-database-4.5.0/dsw_database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:28:59.000000 dsw-database-4.5.0/dsw_database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:28:59.000000 dsw-database-4.5.0/dsw_database.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 10:28:59.000000 dsw-database-4.5.0/dsw_database.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 10:28:59.000000 dsw-database-4.5.0/dsw_database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-02 10:28:55.000000 dsw-database-4.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:28:59.916200 dsw-database-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:28:55.000000 dsw-database-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:51.576674 dsw_database-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-07 07:12:46.000000 dsw_database-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-07 07:12:51.576674 dsw_database-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-07 07:12:46.000000 dsw_database-4.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:51.572674 dsw_database-4.6.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:51.576674 dsw_database-4.6.0/dsw/database/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 07:12:46.000000 dsw_database-4.6.0/dsw/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 07:12:51.000000 dsw_database-4.6.0/dsw/database/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22527 2024-05-07 07:12:46.000000 dsw_database-4.6.0/dsw/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13055 2024-05-07 07:12:46.000000 dsw_database-4.6.0/dsw/database/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:51.576674 dsw_database-4.6.0/dsw_database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-07 07:12:51.000000 dsw_database-4.6.0/dsw_database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-07 07:12:51.000000 dsw_database-4.6.0/dsw_database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:12:51.000000 dsw_database-4.6.0/dsw_database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:12:51.000000 dsw_database-4.6.0/dsw_database.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 07:12:51.000000 dsw_database-4.6.0/dsw_database.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 07:12:51.000000 dsw_database-4.6.0/dsw_database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-07 07:12:46.000000 dsw_database-4.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:12:51.576674 dsw_database-4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:12:46.000000 dsw_database-4.6.0/setup.py
```

### Comparing `dsw-database-4.5.0/LICENSE` & `dsw_database-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-database-4.5.0/PKG-INFO` & `dsw_database-4.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-database
-Version: 4.5.0
+Version: 4.6.0
 Summary: Library for managing DSW database
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,database
@@ -16,15 +16,15 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psycopg[binary]
 Requires-Dist: tenacity
-Requires-Dist: dsw-config==4.5.0
+Requires-Dist: dsw-config==4.6.0
 
 # Data Stewardship Wizard: Database
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-database)](https://pypi.org/project/dsw-database/)
 [![LICENSE](https://img.shields.io/github/license/ds-wizard/engine-tools)](LICENSE)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4975/badge)](https://bestpractices.coreinfrastructure.org/projects/4975)
```

### Comparing `dsw-database-4.5.0/README.md` & `dsw_database-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-database-4.5.0/dsw/database/database.py` & `dsw_database-4.6.0/dsw/database/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
         before=tenacity.before_log(LOG, logging.DEBUG),
         after=tenacity.after_log(LOG, logging.DEBUG),
     )
     def update_component_info(self, name: str, version: str, built_at: datetime.datetime):
         with self.conn_query.new_cursor(use_dict=True) as cursor:
             if not self._check_table_exists(table_name='component'):
                 return None
-            ts_now = datetime.datetime.utcnow()
+            ts_now = datetime.datetime.now(tz=datetime.UTC)
             try:
                 cursor.execute(
                     query=self.UPDATE_COMPONENT_INFO,
                     params={
                         'name': name,
                         'version': version,
                         'built_at': built_at,
```

### Comparing `dsw-database-4.5.0/dsw/database/model.py` & `dsw_database-4.6.0/dsw/database/model.py`

 * *Files identical despite different names*

### Comparing `dsw-database-4.5.0/dsw_database.egg-info/PKG-INFO` & `dsw_database-4.6.0/dsw_database.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-database
-Version: 4.5.0
+Version: 4.6.0
 Summary: Library for managing DSW database
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,database
@@ -16,15 +16,15 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psycopg[binary]
 Requires-Dist: tenacity
-Requires-Dist: dsw-config==4.5.0
+Requires-Dist: dsw-config==4.6.0
 
 # Data Stewardship Wizard: Database
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-database)](https://pypi.org/project/dsw-database/)
 [![LICENSE](https://img.shields.io/github/license/ds-wizard/engine-tools)](LICENSE)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4975/badge)](https://bestpractices.coreinfrastructure.org/projects/4975)
```

### Comparing `dsw-database-4.5.0/pyproject.toml` & `dsw_database-4.6.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-database'
-version = "4.5.0"
+version = "4.6.0"
 description = 'Library for managing DSW database'
 readme = 'README.md'
 keywords = ['dsw', 'database']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
@@ -22,15 +22,15 @@
     'Topic :: Utilities',
 ]
 requires-python = '>=3.10, <4'
 dependencies = [
     'psycopg[binary]',
     'tenacity',
     # DSW
-    "dsw-config==4.5.0",
+    "dsw-config==4.6.0",
 ]
 
 [project.urls]
 Homepage = 'https://ds-wizard.org'
 Repository = 'https://github.com/ds-wizard/engine-tools'
 Documentation = 'https://guide.ds-wizard.org'
```

