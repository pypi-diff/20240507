# Comparing `tmp/crud_repository-0.1.6.tar.gz` & `tmp/crud_repository-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crud_repository-0.1.6.tar", last modified: Tue Apr 30 20:56:40 2024, max compression
+gzip compressed data, was "crud_repository-0.1.7.tar", last modified: Tue May  7 10:24:04 2024, max compression
```

## Comparing `crud_repository-0.1.6.tar` & `crud_repository-0.1.7.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:40.836965 crud_repository-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 20:56:33.000000 crud_repository-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-30 20:56:33.000000 crud_repository-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-30 20:56:40.836965 crud_repository-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-30 20:56:33.000000 crud_repository-0.1.6/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-04-30 20:56:33.000000 crud_repository-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:40.836965 crud_repository-0.1.6/crud_repository.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-30 20:56:40.000000 crud_repository-0.1.6/crud_repository.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-30 20:56:40.000000 crud_repository-0.1.6/crud_repository.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:56:40.000000 crud_repository-0.1.6/crud_repository.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:56:40.000000 crud_repository-0.1.6/crud_repository.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-30 20:56:40.000000 crud_repository-0.1.6/crud_repository.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-30 20:56:40.000000 crud_repository-0.1.6/crud_repository.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-30 20:56:39.000000 crud_repository-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 20:56:40.836965 crud_repository-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-30 20:56:33.000000 crud_repository-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:40.832965 crud_repository-0.1.6/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/__config__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:40.836965 crud_repository-0.1.6/src/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/db/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/db/idatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:40.836965 crud_repository-0.1.6/src/db/mariadb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/db/mariadb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/db/mariadb/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:40.836965 crud_repository-0.1.6/src/db/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/db/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/db/mysql/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:40.836965 crud_repository-0.1.6/src/db/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/db/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/db/postgres/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:40.836965 crud_repository-0.1.6/src/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:40.836965 crud_repository-0.1.6/src/my_logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/my_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/my_logger/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/my_logger/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/my_logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/my_logger/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:40.836965 crud_repository-0.1.6/src/repo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-30 20:56:33.000000 crud_repository-0.1.6/src/repo/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:24:04.019290 crud_repository-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 10:23:56.000000 crud_repository-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-07 10:23:56.000000 crud_repository-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-07 10:24:04.019290 crud_repository-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-07 10:23:56.000000 crud_repository-0.1.7/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15987 2024-05-07 10:23:56.000000 crud_repository-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:24:04.015290 crud_repository-0.1.7/crud_repository/
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/__config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:24:04.015290 crud_repository-0.1.7/crud_repository/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/db/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/db/idatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:24:04.015290 crud_repository-0.1.7/crud_repository/db/mariadb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/db/mariadb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/db/mariadb/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:24:04.015290 crud_repository-0.1.7/crud_repository/db/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/db/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/db/mysql/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:24:04.015290 crud_repository-0.1.7/crud_repository/db/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/db/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/db/postgres/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:24:04.015290 crud_repository-0.1.7/crud_repository/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:24:04.019290 crud_repository-0.1.7/crud_repository/my_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/my_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/my_logger/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/my_logger/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/my_logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/my_logger/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:24:04.019290 crud_repository-0.1.7/crud_repository/repo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/repo/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:24:04.019290 crud_repository-0.1.7/crud_repository/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 10:23:56.000000 crud_repository-0.1.7/crud_repository/utils/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:24:04.019290 crud_repository-0.1.7/crud_repository.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-07 10:24:04.000000 crud_repository-0.1.7/crud_repository.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-07 10:24:04.000000 crud_repository-0.1.7/crud_repository.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 10:24:04.000000 crud_repository-0.1.7/crud_repository.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 10:24:03.000000 crud_repository-0.1.7/crud_repository.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 10:24:04.000000 crud_repository-0.1.7/crud_repository.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 10:24:04.000000 crud_repository-0.1.7/crud_repository.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-07 10:24:02.000000 crud_repository-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 10:24:04.019290 crud_repository-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 10:23:56.000000 crud_repository-0.1.7/setup.py
```

### Comparing `crud_repository-0.1.6/LICENSE` & `crud_repository-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.6/PKG-INFO` & `crud_repository-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.1.6
+Version: 0.1.7
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
         
@@ -92,21 +92,21 @@
 ```
 
 ## Code Example Usage
 
 ```python
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from src.db.factory import DatabaseFactory
+from crud_repository.db.factory import DatabaseFactory
 from typing import Optional
 from sqlalchemy import Column, Sequence, Integer, String
 from sqlalchemy.orm import Mapped
-from src.model.base import Base
+from crud_repository.model.base import Base
 from db.idatabase import IDatabase
-from src.repo.repository import Repository
+from crud_repository.repo.repository import Repository
 
 
 # ---------------------------------------------------------
 # Create a User model
 # ---------------------------------------------------------
 class User(Base):
     __tablename__ = "user"
```

### Comparing `crud_repository-0.1.6/PYPI.md` & `crud_repository-0.1.7/PYPI.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,21 +43,21 @@
 ```
 
 ## Code Example Usage
 
 ```python
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from src.db.factory import DatabaseFactory
+from crud_repository.db.factory import DatabaseFactory
 from typing import Optional
 from sqlalchemy import Column, Sequence, Integer, String
 from sqlalchemy.orm import Mapped
-from src.model.base import Base
+from crud_repository.model.base import Base
 from db.idatabase import IDatabase
-from src.repo.repository import Repository
+from crud_repository.repo.repository import Repository
 
 
 # ---------------------------------------------------------
 # Create a User model
 # ---------------------------------------------------------
 class User(Base):
     __tablename__ = "user"
```

### Comparing `crud_repository-0.1.6/crud_repository.egg-info/PKG-INFO` & `crud_repository-0.1.7/crud_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.1.6
+Version: 0.1.7
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
         
@@ -92,21 +92,21 @@
 ```
 
 ## Code Example Usage
 
 ```python
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from src.db.factory import DatabaseFactory
+from crud_repository.db.factory import DatabaseFactory
 from typing import Optional
 from sqlalchemy import Column, Sequence, Integer, String
 from sqlalchemy.orm import Mapped
-from src.model.base import Base
+from crud_repository.model.base import Base
 from db.idatabase import IDatabase
-from src.repo.repository import Repository
+from crud_repository.repo.repository import Repository
 
 
 # ---------------------------------------------------------
 # Create a User model
 # ---------------------------------------------------------
 class User(Base):
     __tablename__ = "user"
```

### Comparing `crud_repository-0.1.6/pyproject.toml` & `crud_repository-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crud_repository"
-version = "0.1.6"
+version = "0.1.7"
 description = "The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases."
 authors = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"},
   {email = "info@hyfisolutions.com"},
 ]
 maintainers = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"}
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 license = {file = "LICENSE", content-type = "text/plain"}
 
 
-# Update the 'include' directive to include the "src" directory
+# Update the 'include' directive to include the "crud_repository" directory
 
 dependencies = [
     "sqlalchemy>=2.0.29",
     "psycopg2-binary>=2.9.9",
     "python-dotenv>=1.0.1",
     "colorlog>=6.4.1",
     "cryptography>=42.0.5",
```

### Comparing `crud_repository-0.1.6/setup.py` & `crud_repository-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,11 +12,11 @@
     author_email="dalexander@hyfisolutions.com",
     description="The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.",
     packages=find_packages(
         exclude=["tests", "*.tests", "*.tests.*", "tests.*", "dist", "build", "logs"]
     ),
     long_description=Path("README.md").read_text(encoding="utf-8"),
     package_dir={
-        "crud_repository": "src"
+        "crud_repository": "crud_repository"
     },
 )
```

### Comparing `crud_repository-0.1.6/src/__config__.py` & `crud_repository-0.1.7/crud_repository/__config__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,20 +18,20 @@
             raise_error_if_not_found=True,
             usecwd=True,
         )
     )
 
 # --------------------------------------------------------------
 # Load and setup environment variables
-ROOT_DIR = os.path.dirname(os.path.abspath(__file__))  # ~/CRUDRepository/src
+ROOT_DIR = os.path.dirname(os.path.abspath(__file__))  # ~/CRUDRepository/crud_repository
 # --------------------------------------------------------------
-DATA_DIR = os.path.join(ROOT_DIR, "data")  # ~/CRUDRepository/src/data
+DATA_DIR = os.path.join(ROOT_DIR, "data")  # ~/CRUDRepository/crud_repository/data
 LOG_LEVEL = os.getenv("LOG_LEVEL", "DEBUG")
 LOG_FILE = f'{ROOT_DIR}/logs/crud_{time.strftime("%Y%m%d%H%M%S")}.log'
-LOG_DIR = os.path.join(ROOT_DIR, "logs")  # ~/CRUDRepository/src/logs
+LOG_DIR = os.path.join(ROOT_DIR, "logs")  # ~/CRUDRepository/crud_repository/logs
 # --------------------------------------------------------------
 # Set environment variables
 os.environ.setdefault("ROOT_DIR", ROOT_DIR)
 os.environ.setdefault("LOG_FILE", LOG_FILE)
 os.environ.setdefault("LOG_LEVEL", LOG_LEVEL)
 os.environ.setdefault("LOG_DIR", LOG_DIR)
 print(json.dumps(dotenv_values(), indent=2, sort_keys=True))
@@ -67,15 +67,15 @@
     "handlers": {
         "console": {
             "class": "logging.StreamHandler",
             "level": "DEBUG",
             "formatter": "colored",
         },
         "file_handler": {
-            "class": "src.my_logger.handlers.CustomTimedRotatingFileHandler",
+            "class": "crud_repository.my_logger.handlers.CustomTimedRotatingFileHandler",
             "filename": f"{LOG_FILE}",
             "when": "midnight",
             "interval": 1,
             "backup_count": 2,  # Modified this line to keep only 2 log files
             "encoding": "utf-8",
             "delay": False,
             "utc": False,
```

### Comparing `crud_repository-0.1.6/src/db/factory.py` & `crud_repository-0.1.7/crud_repository/db/factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 This module provides classes for managing databases.
 """
-from src.db.idatabase import IDatabase
-from src.db.mariadb.db import MariaDBDatabase
-from src.db.mysql.db import MySQLDatabase
-from src.db.postgres.db import PostgreSQLDatabase
-from src.my_logger.logger import CustomLogger
+from crud_repository.db.idatabase import IDatabase
+from crud_repository.db.mariadb.db import MariaDBDatabase
+from crud_repository.db.mysql.db import MySQLDatabase
+from crud_repository.db.postgres.db import PostgreSQLDatabase
+from crud_repository.my_logger.logger import CustomLogger
 
 log = CustomLogger(__name__).get_logger("DEBUG")
 
 
 # ---------------------------------------------------------
 class DatabaseFactory:
     """
     This class provides a factory for creating database instances.
     """
-
     @staticmethod
     def create(config: dict) -> IDatabase:
         """
         Create a database instance based on the provided configuration.
 
         :param config: The configuration for the database.
         :return: (IDatabase) The created database instance.
         """
-        # Create the appropriate database instance based on the configuration
-        # (e.g., PostgreSQL, MySQL, MariaDB, etc.)
-        if config["type"] == "postgresql":
-            return PostgreSQLDatabase(
-                **{
-                    "db_name": config["db_name"],
-                    "user": config["user"],
-                    "password": config["password"],
-                    "host": config["host"],
-                    "port": config["port"],
-                }
-            )
-        if config["type"] == "mysql":
-            return MySQLDatabase(
-                **{
-                    "db_name": config["db_name"],
-                    "user": config["user"],
-                    "password": config["password"],
-                    "host": config["host"],
-                    "port": config["port"],
-                }
-            )
-        if config["type"] == "mariadb":
-            return MariaDBDatabase(
-                **{
-                    "db_name": config["db_name"],
-                    "user": config["user"],
-                    "password": config["password"],
-                    "host": config["host"],
-                    "port": config["port"],
-                }
-            )
-        # ... other database types
-        raise ValueError("Invalid database type")
+        try:
+            # Create the appropriate database instance based on the configuration
+            # (e.g., PostgreSQL, MySQL, MariaDB, etc.)
+            if config["type"] == "postgresql":
+                return PostgreSQLDatabase(
+                    **{
+                        "db_name": config["db_name"],
+                        "user": config["user"],
+                        "password": config["password"],
+                        "host": config["host"],
+                        "port": config["port"],
+                    }
+                )
+            if config["type"] == "mysql":
+                return MySQLDatabase(
+                    **{
+                        "db_name": config["db_name"],
+                        "user": config["user"],
+                        "password": config["password"],
+                        "host": config["host"],
+                        "port": config["port"],
+                    }
+                )
+            if config["type"] == "mariadb":
+                return MariaDBDatabase(
+                    **{
+                        "db_name": config["db_name"],
+                        "user": config["user"],
+                        "password": config["password"],
+                        "host": config["host"],
+                        "port": config["port"],
+                    }
+                )
+            # ... other database types
+            raise ValueError("Invalid database type")
+        except Exception as e:
+            log.debug(f"Error creating database instance: {e}")
+            raise e
```

### Comparing `crud_repository-0.1.6/src/db/idatabase.py` & `crud_repository-0.1.7/crud_repository/db/idatabase.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 This module provides classes for managing databases.
 """
 from abc import ABC, abstractmethod
 from sqlalchemy import Engine, Connection
-from sqlalchemy.orm import scoped_session
-from src.my_logger.logger import CustomLogger
-
-log = CustomLogger(__name__).get_logger("DEBUG")
+from sqlalchemy.orm import scoped_session, sessionmaker
+from crud_repository.my_logger.logger import CustomLogger
 
 
 # ---------------------------------------------------------
 class IDatabase(ABC):
     """
-    This class defines the interface for a database.
+    This class defines the interface for all databases.
 
     Attributes:
         engine (Engine): The SQLAlchemy engine for the database.
         session (Session): The SQLAlchemy session for the database.
     """
-
-    session: scoped_session
     engine: Engine
+    session: scoped_session
 
-    @abstractmethod
     def connect(self) -> Connection:
         """
-        Connect to the database.
+        Connect to the PostgreSQL database.
+        :return: (Connection) The SQLAlchemy connection for the PostgreSQL database.
         """
-        raise NotImplementedError("Subclasses must implement this method.")
+        return self.engine.connect()
 
-    @abstractmethod
-    def get_session(self) -> scoped_session:
+    def get_scoped_session(self) -> scoped_session:
         """
-        Get a session from the database.
-
-        Returns:
-            Session: The SQLAlchemy session for the database.
+        Get a session from the PostgreSQL database.  .
+        :return: (scoped_session) The SQLAlchemy session for the PostgreSQL database.
         """
-        raise NotImplementedError("Subclasses must implement this method.")
+        _scoped_session = scoped_session(sessionmaker(bind=self.engine))
+        return _scoped_session
 
     def __dict__(self):
         return {"engine": self.engine, "session": self.session}
 
     def __repr__(self):
         return f"DatabaseInterface(engine={self.engine!r}, session={self.session!r})"
```

### Comparing `crud_repository-0.1.6/src/db/mariadb/db.py` & `crud_repository-0.1.7/crud_repository/db/mariadb/db.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from sqlalchemy import create_engine, Engine, Connection
 from sqlalchemy.exc import OperationalError
 from sqlalchemy.orm import Session
 from sqlalchemy.orm import scoped_session
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy_utils import database_exists, create_database
 
-from src.db.idatabase import IDatabase
-from src.model.base import Base
-from src.my_logger.logger import CustomLogger
+from crud_repository.db.idatabase import IDatabase
+from crud_repository.model.base import Base
+from crud_repository.my_logger.logger import CustomLogger
 
 log = CustomLogger(__name__).get_logger("DEBUG")
 
 
 # ---------------------------------------------------------
 class MariaDBDatabase(IDatabase):
     """
@@ -58,18 +58,7 @@
             traceback.print_exc()
             raise e
         except Exception as e:
             log.debug(f"Error initializing MySQL database: {e}")
             traceback.print_exc()
             sys.exit(1)
 
-    def connect(self) -> Connection:
-        """
-        Connect to the MariaDB database and return the connection.
-        """
-        return self.engine.connect()
-
-    def get_session(self) -> scoped_session:
-        """
-        Get a session from the MariaDB database.
-        """
-        return self.session
```

### Comparing `crud_repository-0.1.6/src/db/mysql/db.py` & `crud_repository-0.1.7/crud_repository/db/postgres/db.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,42 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 This module provides classes for managing databases.
 """
-import sys
-import traceback
-
-from sqlalchemy import create_engine, Connection, sql
-from sqlalchemy.exc import OperationalError
-from sqlalchemy.orm import scoped_session
-from sqlalchemy.orm import sessionmaker
+from sqlalchemy import create_engine, Connection, text
+from sqlalchemy.orm import scoped_session, sessionmaker
 from sqlalchemy_utils import database_exists, create_database
 
-from src.db.idatabase import IDatabase
-from src.model.base import Base
-from src.my_logger.logger import CustomLogger
+from crud_repository.db.idatabase import IDatabase
+from crud_repository.model.base import Base
+from crud_repository.my_logger.logger import CustomLogger
 
 log = CustomLogger(__name__).get_logger("DEBUG")
 
 
-# ---------------------------------------------------------
-class MySQLDatabase(IDatabase):
+class PostgreSQLDatabase(IDatabase):
+
     """
-    This class provides a MySQL implementation of the Database.
+    This class provides a PostgreSQL implementation of the Database using sqlalchemy_utils.
     """
 
     def __init__(self, **kwargs):
         """
-        Initialize the MySQLDatabase.
+        Initialize the PostgreSQLDatabase.
         :param kwargs: (dict) The keyword arguments for the PostgreSQL database.
         """
-        try:
-            db_name = kwargs.get("db_name", None)
-            user = kwargs.get("user", None)
-            password = kwargs.get("password", None)
-            host = kwargs.get("host", None)
-            port = kwargs.get("port", None)
-            url = kwargs.get("url", f"mysql+pymysql://{user}:{password}@{host}:{port}/{db_name}")
-            # Create the database if it doesn't exist
-            if not database_exists(url):
-                create_database(url)
-            # Create the engine and session
-            self.engine = create_engine(url)
-            self.session = scoped_session(sessionmaker(bind=self.engine))
-            # Add this line to create all tables based on Base class
-            Base.metadata.create_all(self.engine)
-        except OperationalError as e:
-            log.debug(f"Error connecting to MySQL database: {e}")
-            traceback.print_exc()
-            raise e
-        except Exception as e:
-            log.debug(f"Error initializing MySQL database: {e}")
-            traceback.print_exc()
-            sys.exit(1)
+        db_name = kwargs.get("db_name", None)
+        user = kwargs.get("user", None)
+        password = kwargs.get("password", None)
+        host = kwargs.get("host", None)
+        port = kwargs.get("port", None)
+        url = kwargs.get("url", f"postgresql+psycopg2://{user}:{password}@{host}:{port}/{db_name}")
+        # Create the database if it doesn't exist
+        if not database_exists(url):
+            create_database(url)
+        # Create the engine and session
+        self.engine = create_engine(url)
+        self.session = scoped_session(sessionmaker(bind=self.engine))
+        Base.metadata.create_all(self.engine)
 
-    def connect(self) -> Connection:
-        """
-        Connect to the MySQL database and return the connection.
-        """
-        return self.engine.connect()
 
-    def get_session(self) -> scoped_session:
-        """
-        Get a session from the MySQL database.
-        """
-        return self.session
```

### Comparing `crud_repository-0.1.6/src/my_logger/formatters.py` & `crud_repository-0.1.7/crud_repository/my_logger/formatters.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.6/src/my_logger/handlers.py` & `crud_repository-0.1.7/crud_repository/my_logger/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import traceback
 import sys
 import time
 from logging import StreamHandler, DEBUG, Formatter
 from typing import Optional
 
-from src.my_logger.formatters import CustomFormatter
+from crud_repository.my_logger.formatters import CustomFormatter
 
 
 # ------------------------------------------------------------------------
 class CustomStreamHandler(StreamHandler):
     """
     This class is a custom stream handler for logging.
     """
```

### Comparing `crud_repository-0.1.6/src/my_logger/logger.py` & `crud_repository-0.1.7/crud_repository/my_logger/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module contains the CustomLogger class which is used for custom logging.
 """
 
 import logging
 import logging.config
 import sys
 
-from src.__config__ import log_config
+from crud_repository.__config__ import log_config
 
 
 # ---------------------------------------------------------
 class CustomLogger(logging.Logger):
     """
     This class is used for custom logging.
     """
```

### Comparing `crud_repository-0.1.6/src/my_logger/monitor.py` & `crud_repository-0.1.7/crud_repository/my_logger/monitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains the CommandLogger class which is used for logging command events.
 """
 
-from src.my_logger.logger import CustomLogger
+from crud_repository.my_logger.logger import CustomLogger
 
 log = CustomLogger(__name__).get_logger("DEBUG")
 
 
 class CommandLogger:
     """
     This class is used for logging command events.
```

### Comparing `crud_repository-0.1.6/src/repo/repository.py` & `crud_repository-0.1.7/crud_repository/repo/repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from abc import ABC, abstractmethod
 from typing import Generic, TypeVar
 import sqlalchemy
 from sqlalchemy.exc import SQLAlchemyError
-from src.db.idatabase import IDatabase
-from src.model.base import Base
-from src.my_logger.logger import CustomLogger
+from crud_repository.db.idatabase import IDatabase
+from crud_repository.model.base import Base
+from crud_repository.my_logger.logger import CustomLogger
 
 log = CustomLogger(__name__).get_logger("DEBUG")
 T = TypeVar("T", bound=Base)
 
 
 # ---------------------------------------------------------
 class IRepository(ABC, Generic[T]):
@@ -34,15 +34,15 @@
 # ---------------------------------------------------------
 class Repository(IRepository[T]):
     def __init__(self, database: IDatabase, model: type[T]):
         self.database = database
         self.model = model
 
     def create(self, entity: T) -> T:
-        session = self.database.get_session()
+        session = self.database.get_scoped_session()
         try:
             session.add(entity)
             session.commit()
             return self.model(
                 **{
                     c.key: getattr(entity, c.key)
                     for c in sqlalchemy.inspect(entity).mapper.column_attrs
@@ -52,25 +52,25 @@
             session.rollback()
             log.error(f"Error creating entity in {self.model.__name__} table: {e}")
             raise e
         finally:
             session.close()
 
     def read(self, id) -> T:
-        session = self.database.get_session()
+        session = self.database.get_scoped_session()
         try:
             return session.get(self.model, id)
         except SQLAlchemyError as e:
             log.error(f"Error reading entity from {self.model.__name__} table: {e}")
             raise e
         finally:
             session.close()
 
     def update(self, entity: T) -> T:
-        session = self.database.get_session()
+        session = self.database.get_scoped_session()
         try:
             session.merge(entity)
             session.commit()
             return self.model(
                 **{
                     c.key: getattr(entity, c.key)
                     for c in sqlalchemy.inspect(entity).mapper.column_attrs
@@ -80,15 +80,15 @@
             session.rollback()
             log.error(f"Error updating entity from {entity.__name__} table: {e}")
             raise e
         finally:
             session.close()
 
     def delete(self, entity: T) -> None:
-        session = self.database.get_session()
+        session = self.database.get_scoped_session()
         try:
             session.delete(entity)
             session.commit()
         except SQLAlchemyError as e:
             session.rollback()
             log.error(f"Error deleting entity from {entity.__name__} table: {e}")
             raise e
```

