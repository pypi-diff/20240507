# Comparing `tmp/dbt-risingwave-1.7.3.tar.gz` & `tmp/dbt_risingwave-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-risingwave-1.7.3.tar", last modified: Fri Mar 15 06:29:03 2024, max compression
+gzip compressed data, was "dbt_risingwave-1.7.4.tar", last modified: Tue May  7 03:27:51 2024, max compression
```

## Comparing `dbt-risingwave-1.7.3.tar` & `dbt_risingwave-1.7.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-03-15 06:29:03.925182 dbt-risingwave-1.7.3/
--rw-r--r--   0 dylan      (501) staff       (20)    11357 2023-07-11 08:53:56.000000 dbt-risingwave-1.7.3/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)       47 2023-07-11 08:53:56.000000 dbt-risingwave-1.7.3/MANIFEST.in
--rw-r--r--   0 dylan      (501) staff       (20)     5107 2024-03-15 06:29:03.924972 dbt-risingwave-1.7.3/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     4708 2024-03-15 06:28:35.000000 dbt-risingwave-1.7.3/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-03-15 06:29:03.920762 dbt-risingwave-1.7.3/dbt/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-03-15 06:29:03.920675 dbt-risingwave-1.7.3/dbt/adapters/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-03-15 06:29:03.922370 dbt-risingwave-1.7.3/dbt/adapters/risingwave/
--rw-r--r--   0 dylan      (501) staff       (20)      467 2023-07-11 08:53:56.000000 dbt-risingwave-1.7.3/dbt/adapters/risingwave/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)       18 2024-03-15 06:28:35.000000 dbt-risingwave-1.7.3/dbt/adapters/risingwave/__version__.py
--rw-r--r--   0 dylan      (501) staff       (20)     5222 2024-03-08 03:00:55.000000 dbt-risingwave-1.7.3/dbt/adapters/risingwave/connections.py
--rw-r--r--   0 dylan      (501) staff       (20)      556 2024-03-15 06:28:35.000000 dbt-risingwave-1.7.3/dbt/adapters/risingwave/impl.py
--rw-r--r--   0 dylan      (501) staff       (20)      885 2023-12-26 12:25:42.000000 dbt-risingwave-1.7.3/dbt/adapters/risingwave/relation.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-03-15 06:29:03.920829 dbt-risingwave-1.7.3/dbt/include/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-03-15 06:29:03.922756 dbt-risingwave-1.7.3/dbt/include/risingwave/
--rw-r--r--   0 dylan      (501) staff       (20)       52 2023-07-11 08:53:56.000000 dbt-risingwave-1.7.3/dbt/include/risingwave/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)       77 2023-07-24 07:32:00.000000 dbt-risingwave-1.7.3/dbt/include/risingwave/dbt_project.yml
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-03-15 06:29:03.923008 dbt-risingwave-1.7.3/dbt/include/risingwave/macros/
--rw-r--r--   0 dylan      (501) staff       (20)     7094 2024-03-13 05:05:28.000000 dbt-risingwave-1.7.3/dbt/include/risingwave/macros/adapters.sql
--rw-r--r--   0 dylan      (501) staff       (20)     2771 2024-02-06 08:49:13.000000 dbt-risingwave-1.7.3/dbt/include/risingwave/macros/catalog.sql
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-03-15 06:29:03.923994 dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/
--rw-r--r--   0 dylan      (501) staff       (20)     4281 2024-03-13 05:05:28.000000 dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/incremental.sql
--rw-r--r--   0 dylan      (501) staff       (20)     2652 2024-03-08 03:01:00.000000 dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/materialized_view.sql
--rw-r--r--   0 dylan      (501) staff       (20)     2650 2024-03-08 03:01:00.000000 dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/materializedview.sql
--rw-r--r--   0 dylan      (501) staff       (20)     1395 2024-03-08 03:01:00.000000 dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/sink.sql
--rw-r--r--   0 dylan      (501) staff       (20)     1312 2024-01-24 06:08:48.000000 dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/source.sql
--rw-r--r--   0 dylan      (501) staff       (20)     1378 2024-01-24 06:08:48.000000 dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/table.sql
--rw-r--r--   0 dylan      (501) staff       (20)     1325 2024-01-24 06:08:48.000000 dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/table_with_connector.sql
--rw-r--r--   0 dylan      (501) staff       (20)     1332 2024-01-24 06:08:48.000000 dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/view.sql
--rw-r--r--   0 dylan      (501) staff       (20)      445 2023-08-08 05:46:01.000000 dbt-risingwave-1.7.3/dbt/include/risingwave/profile_template.yml
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-03-15 06:29:03.924737 dbt-risingwave-1.7.3/dbt_risingwave.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     5107 2024-03-15 06:29:03.000000 dbt-risingwave-1.7.3/dbt_risingwave.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     1111 2024-03-15 06:29:03.000000 dbt-risingwave-1.7.3/dbt_risingwave.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2024-03-15 06:29:03.000000 dbt-risingwave-1.7.3/dbt_risingwave.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)       20 2024-03-15 06:29:03.000000 dbt-risingwave-1.7.3/dbt_risingwave.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)        4 2024-03-15 06:29:03.000000 dbt-risingwave-1.7.3/dbt_risingwave.egg-info/top_level.txt
--rw-r--r--   0 dylan      (501) staff       (20)       38 2024-03-15 06:29:03.925221 dbt-risingwave-1.7.3/setup.cfg
--rw-r--r--   0 dylan      (501) staff       (20)      898 2024-03-15 06:28:35.000000 dbt-risingwave-1.7.3/setup.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-07 03:27:51.097288 dbt_risingwave-1.7.4/
+-rw-r--r--   0 dylan      (501) staff       (20)    11357 2023-07-11 08:53:56.000000 dbt_risingwave-1.7.4/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)       47 2023-07-11 08:53:56.000000 dbt_risingwave-1.7.4/MANIFEST.in
+-rw-r--r--   0 dylan      (501) staff       (20)     5107 2024-05-07 03:27:51.097065 dbt_risingwave-1.7.4/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)     4708 2024-03-15 06:28:35.000000 dbt_risingwave-1.7.4/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-07 03:27:51.089281 dbt_risingwave-1.7.4/dbt/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-07 03:27:51.089192 dbt_risingwave-1.7.4/dbt/adapters/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-07 03:27:51.092168 dbt_risingwave-1.7.4/dbt/adapters/risingwave/
+-rw-r--r--   0 dylan      (501) staff       (20)      467 2023-07-11 08:53:56.000000 dbt_risingwave-1.7.4/dbt/adapters/risingwave/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)       18 2024-05-07 03:27:02.000000 dbt_risingwave-1.7.4/dbt/adapters/risingwave/__version__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     5222 2024-03-08 03:00:55.000000 dbt_risingwave-1.7.4/dbt/adapters/risingwave/connections.py
+-rw-r--r--   0 dylan      (501) staff       (20)      556 2024-03-15 06:28:35.000000 dbt_risingwave-1.7.4/dbt/adapters/risingwave/impl.py
+-rw-r--r--   0 dylan      (501) staff       (20)      885 2023-12-26 12:25:42.000000 dbt_risingwave-1.7.4/dbt/adapters/risingwave/relation.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-07 03:27:51.089341 dbt_risingwave-1.7.4/dbt/include/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-07 03:27:51.092946 dbt_risingwave-1.7.4/dbt/include/risingwave/
+-rw-r--r--   0 dylan      (501) staff       (20)       52 2023-07-11 08:53:56.000000 dbt_risingwave-1.7.4/dbt/include/risingwave/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)       77 2023-07-24 07:32:00.000000 dbt_risingwave-1.7.4/dbt/include/risingwave/dbt_project.yml
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-07 03:27:51.093461 dbt_risingwave-1.7.4/dbt/include/risingwave/macros/
+-rw-r--r--   0 dylan      (501) staff       (20)     7072 2024-05-07 03:27:02.000000 dbt_risingwave-1.7.4/dbt/include/risingwave/macros/adapters.sql
+-rw-r--r--   0 dylan      (501) staff       (20)     2771 2024-02-06 08:49:13.000000 dbt_risingwave-1.7.4/dbt/include/risingwave/macros/catalog.sql
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-07 03:27:51.095856 dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/
+-rw-r--r--   0 dylan      (501) staff       (20)     4281 2024-03-13 05:05:28.000000 dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/incremental.sql
+-rw-r--r--   0 dylan      (501) staff       (20)     2652 2024-03-08 03:01:00.000000 dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/materialized_view.sql
+-rw-r--r--   0 dylan      (501) staff       (20)     2650 2024-03-08 03:01:00.000000 dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/materializedview.sql
+-rw-r--r--   0 dylan      (501) staff       (20)     1394 2024-05-07 03:27:02.000000 dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/sink.sql
+-rw-r--r--   0 dylan      (501) staff       (20)     1312 2024-01-24 06:08:48.000000 dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/source.sql
+-rw-r--r--   0 dylan      (501) staff       (20)     1378 2024-01-24 06:08:48.000000 dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/table.sql
+-rw-r--r--   0 dylan      (501) staff       (20)     1325 2024-01-24 06:08:48.000000 dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/table_with_connector.sql
+-rw-r--r--   0 dylan      (501) staff       (20)     1332 2024-01-24 06:08:48.000000 dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/view.sql
+-rw-r--r--   0 dylan      (501) staff       (20)      445 2023-08-08 05:46:01.000000 dbt_risingwave-1.7.4/dbt/include/risingwave/profile_template.yml
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-07 03:27:51.096803 dbt_risingwave-1.7.4/dbt_risingwave.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     5107 2024-05-07 03:27:51.000000 dbt_risingwave-1.7.4/dbt_risingwave.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)     1111 2024-05-07 03:27:51.000000 dbt_risingwave-1.7.4/dbt_risingwave.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2024-05-07 03:27:51.000000 dbt_risingwave-1.7.4/dbt_risingwave.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       20 2024-05-07 03:27:51.000000 dbt_risingwave-1.7.4/dbt_risingwave.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        4 2024-05-07 03:27:51.000000 dbt_risingwave-1.7.4/dbt_risingwave.egg-info/top_level.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2024-05-07 03:27:51.097333 dbt_risingwave-1.7.4/setup.cfg
+-rw-r--r--   0 dylan      (501) staff       (20)      898 2024-05-07 03:27:02.000000 dbt_risingwave-1.7.4/setup.py
```

### Comparing `dbt-risingwave-1.7.3/LICENSE` & `dbt_risingwave-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/PKG-INFO` & `dbt_risingwave-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-risingwave
-Version: 1.7.3
+Version: 1.7.4
 Summary: The RisingWave adapter plugin for dbt
 Home-page: https://github.com/risingwavelabs/dbt-risingwave
 Author: Dylan Chen
 Author-email: zilin@risingwave-labs.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Keywords: dbt RisingWave
 Description-Content-Type: text/markdown
```

### Comparing `dbt-risingwave-1.7.3/README.md` & `dbt_risingwave-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/dbt/adapters/risingwave/connections.py` & `dbt_risingwave-1.7.4/dbt/adapters/risingwave/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/dbt/adapters/risingwave/impl.py` & `dbt_risingwave-1.7.4/dbt/adapters/risingwave/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/dbt/adapters/risingwave/relation.py` & `dbt_risingwave-1.7.4/dbt/adapters/risingwave/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/dbt/include/risingwave/macros/adapters.sql` & `dbt_risingwave-1.7.4/dbt/include/risingwave/macros/adapters.sql`

 * *Files 2% similar despite different names*

```diff
@@ -76,42 +76,39 @@
 
 {% macro risingwave__create_view_as(relation, sql) -%}
   create view if not exists {{ relation }}
     {% set contract_config = config.get('contract') %}
     {% if contract_config.enforced %}
       {{ get_assert_columns_equivalent(sql) }}
     {%- endif %}
-  as (
-    {{ sql }}
-  );
+  as {{ sql }}
+  ;
 {%- endmacro %}
 
 {% macro risingwave__create_table_as(relation, sql) -%}
   create table if not exists {{ relation }}
     {% set contract_config = config.get('contract') %}
     {% if contract_config.enforced %}
       {{ get_assert_columns_equivalent(sql) }}
     {%- endif %}
-  as (
-    {{ sql }}
-  );
+  as {{ sql }}
+  ;
 {%- endmacro %}
 
 {% macro risingwave__create_materialized_view_as(relation, sql) -%}
   create materialized view if not exists {{ relation }}
     {% set contract_config = config.get('contract') %}
     {% if contract_config.enforced %}
       {{ get_assert_columns_equivalent(sql) }}
     {%- endif %}
-  as (
-    {{ sql }}
-  );
+  as {{ sql }}
+  ;
 {%- endmacro %}
 
-{% macro rising_wave__create_sink(relation, sql) -%}
+{% macro risingwave__create_sink(relation, sql) -%}
     {%- set _format_parameters = config.get("format_parameters") -%}
     {%- set data_format = config.get("data_format") -%}
     {%- set data_encode = config.get("data_encode") -%}
 
     {%- set _connector_parameters = config.require("connector_parameters") -%}
     {%- set connector = config.require("connector") -%}
```

### Comparing `dbt-risingwave-1.7.3/dbt/include/risingwave/macros/catalog.sql` & `dbt_risingwave-1.7.4/dbt/include/risingwave/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/incremental.sql` & `dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/materialized_view.sql` & `dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/materializedview.sql` & `dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/materializedview.sql`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/sink.sql` & `dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/sink.sql`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     {{ run_hooks(pre_hooks, inside_transaction=False) }}
     {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
     {% if old_relation is none or (full_refresh_mode and old_relation) %}
         {%- set connector = config.get("connector") -%}
         {% call statement("main") -%}
             {% if connector %}
-              {{ rising_wave__create_sink(target_relation, sql) }}
+              {{ risingwave__create_sink(target_relation, sql) }}
             {% else %}
               {{ risingwave__run_sql(sql) }}
             {% endif %}
         {%- endcall %}
     {% else %}
       {{ risingwave__execute_no_op(target_relation) }}
     {% endif %}
```

### Comparing `dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/source.sql` & `dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/source.sql`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/table.sql` & `dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/table_with_connector.sql` & `dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/table_with_connector.sql`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/dbt/include/risingwave/macros/materializations/view.sql` & `dbt_risingwave-1.7.4/dbt/include/risingwave/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/dbt_risingwave.egg-info/PKG-INFO` & `dbt_risingwave-1.7.4/dbt_risingwave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-risingwave
-Version: 1.7.3
+Version: 1.7.4
 Summary: The RisingWave adapter plugin for dbt
 Home-page: https://github.com/risingwavelabs/dbt-risingwave
 Author: Dylan Chen
 Author-email: zilin@risingwave-labs.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Keywords: dbt RisingWave
 Description-Content-Type: text/markdown
```

### Comparing `dbt-risingwave-1.7.3/dbt_risingwave.egg-info/SOURCES.txt` & `dbt_risingwave-1.7.4/dbt_risingwave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-risingwave-1.7.3/setup.py` & `dbt_risingwave-1.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 import os
 from setuptools import find_namespace_packages, setup
 
 package_name = "dbt-risingwave"
 # make sure this always matches dbt/adapters/{adapter}/__version__.py
-package_version = "1.7.3"
+package_version = "1.7.4"
 description = """The RisingWave adapter plugin for dbt"""
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as f:
     README = f.read()
 
 setup(
     name=package_name,
```

