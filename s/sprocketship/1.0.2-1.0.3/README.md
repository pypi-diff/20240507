# Comparing `tmp/sprocketship-1.0.2.tar.gz` & `tmp/sprocketship-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-1.0.2.tar", last modified: Wed Apr 24 20:29:06 2024, max compression
+gzip compressed data, was "sprocketship-1.0.3.tar", last modified: Tue May  7 16:01:18 2024, max compression
```

## Comparing `sprocketship-1.0.2.tar` & `sprocketship-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:29:06.714528 sprocketship-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 20:29:03.000000 sprocketship-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 20:29:03.000000 sprocketship-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-04-24 20:29:06.714528 sprocketship-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-04-24 20:29:03.000000 sprocketship-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 20:29:03.000000 sprocketship-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 20:29:06.714528 sprocketship-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:29:06.710528 sprocketship-1.0.2/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-24 20:29:03.000000 sprocketship-1.0.2/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:29:06.714528 sprocketship-1.0.2/sprocketship/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 20:29:03.000000 sprocketship-1.0.2/sprocketship/templates/javascript.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-24 20:29:03.000000 sprocketship-1.0.2/sprocketship/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:29:06.714528 sprocketship-1.0.2/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-04-24 20:29:06.000000 sprocketship-1.0.2/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-24 20:29:06.000000 sprocketship-1.0.2/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:29:06.000000 sprocketship-1.0.2/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-24 20:29:06.000000 sprocketship-1.0.2/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 20:29:06.000000 sprocketship-1.0.2/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 20:29:06.000000 sprocketship-1.0.2/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:01:18.380092 sprocketship-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-07 16:01:14.000000 sprocketship-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 16:01:14.000000 sprocketship-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-07 16:01:18.380092 sprocketship-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-07 16:01:14.000000 sprocketship-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-07 16:01:14.000000 sprocketship-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:01:18.380092 sprocketship-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:01:18.376092 sprocketship-1.0.3/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-07 16:01:14.000000 sprocketship-1.0.3/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:01:18.380092 sprocketship-1.0.3/sprocketship/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-07 16:01:14.000000 sprocketship-1.0.3/sprocketship/templates/javascript.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-07 16:01:14.000000 sprocketship-1.0.3/sprocketship/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:01:18.380092 sprocketship-1.0.3/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-07 16:01:18.000000 sprocketship-1.0.3/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-07 16:01:18.000000 sprocketship-1.0.3/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:01:18.000000 sprocketship-1.0.3/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 16:01:18.000000 sprocketship-1.0.3/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 16:01:18.000000 sprocketship-1.0.3/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 16:01:18.000000 sprocketship-1.0.3/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-1.0.2/LICENSE` & `sprocketship-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-1.0.2/PKG-INFO` & `sprocketship-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: sprocketship
-Version: 1.0.2
-Summary: Better stored procedure management
-Author-email: Nicklaus Roach <nicklausroach@gmail.com>
-Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
-Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: snowflake-connector-python
-Requires-Dist: ABSQL
-Requires-Dist: ruamel.yaml
-Requires-Dist: jinja2
-
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
 *** that would make this better, please fork the repo and create a pull request
 *** or simply open an issue with the tag "enhancement".
 *** Don't forget to give the project a star!
@@ -44,15 +26,15 @@
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 60px; text-decoration: none;">
-    ⚙️ 🚀
+    <img src="./sprocketship/resources/logo.webp" width='500'>
   </a>
 <h3 align="center">Sprocketship</h3>
 
   <p align="center">
     Better stored procedure management
   </p>
 </div>
@@ -127,42 +109,42 @@
 │   ├── sysadmin
 │   │   ├── create_temp_database.js
 └── .sprocketship.yml
 ```
 
 The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
 
-```
+```yml
 procedures:
   development:
-    - name: create_temp_database
+    create_temp_database:
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
   admin:
-    - name: create_database_reader
+    create_database_reader:
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
-    - name: create_database_writer
+    create_database_writer:
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 ```
 
 ### Directory-level Default Parameters
 
 sprocketship allows providing default parameters at any given level of
 your project. These defaults will be applied recursively to any procedures
 defined in any of the subdirectories, unless overridden by a default in one
 of the subdirectories.
 
-```
+```yml
 procedures:
   # for all procedures, default to the below database and schema
   +database: !env_var SNOWFLAKE_DATABASE
   +schema: !env_var SNOWFLAKE_SCHEMA
   development:
     # for all procedures in the development directory,
     # default to using the sysadmin role
@@ -189,27 +171,58 @@
 */
 ```
 
 sprocketship will automatically parse and apply the parameters defined in the frontmatter to the stored procedure.
 
 ### Recommended Configuration
 
-When setting up your sprocketship project, we recommend setting more general parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml` file, and anything that's specific to a given procedure should be defined in the file frontmatter of that procedure, such as the args or return type.
+When setting up your sprocketship project, we recommend setting more general parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml` file, and anything that's specific to a given procedure should be defined in the file frontmatter of that procedure, such as the args or return type. Example below:
+
+```yml
+# .sprocketship.yml
+procedures:
+  +database: my_database
+  +schema: my_schema
+  +language: javascript
+  +execute_as: owner
+  sysadmin:
+    +use_role: sysadmin
+  useradmin:
+    +use_role: useradmin
+```
+
+In the above `.sprocketship.yml`, we've set the database, schema, language, and executor at the highest level. This means that all procedures in the `sysadmin` and `useradmin` directories will inherit these defaults unless overridden. Now we can define procedure-specific
+parameters in the file frontmatter:
+
+```js
+// procedures/useradmin/create_role.js
+/*
+args:
+  - name: role_name
+    type: varchar
+returns: varchar
+comment: |
+  Creates a role with the provided name
+*/
+
+var roleName = ROLE_NAME;
+snowflake.execute(`CREATE ROLE IF NOT EXISTS ${roleName}`)
+```
 
 ### Execution
 
 From here, simply run 
 
 `$ sprocketship liftoff` 
 
 from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
 
 ### Exhaustive Options for Stored Procedure Configuration
 
-```
+```yml
 database: The name of the database where the procedure will be stored
 schema: The name of the schema where the procedure will be stored
 language: The language of the procedure definition
 execute_as: caller or owner
 use_role: The role you'd like to own the procedure
 args:
     - name: Name of argument
```

#### html2text {}

```diff
@@ -1,20 +1,11 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 1.0.2 Summary: Better stored
-procedure management Author-email: Nicklaus Roach
-gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
-Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
-Dist: ruamel.yaml Requires-Dist: jinja2 [![Contributors][contributors-shield]]
-[contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
-shield]][stars-url] [![Issues][issues-shield]][issues-url] [![LinkedIn]
-[linkedin-shield]][linkedin-url]
-                                  _â___ï_¸__ _ð___
+[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
+shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
+shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-url]
+                     _[_._/_s_p_r_o_c_k_e_t_s_h_i_p_/_r_e_s_o_u_r_c_e_s_/_l_o_g_o_._w_e_b_p_]
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _I_n_s_t_a_l_l_a_t_i_o_n
@@ -31,56 +22,66 @@
 Structure Currently, sprocketship expects a `.sprocketship.yml` file in a
 `procedures/` directory. ``` âââ dbt_models â âââ customers.sql
 â âââ products.sql âââ procedures â âââ useradmin â â
 âââ create_database_writer_role.js â â âââ
 create_database_reader_role.js â âââ sysadmin â â âââ
 create_temp_database.js âââ .sprocketship.yml ``` The yaml path to each
 procedure in the `sprocketship.yml` should follow that of the paths to their
-corresponding files in the `procedures/` directory. ``` procedures:
-development: - name: create_temp_database database: !env_var SNOWFLAKE_DATABASE
-schema: !env_var SNOWFLAKE_SCHEMA ... admin: - name: create_database_reader
-database: !env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... -
-name: create_database_writer database: !env_var SNOWFLAKE_DATABASE schema:
-!env_var SNOWFLAKE_SCHEMA ... ``` ### Directory-level Default Parameters
-sprocketship allows providing default parameters at any given level of your
-project. These defaults will be applied recursively to any procedures defined
-in any of the subdirectories, unless overridden by a default in one of the
-subdirectories. ``` procedures: # for all procedures, default to the below
-database and schema +database: !env_var SNOWFLAKE_DATABASE +schema: !env_var
+corresponding files in the `procedures/` directory. ```yml procedures:
+development: create_temp_database: database: !env_var SNOWFLAKE_DATABASE
+schema: !env_var SNOWFLAKE_SCHEMA ... admin: create_database_reader: database:
+!env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ...
+create_database_writer: database: !env_var SNOWFLAKE_DATABASE schema: !env_var
+SNOWFLAKE_SCHEMA ... ``` ### Directory-level Default Parameters sprocketship
+allows providing default parameters at any given level of your project. These
+defaults will be applied recursively to any procedures defined in any of the
+subdirectories, unless overridden by a default in one of the subdirectories.
+```yml procedures: # for all procedures, default to the below database and
+schema +database: !env_var SNOWFLAKE_DATABASE +schema: !env_var
 SNOWFLAKE_SCHEMA development: # for all procedures in the development
 directory, # default to using the sysadmin role +use_role: sysadmin
 create_temp_database: args: - name: Name of argument type: Type of argument
 default: (Optional) default value for the argument returns: varchar ``` ###
 File Frontmatter Thanks to ABSQL, sprocketship also provides the ability to
 define parameters using file frontmatter. Suppose we have a file
 `create_database_writer_role.js`, we can define parameters for the stored
 procedure within the file using frontmatter: ```js /* database: my_database
 schema: my_schema language: javascript execute_as: owner use_role: sysadmin */
 ``` sprocketship will automatically parse and apply the parameters defined in
 the frontmatter to the stored procedure. ### Recommended Configuration When
 setting up your sprocketship project, we recommend setting more general
 parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml`
 file, and anything that's specific to a given procedure should be defined in
-the file frontmatter of that procedure, such as the args or return type. ###
-Execution From here, simply run `$ sprocketship liftoff` from the project
-directory (or provide the directory, e.g. `sprocketship liftoff my/directory/
-path`) and sprocketship will launch your stored procedures into the given
-directory. ### Exhaustive Options for Stored Procedure Configuration ```
-database: The name of the database where the procedure will be stored schema:
-The name of the schema where the procedure will be stored language: The
-language of the procedure definition execute_as: caller or owner use_role: The
-role you'd like to own the procedure args: - name: Name of argument type: Type
-of argument default: (Optional) default value for the argument returns: The
-return type, this can include the `NOT NULL` option comment: Explanation of the
-procedure ``` ## Support sprocketship currently only supports Javascript-based
-stored procedures (Python support coming soon!). Additionally, there are a few
-options from the `CREATE STORED PROCEDURE` function that are not yet supported:
-* `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT | STRICT }` * `VOLATILE
-| IMMUTABLE` (deprecated) ## License Distributed under the MIT License. See
-`LICENSE` for more information.
+the file frontmatter of that procedure, such as the args or return type.
+Example below: ```yml # .sprocketship.yml procedures: +database: my_database
++schema: my_schema +language: javascript +execute_as: owner sysadmin:
++use_role: sysadmin useradmin: +use_role: useradmin ``` In the above
+`.sprocketship.yml`, we've set the database, schema, language, and executor at
+the highest level. This means that all procedures in the `sysadmin` and
+`useradmin` directories will inherit these defaults unless overridden. Now we
+can define procedure-specific parameters in the file frontmatter: ```js /
+/ procedures/useradmin/create_role.js /* args: - name: role_name type: varchar
+returns: varchar comment: | Creates a role with the provided name */ var
+roleName = ROLE_NAME; snowflake.execute(`CREATE ROLE IF NOT EXISTS $
+{roleName}`) ``` ### Execution From here, simply run `$ sprocketship liftoff`
+from the project directory (or provide the directory, e.g. `sprocketship
+liftoff my/directory/path`) and sprocketship will launch your stored procedures
+into the given directory. ### Exhaustive Options for Stored Procedure
+Configuration ```yml database: The name of the database where the procedure
+will be stored schema: The name of the schema where the procedure will be
+stored language: The language of the procedure definition execute_as: caller or
+owner use_role: The role you'd like to own the procedure args: - name: Name of
+argument type: Type of argument default: (Optional) default value for the
+argument returns: The return type, this can include the `NOT NULL` option
+comment: Explanation of the procedure ``` ## Support sprocketship currently
+only supports Javascript-based stored procedures (Python support coming soon!).
+Additionally, there are a few options from the `CREATE STORED PROCEDURE`
+function that are not yet supported: * `CALLED ON NULL INPUT | { RETURNS NULL
+ON NULL INPUT | STRICT }` * `VOLATILE | IMMUTABLE` (deprecated) ## License
+Distributed under the MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

### Comparing `sprocketship-1.0.2/README.md` & `sprocketship-1.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: sprocketship
+Version: 1.0.3
+Summary: Better stored procedure management
+Author-email: Nicklaus Roach <nicklausroach@gmail.com>
+Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
+Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: snowflake-connector-python
+Requires-Dist: ABSQL
+Requires-Dist: ruamel.yaml
+Requires-Dist: jinja2
+
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
 *** that would make this better, please fork the repo and create a pull request
 *** or simply open an issue with the tag "enhancement".
 *** Don't forget to give the project a star!
@@ -26,15 +44,15 @@
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 60px; text-decoration: none;">
-    ⚙️ 🚀
+    <img src="./sprocketship/resources/logo.webp" width='500'>
   </a>
 <h3 align="center">Sprocketship</h3>
 
   <p align="center">
     Better stored procedure management
   </p>
 </div>
@@ -109,42 +127,42 @@
 │   ├── sysadmin
 │   │   ├── create_temp_database.js
 └── .sprocketship.yml
 ```
 
 The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
 
-```
+```yml
 procedures:
   development:
-    - name: create_temp_database
+    create_temp_database:
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
   admin:
-    - name: create_database_reader
+    create_database_reader:
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
-    - name: create_database_writer
+    create_database_writer:
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 ```
 
 ### Directory-level Default Parameters
 
 sprocketship allows providing default parameters at any given level of
 your project. These defaults will be applied recursively to any procedures
 defined in any of the subdirectories, unless overridden by a default in one
 of the subdirectories.
 
-```
+```yml
 procedures:
   # for all procedures, default to the below database and schema
   +database: !env_var SNOWFLAKE_DATABASE
   +schema: !env_var SNOWFLAKE_SCHEMA
   development:
     # for all procedures in the development directory,
     # default to using the sysadmin role
@@ -171,27 +189,58 @@
 */
 ```
 
 sprocketship will automatically parse and apply the parameters defined in the frontmatter to the stored procedure.
 
 ### Recommended Configuration
 
-When setting up your sprocketship project, we recommend setting more general parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml` file, and anything that's specific to a given procedure should be defined in the file frontmatter of that procedure, such as the args or return type.
+When setting up your sprocketship project, we recommend setting more general parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml` file, and anything that's specific to a given procedure should be defined in the file frontmatter of that procedure, such as the args or return type. Example below:
+
+```yml
+# .sprocketship.yml
+procedures:
+  +database: my_database
+  +schema: my_schema
+  +language: javascript
+  +execute_as: owner
+  sysadmin:
+    +use_role: sysadmin
+  useradmin:
+    +use_role: useradmin
+```
+
+In the above `.sprocketship.yml`, we've set the database, schema, language, and executor at the highest level. This means that all procedures in the `sysadmin` and `useradmin` directories will inherit these defaults unless overridden. Now we can define procedure-specific
+parameters in the file frontmatter:
+
+```js
+// procedures/useradmin/create_role.js
+/*
+args:
+  - name: role_name
+    type: varchar
+returns: varchar
+comment: |
+  Creates a role with the provided name
+*/
+
+var roleName = ROLE_NAME;
+snowflake.execute(`CREATE ROLE IF NOT EXISTS ${roleName}`)
+```
 
 ### Execution
 
 From here, simply run 
 
 `$ sprocketship liftoff` 
 
 from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
 
 ### Exhaustive Options for Stored Procedure Configuration
 
-```
+```yml
 database: The name of the database where the procedure will be stored
 schema: The name of the schema where the procedure will be stored
 language: The language of the procedure definition
 execute_as: caller or owner
 use_role: The role you'd like to own the procedure
 args:
     - name: Name of argument
```

#### html2text {}

```diff
@@ -1,11 +1,20 @@
-[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
-shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-url]
-                                  _â___ï_¸__ _ð___
+Metadata-Version: 2.1 Name: sprocketship Version: 1.0.3 Summary: Better stored
+procedure management Author-email: Nicklaus Roach
+gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
+Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
+Dist: ruamel.yaml Requires-Dist: jinja2 [![Contributors][contributors-shield]]
+[contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
+shield]][stars-url] [![Issues][issues-shield]][issues-url] [![LinkedIn]
+[linkedin-shield]][linkedin-url]
+                     _[_._/_s_p_r_o_c_k_e_t_s_h_i_p_/_r_e_s_o_u_r_c_e_s_/_l_o_g_o_._w_e_b_p_]
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _I_n_s_t_a_l_l_a_t_i_o_n
@@ -22,56 +31,66 @@
 Structure Currently, sprocketship expects a `.sprocketship.yml` file in a
 `procedures/` directory. ``` âââ dbt_models â âââ customers.sql
 â âââ products.sql âââ procedures â âââ useradmin â â
 âââ create_database_writer_role.js â â âââ
 create_database_reader_role.js â âââ sysadmin â â âââ
 create_temp_database.js âââ .sprocketship.yml ``` The yaml path to each
 procedure in the `sprocketship.yml` should follow that of the paths to their
-corresponding files in the `procedures/` directory. ``` procedures:
-development: - name: create_temp_database database: !env_var SNOWFLAKE_DATABASE
-schema: !env_var SNOWFLAKE_SCHEMA ... admin: - name: create_database_reader
-database: !env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... -
-name: create_database_writer database: !env_var SNOWFLAKE_DATABASE schema:
-!env_var SNOWFLAKE_SCHEMA ... ``` ### Directory-level Default Parameters
-sprocketship allows providing default parameters at any given level of your
-project. These defaults will be applied recursively to any procedures defined
-in any of the subdirectories, unless overridden by a default in one of the
-subdirectories. ``` procedures: # for all procedures, default to the below
-database and schema +database: !env_var SNOWFLAKE_DATABASE +schema: !env_var
+corresponding files in the `procedures/` directory. ```yml procedures:
+development: create_temp_database: database: !env_var SNOWFLAKE_DATABASE
+schema: !env_var SNOWFLAKE_SCHEMA ... admin: create_database_reader: database:
+!env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ...
+create_database_writer: database: !env_var SNOWFLAKE_DATABASE schema: !env_var
+SNOWFLAKE_SCHEMA ... ``` ### Directory-level Default Parameters sprocketship
+allows providing default parameters at any given level of your project. These
+defaults will be applied recursively to any procedures defined in any of the
+subdirectories, unless overridden by a default in one of the subdirectories.
+```yml procedures: # for all procedures, default to the below database and
+schema +database: !env_var SNOWFLAKE_DATABASE +schema: !env_var
 SNOWFLAKE_SCHEMA development: # for all procedures in the development
 directory, # default to using the sysadmin role +use_role: sysadmin
 create_temp_database: args: - name: Name of argument type: Type of argument
 default: (Optional) default value for the argument returns: varchar ``` ###
 File Frontmatter Thanks to ABSQL, sprocketship also provides the ability to
 define parameters using file frontmatter. Suppose we have a file
 `create_database_writer_role.js`, we can define parameters for the stored
 procedure within the file using frontmatter: ```js /* database: my_database
 schema: my_schema language: javascript execute_as: owner use_role: sysadmin */
 ``` sprocketship will automatically parse and apply the parameters defined in
 the frontmatter to the stored procedure. ### Recommended Configuration When
 setting up your sprocketship project, we recommend setting more general
 parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml`
 file, and anything that's specific to a given procedure should be defined in
-the file frontmatter of that procedure, such as the args or return type. ###
-Execution From here, simply run `$ sprocketship liftoff` from the project
-directory (or provide the directory, e.g. `sprocketship liftoff my/directory/
-path`) and sprocketship will launch your stored procedures into the given
-directory. ### Exhaustive Options for Stored Procedure Configuration ```
-database: The name of the database where the procedure will be stored schema:
-The name of the schema where the procedure will be stored language: The
-language of the procedure definition execute_as: caller or owner use_role: The
-role you'd like to own the procedure args: - name: Name of argument type: Type
-of argument default: (Optional) default value for the argument returns: The
-return type, this can include the `NOT NULL` option comment: Explanation of the
-procedure ``` ## Support sprocketship currently only supports Javascript-based
-stored procedures (Python support coming soon!). Additionally, there are a few
-options from the `CREATE STORED PROCEDURE` function that are not yet supported:
-* `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT | STRICT }` * `VOLATILE
-| IMMUTABLE` (deprecated) ## License Distributed under the MIT License. See
-`LICENSE` for more information.
+the file frontmatter of that procedure, such as the args or return type.
+Example below: ```yml # .sprocketship.yml procedures: +database: my_database
++schema: my_schema +language: javascript +execute_as: owner sysadmin:
++use_role: sysadmin useradmin: +use_role: useradmin ``` In the above
+`.sprocketship.yml`, we've set the database, schema, language, and executor at
+the highest level. This means that all procedures in the `sysadmin` and
+`useradmin` directories will inherit these defaults unless overridden. Now we
+can define procedure-specific parameters in the file frontmatter: ```js /
+/ procedures/useradmin/create_role.js /* args: - name: role_name type: varchar
+returns: varchar comment: | Creates a role with the provided name */ var
+roleName = ROLE_NAME; snowflake.execute(`CREATE ROLE IF NOT EXISTS $
+{roleName}`) ``` ### Execution From here, simply run `$ sprocketship liftoff`
+from the project directory (or provide the directory, e.g. `sprocketship
+liftoff my/directory/path`) and sprocketship will launch your stored procedures
+into the given directory. ### Exhaustive Options for Stored Procedure
+Configuration ```yml database: The name of the database where the procedure
+will be stored schema: The name of the schema where the procedure will be
+stored language: The language of the procedure definition execute_as: caller or
+owner use_role: The role you'd like to own the procedure args: - name: Name of
+argument type: Type of argument default: (Optional) default value for the
+argument returns: The return type, this can include the `NOT NULL` option
+comment: Explanation of the procedure ``` ## Support sprocketship currently
+only supports Javascript-based stored procedures (Python support coming soon!).
+Additionally, there are a few options from the `CREATE STORED PROCEDURE`
+function that are not yet supported: * `CALLED ON NULL INPUT | { RETURNS NULL
+ON NULL INPUT | STRICT }` * `VOLATILE | IMMUTABLE` (deprecated) ## License
+Distributed under the MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

### Comparing `sprocketship-1.0.2/pyproject.toml` & `sprocketship-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Nicklaus Roach", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 description = "Better stored procedure management"
 dependencies = [
     "click",
```

### Comparing `sprocketship-1.0.2/sprocketship/cli.py` & `sprocketship-1.0.3/sprocketship/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 **proc, **{"project_dir": dir}
             )
             if "use_role" in proc.keys():
                 con.cursor().execute(f"USE ROLE {proc_dict['use_role'].upper()}")
             else:
                 con.cursor().execute(f"USE ROLE {data['snowflake']['role']}")
             con.cursor().execute(proc_dict["rendered_file"])
-            if "grant_usage" in proc.keys():
+            if "grant_usage" in proc_dict.keys():
                 grant_usage(proc_dict, con)
 
             msg = click.style(f"{proc_dict['name']} ", fg="green", bold=True)
             msg += click.style(f"launched into schema ", fg="white", bold=True)
             msg += click.style(
                 f"{proc_dict['database']}.{proc_dict['schema']}", fg="blue", bold=True
             )
```

### Comparing `sprocketship-1.0.2/sprocketship/utils.py` & `sprocketship-1.0.3/sprocketship/utils.py`

 * *Files identical despite different names*

### Comparing `sprocketship-1.0.2/sprocketship.egg-info/PKG-INFO` & `sprocketship-1.0.3/sprocketship.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 1.0.2
+Version: 1.0.3
 Summary: Better stored procedure management
 Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -44,15 +44,15 @@
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/nicklausroach/sprocketship" style="font-size: 60px; text-decoration: none;">
-    ⚙️ 🚀
+    <img src="./sprocketship/resources/logo.webp" width='500'>
   </a>
 <h3 align="center">Sprocketship</h3>
 
   <p align="center">
     Better stored procedure management
   </p>
 </div>
@@ -127,42 +127,42 @@
 │   ├── sysadmin
 │   │   ├── create_temp_database.js
 └── .sprocketship.yml
 ```
 
 The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
 
-```
+```yml
 procedures:
   development:
-    - name: create_temp_database
+    create_temp_database:
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
   admin:
-    - name: create_database_reader
+    create_database_reader:
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 
-    - name: create_database_writer
+    create_database_writer:
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 ```
 
 ### Directory-level Default Parameters
 
 sprocketship allows providing default parameters at any given level of
 your project. These defaults will be applied recursively to any procedures
 defined in any of the subdirectories, unless overridden by a default in one
 of the subdirectories.
 
-```
+```yml
 procedures:
   # for all procedures, default to the below database and schema
   +database: !env_var SNOWFLAKE_DATABASE
   +schema: !env_var SNOWFLAKE_SCHEMA
   development:
     # for all procedures in the development directory,
     # default to using the sysadmin role
@@ -189,27 +189,58 @@
 */
 ```
 
 sprocketship will automatically parse and apply the parameters defined in the frontmatter to the stored procedure.
 
 ### Recommended Configuration
 
-When setting up your sprocketship project, we recommend setting more general parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml` file, and anything that's specific to a given procedure should be defined in the file frontmatter of that procedure, such as the args or return type.
+When setting up your sprocketship project, we recommend setting more general parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml` file, and anything that's specific to a given procedure should be defined in the file frontmatter of that procedure, such as the args or return type. Example below:
+
+```yml
+# .sprocketship.yml
+procedures:
+  +database: my_database
+  +schema: my_schema
+  +language: javascript
+  +execute_as: owner
+  sysadmin:
+    +use_role: sysadmin
+  useradmin:
+    +use_role: useradmin
+```
+
+In the above `.sprocketship.yml`, we've set the database, schema, language, and executor at the highest level. This means that all procedures in the `sysadmin` and `useradmin` directories will inherit these defaults unless overridden. Now we can define procedure-specific
+parameters in the file frontmatter:
+
+```js
+// procedures/useradmin/create_role.js
+/*
+args:
+  - name: role_name
+    type: varchar
+returns: varchar
+comment: |
+  Creates a role with the provided name
+*/
+
+var roleName = ROLE_NAME;
+snowflake.execute(`CREATE ROLE IF NOT EXISTS ${roleName}`)
+```
 
 ### Execution
 
 From here, simply run 
 
 `$ sprocketship liftoff` 
 
 from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
 
 ### Exhaustive Options for Stored Procedure Configuration
 
-```
+```yml
 database: The name of the database where the procedure will be stored
 schema: The name of the schema where the procedure will be stored
 language: The language of the procedure definition
 execute_as: caller or owner
 use_role: The role you'd like to own the procedure
 args:
     - name: Name of argument
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 1.0.2 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 1.0.3 Summary: Better stored
 procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
 Dist: ruamel.yaml Requires-Dist: jinja2 [![Contributors][contributors-shield]]
 [contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
 shield]][stars-url] [![Issues][issues-shield]][issues-url] [![LinkedIn]
 [linkedin-shield]][linkedin-url]
-                                  _â___ï_¸__ _ð___
+                     _[_._/_s_p_r_o_c_k_e_t_s_h_i_p_/_r_e_s_o_u_r_c_e_s_/_l_o_g_o_._w_e_b_p_]
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _I_n_s_t_a_l_l_a_t_i_o_n
@@ -31,56 +31,66 @@
 Structure Currently, sprocketship expects a `.sprocketship.yml` file in a
 `procedures/` directory. ``` âââ dbt_models â âââ customers.sql
 â âââ products.sql âââ procedures â âââ useradmin â â
 âââ create_database_writer_role.js â â âââ
 create_database_reader_role.js â âââ sysadmin â â âââ
 create_temp_database.js âââ .sprocketship.yml ``` The yaml path to each
 procedure in the `sprocketship.yml` should follow that of the paths to their
-corresponding files in the `procedures/` directory. ``` procedures:
-development: - name: create_temp_database database: !env_var SNOWFLAKE_DATABASE
-schema: !env_var SNOWFLAKE_SCHEMA ... admin: - name: create_database_reader
-database: !env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... -
-name: create_database_writer database: !env_var SNOWFLAKE_DATABASE schema:
-!env_var SNOWFLAKE_SCHEMA ... ``` ### Directory-level Default Parameters
-sprocketship allows providing default parameters at any given level of your
-project. These defaults will be applied recursively to any procedures defined
-in any of the subdirectories, unless overridden by a default in one of the
-subdirectories. ``` procedures: # for all procedures, default to the below
-database and schema +database: !env_var SNOWFLAKE_DATABASE +schema: !env_var
+corresponding files in the `procedures/` directory. ```yml procedures:
+development: create_temp_database: database: !env_var SNOWFLAKE_DATABASE
+schema: !env_var SNOWFLAKE_SCHEMA ... admin: create_database_reader: database:
+!env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ...
+create_database_writer: database: !env_var SNOWFLAKE_DATABASE schema: !env_var
+SNOWFLAKE_SCHEMA ... ``` ### Directory-level Default Parameters sprocketship
+allows providing default parameters at any given level of your project. These
+defaults will be applied recursively to any procedures defined in any of the
+subdirectories, unless overridden by a default in one of the subdirectories.
+```yml procedures: # for all procedures, default to the below database and
+schema +database: !env_var SNOWFLAKE_DATABASE +schema: !env_var
 SNOWFLAKE_SCHEMA development: # for all procedures in the development
 directory, # default to using the sysadmin role +use_role: sysadmin
 create_temp_database: args: - name: Name of argument type: Type of argument
 default: (Optional) default value for the argument returns: varchar ``` ###
 File Frontmatter Thanks to ABSQL, sprocketship also provides the ability to
 define parameters using file frontmatter. Suppose we have a file
 `create_database_writer_role.js`, we can define parameters for the stored
 procedure within the file using frontmatter: ```js /* database: my_database
 schema: my_schema language: javascript execute_as: owner use_role: sysadmin */
 ``` sprocketship will automatically parse and apply the parameters defined in
 the frontmatter to the stored procedure. ### Recommended Configuration When
 setting up your sprocketship project, we recommend setting more general
 parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml`
 file, and anything that's specific to a given procedure should be defined in
-the file frontmatter of that procedure, such as the args or return type. ###
-Execution From here, simply run `$ sprocketship liftoff` from the project
-directory (or provide the directory, e.g. `sprocketship liftoff my/directory/
-path`) and sprocketship will launch your stored procedures into the given
-directory. ### Exhaustive Options for Stored Procedure Configuration ```
-database: The name of the database where the procedure will be stored schema:
-The name of the schema where the procedure will be stored language: The
-language of the procedure definition execute_as: caller or owner use_role: The
-role you'd like to own the procedure args: - name: Name of argument type: Type
-of argument default: (Optional) default value for the argument returns: The
-return type, this can include the `NOT NULL` option comment: Explanation of the
-procedure ``` ## Support sprocketship currently only supports Javascript-based
-stored procedures (Python support coming soon!). Additionally, there are a few
-options from the `CREATE STORED PROCEDURE` function that are not yet supported:
-* `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT | STRICT }` * `VOLATILE
-| IMMUTABLE` (deprecated) ## License Distributed under the MIT License. See
-`LICENSE` for more information.
+the file frontmatter of that procedure, such as the args or return type.
+Example below: ```yml # .sprocketship.yml procedures: +database: my_database
++schema: my_schema +language: javascript +execute_as: owner sysadmin:
++use_role: sysadmin useradmin: +use_role: useradmin ``` In the above
+`.sprocketship.yml`, we've set the database, schema, language, and executor at
+the highest level. This means that all procedures in the `sysadmin` and
+`useradmin` directories will inherit these defaults unless overridden. Now we
+can define procedure-specific parameters in the file frontmatter: ```js /
+/ procedures/useradmin/create_role.js /* args: - name: role_name type: varchar
+returns: varchar comment: | Creates a role with the provided name */ var
+roleName = ROLE_NAME; snowflake.execute(`CREATE ROLE IF NOT EXISTS $
+{roleName}`) ``` ### Execution From here, simply run `$ sprocketship liftoff`
+from the project directory (or provide the directory, e.g. `sprocketship
+liftoff my/directory/path`) and sprocketship will launch your stored procedures
+into the given directory. ### Exhaustive Options for Stored Procedure
+Configuration ```yml database: The name of the database where the procedure
+will be stored schema: The name of the schema where the procedure will be
+stored language: The language of the procedure definition execute_as: caller or
+owner use_role: The role you'd like to own the procedure args: - name: Name of
+argument type: Type of argument default: (Optional) default value for the
+argument returns: The return type, this can include the `NOT NULL` option
+comment: Explanation of the procedure ``` ## Support sprocketship currently
+only supports Javascript-based stored procedures (Python support coming soon!).
+Additionally, there are a few options from the `CREATE STORED PROCEDURE`
+function that are not yet supported: * `CALLED ON NULL INPUT | { RETURNS NULL
+ON NULL INPUT | STRICT }` * `VOLATILE | IMMUTABLE` (deprecated) ## License
+Distributed under the MIT License. See `LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

