# Comparing `tmp/fused-1.5.4.tar.gz` & `tmp/fused-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fused-1.5.4.tar", max compression
+gzip compressed data, was "fused-1.6.1.tar", max compression
```

## Comparing `fused-1.5.4.tar` & `fused-1.6.1.tar`

### file list

```diff
@@ -1,114 +1,115 @@
--rw-r--r--   0        0        0     1144 2024-03-14 18:20:20.452694 fused-1.5.4/README.md
--rw-r--r--   0        0        0        6 2023-10-13 17:39:24.936083 fused-1.5.4/fused/MIGRATION_VERSION
--rw-r--r--   0        0        0     1111 2024-04-16 17:35:47.488366 fused-1.5.4/fused/__init__.py
--rw-r--r--   0        0        0       66 2023-08-29 21:43:53.192271 fused-1.5.4/fused/__main__.py
--rw-r--r--   0        0        0    10367 2024-03-01 23:09:39.488200 fused-1.5.4/fused/_auth.py
--rw-r--r--   0        0        0       66 2023-10-13 17:39:24.936596 fused-1.5.4/fused/_cache/__init__.py
--rw-r--r--   0        0        0     1401 2023-10-13 17:39:24.936653 fused-1.5.4/fused/_cache/memory.py
--rw-r--r--   0        0        0       77 2023-10-13 17:39:24.936726 fused-1.5.4/fused/_constants.py
--rw-r--r--   0        0        0     4181 2023-10-13 17:39:24.936791 fused-1.5.4/fused/_deserialize.py
--rw-r--r--   0        0        0      287 2023-10-13 17:39:24.937361 fused-1.5.4/fused/_deserialize_parquet.py
--rw-r--r--   0        0        0     2504 2023-10-13 17:39:24.937551 fused-1.5.4/fused/_environment.py
--rw-r--r--   0        0        0      357 2024-02-29 19:31:09.757442 fused-1.5.4/fused/_experimental.py
--rw-r--r--   0        0        0     2364 2024-02-29 19:31:09.757801 fused-1.5.4/fused/_formatter/common.py
--rw-r--r--   0        0        0    14878 2024-02-27 23:12:15.998414 fused-1.5.4/fused/_formatter/formatter_dataset.py
--rw-r--r--   0        0        0    11761 2024-01-03 19:21:18.331904 fused-1.5.4/fused/_formatter/formatter_eval_result.py
--rw-r--r--   0        0        0    16550 2023-10-13 20:24:00.322327 fused-1.5.4/fused/_formatter/formatter_job_config.py
--rw-r--r--   0        0        0     6962 2024-02-27 23:12:15.998885 fused-1.5.4/fused/_formatter/formatter_jobs.py
--rw-r--r--   0        0        0     2020 2023-10-13 17:39:24.939257 fused-1.5.4/fused/_formatter/formatter_options.py
--rw-r--r--   0        0        0     7031 2023-10-13 17:39:24.939757 fused-1.5.4/fused/_formatter/formatter_project.py
--rw-r--r--   0        0        0     1939 2024-02-29 19:31:09.758102 fused-1.5.4/fused/_formatter/formatter_templates.py
--rw-r--r--   0        0        0     5370 2024-02-16 20:07:37.387760 fused-1.5.4/fused/_formatter/formatter_udf_access_token.py
--rw-r--r--   0        0        0     1013 2023-10-13 17:39:24.940039 fused-1.5.4/fused/_formatter/noraise.py
--rw-r--r--   0        0        0     5379 2024-02-29 19:31:09.758573 fused-1.5.4/fused/_formatter/template.py
--rw-r--r--   0        0        0    11611 2024-02-07 21:35:13.328473 fused-1.5.4/fused/_formatter/udf.py
--rw-r--r--   0        0        0      905 2023-10-13 17:39:24.940709 fused-1.5.4/fused/_global_api.py
--rw-r--r--   0        0        0     2752 2024-04-01 21:12:17.245535 fused-1.5.4/fused/_load_udf.py
--rw-r--r--   0        0        0      721 2023-10-13 17:39:24.940878 fused-1.5.4/fused/_magic/__init__.py
--rw-r--r--   0        0        0     2853 2024-02-27 23:12:15.999392 fused-1.5.4/fused/_magic/magics.py
--rw-r--r--   0        0        0      608 2023-10-13 17:39:24.941393 fused-1.5.4/fused/_magic/output.py
--rw-r--r--   0        0        0     7783 2024-04-01 21:12:17.246431 fused-1.5.4/fused/_options.py
--rw-r--r--   0        0        0    39426 2024-04-01 21:12:17.247134 fused-1.5.4/fused/_project.py
--rw-r--r--   0        0        0    32913 2024-04-01 21:12:17.247928 fused-1.5.4/fused/_public_api.py
--rw-r--r--   0        0        0       40 2024-02-29 19:31:09.759028 fused-1.5.4/fused/_quick/__init__.py
--rw-r--r--   0        0        0    16830 2024-03-04 22:08:50.310839 fused-1.5.4/fused/_quick/udf.py
--rw-r--r--   0        0        0      118 2024-02-29 19:31:09.759558 fused-1.5.4/fused/_raster/__init__.py
--rw-r--r--   0        0        0     1431 2024-02-29 19:31:09.759769 fused-1.5.4/fused/_raster/signer.py
--rw-r--r--   0        0        0     4213 2024-02-29 19:31:09.759965 fused-1.5.4/fused/_raster/stac.py
--rw-r--r--   0        0        0     1015 2023-10-13 17:39:24.943010 fused-1.5.4/fused/_registry.py
--rw-r--r--   0        0        0      995 2023-10-13 17:39:24.943187 fused-1.5.4/fused/_request.py
--rw-r--r--   0        0        0    13798 2024-04-01 21:12:17.248121 fused-1.5.4/fused/_run.py
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.759996 fused-1.5.4/fused/_static/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.760075 fused-1.5.4/fused/_static/css/__init__.py
--rw-r--r--   0        0        0     7272 2024-02-29 19:31:09.762187 fused-1.5.4/fused/_static/css/style.css
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762251 fused-1.5.4/fused/_static/html/__init__.py
--rw-r--r--   0        0        0     3891 2024-02-29 19:31:09.762366 fused-1.5.4/fused/_static/html/icons-svg-inline.html
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762441 fused-1.5.4/fused/_static/templates/__init__.py
--rw-r--r--   0        0        0     1495 2023-10-18 19:12:32.880479 fused-1.5.4/fused/_str_utils.py
--rw-r--r--   0        0        0      176 2024-02-29 19:31:09.762566 fused-1.5.4/fused/_templates/__init__.py
--rw-r--r--   0        0        0      396 2024-02-29 19:31:09.762690 fused-1.5.4/fused/_templates/loaders.py
--rw-r--r--   0        0        0    15844 2024-02-29 19:31:09.763050 fused-1.5.4/fused/_templates/templates.py
--rw-r--r--   0        0        0      126 2023-10-13 17:39:24.943664 fused-1.5.4/fused/_udf/__init__.py
--rw-r--r--   0        0        0     1522 2023-10-13 17:39:24.943754 fused-1.5.4/fused/_udf/coerce.py
--rw-r--r--   0        0        0      790 2023-10-13 17:39:24.943812 fused-1.5.4/fused/_udf/context.py
--rw-r--r--   0        0        0     9116 2024-03-04 19:13:44.145677 fused-1.5.4/fused/_udf/decorators.py
--rw-r--r--   0        0        0     9049 2024-03-04 17:12:17.771016 fused-1.5.4/fused/_udf/execute_v2.py
--rw-r--r--   0        0        0    14851 2024-02-08 00:33:54.700810 fused-1.5.4/fused/_udf/load.py
--rw-r--r--   0        0        0      225 2023-10-13 17:39:24.944631 fused-1.5.4/fused/_udf/noop_decorators.py
--rw-r--r--   0        0        0      659 2023-10-13 17:39:24.944746 fused-1.5.4/fused/_udf/state.py
--rw-r--r--   0        0        0     3202 2024-04-01 21:12:17.248259 fused-1.5.4/fused/_utils.py
--rw-r--r--   0        0        0      404 2024-02-27 23:12:16.001476 fused-1.5.4/fused/api/__init__.py
--rw-r--r--   0        0        0      975 2023-10-13 17:39:24.945994 fused-1.5.4/fused/api/_open_dataset.py
--rw-r--r--   0        0        0     3586 2023-10-13 17:39:24.946052 fused-1.5.4/fused/api/_public_api.py
--rw-r--r--   0        0        0    40857 2024-04-16 17:35:39.170109 fused-1.5.4/fused/api/api.py
--rw-r--r--   0        0        0     3363 2024-03-11 21:21:34.935322 fused-1.5.4/fused/api/credentials.py
--rw-r--r--   0        0        0    25931 2024-04-01 21:12:17.249314 fused-1.5.4/fused/api/docker_api.py
--rw-r--r--   0        0        0    16529 2024-04-01 21:12:17.249955 fused-1.5.4/fused/api/docker_http_api.py
--rw-r--r--   0        0        0      290 2024-02-27 23:12:16.002737 fused-1.5.4/fused/cli.py
--rw-r--r--   0        0        0      492 2024-03-04 16:53:04.882953 fused-1.5.4/fused/core/__init__.py
--rw-r--r--   0        0        0    10279 2024-04-01 21:12:17.250418 fused-1.5.4/fused/core/_cache.py
--rw-r--r--   0        0        0     6513 2024-04-01 21:12:17.250608 fused-1.5.4/fused/core/_download.py
--rw-r--r--   0        0        0      509 2024-03-01 23:09:39.489541 fused-1.5.4/fused/core/_impl/_context_impl.py
--rw-r--r--   0        0        0     2995 2024-02-27 23:12:16.003344 fused-1.5.4/fused/core/_impl/_download_impl.py
--rw-r--r--   0        0        0     1022 2024-03-02 00:21:59.447576 fused-1.5.4/fused/core/_impl/_realtime_ops_impl.py
--rw-r--r--   0        0        0      254 2024-03-04 16:53:04.883231 fused-1.5.4/fused/core/_impl/_reimports.py
--rw-r--r--   0        0        0     2427 2024-03-14 21:19:20.148282 fused-1.5.4/fused/core/_impl/_table_ops_impl.py
--rw-r--r--   0        0        0     1369 2024-03-04 16:53:04.883573 fused-1.5.4/fused/core/_impl/_udf_ops_impl.py
--rw-r--r--   0        0        0    23387 2024-03-01 23:09:39.489874 fused-1.5.4/fused/core/_realtime_ops.py
--rw-r--r--   0        0        0     1067 2024-04-01 21:12:17.251472 fused-1.5.4/fused/core/_table_ops.py
--rw-r--r--   0        0        0     1767 2024-03-04 16:53:04.883828 fused-1.5.4/fused/core/_udf_ops.py
--rw-r--r--   0        0        0      752 2024-04-16 17:35:39.170492 fused-1.5.4/fused/models/__init__.py
--rw-r--r--   0        0        0      298 2023-10-13 17:39:24.948177 fused-1.5.4/fused/models/_codegen/__init__.py
--rw-r--r--   0        0        0     4861 2024-03-04 02:10:26.519019 fused-1.5.4/fused/models/_codegen/job.py
--rw-r--r--   0        0        0     4280 2024-02-08 00:33:54.701166 fused-1.5.4/fused/models/_codegen/udf.py
--rw-r--r--   0        0        0      224 2023-10-13 17:39:24.948705 fused-1.5.4/fused/models/_inplace.py
--rw-r--r--   0        0        0      250 2023-10-13 17:39:24.948775 fused-1.5.4/fused/models/_project_aware.py
--rw-r--r--   0        0        0      506 2024-02-16 20:07:37.390698 fused-1.5.4/fused/models/api/__init__.py
--rw-r--r--   0        0        0      221 2023-10-13 17:39:24.949226 fused-1.5.4/fused/models/api/_folder.py
--rw-r--r--   0        0        0    30327 2024-04-16 17:35:39.170855 fused-1.5.4/fused/models/api/dataset.py
--rw-r--r--   0        0        0       89 2023-05-12 15:11:04.143892 fused-1.5.4/fused/models/api/enums.py
--rw-r--r--   0        0        0    70205 2024-04-16 17:35:39.171363 fused-1.5.4/fused/models/api/job.py
--rw-r--r--   0        0        0     3235 2024-02-16 20:07:37.391066 fused-1.5.4/fused/models/api/udf_access_token.py
--rw-r--r--   0        0        0     3135 2023-10-13 17:39:24.950268 fused-1.5.4/fused/models/base.py
--rw-r--r--   0        0        0     1616 2024-03-04 16:53:04.884210 fused-1.5.4/fused/models/coerce_dataset.py
--rw-r--r--   0        0        0     3223 2024-02-08 20:07:13.852325 fused-1.5.4/fused/models/input.py
--rw-r--r--   0        0        0      330 2023-10-13 17:39:24.950681 fused-1.5.4/fused/models/internal/__init__.py
--rw-r--r--   0        0        0     7757 2024-04-16 17:35:39.171815 fused-1.5.4/fused/models/internal/dataset.py
--rw-r--r--   0        0        0    12158 2023-11-01 00:31:41.970766 fused-1.5.4/fused/models/internal/job.py
--rw-r--r--   0        0        0     1434 2023-10-13 17:39:24.952019 fused-1.5.4/fused/models/migrations.py
--rw-r--r--   0        0        0     5221 2024-02-16 20:07:37.391813 fused-1.5.4/fused/models/request.py
--rw-r--r--   0        0        0    29988 2024-03-25 21:04:06.819025 fused-1.5.4/fused/models/schema.py
--rw-r--r--   0        0        0      241 2023-10-13 17:39:24.953204 fused-1.5.4/fused/models/udf/__init__.py
--rw-r--r--   0        0        0     1432 2024-01-03 19:21:18.332999 fused-1.5.4/fused/models/udf/_eval_result.py
--rw-r--r--   0        0        0     8835 2024-03-04 16:53:21.723025 fused-1.5.4/fused/models/udf/_specialized_udfs.py
--rw-r--r--   0        0        0      781 2023-10-13 17:39:24.953888 fused-1.5.4/fused/models/udf/_udf_registry.py
--rw-r--r--   0        0        0    13495 2024-04-01 21:12:35.530426 fused-1.5.4/fused/models/udf/base_udf.py
--rw-r--r--   0        0        0     5358 2023-10-27 22:44:48.239852 fused-1.5.4/fused/models/udf/common.py
--rw-r--r--   0        0        0     5927 2024-04-09 19:05:13.177073 fused-1.5.4/fused/models/udf/header.py
--rw-r--r--   0        0        0     5564 2023-12-11 22:59:41.284263 fused-1.5.4/fused/models/udf/output.py
--rw-r--r--   0        0        0     3580 2024-03-04 17:12:17.771844 fused-1.5.4/fused/models/udf/udf.py
--rw-r--r--   0        0        0     1575 2023-10-13 17:39:24.955946 fused-1.5.4/fused/models/urls.py
--rw-r--r--   0        0        0      254 2024-03-11 20:54:28.030281 fused-1.5.4/fused/types.py
--rw-r--r--   0        0        0      675 2023-10-13 17:39:24.961379 fused-1.5.4/fused/warnings.py
--rw-r--r--   0        0        0     3111 2024-04-16 17:35:47.477699 fused-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 fused-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1144 2024-03-14 18:20:20.452694 fused-1.6.1/README.md
+-rw-r--r--   0        0        0        6 2023-10-13 17:39:24.936083 fused-1.6.1/fused/MIGRATION_VERSION
+-rw-r--r--   0        0        0     1111 2024-05-06 22:05:32.725322 fused-1.6.1/fused/__init__.py
+-rw-r--r--   0        0        0       66 2023-08-29 21:43:53.192271 fused-1.6.1/fused/__main__.py
+-rw-r--r--   0        0        0    10431 2024-05-02 18:32:09.965034 fused-1.6.1/fused/_auth.py
+-rw-r--r--   0        0        0       66 2023-10-13 17:39:24.936596 fused-1.6.1/fused/_cache/__init__.py
+-rw-r--r--   0        0        0     1401 2023-10-13 17:39:24.936653 fused-1.6.1/fused/_cache/memory.py
+-rw-r--r--   0        0        0       77 2023-10-13 17:39:24.936726 fused-1.6.1/fused/_constants.py
+-rw-r--r--   0        0        0     4181 2023-10-13 17:39:24.936791 fused-1.6.1/fused/_deserialize.py
+-rw-r--r--   0        0        0      287 2023-10-13 17:39:24.937361 fused-1.6.1/fused/_deserialize_parquet.py
+-rw-r--r--   0        0        0     2504 2023-10-13 17:39:24.937551 fused-1.6.1/fused/_environment.py
+-rw-r--r--   0        0        0      357 2024-02-29 19:31:09.757442 fused-1.6.1/fused/_experimental.py
+-rw-r--r--   0        0        0     2364 2024-02-29 19:31:09.757801 fused-1.6.1/fused/_formatter/common.py
+-rw-r--r--   0        0        0    14878 2024-02-27 23:12:15.998414 fused-1.6.1/fused/_formatter/formatter_dataset.py
+-rw-r--r--   0        0        0    11761 2024-01-03 19:21:18.331904 fused-1.6.1/fused/_formatter/formatter_eval_result.py
+-rw-r--r--   0        0        0    16550 2023-10-13 20:24:00.322327 fused-1.6.1/fused/_formatter/formatter_job_config.py
+-rw-r--r--   0        0        0     6962 2024-02-27 23:12:15.998885 fused-1.6.1/fused/_formatter/formatter_jobs.py
+-rw-r--r--   0        0        0     2020 2023-10-13 17:39:24.939257 fused-1.6.1/fused/_formatter/formatter_options.py
+-rw-r--r--   0        0        0     7031 2023-10-13 17:39:24.939757 fused-1.6.1/fused/_formatter/formatter_project.py
+-rw-r--r--   0        0        0     1939 2024-02-29 19:31:09.758102 fused-1.6.1/fused/_formatter/formatter_templates.py
+-rw-r--r--   0        0        0     5491 2024-05-02 18:32:09.965324 fused-1.6.1/fused/_formatter/formatter_udf_access_token.py
+-rw-r--r--   0        0        0     1013 2023-10-13 17:39:24.940039 fused-1.6.1/fused/_formatter/noraise.py
+-rw-r--r--   0        0        0     5379 2024-02-29 19:31:09.758573 fused-1.6.1/fused/_formatter/template.py
+-rw-r--r--   0        0        0    11611 2024-02-07 21:35:13.328473 fused-1.6.1/fused/_formatter/udf.py
+-rw-r--r--   0        0        0      905 2023-10-13 17:39:24.940709 fused-1.6.1/fused/_global_api.py
+-rw-r--r--   0        0        0     2752 2024-04-01 21:12:17.245535 fused-1.6.1/fused/_load_udf.py
+-rw-r--r--   0        0        0      721 2023-10-13 17:39:24.940878 fused-1.6.1/fused/_magic/__init__.py
+-rw-r--r--   0        0        0     2853 2024-02-27 23:12:15.999392 fused-1.6.1/fused/_magic/magics.py
+-rw-r--r--   0        0        0      608 2023-10-13 17:39:24.941393 fused-1.6.1/fused/_magic/output.py
+-rw-r--r--   0        0        0     7895 2024-05-02 18:32:09.965770 fused-1.6.1/fused/_options.py
+-rw-r--r--   0        0        0    39426 2024-04-01 21:12:17.247134 fused-1.6.1/fused/_project.py
+-rw-r--r--   0        0        0    33269 2024-05-06 21:22:59.479974 fused-1.6.1/fused/_public_api.py
+-rw-r--r--   0        0        0       40 2024-02-29 19:31:09.759028 fused-1.6.1/fused/_quick/__init__.py
+-rw-r--r--   0        0        0    15167 2024-05-02 18:12:03.590398 fused-1.6.1/fused/_quick/udf.py
+-rw-r--r--   0        0        0      118 2024-02-29 19:31:09.759558 fused-1.6.1/fused/_raster/__init__.py
+-rw-r--r--   0        0        0     1431 2024-02-29 19:31:09.759769 fused-1.6.1/fused/_raster/signer.py
+-rw-r--r--   0        0        0     4213 2024-02-29 19:31:09.759965 fused-1.6.1/fused/_raster/stac.py
+-rw-r--r--   0        0        0     1015 2023-10-13 17:39:24.943010 fused-1.6.1/fused/_registry.py
+-rw-r--r--   0        0        0      995 2023-10-13 17:39:24.943187 fused-1.6.1/fused/_request.py
+-rw-r--r--   0        0        0    14387 2024-05-03 18:18:28.457181 fused-1.6.1/fused/_run.py
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.759996 fused-1.6.1/fused/_static/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.760075 fused-1.6.1/fused/_static/css/__init__.py
+-rw-r--r--   0        0        0     7272 2024-02-29 19:31:09.762187 fused-1.6.1/fused/_static/css/style.css
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762251 fused-1.6.1/fused/_static/html/__init__.py
+-rw-r--r--   0        0        0     3891 2024-02-29 19:31:09.762366 fused-1.6.1/fused/_static/html/icons-svg-inline.html
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762441 fused-1.6.1/fused/_static/templates/__init__.py
+-rw-r--r--   0        0        0     1495 2023-10-18 19:12:32.880479 fused-1.6.1/fused/_str_utils.py
+-rw-r--r--   0        0        0      176 2024-02-29 19:31:09.762566 fused-1.6.1/fused/_templates/__init__.py
+-rw-r--r--   0        0        0      396 2024-02-29 19:31:09.762690 fused-1.6.1/fused/_templates/loaders.py
+-rw-r--r--   0        0        0    15844 2024-02-29 19:31:09.763050 fused-1.6.1/fused/_templates/templates.py
+-rw-r--r--   0        0        0      126 2023-10-13 17:39:24.943664 fused-1.6.1/fused/_udf/__init__.py
+-rw-r--r--   0        0        0     1522 2023-10-13 17:39:24.943754 fused-1.6.1/fused/_udf/coerce.py
+-rw-r--r--   0        0        0      790 2023-10-13 17:39:24.943812 fused-1.6.1/fused/_udf/context.py
+-rw-r--r--   0        0        0     9116 2024-03-04 19:13:44.145677 fused-1.6.1/fused/_udf/decorators.py
+-rw-r--r--   0        0        0     9049 2024-03-04 17:12:17.771016 fused-1.6.1/fused/_udf/execute_v2.py
+-rw-r--r--   0        0        0    14851 2024-02-08 00:33:54.700810 fused-1.6.1/fused/_udf/load.py
+-rw-r--r--   0        0        0      225 2023-10-13 17:39:24.944631 fused-1.6.1/fused/_udf/noop_decorators.py
+-rw-r--r--   0        0        0      659 2023-10-13 17:39:24.944746 fused-1.6.1/fused/_udf/state.py
+-rw-r--r--   0        0        0     3202 2024-04-01 21:12:17.248259 fused-1.6.1/fused/_utils.py
+-rw-r--r--   0        0        0      404 2024-02-27 23:12:16.001476 fused-1.6.1/fused/api/__init__.py
+-rw-r--r--   0        0        0      975 2023-10-13 17:39:24.945994 fused-1.6.1/fused/api/_open_dataset.py
+-rw-r--r--   0        0        0     3586 2023-10-13 17:39:24.946052 fused-1.6.1/fused/api/_public_api.py
+-rw-r--r--   0        0        0    44821 2024-05-06 21:22:59.481103 fused-1.6.1/fused/api/api.py
+-rw-r--r--   0        0        0     3363 2024-03-11 21:21:34.935322 fused-1.6.1/fused/api/credentials.py
+-rw-r--r--   0        0        0    26401 2024-05-06 21:22:59.481913 fused-1.6.1/fused/api/docker_api.py
+-rw-r--r--   0        0        0    16999 2024-05-06 21:22:59.482959 fused-1.6.1/fused/api/docker_http_api.py
+-rw-r--r--   0        0        0      290 2024-02-27 23:12:16.002737 fused-1.6.1/fused/cli.py
+-rw-r--r--   0        0        0      492 2024-03-04 16:53:04.882953 fused-1.6.1/fused/core/__init__.py
+-rw-r--r--   0        0        0    10279 2024-04-01 21:12:17.250418 fused-1.6.1/fused/core/_cache.py
+-rw-r--r--   0        0        0     6513 2024-04-01 21:12:17.250608 fused-1.6.1/fused/core/_download.py
+-rw-r--r--   0        0        0      509 2024-03-01 23:09:39.489541 fused-1.6.1/fused/core/_impl/_context_impl.py
+-rw-r--r--   0        0        0     2995 2024-02-27 23:12:16.003344 fused-1.6.1/fused/core/_impl/_download_impl.py
+-rw-r--r--   0        0        0     1022 2024-03-02 00:21:59.447576 fused-1.6.1/fused/core/_impl/_realtime_ops_impl.py
+-rw-r--r--   0        0        0      270 2024-05-03 18:18:28.457553 fused-1.6.1/fused/core/_impl/_reimports.py
+-rw-r--r--   0        0        0     2427 2024-03-14 21:19:20.148282 fused-1.6.1/fused/core/_impl/_table_ops_impl.py
+-rw-r--r--   0        0        0     1369 2024-03-04 16:53:04.883573 fused-1.6.1/fused/core/_impl/_udf_ops_impl.py
+-rw-r--r--   0        0        0    23387 2024-03-01 23:09:39.489874 fused-1.6.1/fused/core/_realtime_ops.py
+-rw-r--r--   0        0        0     1067 2024-04-01 21:12:17.251472 fused-1.6.1/fused/core/_table_ops.py
+-rw-r--r--   0        0        0     1767 2024-03-04 16:53:04.883828 fused-1.6.1/fused/core/_udf_ops.py
+-rw-r--r--   0        0        0      752 2024-04-16 17:35:39.170492 fused-1.6.1/fused/models/__init__.py
+-rw-r--r--   0        0        0      298 2023-10-13 17:39:24.948177 fused-1.6.1/fused/models/_codegen/__init__.py
+-rw-r--r--   0        0        0     4861 2024-03-04 02:10:26.519019 fused-1.6.1/fused/models/_codegen/job.py
+-rw-r--r--   0        0        0     4280 2024-02-08 00:33:54.701166 fused-1.6.1/fused/models/_codegen/udf.py
+-rw-r--r--   0        0        0      224 2023-10-13 17:39:24.948705 fused-1.6.1/fused/models/_inplace.py
+-rw-r--r--   0        0        0      250 2023-10-13 17:39:24.948775 fused-1.6.1/fused/models/_project_aware.py
+-rw-r--r--   0        0        0      537 2024-05-06 21:22:59.483270 fused-1.6.1/fused/models/api/__init__.py
+-rw-r--r--   0        0        0      221 2023-10-13 17:39:24.949226 fused-1.6.1/fused/models/api/_folder.py
+-rw-r--r--   0        0        0      280 2024-05-06 21:22:59.483513 fused-1.6.1/fused/models/api/_list.py
+-rw-r--r--   0        0        0    30327 2024-04-18 16:14:06.864717 fused-1.6.1/fused/models/api/dataset.py
+-rw-r--r--   0        0        0       89 2023-05-12 15:11:04.143892 fused-1.6.1/fused/models/api/enums.py
+-rw-r--r--   0        0        0    71616 2024-05-06 22:04:00.830391 fused-1.6.1/fused/models/api/job.py
+-rw-r--r--   0        0        0     3319 2024-05-02 18:32:09.966327 fused-1.6.1/fused/models/api/udf_access_token.py
+-rw-r--r--   0        0        0     3135 2024-04-18 16:14:06.869177 fused-1.6.1/fused/models/base.py
+-rw-r--r--   0        0        0     1616 2024-03-04 16:53:04.884210 fused-1.6.1/fused/models/coerce_dataset.py
+-rw-r--r--   0        0        0     3223 2024-04-18 16:14:06.869588 fused-1.6.1/fused/models/input.py
+-rw-r--r--   0        0        0      330 2023-10-13 17:39:24.950681 fused-1.6.1/fused/models/internal/__init__.py
+-rw-r--r--   0        0        0     7757 2024-04-18 16:14:06.871153 fused-1.6.1/fused/models/internal/dataset.py
+-rw-r--r--   0        0        0    12158 2024-04-18 16:14:06.873206 fused-1.6.1/fused/models/internal/job.py
+-rw-r--r--   0        0        0     1434 2023-10-13 17:39:24.952019 fused-1.6.1/fused/models/migrations.py
+-rw-r--r--   0        0        0     5288 2024-05-02 18:32:09.966536 fused-1.6.1/fused/models/request.py
+-rw-r--r--   0        0        0    29988 2024-04-18 16:14:06.876143 fused-1.6.1/fused/models/schema.py
+-rw-r--r--   0        0        0      241 2023-10-13 17:39:24.953204 fused-1.6.1/fused/models/udf/__init__.py
+-rw-r--r--   0        0        0     1432 2024-04-18 16:14:06.876792 fused-1.6.1/fused/models/udf/_eval_result.py
+-rw-r--r--   0        0        0     8835 2024-03-04 16:53:21.723025 fused-1.6.1/fused/models/udf/_specialized_udfs.py
+-rw-r--r--   0        0        0      781 2023-10-13 17:39:24.953888 fused-1.6.1/fused/models/udf/_udf_registry.py
+-rw-r--r--   0        0        0    13545 2024-05-02 18:32:09.966787 fused-1.6.1/fused/models/udf/base_udf.py
+-rw-r--r--   0        0        0     5358 2024-04-18 16:14:06.880981 fused-1.6.1/fused/models/udf/common.py
+-rw-r--r--   0        0        0     5927 2024-04-18 16:14:06.882192 fused-1.6.1/fused/models/udf/header.py
+-rw-r--r--   0        0        0     5564 2024-04-18 16:14:06.882422 fused-1.6.1/fused/models/udf/output.py
+-rw-r--r--   0        0        0     3580 2024-03-04 17:12:17.771844 fused-1.6.1/fused/models/udf/udf.py
+-rw-r--r--   0        0        0     1575 2023-10-13 17:39:24.955946 fused-1.6.1/fused/models/urls.py
+-rw-r--r--   0        0        0      254 2024-03-11 20:54:28.030281 fused-1.6.1/fused/types.py
+-rw-r--r--   0        0        0      675 2023-10-13 17:39:24.961379 fused-1.6.1/fused/warnings.py
+-rw-r--r--   0        0        0     3111 2024-05-06 22:05:32.719366 fused-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 fused-1.6.1/PKG-INFO
```

### Comparing `fused-1.5.4/README.md` & `fused-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/__init__.py` & `fused-1.6.1/fused/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 from .core import cache, download, get_chunk_from_table, get_chunks_metadata
 
 # Must be later so that models get imported first
 from . import _experimental as experimental  # isort:skip
 
 # Version is set to 0.0.0 as the version string is automatically generated by
 # https://github.com/mtkennerly/poetry-dynamic-versioning
-__version__ = "1.5.4"
+__version__ = "1.6.1"
```

### Comparing `fused-1.5.4/fused/_auth.py` & `fused-1.6.1/fused/_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,21 +119,22 @@
 
     _credentials: Optional[Credentials] = None
 
     def __init__(self) -> None:
         try:
             self._credentials = Credentials.from_disk()
         except ValueError:
-            auth_msg = """\
-                Credentials not found on disk. Authenticate with:
+            if OPTIONS.prompt_to_login:
+                auth_msg = """\
+                    Credentials not found on disk. Authenticate with:
 
-                from fused import NotebookCredentials
-                credentials = NotebookCredentials()
-            """
-            print(dedent(auth_msg))
+                    from fused import NotebookCredentials
+                    credentials = NotebookCredentials()
+                """
+                print(dedent(auth_msg))
 
     def initialize(self) -> None:
         """Force initialization of credentials."""
         _ = self.credentials
 
     @property
     def credentials(self) -> Credentials:
```

### Comparing `fused-1.5.4/fused/_cache/memory.py` & `fused-1.6.1/fused/_cache/memory.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_deserialize.py` & `fused-1.6.1/fused/_deserialize.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_environment.py` & `fused-1.6.1/fused/_environment.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_formatter/common.py` & `fused-1.6.1/fused/_formatter/common.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_formatter/formatter_dataset.py` & `fused-1.6.1/fused/_formatter/formatter_dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_formatter/formatter_eval_result.py` & `fused-1.6.1/fused/_formatter/formatter_eval_result.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_formatter/formatter_job_config.py` & `fused-1.6.1/fused/_formatter/formatter_job_config.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_formatter/formatter_jobs.py` & `fused-1.6.1/fused/_formatter/formatter_jobs.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_formatter/formatter_options.py` & `fused-1.6.1/fused/_formatter/formatter_options.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_formatter/formatter_project.py` & `fused-1.6.1/fused/_formatter/formatter_project.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_formatter/formatter_templates.py` & `fused-1.6.1/fused/_formatter/formatter_templates.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_formatter/formatter_udf_access_token.py` & `fused-1.6.1/fused/_formatter/formatter_udf_access_token.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,16 +63,17 @@
             configuration.append(f"<li>{key}: <code>{escape(repr(value))}</code></li>")
 
     # TODO: Fix for no schema, fix for parameters expected by the UDF, fix for copy decorator, fix for entrypoint
     attrs_ul = f"""
     <h4 style="margin-left: 20px;">Token</h4>
     <ul style="margin-top: 0; margin-bottom: 0px;">
     <li>{copyable_text(token.token, show_text=True)}</li>
-    <li>UDF owner email: <code>{escape(token.udf_email)}</code></li>
-    <li>UDF ID: <code>{escape(token.udf_slug)}</code></li>
+    <li>UDF owner email: <code>{escape(token.udf_email) if token.udf_email else 'None'}</code></li>
+    <li>UDF name: <code>{escape(token.udf_slug)}</code></li>
+    <li>UDF ID: <code>{escape(token.udf_id) if token.udf_id else 'Unknown'}</code></li>
     </ul>
     <h4 style="margin-left: 20px;">Configuration</h4>
     <ul style="margin-top: 0; margin-bottom: 0px;">
     {''.join(configuration)}
     </ul>
     <h4 style="margin-left: 20px;">Toolkit</h4>
     <ul style="margin-top: 0; margin-bottom: 0px;">
```

### Comparing `fused-1.5.4/fused/_formatter/noraise.py` & `fused-1.6.1/fused/_formatter/noraise.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_formatter/template.py` & `fused-1.6.1/fused/_formatter/template.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_formatter/udf.py` & `fused-1.6.1/fused/_formatter/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_global_api.py` & `fused-1.6.1/fused/_global_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_load_udf.py` & `fused-1.6.1/fused/_load_udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_magic/__init__.py` & `fused-1.6.1/fused/_magic/__init__.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_magic/magics.py` & `fused-1.6.1/fused/_magic/magics.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_magic/output.py` & `fused-1.6.1/fused/_magic/output.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_options.py` & `fused-1.6.1/fused/_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,17 @@
     default_udf_run_engine: Optional[StrictStr] = None
     """Default engine to run UDFs, one of: `local`, `realtime`, `batch`."""
 
     default_validate_imports: StrictBool = False
     """Default for whether to validate imports in UDFs before `run_local`,
     `run_batch`."""
 
+    prompt_to_login: StrictBool = False
+    """Automatically prompt the user to login when importing Fused."""
+
     @validator("base_url")
     def _validate_base_url(cls, v):
         reset_api()
         return v
 
     def save(self):
         """Save Fused options to `~/.fused/settings.toml`. They will be automatically
```

### Comparing `fused-1.5.4/fused/_project.py` & `fused-1.6.1/fused/_project.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_public_api.py` & `fused-1.6.1/fused/_public_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Iterable,
     List,
     Literal,
     Optional,
     Sequence,
     Tuple,
     Union,
+    overload,
 )
 
 import contextily as cx
 import geopandas as gpd
 from xyzservices.lib import TileProvider
 
 import fused
@@ -31,14 +32,15 @@
 from fused.models._codegen import CustomJobConfig
 from fused.models.api import (
     Dataset,
     GeospatialPartitionJobStepConfig,
     JobConfig,
     JobStepConfig,
     JoinJobStepConfig,
+    ListDetails,
     MapJobStepConfig,
     NonGeospatialPartitionJobStepConfig,
     Table,
 )
 from fused.models.api.job import GDALOpenConfig, JoinType
 from fused.models.internal import (
     DatasetInput,
@@ -589,30 +591,43 @@
         fused.delete("fd://bucket-name/deprecated_table/")
         ```
     """
     api = get_api()
     return api.delete(path, max_deletion_depth=max_deletion_depth)
 
 
-def list(path: str) -> List[str]:
+@overload
+def list(path: str, *, details: Literal[False] = False) -> List[str]:
+    ...
+
+
+@overload
+def list(path: str, *, details: Literal[True]) -> List[ListDetails]:
+    ...
+
+
+def list(path: str, *, details: bool = False):
     """List the files at the path.
 
     Args:
         path: Parent directory URL, like `fd://bucket-name/`
 
+    Keyword Args:
+        details: If True, return additional metadata about each record.
+
     Returns:
-        A list of paths as URLs
+        A list of paths as URLs, or as metadata objects.
 
     Examples:
         ```python
         fused.list("fd://bucket-name/")
         ```
     """
     api = get_api()
-    return api.list(path)
+    return api.list(path, details=details)
 
 
 def get(path: str) -> bytes:
     """Download the contents at the path to memory.
 
     Args:
         path: URL to a file, like `fd://bucket-name/file.parquet`
```

### Comparing `fused-1.5.4/fused/_quick/udf.py` & `fused-1.6.1/fused/_quick/udf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# TODO: This file is no longer the most recent -- use fused.utils.run_* instead
+# TODO: This file is no longer the most recent -- use fused.core.run_* instead
+# This file is only for running non-saved (code included) UDFs
 
 import base64
 import json
 import time
 import warnings
 from io import BytesIO
 from pathlib import Path
@@ -47,120 +48,98 @@
 
 def run_tile(
     x: float,
     y: float,
     z: float,
     data: Optional[Union[pd.DataFrame, gpd.GeoDataFrame, pa.Table, str, Path, Any]],
     step_config: Optional[JobStepConfig] = None,
-    udf_email: Optional[str] = None,
-    udf_id: Optional[str] = None,
+    params: Optional[Dict[str, str]] = None,
+    *,
     print_time: bool = False,
     client_id: Optional[str] = None,
     dtype_out_vector: str = "parquet",
     dtype_out_raster: str = "tiff",
 ) -> UdfEvaluationResult:  # TODO: return png
     time_start = time.perf_counter()
     # We need to get the auth headers from the FusedAPI. Don't enable set_global_api
     # to avoid messing up the user's environment.
     api = FusedAPI(set_global_api=False)
 
     udf_server_url = _resolve_udf_server_url(client_id)
 
-    if step_config is not None:
-        assert (
-            udf_email is None and udf_id is None
-        ), "udf_email and udf_id must not be set if step_config is passed"
-        url = f"{udf_server_url}/api/v1/run/udf/tiles/{z}/{x}/{y}"
-
-        # Headers
-        headers = api._generate_headers({"Content-Type": "application/json"})
-
-        # Payload
-        post_attr_json = {
-            "data_left": data,
-            "data_right": None,
-            "step_config": step_config.json(),
-            "dtype_in": "json",
-            "dtype_out_vector": dtype_out_vector,
-            "dtype_out_raster": dtype_out_raster,
-        }
-
-        # Params
-        req_params = {}
-
-        # Make request
-        start = time.time()
-
-        r = requests.post(
-            url=url,
-            params=req_params,
-            json=post_attr_json,
-            headers=headers,
-            timeout=OPTIONS.request_timeout,
-        )
-    else:
-        assert (
-            udf_email is not None and udf_id is not None
-        ), "udf_email and udf_id must be provided if step_config is not passed"
-        url = f"{udf_server_url}/api/v1/run/udf/saved/{udf_email}/{udf_id}/tiles/{z}/{x}/{y}"
-
-        # Headers
-        headers = api._generate_headers()
-
-        # TODO: Params
-        req_params = {
-            "dtype_out_vector": dtype_out_vector,
-            "dtype_out_raster": dtype_out_raster,
-            **data,
-        }
-
-        # Make request
-        start = time.time()
-
-        r = requests.get(
-            url=url,
-            params=req_params,
-            headers=headers,
-            timeout=OPTIONS.request_timeout,
-        )
+    assert step_config is not None
+    # Apply parameters, if we want to step_config that's returned to have this,
+    # overwrite step_config.
+    step_config_with_params = step_config.set_udf(
+        udf=step_config.udf, parameters=params
+    )
+
+    url = f"{udf_server_url}/api/v1/run/udf/tiles/{z}/{x}/{y}"
+
+    # Headers
+    headers = api._generate_headers({"Content-Type": "application/json"})
+
+    # Payload
+    post_attr_json = {
+        "data_left": data,
+        "data_right": None,
+        "step_config": step_config_with_params.json(),
+        "dtype_in": "json",
+        "dtype_out_vector": dtype_out_vector,
+        "dtype_out_raster": dtype_out_raster,
+    }
+
+    # Params
+    req_params = {}
+
+    # Make request
+    start = time.time()
+
+    r = requests.post(
+        url=url,
+        params=req_params,
+        json=post_attr_json,
+        headers=headers,
+        timeout=OPTIONS.request_timeout,
+    )
 
     end = time.time()
     if print_time:
         logger.info(f"Time in request: {end - start}")
 
     time_end = time.perf_counter()
     time_taken_seconds = time_end - time_start
 
-    return _process_response(r, step_config, time_taken_seconds)
+    return _process_response(
+        r, step_config=step_config_with_params, time_taken_seconds=time_taken_seconds
+    )
 
 
 def run(
-    df_left: Optional[Union[pd.DataFrame, gpd.GeoDataFrame, pa.Table, str, Path, Any]],
+    df_left: Optional[
+        Union[pd.DataFrame, gpd.GeoDataFrame, pa.Table, str, Path, Any]
+    ] = None,
     df_right: Optional[
         Union[pd.DataFrame, gpd.GeoDataFrame, pa.Table, str, Path]
     ] = None,
     step_config: Optional[JobStepConfig] = None,
-    udf_email: Optional[str] = None,
-    udf_id: Optional[str] = None,
     params: Optional[Dict[str, str]] = None,
     *,
     print_time: bool = False,
     read_options: Optional[Dict] = None,
     client_id: Optional[str] = None,
     dtype_out_vector: str = "parquet",
     dtype_out_raster: str = "tiff",
 ) -> pd.DataFrame:
     """Run a UDF over a DataFrame.
 
     Args:
         df_left: Input DataFrame, or path to a local Parquet file.
         df_right: Input DataFrame, or path to a local Parquet file.
-        step_config: JobStepConfig, if not running a saved UDF.
-        udf_email: Saved UDF's owner.
-        udf_id: Saved UDF's ID.
+        step_config: JobStepConfig.
         params: Additional parameters to pass to the UDF. Must be JSON serializable.
 
     Keyword Args:
         print_time: If True, print the amount of time taken in the request.
         read_options: If not None, options for reading `df` that will be passed to GeoPandas.
     """
     # TODO: This function is too complicated
@@ -168,73 +147,55 @@
     time_start = time.perf_counter()
     # We need to get the auth headers from the FusedAPI. Don't enable set_global_api
     # to avoid messing up the user's environment.
     api = FusedAPI(set_global_api=False)
 
     udf_server_url = _resolve_udf_server_url(client_id)
 
-    step_config_with_params: Optional[JobStepConfig] = None
-    if step_config is not None:
-        assert (
-            udf_email is None and udf_id is None
-        ), "udf_email and udf_id must not be set if step_config is passed"
-        # Apply parameters, if we want to step_config that's returned to have this,
-        # overwrite step_config.
-        step_config_with_params = step_config.set_udf(
-            udf=step_config.udf, parameters=params
-        )
-
-        # Note: Custom UDF uses the json POST attribute.
-        url = f"{udf_server_url}/api/v1/run/udf"
-
-        # This is the body for when step_config_with_params.type == "udf".
-        body = {
-            "data_left": df_left,
-            "step_config": step_config_with_params.json(),
-            "dtype_in": "json",
-            "dtype_out_vector": dtype_out_vector,
-            "dtype_out_raster": dtype_out_raster,
-        }
-
-        if step_config_with_params.type != "udf":
-            # Infer dtype_in from df_left. Ensure df_right, if present, is same type.
-            if df_left is not None:
-                data_left, dtype_in_left = _serialize_input(df_left, read_options)
-                body["data_left"] = data_left
-                body["dtype_in"] = dtype_in_left
-
-            if df_right is not None:
-                body["data_right"], dtype_in_right = _serialize_input(
-                    df_right, read_options
-                )
-                assert (
-                    dtype_in_left == dtype_in_right
-                ), "Left and right must be same type. Fused currently supports 'GeoDataFrame' and 'geojson'."
-
-        method = "POST"
-        post_attr_data = None
-        post_attr_json = body
-        post_attr_headers = api._generate_headers({"Content-Type": "application/json"})
-
-        req_params = {}
-    else:
-        assert (
-            udf_email is not None and udf_id is not None
-        ), "udf_email and udf_id must be set if step_config is not passed"
-        url = f"{udf_server_url}/api/v1/run/udf/saved/{udf_email}/{udf_id}"
-
-        # TODO: doesn't handle df_left
-        method = "GET"
-        assert df_left is None
-        post_attr_data = None
-        post_attr_json = None
-        post_attr_headers = api._generate_headers()
-        req_params = {} if params is None else params
-        req_params["dtype_out_vector"] = dtype_out_vector
-        req_params["dtype_out_raster"] = dtype_out_raster
+    assert step_config is not None
+    # Apply parameters, if we want to step_config that's returned to have this,
+    # overwrite step_config.
+    step_config_with_params = step_config.set_udf(
+        udf=step_config.udf, parameters=params
+    )
+
+    # Note: Custom UDF uses the json POST attribute.
+    url = f"{udf_server_url}/api/v1/run/udf"
+
+    # This is the body for when step_config_with_params.type == "udf".
+    body = {
+        "data_left": df_left,
+        "step_config": step_config_with_params.json(),
+        "dtype_in": "json",
+        "dtype_out_vector": dtype_out_vector,
+        "dtype_out_raster": dtype_out_raster,
+    }
+
+    # TODO: This is not really supported
+    if step_config_with_params.type != "udf":
+        # Infer dtype_in from df_left. Ensure df_right, if present, is same type.
+        if df_left is not None:
+            data_left, dtype_in_left = _serialize_input(df_left, read_options)
+            body["data_left"] = data_left
+            body["dtype_in"] = dtype_in_left
+
+        if df_right is not None:
+            body["data_right"], dtype_in_right = _serialize_input(
+                df_right, read_options
+            )
+            assert (
+                dtype_in_left == dtype_in_right
+            ), "Left and right must be same type. Fused currently supports 'GeoDataFrame' and 'geojson'."
+
+    method = "POST"
+    post_attr_data = None
+    post_attr_json = body
+    post_attr_headers = api._generate_headers({"Content-Type": "application/json"})
+
+    req_params = {}
 
     # Make request
     start = time.time()
 
     r = requests.request(
         method=method,
         url=url,
```

### Comparing `fused-1.5.4/fused/_raster/signer.py` & `fused-1.6.1/fused/_raster/signer.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_raster/stac.py` & `fused-1.6.1/fused/_raster/stac.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_registry.py` & `fused-1.6.1/fused/_registry.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_request.py` & `fused-1.6.1/fused/_request.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_run.py` & `fused-1.6.1/fused/_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,24 @@
     run_shared_file_async,
     run_shared_tile,
     run_shared_tile_async,
     run_tile,
     run_tile_async,
 )
 from .core._impl._realtime_ops_impl import default_run_engine
-from .core._impl._reimports import GeoPandasUdfV2, UdfJobStepConfig
+from .core._impl._reimports import GeoPandasUdfV2, UdfAccessToken, UdfJobStepConfig
 
 ResultType = Union[xr.Dataset, pd.DataFrame, gpd.GeoDataFrame]
 
 
 @overload
 def run(
-    email_or_udf_or_token: Union[str, None, UdfJobStepConfig, GeoPandasUdfV2],
+    email_or_udf_or_token: Union[
+        str, None, UdfJobStepConfig, GeoPandasUdfV2, UdfAccessToken
+    ],
     /,
     udf_name: Optional[str],
     *,
     udf: Optional[GeoPandasUdfV2],
     job_step: Optional[UdfJobStepConfig],
     token: Optional[str],
     udf_email: Optional[str],
@@ -70,15 +72,17 @@
     parameters: Optional[Dict[str, Any]] = None,
     **kw_parameters,
 ) -> ResultType:
     ...
 
 
 def run(
-    email_or_udf_or_token: Union[str, None, UdfJobStepConfig, GeoPandasUdfV2] = None,
+    email_or_udf_or_token: Union[
+        str, None, UdfJobStepConfig, GeoPandasUdfV2, UdfAccessToken
+    ] = None,
     /,
     udf_name: Optional[str] = None,
     *,
     udf: Optional[GeoPandasUdfV2] = None,
     job_step: Optional[UdfJobStepConfig] = None,
     token: Optional[str] = None,
     udf_email: Optional[str] = None,
@@ -170,14 +174,16 @@
                 "udf_email parameter is being ignored in favor of the first positional parameter.",
             )
 
         if isinstance(email_or_udf_or_token, UdfJobStepConfig):
             job_step = email_or_udf_or_token
         elif isinstance(email_or_udf_or_token, GeoPandasUdfV2):
             udf = email_or_udf_or_token
+        elif isinstance(email_or_udf_or_token, UdfAccessToken):
+            token = email_or_udf_or_token.token
         elif isinstance(email_or_udf_or_token, str):
             if "/" in email_or_udf_or_token:
                 udf_email, udf_name = email_or_udf_or_token.split("/", maxsplit=1)
             elif "@" in email_or_udf_or_token:
                 udf_email = email_or_udf_or_token
             else:
                 # TODO: no way to specify only UDF name
@@ -355,14 +361,21 @@
 
     dispatch_params = ("sync" if sync else "async", type, udf_storage, engine)
 
     # Ellipsis is the sentinal value for not found in the dictionary at all
     fn = dispatch.get(dispatch_params, ...)
 
     if fn is Ellipsis:
-        raise ValueError(
-            f"Could not determine how to call with settings: {dispatch_params}"
-        )
+        if udf_storage == "token" and engine != "realtime":
+            raise ValueError("UDF tokens can only be called on the realtime engine.")
+        elif udf_storage == "saved" and engine != "realtime":
+            raise ValueError(
+                "Saved UDFs can only be called on the realtime engine. To use another engine, load the UDF locally first."
+            )
+        else:
+            raise ValueError(
+                f"Could not determine how to call with settings: {dispatch_params}"
+            )
     if fn is None:
         raise ValueError(f"Call type is not yet implemented: {dispatch_params}")
 
     return fn()
```

### Comparing `fused-1.5.4/fused/_static/css/style.css` & `fused-1.6.1/fused/_static/css/style.css`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_static/html/icons-svg-inline.html` & `fused-1.6.1/fused/_static/html/icons-svg-inline.html`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_str_utils.py` & `fused-1.6.1/fused/_str_utils.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_templates/templates.py` & `fused-1.6.1/fused/_templates/templates.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_udf/coerce.py` & `fused-1.6.1/fused/_udf/coerce.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_udf/context.py` & `fused-1.6.1/fused/_udf/context.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_udf/decorators.py` & `fused-1.6.1/fused/_udf/decorators.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_udf/execute_v2.py` & `fused-1.6.1/fused/_udf/execute_v2.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_udf/load.py` & `fused-1.6.1/fused/_udf/load.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_udf/state.py` & `fused-1.6.1/fused/_udf/state.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/_utils.py` & `fused-1.6.1/fused/_utils.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/api/_open_dataset.py` & `fused-1.6.1/fused/api/_open_dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/api/_public_api.py` & `fused-1.6.1/fused/api/_public_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/api/api.py` & `fused-1.6.1/fused/api/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 from __future__ import annotations
 
 import shutil
 import time
+import uuid
 import warnings
 from functools import lru_cache
 from io import SEEK_SET
 from pathlib import Path
 from tempfile import TemporaryFile
-from typing import Any, BinaryIO, Dict, List, Literal, Optional, Sequence, Union
+from typing import (
+    Any,
+    BinaryIO,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Sequence,
+    Union,
+    overload,
+)
 
 import geopandas as gpd
 import pandas as pd
 import requests
 
 import fused
 import fused.models.request as request_models
@@ -29,25 +40,31 @@
 from fused.api._open_dataset import post_open_table
 from fused.models import JoinInput, JoinSingleFileInput, MapInput
 from fused.models.api import (
     JobConfig,
     JobStepConfig,
     JoinJobStepConfig,
     JoinSinglefileJobStepConfig,
+    ListDetails,
     MapJobStepConfig,
     Table,
     UdfAccessToken,
     UdfAccessTokenList,
 )
 from fused.models.api._folder import Folder
 from fused.models.internal import Jobs, RunResponse
 from fused.models.internal.job import CoerceableToJobId, _object_to_job_id
 from fused.models.request import WHITELISTED_INSTANCE_TYPES
 from fused.models.udf._udf_registry import UdfRegistry
-from fused.models.udf.base_udf import METADATA_FUSED_ID, METADATA_FUSED_SLUG, BaseUdf
+from fused.models.udf.base_udf import (
+    METADATA_FUSED_EXPLORER_TAB,
+    METADATA_FUSED_ID,
+    METADATA_FUSED_SLUG,
+    BaseUdf,
+)
 from fused.warnings import FusedNonProductionWarning
 
 
 class FusedAPI:
     """API for running jobs in the Fused service."""
 
     base_url: str
@@ -394,25 +411,33 @@
         self,
         n: int = 5,
         *,
         skip: int = 0,
         per_request: int = 25,
         max_requests: Optional[int] = 1,
         by: Literal["name", "id", "slug"] = "name",
-        whose: Literal["self", "public"] = "self",
+        whose: Literal["self", "public", "community", "team"] = "self",
     ):
         request_count = 0
         has_content = True
         udfs = []
 
         assert per_request >= 0
 
         while has_content:
-            # TODO: This is only for my UDFs, not for public, etc.
-            url = f"{self.base_url}/udf/{whose}"
+            if whose == "self":
+                url = f"{self.base_url}/udf/self"
+            elif whose == "public" or whose == "community":
+                url = f"{self.base_url}/udf/public"
+            elif whose == "team":
+                url = f"{self.base_url}/udf/exec-env/self"
+            else:
+                raise ValueError(
+                    'Invalid value for `whose`, should be one of: "self", "public", "community", "team"'
+                )
 
             params = request_models.ListUdfsRequest(
                 skip=skip,
                 limit=per_request,
             )
             skip += per_request
 
@@ -434,35 +459,56 @@
                 max_requests is not None and request_count == max_requests
             ):
                 break
 
         deserialized_udfs = {}
         for udf in udfs:
             if "udf_body" in udf and udf["udf_body"]:
-                deserialized_udf = BaseUdf.parse_raw(udf["udf_body"])
-                udf_id = (
-                    deserialized_udf.name
-                    if by == "name"
-                    else (
-                        udf["id"]
-                        if by == "id"
-                        else (udf["slug"] if by == "slug" else None)
+                try:
+                    deserialized_udf = BaseUdf.parse_raw(udf["udf_body"])
+                    udf_id = (
+                        deserialized_udf.name
+                        if by == "name"
+                        else (
+                            udf["id"]
+                            if by == "id"
+                            else (udf["slug"] if by == "slug" else None)
+                        )
                     )
-                )
 
-                # Restore metadata fields if they were not already present
-                if not deserialized_udf._get_metadata_safe(METADATA_FUSED_ID):
-                    deserialized_udf._set_metadata_safe(METADATA_FUSED_ID, udf["id"])
-                if not deserialized_udf._get_metadata_safe(METADATA_FUSED_SLUG):
-                    deserialized_udf._set_metadata_safe(
-                        METADATA_FUSED_SLUG, udf["slug"]
+                    # Restore metadata fields if they were not already present
+                    if not deserialized_udf._get_metadata_safe(METADATA_FUSED_ID):
+                        deserialized_udf._set_metadata_safe(
+                            METADATA_FUSED_ID, udf["id"]
+                        )
+                    if not deserialized_udf._get_metadata_safe(METADATA_FUSED_SLUG):
+                        deserialized_udf._set_metadata_safe(
+                            METADATA_FUSED_SLUG, udf["slug"]
+                        )
+
+                    filtered_public_udf = (
+                        whose == "public"
+                        and deserialized_udf._get_metadata_safe(
+                            METADATA_FUSED_EXPLORER_TAB
+                        )
+                        == "community"
+                    ) or (
+                        whose == "community"
+                        and deserialized_udf._get_metadata_safe(
+                            METADATA_FUSED_EXPLORER_TAB
+                        )
+                        != "community"
                     )
 
-                if udf_id is not None:
-                    deserialized_udfs[udf_id] = deserialized_udf
+                    if udf_id is not None and not filtered_public_udf:
+                        deserialized_udfs[udf_id] = deserialized_udf
+                except Exception as e:
+                    warnings.warn(
+                        f"UDF {udf['slug']} ({udf['id']}) could not be deserialized: {e}"
+                    )
         return UdfRegistry(deserialized_udfs)
 
     def get_udf_access_tokens(
         self,
         n: Optional[int] = None,
         *,
         skip: int = 0,
@@ -509,49 +555,55 @@
         for token in tokens:
             tokens_deserialized.append(UdfAccessToken.parse_obj(token))
 
         return tokens_deserialized
 
     def get_udf_access_token(
         self,
-        token: str,
+        token: Union[str, UdfAccessToken],
     ) -> UdfAccessToken:
+        if isinstance(token, UdfAccessToken):
+            token = token.token
         url = f"{self.base_url}/udf-access-token/by-token/{token}"
 
         r = requests.get(
             url=url,
             headers=self._generate_headers(),
             timeout=OPTIONS.request_timeout,
         )
         raise_for_status(r)
         return UdfAccessToken.parse_raw(r.content, content_type="json")
 
     def delete_udf_access_token(
         self,
-        token: str,
+        token: Union[str, UdfAccessToken],
     ) -> UdfAccessToken:
+        if isinstance(token, UdfAccessToken):
+            token = token.token
         url = f"{self.base_url}/udf-access-token/by-token/{token}"
 
         r = requests.delete(
             url=url,
             headers=self._generate_headers(),
             timeout=OPTIONS.request_timeout,
         )
         raise_for_status(r)
         return UdfAccessToken.parse_raw(r.content, content_type="json")
 
     def update_udf_access_token(
         self,
-        token: str,
+        token: Union[str, UdfAccessToken],
         *,
         client_id: Optional[str] = None,
         cache: Optional[bool] = None,
         metadata_json: Optional[Dict[str, Any]] = None,
         enabled: Optional[bool] = None,
     ) -> UdfAccessToken:
+        if isinstance(token, UdfAccessToken):
+            token = token.token
         url = f"{self.base_url}/udf-access-token/by-token/{token}"
 
         body = request_models.UpdateUdfAccessTokenRequest(
             client_id=client_id,
             cache=cache,
             metadata_json=metadata_json,
             enabled=enabled,
@@ -564,55 +616,95 @@
             timeout=OPTIONS.request_timeout,
         )
         raise_for_status(r)
         return UdfAccessToken.parse_raw(r.content, content_type="json")
 
     def create_udf_access_token(
         self,
-        udf_email: str,
+        udf_email_or_name_or_id: Optional[str] = None,
+        /,
         udf_name: Optional[str] = None,
         *,
+        udf_email: Optional[str] = None,
+        udf_id: Optional[str] = None,
         client_id: Union[str, Ellipsis, None] = ...,
         cache: bool = True,
         metadata_json: Optional[Dict[str, Any]] = None,
         enabled: bool = True,
     ) -> UdfAccessToken:
         """
         Create a token for running a UDF. The token allows anyone who has it to run
         the UDF, with the parameters they choose. The UDF will run under your environment.
 
         The token does not allow running any other UDF on your account.
 
         Args:
-            udf_email: The email of the user owning the UDF, or, if udf_name is None, the name of the UDF.
+            udf_email_or_name_or_id: A UDF ID, email address (for use with udf_name), or UDF name.
             udf_name: The name of the UDF to create the
 
         Keyword Args:
+            udf_email: The email of the user owning the UDF, or, if udf_name is None, the name of the UDF.
+            udf_id: The backend ID of the UDF to create the token for.
             client_id: If specified, overrides which realtime environment to run the UDF under.
             cache: If True, UDF tiles will be cached.
             metadata_json: Additional metadata to serve as part of the tiles metadata.json.
             enable: If True, the token can be used.
         """
-        if udf_name is None:
-            udf_name = udf_email
-            udf_email = self._whoami()["email"]
+        if udf_id is not None:
+            if (
+                udf_name is not None
+                or udf_email is not None
+                or udf_email_or_name_or_id is not None
+            ):
+                warnings.warn(
+                    "All other ways of specifying the UDF are ignored in favor of udf_id.",
+                )
+                udf_name = None
+                udf_email = None
+        elif udf_name is not None:
+            if udf_email_or_name_or_id is not None:
+                if udf_email is not None:
+                    warnings.warn(
+                        "All other ways of specifying the UDF are ignored in favor of the first argument and udf_name.",
+                    )
+                udf_email = udf_email_or_name_or_id
+        elif udf_email_or_name_or_id is not None:
+            if udf_name is not None:
+                udf_email = udf_email_or_name_or_id
+            else:
+                # Need to figure out what exactly the first argument is and how it specifies a UDF
+                is_valid_uuid = True
+                try:
+                    uuid.UUID(udf_email_or_name_or_id)
+                except ValueError:
+                    is_valid_uuid = False
+                if is_valid_uuid:
+                    udf_id = udf_email_or_name_or_id
+                elif "/" in udf_email_or_name_or_id:
+                    udf_email, udf_name = udf_email_or_name_or_id.split("/", maxsplit=1)
+                else:
+                    udf_name = udf_email_or_name_or_id
+                    udf_email = self._whoami()["email"]
+        else:
+            raise ValueError("No UDF specified to create an access token for.")
 
         if client_id is Ellipsis:
             client_id = self._automatic_realtime_client_id()
 
         if client_id is Ellipsis:
             raise ValueError("Failed to detect realtime client ID")
 
         url = f"{self.base_url}/udf-access-token/new"
 
         metadata_json = metadata_json or {}
 
         body = request_models.CreateUdfAccessTokenRequest(
             udf_email=udf_email,
             udf_slug=udf_name,
+            udf_id=udf_id,
             client_id=client_id,
             cache=cache,
             metadata_json=metadata_json,
             enabled=enabled,
         ).dict()  # type: ignore
 
         r = requests.post(
@@ -1028,25 +1120,36 @@
             post_open_table(
                 table=table,
                 fetch_samples=fetch_samples,
             )
 
         return folder
 
-    def list(self, path: str) -> List[str]:
-        list_request_url = f"{self.base_url}/files/list"
+    @overload
+    def list(self, path: str, *, details: Literal[True]) -> List[ListDetails]:
+        ...
+
+    @overload
+    def list(self, path: str, *, details: Literal[False] = False) -> List[str]:
+        ...
+
+    def list(self, path: str, *, details: bool = False):
+        list_request_url = f"{self.base_url}/files/list{'-details' if details else ''}"
         params = request_models.ListPathRequest(path=path)
         r = requests.get(
             url=list_request_url,
             params=params.dict(),
             headers=self._generate_headers(),
             timeout=OPTIONS.request_timeout,
         )
         raise_for_status(r)
-        return r.json()
+        result = r.json()
+        if details:
+            result = [ListDetails.parse_obj(detail) for detail in result]
+        return result
 
     def delete(
         self,
         path: str,
         max_deletion_depth: Union[int, Literal["unlimited"]] = 2,
     ) -> bool:
         delete_request_url = f"{self.base_url}/files/delete"
```

### Comparing `fused-1.5.4/fused/api/credentials.py` & `fused-1.6.1/fused/api/credentials.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/api/docker_api.py` & `fused-1.6.1/fused/api/docker_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,25 @@
 import shlex
 import shutil
 import subprocess
 from base64 import b64encode
 from functools import lru_cache
 from io import SEEK_SET, BytesIO
 from pathlib import Path
-from typing import BinaryIO, Callable, Dict, List, Literal, Optional, Sequence, Union
+from typing import (
+    BinaryIO,
+    Callable,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Sequence,
+    Union,
+    overload,
+)
 from uuid import uuid4
 
 import geopandas as gpd
 import pandas as pd
 import requests
 from pydantic import BaseModel
 
@@ -30,14 +40,15 @@
 from fused.api.api import FusedAPI
 from fused.models import JoinInput, JoinSingleFileInput, MapInput
 from fused.models.api import (
     JobConfig,
     JobStepConfig,
     JoinJobStepConfig,
     JoinSinglefileJobStepConfig,
+    ListDetails,
     MapJobStepConfig,
     Table,
 )
 from fused.models.api._folder import Folder
 
 # TODO: Consider making this us-west-2, depending on where the user is logged in
 # DEFAULT_REPOSITORY = "926411091187.dkr.ecr.us-east-1.amazonaws.com/fused-job2"
@@ -623,20 +634,34 @@
 
     def _health(self) -> bool:
         """Check the health of the API backend"""
         runnable = self._make_run_command("version", [])
         runnable.run_and_get_output()
         return True
 
-    def list(self, path: str) -> List[str]:
+    @overload
+    def list(self, path: str, *, details: Literal[True]) -> List[ListDetails]:
+        ...
+
+    @overload
+    def list(self, path: str, *, details: Literal[False] = False) -> List[str]:
+        ...
+
+    def list(self, path: str, *, details: bool = False):
         args = ["--path", path]
 
+        if details:
+            args.append("--details")
+
         runnable = self._make_run_command("files-list", args)
         content = runnable.run_and_get_bytes()
-        return json.loads(content)
+        result = json.loads(content)
+        if details:
+            result = [ListDetails.parse_obj(detail) for detail in result]
+        return result
 
     def delete(self, path: str, max_deletion_depth: int | Literal["unlimited"]) -> bool:
         args = ["--path", path, "--max-deletion-depth", str(max_deletion_depth)]
         runnable = self._make_run_command("files-delete", args)
         content = runnable.run_and_get_bytes()
         return json.loads(content)
```

### Comparing `fused-1.5.4/fused/api/docker_http_api.py` & `fused-1.6.1/fused/api/docker_http_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 from __future__ import annotations
 
 import json
 import shutil
 from functools import lru_cache
 from pathlib import Path
-from typing import Any, BinaryIO, Dict, List, Literal, Optional, Sequence, Union
+from typing import (
+    Any,
+    BinaryIO,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Sequence,
+    Union,
+    overload,
+)
 
 import geopandas as gpd
 import pandas as pd
 import requests
 from pydantic import BaseModel
 
 from fused._deserialize import (
@@ -23,14 +33,15 @@
 from fused.api._open_dataset import post_open_table
 from fused.models import JoinInput, JoinSingleFileInput, MapInput
 from fused.models.api import (
     JobConfig,
     JobStepConfig,
     JoinJobStepConfig,
     JoinSinglefileJobStepConfig,
+    ListDetails,
     MapJobStepConfig,
     Table,
 )
 from fused.models.api._folder import Folder
 
 DEFAULT_ENDPOINT = "http://localhost:8789"
 
@@ -443,20 +454,34 @@
         r = requests.get(
             url=f"{self.endpoint}/health",
             timeout=OPTIONS.request_timeout,
         )
         raise_for_status(r)
         return True
 
-    def list(self, path: str) -> List[str]:
+    @overload
+    def list(self, path: str, *, details: Literal[True]) -> List[ListDetails]:
+        ...
+
+    @overload
+    def list(self, path: str, *, details: Literal[False] = False) -> List[str]:
+        ...
+
+    def list(self, path: str, *, details: bool = False):
         args = ["--path", path]
 
+        if details:
+            args.append("--details")
+
         runnable = self._make_run_command("files-list", args)
         content = runnable.run_and_get_bytes()
-        return json.loads(content)
+        result = json.loads(content)
+        if details:
+            result = [ListDetails.parse_obj(detail) for detail in result]
+        return result
 
     def delete(self, path: str, max_deletion_depth: int | Literal["unlimited"]) -> bool:
         args = ["--path", path, "--max-deletion-depth", str(max_deletion_depth)]
         runnable = self._make_run_command("files-delete", args)
         content = runnable.run_and_get_bytes()
         return json.loads(content)
```

### Comparing `fused-1.5.4/fused/core/_cache.py` & `fused-1.6.1/fused/core/_cache.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/core/_download.py` & `fused-1.6.1/fused/core/_download.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/core/_impl/_download_impl.py` & `fused-1.6.1/fused/core/_impl/_download_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/core/_impl/_realtime_ops_impl.py` & `fused-1.6.1/fused/core/_impl/_realtime_ops_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/core/_impl/_table_ops_impl.py` & `fused-1.6.1/fused/core/_impl/_table_ops_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/core/_impl/_udf_ops_impl.py` & `fused-1.6.1/fused/core/_impl/_udf_ops_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/core/_realtime_ops.py` & `fused-1.6.1/fused/core/_realtime_ops.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/core/_table_ops.py` & `fused-1.6.1/fused/core/_table_ops.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/core/_udf_ops.py` & `fused-1.6.1/fused/core/_udf_ops.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/__init__.py` & `fused-1.6.1/fused/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/_codegen/job.py` & `fused-1.6.1/fused/models/_codegen/job.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/_codegen/udf.py` & `fused-1.6.1/fused/models/_codegen/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/api/dataset.py` & `fused-1.6.1/fused/models/api/dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/api/job.py` & `fused-1.6.1/fused/models/api/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     List,
     Literal,
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
-    overload,
 )
 from urllib.parse import urlparse
 
 from IPython import get_ipython
 from IPython.core.inputsplitter import IPythonInputSplitter
 from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr
 
@@ -28,15 +27,20 @@
     fused_join_repr,
     fused_join_singlefile_repr,
     fused_map_repr,
     fused_udf_step_repr,
 )
 from fused._str_utils import append_url_part, is_url
 from fused._udf.execute_v2 import execute_against_sample, validate_imports_whitelist
-from fused.warnings import FusedDefaultWarning, FusedIgnoredWarning, FusedTypeWarning
+from fused.warnings import (
+    FusedDefaultWarning,
+    FusedIgnoredWarning,
+    FusedPathWarning,
+    FusedTypeWarning,
+)
 
 from ...models.schema import Schema
 from .._codegen import (
     create_directory_and_zip,
     extract_parameters,
     generate_meta_json,
     generate_readme,
@@ -199,14 +203,15 @@
 
     def _validate_for_run(
         self,
         *,
         ignore_no_udf: bool = False,
         ignore_no_output: bool = False,
         validate_imports: Optional[bool] = None,
+        validate_inputs: bool = True,
     ):
         has_udf = hasattr(self, "udf")
         has_output = hasattr(self, "output")
         _common_validate_for_run(
             output=self.output if has_output else None,
             udf=self.udf if has_udf else None,
             ignore_no_udf=ignore_no_udf if has_udf else True,
@@ -222,14 +227,15 @@
         region: str | None = None,
         disk_size_gb: int | None = None,
         additional_env: List[str] | None = None,
         image_name: Optional[str] = None,
         ignore_no_udf: bool = False,
         ignore_no_output: bool = False,
         validate_imports: Optional[bool] = None,
+        validate_inputs: bool = True,
         overwrite: Optional[bool] = None,
     ) -> RunResponse:
         """Execute this operation
 
         Args:
             output_table: The name of the table to write to. Defaults to None.
             instance_type: The AWS EC2 instance type to use for the job. Acceptable strings are "m5.large", "m5.xlarge", "m5.2xlarge", "m5.4xlarge", "r5.large", "r5.xlarge", "r5.2xlarge", "r5.4xlarge". Defaults to None.
@@ -260,33 +266,36 @@
             region=region,
             disk_size_gb=disk_size_gb,
             additional_env=additional_env,
             image_name=image_name,
             ignore_no_udf=ignore_no_udf,
             ignore_no_output=ignore_no_output,
             validate_imports=validate_imports,
+            validate_inputs=validate_inputs,
         )
 
     def _run_remote(
         self,
         instance_type: Optional[WHITELISTED_INSTANCE_TYPES] = None,
         *,
         region: str | None = None,
         disk_size_gb: int | None = None,
         additional_env: List[str] | None = None,
         image_name: Optional[str] = None,
         ignore_no_udf: bool = False,
         ignore_no_output: bool = False,
         validate_imports: Optional[bool] = None,
+        validate_inputs: bool = True,
     ) -> RunResponse:
         # TODO: if the user uses start_job, this validation will never happen
         self._validate_for_run(
             ignore_no_udf=ignore_no_udf,
             ignore_no_output=ignore_no_output,
             validate_imports=validate_imports,
+            validate_inputs=validate_inputs,
         )
         config = JobConfig(steps=[self])
         return self._api.start_job(
             config,
             instance_type=instance_type,
             region=region,
             disk_size_gb=disk_size_gb,
@@ -464,14 +473,58 @@
     """Maximum value for `partitioning_method` to use per file. If `None`, defaults to _1/10th_ of the total value of `partitioning_method`. So if the value is `None` and `partitioning_method` is `"area"`, then each file will be have no more than 1/10th the total area of all geometries.
     """
 
     partitioning_maximum_per_chunk: Optional[int] = 65000
     """Maximum value for `partitioning_method` to use per chunk. If `None`, defaults to _1/100th_ of the total value of `partitioning_method`. So if the value is `None` and `partitioning_method` is `"area"`, then each file will be have no more than 1/100th the total area of all geometries.
     """
 
+    def _validate_for_run(
+        self,
+        *,
+        ignore_no_udf: bool = False,
+        ignore_no_output: bool = False,
+        validate_imports: Optional[bool] = None,
+        validate_inputs: bool = True,
+    ):
+        super()._validate_for_run(
+            ignore_no_udf=ignore_no_udf,
+            ignore_no_output=ignore_no_output,
+            validate_imports=validate_imports,
+            validate_inputs=validate_inputs,
+        )
+
+        if validate_inputs:
+
+            def _validate_input(input: str):
+                if isinstance(input, str):
+                    if (
+                        input.startswith("file://")
+                        or input.startswith("/")
+                        or input.startswith("./")
+                    ):
+                        warnings.warn(
+                            f"Input to partition job step ({input}) is a local file reference, which will be resolved on the backend and not on your local system. If you meant to partition a local file, use `fused.upload` first and then use the remote path.",
+                            FusedPathWarning,
+                        )
+                    elif input.startswith("fd://"):
+                        warnings.warn(
+                            f"Input to partition job step ({input}) is fd:// path, which may not be accepted by this version of the backend. Pass the exact S3 or GCS URL instead.",
+                            FusedPathWarning,
+                        )
+                else:
+                    warnings.warn(
+                        "Input to partition job step is not a string.", FusedTypeWarning
+                    )
+
+            if isinstance(self.input, (list, tuple)):
+                for input in self.input:
+                    _validate_input(input)
+            else:
+                _validate_input(self.input)
+
     def _repr_html_(self) -> str:
         return fused_ingestion_repr(self)
 
 
 class GDALOpenConfig(BaseModel):
     """A class to define options for how to open files with GDAL."""
 
@@ -554,14 +607,15 @@
         region: str | None = None,
         disk_size_gb: int | None = None,
         additional_env: List[str] | None = None,
         image_name: Optional[str] = None,
         ignore_no_udf: bool = False,
         ignore_no_output: bool = False,
         validate_imports: Optional[bool] = None,
+        validate_inputs: bool = True,
         overwrite: Optional[bool] = None,
     ) -> RunResponse:
         """Execute this operation
 
         Args:
             output_table: The name of the table to write to. Defaults to None.
             instance_type: The AWS EC2 instance type to use for the job. Acceptable strings are "m5.large", "m5.xlarge", "m5.2xlarge", "m5.4xlarge", "r5.large", "r5.xlarge", "r5.2xlarge", "r5.4xlarge". Defaults to None.
@@ -593,14 +647,15 @@
             region=region,
             disk_size_gb=disk_size_gb,
             additional_env=additional_env,
             image_name=image_name,
             ignore_no_udf=ignore_no_udf,
             ignore_no_output=ignore_no_output,
             validate_imports=validate_imports,
+            validate_inputs=validate_inputs,
         )
 
     def set_output(
         self,
         output: Optional[str] = None,
         output_metadata: Optional[str] = None,
         inplace: bool = False,
@@ -727,14 +782,15 @@
 
     def _validate_for_run(
         self,
         *,
         ignore_no_udf: bool = False,
         ignore_no_output: bool = False,
         validate_imports: Optional[bool] = None,
+        validate_inputs: bool = True,
     ):
         if not ignore_no_udf and not self.udf.code:
             raise ValueError(
                 "No UDF code is set. Set the `udf` attribute or pass `ignore_no_udf=True`."
             )
 
         # TODO: should _common_validate_before_run be used here?
@@ -751,97 +807,60 @@
         if self.input is not None and len(self.input) >= file_id:
             return self.run_local(self.input[file_id])
         else:
             raise ValueError("No input is set.")
 
     def run_file(
         self,
-        df_left: Any = None,
+        *,
         _client_id: Optional[str] = None,
         _include_log: bool = False,
         _dtype_out_vector: str = "parquet",
         _dtype_out_raster: str = "tiff",
         **kwargs,
     ) -> UdfEvaluationResult:
         # TODO: fix circular import error
         from fused._quick.udf import run as _run_realtime
 
         res = _run_realtime(
-            df_left=df_left,
             step_config=self,
             params=kwargs,
             client_id=_client_id,
             dtype_out_raster=_dtype_out_raster,
             dtype_out_vector=_dtype_out_vector,
         )
         if _include_log:
             return res
         else:
             return res.data
 
-    @overload
-    def run_tile(
-        input_tiff_path: str = None,
-        *,
-        x: float,
-        y: float,
-        z: float,
-        lat: float = None,
-        lon: float = None,
-        _include_log: bool = False,
-        _client_id: Optional[str] = None,
-        _dtype_out_vector: str = "parquet",
-        _dtype_out_raster: str = "tiff",
-    ) -> UdfTileEvaluationResult:
-        ...
-
     # TODO: do we enforce pattern to have same args in overload, for typehints?
     def run_tile(
         self,
-        data: Any = None,
         *,
-        lat: float = None,
-        lon: float = None,
         x: float = None,
         y: float = None,
         z: float = None,
         _include_log: bool = False,
         _client_id: Optional[str] = None,
         _dtype_out_vector: str = "parquet",
         _dtype_out_raster: str = "tiff",
+        **kwargs,
     ) -> UdfTileEvaluationResult:
         from fused._quick.udf import run_tile as _run_realtime_tile
 
-        def lat_lon_to_xyz(lat, lon, radius=1.0):
-            import math
-
-            # Convert latitude and longitude from degrees to radians
-            lat_rad = math.radians(lat)
-            lon_rad = math.radians(lon)
-
-            # Calculate x, y, and z coordinates
-            x = radius * math.cos(lat_rad) * math.cos(lon_rad)
-            y = radius * math.cos(lat_rad) * math.sin(lon_rad)
-            z = radius * math.sin(lat_rad)
-
-            return x, y, z
-
-        # lat-lon to xyz
-        if lat is not None and lon is not None:
-            x, y, z = lat_lon_to_xyz(lat, lon)
-
         res = _run_realtime_tile(
-            data=data,
             step_config=self,
             x=x,
             y=y,
             z=z,
             client_id=_client_id,
             dtype_out_raster=_dtype_out_raster,
             dtype_out_vector=_dtype_out_vector,
+            params=kwargs,
         )
         if _include_log:
             return res
         else:
             return res.data
 
 
@@ -936,14 +955,15 @@
 
     def _validate_for_run(
         self,
         *,
         ignore_no_udf: bool = False,
         ignore_no_output: bool = False,
         validate_imports: Optional[bool] = None,
+        validate_inputs: bool = True,
     ):
         _common_validate_for_run(
             output=self.output,
             udf=self.udf,
             ignore_no_udf=ignore_no_udf,
             ignore_no_output=ignore_no_output,
             validate_imports=validate_imports,
@@ -1116,14 +1136,15 @@
         return fused_map_repr(self)
 
     def run_realtime(
         self,
         df_left: Optional[
             Union[pd.DataFrame, gpd.GeoDataFrame, pa.Table, str, Path]
         ] = None,
+        *,
         _client_id: Optional[str] = None,
         **kwargs,
     ) -> UdfEvaluationResult:
         # TODO: fix circular import error
         from fused._quick.udf import run as _run_realtime
 
         return _run_realtime(
@@ -1223,14 +1244,15 @@
 
     def _validate_for_run(
         self,
         *,
         ignore_no_udf: bool = False,
         ignore_no_output: bool = False,
         validate_imports: Optional[bool] = None,
+        validate_inputs: bool = True,
     ):
         _common_validate_for_run(
             output=self.output,
             udf=self.udf,
             ignore_no_udf=ignore_no_udf,
             ignore_no_output=ignore_no_output,
             validate_imports=validate_imports,
@@ -1395,14 +1417,15 @@
         self,
         df_left: Optional[
             Union[pd.DataFrame, gpd.GeoDataFrame, pa.Table, str, Path]
         ] = None,
         df_right: Optional[
             Union[pd.DataFrame, gpd.GeoDataFrame, pa.Table, str, Path]
         ] = None,
+        *,
         _client_id: Optional[str] = None,
         **kwargs,
     ) -> UdfEvaluationResult:
         # TODO: fix circular import error
         from fused._quick.udf import run as _run_realtime
 
         return _run_realtime(
@@ -1505,14 +1528,15 @@
 
     def _validate_for_run(
         self,
         *,
         ignore_no_udf: bool = False,
         ignore_no_output: bool = False,
         validate_imports: Optional[bool] = None,
+        validate_inputs: bool = True,
     ):
         _common_validate_for_run(
             output=self.output,
             udf=self.udf,
             ignore_no_udf=ignore_no_udf,
             ignore_no_output=ignore_no_output,
             validate_imports=validate_imports,
@@ -1694,33 +1718,36 @@
 
     def _validate_for_run(
         self,
         *,
         ignore_no_udf: bool = False,
         ignore_no_output: bool = False,
         validate_imports: Optional[bool] = None,
+        validate_inputs: bool = True,
     ):
         for step in self.steps:
             step._validate_for_run(
                 ignore_no_udf=ignore_no_udf,
                 ignore_no_output=ignore_no_output,
                 validate_imports=validate_imports,
+                validate_inputs=validate_inputs,
             )
 
     def run_remote(
         self,
         instance_type: Optional[WHITELISTED_INSTANCE_TYPES] = None,
         *,
         region: str | None = None,
         disk_size_gb: int | None = None,
         additional_env: List[str] | None = None,
         image_name: Optional[str] = None,
         ignore_no_udf: bool = False,
         ignore_no_output: bool = False,
         validate_imports: Optional[bool] = None,
+        validate_inputs: bool = True,
         **kwargs,
     ) -> RunResponse:
         """Execute an operation
 
         Keyword Args:
             region: The AWS region in which to run. Defaults to None.
             instance_type: The AWS EC2 instance type to use for the job. Acceptable strings are "m5.large", "m5.xlarge", "m5.2xlarge", "m5.4xlarge", "r5.large", "r5.xlarge", "r5.2xlarge", "r5.4xlarge". Defaults to None.
@@ -1734,14 +1761,15 @@
         ret = _maybe_inplace(self, inplace=False)
 
         # TODO: if the user uses start_job, this validation will never happen
         ret._validate_for_run(
             ignore_no_udf=ignore_no_udf,
             ignore_no_output=ignore_no_output,
             validate_imports=validate_imports,
+            validate_inputs=validate_inputs,
         )
 
         for step in ret.steps:
             if hasattr(step, "udf"):
                 filtered_kwargs = {
                     k: v for k, v in kwargs.items() if k in step.udf._parameter_list
                 }
```

### Comparing `fused-1.5.4/fused/models/api/udf_access_token.py` & `fused-1.6.1/fused/models/api/udf_access_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,20 +23,21 @@
     if ret:
         return f"?{ret}"
     return ret
 
 
 class UdfAccessToken(FusedBaseModel):
     token: str
-    udf_email: str
-    udf_slug: str
+    udf_email: Optional[str] = None
+    udf_slug: Optional[str] = None
+    udf_id: Optional[str] = None
     enabled: bool
     owning_user_id: str
     client_id: Optional[str]
-    cache: bool
+    cache: Optional[bool] = None
     metadata_json: Optional[Dict[str, Any]]
     last_updated: datetime
 
     def update(
         self,
         client_id: Optional[str] = None,
         cache: Optional[bool] = None,
```

### Comparing `fused-1.5.4/fused/models/base.py` & `fused-1.6.1/fused/models/base.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/coerce_dataset.py` & `fused-1.6.1/fused/models/coerce_dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/input.py` & `fused-1.6.1/fused/models/input.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/internal/dataset.py` & `fused-1.6.1/fused/models/internal/dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/internal/job.py` & `fused-1.6.1/fused/models/internal/job.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/migrations.py` & `fused-1.6.1/fused/models/migrations.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/request.py` & `fused-1.6.1/fused/models/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -197,16 +197,17 @@
 
 class ListUdfAccessTokensRequest(BaseModel):
     skip: Optional[StrictInt] = None
     limit: Optional[StrictInt] = None
 
 
 class CreateUdfAccessTokenRequest(BaseModel):
-    udf_email: str
-    udf_slug: str
+    udf_email: Optional[str] = None
+    udf_slug: Optional[str] = None
+    udf_id: Optional[str] = None
     client_id: Optional[str] = None
     cache: bool = True
     metadata_json: Dict[str, Any] = {}
     enabled: bool = True
 
 
 class UpdateUdfAccessTokenRequest(BaseModel):
```

### Comparing `fused-1.5.4/fused/models/schema.py` & `fused-1.6.1/fused/models/schema.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/udf/_eval_result.py` & `fused-1.6.1/fused/models/udf/_eval_result.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/udf/_specialized_udfs.py` & `fused-1.6.1/fused/models/udf/_specialized_udfs.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/udf/_udf_registry.py` & `fused-1.6.1/fused/models/udf/_udf_registry.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/udf/base_udf.py` & `fused-1.6.1/fused/models/udf/base_udf.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     stringify_named_params,
     structure_params,
 )
 from .._inplace import _maybe_inplace
 
 METADATA_FUSED_ID = "fused:id"
 METADATA_FUSED_SLUG = "fused:slug"
+METADATA_FUSED_EXPLORER_TAB = "fused:explorerTab"
 
 
 class HeaderSequence(BaseModel):
     __root__: Sequence[Header]
 
     def _repr_html_(self) -> str:
         return fused_header_repr(self)
```

### Comparing `fused-1.5.4/fused/models/udf/common.py` & `fused-1.6.1/fused/models/udf/common.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/udf/header.py` & `fused-1.6.1/fused/models/udf/header.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/udf/output.py` & `fused-1.6.1/fused/models/udf/output.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/udf/udf.py` & `fused-1.6.1/fused/models/udf/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/models/urls.py` & `fused-1.6.1/fused/models/urls.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/fused/warnings.py` & `fused-1.6.1/fused/warnings.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.4/pyproject.toml` & `fused-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "fused"
 # Version is set to 0.0.0 as the version string is automatically generated by
 # https://github.com/mtkennerly/poetry-dynamic-versioning
-version = "1.5.4"
+version = "1.6.1"
 description = ""
 authors = []
 readme = "README.md"
 packages = [{ include = "fused" }]
 
 [project.urls]
 Homepage = "https://www.fused.io"
```

### Comparing `fused-1.5.4/PKG-INFO` & `fused-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fused
-Version: 1.5.4
+Version: 1.6.1
 Summary: 
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

