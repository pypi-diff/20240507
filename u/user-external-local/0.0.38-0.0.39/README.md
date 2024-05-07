# Comparing `tmp/user-external-local-0.0.38.tar.gz` & `tmp/user_external_local-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user-external-local-0.0.38.tar", last modified: Thu Jan 25 19:19:28 2024, max compression
+gzip compressed data, was "user_external_local-0.0.39.tar", last modified: Tue May  7 08:34:17 2024, max compression
```

## Comparing `user-external-local-0.0.38.tar` & `user_external_local-0.0.39.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 19:19:28.313938 user-external-local-0.0.38/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-25 19:19:28.313938 user-external-local-0.0.38/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-25 19:19:01.000000 user-external-local-0.0.38/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-01-25 19:19:01.000000 user-external-local-0.0.38/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 19:19:28.313938 user-external-local-0.0.38/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-01-25 19:19:01.000000 user-external-local-0.0.38/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 19:19:28.309938 user-external-local-0.0.38/user_external_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 19:19:28.313938 user-external-local-0.0.38/user_external_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 19:19:01.000000 user-external-local-0.0.38/user_external_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22732 2024-01-25 19:19:01.000000 user-external-local-0.0.38/user_external_local/src/user_externals_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 19:19:28.313938 user-external-local-0.0.38/user_external_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-25 19:19:28.000000 user-external-local-0.0.38/user_external_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-25 19:19:28.000000 user-external-local-0.0.38/user_external_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 19:19:28.000000 user-external-local-0.0.38/user_external_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-25 19:19:28.000000 user-external-local-0.0.38/user_external_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-25 19:19:28.000000 user-external-local-0.0.38/user_external_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:34:17.582368 user_external_local-0.0.39/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 08:34:17.582368 user_external_local-0.0.39/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-07 08:33:52.000000 user_external_local-0.0.39/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 08:33:52.000000 user_external_local-0.0.39/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:34:17.582368 user_external_local-0.0.39/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-07 08:33:52.000000 user_external_local-0.0.39/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:34:17.582368 user_external_local-0.0.39/user_external_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:34:17.582368 user_external_local-0.0.39/user_external_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 08:33:52.000000 user_external_local-0.0.39/user_external_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-05-07 08:33:52.000000 user_external_local-0.0.39/user_external_local/src/user_externals_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:34:17.582368 user_external_local-0.0.39/user_external_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 08:34:17.000000 user_external_local-0.0.39/user_external_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 08:34:17.000000 user_external_local-0.0.39/user_external_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:34:17.000000 user_external_local-0.0.39/user_external_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-07 08:34:17.000000 user_external_local-0.0.39/user_external_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 08:34:17.000000 user_external_local-0.0.39/user_external_local.egg-info/top_level.txt
```

### Comparing `user-external-local-0.0.38/PKG-INFO` & `user_external_local-0.0.39/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: user-external-local
-Version: 0.0.38
+Version: 0.0.39
 Home-page: https://github.com/circles-zone/user-external-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: logger-local>=0.0.60
-Requires-Dist: database-without-orm-local>=0.0.83
+Requires-Dist: database-mysql-local>=0.0.83
 Requires-Dist: python-sdk-remote>=0.0.64
 Requires-Dist: user-context-remote>=0.0.54
 Requires-Dist: database-infrastructure-local>=0.0.23
 
 user-external-local
```

### Comparing `user-external-local-0.0.38/README.md` & `user_external_local-0.0.39/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 # External User Local Python Package
 
-The External User Local Python Package is a library designed to manage access tokens for external users. It provides functions to insert, update, retrieve, and delete access tokens from a database. This library is intended to be used in conjunction with your own project.
+The External User Local Python Package is a library designed to manage access tokens for external users. It provides
+functions to insert, update, retrieve, and delete access tokens from a database. This library is intended to be used in
+conjunction with your own project.
 
 ## Installation
 
 -pip install external-user-local 0.0.25
 -add to requirements.txt external-user-local== 0.0.25
 
 # Importing the Library
+
 from library import library_DB import Accsess_Token_Library
+
 # Usage Example: assuming system_id=1
+
 # Initialize the access token library
+
 all methods are static, no initialize required
 
 # Insert a new access token
-ExternalUser.insert_or_update_external_user_access_token("example_user", 123,1, "example_token","example_expiry","example refresh")
-notice! refresh and expiry arent a mandatory 
+
+ExternalUser.insert_or_update_external_user_access_token("example_user", 123,1, "example_token","example_expiry","
+example refresh")
+notice! refresh and expiry arent a mandatory
+
 # Update an existing access token
+
 ExternalUser.update_user_external(123, "updated_token")
 
 # Retrieve an access token by profile ID
+
 access_token = ExternalUser.get_access_token_by_profile_id(123)
 
 # Retrieve an access token by user name
+
 access_token = ExternalUser.get_access_token_by_user_name("example_user",1)
 
 # Delete an access token by profile ID
+
 ExternalUser.delete_access_token_by_profile_id(123)
 
 # Update an existing access token by username
+
 ExternalUser.update_user_external_by_user_name("example_user",1, "new_token")
```

### Comparing `user-external-local-0.0.38/setup.py` & `user_external_local-0.0.39/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 PACKAGE_NAME = "user-external-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/user-external-local
-    version='0.0.38',
+    version='0.0.39',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="user-external-local",
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'logger-local>= 0.0.60',
-        'database-without-orm-local>=0.0.83',
+        'logger-local>=0.0.60',
+        'database-mysql-local>=0.0.83',
         'python-sdk-remote>=0.0.64',
         'user-context-remote>=0.0.54',
         'database-infrastructure-local>=0.0.23'
     ],
 )
```

### Comparing `user-external-local-0.0.38/user_external_local/src/user_externals_local.py` & `user_external_local-0.0.39/user_external_local/src/user_externals_local.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-from logger_local.LoggerComponentEnum import LoggerComponentEnum
-import dotenv
-import os
-import sys
-from logger_local.Logger import Logger
 from database_mysql_local.connector import Connector
 from database_mysql_local.generic_crud import GenericCRUD
-sys.path.append(os.path.abspath(os.path.join(
-    os.path.dirname(__file__), '..')))
-dotenv.load_dotenv()
+from logger_local.LoggerComponentEnum import LoggerComponentEnum
+from logger_local.LoggerLocal import Logger
+
 USER_EXTERNAL_LOCAL_PYTHON_PACKAGE_COMPONENT_ID = 115
 USER_EXTERNAL_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME = 'user_external_local_python'
 DEVELOPER_EMAIL = "idan.a@circ.zone"
 object_init = {
     'component_id': USER_EXTERNAL_LOCAL_PYTHON_PACKAGE_COMPONENT_ID,
     'component_name': USER_EXTERNAL_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
@@ -28,30 +23,29 @@
 class UserExternalsLocal(GenericCRUD):
     def __init__(self, is_test_data: bool = False):
         super().__init__(default_schema_name=DEFAULT_SCHEMA_NAME, default_table_name=DEFAULT_TABLE_NAME,
                          default_view_table_name=DEFAULT_VIEW_NAME, default_id_column_name=DEFAULT_ID_COLUMN_NAME,
                          is_test_data=is_test_data)
 
     # TODO change the order of the parameters: system_id, username, profile_id ..
-    def insert_or_update_user_external_access_token(username: str, profile_id: int, system_id: int, access_token: str,
+    def insert_or_update_user_external_access_token(self, username: str, profile_id: int, system_id: int, access_token: str,
                                                     expiry=None, refresh_token: str = None) -> None:
         object_start = {
             'username': username,
             'profile_id': profile_id,
             'system_id': system_id,
             'access_token': access_token,
             'expiry': expiry,
             'refresh_token': refresh_token
         }
         logger.start(object=object_start)
         try:
-            current_token = UserExternalsLocal.get_access_token(
-                username, profile_id, system_id)
+            current_token = self.get_access_token(username, profile_id, system_id)
             if current_token is not None:
-                UserExternalsLocal.delete_access_token(
+                self.delete_access_token(
                     username, system_id, profile_id)
 
             connection = Connector.connect('user_external')
             if (expiry is None):
                 expiry = ""
             if (refresh_token is None):
                 refresh_token = ""
@@ -81,15 +75,15 @@
             logger.info("external user inserted", object=object_info)
         except Exception as error:
             logger.exception(object=error)
             logger.end()
             raise
         logger.end(object={})
 
-    def get_access_token_by_username_and_system_id(username: str, system_id: int) -> str:
+    def get_access_token_by_username_and_system_id(self, username: str, system_id: int) -> str:
         access_token = None
         try:
             object_start = {
                 'username': username,
                 'system_id': system_id
             }
             logger.start(object=object_start)
@@ -104,15 +98,15 @@
             logger.end()
             raise
         logger.end(object={'access_token': access_token})
         return access_token
 
     # TODO I think think the order of the paramters should be system_id, username and profile_id
     # TODO Shall we default the profile_id to profile_id from User Context?
-    def get_access_token(username: str, profile_id: int, system_id: int) -> str:
+    def get_access_token(self, username: str, profile_id: int, system_id: int) -> str:
         access_token = None
         try:
             object_start = {
                 'username': username,
                 'profile_id': profile_id,
                 'system_id': system_id
             }
@@ -129,15 +123,15 @@
         except Exception as error:
             logger.exception(object=error)
             logger.end()
             raise
         logger.end(object={'access_token': access_token})
         return access_token
 
-    def update_user_external_access_token(username: str, system_id: int, profile_id: int, access_token, expiry=None,
+    def update_user_external_access_token(self, username: str, system_id: int, profile_id: int, access_token, expiry=None,
                                           refresh_token: str = None) -> None:
         try:
             object_start = {
                 'username': username,
                 'system_id': system_id,
                 'profile_id': profile_id,
                 'access_token': access_token,
@@ -162,15 +156,15 @@
             logger.info("external user updated", object=object_info)
         except Exception as error:
             logger.exception(object=error)
             logger.end()
             raise
         logger.end(object={})
 
-    def delete_access_token(username: str, system_id: int, profile_id: int):
+    def delete_access_token(self, username: str, system_id: int, profile_id: int):
         try:
             object_start = {
                 'username': username,
                 'system_id': system_id,
                 'profile_id': profile_id,
             }
             logger.start(object=object_start)
@@ -192,16 +186,15 @@
             logger.info("external user updated", object=object_info)
         except Exception as error:
             logger.exception(object=error)
             logger.end()
             raise
         logger.end(object={})
 
-    def get_auth_details_by_system_id_and_profile_id(system_id: int, profile_id: int) -> None:
-        auth_details = None
+    def get_auth_details_by_system_id_and_profile_id(self, system_id: int, profile_id: int) -> tuple:
         try:
             object_start = {
                 'system_id': system_id,
                 "profile_id": profile_id
             }
             logger.warning(
                 log_message="This static method is deprecated, "
@@ -212,293 +205,38 @@
             query_get_all = (
                 "SELECT eu.user_external_id, access_token,refresh_token,expiry FROM user_external.user_external_view AS eu"
                 " JOIN profile_user_external.profile_user_external_table AS eup on eu.user_external_id=eup.user_external_id"
                 " WHERE eu.system_id=%s AND eup.profile_id=%s order BY eu.start_timestamp DESC LIMIT 1"
             )
             cursor = connection.cursor()
             cursor.execute(query_get_all, (system_id, profile_id))
-            auth_details = cursor.fetchall()[0]
+            auth_details = cursor.fetchone()
         except Exception as error:
             logger.exception(object=error)
             logger.end()
             raise
         logger.end(object={'auth_details': auth_details})
         return auth_details
 
     # TODO Change the order of the parameters to system_id, username, profile_id
-    def get_auth_details(username: str, system_id: int, profile_id: int) -> None:
+    def get_auth_details(self, username: str, system_id: int, profile_id: int) -> None:
         auth_details = None
         try:
             object_start = {
                 "username": username,
                 'system_id': system_id,
                 "profile_id": profile_id,
             }
             logger.start(object=object_start)
             connection = Connector.connect('user_external')
             query_get_all = (
                 "SELECT access_token,refresh_token,expiry FROM user_external.user_external_view AS eu JOIN"
                 " profile_user_external.profile_user_external_view AS eup ON eu.user_external_id=eup.user_external_id WHERE"
                 " eu.username=%s AND eu.system_id=%s AND eup.profile_id=%s ORDER BY eu.start_timestamp DESC LIMIT 1"
             )
-            cursor = connection.cursor()
-            cursor.execute(query_get_all, (username, system_id, profile_id))
-            auth_details_list = cursor.fetchall()
-            if auth_details_list:
-                auth_details = auth_details_list[0]
-            else:
-                logger.error(log_message="user external not found", object={"auth_details_list": auth_details_list})
-        except Exception as error:
-            logger.exception(object=error)
-            logger.end()
-            raise
-        logger.end(object={'auth_details': auth_details})
-        return auth_details
-
-    # These static methods are deprecated and should be removed by the end of Mars 2024
-    @staticmethod
-    # TODO change the order of the parameters: system_id, username, profile_id ..
-    def insert_or_update_user_external_access_token(username: str, profile_id: int, system_id: int, access_token: str,
-                                                    expiry=None, refresh_token: str = None) -> None:
-        object_start = {
-            'username': username,
-            'profile_id': profile_id,
-            'system_id': system_id,
-            'access_token': access_token,
-            'expiry': expiry,
-            'refresh_token': refresh_token
-        }
-        logger.warning(
-            log_message="This static method is deprecated, "
-                        "please use the non static method",
-        )
-        logger.start(object=object_start)
-        try:
-            current_token = UserExternalsLocal.get_access_token(
-                username, profile_id, system_id)
-            if current_token is not None:
-                UserExternalsLocal.delete_access_token(
-                    username, system_id, profile_id)
-
-            connection = Connector.connect('user_external')
-            if (expiry is None):
-                expiry = ""
-            if (refresh_token is None):
-                refresh_token = ""
-            query_insert_external = (
-                "INSERT INTO user_external_table (system_id,username,access_token,expiry,refresh_token)"
-                " VALUES (%s,%s,%s,%s,%s)"
-            )
-            values = (system_id, username, access_token, expiry, refresh_token)
-            cursor = connection.cursor()
-            cursor.execute(query_insert_external, values)
-            id_new = cursor.lastrowid()
-            values = (id_new, profile_id)
-            connection.commit()
-            connection_profile = Connector.connect('profile_user_external')
-            query_insert_profile_user_external = (
-                "INSERT INTO profile_user_external_table (user_external_id,profile_id) VALUES (%s,%s)"
-            )
-            cursor = connection_profile.cursor()
-            cursor.execute(query_insert_profile_user_external, values)
-            connection_profile.commit()
-            object_info = {
-                'username': username,
-                'system_id': system_id,
-                'profile_id': profile_id,
-                'access_token': access_token,
-            }
-            logger.info("external user inserted", object=object_info)
-        except Exception as error:
-            logger.exception(object=error)
-            logger.end()
-            raise
-        logger.end(object={})
-
-    @staticmethod
-    def get_access_token_by_username_and_system_id(username: str, system_id: int) -> str:
-        access_token = None
-        try:
-            object_start = {
-                'username': username,
-                'system_id': system_id
-            }
-            logger.warning(
-                log_message="This static method is deprecated, "
-                            "please use the non static method",
-            )
-            logger.start(object=object_start)
-            connection = Connector.connect('user_external')
-            # TODO: move to generic crud
-            query_get = "SELECT access_token FROM user_external.user_external_view WHERE username=%s AND system_id=%s"
-            cursor = connection.cursor()
-            cursor.execute(query_get, (username, system_id))
-            access_token = cursor.fetchone()
-        except Exception as error:
-            logger.exception(object=error)
-            logger.end()
-            raise
-        logger.end(object={'access_token': access_token})
-        return access_token
-
-    @staticmethod
-    # TODO I think think the order of the paramters should be system_id, username and profile_id
-    # TODO Shall we default the profile_id to profile_id from User Context?
-    def get_access_token(username: str, profile_id: int, system_id: int) -> str:
-        access_token = None
-        try:
-            object_start = {
-                'username': username,
-                'profile_id': profile_id,
-                'system_id': system_id
-            }
-            logger.warning(
-                log_message="This static method is deprecated, "
-                            "please use the non static method",
-            )
-            logger.start(object=object_start)
-            connection = Connector.connect('user_external')
-            query_get = (
-                "SELECT access_token FROM user_external.user_external_view as eu"
-                " join profile_user_external.profile_user_external_table as eup on eu.user_external_id=eup.user_external_id"
-                " WHERE eu.username=%s AND eu.system_id=%s And eup.profile_id=%s"
-            )
-            cursor = connection.cursor()
-            cursor.execute(query_get, (username, system_id, profile_id))
-            access_token = cursor.fetchone()
-        except Exception as error:
-            logger.exception(object=error)
-            logger.end()
-            raise
-        logger.end(object={'access_token': access_token})
-        return access_token
-
-    @staticmethod
-    def update_user_external_access_token(username: str, system_id: int, profile_id: int, access_token, expiry=None,
-                                          refresh_token: str = None) -> None:
-        try:
-            object_start = {
-                'username': username,
-                'system_id': system_id,
-                'profile_id': profile_id,
-                'access_token': access_token,
-            }
-            logger.warning(
-                log_message="This static method is deprecated, "
-                            "please use the non static method",
-            )
-            logger.start(object=object_start)
-            connection = Connector.connect('user_external')
-            update_query = (
-                "UPDATE user_external.user_external_table AS eu JOIN profile_user_external.profile_user_external_table AS eup"
-                " ON eu.user_external_id = eup.user_external_id SET eu.access_token = %s WHERE eu.username = %s AND"
-                " eu.system_id = %s AND eup.profile_id = %s;"
-            )
-            values = (access_token, username, system_id, profile_id)
-            cursor = connection.cursor()
-            cursor.execute(update_query, values)
-            connection.commit()
-            object_info = {
-                'username': username,
-                'system_id': system_id,
-                'profile_id': profile_id,
-                'access_token': access_token,
-            }
-            logger.info("external user updated", object=object_info)
-        except Exception as error:
-            logger.exception(object=error)
-            logger.end()
-            raise
-        logger.end(object={})
-
-    @staticmethod
-    def delete_access_token(username: str, system_id: int, profile_id: int):
-        try:
-            object_start = {
-                'username': username,
-                'system_id': system_id,
-                'profile_id': profile_id,
-            }
-            logger.warning(
-                log_message="This static method is deprecated, "
-                            "please use the non static method",
-            )
-            logger.start(object=object_start)
-            connection = Connector.connect('user_external')
-            cursor = connection.cursor()
-            update_query = (
-                "UPDATE user_external.user_external_table AS eu JOIN profile_user_external.profile_user_external_table AS eup"
-                " ON eu.user_external_id = eup.user_external_id SET eu.end_timestamp = now() WHERE eu.username = %s AND"
-                " eu.system_id = %s AND eup.profile_id = %s;"
-            )
-            values = (username, system_id, profile_id)
-            cursor.execute(update_query, values)
-            connection.commit()
-            object_info = {
-                'username': username,
-                'system_id': system_id,
-                'profile_id': profile_id,
-            }
-            logger.info("external user updated", object=object_info)
-        except Exception as error:
-            logger.exception(object=error)
-            logger.end()
-            raise
-        logger.end(object={})
-
-    @staticmethod
-    def get_auth_details_by_system_id_and_profile_id(system_id: int, profile_id: int) -> None:
-        auth_details = None
-        try:
-            object_start = {
-                'system_id': system_id,
-                "profile_id": profile_id
-            }
-            logger.warning(
-                log_message="This static method is deprecated, "
-                            "please use the non static method",
-            )
-            logger.start(object=object_start)
-            connection = Connector.connect('user_external')
-            query_get_all = (
-                "SELECT eu.user_external_id, access_token,refresh_token,expiry FROM user_external.user_external_view AS eu"
-                " JOIN profile_user_external.profile_user_external_table AS eup on eu.user_external_id=eup.user_external_id"
-                " WHERE eu.system_id=%s AND eup.profile_id=%s order BY eu.start_timestamp DESC LIMIT 1"
-            )
-            cursor = connection.cursor()
-            cursor.execute(query_get_all, (system_id, profile_id))
-            auth_details = cursor.fetchall()[0]
-        except Exception as error:
-            logger.exception(object=error)
-            logger.end()
-            raise
-        logger.end(object={'auth_details': auth_details})
-        return auth_details
-
-    @staticmethod
-    # TODO Change the order of the parameters to system_id, username, profile_id
-    def get_auth_details(username: str, system_id: int, profile_id: int) -> None:
-        auth_details = None
-        try:
-            object_start = {
-                "username": username,
-                'system_id': system_id,
-                "profile_id": profile_id,
-            }
-            logger.warning(
-                log_message="This static method is deprecated, "
-                            "please use the non static method",
-            )
-            logger.start(object=object_start)
-            connection = Connector.connect('user_external')
-            query_get_all = (
-                "SELECT access_token,refresh_token,expiry FROM user_external.user_external_view AS eu JOIN"
-                " profile_user_external.profile_user_external_view AS eup ON eu.user_external_id=eup.user_external_id WHERE"
-                " eu.username=%s AND eu.system_id=%s AND eup.profile_id=%s ORDER BY eu.start_timestamp DESC LIMIT 1"
-            )
             cursor = connection.cursor()
             cursor.execute(query_get_all, (username, system_id, profile_id))
             auth_details_list = cursor.fetchall()
             if auth_details_list:
                 auth_details = auth_details_list[0]
             else:
                 logger.error(log_message="user external not found", object={"auth_details_list": auth_details_list})
```

### Comparing `user-external-local-0.0.38/user_external_local.egg-info/PKG-INFO` & `user_external_local-0.0.39/user_external_local.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: user-external-local
-Version: 0.0.38
+Version: 0.0.39
 Home-page: https://github.com/circles-zone/user-external-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: logger-local>=0.0.60
-Requires-Dist: database-without-orm-local>=0.0.83
+Requires-Dist: database-mysql-local>=0.0.83
 Requires-Dist: python-sdk-remote>=0.0.64
 Requires-Dist: user-context-remote>=0.0.54
 Requires-Dist: database-infrastructure-local>=0.0.23
 
 user-external-local
```

