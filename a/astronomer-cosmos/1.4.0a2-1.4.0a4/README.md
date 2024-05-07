# Comparing `tmp/astronomer_cosmos-1.4.0a2.tar.gz` & `tmp/astronomer_cosmos-1.4.0a4.tar.gz`

## Comparing `astronomer_cosmos-1.4.0a2.tar` & `astronomer_cosmos-1.4.0a4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/__init__.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/cache.py
--rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/config.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/constants.py
--rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/converter.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/exceptions.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/log.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/airflow/__init__.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/airflow/dag.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/airflow/graph.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/airflow/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/core/__init__.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/executable.py
--rw-r--r--   0        0        0    18527 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/graph.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/project.py
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/selector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/parser/__init__.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/parser/output.py
--rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/dbt/parser/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/hooks/__init__.py
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/hooks/subprocess.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/__init__.py
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/azure_container_instance.py
--rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/base.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/docker.py
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/kubernetes.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/lazy_load.py
--rw-r--r--   0        0        0    32029 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/local.py
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/operators/virtualenv.py
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/plugin/__init__.py
--rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/plugin/static/iframeResizer.contentWindow.min.js
--rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/plugin/static/iframeResizer.min.js
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/plugin/templates/dbt_docs.html
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/plugin/templates/dbt_docs_not_set_up.html
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/__init__.py
--rwxr-xr-x   0        0        0    11351 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/base.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/athena/__init__.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/athena/access_key.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/oauth.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/service_account_keyfile_dict.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/databricks/token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_privatekey.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/spark/thrift.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/base.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/ldap.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/vertica/__init__.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/cosmos/profiles/vertica/user_pass.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/LICENSE
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/README.rst
--rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/pyproject.toml
--rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a2/PKG-INFO
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/__init__.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/cache.py
+-rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/config.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/constants.py
+-rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/converter.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/exceptions.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/log.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/airflow/__init__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/airflow/dag.py
+-rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/airflow/graph.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/airflow/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/executable.py
+-rw-r--r--   0        0        0    18527 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/graph.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/project.py
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/selector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/parser/__init__.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/parser/output.py
+-rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/dbt/parser/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/hooks/__init__.py
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/hooks/subprocess.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/__init__.py
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/azure_container_instance.py
+-rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/base.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/docker.py
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/kubernetes.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/lazy_load.py
+-rw-r--r--   0        0        0    32095 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/local.py
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/operators/virtualenv.py
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/plugin/__init__.py
+-rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/plugin/static/iframeResizer.contentWindow.min.js
+-rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/plugin/static/iframeResizer.min.js
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/plugin/templates/dbt_docs.html
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/plugin/templates/dbt_docs_not_set_up.html
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/__init__.py
+-rwxr-xr-x   0        0        0    11351 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/base.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/athena/__init__.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/athena/access_key.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/oauth.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/service_account_keyfile_dict.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/databricks/token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_privatekey.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/spark/thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/base.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/ldap.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/vertica/__init__.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/cosmos/profiles/vertica/user_pass.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/LICENSE
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/README.rst
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/pyproject.toml
+-rw-r--r--   0        0        0     7718 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0a4/PKG-INFO
```

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/__init__.py` & `astronomer_cosmos-1.4.0a4/cosmos/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # type: ignore # ignores "Cannot assign to a type" MyPy error
 
 """
 Astronomer Cosmos is a library for rendering dbt workflows in Airflow.
 
 Contains dags, task groups, and operators.
 """
-__version__ = "1.4.0a2"
+__version__ = "1.4.0a4"
 
 
 from cosmos.airflow.dag import DbtDag
 from cosmos.airflow.task_group import DbtTaskGroup
 from cosmos.config import (
     ExecutionConfig,
     ProfileConfig,
```

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/cache.py` & `astronomer_cosmos-1.4.0a4/cosmos/cache.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/config.py` & `astronomer_cosmos-1.4.0a4/cosmos/config.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/constants.py` & `astronomer_cosmos-1.4.0a4/cosmos/constants.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/converter.py` & `astronomer_cosmos-1.4.0a4/cosmos/converter.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/log.py` & `astronomer_cosmos-1.4.0a4/cosmos/log.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/airflow/dag.py` & `astronomer_cosmos-1.4.0a4/cosmos/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/airflow/graph.py` & `astronomer_cosmos-1.4.0a4/cosmos/airflow/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/airflow/task_group.py` & `astronomer_cosmos-1.4.0a4/cosmos/airflow/task_group.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/core/airflow.py` & `astronomer_cosmos-1.4.0a4/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/core/graph/entities.py` & `astronomer_cosmos-1.4.0a4/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/dbt/graph.py` & `astronomer_cosmos-1.4.0a4/cosmos/dbt/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/dbt/project.py` & `astronomer_cosmos-1.4.0a4/cosmos/dbt/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/dbt/selector.py` & `astronomer_cosmos-1.4.0a4/cosmos/dbt/selector.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/dbt/parser/output.py` & `astronomer_cosmos-1.4.0a4/cosmos/dbt/parser/output.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/dbt/parser/project.py` & `astronomer_cosmos-1.4.0a4/cosmos/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/hooks/subprocess.py` & `astronomer_cosmos-1.4.0a4/cosmos/hooks/subprocess.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/operators/__init__.py` & `astronomer_cosmos-1.4.0a4/cosmos/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/operators/azure_container_instance.py` & `astronomer_cosmos-1.4.0a4/cosmos/operators/azure_container_instance.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/operators/base.py` & `astronomer_cosmos-1.4.0a4/cosmos/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/operators/docker.py` & `astronomer_cosmos-1.4.0a4/cosmos/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/operators/kubernetes.py` & `astronomer_cosmos-1.4.0a4/cosmos/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/operators/local.py` & `astronomer_cosmos-1.4.0a4/cosmos/operators/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,14 +402,15 @@
         Return a list of Dataset URIs (strings).
         """
         uris = []
         for completed in self.openlineage_events_completes:
             for output in getattr(completed, source):
                 dataset_uri = output.namespace + "/" + output.name
                 uris.append(dataset_uri)
+        logger.debug("URIs to be converted to Dataset: %s", uris)
         return [Dataset(uri) for uri in uris]
 
     def register_dataset(self, new_inlets: list[Dataset], new_outlets: list[Dataset]) -> None:
         """
         Register a list of datasets as outlets of the current task.
         Until Airflow 2.7, there was not a better interface to associate outlets to a task during execution.
         """
```

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/operators/virtualenv.py` & `astronomer_cosmos-1.4.0a4/cosmos/operators/virtualenv.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/plugin/__init__.py` & `astronomer_cosmos-1.4.0a4/cosmos/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/plugin/static/iframeResizer.contentWindow.min.js` & `astronomer_cosmos-1.4.0a4/cosmos/plugin/static/iframeResizer.contentWindow.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/plugin/static/iframeResizer.min.js` & `astronomer_cosmos-1.4.0a4/cosmos/plugin/static/iframeResizer.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/__init__.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/base.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/athena/access_key.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/athena/access_key.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/oauth.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/oauth.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/service_account_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/bigquery/service_account_keyfile_dict.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/bigquery/service_account_keyfile_dict.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/databricks/token.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/databricks/token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/exasol/user_pass.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/exasol/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/postgres/user_pass.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/postgres/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/redshift/user_pass.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/redshift/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/__init__.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_pass.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/snowflake/user_privatekey.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/snowflake/user_privatekey.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/spark/thrift.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/spark/thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/base.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/certificate.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/certificate.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/jwt.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/jwt.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/trino/ldap.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/trino/ldap.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/cosmos/profiles/vertica/user_pass.py` & `astronomer_cosmos-1.4.0a4/cosmos/profiles/vertica/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/.gitignore` & `astronomer_cosmos-1.4.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/LICENSE` & `astronomer_cosmos-1.4.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/README.rst` & `astronomer_cosmos-1.4.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0a2/pyproject.toml` & `astronomer_cosmos-1.4.0a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 ]
 dependencies = [
     "aenum",
     "attrs",
     "apache-airflow>=2.3.0",
     "importlib-metadata; python_version < '3.8'",
     "Jinja2>=3.0.0",
+    "pydantic>=1.10.0",
     "typing-extensions; python_version < '3.8'",
     "virtualenv",
 ]
 
 [project.optional-dependencies]
 dbt-all = [
     "dbt-athena",
@@ -81,17 +82,14 @@
 ]
 docker = [
     "apache-airflow-providers-docker>=3.5.0",
 ]
 kubernetes = [
     "apache-airflow-providers-cncf-kubernetes>=5.1.1",
 ]
-pydantic = [
-        "pydantic>=1.10.0",
-]
 azure-container-instance = [
     "apache-airflow-providers-microsoft-azure>=8.4.0",
 ]
 
 [project.entry-points.cosmos]
 provider_info = "cosmos:get_provider_info"
 
@@ -106,15 +104,15 @@
 [tool.hatch.version]
 path = "cosmos/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = ["/cosmos"]
 
 [tool.hatch.build.targets.wheel]
-packages = ["cosmos"]
+packages = ["/cosmos"]
 
 ######################################
 # TESTING
 ######################################
 
 [tool.hatch.envs.tests]
 dependencies = [
@@ -129,15 +127,15 @@
     "Werkzeug<3.0.0",
     "apache-airflow=={matrix:airflow}.0",
 ]
 pre-install-commands = ["sh scripts/test/pre-install-airflow.sh {matrix:airflow} {matrix:python}"]
 
 [[tool.hatch.envs.tests.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11"]
-airflow = ["2.3", "2.4", "2.5", "2.6", "2.7", "2.8"]
+airflow = ["2.3", "2.4", "2.5", "2.6", "2.7", "2.8", "2.9"]
 
 [tool.hatch.envs.tests.overrides]
 matrix.airflow.dependencies = [
     { value = "typing_extensions<4.6", if = ["2.6"] }
 ]
 
 [tool.hatch.envs.tests.scripts]
```

### Comparing `astronomer_cosmos-1.4.0a2/PKG-INFO` & `astronomer_cosmos-1.4.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: astronomer-cosmos
-Version: 1.4.0a2
+Version: 1.4.0a4
 Summary: Orchestrate your dbt projects in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://astronomer.github.io/astronomer-cosmos
 Project-URL: Source code, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: aenum
 Requires-Dist: apache-airflow>=2.3.0
 Requires-Dist: attrs
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: jinja2>=3.0.0
+Requires-Dist: pydantic>=1.10.0
 Requires-Dist: typing-extensions; python_version < '3.8'
 Requires-Dist: virtualenv
 Provides-Extra: all
 Requires-Dist: dbt-athena; extra == 'all'
 Requires-Dist: dbt-bigquery; extra == 'all'
 Requires-Dist: dbt-databricks; extra == 'all'
 Requires-Dist: dbt-exasol; extra == 'all'
@@ -82,16 +83,14 @@
 Requires-Dist: sphinx-autoapi; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
 Provides-Extra: kubernetes
 Requires-Dist: apache-airflow-providers-cncf-kubernetes>=5.1.1; extra == 'kubernetes'
 Provides-Extra: openlineage
 Requires-Dist: openlineage-airflow; extra == 'openlineage'
 Requires-Dist: openlineage-integration-common; extra == 'openlineage'
-Provides-Extra: pydantic
-Requires-Dist: pydantic>=1.10.0; extra == 'pydantic'
 Provides-Extra: tests
 Requires-Dist: mypy; extra == 'tests'
 Requires-Dist: packaging; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Requires-Dist: pytest-describe; extra == 'tests'
 Requires-Dist: pytest-dotenv; extra == 'tests'
 Requires-Dist: pytest-split; extra == 'tests'
```

