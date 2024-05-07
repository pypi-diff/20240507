# Comparing `tmp/remoulade-3.2.0.tar.gz` & `tmp/remoulade-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remoulade-3.2.0.tar", last modified: Wed Jan 24 16:32:46 2024, max compression
+gzip compressed data, was "remoulade-3.2.1.tar", last modified: Tue May  7 14:57:35 2024, max compression
```

## Comparing `remoulade-3.2.0.tar` & `remoulade-3.2.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.077200 remoulade-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-01-24 16:32:33.000000 remoulade-3.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-01-24 16:32:33.000000 remoulade-3.2.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-24 16:32:33.000000 remoulade-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-01-24 16:32:46.077200 remoulade-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-01-24 16:32:33.000000 remoulade-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.053200 remoulade-3.2.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      275 2024-01-24 16:32:33.000000 remoulade-3.2.0/bin/remoulade-gevent
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-24 16:32:33.000000 remoulade-3.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.057200 remoulade-3.2.0/remoulade/
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.057200 remoulade-3.2.0/remoulade/api/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/api/apispec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/api/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/api/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/api/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.057200 remoulade-3.2.0/remoulade/brokers/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/brokers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/brokers/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    21619 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/brokers/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/brokers/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.061200 remoulade-3.2.0/remoulade/cancel/
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/cancel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/cancel/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.061200 remoulade-3.2.0/remoulade/cancel/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/cancel/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/cancel/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/cancel/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/cancel/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/cancel/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.061200 remoulade-3.2.0/remoulade/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/cli/remoulade_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/cli/remoulade_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/cli/remoulade_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/collection_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12155 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.061200 remoulade-3.2.0/remoulade/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/helpers/actor_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/helpers/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/helpers/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/helpers/redis_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/helpers/reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.065200 remoulade-3.2.0/remoulade/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/age_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/catch_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/current_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/logging_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/max_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/max_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/middleware/worker_thread_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.065200 remoulade-3.2.0/remoulade/rate_limits/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/rate_limits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/rate_limits/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.065200 remoulade-3.2.0/remoulade/rate_limits/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/rate_limits/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/rate_limits/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/rate_limits/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/rate_limits/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/rate_limits/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/rate_limits/rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/rate_limits/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.065200 remoulade-3.2.0/remoulade/results/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/results/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.065200 remoulade-3.2.0/remoulade/results/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/results/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/results/backends/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/results/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/results/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/results/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/results/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.065200 remoulade-3.2.0/remoulade/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10477 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.069200 remoulade-3.2.0/remoulade/state/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/state/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.069200 remoulade-3.2.0/remoulade/state/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/state/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/state/backends/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/state/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/state/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/state/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/state/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19505 2024-01-24 16:32:33.000000 remoulade-3.2.0/remoulade/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.073200 remoulade-3.2.0/remoulade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-01-24 16:32:46.000000 remoulade-3.2.0/remoulade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-01-24 16:32:46.000000 remoulade-3.2.0/remoulade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 16:32:46.000000 remoulade-3.2.0/remoulade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-24 16:32:46.000000 remoulade-3.2.0/remoulade.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-01-24 16:32:46.000000 remoulade-3.2.0/remoulade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-24 16:32:46.000000 remoulade-3.2.0/remoulade.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-01-24 16:32:46.077200 remoulade-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-01-24 16:32:33.000000 remoulade-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 16:32:46.073200 remoulade-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    21789 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_actors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_bucket_rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_channel_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    24688 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_concurrent_rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11408 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_generic_actors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_pidfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)    17403 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_stub_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_window_rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-01-24 16:32:33.000000 remoulade-3.2.0/tests/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.170499 remoulade-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-07 14:57:26.000000 remoulade-3.2.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-07 14:57:26.000000 remoulade-3.2.1/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 14:57:26.000000 remoulade-3.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-05-07 14:57:35.170499 remoulade-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-07 14:57:26.000000 remoulade-3.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.146499 remoulade-3.2.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      275 2024-05-07 14:57:26.000000 remoulade-3.2.1/bin/remoulade-gevent
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-07 14:57:26.000000 remoulade-3.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.146499 remoulade-3.2.1/remoulade/
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.150499 remoulade-3.2.1/remoulade/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/api/apispec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/api/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/api/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17584 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.150499 remoulade-3.2.1/remoulade/brokers/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/brokers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/brokers/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21619 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/brokers/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/brokers/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.150499 remoulade-3.2.1/remoulade/cancel/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/cancel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/cancel/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.150499 remoulade-3.2.1/remoulade/cancel/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/cancel/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/cancel/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/cancel/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/cancel/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/cancel/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.150499 remoulade-3.2.1/remoulade/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/cli/remoulade_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/cli/remoulade_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/cli/remoulade_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/collection_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12155 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.154499 remoulade-3.2.1/remoulade/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/helpers/actor_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/helpers/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/helpers/queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/helpers/redis_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/helpers/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.154499 remoulade-3.2.1/remoulade/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/age_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/catch_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/current_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/logging_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/max_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/max_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/middleware/worker_thread_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.154499 remoulade-3.2.1/remoulade/rate_limits/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/rate_limits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/rate_limits/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.158499 remoulade-3.2.1/remoulade/rate_limits/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/rate_limits/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/rate_limits/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/rate_limits/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/rate_limits/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/rate_limits/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/rate_limits/rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/rate_limits/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.158499 remoulade-3.2.1/remoulade/results/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/results/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.158499 remoulade-3.2.1/remoulade/results/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/results/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/results/backends/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/results/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/results/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/results/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/results/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.158499 remoulade-3.2.1/remoulade/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10477 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.158499 remoulade-3.2.1/remoulade/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/state/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.158499 remoulade-3.2.1/remoulade/state/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/state/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/state/backends/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/state/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/state/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/state/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/state/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19505 2024-05-07 14:57:26.000000 remoulade-3.2.1/remoulade/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.162499 remoulade-3.2.1/remoulade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-05-07 14:57:35.000000 remoulade-3.2.1/remoulade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-07 14:57:35.000000 remoulade-3.2.1/remoulade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:57:35.000000 remoulade-3.2.1/remoulade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-07 14:57:35.000000 remoulade-3.2.1/remoulade.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-07 14:57:35.000000 remoulade-3.2.1/remoulade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 14:57:35.000000 remoulade-3.2.1/remoulade.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-07 14:57:35.170499 remoulade-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-07 14:57:26.000000 remoulade-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:35.162499 remoulade-3.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    21789 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_actors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_bucket_rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_channel_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24688 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_concurrent_rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11408 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_generic_actors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_pidfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17403 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_stub_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_window_rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-07 14:57:26.000000 remoulade-3.2.1/tests/test_worker.py
```

### Comparing `remoulade-3.2.0/COPYING` & `remoulade-3.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/COPYING.LESSER` & `remoulade-3.2.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/PKG-INFO` & `remoulade-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remoulade
-Version: 3.2.0
+Version: 3.2.1
 Summary: Background Processing for Python 3.
 Author: Wiremind
 Author-email: dev@wiremind.io
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -32,44 +32,45 @@
 Provides-Extra: postgres
 Requires-Dist: sqlalchemy<2,>=1.4.29; extra == "postgres"
 Requires-Dist: psycopg2==2.9.5; extra == "postgres"
 Provides-Extra: pydantic
 Requires-Dist: pydantic>=2.0; extra == "pydantic"
 Requires-Dist: simplejson; extra == "pydantic"
 Provides-Extra: all
-Requires-Dist: redis~=5.0; extra == "all"
-Requires-Dist: simplejson; extra == "all"
-Requires-Dist: pydantic>=2.0; extra == "all"
-Requires-Dist: psycopg2==2.9.5; extra == "all"
-Requires-Dist: flask-apispec; extra == "all"
 Requires-Dist: marshmallow>=3; extra == "all"
 Requires-Dist: sqlalchemy<2,>=1.4.29; extra == "all"
-Requires-Dist: flask>=1.1,~=2.3.3; extra == "all"
+Requires-Dist: pydantic>=2.0; extra == "all"
+Requires-Dist: psycopg2==2.9.5; extra == "all"
+Requires-Dist: simplejson; extra == "all"
+Requires-Dist: redis~=5.0; extra == "all"
 Requires-Dist: amqpstorm<3,>=2.6; extra == "all"
+Requires-Dist: flask>=1.1,~=2.3.3; extra == "all"
+Requires-Dist: flask-apispec; extra == "all"
 Provides-Extra: dev
-Requires-Dist: redis~=5.0; extra == "dev"
-Requires-Dist: simplejson; extra == "dev"
-Requires-Dist: pydantic>=2.0; extra == "dev"
-Requires-Dist: psycopg2==2.9.5; extra == "dev"
-Requires-Dist: flask-apispec; extra == "dev"
 Requires-Dist: marshmallow>=3; extra == "dev"
 Requires-Dist: sqlalchemy<2,>=1.4.29; extra == "dev"
-Requires-Dist: flask>=1.1,~=2.3.3; extra == "dev"
+Requires-Dist: pydantic>=2.0; extra == "dev"
+Requires-Dist: psycopg2==2.9.5; extra == "dev"
+Requires-Dist: simplejson; extra == "dev"
+Requires-Dist: redis~=5.0; extra == "dev"
 Requires-Dist: amqpstorm<3,>=2.6; extra == "dev"
+Requires-Dist: flask>=1.1,~=2.3.3; extra == "dev"
+Requires-Dist: flask-apispec; extra == "dev"
 Requires-Dist: alabaster; extra == "dev"
 Requires-Dist: sphinx==4.1.1; extra == "dev"
 Requires-Dist: sphinxcontrib-napoleon; extra == "dev"
 Requires-Dist: sphinxcontrib-versioning; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: flake8-bugbear; extra == "dev"
 Requires-Dist: flake8-quotes; extra == "dev"
 Requires-Dist: isort; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: mypy>=0.930; extra == "dev"
+Requires-Dist: black~=23.12; extra == "dev"
+Requires-Dist: mypy~=1.10.0; extra == "dev"
+Requires-Dist: pyupgrade~=3.15.0; extra == "dev"
 Requires-Dist: sqlalchemy[mypy]; extra == "dev"
 Requires-Dist: types-redis; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: bumpversion; extra == "dev"
 Requires-Dist: hiredis; extra == "dev"
 Requires-Dist: twine; extra == "dev"
```

### Comparing `remoulade-3.2.0/README.md` & `remoulade-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/pyproject.toml` & `remoulade-3.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/__init__.py` & `remoulade-3.2.1/remoulade/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,8 +86,8 @@
     # Workers
     "Worker",
     # Scheduler
     "get_scheduler",
     "set_scheduler",
 ]
 
-__version__ = "3.2.0"
+__version__ = "3.2.1"
```

### Comparing `remoulade-3.2.0/remoulade/__main__.py` & `remoulade-3.2.1/remoulade/__main__.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/actor.py` & `remoulade-3.2.1/remoulade/actor.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/api/apispec.py` & `remoulade-3.2.1/remoulade/api/apispec.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/api/main.py` & `remoulade-3.2.1/remoulade/api/main.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/api/scheduler.py` & `remoulade-3.2.1/remoulade/api/scheduler.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/api/state.py` & `remoulade-3.2.1/remoulade/api/state.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/broker.py` & `remoulade-3.2.1/remoulade/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,36 +44,47 @@
     from .message import Message  # noqa
     from .middleware import Middleware
 
     M = TypeVar("M", bound=Middleware)
 #: The global broker instance.
 global_broker: "Optional[Broker]" = None
 
-#: The order in which middlewares are sorted
-middleware_order = [
-    WorkerThreadLogging,
-    AgeLimit,
-    TimeLimit,
-    ShutdownNotifications,
-    Pipelines,
-    Results,
-    CatchError,
-    Retries,
-    CurrentMessage,
-    LoggingMetadata,
-    MaxMemory,
-    MaxTasks,
-    MessageState,
-    Cancel,
-]
-
 #: A list of extra middleware that will be added to every new instance of Broker
 extra_default_middleware: "List[Middleware]" = []
 
 
+def _get_middleware_order():
+    #: The order in which middlewares are sorted
+    middleware_order = [
+        WorkerThreadLogging,
+        AgeLimit,
+        TimeLimit,
+        ShutdownNotifications,
+        Pipelines,
+        Results,
+        CatchError,
+        Retries,
+        CurrentMessage,
+        LoggingMetadata,
+        MaxMemory,
+        MaxTasks,
+        MessageState,
+        Cancel,
+    ]
+
+    try:
+        from opentelemetry.instrumentation.remoulade import _InstrumentationMiddleware
+
+        middleware_order.insert(0, _InstrumentationMiddleware)
+    except ImportError:
+        pass
+
+    return middleware_order
+
+
 def get_broker() -> "Broker":
     """Get the global broker instance.  If no global broker is set,
     this initializes a RabbitmqBroker and returns it.
 
     Returns:
       Broker: The default Broker.
     Raises:
@@ -266,14 +277,15 @@
 
 
         Parameters:
           middleware(Middleware): The middleware.
         """
         middleware_order_count = 0
         added_middleware_count = 0
+        middleware_order = _get_middleware_order()
 
         while added_middleware_count < len(self.middleware) and middleware_order_count < len(middleware_order):
             current_middleware = middleware_order[middleware_order_count]
             if isinstance(middleware, current_middleware):
                 if isinstance(self.middleware[added_middleware_count], current_middleware):
                     self.middleware[added_middleware_count] = middleware
                 else:
```

### Comparing `remoulade-3.2.0/remoulade/brokers/__init__.py` & `remoulade-3.2.1/remoulade/brokers/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/brokers/local.py` & `remoulade-3.2.1/remoulade/brokers/local.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/brokers/rabbitmq.py` & `remoulade-3.2.1/remoulade/brokers/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/brokers/stub.py` & `remoulade-3.2.1/remoulade/brokers/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/cancel/__init__.py` & `remoulade-3.2.1/remoulade/cancel/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/cancel/backend.py` & `remoulade-3.2.1/remoulade/cancel/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/cancel/backends/__init__.py` & `remoulade-3.2.1/remoulade/cancel/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/cancel/backends/redis.py` & `remoulade-3.2.1/remoulade/cancel/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/cancel/backends/stub.py` & `remoulade-3.2.1/remoulade/cancel/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/cancel/errors.py` & `remoulade-3.2.1/remoulade/cancel/errors.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/cancel/middleware.py` & `remoulade-3.2.1/remoulade/cancel/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/cli/remoulade_ls.py` & `remoulade-3.2.1/remoulade/cli/remoulade_ls.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/cli/remoulade_run.py` & `remoulade-3.2.1/remoulade/cli/remoulade_run.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/cli/remoulade_scheduler.py` & `remoulade-3.2.1/remoulade/cli/remoulade_scheduler.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/collection_results.py` & `remoulade-3.2.1/remoulade/collection_results.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/common.py` & `remoulade-3.2.1/remoulade/common.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/composition.py` & `remoulade-3.2.1/remoulade/composition.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/encoder.py` & `remoulade-3.2.1/remoulade/encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             else:
                 raise e
 
     def decode(self, data: bytes) -> MessageData:
         from remoulade import get_broker
 
         try:
-            raw_message = self.json_decoder.decode(data.decode("utf-8"))  # type: ignore
+            raw_message = self.json_decoder.decode(data.decode("utf-8"))
             actor_name = raw_message["actor_name"]
             actor_fn = get_broker().get_actor(actor_name).fn
 
             # Retrieve the Pydantic schemas from typing
             schemas_by_param_name = {}
             for param_name, type_hint in get_type_hints(actor_fn).items():
                 schemas_by_param_name[param_name] = TypeAdapter(
```

### Comparing `remoulade-3.2.0/remoulade/errors.py` & `remoulade-3.2.1/remoulade/errors.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/generic.py` & `remoulade-3.2.1/remoulade/generic.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/helpers/__init__.py` & `remoulade-3.2.1/remoulade/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/helpers/actor_arguments.py` & `remoulade-3.2.1/remoulade/helpers/actor_arguments.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/helpers/backoff.py` & `remoulade-3.2.1/remoulade/helpers/backoff.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/helpers/queues.py` & `remoulade-3.2.1/remoulade/helpers/queues.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/helpers/redis_client.py` & `remoulade-3.2.1/remoulade/helpers/redis_client.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/helpers/reduce.py` & `remoulade-3.2.1/remoulade/helpers/reduce.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/logging.py` & `remoulade-3.2.1/remoulade/logging.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/message.py` & `remoulade-3.2.1/remoulade/message.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/__init__.py` & `remoulade-3.2.1/remoulade/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/age_limit.py` & `remoulade-3.2.1/remoulade/middleware/age_limit.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/catch_error.py` & `remoulade-3.2.1/remoulade/middleware/catch_error.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/current_message.py` & `remoulade-3.2.1/remoulade/middleware/current_message.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/logging_metadata.py` & `remoulade-3.2.1/remoulade/middleware/logging_metadata.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/max_memory.py` & `remoulade-3.2.1/remoulade/middleware/max_memory.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/max_tasks.py` & `remoulade-3.2.1/remoulade/middleware/max_tasks.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/middleware.py` & `remoulade-3.2.1/remoulade/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/pipelines.py` & `remoulade-3.2.1/remoulade/middleware/pipelines.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/prometheus.py` & `remoulade-3.2.1/remoulade/middleware/prometheus.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/retries.py` & `remoulade-3.2.1/remoulade/middleware/retries.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/shutdown.py` & `remoulade-3.2.1/remoulade/middleware/shutdown.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/threading.py` & `remoulade-3.2.1/remoulade/middleware/threading.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/time_limit.py` & `remoulade-3.2.1/remoulade/middleware/time_limit.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/middleware/worker_thread_logging.py` & `remoulade-3.2.1/remoulade/middleware/worker_thread_logging.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/rate_limits/__init__.py` & `remoulade-3.2.1/remoulade/rate_limits/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/rate_limits/backend.py` & `remoulade-3.2.1/remoulade/rate_limits/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/rate_limits/backends/__init__.py` & `remoulade-3.2.1/remoulade/rate_limits/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/rate_limits/backends/redis.py` & `remoulade-3.2.1/remoulade/rate_limits/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/rate_limits/backends/stub.py` & `remoulade-3.2.1/remoulade/rate_limits/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/rate_limits/bucket.py` & `remoulade-3.2.1/remoulade/rate_limits/bucket.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/rate_limits/concurrent.py` & `remoulade-3.2.1/remoulade/rate_limits/concurrent.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/rate_limits/rate_limiter.py` & `remoulade-3.2.1/remoulade/rate_limits/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/rate_limits/window.py` & `remoulade-3.2.1/remoulade/rate_limits/window.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/result.py` & `remoulade-3.2.1/remoulade/result.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/results/__init__.py` & `remoulade-3.2.1/remoulade/results/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/results/backend.py` & `remoulade-3.2.1/remoulade/results/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/results/backends/__init__.py` & `remoulade-3.2.1/remoulade/results/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/results/backends/local.py` & `remoulade-3.2.1/remoulade/results/backends/local.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/results/backends/redis.py` & `remoulade-3.2.1/remoulade/results/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/results/backends/stub.py` & `remoulade-3.2.1/remoulade/results/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/results/errors.py` & `remoulade-3.2.1/remoulade/results/errors.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/results/middleware.py` & `remoulade-3.2.1/remoulade/results/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/scheduler/__init__.py` & `remoulade-3.2.1/remoulade/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/scheduler/scheduler.py` & `remoulade-3.2.1/remoulade/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/state/backend.py` & `remoulade-3.2.1/remoulade/state/backend.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/state/backends/__init__.py` & `remoulade-3.2.1/remoulade/state/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/state/backends/postgres.py` & `remoulade-3.2.1/remoulade/state/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/state/backends/redis.py` & `remoulade-3.2.1/remoulade/state/backends/redis.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/state/backends/stub.py` & `remoulade-3.2.1/remoulade/state/backends/stub.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/state/middleware.py` & `remoulade-3.2.1/remoulade/state/middleware.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/utils.py` & `remoulade-3.2.1/remoulade/utils.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade/worker.py` & `remoulade-3.2.1/remoulade/worker.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade.egg-info/PKG-INFO` & `remoulade-3.2.1/remoulade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remoulade
-Version: 3.2.0
+Version: 3.2.1
 Summary: Background Processing for Python 3.
 Author: Wiremind
 Author-email: dev@wiremind.io
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -32,44 +32,45 @@
 Provides-Extra: postgres
 Requires-Dist: sqlalchemy<2,>=1.4.29; extra == "postgres"
 Requires-Dist: psycopg2==2.9.5; extra == "postgres"
 Provides-Extra: pydantic
 Requires-Dist: pydantic>=2.0; extra == "pydantic"
 Requires-Dist: simplejson; extra == "pydantic"
 Provides-Extra: all
-Requires-Dist: redis~=5.0; extra == "all"
-Requires-Dist: simplejson; extra == "all"
-Requires-Dist: pydantic>=2.0; extra == "all"
-Requires-Dist: psycopg2==2.9.5; extra == "all"
-Requires-Dist: flask-apispec; extra == "all"
 Requires-Dist: marshmallow>=3; extra == "all"
 Requires-Dist: sqlalchemy<2,>=1.4.29; extra == "all"
-Requires-Dist: flask>=1.1,~=2.3.3; extra == "all"
+Requires-Dist: pydantic>=2.0; extra == "all"
+Requires-Dist: psycopg2==2.9.5; extra == "all"
+Requires-Dist: simplejson; extra == "all"
+Requires-Dist: redis~=5.0; extra == "all"
 Requires-Dist: amqpstorm<3,>=2.6; extra == "all"
+Requires-Dist: flask>=1.1,~=2.3.3; extra == "all"
+Requires-Dist: flask-apispec; extra == "all"
 Provides-Extra: dev
-Requires-Dist: redis~=5.0; extra == "dev"
-Requires-Dist: simplejson; extra == "dev"
-Requires-Dist: pydantic>=2.0; extra == "dev"
-Requires-Dist: psycopg2==2.9.5; extra == "dev"
-Requires-Dist: flask-apispec; extra == "dev"
 Requires-Dist: marshmallow>=3; extra == "dev"
 Requires-Dist: sqlalchemy<2,>=1.4.29; extra == "dev"
-Requires-Dist: flask>=1.1,~=2.3.3; extra == "dev"
+Requires-Dist: pydantic>=2.0; extra == "dev"
+Requires-Dist: psycopg2==2.9.5; extra == "dev"
+Requires-Dist: simplejson; extra == "dev"
+Requires-Dist: redis~=5.0; extra == "dev"
 Requires-Dist: amqpstorm<3,>=2.6; extra == "dev"
+Requires-Dist: flask>=1.1,~=2.3.3; extra == "dev"
+Requires-Dist: flask-apispec; extra == "dev"
 Requires-Dist: alabaster; extra == "dev"
 Requires-Dist: sphinx==4.1.1; extra == "dev"
 Requires-Dist: sphinxcontrib-napoleon; extra == "dev"
 Requires-Dist: sphinxcontrib-versioning; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: flake8-bugbear; extra == "dev"
 Requires-Dist: flake8-quotes; extra == "dev"
 Requires-Dist: isort; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: mypy>=0.930; extra == "dev"
+Requires-Dist: black~=23.12; extra == "dev"
+Requires-Dist: mypy~=1.10.0; extra == "dev"
+Requires-Dist: pyupgrade~=3.15.0; extra == "dev"
 Requires-Dist: sqlalchemy[mypy]; extra == "dev"
 Requires-Dist: types-redis; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: bumpversion; extra == "dev"
 Requires-Dist: hiredis; extra == "dev"
 Requires-Dist: twine; extra == "dev"
```

### Comparing `remoulade-3.2.0/remoulade.egg-info/SOURCES.txt` & `remoulade-3.2.1/remoulade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/remoulade.egg-info/requires.txt` & `remoulade-3.2.1/remoulade.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 prometheus-client>=0.2
 pytz
 python-dateutil>=2.8.0
 typing-extensions>=3.8
 attrs>=19.2.0
 
 [all]
-redis~=5.0
-simplejson
-pydantic>=2.0
-psycopg2==2.9.5
-flask-apispec
 marshmallow>=3
 sqlalchemy<2,>=1.4.29
-flask>=1.1,~=2.3.3
-amqpstorm<3,>=2.6
-
-[dev]
-redis~=5.0
-simplejson
 pydantic>=2.0
 psycopg2==2.9.5
+simplejson
+redis~=5.0
+amqpstorm<3,>=2.6
+flask>=1.1,~=2.3.3
 flask-apispec
+
+[dev]
 marshmallow>=3
 sqlalchemy<2,>=1.4.29
-flask>=1.1,~=2.3.3
+pydantic>=2.0
+psycopg2==2.9.5
+simplejson
+redis~=5.0
 amqpstorm<3,>=2.6
+flask>=1.1,~=2.3.3
+flask-apispec
 alabaster
 sphinx==4.1.1
 sphinxcontrib-napoleon
 sphinxcontrib-versioning
 sphinx-copybutton
 flake8
 flake8-bugbear
 flake8-quotes
 isort
-black
-mypy>=0.930
+black~=23.12
+mypy~=1.10.0
+pyupgrade~=3.15.0
 sqlalchemy[mypy]
 types-redis
 types-python-dateutil
 pre-commit
 bumpversion
 hiredis
 twine
```

### Comparing `remoulade-3.2.0/setup.cfg` & `remoulade-3.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/setup.py` & `remoulade-3.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,17 @@
     "sphinxcontrib-versioning",
     "sphinx-copybutton",
     # Linting
     "flake8",
     "flake8-bugbear",
     "flake8-quotes",
     "isort",
-    "black",
-    "mypy>=0.930",
+    "black~=23.12",
+    "mypy~=1.10.0",
+    "pyupgrade~=3.15.0",
     "sqlalchemy[mypy]",
     "types-redis",
     "types-python-dateutil",
     # Misc
     "pre-commit",
     "bumpversion",
     "hiredis",
```

### Comparing `remoulade-3.2.0/tests/test_actors.py` & `remoulade-3.2.1/tests/test_actors.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_broker.py` & `remoulade-3.2.1/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_bucket_rate_limiter.py` & `remoulade-3.2.1/tests/test_bucket_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_cancel.py` & `remoulade-3.2.1/tests/test_cancel.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_channel_pool.py` & `remoulade-3.2.1/tests/test_channel_pool.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_cli.py` & `remoulade-3.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_common.py` & `remoulade-3.2.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_composition.py` & `remoulade-3.2.1/tests/test_composition.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_concurrent_rate_limiter.py` & `remoulade-3.2.1/tests/test_concurrent_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_encoders.py` & `remoulade-3.2.1/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_generic_actors.py` & `remoulade-3.2.1/tests/test_generic_actors.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_helpers.py` & `remoulade-3.2.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_local.py` & `remoulade-3.2.1/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_pidfile.py` & `remoulade-3.2.1/tests/test_pidfile.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_rabbitmq.py` & `remoulade-3.2.1/tests/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_results.py` & `remoulade-3.2.1/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_scheduler.py` & `remoulade-3.2.1/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_stub_broker.py` & `remoulade-3.2.1/tests/test_stub_broker.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_window_rate_limiter.py` & `remoulade-3.2.1/tests/test_window_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `remoulade-3.2.0/tests/test_worker.py` & `remoulade-3.2.1/tests/test_worker.py`

 * *Files identical despite different names*

