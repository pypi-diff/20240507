# Comparing `tmp/fractal_server-2.0.3.tar.gz` & `tmp/fractal_server-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-2.0.3.tar", max compression
+gzip compressed data, was "fractal_server-2.0.4.tar", max compression
```

## Comparing `fractal_server-2.0.3.tar` & `fractal_server-2.0.4.tar`

### file list

```diff
@@ -1,169 +1,169 @@
--rw-r--r--   0        0        0     1576 2024-05-03 06:48:17.928800 fractal_server-2.0.3/LICENSE
--rw-r--r--   0        0        0     2466 2024-05-03 06:48:17.928800 fractal_server-2.0.3/README.md
--rw-r--r--   0        0        0       22 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/__init__.py
--rw-r--r--   0        0        0     4958 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/__init__.py
--rw-r--r--   0        0        0     4042 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      267 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0      567 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     3378 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/security.py
--rw-r--r--   0        0        0      458 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v1/__init__.py
--rw-r--r--   0        0        0     2017 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v1/dataset.py
--rw-r--r--   0        0        0     3304 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v1/job.py
--rw-r--r--   0        0        0      859 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v1/project.py
--rw-r--r--   0        0        0     1095 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v1/state.py
--rw-r--r--   0        0        0     2782 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v1/task.py
--rw-r--r--   0        0        0     3950 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v1/workflow.py
--rw-r--r--   0        0        0      473 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v2/__init__.py
--rw-r--r--   0        0        0      588 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v2/collection_state.py
--rw-r--r--   0        0        0     1455 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v2/dataset.py
--rw-r--r--   0        0        0     1535 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v2/job.py
--rw-r--r--   0        0        0      817 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v2/project.py
--rw-r--r--   0        0        0     3257 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v2/task.py
--rw-r--r--   0        0        0     1069 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v2/workflow.py
--rw-r--r--   0        0        0     1532 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/models/v2/workflowtask.py
--rw-r--r--   0        0        0        0 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/admin/__init__.py
--rw-r--r--   0        0        0    13996 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/admin/v1.py
--rw-r--r--   0        0        0     9830 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/admin/v2.py
--rw-r--r--   0        0        0      315 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/__init__.py
--rw-r--r--   0        0        0      958 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v1/__init__.py
--rw-r--r--   0        0        0    11973 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v1/_aux_functions.py
--rw-r--r--   0        0        0    16923 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v1/dataset.py
--rw-r--r--   0        0        0     5436 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v1/job.py
--rw-r--r--   0        0        0    15799 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v1/project.py
--rw-r--r--   0        0        0     6129 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v1/task.py
--rw-r--r--   0        0        0     8882 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v1/task_collection.py
--rw-r--r--   0        0        0    10942 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v1/workflow.py
--rw-r--r--   0        0        0     5582 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v1/workflowtask.py
--rw-r--r--   0        0        0     1487 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v2/__init__.py
--rw-r--r--   0        0        0    14301 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v2/_aux_functions.py
--rw-r--r--   0        0        0     8248 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v2/dataset.py
--rw-r--r--   0        0        0     7894 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v2/images.py
--rw-r--r--   0        0        0     5325 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v2/job.py
--rw-r--r--   0        0        0     5594 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v2/project.py
--rw-r--r--   0        0        0     6394 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v2/status.py
--rw-r--r--   0        0        0     6940 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v2/submit.py
--rw-r--r--   0        0        0     7130 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v2/task.py
--rw-r--r--   0        0        0     8988 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v2/task_collection.py
--rw-r--r--   0        0        0     1628 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v2/task_legacy.py
--rw-r--r--   0        0        0    11863 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v2/workflow.py
--rw-r--r--   0        0        0     8802 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/api/v2/workflowtask.py
--rw-r--r--   0        0        0     4885 2024-05-03 06:48:17.932800 fractal_server-2.0.3/fractal_server/app/routes/auth.py
--rw-r--r--   0        0        0        0 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/routes/aux/__init__.py
--rw-r--r--   0        0        0     1251 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/routes/aux/_job.py
--rw-r--r--   0        0        0      675 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/routes/aux/_runner.py
--rw-r--r--   0        0        0       16 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0        0 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0      829 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/async_wrap.py
--rw-r--r--   0        0        0      119 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/components.py
--rw-r--r--   0        0        0     4159 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/executors/__init__.py
--rw-r--r--   0        0        0       65 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/__init__.py
--rw-r--r--   0        0        0     8841 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/_batching.py
--rw-r--r--   0        0        0     1908 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
--rw-r--r--   0        0        0     4421 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    15552 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/_slurm_config.py
--rw-r--r--   0        0        0     5123 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    44451 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/executor.py
--rw-r--r--   0        0        0     5852 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/remote.py
--rw-r--r--   0        0        0      206 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/filenames.py
--rw-r--r--   0        0        0     1254 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/set_start_and_last_task_index.py
--rw-r--r--   0        0        0     3180 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/task_files.py
--rw-r--r--   0        0        0    13620 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v1/__init__.py
--rw-r--r--   0        0        0    21246 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v1/_common.py
--rw-r--r--   0        0        0     6839 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v1/_local/__init__.py
--rw-r--r--   0        0        0     3147 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v1/_local/_local_config.py
--rw-r--r--   0        0        0     1493 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v1/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v1/_local/executor.py
--rw-r--r--   0        0        0    10853 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v1/_slurm/__init__.py
--rw-r--r--   0        0        0     2738 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v1/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     5977 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0     3294 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v1/common.py
--rw-r--r--   0        0        0     4684 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v1/handle_failed_job.py
--rw-r--r--   0        0        0    12500 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/__init__.py
--rw-r--r--   0        0        0     5881 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/_local/__init__.py
--rw-r--r--   0        0        0     3630 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/_local/_local_config.py
--rw-r--r--   0        0        0     1614 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/_local/executor.py
--rw-r--r--   0        0        0     4409 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/_slurm/__init__.py
--rw-r--r--   0        0        0     2793 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     6726 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0      639 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/deduplicate_list.py
--rw-r--r--   0        0        0     5415 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/handle_failed_job.py
--rw-r--r--   0        0        0     1281 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/merge_outputs.py
--rw-r--r--   0        0        0    14160 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/runner.py
--rw-r--r--   0        0        0    11067 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/runner_functions.py
--rw-r--r--   0        0        0     3710 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/runner_functions_low_level.py
--rw-r--r--   0        0        0     1866 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/task_interface.py
--rw-r--r--   0        0        0      912 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/runner/v2/v1_compat.py
--rw-r--r--   0        0        0       40 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/__init__.py
--rw-r--r--   0        0        0     3461 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/_validators.py
--rw-r--r--   0        0        0      692 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/state.py
--rw-r--r--   0        0        0     3113 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/user.py
--rw-r--r--   0        0        0     1809 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v1/__init__.py
--rw-r--r--   0        0        0     4302 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v1/applyworkflow.py
--rw-r--r--   0        0        0     3444 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v1/dataset.py
--rw-r--r--   0        0        0     1274 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v1/dumps.py
--rw-r--r--   0        0        0     3829 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v1/manifest.py
--rw-r--r--   0        0        0     1218 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v1/project.py
--rw-r--r--   0        0        0     3704 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v1/task.py
--rw-r--r--   0        0        0     3057 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v1/task_collection.py
--rw-r--r--   0        0        0     4618 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v1/workflow.py
--rw-r--r--   0        0        0     1852 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v2/__init__.py
--rw-r--r--   0        0        0     2599 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v2/dataset.py
--rw-r--r--   0        0        0     2063 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v2/dumps.py
--rw-r--r--   0        0        0     3250 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v2/job.py
--rw-r--r--   0        0        0     6243 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v2/manifest.py
--rw-r--r--   0        0        0      736 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v2/project.py
--rw-r--r--   0        0        0      332 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v2/status.py
--rw-r--r--   0        0        0     4672 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v2/task.py
--rw-r--r--   0        0        0     3171 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v2/task_collection.py
--rw-r--r--   0        0        0     1827 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v2/workflow.py
--rw-r--r--   0        0        0     6552 2024-05-03 06:48:17.936800 fractal_server-2.0.3/fractal_server/app/schemas/v2/workflowtask.py
--rw-r--r--   0        0        0    11203 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0    14859 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/config.py
--rw-r--r--   0        0        0     2918 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/data_migrations/2_0_3.py
--rw-r--r--   0        0        0      398 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/data_migrations/README.md
--rw-r--r--   0        0        0      196 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/images/__init__.py
--rw-r--r--   0        0        0     4167 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/images/models.py
--rw-r--r--   0        0        0     2209 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/images/tools.py
--rw-r--r--   0        0        0     4178 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/logger.py
--rw-r--r--   0        0        0     3381 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/main.py
--rw-r--r--   0        0        0       59 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/README
--rw-r--r--   0        0        0     2630 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      526 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     1157 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
--rw-r--r--   0        0        0     8770 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0     8433 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/5bf02391cfef_v2.py
--rw-r--r--   0        0        0     1632 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
--rw-r--r--   0        0        0     1353 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
--rw-r--r--   0        0        0     2684 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
--rw-r--r--   0        0        0     1115 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
--rw-r--r--   0        0        0     1057 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
--rw-r--r--   0        0        0      883 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
--rw-r--r--   0        0        0     1849 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
--rw-r--r--   0        0        0      867 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
--rw-r--r--   0        0        0      949 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
--rw-r--r--   0        0        0      963 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
--rw-r--r--   0        0        0     1221 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
--rw-r--r--   0        0        0      746 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/syringe.py
--rw-r--r--   0        0        0       23 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0     5379 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/tasks/endpoint_operations.py
--rw-r--r--   0        0        0     3278 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/tasks/utils.py
--rw-r--r--   0        0        0     3775 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/tasks/v1/_TaskCollectPip.py
--rw-r--r--   0        0        0        0 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/tasks/v1/__init__.py
--rw-r--r--   0        0        0    11731 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/tasks/v1/background_operations.py
--rw-r--r--   0        0        0      502 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/tasks/v1/get_collection_data.py
--rw-r--r--   0        0        0     3775 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/tasks/v2/_TaskCollectPip.py
--rw-r--r--   0        0        0        0 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/tasks/v2/__init__.py
--rw-r--r--   0        0        0    12922 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/tasks/v2/background_operations.py
--rw-r--r--   0        0        0      502 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/tasks/v2/get_collection_data.py
--rw-r--r--   0        0        0      448 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/urls.py
--rw-r--r--   0        0        0     2115 2024-05-03 06:48:17.940800 fractal_server-2.0.3/fractal_server/utils.py
--rw-r--r--   0        0        0     3052 2024-05-03 06:48:17.940800 fractal_server-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     4202 1970-01-01 00:00:00.000000 fractal_server-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1576 2024-05-06 12:52:10.654958 fractal_server-2.0.4/LICENSE
+-rw-r--r--   0        0        0     2486 2024-05-06 12:52:10.654958 fractal_server-2.0.4/README.md
+-rw-r--r--   0        0        0       22 2024-05-06 12:52:10.658958 fractal_server-2.0.4/fractal_server/__init__.py
+-rw-r--r--   0        0        0     4958 2024-05-06 12:52:10.658958 fractal_server-2.0.4/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2024-05-06 12:52:10.658958 fractal_server-2.0.4/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2024-05-06 12:52:10.658958 fractal_server-2.0.4/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0     4042 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      267 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0      567 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     3378 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0      458 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/__init__.py
+-rw-r--r--   0        0        0     2017 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/dataset.py
+-rw-r--r--   0        0        0     3304 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/job.py
+-rw-r--r--   0        0        0      859 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/project.py
+-rw-r--r--   0        0        0     1095 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/state.py
+-rw-r--r--   0        0        0     2782 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/task.py
+-rw-r--r--   0        0        0     3950 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v1/workflow.py
+-rw-r--r--   0        0        0      473 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/__init__.py
+-rw-r--r--   0        0        0      588 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/collection_state.py
+-rw-r--r--   0        0        0     1455 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/dataset.py
+-rw-r--r--   0        0        0     1535 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/job.py
+-rw-r--r--   0        0        0      817 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/project.py
+-rw-r--r--   0        0        0     3257 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/task.py
+-rw-r--r--   0        0        0     1069 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/workflow.py
+-rw-r--r--   0        0        0     1532 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/models/v2/workflowtask.py
+-rw-r--r--   0        0        0        0 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/admin/__init__.py
+-rw-r--r--   0        0        0    13996 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/admin/v1.py
+-rw-r--r--   0        0        0     9830 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/admin/v2.py
+-rw-r--r--   0        0        0      315 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/__init__.py
+-rw-r--r--   0        0        0      958 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/__init__.py
+-rw-r--r--   0        0        0    11973 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0    16923 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/dataset.py
+-rw-r--r--   0        0        0     5436 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/job.py
+-rw-r--r--   0        0        0    15799 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/project.py
+-rw-r--r--   0        0        0     6129 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/task.py
+-rw-r--r--   0        0        0     8882 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/task_collection.py
+-rw-r--r--   0        0        0    10942 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/workflow.py
+-rw-r--r--   0        0        0     5582 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v1/workflowtask.py
+-rw-r--r--   0        0        0     1487 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/__init__.py
+-rw-r--r--   0        0        0    14301 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/_aux_functions.py
+-rw-r--r--   0        0        0     8248 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/dataset.py
+-rw-r--r--   0        0        0     7894 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/images.py
+-rw-r--r--   0        0        0     5325 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/job.py
+-rw-r--r--   0        0        0     5594 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/project.py
+-rw-r--r--   0        0        0     6394 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/status.py
+-rw-r--r--   0        0        0     6940 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/submit.py
+-rw-r--r--   0        0        0     7130 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/task.py
+-rw-r--r--   0        0        0     8988 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/task_collection.py
+-rw-r--r--   0        0        0     1628 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/task_legacy.py
+-rw-r--r--   0        0        0    11863 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/workflow.py
+-rw-r--r--   0        0        0     8802 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/api/v2/workflowtask.py
+-rw-r--r--   0        0        0     4885 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/auth.py
+-rw-r--r--   0        0        0        0 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/aux/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/aux/_job.py
+-rw-r--r--   0        0        0      675 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/routes/aux/_runner.py
+-rw-r--r--   0        0        0       16 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0        0 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0      829 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/async_wrap.py
+-rw-r--r--   0        0        0      119 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/components.py
+-rw-r--r--   0        0        0     4159 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/__init__.py
+-rw-r--r--   0        0        0     8841 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_batching.py
+-rw-r--r--   0        0        0     1908 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
+-rw-r--r--   0        0        0     4421 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    15552 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_slurm_config.py
+-rw-r--r--   0        0        0     5123 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    44655 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/executor.py
+-rw-r--r--   0        0        0     5852 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/remote.py
+-rw-r--r--   0        0        0      206 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/filenames.py
+-rw-r--r--   0        0        0     1254 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/set_start_and_last_task_index.py
+-rw-r--r--   0        0        0     3180 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/task_files.py
+-rw-r--r--   0        0        0    13620 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/v1/__init__.py
+-rw-r--r--   0        0        0    21246 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/v1/_common.py
+-rw-r--r--   0        0        0     6839 2024-05-06 12:52:10.662958 fractal_server-2.0.4/fractal_server/app/runner/v1/_local/__init__.py
+-rw-r--r--   0        0        0     3147 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/_local/_local_config.py
+-rw-r--r--   0        0        0     1493 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/_local/executor.py
+-rw-r--r--   0        0        0    10853 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/_slurm/__init__.py
+-rw-r--r--   0        0        0     2738 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     5977 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0     3294 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/common.py
+-rw-r--r--   0        0        0     4684 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v1/handle_failed_job.py
+-rw-r--r--   0        0        0    12500 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/__init__.py
+-rw-r--r--   0        0        0     5881 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_local/__init__.py
+-rw-r--r--   0        0        0     3630 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_local/_local_config.py
+-rw-r--r--   0        0        0     1614 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_local/executor.py
+-rw-r--r--   0        0        0     4409 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_slurm/__init__.py
+-rw-r--r--   0        0        0     2793 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     6726 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0      639 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/deduplicate_list.py
+-rw-r--r--   0        0        0     5415 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/handle_failed_job.py
+-rw-r--r--   0        0        0     1281 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/merge_outputs.py
+-rw-r--r--   0        0        0    14160 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/runner.py
+-rw-r--r--   0        0        0    11067 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/runner_functions.py
+-rw-r--r--   0        0        0     3710 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/runner_functions_low_level.py
+-rw-r--r--   0        0        0     1866 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/task_interface.py
+-rw-r--r--   0        0        0      912 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/runner/v2/v1_compat.py
+-rw-r--r--   0        0        0       40 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/__init__.py
+-rw-r--r--   0        0        0     3461 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/_validators.py
+-rw-r--r--   0        0        0      692 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/state.py
+-rw-r--r--   0        0        0     3113 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/user.py
+-rw-r--r--   0        0        0     1809 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/__init__.py
+-rw-r--r--   0        0        0     4302 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/applyworkflow.py
+-rw-r--r--   0        0        0     3444 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/dataset.py
+-rw-r--r--   0        0        0     1274 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/dumps.py
+-rw-r--r--   0        0        0     3829 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/manifest.py
+-rw-r--r--   0        0        0     1218 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/project.py
+-rw-r--r--   0        0        0     3704 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/task.py
+-rw-r--r--   0        0        0     3057 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/task_collection.py
+-rw-r--r--   0        0        0     4618 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v1/workflow.py
+-rw-r--r--   0        0        0     1852 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/__init__.py
+-rw-r--r--   0        0        0     2599 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/dataset.py
+-rw-r--r--   0        0        0     2063 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/dumps.py
+-rw-r--r--   0        0        0     3250 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/job.py
+-rw-r--r--   0        0        0     6243 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/manifest.py
+-rw-r--r--   0        0        0      736 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/project.py
+-rw-r--r--   0        0        0      332 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/status.py
+-rw-r--r--   0        0        0     4672 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/task.py
+-rw-r--r--   0        0        0     3171 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/task_collection.py
+-rw-r--r--   0        0        0     1827 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/workflow.py
+-rw-r--r--   0        0        0     6552 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/schemas/v2/workflowtask.py
+-rw-r--r--   0        0        0    11203 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0    15048 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/config.py
+-rw-r--r--   0        0        0     2918 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/data_migrations/2_0_3.py
+-rw-r--r--   0        0        0      398 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/data_migrations/README.md
+-rw-r--r--   0        0        0      196 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/images/__init__.py
+-rw-r--r--   0        0        0     4167 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/images/models.py
+-rw-r--r--   0        0        0     2209 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/images/tools.py
+-rw-r--r--   0        0        0     4178 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/logger.py
+-rw-r--r--   0        0        0     3381 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2630 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      526 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     1157 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
+-rw-r--r--   0        0        0     8770 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0     8433 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/5bf02391cfef_v2.py
+-rw-r--r--   0        0        0     1632 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
+-rw-r--r--   0        0        0     1353 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
+-rw-r--r--   0        0        0     2684 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
+-rw-r--r--   0        0        0     1115 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
+-rw-r--r--   0        0        0     1057 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
+-rw-r--r--   0        0        0      883 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
+-rw-r--r--   0        0        0     1849 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
+-rw-r--r--   0        0        0      867 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
+-rw-r--r--   0        0        0      949 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
+-rw-r--r--   0        0        0      963 2024-05-06 12:52:10.666958 fractal_server-2.0.4/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
+-rw-r--r--   0        0        0     1221 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
+-rw-r--r--   0        0        0      746 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/syringe.py
+-rw-r--r--   0        0        0       23 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0     5379 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/endpoint_operations.py
+-rw-r--r--   0        0        0     3278 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/utils.py
+-rw-r--r--   0        0        0     3775 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v1/_TaskCollectPip.py
+-rw-r--r--   0        0        0        0 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v1/__init__.py
+-rw-r--r--   0        0        0    11731 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v1/background_operations.py
+-rw-r--r--   0        0        0      502 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v1/get_collection_data.py
+-rw-r--r--   0        0        0     3775 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v2/_TaskCollectPip.py
+-rw-r--r--   0        0        0        0 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v2/__init__.py
+-rw-r--r--   0        0        0    12922 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v2/background_operations.py
+-rw-r--r--   0        0        0      502 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/tasks/v2/get_collection_data.py
+-rw-r--r--   0        0        0      448 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/urls.py
+-rw-r--r--   0        0        0     2115 2024-05-06 12:52:10.670958 fractal_server-2.0.4/fractal_server/utils.py
+-rw-r--r--   0        0        0     3052 2024-05-06 12:52:10.670958 fractal_server-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4222 1970-01-01 00:00:00.000000 fractal_server-2.0.4/PKG-INFO
```

### Comparing `fractal_server-2.0.3/LICENSE` & `fractal_server-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/README.md` & `fractal_server-2.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Fractal Server
 
 [![PyPI version](https://img.shields.io/pypi/v/fractal-server?color=gree)](https://pypi.org/project/fractal-server/)
-[![CI Status](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml)
+[![CI Status](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml?query=branch%3Amain)
 [![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-server/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-server/blob/python-coverage-comment-action-data/htmlcov/index.html)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Benchmarks](https://img.shields.io/badge/Benchmarks-Done-blue)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-server/blob/benchmark-api/benchmarks/bench.html)
 
 Fractal is a framework to process high content imaging data at scale and
 prepare it for interactive visualization.
```

### Comparing `fractal_server-2.0.3/fractal_server/__main__.py` & `fractal_server-2.0.4/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/alembic.ini` & `fractal_server-2.0.4/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/db/__init__.py` & `fractal_server-2.0.4/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/linkuserproject.py` & `fractal_server-2.0.4/fractal_server/app/models/linkuserproject.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/security.py` & `fractal_server-2.0.4/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/v1/dataset.py` & `fractal_server-2.0.4/fractal_server/app/models/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/v1/job.py` & `fractal_server-2.0.4/fractal_server/app/models/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/v1/project.py` & `fractal_server-2.0.4/fractal_server/app/models/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/v1/state.py` & `fractal_server-2.0.4/fractal_server/app/models/v1/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/v1/task.py` & `fractal_server-2.0.4/fractal_server/app/models/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/v1/workflow.py` & `fractal_server-2.0.4/fractal_server/app/models/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/v2/collection_state.py` & `fractal_server-2.0.4/fractal_server/app/models/v2/collection_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/v2/dataset.py` & `fractal_server-2.0.4/fractal_server/app/models/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/v2/job.py` & `fractal_server-2.0.4/fractal_server/app/models/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/v2/project.py` & `fractal_server-2.0.4/fractal_server/app/models/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/v2/task.py` & `fractal_server-2.0.4/fractal_server/app/models/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/v2/workflow.py` & `fractal_server-2.0.4/fractal_server/app/models/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/models/v2/workflowtask.py` & `fractal_server-2.0.4/fractal_server/app/models/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/admin/v1.py` & `fractal_server-2.0.4/fractal_server/app/routes/admin/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/admin/v2.py` & `fractal_server-2.0.4/fractal_server/app/routes/admin/v2.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v1/__init__.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v1/_aux_functions.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v1/dataset.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v1/job.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v1/project.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v1/task.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v1/task_collection.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v1/workflow.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v1/workflowtask.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v1/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v2/__init__.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v2/_aux_functions.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v2/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v2/dataset.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v2/images.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v2/images.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v2/job.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v2/project.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v2/status.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v2/status.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v2/submit.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v2/submit.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v2/task.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v2/task_collection.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v2/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v2/task_legacy.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v2/task_legacy.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v2/workflow.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/api/v2/workflowtask.py` & `fractal_server-2.0.4/fractal_server/app/routes/api/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/auth.py` & `fractal_server-2.0.4/fractal_server/app/routes/auth.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/aux/_job.py` & `fractal_server-2.0.4/fractal_server/app/routes/aux/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/routes/aux/_runner.py` & `fractal_server-2.0.4/fractal_server/app/routes/aux/_runner.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/async_wrap.py` & `fractal_server-2.0.4/fractal_server/app/runner/async_wrap.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/exceptions.py` & `fractal_server-2.0.4/fractal_server/app/runner/exceptions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/_batching.py` & `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/_check_jobs_status.py` & `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_check_jobs_status.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py` & `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/_slurm_config.py` & `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py` & `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/executor.py` & `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -485,14 +485,18 @@
         for ind_chunk in range(0, tot_tasks, batch_size):
             args_batches.append(
                 list_args[ind_chunk : ind_chunk + batch_size]  # noqa
             )
         if len(args_batches) != math.ceil(tot_tasks / tasks_per_job):
             raise RuntimeError("Something wrong here while batching tasks")
 
+        # Fetch configuration variable
+        settings = Inject(get_settings)
+        FRACTAL_SLURM_SBATCH_SLEEP = settings.FRACTAL_SLURM_SBATCH_SLEEP
+
         # Construct list of futures (one per SLURM job, i.e. one per batch)
         fs = []
         current_component_index = 0
         for ind_batch, batch in enumerate(args_batches):
             batch_size = len(batch)
             this_slurm_file_prefix = (
                 f"{general_slurm_file_prefix}_batch_{ind_batch:06d}"
@@ -504,14 +508,15 @@
                     slurm_file_prefix=this_slurm_file_prefix,
                     task_files=task_files,
                     single_task_submission=False,
                     components=batch,
                 )
             )
             current_component_index += batch_size
+            time.sleep(FRACTAL_SLURM_SBATCH_SLEEP)
 
         # Yield must be hidden in closure so that the futures are submitted
         # before the first iterator value is required.
         # NOTE: In this custom map() method, _result_or_cancel(fs.pop()) is an
         # iterable of results (if successful), and we should yield its elements
         # rather than the whole iterable.
         def result_iterator():
```

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/executors/slurm/remote.py` & `fractal_server-2.0.4/fractal_server/app/runner/executors/slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/set_start_and_last_task_index.py` & `fractal_server-2.0.4/fractal_server/app/runner/set_start_and_last_task_index.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/task_files.py` & `fractal_server-2.0.4/fractal_server/app/runner/task_files.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v1/__init__.py` & `fractal_server-2.0.4/fractal_server/app/runner/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v1/_common.py` & `fractal_server-2.0.4/fractal_server/app/runner/v1/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v1/_local/__init__.py` & `fractal_server-2.0.4/fractal_server/app/runner/v1/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v1/_local/_local_config.py` & `fractal_server-2.0.4/fractal_server/app/runner/v1/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v1/_local/_submit_setup.py` & `fractal_server-2.0.4/fractal_server/app/runner/v1/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v1/_local/executor.py` & `fractal_server-2.0.4/fractal_server/app/runner/v1/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v1/_slurm/__init__.py` & `fractal_server-2.0.4/fractal_server/app/runner/v1/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v1/_slurm/_submit_setup.py` & `fractal_server-2.0.4/fractal_server/app/runner/v1/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v1/_slurm/get_slurm_config.py` & `fractal_server-2.0.4/fractal_server/app/runner/v1/_slurm/get_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v1/common.py` & `fractal_server-2.0.4/fractal_server/app/runner/v1/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v1/handle_failed_job.py` & `fractal_server-2.0.4/fractal_server/app/runner/v1/handle_failed_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/__init__.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/_local/__init__.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/_local/_local_config.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/_local/_submit_setup.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/_local/executor.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/_slurm/__init__.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/_slurm/_submit_setup.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/_slurm/get_slurm_config.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/_slurm/get_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/deduplicate_list.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/deduplicate_list.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/handle_failed_job.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/handle_failed_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/merge_outputs.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/merge_outputs.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/runner.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/runner.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/runner_functions.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/runner_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/runner_functions_low_level.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/runner_functions_low_level.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/task_interface.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/task_interface.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/runner/v2/v1_compat.py` & `fractal_server-2.0.4/fractal_server/app/runner/v2/v1_compat.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/_validators.py` & `fractal_server-2.0.4/fractal_server/app/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/state.py` & `fractal_server-2.0.4/fractal_server/app/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/user.py` & `fractal_server-2.0.4/fractal_server/app/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v1/__init__.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v1/applyworkflow.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v1/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v1/dataset.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v1/dumps.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v1/dumps.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v1/manifest.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v1/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v1/project.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v1/task.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v1/task_collection.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v1/workflow.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v2/__init__.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v2/dataset.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v2/dumps.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v2/dumps.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v2/job.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v2/manifest.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v2/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v2/project.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v2/task.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v2/task_collection.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v2/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v2/workflow.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/schemas/v2/workflowtask.py` & `fractal_server-2.0.4/fractal_server/app/schemas/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/app/security/__init__.py` & `fractal_server-2.0.4/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/config.py` & `fractal_server-2.0.4/fractal_server/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,14 +327,20 @@
     FRACTAL_SLURM_POLL_INTERVAL: int = 5
     """
     Interval to wait (in seconds) before checking whether unfinished job are
     still running on SLURM (see `SlurmWaitThread` in
     [`clusterfutures`](https://github.com/sampsyo/clusterfutures/blob/master/cfut/__init__.py)).
     """
 
+    FRACTAL_SLURM_SBATCH_SLEEP: int = 0
+    """
+    Interval to wait (in seconds) between two subsequent `sbatch` calls, when
+    running a task that produces multiple SLURM jobs.
+    """
+
     FRACTAL_SLURM_ERROR_HANDLING_INTERVAL: int = 5
     """
     Interval to wait (in seconds) when the SLURM backend does not find an
     output pickle file - which could be due to several reasons (e.g. the SLURM
     job was cancelled or failed, or writing the file is taking long). If the
     file is still missing after this time interval, this leads to a
     `JobExecutionError`.
```

### Comparing `fractal_server-2.0.3/fractal_server/data_migrations/2_0_3.py` & `fractal_server-2.0.4/fractal_server/data_migrations/2_0_3.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/images/models.py` & `fractal_server-2.0.4/fractal_server/images/models.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/images/tools.py` & `fractal_server-2.0.4/fractal_server/images/tools.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/logger.py` & `fractal_server-2.0.4/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/main.py` & `fractal_server-2.0.4/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/env.py` & `fractal_server-2.0.4/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/script.py.mako` & `fractal_server-2.0.4/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/5bf02391cfef_v2.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/5bf02391cfef_v2.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-2.0.4/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/syringe.py` & `fractal_server-2.0.4/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/tasks/endpoint_operations.py` & `fractal_server-2.0.4/fractal_server/tasks/endpoint_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/tasks/utils.py` & `fractal_server-2.0.4/fractal_server/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/tasks/v1/_TaskCollectPip.py` & `fractal_server-2.0.4/fractal_server/tasks/v1/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/tasks/v1/background_operations.py` & `fractal_server-2.0.4/fractal_server/tasks/v1/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/tasks/v2/_TaskCollectPip.py` & `fractal_server-2.0.4/fractal_server/tasks/v2/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/tasks/v2/background_operations.py` & `fractal_server-2.0.4/fractal_server/tasks/v2/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/fractal_server/utils.py` & `fractal_server-2.0.4/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.3/pyproject.toml` & `fractal_server-2.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "2.0.3"
+version = "2.0.4"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Yuri Chiucconi <yuri.chiucconi@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
@@ -83,15 +83,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "2.0.3"
+current_version = "2.0.4"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-2.0.3/PKG-INFO` & `fractal_server-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 2.0.3
+Version: 2.0.4
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Tommaso Comparin
 Author-email: tommaso.comparin@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -35,15 +35,15 @@
 Project-URL: Documentation, https://fractal-analytics-platform.github.io/fractal-server
 Project-URL: Repository, https://github.com/fractal-analytics-platform/fractal-server
 Description-Content-Type: text/markdown
 
 # Fractal Server
 
 [![PyPI version](https://img.shields.io/pypi/v/fractal-server?color=gree)](https://pypi.org/project/fractal-server/)
-[![CI Status](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml)
+[![CI Status](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml?query=branch%3Amain)
 [![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-server/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-server/blob/python-coverage-comment-action-data/htmlcov/index.html)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Benchmarks](https://img.shields.io/badge/Benchmarks-Done-blue)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-server/blob/benchmark-api/benchmarks/bench.html)
 
 Fractal is a framework to process high content imaging data at scale and
 prepare it for interactive visualization.
```

