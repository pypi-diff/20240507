# Comparing `tmp/parameterframe-0.0.3.tar.gz` & `tmp/parameterframe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parameterframe-0.0.3.tar", last modified: Fri May  3 10:28:18 2024, max compression
+gzip compressed data, was "parameterframe-0.1.1.tar", last modified: Tue May  7 18:09:30 2024, max compression
```

## Comparing `parameterframe-0.0.3.tar` & `parameterframe-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:28:18.392570 parameterframe-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-03 10:24:29.000000 parameterframe-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    39020 2024-05-03 10:28:18.392570 parameterframe-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-03 10:24:29.000000 parameterframe-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:28:18.392570 parameterframe-0.0.3/parameterframe/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 10:28:17.000000 parameterframe-0.0.3/parameterframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    79272 2024-05-03 10:28:17.000000 parameterframe-0.0.3/parameterframe/parameterframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-03 10:28:18.000000 parameterframe-0.0.3/parameterframe/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:28:18.392570 parameterframe-0.0.3/parameterframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    39020 2024-05-03 10:28:18.000000 parameterframe-0.0.3/parameterframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-03 10:28:18.000000 parameterframe-0.0.3/parameterframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:28:18.000000 parameterframe-0.0.3/parameterframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 10:28:18.000000 parameterframe-0.0.3/parameterframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 10:28:18.000000 parameterframe-0.0.3/parameterframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:28:18.392570 parameterframe-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:09:30.053840 parameterframe-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-07 18:06:28.000000 parameterframe-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40400 2024-05-07 18:09:30.053840 parameterframe-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-07 18:06:28.000000 parameterframe-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:09:30.049840 parameterframe-0.1.1/parameterframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93187 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe/parameterframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:09:30.053840 parameterframe-0.1.1/parameterframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40400 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-07 18:09:30.000000 parameterframe-0.1.1/parameterframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 18:09:29.000000 parameterframe-0.1.1/parameterframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 18:09:30.053840 parameterframe-0.1.1/setup.cfg
```

### Comparing `parameterframe-0.0.3/LICENSE` & `parameterframe-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parameterframe-0.0.3/README.md` & `parameterframe-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 with a use of more expensive, slower or simply no-existant method.
 
 [module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
 
 This module provides a set of functions for interacting with the Google Drive API.
 It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
 
-[module](python_modules/parameterframe.py) | [usage](docs/parameterframe.md) | [drawio: -flow](docs/parameterframe-flow.png) | [drawio: -schema](docs/parameterframe-schema.png) | [drawio: -usage](docs/parameterframe-usage.png) | [![PyPiVersion](https://img.shields.io/pypi/v/parameterframe)](https://pypi.org/project/parameterframe/) - Parameter frame
+[module](python_modules/parameterframe.py) | [usage](docs/parameterframe.md) | [drawio: -flow](docs/parameterframe-flow.png) | [drawio: -schema](docs/parameterframe-schema.png) | [drawio: -usage](docs/parameterframe-usage.png) | [release notes](release_notes/parameterframe.md) | [![PyPiVersion](https://img.shields.io/pypi/v/parameterframe)](https://pypi.org/project/parameterframe/) - Parameterframe
 
 The module provides an interface for managing solution parameters.
 It allows for the structured storage and retrieval of parameter sets from a database.
 
 [module](python_modules/comparisonframe.py) | [usage](docs/comparisonframe.md) | [plantuml](docs/comparisonframe_plantuml.png) - Comparison Frame
 
 Designed to automate and streamline the process of comparing textual data, particularly focusing on various metrics
```

### Comparing `parameterframe-0.0.3/parameterframe/parameterframe.py` & `parameterframe-0.1.1/parameterframe/parameterframe.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Parameter frame
+Parameterframe
 
 The module provides an interface for managing solution parameters.
 It allows for the structured storage and retrieval of parameter sets from a database.
 """
 
 import attr
 import os
@@ -18,14 +18,15 @@
 import ast
 
 from sqlalchemy import create_engine, Column, String, Text, ForeignKey, DateTime
 from sqlalchemy.orm import relationship, sessionmaker, declarative_base
 from sqlalchemy.exc import SQLAlchemyError, IntegrityError, DBAPIError
 from sqlalchemy import inspect
 
+
 __design_choices__ = {
     "FileTypeHandler" : ['prepares one parameter file and reconstructs one parameter file at a time',
                          'txt and yaml files can be processed',
                          'yaml files are not reconstructed 1to1 but are first make into python dictionary, with python type mapping'],
     "ParameterFrame" : ['parameter_names and paramer_description are optional'],
     "DatabaseConnector" : ['connector is an external component that includes handling of connection to some database',
                            'default connector is meant for MockerDB',
@@ -96,26 +97,50 @@
 
         return True
 
     def fetch_entries(self,
                       filters : dict = None,
                       database_name : str = 'default'):
 
+        """
+        Fetches entries from remove mocker to local mocker
+        """
+
         db_remote_handler = self.db_remote_handler(**self.connection_details)
 
         fetched_data = db_remote_handler.search_data(
             database_name = database_name,
             filter_criteria = filters)
 
         self.db_handler.insert_values(
             values_dict_list = fetched_data['results'],
             embed = False)
 
         return True
 
+    def remove_entries(self,
+                       filters : dict = None,
+                       database_name : str = 'default'):
+
+        """
+        Removes entries from remote and local mocker
+        """
+
+        db_remote_handler = self.db_remote_handler(**self.connection_details)
+
+        db_remote_handler.delete_data(
+            database_name = database_name,
+            filter_criteria = filters)
+
+        self.db_handler.remove_from_database(
+            filter_criteria = filters)
+
+        return True
+
+
     def get_entries(self,
                     table_name: str,
                     return_keys : list = None,
                     filters : dict = None ) -> list:
         try:
 
             if filters is None:
@@ -142,68 +167,75 @@
         db_remote_handler.insert_data(
             data = [d for _, d in self.db_handler.data.items()]
         )
 
         return True
 
     def push_tables(self,
-                      solution_description : list,
-                      solution_parameter_set : list,
-                      parameter_set : list,
-                      parameter_set_description : list,
-                      parameter_description : list,
-                      parameter_attribute : list,
-                      attribute_values : list):
+                      solution_description : list = None,
+                      solution_parameter_set : list = None,
+                      parameter_set : list = None,
+                      parameter_set_description : list = None,
+                      parameter_description : list = None,
+                      parameter_attribute : list = None,
+                      attribute_values : list = None):
 
         """
         Pushes tables with database handler
         """
 
-
-        self.add_entries(table_name = 'solution_description',
-                                            entries = solution_description)
-        self.add_entries(table_name = 'solution_parameter_set',
-                                            entries = solution_parameter_set)
-        self.add_entries(table_name = 'parameter_set',
-                                            entries = parameter_set)
-        self.add_entries(table_name = 'parameter_set_description',
-                                            entries = parameter_set_description)
-        self.add_entries(table_name = 'parameter_description',
-                                            entries = parameter_description)
-        self.add_entries(table_name = 'parameter_attribute',
-                                            entries = parameter_attribute)
-        self.add_entries(table_name = 'attribute_values',
-                                            entries = attribute_values)
+        if solution_description:
+            self.add_entries(table_name = 'solution_description',
+                                                entries = solution_description)
+        if solution_parameter_set:
+            self.add_entries(table_name = 'solution_parameter_set',
+                                                entries = solution_parameter_set)
+        if parameter_set:
+            self.add_entries(table_name = 'parameter_set',
+                                                entries = parameter_set)
+        if parameter_set_description:
+            self.add_entries(table_name = 'parameter_set_description',
+                                                entries = parameter_set_description)
+        if parameter_description:
+            self.add_entries(table_name = 'parameter_description',
+                                                entries = parameter_description)
+        if parameter_attribute:
+            self.add_entries(table_name = 'parameter_attribute',
+                                                entries = parameter_attribute)
+        if attribute_values:
+            self.add_entries(table_name = 'attribute_values',
+                                                entries = attribute_values)
 
         self.commit()
 
         return True
 
     def pull_tables(self,
-                      solution_id : list = None,
-                      parameter_set_id : list = None):
+                      solution_id : str = None,
+                      parameter_set_id : str = None):
 
         """
         Pulls commited tables from database for selected solutions
         """
 
         if solution_id is None:
             raise ValueError("Provide solution_id!")
 
-        if parameter_set_id is None:
-            raise ValueError("Provide parameter_set_id!")
-
-        # fetch tables with solution and parameter_set_ids
-        self.fetch_entries(
-            filters={'table_name' : ['solution_description',
+        fetch_filters = {'table_name' : ['solution_description',
                                           'solution_parameter_set',
                                           'parameter_set',
                                           'parameter_set_description'],
-                          'solution_id': [solution_id, None],
-                          'parameter_set_id' :[parameter_set_id, None]})
+                          'solution_id': [solution_id, None]}
+
+        if parameter_set_id:
+            fetch_filters['parameter_set_id'] = [parameter_set_id, None]
+
+        # fetch tables with solution and parameter_set_ids
+        self.fetch_entries(
+            filters = fetch_filters)
 
         # get parameter_id for fetching next tables
         dict_param_ids = self.get_entries(
             table_name = 'parameter_set',
             return_keys=['parameter_id'])
 
         param_ids = [dict_param_id['parameter_id'] for dict_param_id in dict_param_ids]
@@ -249,14 +281,89 @@
             parameter_sets,
             parameter_set_descriptions,
             parameter_descriptions,
             parameter_attributes,
             attribute_values
         )
 
+    def get_parameter_sets_info(self,
+                            solution_id : str = None,
+                            parameter_set_ids : list = None,
+                            deployment_status : str = None):
+
+        """
+        Get parameter sets for solution id with select deployment status.
+        """
+
+        if solution_id is None:
+            raise ValueError("Provide solution_id!")
+
+
+        fetch_filters = {'table_name' : 'solution_parameter_set',
+                        'solution_id': solution_id}
+
+        get_filters = {'solution_id': solution_id}
+
+        if parameter_set_ids:
+            fetch_filters['parameter_set_id'] = parameter_set_ids
+            get_filters['parameter_set_id'] = parameter_set_ids
+
+        if deployment_status:
+            fetch_filters['deployment_status'] = deployment_status
+            get_filters['deployment_status'] = deployment_status
+
+        # fetch tables with solution and parameter_set_ids
+
+        self.fetch_entries(
+            filters=fetch_filters)
+
+        solution_parameter_sets = self.get_entries(
+            table_name = 'solution_parameter_set',
+            filters=get_filters)
+
+
+        return solution_parameter_sets
+
+    def modify_parameter_set_status(self,
+                                    solution_id : str,
+                                    parameter_set_ids : list,
+                                    current_deployment_status : str,
+                                    new_deployment_status : str):
+
+        """
+        Reuploads solution parameter set entry with different status
+        """
+
+        solution_parameter_sets = self.get_parameter_sets_info(
+            solution_id = solution_id,
+            parameter_set_ids = parameter_set_ids,
+            deployment_status = current_deployment_status
+        )
+
+        if len(solution_parameter_sets) == 0:
+            self.logger.warning(f"No deployed parameter_set_ids with {current_deployment_status} from selected!")
+            return False
+
+        for solution_parameter_set in solution_parameter_sets:
+
+            self.remove_entries(
+                filters = {'table_name' : 'solution_parameter_set',
+                        'solution_id': solution_parameter_set['solution_id'],
+                        'parameter_set_id' : solution_parameter_set['parameter_set_id'],
+                        'deployment_status' : current_deployment_status}
+            )
+            solution_parameter_set['deployment_status'] = new_deployment_status
+
+            self.logger.info(
+                f"{solution_id} + {solution_parameter_set['parameter_set_id']} : {current_deployment_status} -> {new_deployment_status}")
+
+        return self.push_tables(solution_parameter_set = solution_parameter_sets)
+
+
+
 
 @attr.s
 class SqlAlchemyDatabaseManager:
 
 
     connection_details = attr.ib(default = {
         'base_url' : "http://localhost:8000"})
@@ -381,73 +488,97 @@
                     if isinstance(related_data, list):
                         data[relationship.key] = [self._as_dict(child, True) for child in related_data]
                     else:
                         data[relationship.key] = self._as_dict(related_data, True)
         return data
 
     def push_tables(self,
-                      solution_description : list,
-                      solution_parameter_set : list,
-                      parameter_set : list,
-                      parameter_set_description : list,
-                      parameter_description : list,
-                      parameter_attribute : list,
-                      attribute_values : list):
+                      solution_description : list = None,
+                      solution_parameter_set : list = None,
+                      parameter_set : list = None,
+                      parameter_set_description : list = None,
+                      parameter_description : list = None,
+                      parameter_attribute : list = None,
+                      attribute_values : list = None):
 
         """
         Pushes tables with database handler
         """
 
+        inserts = []
 
-        solution_description = [self.SolutionDescription(**data)
-                                for data in solution_description]
-
-        parameter_description = [self.ParameterDescription(**data)
-                                for data in parameter_description]
-
-        parameter_set_description = [self.ParameterSetDescription(**data)
-                                for data in parameter_set_description]
-
-        solution_parameter_set = [self.SolutionParameterSet(**data)
-                                for data in solution_parameter_set]
-
-        parameter_set = [self.ParameterSet(**data)
-                                for data in parameter_set]
-
-        parameter_attribute = [self.ParameterAttribute(**data)
-                                for data in parameter_attribute]
-
-        attribute_values = [self.AttributeValues(**data)
-                                for data in attribute_values]
+        if solution_description:
+            solution_description = [self.SolutionDescription(**data)
+                                    for data in solution_description]
+            inserts += solution_description
+        if parameter_description:
+            parameter_description = [self.ParameterDescription(**data)
+                                    for data in parameter_description]
+            inserts += parameter_description
+        if parameter_set_description:
+            parameter_set_description = [self.ParameterSetDescription(**data)
+                                    for data in parameter_set_description]
+            inserts += parameter_set_description
+        if solution_parameter_set:
+            solution_parameter_set = [self.SolutionParameterSet(**data)
+                                    for data in solution_parameter_set]
+            inserts += solution_parameter_set
+        if parameter_set:
+            parameter_set = [self.ParameterSet(**data)
+                                    for data in parameter_set]
+            inserts += parameter_set
+        if parameter_attribute:
+            parameter_attribute = [self.ParameterAttribute(**data)
+                                    for data in parameter_attribute]
+            inserts += parameter_attribute
+        if attribute_values:
+            attribute_values = [self.AttributeValues(**data)
+                                    for data in attribute_values]
+            inserts += attribute_values
 
+        if inserts:
+            self._merge_entries(entries = inserts)
+            return True
 
-        inserts = solution_description + parameter_description + parameter_set +\
-             solution_parameter_set + parameter_set_description + \
-                attribute_values + parameter_attribute
+        return False
 
-        self._merge_entries(entries = inserts)
+    def pull_tables(self,
+                    solution_id : str = None,
+                    parameter_set_id : str = None):
 
-        return True
+        """
+        Pulls commited tables from database for selected solutions
+        """
 
-    def pull_tables(self, solution_id=None, parameter_set_id=None):
-        if solution_id is None or parameter_set_id is None:
-            raise ValueError("Provide both solution_id and parameter_set_id!")
+        if solution_id is None:
+            raise ValueError("Provide solution_id!")
 
         session = self.Session()
         try:
             # Fetch related entries based on solution_id and parameter_set_id
             solution_descriptions = session.query(self.SolutionDescription).filter(
                 self.SolutionDescription.solution_id == solution_id).all()
-            solution_parameter_sets = session.query(self.SolutionParameterSet).filter(
-                self.SolutionParameterSet.solution_id == solution_id,
-                self.SolutionParameterSet.parameter_set_id == parameter_set_id).all()
-            parameter_sets = session.query(self.ParameterSet).filter(
-                self.ParameterSet.parameter_set_id == parameter_set_id).all()
-            parameter_set_descriptions = session.query(self.ParameterSetDescription).filter(
-                self.ParameterSetDescription.parameter_set_id == parameter_set_id).all()
+            if parameter_set_id:
+                solution_parameter_sets = session.query(self.SolutionParameterSet).filter(
+                    self.SolutionParameterSet.solution_id == solution_id,
+                    self.SolutionParameterSet.parameter_set_id == parameter_set_id).all()
+                parameter_sets = session.query(self.ParameterSet).filter(
+                    self.ParameterSet.parameter_set_id == parameter_set_id).all()
+                parameter_set_descriptions = session.query(self.ParameterSetDescription).filter(
+                    self.ParameterSetDescription.parameter_set_id == parameter_set_id).all()
+            else:
+                solution_parameter_sets = session.query(self.SolutionParameterSet).filter(
+                    self.SolutionParameterSet.solution_id == solution_id).all()
+
+                parameter_set_ids = [solution_parameter_set.parameter_set_id for solution_parameter_set in solution_parameter_sets]
+
+                parameter_sets = session.query(self.ParameterSet).filter(
+                    self.ParameterSet.parameter_set_id.in_(parameter_set_ids)).all()
+                parameter_set_descriptions = session.query(self.ParameterSetDescription).filter(
+                    self.ParameterSetDescription.parameter_set_id.in_(parameter_set_ids)).all()
 
             # Fetch parameter_id from parameter_sets for further queries
             param_ids = [param.parameter_id for param in parameter_sets]
 
             # Continue to fetch related entries based on parameter_id
             parameter_descriptions = session.query(self.ParameterDescription).filter(
                 self.ParameterDescription.parameter_id.in_(param_ids)).all()
@@ -471,14 +602,98 @@
 
         except Exception as e:
             session.rollback()
             print(f"An error occurred: {e}")
         finally:
             session.close()
 
+    def get_parameter_sets_info(self,
+                            solution_id : str = None,
+                            parameter_set_ids : list = None,
+                            deployment_status : str = None):
+
+        """
+        Get parameter sets for solution id with select deployment status.
+        """
+
+        if solution_id is None:
+            raise ValueError("Provide solution_id!")
+
+        session = self.Session()
+        try:
+            if parameter_set_ids :
+                solution_parameter_sets = session.query(self.SolutionParameterSet).filter(
+                    self.SolutionParameterSet.solution_id == solution_id,
+                    self.SolutionParameterSet.parameter_set_id == parameter_set_ids).all()
+            elif parameter_set_ids and deployment_status:
+                solution_parameter_sets = session.query(self.SolutionParameterSet).filter(
+                    self.SolutionParameterSet.solution_id == solution_id,
+                    self.SolutionParameterSet.parameter_set_id == parameter_set_ids,
+                    self.SolutionParameterSet.deployment_status == deployment_status).all()
+            else:
+                solution_parameter_sets = session.query(self.SolutionParameterSet).filter(
+                    self.SolutionParameterSet.solution_id == solution_id,
+                    self.SolutionParameterSet.deployment_status == deployment_status).all()
+
+            return [self._as_dict(data) for data in solution_parameter_sets]
+
+        except Exception as e:
+            session.rollback()
+            print(f"An error occurred: {e}")
+        finally:
+            session.close()
+
+    def modify_parameter_set_status(self,
+                                    solution_id : str,
+                                    parameter_set_ids : list,
+                                    current_deployment_status : str,
+                                    new_deployment_status : str):
+
+        """
+        Reuploads solution parameter set entry with different status
+        """
+
+        solution_parameter_sets = self.get_parameter_sets_info(
+            solution_id = solution_id,
+            parameter_set_ids = parameter_set_ids,
+            deployment_status = current_deployment_status
+        )
+
+        if len(solution_parameter_sets) == 0:
+            self.logger.warning(f"No deployed parameter_set_ids with {current_deployment_status} from selected!")
+            return False
+
+
+        session = self.Session()
+        parameter_set_ids = [t['parameter_set_id'] for t in solution_parameter_sets]
+        try:
+            # Fetch the user record to modify
+            solution_parameter_sets = session.query(self.SolutionParameterSet).filter(
+                self.SolutionParameterSet.solution_id == solution_id,
+                self.SolutionParameterSet.parameter_set_id.in_(parameter_set_ids),
+                self.SolutionParameterSet.deployment_status == current_deployment_status).all()
+
+            if solution_parameter_sets:
+                for solution_parameter_set in solution_parameter_sets:
+                    solution_parameter_set.deployment_status = new_deployment_status
+                    self.logger.info(
+        f"{solution_id} + {solution_parameter_set.parameter_set_id} : {current_deployment_status} -> {new_deployment_status}")
+                    session.commit()
+
+
+
+        except Exception as e:
+            session.rollback()  # Roll back in case of errors
+            print(f"An error occurred: {e}")
+        finally:
+            session.close()  # Close the session to free resources
+
+
+        return True
+
 
 @attr.s
 class FileTypeHandler:
 
     """
     Handles raw files, processes them for storage
     and reconstructs when pulling from storage.
@@ -496,15 +711,15 @@
     parameter_id = attr.ib(default=None, type = str)
 
     file_type = attr.ib(default=None, type = str)
     file_content = attr.ib(default=None, type = str)
 
     is_reconstructed = attr.ib(default=False, type = bool)
     # types for which fth will work
-    available_types = attr.ib(default=['yaml', 'txt' ,'unknown'])
+    available_types = attr.ib(default=['yaml', 'txt' ,'other'])
     chunk_size = attr.ib(default=255)
 
     # logger config
     logger = attr.ib(default=None)
     logger_name = attr.ib(default='FileTypeHandler')
     loggerLvl = attr.ib(default=logging.INFO)
     logger_format = attr.ib(default=None)
@@ -568,15 +783,15 @@
         if file_extension in ['.yml', '.yaml']:
             return 'yaml'
         if file_extension == '.txt':
             return 'txt'
         # if file_extension == '.dill':
         #     return 'dill'
 
-        return 'unknown'
+        return 'other'
 
     def _load_file_content(self,
                             file_path: str,
                             file_type : str) -> object:
 
         """
         Load content based on type.
@@ -963,15 +1178,15 @@
             return self._process_txt(content = file_content,
                                     parameter_id = parameter_id)
 
         if file_type == 'dill':
             return self._process_dill(content = file_content,
                                         parameter_id = parameter_id)
 
-        if file_type == 'unknown':
+        if file_type == 'other':
             return self._process_binary(content = file_content,
                                         parameter_id = parameter_id)
 
 
     def process_file(self,
                      file_path : str = None,
                      parameter_name : str = None,
@@ -1024,15 +1239,15 @@
 
         if file_type == 'txt':
             return self._reconstruct_txt(attribute_values_list = attribute_values_list)
 
         if file_type == 'dill':
             return self._reconstruct_dill(attribute_values_list = attribute_values_list)
 
-        if file_type == 'unknown':
+        if file_type == 'other':
             return self._reconstruct_binary(attribute_values_list = attribute_values_list)
 
         return None
 
 
     def _reconstruct_file(self,
                           file_path : str,
@@ -1060,15 +1275,15 @@
         if file_type == 'dill':
 
             with open(file_path, 'wb') as file:
                 dill.dump(file_content, file)
 
             return True
 
-        if file_type == 'unknown':
+        if file_type == 'other':
 
             with open(file_path, 'wb') as file:
                 file.write(file_content)
 
             return True
 
         return False
@@ -1141,17 +1356,21 @@
         Generates random name that is combionation of color, adjective, noun and 3 digits
         """
         # Sample lists
         colors = ["red", "blue", "green", "yellow", "pink", "silver", "purple", "golden"]
         adjectives = ["fuzzy", "bright", "dark", "shiny", "giant", "tiny", "happy", "sad"]
         nouns = ["toaster", "refrigerator", "microwave", "laptop", "thermostat", "television", "car", "scooter"]
 
+        if seed is None:
+            seed = self.seed
+
         if isinstance(seed, int):
             # Set the seed value
             random.seed(seed)
+            self.seed += 1
 
         # Randomly choose a word from each list
         color = random.choice(colors)
         adj = random.choice(adjectives)
         noun = random.choice(nouns)
         digits = random.randint(100, 999)
         # Combine them to form a name
@@ -1161,15 +1380,15 @@
 
 
 
 
 @attr.s
 class ParameterFrame:
 
-    params_path = attr.ib()
+    params_path = attr.ib(default=None)
 
     # optional
     solution_id = attr.ib(default=None, type=str)
     param_names = attr.ib(default=None, type=dict)
     param_descriptions = attr.ib(default=None, type=dict)
     seed = attr.ib(default=None, type=int)
 
@@ -1178,14 +1397,15 @@
 
     # dependancies
     database_connector = attr.ib(default=None, type=MockerDatabaseConnector)
     file_type_handler = attr.ib(default=FileTypeHandler)
     name_generator = attr.ib(default=ComplexNameGenerator)
 
     # inner
+    seed = attr.ib(default=23, type=int)
     solutions = attr.ib(default={})
     param_sets = attr.ib(default={})
     param_attributes = attr.ib(default={})
 
     commited_tables = attr.ib(default={})
 
 
@@ -1197,17 +1417,25 @@
 
     def __attrs_post_init__(self):
         self._initialize_logger()
 
         if self.database_connector is None:
             self.database_connector = MockerDatabaseConnector(connection_details = self.connection_details)
 
+        self._initialize_name_generator()
+
+        import pandas as pd
 
+        self.pd = pd
+        self.pd.set_option('display.max_colwidth', 70)
 
+        self.solutions = {}
+        self.param_sets = {}
         self.commited_tables = {}
+        self.param_attributes = {}
 
 
     def _initialize_logger(self):
 
         """
         Initialize a logger for the class instance based on the specified logging level and logger name.
         """
@@ -1215,14 +1443,22 @@
         if self.logger is None:
             logging.basicConfig(level=self.loggerLvl, format=self.logger_format)
             logger = logging.getLogger(self.logger_name)
             logger.setLevel(self.loggerLvl)
 
             self.logger = logger
 
+    def _initialize_name_generator(self):
+
+        """
+        Initializing name generator
+        """
+
+        self.name_generator = self.name_generator(seed = self.seed)
+
     def _generate_unique_id(self, txt : str) -> str:
 
         """
         Helper function to generate a unique ID for attribute entries
         """
 
         hash_id = hashlib.sha256(str(txt).encode()).hexdigest()
@@ -1259,14 +1495,16 @@
                 file_path = param_names[param_name],
                 parameter_name = param_name,
                 parameter_description = param_descriptions[param_name]
             )
 
             self.param_attributes[param_name].process_file()
 
+        return True
+
     def make_parameter_set(self,
                            parameter_set_name : str = None,
                            parameter_set_description : str = None,
                            parameter_names : list = None,
                            param_attributes : dict = None,
                            seed : int = None):
 
@@ -1274,15 +1512,15 @@
         Use processed parameters to compose parameter set
         """
 
         if parameter_set_name is None:
 
             if seed is None:
                 seed = self.seed
-            parameter_set_name = self.name_generator().generate_random_name(seed = seed)
+            parameter_set_name = self.name_generator.generate_random_name()
 
         if parameter_set_description is None:
             parameter_set_description = ''
 
         if param_attributes is None:
             param_attributes = self.param_attributes
 
@@ -1303,39 +1541,41 @@
         parameter_set = [{'parameter_set_id' : parameter_set_id,
                                'parameter_id' : parameter_id} for parameter_id in parameter_ids]
 
         # saving parameter set lists
         self.param_sets[parameter_set_name] = {'parameter_set' : parameter_set,
                                                'parameter_set_description' : parameter_set_description}
 
+        self.logger.info(f"Parameter set id for {parameter_set_name}: {parameter_set_id}")
 
-    def add_solution_description(self,
-                                    solution_name : str,
-                                    deployment_date : str = None,
-                                    deprecation_date : str = None,
-                                    solution_description : str = None,
-                                    solution_id : str = None,
-                                    maintainers : list = None):
+
+    def add_solution(self,
+                        solution_name : str,
+                        deployment_date : str = None,
+                        deprecation_date : str = None,
+                        solution_description : str = None,
+                        solution_id : str = None,
+                        maintainers : list = None,
+                        seed : int = None):
 
         """
         Add new solution and its description.
         """
 
-        if solution_id is None:
-            solution_id = self.solution_id
-
+        if seed is None:
+            seed = self.seed
 
         # trim solution name
         solution_name = solution_name[:100]
 
         if solution_id is None:
             # if solution id not provided create new
             solution_id = self._generate_unique_id(
-                txt = self.name_generator().generate_random_name(seed=23) + solution_name)
-
+                txt = self.name_generator.generate_random_name(seed = seed) \
+                    + solution_name)
 
         if solution_name not in self.solutions.keys():
             self.solutions[solution_name] = {}
 
         if 'solution_id' not in self.solutions[solution_name].keys():
             self.solutions[solution_name]['solution_id'] = solution_id
 
@@ -1344,26 +1584,34 @@
             'solution_name' : solution_name,
             'solution_description' : solution_description,
             'deployment_date' : deployment_date,
             'deprecation_date' : deprecation_date,
             'maintainers' : maintainers
         }
 
+        self.logger.info(f"Solution id for {solution_name}: {solution_id}")
+        return True
+
+
+
     def _get_solution_name_from_memory(self, solution_id : str) -> str:
 
         """
         Get solution name from memory from solution id.
         """
 
         try:
-            solution_name = [self.solutions[s]['solution_description']['solution_name'] \
+            solution_name = [self.solutions[s]['solution_id'] \
                 for s in self.solutions \
-                    if self.solutions[s]['solution_description']['solution_id'] == solution_id][0]
+                    if self.solutions[s]['solution_id'] == solution_id][0]
         except Exception as e:
-            raise ValueError(f"{solution_id} is not in solutions saved to memory!")
+            self.logger.warning(f"{solution_id} is not in solutions saved to memory!")
+            solution_name = self.name_generator.generate_random_name()
+            self.logger.warning(f"Name {solution_name} is assigned to {solution_id} temporarily!")
+
 
         return solution_name
 
     def _get_parameter_set_name_from_memory(self, parameter_set_id : str) -> str:
 
         """
         Get parameter set name from memory from parameter set id.
@@ -1430,20 +1678,20 @@
         """
         Add parameter set to solution
         """
 
         if solution_id is None:
             solution_id = self.solution_id
 
-        if solution_id is None:
-            solution_id = self.solutions[solution_name]['solution_id']
-
         if (solution_id is None) and (solution_name is None):
             raise ValueError("Provide either solution_id or solution_name!")
 
+        if solution_id is None:
+            solution_id = self.solutions[solution_name]['solution_id']
+
         if (parameter_set_id is None) and (parameter_set_name is None):
             raise ValueError("Provide either parameter_set_id or parameter_set_name!")
 
         if solution_name is None:
             solution_name = self._get_solution_name_from_memory(solution_id = solution_id)
 
         if (parameter_set_id is not None) and (parameter_set_name is None):
@@ -1453,24 +1701,29 @@
         if (parameter_set_id is None) and (parameter_set_name is not None):
             parameter_set_id = self._get_parameter_set_id_from_memory(
                 parameter_set_name = parameter_set_name)
 
         if solution_name not in self.solutions.keys():
             self.solutions[solution_name] = {}
 
+        if 'solution_id' not in self.solutions[solution_name].keys():
+            self.solutions[solution_name]['solution_id'] = solution_id
+
         if 'solution_parameter_set' not in self.solutions[solution_name].keys():
             self.solutions[solution_name]['solution_parameter_set'] = {}
 
         self.solutions[solution_name]['solution_parameter_set'][parameter_set_name] = {
             'solution_id' : solution_id,
             'parameter_set_id' : parameter_set_id,
             'deployment_status' : "STAGING",
             'insertion_datetime' : datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         }
 
+        return True
+
     def commit_solution(self,
                         solution_id : str = None,
                         solution_name : str = None,
                         parameter_set_ids : list = None,
                         parameter_set_names : list = None):
 
         """
@@ -1490,77 +1743,89 @@
             solution_name = self._get_solution_name_from_memory(solution_id = solution_id)
 
 
         # save solution with param set
         if solution_id not in self.commited_tables.keys():
             self.commited_tables[solution_id] = {}
 
+        solution_description = None
+        if 'solution_description' in self.solutions[solution_name].keys():
+            solution_description = [self.solutions[solution_name]['solution_description']]
+
         ## save solution description
         self.commited_tables[solution_id]= {
-            'solution_description' : [self.solutions[solution_name]['solution_description']],
+            'solution_description' : solution_description,
             'solution_parameter_set' : {},
             'parameter_set' : {},
             'parameter_set_description' : {},
             'parameter_description' : {},
             'parameter_attribute' : {},
             'attribute_values' : {}
         }
 
-        if (parameter_set_ids is not None) and (parameter_set_names is None):
-                parameter_set_names = [self._get_parameter_set_name_from_memory(
-                    parameter_set_id = parameter_set_id) \
-                        for parameter_set_id in parameter_set_ids]
-
-        if (parameter_set_ids is None) and (parameter_set_names is not None):
-            parameter_set_ids = [self._get_parameter_set_id_from_memory(
-                parameter_set_name = parameter_set_name) \
-                    for parameter_set_name in parameter_set_names]
-
-        if (parameter_set_ids is None) and (parameter_set_names is None):
-                raise ValueError("Provide either parameter_set_ids or parameter_set_names!")
-
+        if solution_description:
+            self.logger.info(f"Commited solution description for {solution_id}")
 
-        for parameter_set_id, parameter_set_name in zip(parameter_set_ids, parameter_set_names):
+        if (parameter_set_ids is not None) or (parameter_set_names is not None):
 
-            ## save to solution_parameter_set
-            self.commited_tables[solution_id]['solution_parameter_set'][parameter_set_id] = \
-                [self.solutions[solution_name]['solution_parameter_set'][parameter_set_name]]
-            ## save to parameter_set
-            self.commited_tables[solution_id]['parameter_set'][parameter_set_id] = \
-                self.param_sets[parameter_set_name]['parameter_set']
-            ## save to parameter_set_description
-            self.commited_tables[solution_id]['parameter_set_description'][parameter_set_id] = \
-                self.param_sets[parameter_set_name]['parameter_set_description']
-            ## save to parameter_description
-            for parameter_set in self.param_sets[parameter_set_name]['parameter_set']:
-
-                parameter_id = parameter_set['parameter_id']
-
-                parameter_name = [self.param_attributes[param_name].parameter_name \
-                    for param_name in self.param_attributes \
-                        if self.param_attributes[param_name].parameter_id == parameter_id][0]
-
-                # saving parameter descriptions
-                if parameter_set_id not in self.commited_tables[solution_id]['parameter_description'].keys():
-                    self.commited_tables[solution_id]['parameter_description'][parameter_set_id] = {}
-                self.commited_tables[solution_id]['parameter_description'][parameter_set_id][parameter_id] = \
-                    self.param_attributes[parameter_name].parameter_description
+            if (parameter_set_ids is not None) and (parameter_set_names is None):
+                    parameter_set_names = [self._get_parameter_set_name_from_memory(
+                        parameter_set_id = parameter_set_id) \
+                            for parameter_set_id in parameter_set_ids]
+
+            if (parameter_set_ids is None) and (parameter_set_names is not None):
+                parameter_set_ids = [self._get_parameter_set_id_from_memory(
+                    parameter_set_name = parameter_set_name) \
+                        for parameter_set_name in parameter_set_names]
+
+            if (parameter_set_ids is None) and (parameter_set_names is None):
+                    raise ValueError("Provide either parameter_set_ids or parameter_set_names!")
+
+
+            for parameter_set_id, parameter_set_name in zip(parameter_set_ids, parameter_set_names):
+
+                ## save to solution_parameter_set
+                self.commited_tables[solution_id]['solution_parameter_set'][parameter_set_id] = \
+                    [self.solutions[solution_name]['solution_parameter_set'][parameter_set_name]]
+                ## save to parameter_set
+                self.commited_tables[solution_id]['parameter_set'][parameter_set_id] = \
+                    self.param_sets[parameter_set_name]['parameter_set']
+                ## save to parameter_set_description
+                self.commited_tables[solution_id]['parameter_set_description'][parameter_set_id] = \
+                    self.param_sets[parameter_set_name]['parameter_set_description']
+                ## save to parameter_description
+                for parameter_set in self.param_sets[parameter_set_name]['parameter_set']:
+
+                    parameter_id = parameter_set['parameter_id']
+
+                    parameter_name = [self.param_attributes[param_name].parameter_name \
+                        for param_name in self.param_attributes \
+                            if self.param_attributes[param_name].parameter_id == parameter_id][0]
+
+                    # saving parameter descriptions
+                    if parameter_set_id not in self.commited_tables[solution_id]['parameter_description'].keys():
+                        self.commited_tables[solution_id]['parameter_description'][parameter_set_id] = {}
+                    self.commited_tables[solution_id]['parameter_description'][parameter_set_id][parameter_id] = \
+                        self.param_attributes[parameter_name].parameter_description
+
+                    # saving parameter attributes list
+                    if parameter_set_id not in self.commited_tables[solution_id]['parameter_attribute'].keys():
+                        self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id] = {}
+                    self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id][parameter_id] = \
+                        self.param_attributes[parameter_name].parameter_attributes_list
+
+                    # saving attribute values
+                    if parameter_set_id not in self.commited_tables[solution_id]['attribute_values'].keys():
+                        self.commited_tables[solution_id]['attribute_values'][parameter_set_id] = {}
+                    self.commited_tables[solution_id]['attribute_values'][parameter_set_id][parameter_id] = \
+                        self.param_attributes[parameter_name].attribute_values_list
 
-                # saving parameter attributes list
-                if parameter_set_id not in self.commited_tables[solution_id]['parameter_attribute'].keys():
-                    self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id] = {}
-                self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id][parameter_id] = \
-                    self.param_attributes[parameter_name].parameter_attributes_list
-
-                # saving attribute values
-                if parameter_set_id not in self.commited_tables[solution_id]['attribute_values'].keys():
-                    self.commited_tables[solution_id]['attribute_values'][parameter_set_id] = {}
-                self.commited_tables[solution_id]['attribute_values'][parameter_set_id][parameter_id] = \
-                    self.param_attributes[parameter_name].attribute_values_list
+                self.logger.info(f"Commited solution tables for {solution_id}")
 
+        return True
 
     def _prep_ps_for_reconstruction(self,
                                  solution_id : str,
                                  parameter_set_id : str) -> tuple:
 
         """
         Prepares data for reconstruction from selected solutio and param set ids.
@@ -1662,15 +1927,15 @@
             attribute_values_list = attribute_values_list,
             param_id_paths = param_id_paths,
             params_path = params_path
         )
 
     def _prep_tables_for_pushing(self,
                                  solution_id : str,
-                                 parameter_set_ids : list):
+                                 parameter_set_ids : list = None):
 
         """
         Prepare tables for pushing selected solution
         """
 
         solution_parameter_set = []
         parameter_set = []
@@ -1679,67 +1944,80 @@
         parameter_attribute = []
         attribute_values = []
 
         try:
 
             solution_description = self.commited_tables[solution_id]['solution_description']
             ##
-            for parameter_set_id in parameter_set_ids:
 
-                solution_parameter_set = solution_parameter_set + \
-                    self.commited_tables[solution_id]['solution_parameter_set'][parameter_set_id]
-                parameter_set = parameter_set + \
-                    self.commited_tables[solution_id]['parameter_set'][parameter_set_id]
-                parameter_set_description = parameter_set_description + \
-                    self.commited_tables[solution_id]['parameter_set_description'][parameter_set_id]
-
-                parameter_description_dict = self.commited_tables[solution_id]['parameter_description'][parameter_set_id]
-                parameter_description = parameter_description + \
-                    [item for sublist in parameter_description_dict.values() for item in sublist]
-
-                parameter_attribute_dict = self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id]
-                parameter_attribute = parameter_attribute + \
-                    [item for sublist in parameter_attribute_dict.values() for item in sublist]
-
-                attribute_values_dict = self.commited_tables[solution_id]['attribute_values'][parameter_set_id]
-                attribute_values = attribute_values + \
-                    [item for sublist in attribute_values_dict.values() for item in sublist]
+            if parameter_set_ids:
+                for parameter_set_id in parameter_set_ids:
+
+                    solution_parameter_set = solution_parameter_set + \
+                        self.commited_tables[solution_id]['solution_parameter_set'][parameter_set_id]
+                    parameter_set = parameter_set + \
+                        self.commited_tables[solution_id]['parameter_set'][parameter_set_id]
+                    parameter_set_description = parameter_set_description + \
+                        self.commited_tables[solution_id]['parameter_set_description'][parameter_set_id]
+
+                    parameter_description_dict = self.commited_tables[solution_id]['parameter_description'][parameter_set_id]
+                    parameter_description = parameter_description + \
+                        [item for sublist in parameter_description_dict.values() for item in sublist]
+
+                    parameter_attribute_dict = self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id]
+                    parameter_attribute = parameter_attribute + \
+                        [item for sublist in parameter_attribute_dict.values() for item in sublist]
+
+                    attribute_values_dict = self.commited_tables[solution_id]['attribute_values'][parameter_set_id]
+                    attribute_values = attribute_values + \
+                        [item for sublist in attribute_values_dict.values() for item in sublist]
+
+                    return (solution_description,
+                            solution_parameter_set,
+                            parameter_set,
+                            parameter_set_description,
+                            parameter_description,
+                            parameter_attribute,
+                            attribute_values)
 
         except Exception as e:
             self.logger.error("Problem during preparation of tables for pushing!")
             raise e
 
-        return (solution_description,
-                solution_parameter_set,
-                parameter_set,
-                parameter_set_description,
-                parameter_description,
-                parameter_attribute,
-                attribute_values)
+        return solution_description
 
     def push_solution(self,
                       solution_id : list = None,
                       solution_name : list = None,
                       parameter_set_ids : list = None,
                       parameter_set_names : list = None,):
 
         """
         Pushes commited tables to database handler for selected solutions
         """
 
         if (solution_id is None) and (solution_name is None):
             raise ValueError("Provide either solution_ids or solution_names!")
 
-        if (parameter_set_ids is None) and (parameter_set_names is None):
-            raise ValueError("Provide either parameter_set_ids or parameter_set_names!")
-
         if solution_id is None:
             solution_id = [id for id, dd in self.commited_tables.items() \
                 if dd['solution_description'][0]['solution_name'] == solution_name][0]
 
+        if (parameter_set_ids is None) and (parameter_set_names is None):
+            solution_description = self._prep_tables_for_pushing(
+                solution_id = solution_id
+            )
+
+            self.database_connector.push_tables(
+                solution_description = solution_description
+            )
+
+            return True
+
+
         if parameter_set_ids is None:
             parameter_set_ids = [id for id, dd in self.commited_tables[solution_id]['parameter_set_description'].items() \
                 if dd[0]['parameter_set_name'] in parameter_set_names]
 
 
         (solution_description,
             solution_parameter_set,
@@ -1801,18 +2079,18 @@
             if 'parameter_attribute' not in self.commited_tables[solution_id].keys():
                 self.commited_tables[solution_id]['parameter_attribute'] = {}
             if 'attribute_values' not in self.commited_tables[solution_id].keys():
                 self.commited_tables[solution_id]['attribute_values'] = {}
 
             # Calculate distribution counts for each list based on the number of parameter_set_ids
             num_ids = len(parameter_set_ids)
-            sps_count = len(solution_parameter_sets) // num_ids
-            ps_count = len(parameter_sets) // num_ids
-            psd_count = len(parameter_set_descriptions) // num_ids
-            pd_count = len(parameter_descriptions) // num_ids
+            sps_count = len(solution_parameter_sets)
+            ps_count = len(parameter_sets)
+            psd_count = len(parameter_set_descriptions)
+            pd_count = len(parameter_descriptions)
             # pa_count = len(parameter_attributes) // num_ids
             # av_count = len(attribute_values) // num_ids
 
             # Iterators for each type of data
             sps_iter = iter(solution_parameter_sets)
             ps_iter = iter(parameter_sets)
             psd_iter = iter(parameter_set_descriptions)
@@ -1864,58 +2142,66 @@
         except Exception as e:
             self.logger.error("Problem during rebuilding of tables from pushed data!")
             raise e
 
 
 
     def pull_solution(self,
-                      solution_id : list = None,
-                      parameter_set_id : list = None):
+                      solution_id : str = None,
+                      parameter_set_id : str = None):
 
         """
         Pulls commited tables from database for selected solutions
         """
 
         if solution_id is None:
             raise ValueError("Provide solution_id!")
 
-        if parameter_set_id is None:
-            raise ValueError("Provide parameter_set_id!")
 
         (solution_description,
          solution_parameter_sets,
          parameter_sets,
          parameter_set_descriptions,
          parameter_descriptions,
          parameter_attributes,
          attribute_values) = self.database_connector.pull_tables(
             solution_id = solution_id,
             parameter_set_id = parameter_set_id
         )
 
+        if len(solution_description) == 0:
+            self.logger.warning(f"No solutions with {solution_id} could be pulled!")
+
+        parameter_set_ids = [solution_parameter_set['parameter_set_id'] for solution_parameter_set in solution_parameter_sets]
+
+        if len(parameter_set_ids) == 0:
+            self.logger.warning(f"No parameter sets were pulled for solution_id {solution_id}")
+
         # get table lists into commited
         self._rebuild_tables_from_pulled_data(
             solution_id = solution_id,
-            parameter_set_ids = [parameter_set_id],
+            parameter_set_ids = parameter_set_ids,
             solution_description = solution_description,
             solution_parameter_sets = solution_parameter_sets,
             parameter_sets = parameter_sets,
             parameter_set_descriptions = parameter_set_descriptions,
             parameter_descriptions = parameter_descriptions,
             parameter_attributes = parameter_attributes,
             attribute_values = attribute_values
         )
 
+        return True
+
     def _change_deployment_status(self,
                                  deployment_status : str,
                                  solution_id : str = None,
                                 solution_name : str = None,
                                 parameter_set_id : str = None,
                                 parameter_set_name : str = None,
-                                remote : bool = False):
+                                remote : bool = True):
 
         """
         Change deployment status of parameter set.
         """
 
         if solution_id is None:
             solution_id = self.solution_id
@@ -1940,107 +2226,182 @@
             if (parameter_set_id is None) and (parameter_set_name is not None):
                 parameter_set_id = self._get_parameter_set_id_from_memory(
                     parameter_set_name = parameter_set_name)
 
             self.solutions[solution_name]['solution_parameter_set']\
                 [parameter_set_name]['deployment_status'] = deployment_status
 
-    def get_deployment_status(self,
-                                 solution_id : str = None,
-                                solution_name : str = None,
-                                parameter_set_id : str = None,
-                                parameter_set_name : str = None,
-                                remote : bool = False):
+    def get_parameter_set_id_for_solution(self,
+                                          solution_id : str = None,
+                                          deployment_status : str = None):
 
         """
-        Get deployment status of parameter set.
+        Get parameter set id/s for solution id with select deployment status.
         """
 
-        if solution_id is None:
-            solution_id = self.solution_id
+        tabs = self.database_connector.get_parameter_sets_info(
+            solution_id=solution_id,
+            deployment_status=deployment_status)
 
-        if (solution_id is None) and (solution_name is None):
-            raise ValueError("Provide either solution_id or solution_name!")
+        parameter_set_ids = [t['parameter_set_id'] for t in tabs]
 
-        if (parameter_set_id is None) and (parameter_set_name is None):
-            raise ValueError("Provide either parameter_set_id or parameter_set_name!")
+        return parameter_set_ids
 
-        if remote:
-            raise Exception("Connection with parameter storage was not established!")
-        else:
+    def get_deployment_status(self,
+                                 solution_id : str = None,
+                                parameter_set_id : str = None):
 
-            if solution_name is None:
-                solution_name = self._get_solution_name_from_memory(solution_id = solution_id)
+        """
+        Get deployment status of parameter set.
+        """
 
-            if (parameter_set_id is not None) and (parameter_set_name is None):
-                parameter_set_name = self._get_parameter_set_name_from_memory(
-                    parameter_set_id = parameter_set_id)
+        tabs = self.database_connector.get_parameter_sets_info(
+            solution_id=solution_id,
+            parameter_set_ids=parameter_set_id)
 
-            if (parameter_set_id is None) and (parameter_set_name is not None):
-                parameter_set_id = self._get_parameter_set_id_from_memory(
-                    parameter_set_name = parameter_set_name)
+        return [t['deployment_status'] for t in tabs][0]
 
-            return self.solutions[solution_name]['solution_parameter_set']\
-                [parameter_set_name]['deployment_status']
 
     def change_status_from_staging_to_production(self,
                                                  solution_id : str = None,
-                                                solution_name : str = None,
-                                                parameter_set_id : str = None,
-                                                parameter_set_name : str = None,
-                                                remote : bool = False):
+                                                parameter_set_id : str = None):
 
         """
         Change deployment status of parameter set from staging to production.
         """
 
-        current_deployment_status = self.get_deployment_status(
-            solution_id = solution_id,
-            solution_name = solution_name,
-            parameter_set_id = parameter_set_id,
-            parameter_set_name = parameter_set_name,
-            remote = remote
-        )
-
-        if current_deployment_status != "STAGING":
-            raise Exception(f"Current deployment status is {current_deployment_status}!")
+        self.database_connector.modify_parameter_set_status(
+                solution_id=solution_id,
+                parameter_set_ids = parameter_set_id,
+                current_deployment_status = "STAGING",
+                new_deployment_status = "PRODUCTION"
+            )
 
-        self._change_deployment_status(
-            deployment_status = "PRODUCTION",
-            solution_id = solution_id,
-            solution_name = solution_name,
-            parameter_set_id = parameter_set_id,
-            parameter_set_name = parameter_set_name,
-            remote = remote
-        )
 
     def change_status_from_production_to_archived(self,
                                                  solution_id : str = None,
-                                                solution_name : str = None,
-                                                parameter_set_id : str = None,
-                                                parameter_set_name : str = None,
-                                                remote : bool = False):
+                                                parameter_set_id : str = None):
 
         """
         Change deployment status of parameter set from production to archived.
         """
 
-        current_deployment_status = self.get_deployment_status(
-            solution_id = solution_id,
-            solution_name = solution_name,
-            parameter_set_id = parameter_set_id,
-            parameter_set_name = parameter_set_name,
-            remote = remote
-        )
+        self.database_connector.modify_parameter_set_status(
+                solution_id=solution_id,
+                parameter_set_ids = parameter_set_id,
+                current_deployment_status = "PRODUCTION",
+                new_deployment_status = "ARCHIVED"
+            )
+
+
+    def change_status_from_archived_production(self,
+                                                solution_id : str = None,
+                                                parameter_set_id : str = None):
+
+        """
+        Change deployment status of parameter set from archived to production.
+        """
+
+        self.database_connector.modify_parameter_set_status(
+                solution_id=solution_id,
+                parameter_set_ids = None,
+                current_deployment_status = "PRODUCTION",
+                new_deployment_status = "STAGING"
+            )
+
+        self.database_connector.modify_parameter_set_status(
+                solution_id=solution_id,
+                parameter_set_ids = parameter_set_id,
+                current_deployment_status = "ARCHIVED",
+                new_deployment_status = "PRODUCTION"
+            )
+
+    def show_solutions(self):
+
+        """
+        Show info on locally commited solutions
+        """
+
+        solution_descriptions = [self.commited_tables[sid]['solution_description'][0] \
+             if self.commited_tables[sid]['solution_description'] else {'solution_id' : sid} for sid in self.commited_tables]
+
+        for solution_description in solution_descriptions:
+
+            if 'solution_name' not in solution_description.keys():
+                solution_description['solution_name'] = None
+                solution_description['solution_description'] = None
+                solution_description['deployment_date'] = None
+                solution_description['deprecation_date'] = None
+                solution_description['maintainers'] = None
+
+
+        solution_descriptions_pd = self.pd.DataFrame(solution_descriptions)
+
+        if solution_descriptions_pd.shape[0] == 0:
+            solution_descriptions_pd['solution_id'] = [sid for sid in self.commited_tables]
+            solution_descriptions_pd['solution_name'] = [None for sid in self.commited_tables]
+            solution_descriptions_pd['solution_description'] = [None for sid in self.commited_tables]
+            solution_descriptions_pd['deployment_date'] = [None for sid in self.commited_tables]
+            solution_descriptions_pd['deprecation_date'] = [None for sid in self.commited_tables]
+            solution_descriptions_pd['maintainers'] = [None for sid in self.commited_tables]
+
+        solution_descriptions_pd['commited_parameter_sets'] = [
+                    len(self.commited_tables[sid]['solution_parameter_set']) \
+                    if self.commited_tables[sid]['solution_parameter_set'] != {}\
+                    else 0
+                    for sid in self.commited_tables
+                ]
+
+        return solution_descriptions_pd
+
+    def show_parameter_sets(self, solution_id : str):
+
+        """
+        Show info on locally commited parameter_sets for solution_id
+        """
+
+
+        solution_parameter_sets = [
+            sps for spsid in self.commited_tables[solution_id]['solution_parameter_set'] \
+                for sps in self.commited_tables[solution_id]['solution_parameter_set'][spsid]]
+        solution_parameter_sets_pd = self.pd.DataFrame(solution_parameter_sets)
+
+        if solution_parameter_sets_pd.shape[0] == 0:
+            raise ValueError(f"Solution with id {solution_id} does not exist locally!")
+
+        solution_parameter_sets_pd = solution_parameter_sets_pd.drop(columns=["solution_id"])
+
+        parameter_set_descriptions = [
+            sps for spsid in self.commited_tables[solution_id]['parameter_set_description'] \
+                for sps in self.commited_tables[solution_id]['parameter_set_description'][spsid]]
+        parameter_set_descriptions_pd = self.pd.DataFrame(parameter_set_descriptions)
+
+
+        psdsp_id_pd = parameter_set_descriptions_pd.merge(
+            solution_parameter_sets_pd, on = 'parameter_set_id')
+        psdsp_id_pd['commited_parameters'] = [
+            len(self.commited_tables[solution_id]['parameter_set'][pid_d['parameter_set_id']]) \
+                for pid_d in parameter_set_descriptions]
+
+        return psdsp_id_pd
+
+    def show_parameters(self, solution_id : str, parameter_set_id : str):
+
+        """
+        Show info on locally commited parameters for solution_id and parameter_set_id
+        """
+
+        if parameter_set_id not in self.commited_tables[solution_id]['parameter_description']:
+            raise ValueError(f"Parameter set with id {parameter_set_id} does not exist locally for solution {solution_id}!")
+
+        parameter_descriptions = self.commited_tables[solution_id]['parameter_description'][parameter_set_id]
+        parameter_descriptions_l = [parameter_descriptions[pid][0] for pid in parameter_descriptions]
+        parameter_descriptions_pd = self.pd.DataFrame(parameter_descriptions_l)
+        parameter_descriptions_pd['commited_attributes'] = [
+            len(self.commited_tables[solution_id]['parameter_attribute'][parameter_set_id][parameter_id]) \
+                for parameter_id in parameter_descriptions]
+        return parameter_descriptions_pd
+
+
 
-        if current_deployment_status != "PRODUCTION":
-            raise Exception(f"Current deployment status is {current_deployment_status}!")
 
-        self._change_deployment_status(
-            deployment_status = "ARCHIVED",
-            solution_id = solution_id,
-            solution_name = solution_name,
-            parameter_set_id = parameter_set_id,
-            parameter_set_name = parameter_set_name,
-            remote = remote
-        )
```

### Comparing `parameterframe-0.0.3/parameterframe/setup.py` & `parameterframe-0.1.1/parameterframe/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="parameterframe",
     packages=["parameterframe"],
-    install_requires=['### parameterframe.py', 'mocker_db==0.1.1', 'pyyaml', 'attrs', 'dill', 'sqlalchemy'],
+    install_requires=['### parameterframe.py', 'attrs', 'sqlalchemy', 'mocker_db==0.1.1', 'dill', 'pyyaml'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.0.3"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.1.1"
 )
```

