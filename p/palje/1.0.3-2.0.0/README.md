# Comparing `tmp/palje-1.0.3-py3-none-any.whl.zip` & `tmp/palje-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 18666 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      131 b- defN 21-Feb-12 10:47 palje/__init__.py
--rw-rw-rw-  2.0 fat     9730 b- defN 21-Feb-12 10:47 palje/__main__.py
--rw-rw-rw-  2.0 fat     6820 b- defN 21-Feb-12 10:47 palje/confluence_rest.py
--rw-rw-rw-  2.0 fat     9716 b- defN 21-Feb-12 10:47 palje/mssql_database.py
--rw-rw-rw-  2.0 fat     4434 b- defN 21-Feb-18 13:55 palje/storage_format.py
--rw-rw-rw-  2.0 fat      147 b- defN 21-Mar-31 10:10 palje/version.py
--rw-rw-rw-  2.0 fat    10126 b- defN 21-Mar-31 10:07 palje/queries/database_queries.ini
--rw-rw-rw-  2.0 fat    11556 b- defN 21-Mar-31 10:10 palje-1.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7445 b- defN 21-Mar-31 10:10 palje-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 21-Mar-31 10:10 palje-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 21-Mar-31 10:10 palje-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      928 b- defN 21-Mar-31 10:10 palje-1.0.3.dist-info/RECORD
-12 files, 61131 bytes uncompressed, 17126 bytes compressed:  72.0%
+Zip file size: 23804 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      131 b- defN 24-Apr-12 06:36 palje/__init__.py
+-rw-rw-rw-  2.0 fat    10408 b- defN 24-May-06 13:39 palje/__main__.py
+-rw-rw-rw-  2.0 fat     7152 b- defN 24-May-06 13:39 palje/confluence_rest.py
+-rw-rw-rw-  2.0 fat    10947 b- defN 24-Apr-16 13:53 palje/mssql_database.py
+-rw-rw-rw-  2.0 fat     4256 b- defN 24-May-06 13:39 palje/storage_format.py
+-rw-rw-rw-  2.0 fat      427 b- defN 24-May-07 07:15 palje/version.py
+-rw-rw-rw-  2.0 fat    10126 b- defN 24-Apr-12 06:36 palje/queries/database_queries.ini
+-rw-rw-rw-  2.0 fat    11556 b- defN 24-May-07 07:15 palje-2.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    21369 b- defN 24-May-07 07:15 palje-2.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 07:15 palje-2.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       46 b- defN 24-May-07 07:15 palje-2.0.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-07 07:15 palje-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1024 b- defN 24-May-07 07:15 palje-2.0.0.dist-info/RECORD
+13 files, 77540 bytes uncompressed, 22112 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -15,23 +15,26 @@
 
 Filename: palje/version.py
 Comment: 
 
 Filename: palje/queries/database_queries.ini
 Comment: 
 
-Filename: palje-1.0.3.dist-info/LICENSE
+Filename: palje-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: palje-1.0.3.dist-info/METADATA
+Filename: palje-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: palje-1.0.3.dist-info/WHEEL
+Filename: palje-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: palje-1.0.3.dist-info/top_level.txt
+Filename: palje-2.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: palje-1.0.3.dist-info/RECORD
+Filename: palje-2.0.0.dist-info/top_level.txt
+Comment: 
+
+Filename: palje-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## palje/__main__.py

```diff
@@ -7,34 +7,39 @@
 from argparse import ArgumentParser
 
 from . import storage_format
 from .confluence_rest import ConfluenceREST
 from .mssql_database import MSSQLDatabase, DATABASE_OBJECT_TYPES
 
 
-def main(argv):
-    global WIKI, DB, SPACE
+def main(argv: list[str] | None = None):
+    global WIKI, DB, SPACE, space_id
     # TODO: possibility to read params from config?
-    confluence_url, SPACE, parent_page, server, database, schema_filter, database_filter, driver = parse_arguments(argv)
+    (confluence_url, SPACE, parent_page, server, database,
+        schema_filter, database_filter, driver, authentication) = parse_arguments(argv)
     # ============ DATABASE CONNECTION ============
-    DB = MSSQLDatabase(server, database, driver)
+    DB = MSSQLDatabase(server, database, driver, authentication)
     DB.connect()
     # =========== CONFLUENCE CONNECTION ===========
     WIKI = ConfluenceREST(confluence_url)
-    WIKI.login()
+    WIKI.verify_credentials()
+    space_id = WIKI.get_space_id(SPACE)
+    if not space_id:
+        print(f'Failed to retrieve the id of space {SPACE}. Aborting.')
+        quit()
     # ============ SCHEMAS TO DOCUMENT ============
     schemas = collect_schemas_to_document(schema_filter)
     # ==== DATABASES WHERE TO SEEK DEPENDENCIES ===
     dep_databases = collect_databases_to_query_dependencies(database_filter)
     print("--------------------------")
-    print(
-        f"Object dependencies are queried from the following databases: {', '.join(dep_databases)}")
+    print(f"Object dependencies are queried from the following databases: " +
+          f"{', '.join(dep_databases)}")
     print("--------------------------")
     # ================= ROOT PAGE =================
-    root_page_id = create_and_update_root_page(parent_page)
+    root_page_id = create_or_update_root_page(space_id, parent_page)
     # ================ OTHER PAGES ================
     for schema in schemas:
         schema_page_id = create_and_update_schema_page(root_page_id, schema)
         objects = collect_objects_to_document(schema)
         for object_type in objects:
             type_page_id = create_and_update_object_type_page(
                 schema_page_id, schema, object_type)
@@ -58,24 +63,28 @@
                         help='Name of the database that is documented.')
     parser.add_argument('--schemas', nargs='+',
                         help='Names of the schemas that are documented. If not given, all schemas will be documented.')
     parser.add_argument('--dependent', nargs='+',
                         help='Names of the databases, where object dependencies are sought. If not given, dependencies are sought only in documented database.')
     parser.add_argument('--db-driver', default="ODBC Driver 17 for SQL Server",
                         help='Name of the database driver.')
+    parser.add_argument('--authentication', default="SQL",
+                        help='Authentication method to database. If not provided, SQL authentication is used. Other options are "Windows" (Windwos authentication will be used) \
+                             and "AAD" (Azure Active Directory login will be prompted) ')
     args = vars(parser.parse_args(args))
     return (
         args.get('confluence-url'),
         args.get('space'),
         args.get('parent_page'),
         args.get('server'),
         args.get('database'),
         args.get('schemas'),
         args.get('dependent'),
-        args.get('db_driver', 'ODBC Driver 17 for SQL Server')
+        args.get('db_driver', 'ODBC Driver 17 for SQL Server'),
+        args.get('authentication', 'SQL')
     )
 
 
 def collect_schemas_to_document(schema_filter):
     """If documented schemas not given,
     document all schemas.
     """
@@ -117,85 +126,95 @@
             objects[o_type].append(o['name'])
         except:
             objects[o_type] = []
             objects[o_type].append(o['name'])
     return objects
 
 
-def create_and_update_root_page(parent_page):
-    """If parent page given, parent page is the root page.
-    If root page exists, update it.
-    Else, create the root page.
-    """
-    root_page_content = storage_format.objects_list()
-    if parent_page:
-        root_page_name = parent_page
-    else:
-        root_page_name = 'DATABASE: ' + DB.database
-    root_page_id = WIKI.get_page_id(SPACE, root_page_name)
-    if root_page_id:
-        WIKI.update_page(root_page_id, root_page_name, root_page_content)
-    else:
-        WIKI.new_page(SPACE, root_page_name, root_page_content)
-        root_page_id = WIKI.get_page_id(SPACE, root_page_name)
-    return root_page_id
+def create_or_update_root_page(space_id, page_name=None):
+    """Create or update the root page of the documentation.
+
+    If a page name is given, that will be used as the name of the root
+    page. If no name is given, the default name 'DATABASE: <name-of-db>'
+    is used.
+
+    If a page already exists with the page name it and it's children
+    will be updated, otherwise new pages will be created.
+    """
+    default_page_name = 'DATABASE: ' + DB.database
+    page_content = storage_format.objects_list()
+    page_id = None
+
+    if not page_name:
+        page_name = default_page_name
+
+    page_id = WIKI.get_page_id(space_id, page_name)
+
+    if page_id:
+        WIKI.update_page(page_id, page_name, page_content)
+    else:
+        page_id = WIKI.new_page(space_id, page_name, page_content)
+    return page_id
 
 
 def create_and_update_schema_page(root_page_id, schema):
     """First, get schema description.
     Second, check that schema page exists.
     If page exists, update it.
     Else, create schema page under root page.
     """
+    schema_page_name = DB.database + '.' + schema
     description = DB.get_schema_description(schema)
     schema_page_content = storage_format.description_header(description) + \
         storage_format.objects_list()
-    # check schema page existence and update page
-    schema_page_name = DB.database + '.' + schema
-    schema_page_id = WIKI.get_page_id(SPACE, schema_page_name)
+
+    schema_page_id = WIKI.get_page_id(space_id, schema_page_name)
     if schema_page_id:
         WIKI.update_page(schema_page_id, schema_page_name, schema_page_content)
     else:
-        WIKI.new_page(SPACE, schema_page_name,
-                      schema_page_content, root_page_id)
-        schema_page_id = WIKI.get_page_id(SPACE, schema_page_name)
+        schema_page_id = WIKI.new_page(
+            space_id, schema_page_name, schema_page_content, root_page_id)
+
     return schema_page_id
 
 
 def create_and_update_object_type_page(schema_page_id, schema, object_type):
     """First, check that object type page exists.
     If page exists, update it.
     Else, create object type page under schema page.
     """
     type_page_name = object_type + ' ' + DB.database + '.' + schema
     type_page_content = storage_format.objects_list()
-    type_page_id = WIKI.get_page_id(SPACE, type_page_name)
+
+    type_page_id = WIKI.get_page_id(space_id, type_page_name)
     if type_page_id:
         WIKI.update_page(type_page_id, type_page_name, type_page_content)
     else:
-        WIKI.new_page(SPACE, type_page_name, type_page_content, schema_page_id)
-        type_page_id = WIKI.get_page_id(SPACE, type_page_name)
+        type_page_id = WIKI.new_page(
+            space_id, type_page_name, type_page_content, schema_page_id)
     return type_page_id
 
 
-def create_and_update_object_page(type_page_id, schema, object_type, object_name, dep_databases):
+def create_and_update_object_page(
+        type_page_id, schema, object_type, object_name, dep_databases):
     """First, create object page content.
     Second, check that object page exist.
     If page exists, update it.
     Else, create object page under object type page.
     """
     object_page_title = DB.database + '.' + schema + '.' + object_name
     object_page_content = create_object_page_content(
         schema, object_type, object_name, dep_databases)
-    object_page_id = WIKI.get_page_id(SPACE, object_page_title)
+
+    object_page_id = WIKI.get_page_id(space_id, object_page_title)
     if object_page_id:
         WIKI.update_page(object_page_id, object_page_title,
                          object_page_content, parent_id=type_page_id)
     else:
-        WIKI.new_page(SPACE, object_page_title,
+        WIKI.new_page(space_id, object_page_title,
                       object_page_content, parent_id=type_page_id)
 
 
 def create_object_page_content(schema, object_type, object_name, dep_databases):
     """Object page consists of
     - Header with object description
     - For tables and views, HTML table listing
```

## palje/confluence_rest.py

```diff
@@ -1,181 +1,216 @@
 # Palje - Document MSSQL databases to Confluence wiki
 #
 # Copyright 2021 ALM Partners Oy
 # SPDX-License-Identifier: Apache-2.0
 
 import getpass
 import json
-from urllib.parse import urljoin, urlparse
+from urllib.parse import urljoin
 
 from requests import get, post, put
 from requests.exceptions import HTTPError
 
 HEADERS = {"Content-type": "application/json"}
 
 class ConfluenceREST:
     '''Class for confluence REST API tools.
 
     Arguments
     ---------
-    content_url
-        URL to Confluence REST content.
-        The form is https://yourconfluence.atlassian.net/wiki/rest/api/content.
+    atlassian_url
+        URL to Atlassian root page. The form is
+        https://<yourconfluence>.atlassian.net/.
 
     Attributes
     ----------
     name
-        Network location part from content_url.
+        Network location part from atlassian_url.
         Empty if not present.
     headers
         HTTP header to a request.
     auth
         Authentication tuple to a request.
     '''
 
-    def __init__(self, content_url):
-        self.content_url = content_url
-        self.name = self._get_confluence_name()
+    def __init__(self, atlassian_url):
+        self.wiki_root_url = urljoin(atlassian_url, 'wiki/')
+        self.name = atlassian_url
         self.headers = HEADERS
         self.auth = ''
 
-    def _get_confluence_name(self):
-        parsed = urlparse(self.content_url)
-        return parsed[1]
-
-    def login(self):
-        '''Add the authentication tuple to an instance.
-        Ask user for an username and password.
-        Verify that the login with auth is successful.
-        If login fails - quit.
+    def verify_credentials(self):
+        '''Ask for credentials and check that they work.
+
+        Ask the user for a username and API token for Confluence. Verify
+        that the credentials work by sending a request to the wiki's
+        root url. Quit palje if the login fails.
         '''
         uid = input(f"Confluence user for {self.name}: ")
-        password = getpass.getpass(f"Password for user {uid}: ")
+        password = getpass.getpass(f"Atlassian API token for user {uid}: ")
         self.auth = (uid, password)
-        # verify username and password
-        url = urljoin(self.content_url, '.')
         try:
-            r = get(urljoin(url, 'space'), auth=self.auth)
-            r.raise_for_status()
+            response = get(self.wiki_root_url, auth=self.auth)
+            response.raise_for_status()
             return True
-        except:
-            print(f'Failed to login into Confluence {self.name}. Check your username, password and Confluence URL.')
+        except Exception as err:
+            print(err)
+            print(f'Failed to login into Confluence {self.name}.' +
+                  f' Check your username, password and Confluence URL.')
             quit()
 
-    def get_page_id(self, space_key, page_title):
-        '''Return the id of page. Return value is None if no page found.
-        Notice that the name or title of the page is unique inside a space.
+    def get_space_id(self, space_key):
+        '''Return the id of the space or None.
 
         Arguments
         ---------
         space_key
-            The space key of the page.
+            The key of the space.
+        '''
+        url = urljoin(self.wiki_root_url, 'api/v2/spaces')
+        response = get(
+            url,
+            params={'keys': [space_key]},
+            auth=self.auth)
+        response.raise_for_status()
+        if results := response.json()['results']:
+            return results[0]['id']
+        return None
+
+    def get_page_id(self, space_id, page_title):
+        '''Return the id of the page or None if no page is found.
+
+        Page titles are unique inside a space.
+
+        Arguments
+        ---------
+        space_id
+            The id of the space the page is in.
         page_title
             The title of the page.
         '''
-        r = get(self.content_url,
-                            params={'title': page_title,
-                                    'spaceKey': space_key},
-                            auth=self.auth)
+        url = urljoin(self.wiki_root_url, 'api/v2/pages')
+        response = get(
+            url,
+            params={
+                'title': page_title,
+                'space-id': [space_id]},
+            auth=self.auth)
         try:
-            r.raise_for_status()
-            page_by_title = r.json()
-            if page_by_title.get('results'):
-                page_id = page_by_title['results'][0]['id']
-                return page_id
+            response.raise_for_status()
+            if results := response.json()['results']:
+                return results[0]['id']
             return None
         except HTTPError as err:
             print(f'Failed to retrieve the id of the page {page_title}.')
             print(f'Response: {err.response.text}')
             return None
 
-    def new_page(self, space_key, page_title, page_content, parent_id=None):
+    def new_page(self, space_id, page_title, page_content, parent_id=None):
         '''Create a new page.
 
         Arguments
         ---------
-        space_key
-            The space key of a new page.
+        space_id
+            The id of the space where the page will be created.
         page_title
-            The title of a new page.
+            The title of the page.
         page_content
-            Content of a new page. Can be simple HTML or Confluence Storage Format.
+            The content of the page. Can be either simple HTML or
+            Confluence Storage Format.
         parent_id
-            The id number of the parent of a new page.
-            If this is None, no parent is set to a new page.
+            The id number of the page whose child the page should be.
+            If this is None, the page is created into the root of the
+            space.
         '''
+        url = urljoin(self.wiki_root_url, "api/v2/pages")
+        data = {
+            "title": page_title,
+            "spaceId": space_id,
+            "body": {
+                "representation": "storage",
+                "value": page_content}
+        }
         if parent_id:
-            data = json.dumps({"type": "page",
-                               "title": page_title,
-                               "space": {"key": space_key},
-                               "body": {"storage": {"value": page_content, "representation": "storage"}},
-                               "ancestors": [{"id": parent_id}]
-                               })
-        else:
-            data = json.dumps({"type": "page",
-                               "title": page_title,
-                               "space": {"key": space_key},
-                               "body": {"storage": {"value": page_content, "representation": "storage"}}
-                               })
-        r = post(self.content_url,
-                 data=data,
-                 headers=self.headers,
-                 auth=self.auth)
+            data["parentId"] = parent_id
+        response = post(
+            url,
+            data=json.dumps(data),
+            headers=self.headers,
+            auth=self.auth)
         try:
-            r.raise_for_status()
+            response.raise_for_status()
             print(f'Page {page_title} created.')
+            return response.json()['id']
         except HTTPError as err:
             print(f'Failed to create page {page_title}.')
             print(f'Response: {err.response.text}')
 
     def update_page(self, page_id, page_title, page_content, parent_id=None):
-        '''Update page. The version number of the page is increased by one.
+        '''Update the title, content and/or parent of a page.
+
         Notice that this overwrites the previous contents of the page!
 
         Arguments
         ---------
         page_id
             The id number of the page.
         page_title
-            The title of the page.
+            The new title of the page. If the title isn't changed, the
+            old title has to be given.
         page_content
-            Content of the page. Can be simple HTML or Confluence Storage Format.
+            The content of the page. Can be either simple HTML or
+            Confluence Storage Format.
         parent-id
             The new parent of page.
         '''
+        new_page_status = "current"
+        content_representation_type = "storage"
+        page_url = urljoin(self.wiki_root_url, f"api/v2/pages/{page_id}/")
+
         # get current version number
-        page_url = urljoin(self.content_url + '/', str(page_id))
-        v = get(page_url, auth=self.auth)
+        versions_url = urljoin(page_url, 'versions')
+        response = get(
+            versions_url,
+            params={'limit': 1, "sort": "-modified-date"},
+            auth=self.auth)
+        
         try:
-            v.raise_for_status()
-            version = v.json()['version']['number'] + 1
-        # If current version cannot be retrieved - abort.
-        # Update won't succeed if version cannot be set correctly.
+            response.raise_for_status()
+            if results := response.json()['results']:
+                current_version = results[0]['number']
+                new_version = current_version + 1
+            else:
+                print(f'Failed to retrieve the version number of page {page_title}.')
+                print(f"Cannot update page {page_title}.")
+                return
         except HTTPError as err:
-            print(f'Update failed: failed to retrieve the version number of page {page_title}.')
+            print(f'Failed to retrieve the version number of page {page_title}.')
             print(f'Response: {err.response.text}')
             return
+
         # NEW CONTENT
+        new_data = {
+            "id": page_id,
+            "status": new_page_status,
+            "title": page_title,
+            "body": {
+                "representation": content_representation_type,
+                "value": page_content
+            },
+            "version": {"number": new_version}
+        }
         if parent_id:
-            new_data = json.dumps({"type": "page",
-                                   "title": page_title,
-                                   "body": {"storage": {"value": page_content, "representation": "storage"}},
-                                   "ancestors": [{"id": parent_id}],
-                                   "version": {"number": version}
-                                   })
-        else:
-            new_data = json.dumps({"type": "page",
-                                   "title": page_title,
-                                   "body": {"storage": {"value": page_content, "representation": "storage"}},
-                                   "version": {"number": version}
-                                   })
+            new_data["parent_id"] = parent_id
+
         # UPDATE
-        r = put(page_url,
-                data=new_data,
-                headers=self.headers,
-                auth=self.auth)
+        response = put(
+            page_url,
+            data=json.dumps(new_data),
+            headers=self.headers,
+            auth=self.auth)
         try:
-            r.raise_for_status()
+            response.raise_for_status()
             print(f'Page {page_title} updated.')
         except HTTPError as err:
             print(f'Failed to update page {page_title}.')
             print(f'Response: {err.response.text}')
```

## palje/mssql_database.py

```diff
@@ -1,67 +1,92 @@
 # Palje - Document MSSQL databases to Confluence wiki
 #
 # Copyright 2021 ALM Partners Oy
 # SPDX-License-Identifier: Apache-2.0
 
 """Module for querying data from MSSQL database."""
 import getpass
+import struct
+import pyodbc
+import importlib
 from os import path
 from configparser import ConfigParser
 
-import pyodbc
 
 QUERY_FILE = 'queries/database_queries.ini'
 DATABASE_OBJECT_TYPES = {
     'BASE TABLE': 'Tables',
     'VIEW': 'Views',
     'PROCEDURE': 'Procedures',
     'FUNCTION': 'Functions'
 }
+SQL_COPT_SS_ACCESS_TOKEN = 1256  # This connection option is defined by microsoft in msodbcsql.h
 
 
 class MSSQLDatabase():
-    def __init__(self, server, database, driver):
+    def __init__(self, server, database, driver, authentication):
         self.server = server
         self.database = database
         self.driver = driver
+        self.authentication = authentication
         self.connection = None
         self.queries = self._read_queries_from_ini()
 
     @staticmethod
     def _read_queries_from_ini():
         current_dir = path.dirname(path.abspath(__file__))
         config_file = path.join(current_dir, QUERY_FILE)
         config = ConfigParser()
         config.read(config_file)
         return config['Queries']
 
     def connect(self):
         connection_str = self._ask_credentials()
         try:
-            self.connection = pyodbc.connect(connection_str)
+            if self.authentication.lower() == "azureidentity":
+                self.connection = pyodbc.connect(
+                    connection_str,
+                    attrs_before={SQL_COPT_SS_ACCESS_TOKEN: self.get_az_token()}
+                )
+            else:
+                self.connection = pyodbc.connect(connection_str)
         except:
             print(
                 f'Failed to connect to {self.server}.{self.database}. Check your server details, username and password.')
             raise
 
     def close(self):
         try:
             self.connection.close()
         except:
             print(
                 'Failed to close the database connection. Most likely because the connection is already closed.')
 
     def _ask_credentials(self):
-        uid = input(
-            f'User for {self.server}.{self.database}. If you wish to use Windows Authentication, hit enter: ')
-        if uid:
-            pwd = getpass.getpass(f'Password for user {uid}: ')
-            return f'DRIVER={{{self.driver}}};SERVER={self.server};DATABASE={self.database};UID={uid};PWD={pwd}'
-        return f'DRIVER={{{self.driver}}};SERVER={self.server};DATABASE={self.database};Trusted_Connection=yes;'
+        conn_str = f'DRIVER={{{self.driver}}};SERVER={self.server};DATABASE={self.database}'
+        if self.authentication == 'SQL':
+            uid = input(
+                f'User for {self.server}.{self.database}. If you wish to use Windows Authentication, hit enter: ')
+            if uid:
+                pwd = getpass.getpass(f'Password for user {uid}: ')
+                conn_str = f'{conn_str};UID={uid};PWD={pwd}'
+            else: 
+                conn_str = f'{conn_str};Trusted_Connection=yes;'
+        elif self.authentication == 'Windows':
+            conn_str = f'{conn_str};Trusted_Connection=yes;'
+        elif self.authentication == 'AAD':
+            conn_str = f'{conn_str};Authentication=ActiveDirectoryInteractive;'
+        return conn_str
+
+    def get_az_token(self):
+        identity = importlib.import_module('.identity', 'azure')
+        credential = identity.DefaultAzureCredential(exclude_interactive_browser_credential=False)
+        token_bytes = credential.get_token("https://database.windows.net/.default").token.encode("UTF-16-LE")
+        token_struct = struct.pack(f'<I{len(token_bytes)}s', len(token_bytes), token_bytes)
+        return token_struct
 
     def get_databases(self):
         """Return list of database names."""
         cursor = self.connection.cursor()
         try:
             cursor.execute(self.queries['database_names'])
             return [base.database_name for base in cursor.fetchall()]
```

## palje/storage_format.py

```diff
@@ -1,14 +1,14 @@
 # Palje - Document MSSQL databases to Confluence wiki
 #
 # Copyright 2021 ALM Partners Oy
 # SPDX-License-Identifier: Apache-2.0
 
 """Module for formatting content into Confluence storage format."""
-from html import escape
+
 from xml.etree import ElementTree as ET
 
 ET.register_namespace("xmlns:ac", "ac")
 
 
 def objects_list():
     """Create title 'Objects', following children macro."""
@@ -50,43 +50,42 @@
     """This will let the description show in the children macro."""
     macro = ET.Element('ac:structured-macro', attrib={
         "ac:macro-id": "3f6a7cbe-2142-47ac-a9ef-a5226c237a52",
         "ac:name": "excerpt",
         "ac:schema-version": "2"
     })
     body = ET.Element('ac:rich-text-body')
-    body.text = escape(description, quote=False)
+    body.text = description
     macro.append(body)
     return macro
 
 
 def html_table(rows):
     """Create HTML table with header from list of dicts."""
     tbody = ET.Element('tbody')
     # headers
     tr = ET.Element('tr')
     for header in rows[0].keys():
         th = ET.Element('th')
-        th.text = escape(header, quote=False)
+        th.text = header
         tr.append(th)
     tbody.append(tr)
     # rows
     for row in rows:
         tr = ET.Element('tr')
         for cell in row:
             td = ET.Element('td')
             value = row[cell]
             if isinstance(value, list):    # value is list of dicts
                 for dictionary in value:
                     p = ET.Element('p')
-                    p.text = ' '.join([escape(val, quote=False)
-                                       for val in dictionary.values()])
+                    p.text = ' '.join([val for val in dictionary.values()])
                     td.append(p)
             else:
-                td.text = escape(value, quote=False)    # value is string or number
+                td.text = value
             tr.append(td)
         tbody.append(tr)
     table = ET.Element('table')
     table.append(tbody)
     return table
```

## palje/version.py

```diff
@@ -1,5 +1,16 @@
-# coding: utf-8
 # file generated by setuptools_scm
 # don't change, don't track in version control
-version = '1.0.3'
-version_tuple = (1, 0, 3)
+TYPE_CHECKING = False
+if TYPE_CHECKING:
+    from typing import Tuple, Union
+    VERSION_TUPLE = Tuple[Union[int, str], ...]
+else:
+    VERSION_TUPLE = object
+
+version: str
+__version__: str
+__version_tuple__: VERSION_TUPLE
+version_tuple: VERSION_TUPLE
+
+__version__ = version = '2.0.0'
+__version_tuple__ = version_tuple = (2, 0, 0)
```

## Comparing `palje-1.0.3.dist-info/LICENSE` & `palje-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `palje-1.0.3.dist-info/RECORD` & `palje-2.0.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 palje/__init__.py,sha256=p9MBmsdR1dkfxDNT_vLYuaLIbq6vTLRYuRAJKjWontc,131
-palje/__main__.py,sha256=7kwBZ2Ky_vjwJNRvKELyL9EwVAK84rXhU7k27Sobn_A,9730
-palje/confluence_rest.py,sha256=3D9-I8ViV5wXDh0j98A1Bp5zVYxoT3l01sB0zVmeqiE,6820
-palje/mssql_database.py,sha256=zaStpvmq8MOJuVT4wqELwMf9X3bpLiq0DoIIBMRXU8w,9716
-palje/storage_format.py,sha256=1cXmr38ub842VjvXYrY1uLt01L_MagmAgqZfdf5R1Dk,4434
-palje/version.py,sha256=fUeHhYo8Aisg-_mdOxOq6mHLKrFYH-lfz5dJQhNSlK0,147
+palje/__main__.py,sha256=5GWf6HmWaHDCVIYdigSMkkLxKqsq7cGpoZryk1E0Sko,10408
+palje/confluence_rest.py,sha256=WvEAxBUpMiGYuAozbqLtxoPLJD-QHRo0KqV5XqRn7Ws,7152
+palje/mssql_database.py,sha256=h4DMmR8aKe6mBbOu4ugL3w_qVOeNruG86dOK1tjLqmA,10947
+palje/storage_format.py,sha256=K3fbZslt-BHmSdsnDKV7C8m0PmQ1HRpW1AxLN7yN8Y4,4256
+palje/version.py,sha256=hje97DjNnjjzdk2AwQsDgJXvORhASGZ-8JywrlJVLIw,427
 palje/queries/database_queries.ini,sha256=oZnh7P02rfiNDQFCcgqG5jNPWbdDhQPa4A-CJ_eRTRk,10126
-palje-1.0.3.dist-info/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
-palje-1.0.3.dist-info/METADATA,sha256=g3TXu47Sy9z0jJdcc6TP-yMU5yZVHPQqn2cJe3SwRbM,7445
-palje-1.0.3.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-palje-1.0.3.dist-info/top_level.txt,sha256=n64ANesnvcj7pdU1ifEXOLLWMzNK4jiK4Arx76WooIA,6
-palje-1.0.3.dist-info/RECORD,,
+palje-2.0.0.dist-info/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
+palje-2.0.0.dist-info/METADATA,sha256=I4TuQ2fHaZK2J5uZ_W0KJn1LaXfZc8SQ8KIeasmkitU,21369
+palje-2.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+palje-2.0.0.dist-info/entry_points.txt,sha256=oeN2UDXpBFxr2Irspa8WJO3L-HVeoYQb7OFdYr5z6kg,46
+palje-2.0.0.dist-info/top_level.txt,sha256=n64ANesnvcj7pdU1ifEXOLLWMzNK4jiK4Arx76WooIA,6
+palje-2.0.0.dist-info/RECORD,,
```

