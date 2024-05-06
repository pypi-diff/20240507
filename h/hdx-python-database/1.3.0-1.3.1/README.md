# Comparing `tmp/hdx_python_database-1.3.0.tar.gz` & `tmp/hdx_python_database-1.3.1.tar.gz`

## Comparing `hdx_python_database-1.3.0.tar` & `hdx_python_database-1.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     1524 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/.config/coveragerc
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/.config/pytest.ini
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/documentation/.readthedocs.yaml
--rwxr-xr-x   0        0        0     5950 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/documentation/main.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/documentation/pydoc-markdown.yaml
--rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/src/hdx/database/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/src/hdx/database/_version.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/src/hdx/database/dburi.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/src/hdx/database/no_timezone.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/src/hdx/database/postgresql.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/src/hdx/database/utils.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/src/hdx/database/views.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/src/hdx/database/with_timezone.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/tests/fixtures/test.db
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/tests/hdx/database/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/tests/hdx/database/conftest.py
--rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/tests/hdx/database/dbtestdate.py
--rwxr-xr-x   0        0        0     5413 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/tests/hdx/database/test_database.py
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/tests/hdx/database/test_dburi.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/tests/hdx/database/test_postgresql.py
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/LICENSE
--rwxr-xr-x   0        0        0     1248 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/README.md
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 hdx_python_database-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     1129 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/.config/coveragerc
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/.config/pytest.ini
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0     7125 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/documentation/main.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0    10957 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/src/hdx/database/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/src/hdx/database/_version.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/src/hdx/database/dburi.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/src/hdx/database/no_timezone.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/src/hdx/database/postgresql.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/src/hdx/database/utils.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/src/hdx/database/views.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/src/hdx/database/with_timezone.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/tests/fixtures/test.db
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/tests/hdx/database/__init__.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/tests/hdx/database/conftest.py
+-rwxr-xr-x   0        0        0      768 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/tests/hdx/database/dbtestdate.py
+-rwxr-xr-x   0        0        0     5412 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/tests/hdx/database/test_database.py
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/tests/hdx/database/test_dburi.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/tests/hdx/database/test_postgresql.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/LICENSE
+-rwxr-xr-x   0        0        0     1154 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/README.md
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 hdx_python_database-1.3.1/PKG-INFO
```

### Comparing `hdx_python_database-1.3.0/CONTRIBUTING.md` & `hdx_python_database-1.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.3.0/.config/pre-commit-config.yaml` & `hdx_python_database-1.3.1/.config/pre-commit-config.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -4,22 +4,23 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.5.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-ast
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.14
+    rev: v0.4.2
     hooks:
       # Run the linter.
       - id: ruff
         args: [--config, .config/ruff.toml, --fix]
       # Run the formatter.
       - id: ruff-format
         args: [--config, .config/ruff.toml]
-  - repo: https://github.com/jazzband/pip-tools
-    rev: 7.3.0
+  - repo: https://github.com/astral-sh/uv-pre-commit
+    rev: 0.1.38
     hooks:
+      # Run the pip compile
       - id: pip-compile
         name: pip-compile requirements.txt
         files: pyproject.toml
-        args: [pyproject.toml, --resolver=backtracking, --all-extras, --upgrade, -q, -o, requirements.txt]
+        args: [ pyproject.toml, --resolver=backtracking, --all-extras, --upgrade, -q, -o, requirements.txt ]
```

### Comparing `hdx_python_database-1.3.0/.github/workflows/publish.yaml` & `hdx_python_database-1.3.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.3.0/.github/workflows/run-python-tests.yaml` & `hdx_python_database-1.3.1/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.3.0/documentation/main.md` & `hdx_python_database-1.3.1/documentation/main.md`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 
 The `wait_for_postgresql` function is only available if this library is
 installed with extra `postgresql`:
 
     pip install hdx-python-database[postgresql]
 
 ## Breaking changes
+From 1.3.1, Database class refactored. With returns Database not Session
+object and can accept a prepare function called before
+Base.metadata.create_all. get_session can be used to obtain the session.
+get_engine, get_reflected_classes, get_prepare_results methods added.
+build_view, build_views move into Database class and renamed prepare_view and
+prepare_views.
+
 From 1.2.8, the sshtunnel dependency is optional.
 
 From 1.2.7, default table names are no longer plural. The camel case class name
 is converted to snake case, for example `MyTable` becomes `my_table`.
 
 From 1.2.3, Base must be chosen from `hdx.database.no_timezone`
 (`db_has_tz=False`: the default) or `hdx.database.with_timezone`
@@ -47,16 +54,21 @@
 
 Versions from 1.0.6 no longer support Python 2.7.
 
 # Description of Utilities
 
 ## Database
 
+A fresh schema can be created using the function `recreate_schema`. Any
+existing schema with that name will be dropped eg.
+
+    Database.recreate_schema(engine, db_uri)
+
 Your SQLAlchemy database tables must inherit from `Base` in
-`hdx.database.no_timezone` or `hdx.database.with_timezone` eg. :
+`hdx.database.no_timezone` or `hdx.database.with_timezone` eg.
 
     from hdx.database.no_timezone import Base
     class MyTable(Base):
         my_col: Mapped[int] = mapped_column(Integer, ForeignKey(MyTable2.col2), primary_key=True)
 
 A default table name is set which can be overridden: it is the camel case class
 name to converted to snake case, for example `MyTable` becomes `my_table`.
@@ -66,32 +78,46 @@
 
     # Get SQLAlchemy session object given database parameters and
     # if needed SSH parameters. If database is PostgreSQL, will poll
     # till it is up.
     from hdx.database import Database
     with Database(database="db", host="1.2.3.4", username="user",
                   password="pass", dialect="dialect", driver="driver",
+
                   ssh_host="5.6.7.8", ssh_port=2222, ssh_username="sshuser",
                   ssh_private_key="path_to_key", db_has_tz=True,
-                  reflect=False) as session:
+                  reflect=True, prepare_fn=prepare_views) as database:
+        engine = database.get_engine()
+        session = database.get_session()
+        reflected_classes = database.get_reflected_classes()
+        views = database.get_prepare_results()
         session.query(...)
 
 `db_has_tz` which defaults to `False` indicates whether database datetime
 columns have timezones. If `db_has_tz` is `True`, use `Base` from
 `hdx.database.with_timezone`, otherwise use `Base` from
 `hdx.database.no_timezone`. If `db_has_tz` is `False`, conversion occurs
 between Python datetimes with timezones to timezoneless database columns.
 
 If `reflect` (which defaults to `False`) is `True`, classes will be reflected
 from an existing database and the reflected classes are returned in a variable
-`reflected_classes` in the returned Session object. Note that type annotation
+`reflected_classes` in the Database object. Note that type annotation
 maps don't work with reflection and hence `db_has_tz` will be ignored ie.
 there will be no conversion between Python datetimes with timezones to
 timezoneless database columns.
 
+There is an option to wipe and create an empty schema in the database by
+setting `recreate_schema` to `True` and setting a `schema_name` ("public" is
+the default).
+
+If a prepare function is supplied in prepare_fn, it will be executed before
+Base.metadata.create_all and the results of it returned in instance variable
+prepare_results.
+
+
 ## Connection URI
 
 There are functions to handle converting from connection URIs to parameters and
 vice-versa as well as a function to remove the driver string from a connection
 URI that contains both dialect and driver.
 
     # Extract dictionary of parameters from database connection URI
@@ -113,18 +139,17 @@
 
     db_uri_nd = remove_driver_from_uri(
         "postgresql+psycopg://myuser:mypass@myserver:1234/mydatabase"
     )
 
 ## Views
 
-The method to make views described [here](https://github.com/sqlalchemy/sqlalchemy/wiki/Views#sqlalchemy-14-20-version)
-is available in this library.
+The method to prepare views described [here](https://github.com/sqlalchemy/sqlalchemy/wiki/Views#sqlalchemy-14-20-version) is available in this library.
 
-This allows creating views like this:
+This allows preparing views like this:
 ```
 class DBOrgType(Base):
     __tablename__ = "org_type"
 
     code: Mapped[str] = mapped_column(String(32), primary_key=True)
     description: Mapped[str] = mapped_column(String(512), nullable=False)
 
@@ -140,19 +165,21 @@
 
 date_view_params = {
     "name": "date_view",
     "metadata": Base.metadata,
     "selectable": select(*DBTestDate.__table__.columns),
 }
 
-date_view = build_view(date_view_params)
+date_view = Database.prepare_view(date_view_params)
 
-date_view = build_views([date_view_params])[0]
+date_view = Database.prepare_views([date_view_params])[0]
 ```
 
+View preparation must be done before calling Base.metadata.create_all.
+
 ## PostgreSQL specific
 
 There is a PostgreSQL specific call that only returns when the PostgreSQL database
 is available:
 
     # Wait until PostgreSQL is up
     # Library should be installed with hdx-python-database[postgresql]
```

### Comparing `hdx_python_database-1.3.0/documentation/pydoc-markdown.yaml` & `hdx_python_database-1.3.1/documentation/pydoc-markdown.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     packages:
       - hdx.database
 renderer:
   type: mkdocs
   output_directory: docs
   mkdocs_config:
     site_name: HDX Python Database
-    theme: mkdocs
+    theme: material
     repo_url: "https://github.com/OCHA-DAP/hdx-python-database"
   markdown:
     source_linker:
       type: github
       repo: OCHA-DAP/hdx-python-database
   pages:
     - title: Home
```

### Comparing `hdx_python_database-1.3.0/src/hdx/database/dburi.py` & `hdx_python_database-1.3.1/src/hdx/database/dburi.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,16 @@
         dialect (str): Database dialect. Defaults to "postgresql".
         driver (Optional[str]): Database driver. Defaults to None (psycopg if postgresql or None)
         include_driver (bool): Whether to include driver in uri. Defaults to True.
 
     Returns:
         str: Connection URI
     """
+    if not database:
+        return ""
     strings = [dialect]
     if include_driver:
         if dialect == "postgresql" and driver is None:
             driver = "psycopg"
         if driver:
             strings.append(f"+{driver}")
     strings.append("://")
```

### Comparing `hdx_python_database-1.3.0/src/hdx/database/no_timezone.py` & `hdx_python_database-1.3.1/src/hdx/database/no_timezone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for database datetime columns without timezone"""
+
 from datetime import datetime, timezone
 from typing import Optional
 
 from sqlalchemy import DateTime, TypeDecorator
 from sqlalchemy.orm import DeclarativeBase, declared_attr
 
 from .utils import camel_to_snake_case
```

### Comparing `hdx_python_database-1.3.0/src/hdx/database/postgresql.py` & `hdx_python_database-1.3.1/src/hdx/database/postgresql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """PostgreSQL specific utilities"""
+
 import logging
 import time
 
 from .dburi import remove_driver_from_uri
 
 try:
     import psycopg
```

### Comparing `hdx_python_database-1.3.0/src/hdx/database/views.py` & `hdx_python_database-1.3.1/src/hdx/database/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
-Create a DB View.
+Prepare database views ins SQLAlchemy. Must be run before calling
+Base.metadata.create_all.
 
 Copied from:
 https://github.com/sqlalchemy/sqlalchemy/wiki/Views#sqlalchemy-14-20-version
 """
-from typing import Dict, List
 
 import sqlalchemy as sa
 from sqlalchemy import MetaData, Selectable, TableClause
 from sqlalchemy.ext import compiler
 from sqlalchemy.schema import DDLElement
 from sqlalchemy.sql import table
 
@@ -42,15 +42,15 @@
 
 
 def view_doesnt_exist(ddl, target, connection, **kw):
     return not view_exists(ddl, target, connection, **kw)
 
 
 def view(name: str, metadata: MetaData, selectable: Selectable) -> TableClause:
-    """Create SQLAlchemy view
+    """Prepare SQLAlchemy view. Must be run before Base.metadata.create_all.
 
     Args:
         name (str): View name
         metadata (MetaData): Base metadata
         selectable (Selectable): SQLAlchemy select statement
 
     Returns:
@@ -69,35 +69,7 @@
     )
     sa.event.listen(
         metadata,
         "before_drop",
         DropView(name).execute_if(callable_=view_exists),
     )
     return t
-
-
-def build_view(view_params: Dict) -> TableClause:
-    """Create SQLAlchemy view from dictionary with keys: name, metadata and
-    selectable
-
-    Args:
-        view_params (Dict): Dictionary with keys name, metadata, selectable
-
-    Returns:
-        TableClause: SQLAlchemy View
-    """
-    return view(**view_params)
-
-
-def build_views(view_params_list: List[Dict]) -> List[TableClause]:
-    """Create SQLAlchemy views from a list of dictionaries with keys: name,
-    metadata and selectable
-
-    Args:
-        view_params_list (List[Dict]): List of dictionaries with view parameters
-    Returns:
-        List[TableClause]: SQLAlchemy Views
-    """
-    results = []
-    for view_params in view_params_list:
-        results.append(build_view(view_params))
-    return results
```

### Comparing `hdx_python_database-1.3.0/tests/fixtures/test.db` & `hdx_python_database-1.3.1/tests/fixtures/test.db`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.3.0/tests/hdx/database/dbtestdate.py` & `hdx_python_database-1.3.1/tests/hdx/database/dbtestdate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-"""SQLAlchemy class representing DBTestDate row. Holds test data for dates.
-"""
+"""SQLAlchemy class representing DBTestDate row. Holds test data for dates."""
+
 from datetime import datetime
 
 from sqlalchemy import select
 from sqlalchemy.orm import Mapped, mapped_column
 
 from hdx.database.no_timezone import Base
-from hdx.database.views import build_views
 
 
 class DBTestDate(Base):
     """
     test_date: Mapped[datetime] = mapped_column(primary_key=True)
     """
 
@@ -26,9 +25,7 @@
 
 
 date_view_params = {
     "name": "date_view",
     "metadata": Base.metadata,
     "selectable": select(*DBTestDate.__table__.columns),
 }
-
-date_view = build_views([date_view_params])[0]
```

### Comparing `hdx_python_database-1.3.0/tests/hdx/database/test_dburi.py` & `hdx_python_database-1.3.1/tests/hdx/database/test_dburi.py`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.3.0/.gitignore` & `hdx_python_database-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.3.0/LICENSE` & `hdx_python_database-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.3.0/README.md` & `hdx_python_database-1.3.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [![Build Status](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-database/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-database?branch=main)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Downloads](https://img.shields.io/pypi/dm/hdx-python-database.svg)](https://pypistats.org/packages/hdx-python-database)
 
 The HDX Python Database Library provides utilities for connecting to databases in a standard way including
 through an ssh tunnel if needed. It is built on top of SQLAlchemy and simplifies its setup.
 
 For more information, please read the [documentation](https://hdx-python-database.readthedocs.io/en/latest/).
```

### Comparing `hdx_python_database-1.3.0/pyproject.toml` & `hdx_python_database-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.3.0/PKG-INFO` & `hdx_python_database-1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hdx-python-database
-Version: 1.3.0
+Version: 1.3.1
 Summary: HDX Python database utilities
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-database
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,database,postgresql
 Classifier: Development Status :: 5 - Production/Stable
@@ -35,16 +35,15 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 [![Build Status](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-database/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-database?branch=main)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Downloads](https://img.shields.io/pypi/dm/hdx-python-database.svg)](https://pypistats.org/packages/hdx-python-database)
 
 The HDX Python Database Library provides utilities for connecting to databases in a standard way including
 through an ssh tunnel if needed. It is built on top of SQLAlchemy and simplifies its setup.
 
 For more information, please read the [documentation](https://hdx-python-database.readthedocs.io/en/latest/).
```

