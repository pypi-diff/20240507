# Comparing `tmp/laktory-0.2.0.tar.gz` & `tmp/laktory-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laktory-0.2.0.tar", last modified: Thu May  2 06:11:56 2024, max compression
+gzip compressed data, was "laktory-0.2.1.tar", last modified: Tue May  7 03:26:49 2024, max compression
```

## Comparing `laktory-0.2.0.tar` & `laktory-0.2.1.tar`

### file list

```diff
@@ -1,493 +1,493 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.957663 laktory-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.869662 laktory-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.881662 laktory-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/ISSUE_TEMPLATE/bug.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/ISSUE_TEMPLATE/feature.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.881662 laktory-0.2.0/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/scripts/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/scripts/update_quickstart_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/scripts/write_release_body.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.881662 laktory-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/workflows/publish-doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/workflows/run_quickstart.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-02 06:11:47.000000 laktory-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-05-02 06:11:47.000000 laktory-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 06:11:47.000000 laktory-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-02 06:11:47.000000 laktory-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-02 06:11:56.957663 laktory-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-02 06:11:47.000000 laktory-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.881662 laktory-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.885662 laktory-0.2.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/datetime.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.885662 laktory-0.2.0/docs/api/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dispatcher/dispatcher.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dispatcher/dispatcherrunner.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dispatcher/jobrunner.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dispatcher/pipelinerunner.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.885662 laktory-0.2.0/docs/api/dlt/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dlt/apply_changes.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dlt/get_df.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dlt/is_debug.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dlt/is_mocked.md
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dlt/read.md
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dlt/read_stream.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.885662 laktory-0.2.0/docs/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/basemodel.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.889662 laktory-0.2.0/docs/api/models/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/accesscontrol.md
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/cluster.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/directory.md
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/externallocation.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/grants.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/group.md
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/job.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/metastore.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/metastoreassignment.md
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/metastoredataaccess.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/mwspermissionassignment.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/notebook.md
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/secret.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/secretacl.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/secretscope.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/serviceprincipal.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/serviceprincipalrole.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/sqlquery.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/user.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/userrole.md
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/warehouse.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/workspacefile.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/dataevent.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/dataeventheader.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/dataproducer.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.889662 laktory-0.2.0/docs/api/models/datasources/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/datasources/basedatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/datasources/eventdatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/datasources/tabledatasource.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.889662 laktory-0.2.0/docs/api/models/providers/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/providers/aws.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/providers/azure.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/providers/azurepulumi.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/providers/databricks.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.893662 laktory-0.2.0/docs/api/models/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/resources/baseresource.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/resources/pulumiresource.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/resources/terraformresource.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.893662 laktory-0.2.0/docs/api/models/spark/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/spark/sparkchain.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/spark/sparkchainnode.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/spark/sparkfuncarg.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.893662 laktory-0.2.0/docs/api/models/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/catalog.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/column.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/schema.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/table.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/tablebuilder.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/tableexpectation.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/volume.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.893662 laktory-0.2.0/docs/api/models/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/stacks/pulumistack.md
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/stacks/stack.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/stacks/terraformstack.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.869662 laktory-0.2.0/docs/api/spark/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.893662 laktory-0.2.0/docs/api/spark/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/dataframe/groupby_and_agg.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/dataframe/has_column.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/dataframe/schema_flat.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/dataframe/show_string.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/dataframe/smart_join.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/dataframe/window_filter.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.897662 laktory-0.2.0/docs/api/spark/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/_constants.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/add.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/convert_units.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/div.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/mul.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/poly1.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/poly2.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/roundp.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/scaled_power.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/string_split.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/sub.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/uuid.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.897662 laktory-0.2.0/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/dataevent.md
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/deployment.md
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/design.md
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/governance.md
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/models.md
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/spark.md
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/stack.md
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/table.md
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/tablebuilder.md
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/variables.md
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/demos.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.901662 laktory-0.2.0/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/catalog.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/compute.md
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/job.md
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/secrets.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/table.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/users.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.905662 laktory-0.2.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    20095 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/databricks.png
--rw-r--r--   0 runner    (1001) docker     (127)   588404 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/delta_live_tables.png
--rw-r--r--   0 runner    (1001) docker     (127)   187140 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/dlt_debug.png
--rw-r--r--   0 runner    (1001) docker     (127)   307164 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/kappa.png
--rw-r--r--   0 runner    (1001) docker     (127)   118303 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/lakehouse.png
--rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/logo_sg.png
--rw-r--r--   0 runner    (1001) docker     (127)    41747 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/logo_sg_ltb.png
--rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/logo_sw.png
--rw-r--r--   0 runner    (1001) docker     (127)    41214 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/logo_sw_ltw.png
--rw-r--r--   0 runner    (1001) docker     (127)   644132 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/medaillon_complex.png
--rw-r--r--   0 runner    (1001) docker     (127)   449508 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/medallion.png
--rw-r--r--   0 runner    (1001) docker     (127)    48171 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/okube.png
--rw-r--r--   0 runner    (1001) docker     (127)    92500 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/pl_quickstart.png
--rw-r--r--   0 runner    (1001) docker     (127)   168057 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/pl_stock_prices.png
--rw-r--r--   0 runner    (1001) docker     (127)   153436 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/pl_stock_prices_simple.png
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/pulumi.png
--rw-r--r--   0 runner    (1001) docker     (127)   197565 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/stock_prices_lineage.png
--rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/terraform.png
--rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/what_is_laktory.png
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/lakehouseascode.md
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.909663 laktory-0.2.0/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/stylesheets/mkdocstrings.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.909663 laktory-0.2.0/laktory/
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.909663 laktory-0.2.0/laktory/_testing/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_testing/stackvalidator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_testing/stockprices.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.913663 laktory-0.2.0/laktory/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_quickstart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_write.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/quickstart_stack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2702 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.913663 laktory-0.2.0/laktory/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/dispatcher/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/dispatcher/dispatcherrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/dispatcher/jobrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/dispatcher/pipelinerunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.913663 laktory-0.2.0/laktory/dlt/
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/dlt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.913663 laktory-0.2.0/laktory/models/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.913663 laktory-0.2.0/laktory/models/azurenative/
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/azurenative/storageblob.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/basemodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.921663 laktory-0.2.0/laktory/models/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/accesscontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/dbfsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/externallocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/groupmember.py
--rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/metastoreassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/metastoredataaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/mwspermissionassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/secretacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/secretscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/serviceprincipal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/serviceprincipalrole.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/sqlquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/userrole.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/workspacefile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14591 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/dataevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/dataeventheader.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/dataproducer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.921663 laktory-0.2.0/laktory/models/datasources/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/datasources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/datasources/basedatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/datasources/eventdatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/datasources/tabledatasource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.921663 laktory-0.2.0/laktory/models/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/cataloggrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/connectiongrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/externallocationgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/functiongrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/metastoregrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/registeredmodelgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/schemagrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/sharegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/storagecredentialgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/tablegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/viewgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/volumegrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.925663 laktory-0.2.0/laktory/models/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/providers/awsprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/providers/azureprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/providers/azurepulumiprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/providers/baseprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/providers/databricksprovider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.925663 laktory-0.2.0/laktory/models/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/resources/baseresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/resources/pulumiresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/resources/terraformresource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.925663 laktory-0.2.0/laktory/models/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/spark/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/spark/sparkchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/spark/sparkchainnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/spark/sparkfuncarg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.929663 laktory-0.2.0/laktory/models/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12014 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/tablebuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/tableexpectation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.929663 laktory-0.2.0/laktory/models/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/stacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/stacks/pulumistack.py
--rw-r--r--   0 runner    (1001) docker     (127)    18667 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/stacks/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/stacks/terraformstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.873662 laktory-0.2.0/laktory/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.929663 laktory-0.2.0/laktory/resources/data/
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/resources/data/stock_prices.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.929663 laktory-0.2.0/laktory/resources/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/resources/notebooks/dlt_brz_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/resources/notebooks/dlt_gld_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/resources/notebooks/dlt_slv_star_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/resources/notebooks/dlt_slv_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.929663 laktory-0.2.0/laktory/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.929663 laktory-0.2.0/laktory/spark/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/groupby_and_agg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/has_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/schema_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/show_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/smart_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/watermark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/window_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.933663 laktory-0.2.0/laktory/spark/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/functions/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/functions/logical.py
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/functions/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/functions/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.957663 laktory-0.2.0/laktory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-02 06:11:56.000000 laktory-0.2.0/laktory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-02 06:11:56.000000 laktory-0.2.0/laktory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:11:56.000000 laktory-0.2.0/laktory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 06:11:56.000000 laktory-0.2.0/laktory.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-02 06:11:56.000000 laktory-0.2.0/laktory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 06:11:56.000000 laktory-0.2.0/laktory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-02 06:11:47.000000 laktory-0.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-02 06:11:47.000000 laktory-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.933663 laktory-0.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-02 06:11:47.000000 laktory-0.2.0/scripts/databricks_api_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 06:11:47.000000 laktory-0.2.0/scripts/test_computed_filed.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 06:11:47.000000 laktory-0.2.0/scripts/test_db_connect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.933663 laktory-0.2.0/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 06:11:47.000000 laktory-0.2.0/settings/dev.env
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:11:56.957663 laktory-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.937663 laktory-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/build_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.941663 laktory-0.2.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.941663 laktory-0.2.0/tests/data/brz_stock_prices/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/brz_stock_prices/._SUCCESS.crc
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/brz_stock_prices/.part-00000-aff20661-c55f-4489-86fc-8336e06ee376-c000.snappy.parquet.crc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/brz_stock_prices/_SUCCESS
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/brz_stock_prices/part-00000-aff20661-c55f-4489-86fc-8336e06ee376-c000.snappy.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.877662 laktory-0.2.0/tests/data/events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.877662 laktory-0.2.0/tests/data/events/yahoo-finance/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.877662 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.877662 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.877662 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.941663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AAPL_20230901T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AMZN_20230901T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_GOOGL_20230901T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_MSFT_20230901T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.941663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AAPL_20230905T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AMZN_20230905T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_GOOGL_20230905T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_MSFT_20230905T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.941663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AAPL_20230906T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AMZN_20230906T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_GOOGL_20230906T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_MSFT_20230906T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.941663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AAPL_20230907T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AMZN_20230907T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_GOOGL_20230907T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_MSFT_20230907T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.945663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AAPL_20230908T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AMZN_20230908T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_GOOGL_20230908T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_MSFT_20230908T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.945663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AAPL_20230911T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AMZN_20230911T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_GOOGL_20230911T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_MSFT_20230911T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.945663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AAPL_20230912T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AMZN_20230912T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_GOOGL_20230912T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_MSFT_20230912T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.945663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AAPL_20230913T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AMZN_20230913T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_GOOGL_20230913T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_MSFT_20230913T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.945663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AAPL_20230914T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AMZN_20230914T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_GOOGL_20230914T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_MSFT_20230914T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.949663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AAPL_20230915T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AMZN_20230915T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_GOOGL_20230915T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_MSFT_20230915T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.949663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AAPL_20230918T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AMZN_20230918T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_GOOGL_20230918T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_MSFT_20230918T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.949663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AAPL_20230919T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AMZN_20230919T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_GOOGL_20230919T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_MSFT_20230919T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.949663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AAPL_20230920T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AMZN_20230920T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_GOOGL_20230920T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_MSFT_20230920T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.949663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AAPL_20230921T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AMZN_20230921T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_GOOGL_20230921T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_MSFT_20230921T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.953663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AAPL_20230922T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AMZN_20230922T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_GOOGL_20230922T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_MSFT_20230922T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.953663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AAPL_20230925T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AMZN_20230925T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_GOOGL_20230925T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_MSFT_20230925T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.953663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AAPL_20230926T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AMZN_20230926T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_GOOGL_20230926T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_MSFT_20230926T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.953663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AAPL_20230927T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AMZN_20230927T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_GOOGL_20230927T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_MSFT_20230927T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.953663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AAPL_20230928T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AMZN_20230928T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_GOOGL_20230928T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_MSFT_20230928T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.953663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AAPL_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AMZN_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_GOOGL_20230929T000000000Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_MSFT_20230929T000000000Z.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.957663 laktory-0.2.0/tests/data/slv_stock_meta/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_meta/._SUCCESS.crc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_meta/.part-00000-d86fbfe6-5d98-43f6-827b-c18d9f79622f-c000.snappy.parquet.crc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_meta/_SUCCESS
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_meta/part-00000-d86fbfe6-5d98-43f6-827b-c18d9f79622f-c000.snappy.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.957663 laktory-0.2.0/tests/data/slv_stock_prices/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_prices/._SUCCESS.crc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_prices/.part-00000-d12f5de4-d8dd-46fc-b00a-c3c7dc6edc32-c000.snappy.parquet.crc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_prices/_SUCCESS
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_prices/part-00000-d12f5de4-d8dd-46fc-b00a-c3c7dc6edc32-c000.snappy.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/stack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/stack_empty.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/stockprices0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/stockprices1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/stockprices2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_baseresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_dataevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_datasources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_dbfsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_dlt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_spark_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_spark_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_spark_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    26494 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_table_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_workspacefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.487642 laktory-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.395642 laktory-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.403642 laktory-0.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/ISSUE_TEMPLATE/feature.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.407642 laktory-0.2.1/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/scripts/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/scripts/update_quickstart_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/scripts/write_release_body.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.407642 laktory-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/workflows/publish-doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/workflows/run_quickstart.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-07 03:26:40.000000 laktory-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-07 03:26:40.000000 laktory-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-05-07 03:26:40.000000 laktory-0.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 03:26:40.000000 laktory-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 03:26:40.000000 laktory-0.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-07 03:26:49.487642 laktory-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-07 03:26:40.000000 laktory-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.407642 laktory-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.407642 laktory-0.2.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/datetime.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.407642 laktory-0.2.1/docs/api/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dispatcher/dispatcher.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dispatcher/dispatcherrunner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dispatcher/jobrunner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dispatcher/pipelinerunner.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.411642 laktory-0.2.1/docs/api/dlt/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dlt/apply_changes.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dlt/get_df.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dlt/is_debug.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dlt/is_mocked.md
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dlt/read.md
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/dlt/read_stream.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.411642 laktory-0.2.1/docs/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/basemodel.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.415642 laktory-0.2.1/docs/api/models/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/accesscontrol.md
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/cluster.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/directory.md
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/externallocation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/grants.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/group.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/job.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/metastore.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/metastoreassignment.md
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/metastoredataaccess.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/mwspermissionassignment.md
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/notebook.md
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/secret.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/secretacl.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/secretscope.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/serviceprincipal.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/serviceprincipalrole.md
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/sqlquery.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/user.md
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/userrole.md
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/warehouse.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/databricks/workspacefile.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/dataevent.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/dataeventheader.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/dataproducer.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.415642 laktory-0.2.1/docs/api/models/datasources/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/datasources/basedatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/datasources/eventdatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/datasources/tabledatasource.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.415642 laktory-0.2.1/docs/api/models/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/providers/aws.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/providers/azure.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/providers/azurepulumi.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/providers/databricks.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.415642 laktory-0.2.1/docs/api/models/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/resources/baseresource.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/resources/pulumiresource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/resources/terraformresource.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.415642 laktory-0.2.1/docs/api/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/spark/sparkchain.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/spark/sparkchainnode.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/spark/sparkfuncarg.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.419642 laktory-0.2.1/docs/api/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/catalog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/column.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/schema.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/tablebuilder.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/tableexpectation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/sql/volume.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.419642 laktory-0.2.1/docs/api/models/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/stacks/pulumistack.md
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/stacks/stack.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/models/stacks/terraformstack.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.395642 laktory-0.2.1/docs/api/spark/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.419642 laktory-0.2.1/docs/api/spark/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/dataframe/groupby_and_agg.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/dataframe/has_column.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/dataframe/schema_flat.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/dataframe/show_string.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/dataframe/smart_join.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/dataframe/window_filter.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.423642 laktory-0.2.1/docs/api/spark/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/_constants.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/add.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/convert_units.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/div.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/mul.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/poly1.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/poly2.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/roundp.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/scaled_power.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/string_split.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/sub.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/api/spark/functions/uuid.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.423642 laktory-0.2.1/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/dataevent.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/deployment.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/governance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/models.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/spark.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/stack.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/tablebuilder.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/concepts/variables.md
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/demos.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.427642 laktory-0.2.1/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/catalog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/compute.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/job.md
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/secrets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/guides/users.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.431642 laktory-0.2.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20095 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/databricks.png
+-rw-r--r--   0 runner    (1001) docker     (127)   588404 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/delta_live_tables.png
+-rw-r--r--   0 runner    (1001) docker     (127)   187140 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/dlt_debug.png
+-rw-r--r--   0 runner    (1001) docker     (127)   307164 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/kappa.png
+-rw-r--r--   0 runner    (1001) docker     (127)   118303 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/lakehouse.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/logo_sg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41747 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/logo_sg_ltb.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/logo_sw.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41214 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/logo_sw_ltw.png
+-rw-r--r--   0 runner    (1001) docker     (127)   644132 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/medaillon_complex.png
+-rw-r--r--   0 runner    (1001) docker     (127)   449508 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/medallion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48171 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/okube.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92500 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/pl_quickstart.png
+-rw-r--r--   0 runner    (1001) docker     (127)   168057 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/pl_stock_prices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   153436 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/pl_stock_prices_simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/pulumi.png
+-rw-r--r--   0 runner    (1001) docker     (127)   197565 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/stock_prices_lineage.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/terraform.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/images/what_is_laktory.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/lakehouseascode.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.431642 laktory-0.2.1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-07 03:26:40.000000 laktory-0.2.1/docs/stylesheets/mkdocstrings.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.435642 laktory-0.2.1/laktory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.435642 laktory-0.2.1/laktory/_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_testing/stackvalidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_testing/stockprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.439642 laktory-0.2.1/laktory/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_quickstart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/cli/quickstart_stack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2702 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.439642 laktory-0.2.1/laktory/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/dispatcher/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/dispatcher/dispatcherrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/dispatcher/jobrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/dispatcher/pipelinerunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.439642 laktory-0.2.1/laktory/dlt/
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/dlt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.439642 laktory-0.2.1/laktory/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.439642 laktory-0.2.1/laktory/models/azurenative/
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/azurenative/storageblob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/basemodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.443642 laktory-0.2.1/laktory/models/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/accesscontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/dbfsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/externallocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/grants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/groupmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/metastoreassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/metastoredataaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/mwspermissionassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/secretacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/secretscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/serviceprincipal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/serviceprincipalrole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/sqlquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/userrole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/databricks/workspacefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14591 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/dataevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/dataeventheader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/dataproducer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.447642 laktory-0.2.1/laktory/models/datasources/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/datasources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/datasources/basedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/datasources/eventdatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/datasources/tabledatasource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.447642 laktory-0.2.1/laktory/models/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/cataloggrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/connectiongrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/externallocationgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/functiongrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/metastoregrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/registeredmodelgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/schemagrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/sharegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/storagecredentialgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/tablegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/viewgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/grants/volumegrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.451642 laktory-0.2.1/laktory/models/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/providers/awsprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/providers/azureprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/providers/azurepulumiprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/providers/baseprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/providers/databricksprovider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.451642 laktory-0.2.1/laktory/models/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/resources/baseresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/resources/pulumiresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/resources/terraformresource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.451642 laktory-0.2.1/laktory/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/spark/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/spark/sparkchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/spark/sparkchainnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/spark/sparkfuncarg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.451642 laktory-0.2.1/laktory/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12014 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/tablebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/tableexpectation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/sql/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.455642 laktory-0.2.1/laktory/models/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/stacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/stacks/pulumistack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18667 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/stacks/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/models/stacks/terraformstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.399642 laktory-0.2.1/laktory/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.455642 laktory-0.2.1/laktory/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/resources/data/stock_prices.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.455642 laktory-0.2.1/laktory/resources/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/resources/notebooks/dlt_brz_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/resources/notebooks/dlt_gld_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/resources/notebooks/dlt_slv_star_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/resources/notebooks/dlt_slv_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.455642 laktory-0.2.1/laktory/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.455642 laktory-0.2.1/laktory/spark/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/groupby_and_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/has_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/schema_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/show_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/smart_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/watermark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/dataframe/window_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.455642 laktory-0.2.1/laktory/spark/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/functions/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/functions/logical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/functions/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/spark/functions/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-07 03:26:40.000000 laktory-0.2.1/laktory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.483642 laktory-0.2.1/laktory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-07 03:26:49.000000 laktory-0.2.1/laktory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-07 03:26:49.000000 laktory-0.2.1/laktory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 03:26:49.000000 laktory-0.2.1/laktory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 03:26:49.000000 laktory-0.2.1/laktory.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-07 03:26:49.000000 laktory-0.2.1/laktory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 03:26:49.000000 laktory-0.2.1/laktory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-07 03:26:40.000000 laktory-0.2.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-07 03:26:40.000000 laktory-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.459642 laktory-0.2.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-07 03:26:40.000000 laktory-0.2.1/scripts/databricks_api_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 03:26:40.000000 laktory-0.2.1/scripts/test_computed_filed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 03:26:40.000000 laktory-0.2.1/scripts/test_db_connect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.459642 laktory-0.2.1/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 03:26:40.000000 laktory-0.2.1/settings/dev.env
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:26:49.487642 laktory-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.463642 laktory-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/build_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.467642 laktory-0.2.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.467642 laktory-0.2.1/tests/data/brz_stock_prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/brz_stock_prices/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/brz_stock_prices/.part-00000-aff20661-c55f-4489-86fc-8336e06ee376-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/brz_stock_prices/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/brz_stock_prices/part-00000-aff20661-c55f-4489-86fc-8336e06ee376-c000.snappy.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.399642 laktory-0.2.1/tests/data/events/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.399642 laktory-0.2.1/tests/data/events/yahoo-finance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.399642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.399642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.403642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.467642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AAPL_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AMZN_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_GOOGL_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_MSFT_20230901T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.467642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AAPL_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AMZN_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_GOOGL_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_MSFT_20230905T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.467642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AAPL_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AMZN_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_GOOGL_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_MSFT_20230906T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.467642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AAPL_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AMZN_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_GOOGL_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_MSFT_20230907T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.471642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AAPL_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AMZN_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_GOOGL_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_MSFT_20230908T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.471642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AAPL_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AMZN_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_GOOGL_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_MSFT_20230911T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.471642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AAPL_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AMZN_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_GOOGL_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_MSFT_20230912T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.471642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AAPL_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AMZN_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_GOOGL_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_MSFT_20230913T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.471642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AAPL_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AMZN_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_GOOGL_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_MSFT_20230914T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.475642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AAPL_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AMZN_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_GOOGL_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_MSFT_20230915T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.475642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AAPL_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AMZN_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_GOOGL_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_MSFT_20230918T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.475642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AAPL_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AMZN_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_GOOGL_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_MSFT_20230919T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.475642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AAPL_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AMZN_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_GOOGL_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_MSFT_20230920T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.475642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AAPL_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AMZN_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_GOOGL_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_MSFT_20230921T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.479642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AAPL_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AMZN_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_GOOGL_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_MSFT_20230922T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.479642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AAPL_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AMZN_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_GOOGL_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_MSFT_20230925T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.479642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AAPL_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AMZN_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_GOOGL_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_MSFT_20230926T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.479642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AAPL_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AMZN_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_GOOGL_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_MSFT_20230927T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.479642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AAPL_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AMZN_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_GOOGL_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_MSFT_20230928T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.483642 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AAPL_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AMZN_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_GOOGL_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_MSFT_20230929T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.483642 laktory-0.2.1/tests/data/slv_stock_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_meta/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_meta/.part-00000-d86fbfe6-5d98-43f6-827b-c18d9f79622f-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_meta/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_meta/part-00000-d86fbfe6-5d98-43f6-827b-c18d9f79622f-c000.snappy.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:49.483642 laktory-0.2.1/tests/data/slv_stock_prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_prices/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_prices/.part-00000-d12f5de4-d8dd-46fc-b00a-c3c7dc6edc32-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_prices/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/slv_stock_prices/part-00000-d12f5de4-d8dd-46fc-b00a-c3c7dc6edc32-c000.snappy.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/stack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/stack_empty.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/stockprices0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/stockprices1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/data/stockprices2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_baseresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_dataevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_dbfsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_dlt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_spark_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_spark_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_spark_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26494 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_table_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-07 03:26:40.000000 laktory-0.2.1/tests/test_workspacefile.py
```

### Comparing `laktory-0.2.0/.github/ISSUE_TEMPLATE/bug.yaml` & `laktory-0.2.1/.github/ISSUE_TEMPLATE/bug.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/.github/ISSUE_TEMPLATE/feature.yaml` & `laktory-0.2.1/.github/ISSUE_TEMPLATE/feature.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/.github/scripts/bump_version.py` & `laktory-0.2.1/.github/scripts/bump_version.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/.github/scripts/update_quickstart_stack.py` & `laktory-0.2.1/.github/scripts/update_quickstart_stack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/.github/scripts/write_release_body.py` & `laktory-0.2.1/.github/scripts/write_release_body.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/.github/workflows/release.yml` & `laktory-0.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/.github/workflows/run_quickstart.yml` & `laktory-0.2.1/.github/workflows/run_quickstart.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/.github/workflows/test.yml` & `laktory-0.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/.gitignore` & `laktory-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/CHANGELOG.md` & `laktory-0.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 # Release History
 
-## [0.2.0] - Unreleased
+## [0.2.1] - Unreleased
+### Added
+* Support for spark chain for a data source
+* Support for broadcasting in a data source
+* YAML model dump for all base models
+### Fixed
+* Function selection for pyspark connect DataFrames
+
+## [0.2.0] - 2024-05-02
 ### Added
 * `SparkChain` a high level class allowing to declare and execute spark operations on a dataframe 
 * `SparkColumnNode` the node of a `SparkChain` that builds a new column
 * `SparkTableNode` the node of a `SparkChain` that returns a new DataFrame
 * Moved `filter`, `selects` and `watermarks` properties to `models.BaseDataSource` so that it can be used for all source types
 * `models.BaseDataSource` `renames` attribute for renaming columns of the source table
 * `models.BaseDataSource` `drops` attribute for dropping columns of the source table
```

### Comparing `laktory-0.2.0/LICENSE` & `laktory-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/PKG-INFO` & `laktory-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laktory
-Version: 0.2.0
+Version: 0.2.1
 Summary: A DataOps framework for building a lakehouse
 Author-email: Olivier Soucy <olivier.soucy@okube.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/opencubes-ai/laktory
 Project-URL: Bug Tracker, https://github.com/opencubes-ai/laktory/issues
 Keywords: one,two
 Classifier: Development Status :: 4 - Beta
```

### Comparing `laktory-0.2.0/README.md` & `laktory-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/api/models/databricks/cluster.md` & `laktory-0.2.1/docs/api/models/databricks/cluster.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/api/models/databricks/grants.md` & `laktory-0.2.1/docs/api/models/databricks/grants.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/api/models/databricks/job.md` & `laktory-0.2.1/docs/api/models/databricks/job.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/api/models/databricks/metastoredataaccess.md` & `laktory-0.2.1/docs/api/models/databricks/metastoredataaccess.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/concepts/cli.md` & `laktory-0.2.1/docs/concepts/cli.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/concepts/dataevent.md` & `laktory-0.2.1/docs/concepts/dataevent.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/concepts/deployment.md` & `laktory-0.2.1/docs/concepts/deployment.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/concepts/design.md` & `laktory-0.2.1/docs/concepts/design.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/concepts/governance.md` & `laktory-0.2.1/docs/concepts/governance.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/concepts/models.md` & `laktory-0.2.1/docs/concepts/models.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/concepts/pipeline.md` & `laktory-0.2.1/docs/concepts/pipeline.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/concepts/spark.md` & `laktory-0.2.1/docs/concepts/spark.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/concepts/stack.md` & `laktory-0.2.1/docs/concepts/stack.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/concepts/table.md` & `laktory-0.2.1/docs/concepts/table.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/concepts/tablebuilder.md` & `laktory-0.2.1/docs/concepts/tablebuilder.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/concepts/variables.md` & `laktory-0.2.1/docs/concepts/variables.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/databricks.png` & `laktory-0.2.1/docs/images/databricks.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/delta_live_tables.png` & `laktory-0.2.1/docs/images/delta_live_tables.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/dlt_debug.png` & `laktory-0.2.1/docs/images/dlt_debug.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/kappa.png` & `laktory-0.2.1/docs/images/kappa.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/lakehouse.png` & `laktory-0.2.1/docs/images/lakehouse.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/logo_sg.png` & `laktory-0.2.1/docs/images/logo_sg.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/logo_sg_ltb.png` & `laktory-0.2.1/docs/images/logo_sg_ltb.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/logo_sw.png` & `laktory-0.2.1/docs/images/logo_sw.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/logo_sw_ltw.png` & `laktory-0.2.1/docs/images/logo_sw_ltw.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/medaillon_complex.png` & `laktory-0.2.1/docs/images/medaillon_complex.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/medallion.png` & `laktory-0.2.1/docs/images/medallion.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/okube.png` & `laktory-0.2.1/docs/images/okube.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/pl_quickstart.png` & `laktory-0.2.1/docs/images/pl_quickstart.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/pl_stock_prices.png` & `laktory-0.2.1/docs/images/pl_stock_prices.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/pl_stock_prices_simple.png` & `laktory-0.2.1/docs/images/pl_stock_prices_simple.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/pulumi.png` & `laktory-0.2.1/docs/images/pulumi.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/stock_prices_lineage.png` & `laktory-0.2.1/docs/images/stock_prices_lineage.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/terraform.png` & `laktory-0.2.1/docs/images/terraform.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/images/what_is_laktory.png` & `laktory-0.2.1/docs/images/what_is_laktory.png`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/index.md` & `laktory-0.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/install.md` & `laktory-0.2.1/docs/install.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/lakehouseascode.md` & `laktory-0.2.1/docs/lakehouseascode.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/quickstart.md` & `laktory-0.2.1/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/docs/stylesheets/mkdocstrings.css` & `laktory-0.2.1/docs/stylesheets/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/__init__.py` & `laktory-0.2.1/laktory/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/_logger.py` & `laktory-0.2.1/laktory/_logger.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/_parsers.py` & `laktory-0.2.1/laktory/_parsers.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/_settings.py` & `laktory-0.2.1/laktory/_settings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/_testing/stackvalidator.py` & `laktory-0.2.1/laktory/_testing/stackvalidator.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/_testing/stockprices.py` & `laktory-0.2.1/laktory/_testing/stockprices.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/cli/_common.py` & `laktory-0.2.1/laktory/cli/_common.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/cli/_deploy.py` & `laktory-0.2.1/laktory/cli/_deploy.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/cli/_init.py` & `laktory-0.2.1/laktory/cli/_init.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/cli/_preview.py` & `laktory-0.2.1/laktory/cli/_preview.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/cli/_quickstart.py` & `laktory-0.2.1/laktory/cli/_quickstart.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/cli/_run.py` & `laktory-0.2.1/laktory/cli/_run.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/cli/_write.py` & `laktory-0.2.1/laktory/cli/_write.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/cli/quickstart_stack.yaml` & `laktory-0.2.1/laktory/cli/quickstart_stack.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/constants.py` & `laktory-0.2.1/laktory/constants.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/datetime.py` & `laktory-0.2.1/laktory/datetime.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/dispatcher/dispatcher.py` & `laktory-0.2.1/laktory/dispatcher/dispatcher.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/dispatcher/dispatcherrunner.py` & `laktory-0.2.1/laktory/dispatcher/dispatcherrunner.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/dispatcher/jobrunner.py` & `laktory-0.2.1/laktory/dispatcher/jobrunner.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/dispatcher/pipelinerunner.py` & `laktory-0.2.1/laktory/dispatcher/pipelinerunner.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/dlt/__init__.py` & `laktory-0.2.1/laktory/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/azurenative/storageblob.py` & `laktory-0.2.1/laktory/models/azurenative/storageblob.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/basemodel.py` & `laktory-0.2.1/laktory/models/basemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,17 @@
                     d = inject_includes(d)
             return d
 
         data = inject_includes(yaml.safe_load(fp))
 
         return cls.model_validate(data)
 
+    def model_dump_yaml(self, *args, **kwargs):
+        return yaml.dump(self.model_dump(*args, **kwargs))
+
     @classmethod
     def model_validate_json_file(cls, fp: TextIO) -> Model:
         """
         Load model from json file object
 
         Parameters
         ----------
```

### Comparing `laktory-0.2.0/laktory/models/databricks/__init__.py` & `laktory-0.2.1/laktory/models/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/accesscontrol.py` & `laktory-0.2.1/laktory/models/databricks/accesscontrol.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/cluster.py` & `laktory-0.2.1/laktory/models/databricks/cluster.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/dbfsfile.py` & `laktory-0.2.1/laktory/models/databricks/dbfsfile.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/directory.py` & `laktory-0.2.1/laktory/models/databricks/directory.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/externallocation.py` & `laktory-0.2.1/laktory/models/databricks/externallocation.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/grants.py` & `laktory-0.2.1/laktory/models/databricks/grants.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/group.py` & `laktory-0.2.1/laktory/models/databricks/group.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/groupmember.py` & `laktory-0.2.1/laktory/models/databricks/groupmember.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/job.py` & `laktory-0.2.1/laktory/models/databricks/job.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/metastore.py` & `laktory-0.2.1/laktory/models/databricks/metastore.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/metastoreassignment.py` & `laktory-0.2.1/laktory/models/databricks/metastoreassignment.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/metastoredataaccess.py` & `laktory-0.2.1/laktory/models/databricks/metastoredataaccess.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/mwspermissionassignment.py` & `laktory-0.2.1/laktory/models/databricks/mwspermissionassignment.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/notebook.py` & `laktory-0.2.1/laktory/models/databricks/notebook.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/permissions.py` & `laktory-0.2.1/laktory/models/databricks/permissions.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/pipeline.py` & `laktory-0.2.1/laktory/models/databricks/pipeline.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/secret.py` & `laktory-0.2.1/laktory/models/databricks/secret.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/secretacl.py` & `laktory-0.2.1/laktory/models/databricks/secretacl.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/secretscope.py` & `laktory-0.2.1/laktory/models/databricks/secretscope.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/serviceprincipal.py` & `laktory-0.2.1/laktory/models/databricks/serviceprincipal.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/serviceprincipalrole.py` & `laktory-0.2.1/laktory/models/databricks/serviceprincipalrole.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/sqlquery.py` & `laktory-0.2.1/laktory/models/databricks/sqlquery.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/user.py` & `laktory-0.2.1/laktory/models/databricks/user.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/userrole.py` & `laktory-0.2.1/laktory/models/databricks/userrole.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/warehouse.py` & `laktory-0.2.1/laktory/models/databricks/warehouse.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/databricks/workspacefile.py` & `laktory-0.2.1/laktory/models/databricks/workspacefile.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/dataevent.py` & `laktory-0.2.1/laktory/models/dataevent.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/dataeventheader.py` & `laktory-0.2.1/laktory/models/dataeventheader.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/dataproducer.py` & `laktory-0.2.1/laktory/models/dataproducer.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/datasources/basedatasource.py` & `laktory-0.2.1/laktory/models/datasources/basedatasource.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import abstractmethod
 from typing import Any
 from typing import Union
 from laktory.spark import DataFrame
 from pydantic import Field
 
 from laktory.models.basemodel import BaseModel
+from laktory.models.spark.sparkchain import SparkChain
 
 
 class Watermark(BaseModel):
     """
     Definition of a spark structured streaming watermark for joining data
     streams.
 
@@ -50,17 +51,19 @@
         Spark structured streaming watermark specifications
 
     """
 
     drops: Union[list, None] = None
     filter: Union[str, None] = None
     mock_df: Any = Field(default=None, exclude=True)
+    broadcast: Union[bool, None] = False
     read_as_stream: Union[bool, None] = True
     renames: Union[dict[str, str], None] = None
     selects: Union[list[str], dict[str, str], None] = None
+    spark_chain: Union[SparkChain, None] = None
     watermark: Union[Watermark, None] = None
 
     def read(self, spark) -> DataFrame:
         """
         Read data with options specified in attributes.
 
         Parameters
@@ -109,13 +112,21 @@
         # Apply Watermark
         if self.watermark:
             df = df.withWatermark(
                 self.watermark.column,
                 self.watermark.threshold,
             )
 
+        # Broadcast
+        if self.broadcast:
+            df = F.broadcast(df)
+
+        # SparkChain
+        if self.spark_chain:
+            df = self.spark_chain.execute(df, udfs=None, spark=df.sparkSession)
+
         return df
 
     @property
     def is_cdc(self) -> bool:
         """If `True` source data is a change data capture (CDC)"""
         return getattr(self, "cdc", None) is not None
```

### Comparing `laktory-0.2.0/laktory/models/datasources/eventdatasource.py` & `laktory-0.2.1/laktory/models/datasources/eventdatasource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/datasources/tabledatasource.py` & `laktory-0.2.1/laktory/models/datasources/tabledatasource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/grants/__init__.py` & `laktory-0.2.1/laktory/models/grants/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/grants/cataloggrant.py` & `laktory-0.2.1/laktory/models/grants/cataloggrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/grants/connectiongrant.py` & `laktory-0.2.1/laktory/models/grants/connectiongrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/grants/externallocationgrant.py` & `laktory-0.2.1/laktory/models/grants/externallocationgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/grants/functiongrant.py` & `laktory-0.2.1/laktory/models/grants/functiongrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/grants/metastoregrant.py` & `laktory-0.2.1/laktory/models/grants/metastoregrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/grants/registeredmodelgrant.py` & `laktory-0.2.1/laktory/models/grants/registeredmodelgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/grants/schemagrant.py` & `laktory-0.2.1/laktory/models/grants/schemagrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/grants/sharegrant.py` & `laktory-0.2.1/laktory/models/grants/sharegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/grants/storagecredentialgrant.py` & `laktory-0.2.1/laktory/models/grants/storagecredentialgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/grants/tablegrant.py` & `laktory-0.2.1/laktory/models/grants/tablegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/grants/viewgrant.py` & `laktory-0.2.1/laktory/models/grants/viewgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/grants/volumegrant.py` & `laktory-0.2.1/laktory/models/grants/volumegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/providers/awsprovider.py` & `laktory-0.2.1/laktory/models/providers/awsprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/providers/azureprovider.py` & `laktory-0.2.1/laktory/models/providers/azureprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/providers/azurepulumiprovider.py` & `laktory-0.2.1/laktory/models/providers/azurepulumiprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/providers/baseprovider.py` & `laktory-0.2.1/laktory/models/providers/baseprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/providers/databricksprovider.py` & `laktory-0.2.1/laktory/models/providers/databricksprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/resources/baseresource.py` & `laktory-0.2.1/laktory/models/resources/baseresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/resources/pulumiresource.py` & `laktory-0.2.1/laktory/models/resources/pulumiresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/resources/terraformresource.py` & `laktory-0.2.1/laktory/models/resources/terraformresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/spark/_common.py` & `laktory-0.2.1/laktory/models/spark/_common.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/spark/sparkchain.py` & `laktory-0.2.1/laktory/models/spark/sparkchain.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/spark/sparkchainnode.py` & `laktory-0.2.1/laktory/models/spark/sparkchainnode.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,15 @@
 
         Returns
         -------
             Output DataFrame
         """
         import pyspark.sql.functions as F
         from pyspark.sql.dataframe import DataFrame
+        from pyspark.sql.connect.dataframe import DataFrame as DataFrameConnect
         from pyspark.sql import Column
         from laktory.spark.dataframe import has_column
         from laktory.spark import functions as LF
         from laktory.spark import DataFrame as LDF
 
         if udfs is None:
             udfs = []
@@ -229,27 +230,31 @@
             else:
                 raise ValueError(
                     "`spark_func_name` must be specified if `sql_expression` is not specified"
                 )
 
         # Get from UDFs
         f = udfs.get(func_name, None)
+
+        # Get from built-in spark functions
         if f is None:
-            # Get from built-in spark functions
             if self.is_column:
                 f = getattr(F, func_name, None)
             else:
-                f = getattr(DataFrame, func_name, None)
-
-            if f is None:
-                # Get from laktory functions
-                if self.is_column:
-                    f = getattr(LF, func_name, None)
+                if isinstance(df, DataFrameConnect):
+                    f = getattr(DataFrameConnect, func_name, None)
                 else:
-                    f = getattr(LDF, func_name, None)
+                    f = getattr(DataFrame, func_name, None)
+
+        # Get from laktory functions
+        if f is None:
+            if self.is_column:
+                f = getattr(LF, func_name, None)
+            else:
+                f = getattr(LDF, func_name, None)
 
         if f is None:
             raise ValueError(f"Function {func_name} is not available")
 
         _args = self.spark_func_args
         _kwargs = self.spark_func_kwargs
```

### Comparing `laktory-0.2.0/laktory/models/spark/sparkfuncarg.py` & `laktory-0.2.1/laktory/models/spark/sparkfuncarg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-import re
-from pydantic import model_validator
+from pydantic import field_validator
 from typing import Any
-from typing import Literal
 from typing import Union
 
-from laktory._logger import get_logger
 from laktory.models.basemodel import BaseModel
-from laktory.models.datasources.basedatasource import BaseDataSource
-from laktory.models.datasources.tabledatasource import TableDataSource
 
 
 # --------------------------------------------------------------------------- #
 # Main Class                                                                  #
 # --------------------------------------------------------------------------- #
 
 
@@ -21,21 +16,39 @@
 
     Attributes
     ----------
     value:
         Value of the argument
     """
 
-    value: Union[TableDataSource, Any]
+    value: Union[Any]
 
-    # @property
-    # def is_column(self):
-    #     return self.convert_to == "COLUMN"
+    @field_validator("value")
+    def value_to_data_source(cls, v: Any) -> Any:
+        """
+        Data source can't be set as an expected value type as it would create
+        a circular dependency. Instead, we check at validation if the value
+        could be instantiated as a DataSource object.
+        """
+        from laktory.models.datasources.eventdatasource import EventDataSource
+        from laktory.models.datasources.tabledatasource import TableDataSource
+
+        try:
+            v = TableDataSource(**v)
+        except:
+            try:
+                v = EventDataSource(**v)
+            except:
+                pass
+
+        return v
 
     def eval(self, spark=None):
+        from laktory.models.datasources.basedatasource import BaseDataSource
+
         # Imports required to evaluate expressions
         import pyspark.sql.functions as F
         from pyspark.sql.functions import lit
         from pyspark.sql.functions import col
         from pyspark.sql.functions import expr
 
         v = self.value
```

### Comparing `laktory-0.2.0/laktory/models/sql/catalog.py` & `laktory-0.2.1/laktory/models/sql/catalog.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/sql/column.py` & `laktory-0.2.1/laktory/models/sql/column.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/sql/schema.py` & `laktory-0.2.1/laktory/models/sql/schema.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/sql/table.py` & `laktory-0.2.1/laktory/models/sql/table.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/sql/tablebuilder.py` & `laktory-0.2.1/laktory/models/sql/tablebuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from pydantic import model_validator
 from typing import Any
 from typing import Literal
 from typing import Union
-from typing import Callable
 
 from laktory._logger import get_logger
 from laktory.models.basemodel import BaseModel
 from laktory.models.datasources.basedatasource import BaseDataSource
 from laktory.models.datasources import EventDataSource
 from laktory.models.datasources import TableDataSource
 from laktory.models.sql.column import Column
```

### Comparing `laktory-0.2.0/laktory/models/sql/tableexpectation.py` & `laktory-0.2.1/laktory/models/sql/tableexpectation.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/sql/volume.py` & `laktory-0.2.1/laktory/models/sql/volume.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/stacks/pulumistack.py` & `laktory-0.2.1/laktory/models/stacks/pulumistack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/stacks/stack.py` & `laktory-0.2.1/laktory/models/stacks/stack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/models/stacks/terraformstack.py` & `laktory-0.2.1/laktory/models/stacks/terraformstack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/resources/data/stock_prices.json` & `laktory-0.2.1/laktory/resources/data/stock_prices.json`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/resources/notebooks/dlt_brz_template.py` & `laktory-0.2.1/laktory/resources/notebooks/dlt_brz_template.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/resources/notebooks/dlt_gld_template.py` & `laktory-0.2.1/laktory/resources/notebooks/dlt_gld_template.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/resources/notebooks/dlt_slv_star_template.py` & `laktory-0.2.1/laktory/resources/notebooks/dlt_slv_star_template.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/resources/notebooks/dlt_slv_template.py` & `laktory-0.2.1/laktory/resources/notebooks/dlt_slv_template.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/spark/dataframe/__init__.py` & `laktory-0.2.1/laktory/spark/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/spark/dataframe/groupby_and_agg.py` & `laktory-0.2.1/laktory/spark/dataframe/groupby_and_agg.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/spark/dataframe/has_column.py` & `laktory-0.2.1/laktory/spark/dataframe/has_column.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/spark/dataframe/schema_flat.py` & `laktory-0.2.1/laktory/spark/dataframe/schema_flat.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/spark/dataframe/show_string.py` & `laktory-0.2.1/laktory/spark/dataframe/show_string.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/spark/dataframe/smart_join.py` & `laktory-0.2.1/laktory/spark/dataframe/smart_join.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/spark/dataframe/watermark.py` & `laktory-0.2.1/laktory/spark/dataframe/watermark.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/spark/dataframe/window_filter.py` & `laktory-0.2.1/laktory/spark/dataframe/window_filter.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/spark/functions/_common.py` & `laktory-0.2.1/laktory/spark/functions/_common.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/spark/functions/logical.py` & `laktory-0.2.1/laktory/spark/functions/logical.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/spark/functions/math.py` & `laktory-0.2.1/laktory/spark/functions/math.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/spark/functions/string.py` & `laktory-0.2.1/laktory/spark/functions/string.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/spark/functions/units.py` & `laktory-0.2.1/laktory/spark/functions/units.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory/version.py` & `laktory-0.2.1/laktory/version.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/laktory.egg-info/PKG-INFO` & `laktory-0.2.1/laktory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laktory
-Version: 0.2.0
+Version: 0.2.1
 Summary: A DataOps framework for building a lakehouse
 Author-email: Olivier Soucy <olivier.soucy@okube.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/opencubes-ai/laktory
 Project-URL: Bug Tracker, https://github.com/opencubes-ai/laktory/issues
 Keywords: one,two
 Classifier: Development Status :: 4 - Beta
```

### Comparing `laktory-0.2.0/laktory.egg-info/SOURCES.txt` & `laktory-0.2.1/laktory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/mkdocs.yml` & `laktory-0.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/pyproject.toml` & `laktory-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/scripts/databricks_api_call.py` & `laktory-0.2.1/scripts/databricks_api_call.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/build_test_data.py` & `laktory-0.2.1/tests/build_test_data.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/data/brz_stock_prices/part-00000-aff20661-c55f-4489-86fc-8336e06ee376-c000.snappy.parquet` & `laktory-0.2.1/tests/data/brz_stock_prices/part-00000-aff20661-c55f-4489-86fc-8336e06ee376-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/data/slv_stock_meta/part-00000-d86fbfe6-5d98-43f6-827b-c18d9f79622f-c000.snappy.parquet` & `laktory-0.2.1/tests/data/slv_stock_meta/part-00000-d86fbfe6-5d98-43f6-827b-c18d9f79622f-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/data/slv_stock_prices/part-00000-d12f5de4-d8dd-46fc-b00a-c3c7dc6edc32-c000.snappy.parquet` & `laktory-0.2.1/tests/data/slv_stock_prices/part-00000-d12f5de4-d8dd-46fc-b00a-c3c7dc6edc32-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/data/stack.yaml` & `laktory-0.2.1/tests/data/stack.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_basemodel.py` & `laktory-0.2.1/tests/test_basemodel.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,20 @@
                 "timestamp": 3.0,
                 "ohlc": {"open": None, "high": None, "low": 3.0, "close": 4.0},
             },
         ],
     }
 
 
+def test_dump_yaml():
+    assert schema.model_dump_yaml(exclude_none=True).startswith(
+        "catalog_name: ${vars.env}"
+    )
+
+
 def test_camelize():
     settings.camel_serialization = True
     dump = schema.model_dump()
     print(dump)
     assert dump == {
         "comment": None,
         "grants": None,
@@ -299,10 +305,11 @@
     assert isinstance(d1["name"], pulumi.Output)
     assert isinstance(d1["catalog_name"], pulumi.Output)
     assert d1["tables"][0]["columns"][1]["name"] == "${ close.id }"
 
 
 if __name__ == "__main__":
     test_read_yaml()
+    test_dump_yaml()
     test_camelize()
     test_singular()
     test_inject_vars()
```

### Comparing `laktory-0.2.0/tests/test_baseresource.py` & `laktory-0.2.1/tests/test_baseresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_catalog.py` & `laktory-0.2.1/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_cli.py` & `laktory-0.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_column.py` & `laktory-0.2.1/tests/test_column.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_dataevent.py` & `laktory-0.2.1/tests/test_dataevent.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_datasources.py` & `laktory-0.2.1/tests/test_datasources.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,25 +55,36 @@
 def test_table_data_source(df0=df0):
     source = TableDataSource(
         mock_df=df0,
         path="/Volumes/tables/stock_prices/",
         filter="b != 0",
         selects=["a", "b", "c"],
         renames={"a": "aa", "b": "bb", "c": "cc"},
+        broadcast=True,
+        spark_chain={
+            "nodes": [
+                {
+                    "column": {"name": "chain"},
+                    "spark_func_name": "lit",
+                    "spark_func_args": ["chain"],
+                }
+            ]
+        },
     )
 
     # Test paths
     assert source.path == "/Volumes/tables/stock_prices/"
     assert source.from_path
     assert source.path_or_full_name == "/Volumes/tables/stock_prices/"
 
     # Test reader
     df = source.read(spark)
-    assert df.columns == ["aa", "bb", "cc"]
+    assert df.columns == ["aa", "bb", "cc", "chain"]
     assert df.count() == 2
+    assert df.toPandas()["chain"].tolist() == ["chain", "chain"]
 
     # Select with rename
     source = TableDataSource(
         mock_df=df0,
         path="/Volumes/tables/stock_prices/",
         selects={"x": "x1", "n": "n1"},
     )
```

### Comparing `laktory-0.2.0/tests/test_datetime.py` & `laktory-0.2.1/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_dbfsfile.py` & `laktory-0.2.1/tests/test_dbfsfile.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_dispatcher.py` & `laktory-0.2.1/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_docstrings.py` & `laktory-0.2.1/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_job.py` & `laktory-0.2.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_metastore.py` & `laktory-0.2.1/tests/test_metastore.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_notebook.py` & `laktory-0.2.1/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_parsers.py` & `laktory-0.2.1/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_pipeline.py` & `laktory-0.2.1/tests/test_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,19 @@
                     "drop_source_columns": True,
                     "event_source": None,
                     "layer": "SILVER",
                     "pipeline_name": "pl-stock-prices",
                     "table_source": {
                         "drops": None,
                         "filter": None,
+                        "broadcast": False,
                         "read_as_stream": True,
                         "renames": None,
                         "selects": None,
+                        "spark_chain": None,
                         "watermark": None,
                         "catalog_name": "dev",
                         "cdc": None,
                         "fmt": "DELTA",
                         "from_pipeline": True,
                         "name": "brz_stock_prices",
                         "path": None,
@@ -148,17 +150,19 @@
                     "drop_source_columns": False,
                     "event_source": None,
                     "layer": "SILVER",
                     "pipeline_name": "pl-stock-prices",
                     "table_source": {
                         "drops": None,
                         "filter": "created_at = '2023-09-01T00:00:00Z'",
+                        "broadcast": False,
                         "read_as_stream": True,
                         "renames": None,
                         "selects": None,
+                        "spark_chain": None,
                         "watermark": None,
                         "catalog_name": "dev",
                         "cdc": None,
                         "fmt": "DELTA",
                         "from_pipeline": True,
                         "name": "slv_stock_prices",
                         "path": None,
@@ -172,17 +176,19 @@
                                 "column": None,
                                 "spark_func_args": [],
                                 "spark_func_kwargs": {
                                     "other": {
                                         "value": {
                                             "drops": None,
                                             "filter": None,
+                                            "broadcast": False,
                                             "read_as_stream": True,
                                             "renames": {"symbol2": "symbol"},
                                             "selects": None,
+                                            "spark_chain": None,
                                             "watermark": None,
                                             "catalog_name": "dev",
                                             "cdc": None,
                                             "fmt": "DELTA",
                                             "from_pipeline": True,
                                             "name": "slv_stockmeta",
                                             "path": None,
@@ -219,17 +225,19 @@
                                 "column": None,
                                 "spark_func_args": [],
                                 "spark_func_kwargs": {
                                     "other": {
                                         "value": {
                                             "drops": None,
                                             "filter": None,
+                                            "broadcast": False,
                                             "read_as_stream": True,
                                             "renames": None,
                                             "selects": None,
+                                            "spark_chain": None,
                                             "watermark": None,
                                             "catalog_name": "dev",
                                             "cdc": None,
                                             "fmt": "DELTA",
                                             "from_pipeline": True,
                                             "name": "slv_stock_names",
                                             "path": None,
```

### Comparing `laktory-0.2.0/tests/test_schema.py` & `laktory-0.2.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_settings.py` & `laktory-0.2.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_spark_chain.py` & `laktory-0.2.1/tests/test_spark_chain.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_spark_dataframe.py` & `laktory-0.2.1/tests/test_spark_dataframe.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_spark_functions.py` & `laktory-0.2.1/tests/test_spark_functions.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_sql_query.py` & `laktory-0.2.1/tests/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_stack.py` & `laktory-0.2.1/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_table.py` & `laktory-0.2.1/tests/test_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,19 @@
             "drop_source_columns": True,
             "event_source": None,
             "layer": "SILVER",
             "pipeline_name": None,
             "table_source": {
                 "drops": None,
                 "filter": None,
+                "broadcast": False,
                 "read_as_stream": True,
                 "renames": None,
                 "selects": None,
+                "spark_chain": None,
                 "watermark": None,
                 "catalog_name": "dev",
                 "cdc": None,
                 "fmt": "DELTA",
                 "from_pipeline": True,
                 "name": "brz_stock_prices",
                 "path": None,
@@ -154,17 +156,19 @@
             "drop_source_columns": False,
             "event_source": None,
             "layer": "SILVER",
             "pipeline_name": None,
             "table_source": {
                 "drops": None,
                 "filter": "created_at = '2023-09-01T00:00:00Z'",
+                "broadcast": False,
                 "read_as_stream": True,
                 "renames": None,
                 "selects": None,
+                "spark_chain": None,
                 "watermark": None,
                 "catalog_name": "dev",
                 "cdc": None,
                 "fmt": "DELTA",
                 "from_pipeline": True,
                 "name": "slv_stock_prices",
                 "path": None,
@@ -178,17 +182,19 @@
                         "column": None,
                         "spark_func_args": [],
                         "spark_func_kwargs": {
                             "other": {
                                 "value": {
                                     "drops": None,
                                     "filter": None,
+                                    "broadcast": False,
                                     "read_as_stream": True,
                                     "renames": {"symbol2": "symbol"},
                                     "selects": None,
+                                    "spark_chain": None,
                                     "watermark": None,
                                     "catalog_name": "dev",
                                     "cdc": None,
                                     "fmt": "DELTA",
                                     "from_pipeline": True,
                                     "name": "slv_stockmeta",
                                     "path": None,
@@ -221,17 +227,19 @@
                         "column": None,
                         "spark_func_args": [],
                         "spark_func_kwargs": {
                             "other": {
                                 "value": {
                                     "drops": None,
                                     "filter": None,
+                                    "broadcast": False,
                                     "read_as_stream": True,
                                     "renames": None,
                                     "selects": None,
+                                    "spark_chain": None,
                                     "watermark": None,
                                     "catalog_name": "dev",
                                     "cdc": None,
                                     "fmt": "DELTA",
                                     "from_pipeline": True,
                                     "name": "slv_stock_names",
                                     "path": None,
```

### Comparing `laktory-0.2.0/tests/test_table_builder.py` & `laktory-0.2.1/tests/test_table_builder.py`

 * *Files identical despite different names*

### Comparing `laktory-0.2.0/tests/test_workspacefile.py` & `laktory-0.2.1/tests/test_workspacefile.py`

 * *Files identical despite different names*

