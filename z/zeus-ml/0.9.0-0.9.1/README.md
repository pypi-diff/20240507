# Comparing `tmp/zeus_ml-0.9.0.tar.gz` & `tmp/zeus_ml-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeus_ml-0.9.0.tar", last modified: Mon May  6 15:51:24 2024, max compression
+gzip compressed data, was "zeus_ml-0.9.1.tar", last modified: Tue May  7 04:06:42 2024, max compression
```

## Comparing `zeus_ml-0.9.0.tar` & `zeus_ml-0.9.1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.052604 zeus_ml-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 15:51:18.000000 zeus_ml-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-06 15:51:24.052604 zeus_ml-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-05-06 15:51:18.000000 zeus_ml-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/capriccio/
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-06 15:51:18.000000 zeus_ml-0.9.0/capriccio/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-06 15:51:18.000000 zeus_ml-0.9.0/docs/gen_ref_pages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.024604 zeus_ml-0.9.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.024604 zeus_ml-0.9.0/examples/batch_size_optimizer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/examples/batch_size_optimizer/capriccio/
--rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/batch_size_optimizer/capriccio/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/examples/batch_size_optimizer/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/batch_size_optimizer/mnist/train_dp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/batch_size_optimizer/mnist/train_single_gpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/examples/huggingface/
--rw-r--r--   0 runner    (1001) docker     (127)    30412 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/huggingface/run_clm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/huggingface/run_gemma_sft_qlora.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/examples/pipeline_frequency_optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/pipeline_frequency_optimizer/profile_p2p.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/pipeline_frequency_optimizer/run_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.028604 zeus_ml-0.9.0/examples/power_limit_optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)    12553 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/power_limit_optimizer/train_dp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/power_limit_optimizer/train_single.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.024604 zeus_ml-0.9.0/examples/research_reproducibility/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/examples/research_reproducibility/zeus_nsdi23/
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/research_reproducibility/zeus_nsdi23/run_alibaba.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/examples/research_reproducibility/zeus_nsdi23/run_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:51:24.052604 zeus_ml-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/tests/optimizer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/tests/optimizer/batch_size/
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/batch_size/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    20383 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/batch_size/simulate_with_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/batch_size/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/batch_size/test_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/batch_size/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/batch_size/test_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/optimizer/test_power_limit_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17477 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/test_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/tests/utils/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/zeus/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.032604 zeus_ml-0.9.0/zeus/_legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.036605 zeus_ml-0.9.0/zeus/_legacy/policy/
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/policy/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/policy/mab.py
--rw-r--r--   0 runner    (1001) docker     (127)    19971 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/policy/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    36929 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/_legacy/simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.036605 zeus_ml-0.9.0/zeus/device/
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/device/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    37348 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.036605 zeus_ml-0.9.0/zeus/monitor/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/monitor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/monitor/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/monitor/power.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.036605 zeus_ml-0.9.0/zeus/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.036605 zeus_ml-0.9.0/zeus/optimizer/batch_size/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.036605 zeus_ml-0.9.0/zeus/optimizer/batch_size/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.040604 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.040604 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/batch_size_state/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/batch_size_state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/batch_size_state/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/batch_size_state/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/batch_size_state/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.040604 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/database/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/database/db_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/database/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/database/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.040604 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/job/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/job/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/job/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/job/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    11140 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/mab.py
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.040604 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/services/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/services/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    14176 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/batch_size/server/services/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.044604 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11589 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/frequency_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.044604 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/job_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    22745 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/optimizer/power_limit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.044604 zeus_ml-0.9.0/zeus/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/lr_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/pydantic_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-05-06 15:51:19.000000 zeus_ml-0.9.0/zeus/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:51:24.044604 zeus_ml-0.9.0/zeus_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-06 15:51:24.000000 zeus_ml-0.9.0/zeus_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-06 15:51:24.000000 zeus_ml-0.9.0/zeus_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:51:24.000000 zeus_ml-0.9.0/zeus_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-06 15:51:24.000000 zeus_ml-0.9.0/zeus_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-06 15:51:24.000000 zeus_ml-0.9.0/zeus_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.174548 zeus_ml-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-05-07 04:06:42.174548 zeus_ml-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.154549 zeus_ml-0.9.1/capriccio/
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/capriccio/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.154549 zeus_ml-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/docs/gen_ref_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.150549 zeus_ml-0.9.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.150549 zeus_ml-0.9.1/examples/batch_size_optimizer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.154549 zeus_ml-0.9.1/examples/batch_size_optimizer/capriccio/
+-rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/examples/batch_size_optimizer/capriccio/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.154549 zeus_ml-0.9.1/examples/batch_size_optimizer/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/examples/batch_size_optimizer/mnist/train_dp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/examples/batch_size_optimizer/mnist/train_single_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.154549 zeus_ml-0.9.1/examples/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (127)    30412 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/examples/huggingface/run_clm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/examples/huggingface/run_gemma_sft_qlora.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.154549 zeus_ml-0.9.1/examples/pipeline_frequency_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/examples/pipeline_frequency_optimizer/profile_p2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/examples/pipeline_frequency_optimizer/run_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.154549 zeus_ml-0.9.1/examples/power_limit_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)    12553 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/examples/power_limit_optimizer/train_dp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/examples/power_limit_optimizer/train_single.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.150549 zeus_ml-0.9.1/examples/research_reproducibility/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.154549 zeus_ml-0.9.1/examples/research_reproducibility/zeus_nsdi23/
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/examples/research_reproducibility/zeus_nsdi23/run_alibaba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/examples/research_reproducibility/zeus_nsdi23/run_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 04:06:42.174548 zeus_ml-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.154549 zeus_ml-0.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.158548 zeus_ml-0.9.1/tests/optimizer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.158548 zeus_ml-0.9.1/tests/optimizer/batch_size/
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/tests/optimizer/batch_size/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20383 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/tests/optimizer/batch_size/simulate_with_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/tests/optimizer/batch_size/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/tests/optimizer/batch_size/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/tests/optimizer/batch_size/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/tests/optimizer/batch_size/test_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/tests/optimizer/test_power_limit_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17477 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/tests/test_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.158548 zeus_ml-0.9.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/tests/utils/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.158548 zeus_ml-0.9.1/zeus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.158548 zeus_ml-0.9.1/zeus/_legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/_legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/_legacy/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.158548 zeus_ml-0.9.1/zeus/_legacy/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/_legacy/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/_legacy/policy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/_legacy/policy/mab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19971 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/_legacy/policy/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36929 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/_legacy/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.158548 zeus_ml-0.9.1/zeus/device/
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/device/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37607 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.162549 zeus_ml-0.9.1/zeus/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/monitor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/monitor/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/monitor/power.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.162549 zeus_ml-0.9.1/zeus/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.162549 zeus_ml-0.9.1/zeus/optimizer/batch_size/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.162549 zeus_ml-0.9.1/zeus/optimizer/batch_size/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.162549 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.162549 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/batch_size_state/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/batch_size_state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/batch_size_state/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/batch_size_state/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/batch_size_state/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.166549 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/database/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/database/db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/database/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/database/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.166549 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/job/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/job/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/job/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/job/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11140 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/mab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.166549 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/services/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14176 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/batch_size/server/services/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.166549 zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11589 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/frequency_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.166549 zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/server/job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/server/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/server/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22745 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/optimizer/power_limit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.170549 zeus_ml-0.9.1/zeus/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/utils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/utils/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/utils/lr_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/utils/pydantic_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-05-07 04:06:36.000000 zeus_ml-0.9.1/zeus/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:06:42.170549 zeus_ml-0.9.1/zeus_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-05-07 04:06:42.000000 zeus_ml-0.9.1/zeus_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-07 04:06:42.000000 zeus_ml-0.9.1/zeus_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 04:06:42.000000 zeus_ml-0.9.1/zeus_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-07 04:06:42.000000 zeus_ml-0.9.1/zeus_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 04:06:42.000000 zeus_ml-0.9.1/zeus_ml.egg-info/top_level.txt
```

### Comparing `zeus_ml-0.9.0/LICENSE` & `zeus_ml-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/PKG-INFO` & `zeus_ml-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeus-ml
-Version: 0.9.0
+Version: 0.9.1
 Summary: A framework for deep learning energy measurement and optimization.
 Author-email: Jae-Won Chung <jwnchung@umich.edu>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ml-energy/zeus
 Project-URL: Homepage, https://ml.energy/zeus
 Project-URL: Documentation, https://ml.energy/zeus
 Keywords: deep-learning,power,energy,sustainability,mlsys
@@ -75,15 +75,15 @@
 Requires-Dist: zeus-ml[bso,bso-server,lint,migration,pfo-server,test]; extra == "dev"
 Requires-Dist: greenlet; extra == "dev"
 
 <div align="center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ml-energy/zeus/master/docs/assets/img/logo_dark.svg">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ml-energy/zeus/master/docs/assets/img/logo_light.svg">
-  <img alt="Zeus logo" width="55%" src="https://raw.githubusercontent.com/ml-energy/zeus/master/docs/assets/img/logo_dark.svg">
+  <img alt="Zeus logo" width="55%" src="https://raw.githubusercontent.com/ml-energy/zeus/master/docs/assets/img/logo_light.svg">
 </picture>
 <h1>Deep Learning Energy Measurement and Optimization</h1>
 
 [![Slack workspace](https://badgen.net/badge/icon/Join%20workspace/b31b1b?icon=slack&label=Slack)](https://join.slack.com/t/zeus-ml/shared_invite/zt-1najba5mb-WExy7zoNTyaZZfTlUWoLLg)
 [![Docker Hub](https://badgen.net/docker/pulls/symbioticlab/zeus?icon=docker&label=Docker%20pulls)](https://hub.docker.com/r/symbioticlab/zeus)
 [![Homepage](https://custom-icon-badges.demolab.com/badge/Homepage-ml.energy-23d175.svg?logo=home&logoColor=white&logoSource=feather)](https://ml.energy/zeus)
 [![Apache-2.0 License](https://custom-icon-badges.herokuapp.com/github/license/ml-energy/zeus?logo=law)](/LICENSE)
```

### Comparing `zeus_ml-0.9.0/README.md` & `zeus_ml-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <div align="center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ml-energy/zeus/master/docs/assets/img/logo_dark.svg">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ml-energy/zeus/master/docs/assets/img/logo_light.svg">
-  <img alt="Zeus logo" width="55%" src="https://raw.githubusercontent.com/ml-energy/zeus/master/docs/assets/img/logo_dark.svg">
+  <img alt="Zeus logo" width="55%" src="https://raw.githubusercontent.com/ml-energy/zeus/master/docs/assets/img/logo_light.svg">
 </picture>
 <h1>Deep Learning Energy Measurement and Optimization</h1>
 
 [![Slack workspace](https://badgen.net/badge/icon/Join%20workspace/b31b1b?icon=slack&label=Slack)](https://join.slack.com/t/zeus-ml/shared_invite/zt-1najba5mb-WExy7zoNTyaZZfTlUWoLLg)
 [![Docker Hub](https://badgen.net/docker/pulls/symbioticlab/zeus?icon=docker&label=Docker%20pulls)](https://hub.docker.com/r/symbioticlab/zeus)
 [![Homepage](https://custom-icon-badges.demolab.com/badge/Homepage-ml.energy-23d175.svg?logo=home&logoColor=white&logoSource=feather)](https://ml.energy/zeus)
 [![Apache-2.0 License](https://custom-icon-badges.herokuapp.com/github/license/ml-energy/zeus?logo=law)](/LICENSE)
```

### Comparing `zeus_ml-0.9.0/capriccio/generate.py` & `zeus_ml-0.9.1/capriccio/generate.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/docs/gen_ref_pages.py` & `zeus_ml-0.9.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/examples/batch_size_optimizer/capriccio/train.py` & `zeus_ml-0.9.1/examples/batch_size_optimizer/capriccio/train.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/examples/batch_size_optimizer/mnist/train_dp.py` & `zeus_ml-0.9.1/examples/batch_size_optimizer/mnist/train_dp.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/examples/batch_size_optimizer/mnist/train_single_gpu.py` & `zeus_ml-0.9.1/examples/batch_size_optimizer/mnist/train_single_gpu.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/examples/huggingface/run_clm.py` & `zeus_ml-0.9.1/examples/huggingface/run_clm.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/examples/huggingface/run_gemma_sft_qlora.py` & `zeus_ml-0.9.1/examples/huggingface/run_gemma_sft_qlora.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/examples/pipeline_frequency_optimizer/profile_p2p.py` & `zeus_ml-0.9.1/examples/pipeline_frequency_optimizer/profile_p2p.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/examples/pipeline_frequency_optimizer/run_optimization.py` & `zeus_ml-0.9.1/examples/pipeline_frequency_optimizer/run_optimization.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/examples/power_limit_optimizer/train_dp.py` & `zeus_ml-0.9.1/examples/power_limit_optimizer/train_dp.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/examples/power_limit_optimizer/train_single.py` & `zeus_ml-0.9.1/examples/power_limit_optimizer/train_single.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/examples/research_reproducibility/zeus_nsdi23/run_alibaba.py` & `zeus_ml-0.9.1/examples/research_reproducibility/zeus_nsdi23/run_alibaba.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/examples/research_reproducibility/zeus_nsdi23/run_single.py` & `zeus_ml-0.9.1/examples/research_reproducibility/zeus_nsdi23/run_single.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/pyproject.toml` & `zeus_ml-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/tests/optimizer/batch_size/conftest.py` & `zeus_ml-0.9.1/tests/optimizer/batch_size/conftest.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/tests/optimizer/batch_size/simulate_with_server.py` & `zeus_ml-0.9.1/tests/optimizer/batch_size/simulate_with_server.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/tests/optimizer/batch_size/test_client.py` & `zeus_ml-0.9.1/tests/optimizer/batch_size/test_client.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/tests/optimizer/batch_size/test_explorer.py` & `zeus_ml-0.9.1/tests/optimizer/batch_size/test_explorer.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/tests/optimizer/batch_size/test_server.py` & `zeus_ml-0.9.1/tests/optimizer/batch_size/test_server.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/tests/optimizer/batch_size/test_simulator.py` & `zeus_ml-0.9.1/tests/optimizer/batch_size/test_simulator.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/tests/optimizer/test_power_limit_optimizer.py` & `zeus_ml-0.9.1/tests/optimizer/test_power_limit_optimizer.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/tests/test_monitor.py` & `zeus_ml-0.9.1/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/tests/utils/test_env.py` & `zeus_ml-0.9.1/tests/utils/test_env.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/__init__.py` & `zeus_ml-0.9.1/zeus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 - [`monitor`][zeus.monitor]: Programmatic power and energy measurement tools
 - [`utils`][zeus.utils]: Utility functions and classes.
 - [`_legacy`][zeus._legacy.policy]: Legacy code mostly to keep our papers reproducible
 - [`device`][zeus.device]: Abstraction layer over compute devices
 - [`callback`][zeus.callback]: Callback definition
 """
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
```

### Comparing `zeus_ml-0.9.0/zeus/_legacy/job.py` & `zeus_ml-0.9.1/zeus/_legacy/job.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/_legacy/policy/__init__.py` & `zeus_ml-0.9.1/zeus/_legacy/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/_legacy/policy/interface.py` & `zeus_ml-0.9.1/zeus/_legacy/policy/interface.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/_legacy/policy/mab.py` & `zeus_ml-0.9.1/zeus/_legacy/policy/mab.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/_legacy/policy/optimizer.py` & `zeus_ml-0.9.1/zeus/_legacy/policy/optimizer.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/_legacy/simulate.py` & `zeus_ml-0.9.1/zeus/_legacy/simulate.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/callback.py` & `zeus_ml-0.9.1/zeus/callback.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/device/__init__.py` & `zeus_ml-0.9.1/zeus/device/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/device/gpu.py` & `zeus_ml-0.9.1/zeus/device/gpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,16 +264,16 @@
 
     @abc.abstractmethod
     def resetGpuLockedClocks(self) -> None:
         """Reset the GPU locked clocks to default values."""
         pass
 
     @abc.abstractmethod
-    def getPowerUsage(self) -> int:
-        """Return the current power usage of the GPU. Units: mW."""
+    def getInstantPowerUsage(self) -> int:
+        """Returns the current power usage of the GPU. Units: mW."""
         pass
 
     @abc.abstractmethod
     def supportsGetTotalEnergyConsumption(self) -> bool:
         """Check if the GPU supports retrieving total energy consumption."""
         pass
 
@@ -407,17 +407,22 @@
 
     @_handle_nvml_errors
     def resetGpuLockedClocks(self) -> None:
         """Resets the GPU locked clocks of the specified GPU to their default values."""
         pynvml.nvmlDeviceResetGpuLockedClocks(self.handle)
 
     @_handle_nvml_errors
-    def getPowerUsage(self) -> int:
-        """Returns the power usage of the specified GPU. Units: mW."""
-        return pynvml.nvmlDeviceGetPowerUsage(self.handle)
+    def getInstantPowerUsage(self) -> int:
+        """Returns the current power usage of the specified GPU. Units: mW."""
+        metric = pynvml.nvmlDeviceGetFieldValues(
+            self.handle, [pynvml.NVML_FI_DEV_POWER_INSTANT]
+        )[0]
+        if (ret := metric.nvmlReturn) != pynvml.NVML_SUCCESS:
+            raise pynvml.NVMLError(ret)
+        return metric.value.siVal
 
     @_handle_nvml_errors
     def supportsGetTotalEnergyConsumption(self) -> bool:
         """Returns True if the specified GPU supports retrieving the total energy consumption."""
         # NVIDIA GPUs Volta or newer support this method
         if self._supportsGetTotalEnergyConsumption is None:
             self._supportsGetTotalEnergyConsumption = (
@@ -598,19 +603,20 @@
             self.handle,
             info["min_clk"],
             info["max_clk"],
             clk_type=amdsmi.AmdSmiClkType.GFX,
         )  # expects MHz
 
     @_handle_amdsmi_errors
-    def getPowerUsage(self) -> int:
-        """Returns the power usage of the specified GPU. Units: mW."""
+    def getInstantPowerUsage(self) -> int:
+        """Returns the current power usage of the specified GPU. Units: mW."""
+        # returns in W, convert to mW
         return int(
             amdsmi.amdsmi_get_power_info(self.handle)["average_socket_power"] * 1000
-        )  # returns in W, convert to mW
+        )
 
     @_handle_amdsmi_errors
     def supportsGetTotalEnergyConsumption(self) -> bool:
         """Returns True if the specified GPU supports retrieving the total energy consumption."""
         if self._supportsGetTotalEnergyConsumption is None:
             try:
                 _ = amdsmi.amdsmi_get_energy_count(self.handle)
@@ -719,17 +725,17 @@
         """Resets the memory locked clocks of the specified GPU to their default values."""
         self.gpus[index].resetMemoryLockedClocks()
 
     def resetGpuLockedClocks(self, index: int) -> None:
         """Resets the GPU locked clocks of the specified GPU to their default values."""
         self.gpus[index].resetGpuLockedClocks()
 
-    def getPowerUsage(self, index: int) -> int:
+    def getInstantPowerUsage(self, index: int) -> int:
         """Returns the power usage of the specified GPU. Units: mW."""
-        return self.gpus[index].getPowerUsage()
+        return self.gpus[index].getInstantPowerUsage()
 
     def supportsGetTotalEnergyConsumption(self, index: int) -> bool:
         """Returns True if the specified GPU supports retrieving the total energy consumption."""
         return self.gpus[index].supportsGetTotalEnergyConsumption()
 
     def getTotalEnergyConsumption(self, index: int) -> int:
         """Returns the total energy consumption of the specified GPU. Units: mJ."""
```

### Comparing `zeus_ml-0.9.0/zeus/monitor/__init__.py` & `zeus_ml-0.9.1/zeus/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/monitor/__main__.py` & `zeus_ml-0.9.1/zeus/monitor/__main__.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/monitor/energy.py` & `zeus_ml-0.9.1/zeus/monitor/energy.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,17 @@
             )
         else:
             self.power_monitor = None
 
     def _get_instant_power(self) -> tuple[dict[int, float], float]:
         """Measure the power consumption of all GPUs at the current time."""
         power_measurement_start_time: float = time()
-        power = {i: self.gpus.getPowerUsage(i) / 1000.0 for i in self.gpu_indices}
+        power = {
+            i: self.gpus.getInstantPowerUsage(i) / 1000.0 for i in self.gpu_indices
+        }
         power_measurement_time = time() - power_measurement_start_time
         return power, power_measurement_time
 
     def begin_window(self, key: str, sync_cuda: bool = True) -> None:
         """Begin a new measurement window.
 
         Args:
```

### Comparing `zeus_ml-0.9.0/zeus/monitor/power.py` & `zeus_ml-0.9.1/zeus/monitor/power.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,27 +79,33 @@
     # get gpus
     gpus = get_gpus()
     # Collect 1000 samples of the power counter with timestamps.
     time_power_samples: list[tuple[float, int]] = [(0.0, 0) for _ in range(1000)]
     for i in range(len(time_power_samples)):
         time_power_samples[i] = (
             time(),
-            gpus.getPowerUsage(gpu_index),
+            gpus.getInstantPowerUsage(gpu_index),
         )
 
     # Find the timestamps when the power readings changed.
+    time_power_samples = time_power_samples[10:]
     changed_times = []
     prev_power = time_power_samples[0][1]
     for t, p in time_power_samples:
         if p != prev_power:
             changed_times.append(t)
             prev_power = p
 
     # Compute the minimum time difference between power change timestamps.
-    return min(time2 - time1 for time1, time2 in zip(changed_times, changed_times[1:]))
+    intervals = [
+        time2 - time1 for time1, time2 in zip(changed_times, changed_times[1:])
+    ]
+    if len(intervals) == 0:
+        return 0.1
+    return min(intervals)
 
 
 class PowerMonitor:
     """Monitor power usage from GPUs.
 
     This class acts as a lower level wrapper around a Python process that polls
     the power consumption of GPUs. This is primarily used by
@@ -116,15 +122,16 @@
         self,
         gpu_indices: list[int] | None = None,
         update_period: float | None = None,
     ) -> None:
         """Initialize the power monitor.
 
         Initialization should not be done in global scope due to python's protection.
-        Refer to the "Safe importing of main module" section in https://docs.python.org/3/library/multiprocessing.html for more detail.
+        Refer to the "Safe importing of main module" section in
+        https://docs.python.org/3/library/multiprocessing.html for more details.
 
         Args:
             gpu_indices: Indices of the GPUs to monitor. If None, monitor all GPUs.
             update_period: Update period of the power monitor in seconds. If None,
                 infer the update period by max speed polling the power counter for
                 each GPU model.
         """
@@ -253,14 +260,14 @@
 
         # Use line buffering.
         with open(power_csv, "w", buffering=1) as power_f:
             while True:
                 power: list[float] = []
                 now = time()
                 for index in gpu_indices:
-                    power.append(gpus.getPowerUsage(index))
+                    power.append(gpus.getInstantPowerUsage(index))
                 power_str = ",".join(map(lambda p: str(p / 1000), power))
                 power_f.write(f"{now},{power_str}\n")
                 if (sleep_time := update_period - (time() - now)) > 0:
                     sleep(sleep_time)
     except KeyboardInterrupt:
         return
```

### Comparing `zeus_ml-0.9.0/zeus/optimizer/__init__.py` & `zeus_ml-0.9.1/zeus/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/client.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/client.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/common.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/common.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/exceptions.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/exceptions.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/migrations/env.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/migrations/env.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/__init__.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/batch_size_state/commands.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/batch_size_state/commands.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/batch_size_state/models.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/batch_size_state/models.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/batch_size_state/repository.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/batch_size_state/repository.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/config.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/config.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/database/db_connection.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/database/db_connection.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/database/schema.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/database/schema.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/exceptions.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/exceptions.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/explorer.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/explorer.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/job/commands.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/job/commands.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/job/models.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/job/models.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/job/repository.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/job/repository.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/mab.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/mab.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/optimizer.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/optimizer.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/router.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/router.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/services/commands.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/services/commands.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/batch_size/server/services/service.py` & `zeus_ml-0.9.1/zeus/optimizer/batch_size/server/services/service.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/__init__.py` & `zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/common.py` & `zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/common.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/frequency_controller.py` & `zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/frequency_controller.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/optimizer.py` & `zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/optimizer.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/__init__.py` & `zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/server/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/job_manager.py` & `zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/server/job_manager.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/router.py` & `zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/server/router.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/pipeline_frequency/server/scheduler.py` & `zeus_ml-0.9.1/zeus/optimizer/pipeline_frequency/server/scheduler.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/optimizer/power_limit.py` & `zeus_ml-0.9.1/zeus/optimizer/power_limit.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/utils/__init__.py` & `zeus_ml-0.9.1/zeus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/utils/async_utils.py` & `zeus_ml-0.9.1/zeus/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/utils/env.py` & `zeus_ml-0.9.1/zeus/utils/env.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/utils/framework.py` & `zeus_ml-0.9.1/zeus/utils/framework.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/utils/logging.py` & `zeus_ml-0.9.1/zeus/utils/logging.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/utils/lr_scaler.py` & `zeus_ml-0.9.1/zeus/utils/lr_scaler.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/utils/metric.py` & `zeus_ml-0.9.1/zeus/utils/metric.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/utils/pydantic_v1.py` & `zeus_ml-0.9.1/zeus/utils/pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus/utils/testing.py` & `zeus_ml-0.9.1/zeus/utils/testing.py`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus_ml.egg-info/PKG-INFO` & `zeus_ml-0.9.1/zeus_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeus-ml
-Version: 0.9.0
+Version: 0.9.1
 Summary: A framework for deep learning energy measurement and optimization.
 Author-email: Jae-Won Chung <jwnchung@umich.edu>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ml-energy/zeus
 Project-URL: Homepage, https://ml.energy/zeus
 Project-URL: Documentation, https://ml.energy/zeus
 Keywords: deep-learning,power,energy,sustainability,mlsys
@@ -75,15 +75,15 @@
 Requires-Dist: zeus-ml[bso,bso-server,lint,migration,pfo-server,test]; extra == "dev"
 Requires-Dist: greenlet; extra == "dev"
 
 <div align="center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ml-energy/zeus/master/docs/assets/img/logo_dark.svg">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ml-energy/zeus/master/docs/assets/img/logo_light.svg">
-  <img alt="Zeus logo" width="55%" src="https://raw.githubusercontent.com/ml-energy/zeus/master/docs/assets/img/logo_dark.svg">
+  <img alt="Zeus logo" width="55%" src="https://raw.githubusercontent.com/ml-energy/zeus/master/docs/assets/img/logo_light.svg">
 </picture>
 <h1>Deep Learning Energy Measurement and Optimization</h1>
 
 [![Slack workspace](https://badgen.net/badge/icon/Join%20workspace/b31b1b?icon=slack&label=Slack)](https://join.slack.com/t/zeus-ml/shared_invite/zt-1najba5mb-WExy7zoNTyaZZfTlUWoLLg)
 [![Docker Hub](https://badgen.net/docker/pulls/symbioticlab/zeus?icon=docker&label=Docker%20pulls)](https://hub.docker.com/r/symbioticlab/zeus)
 [![Homepage](https://custom-icon-badges.demolab.com/badge/Homepage-ml.energy-23d175.svg?logo=home&logoColor=white&logoSource=feather)](https://ml.energy/zeus)
 [![Apache-2.0 License](https://custom-icon-badges.herokuapp.com/github/license/ml-energy/zeus?logo=law)](/LICENSE)
```

### Comparing `zeus_ml-0.9.0/zeus_ml.egg-info/SOURCES.txt` & `zeus_ml-0.9.1/zeus_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zeus_ml-0.9.0/zeus_ml.egg-info/requires.txt` & `zeus_ml-0.9.1/zeus_ml.egg-info/requires.txt`

 * *Files identical despite different names*

