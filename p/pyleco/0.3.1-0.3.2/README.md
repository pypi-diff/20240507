# Comparing `tmp/pyleco-0.3.1.tar.gz` & `tmp/pyleco-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyleco-0.3.1.tar", last modified: Fri Apr 12 08:28:50 2024, max compression
+gzip compressed data, was "pyleco-0.3.2.tar", last modified: Tue May  7 09:22:01 2024, max compression
```

## Comparing `pyleco-0.3.1.tar` & `pyleco-0.3.2.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.287855 pyleco-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.271855 pyleco-0.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-12 08:28:40.000000 pyleco-0.3.1/.github/pytest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 08:28:40.000000 pyleco-0.3.1/.github/sphinx.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.271855 pyleco-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-12 08:28:40.000000 pyleco-0.3.1/.github/workflows/pyleco_CI.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-12 08:28:40.000000 pyleco-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-12 08:28:40.000000 pyleco-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 08:28:40.000000 pyleco-0.3.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-12 08:28:40.000000 pyleco-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-04-12 08:28:40.000000 pyleco-0.3.1/GETTING_STARTED.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-12 08:28:40.000000 pyleco-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-04-12 08:28:50.287855 pyleco-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-04-12 08:28:40.000000 pyleco-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-12 08:28:40.000000 pyleco-0.3.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.275856 pyleco-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-12 08:28:40.000000 pyleco-0.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-12 08:28:40.000000 pyleco-0.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 08:28:40.000000 pyleco-0.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-12 08:28:40.000000 pyleco-0.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-12 08:28:40.000000 pyleco-0.3.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.275856 pyleco-0.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-12 08:28:40.000000 pyleco-0.3.1/examples/measurement_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-12 08:28:40.000000 pyleco-0.3.1/examples/pymeasure_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.275856 pyleco-0.3.1/pyleco/
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.275856 pyleco-0.3.1/pyleco/actors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/actors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/actors/actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.275856 pyleco-0.3.1/pyleco/coordinators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/coordinators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21798 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/coordinators/coordinator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/coordinators/proxy_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.279856 pyleco-0.3.1/pyleco/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/core/data_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/core/internal_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/core/leco_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/core/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.279856 pyleco-0.3.1/pyleco/directors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/directors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/directors/coordinator_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/directors/data_logger_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/directors/director.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/directors/starter_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/directors/transparent_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.279856 pyleco-0.3.1/pyleco/json_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/json_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/json_utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/json_utils/json_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/json_utils/rpc_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/json_utils/rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/json_utils/rpc_server_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.279856 pyleco-0.3.1/pyleco/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/management/data_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/management/starter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.279856 pyleco-0.3.1/pyleco/management/test_tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/management/test_tasks/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/pyleco/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/base_communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21601 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/coordinator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/data_publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/extended_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/log_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15471 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/pipe_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/qt_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/timers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/zmq_log_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.287855 pyleco-0.3.1/pyleco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-04-12 08:28:50.000000 pyleco-0.3.1/pyleco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-12 08:28:50.000000 pyleco-0.3.1/pyleco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:28:50.000000 pyleco-0.3.1/pyleco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-12 08:28:50.000000 pyleco-0.3.1/pyleco.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 08:28:50.000000 pyleco-0.3.1/pyleco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 08:28:50.000000 pyleco-0.3.1/pyleco.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:28:50.287855 pyleco-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/tests/acceptance_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/acceptance_tests/test_coordinator_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/acceptance_tests/test_director_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/acceptance_tests/test_proxy_server_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/acceptance_tests/test_starter_live.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/tests/actors/
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/actors/test_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/tests/coordinators/
--rw-r--r--   0 runner    (1001) docker     (127)    33403 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/coordinators/test_coordinator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/core/test_data_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/core/test_internal_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/core/test_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/core/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/tests/directors/
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/directors/test_coordinator_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/directors/test_data_logger_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/directors/test_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/directors/test_starter_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/directors/test_transparent_director.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.287855 pyleco-0.3.1/tests/json_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/json_utils/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/json_utils/test_json_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/json_utils/test_rpc_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/json_utils/test_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.287855 pyleco-0.3.1/tests/management/
--rw-r--r--   0 runner    (1001) docker     (127)    16238 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/management/test_data_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/management/test_starter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/test_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.287855 pyleco-0.3.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_base_communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22466 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_coordinator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_data_publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_extended_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_log_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)    26879 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    14522 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_pipe_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_qt_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_zmq_log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.177645 pyleco-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.161644 pyleco-0.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-07 09:21:49.000000 pyleco-0.3.2/.github/pytest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-07 09:21:49.000000 pyleco-0.3.2/.github/sphinx.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.161644 pyleco-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-07 09:21:49.000000 pyleco-0.3.2/.github/workflows/pyleco_CI.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-07 09:21:49.000000 pyleco-0.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-07 09:21:49.000000 pyleco-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 09:21:49.000000 pyleco-0.3.2/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-07 09:21:49.000000 pyleco-0.3.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-07 09:21:49.000000 pyleco-0.3.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-05-07 09:21:49.000000 pyleco-0.3.2/GETTING_STARTED.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 09:21:49.000000 pyleco-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-07 09:22:01.177645 pyleco-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-07 09:21:49.000000 pyleco-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-07 09:21:49.000000 pyleco-0.3.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.165644 pyleco-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-07 09:21:49.000000 pyleco-0.3.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-07 09:21:49.000000 pyleco-0.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 09:21:49.000000 pyleco-0.3.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-07 09:21:49.000000 pyleco-0.3.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 09:21:49.000000 pyleco-0.3.2/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.165644 pyleco-0.3.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-07 09:21:49.000000 pyleco-0.3.2/examples/measurement_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-07 09:21:49.000000 pyleco-0.3.2/examples/pymeasure_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.165644 pyleco-0.3.2/pyleco/
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.165644 pyleco-0.3.2/pyleco/actors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/actors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/actors/actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.165644 pyleco-0.3.2/pyleco/coordinators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/coordinators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21798 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/coordinators/coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/coordinators/proxy_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.169644 pyleco-0.3.2/pyleco/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/core/data_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/core/internal_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/core/leco_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/core/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.169644 pyleco-0.3.2/pyleco/directors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/directors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/directors/coordinator_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/directors/data_logger_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/directors/director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/directors/starter_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/directors/transparent_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.169644 pyleco-0.3.2/pyleco/json_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/json_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/json_utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/json_utils/json_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/json_utils/rpc_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/json_utils/rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/json_utils/rpc_server_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.169644 pyleco-0.3.2/pyleco/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/management/data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/management/starter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.169644 pyleco-0.3.2/pyleco/management/test_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/management/test_tasks/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.173644 pyleco-0.3.2/pyleco/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/base_communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21591 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/coordinator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/data_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/extended_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15471 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/pipe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/qt_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/timers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyleco/utils/zmq_log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.177645 pyleco-0.3.2/pyleco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-07 09:22:01.000000 pyleco-0.3.2/pyleco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-07 09:22:01.000000 pyleco-0.3.2/pyleco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:22:01.000000 pyleco-0.3.2/pyleco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 09:22:01.000000 pyleco-0.3.2/pyleco.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 09:22:01.000000 pyleco-0.3.2/pyleco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 09:22:01.000000 pyleco-0.3.2/pyleco.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-07 09:21:49.000000 pyleco-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:22:01.177645 pyleco-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.173644 pyleco-0.3.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.173644 pyleco-0.3.2/tests/acceptance_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/acceptance_tests/test_coordinator_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/acceptance_tests/test_director_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/acceptance_tests/test_proxy_server_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/acceptance_tests/test_starter_live.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.173644 pyleco-0.3.2/tests/actors/
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/actors/test_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.173644 pyleco-0.3.2/tests/coordinators/
+-rw-r--r--   0 runner    (1001) docker     (127)    33403 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/coordinators/test_coordinator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.173644 pyleco-0.3.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/core/test_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/core/test_internal_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/core/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/core/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.173644 pyleco-0.3.2/tests/directors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/directors/test_coordinator_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/directors/test_data_logger_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/directors/test_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/directors/test_starter_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/directors/test_transparent_director.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.173644 pyleco-0.3.2/tests/json_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/json_utils/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/json_utils/test_json_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/json_utils/test_rpc_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/json_utils/test_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.177645 pyleco-0.3.2/tests/management/
+-rw-r--r--   0 runner    (1001) docker     (127)    16238 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/management/test_data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/management/test_starter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:22:01.177645 pyleco-0.3.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/utils/test_base_communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/utils/test_communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22466 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/utils/test_coordinator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/utils/test_data_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/utils/test_extended_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/utils/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/utils/test_log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26879 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/utils/test_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/utils/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14522 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/utils/test_pipe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/utils/test_qt_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-07 09:21:49.000000 pyleco-0.3.2/tests/utils/test_zmq_log_handler.py
```

### Comparing `pyleco-0.3.1/.github/pytest.json` & `pyleco-0.3.2/.github/pytest.json`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/.github/sphinx.json` & `pyleco-0.3.2/.github/sphinx.json`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/.github/workflows/pyleco_CI.yml` & `pyleco-0.3.2/.github/workflows/pyleco_CI.yml`

 * *Files 2% similar despite different names*

```diff
@@ -87,19 +87,17 @@
         run: python --version
       - name: Install Pyleco
         # If the pytest problem matcher stops working because of bad paths, do an editable install
         run: pip install -e .[dev]  # editable for covtest
       - name: Test for Coverage
         run: pytest --cov=pyleco --cov-report=xml
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
-          directory: ./coverage/reports/
-          # env_vars: OS,PYTHON
           fail_ci_if_error: true
           files: ./coverage.xml,!./cache
           flags: unittests
           name: codecov-umbrella
           verbose: true
 
   test:
```

### Comparing `pyleco-0.3.1/.github/workflows/python-publish.yml` & `pyleco-0.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/.gitignore` & `pyleco-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/CHANGELOG.md` & `pyleco-0.3.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # CHANGELOG
 
+## [0.3.2] 2024-5-07
+
+### Fixed
+
+* Fix dependency on outdated UUIDv7 generating library to `uuid6` package ([#75](https://github.com/pymeasure/pyleco/pull/75))
+* Fix codecov CI ([#73](https://github.com/pymeasure/pyleco/pull/73))
+
+**Full Changelog**: https://github.com/pymeasure/pyleco/compare/v0.3.1...v0.3.2
+
+
 ## [0.3.1] 2024-04-12
 
 ### Fixed
 
 * Fix `Coordinator` to not use period in hostname as namespace ([#69](https://github.com/pymeasure/pyleco/pull/69))
 * Fix `DataLogger` timer ([#70](https://github.com/pymeasure/pyleco/pull/70))
 
@@ -122,15 +132,16 @@
 _Initial alpha version, complies with [LECO protocol alpha-0.0.1](https://github.com/pymeasure/leco-protocol/releases/tag/alpha-0.0.1)_
 
 ### New Contributors
 
 @BenediktBurger, @bilderbuchi, @bklebel
 
 
-[unreleased]: https://github.com/pymeasure/pyleco/compare/v0.3.1...HEAD
+[unreleased]: https://github.com/pymeasure/pyleco/compare/v0.3.2...HEAD
+[0.3.2]: https://github.com/pymeasure/pyleco/releases/tag/v0.3.2
 [0.3.1]: https://github.com/pymeasure/pyleco/releases/tag/v0.3.1
 [0.3.0]: https://github.com/pymeasure/pyleco/releases/tag/v0.3.0
 [0.2.2]: https://github.com/pymeasure/pyleco/releases/tag/v0.2.2
 [0.2.1]: https://github.com/pymeasure/pyleco/releases/tag/v0.2.1
 [0.2.0]: https://github.com/pymeasure/pyleco/releases/tag/v0.2.0
 [0.1.0]: https://github.com/pymeasure/pyleco/releases/tag/v0.1.0
 [alpha-0.0.1]: https://github.com/pymeasure/pyleco/releases/tag/alpha-0.0.1
```

### Comparing `pyleco-0.3.1/GETTING_STARTED.md` & `pyleco-0.3.2/GETTING_STARTED.md`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/LICENSE` & `pyleco-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/PKG-INFO` & `pyleco-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyleco
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python reference implementation of the Laboratory Experiment COntrol (LECO) protocol
 Author: PyLECO Developers
 License: MIT License
         
         Copyright (c) 2023-2024 PyLECO Developers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,37 +36,37 @@
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
 Requires-Dist: pyzmq>=22.3.0
 Requires-Dist: openrpc>=8.1.0; python_version >= "3.9"
-Requires-Dist: uuid7>=0.1.0
+Requires-Dist: uuid6>=2024.1.12
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 
 # PyLECO
 
+[![codecov](https://codecov.io/gh/pymeasure/pyleco/graph/badge.svg?token=9OB3GWDLRB)](https://codecov.io/gh/pymeasure/pyleco)
+[![pypi release](https://img.shields.io/pypi/v/pyleco.svg)](https://pypi.org/project/pyleco/)
+[![DOI](https://zenodo.org/badge/594982645.svg)](https://zenodo.org/doi/10.5281/zenodo.10837366)
+[![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
+
 Python reference implementation of the [Laboratory Experiment COntrol (LECO) protocol](https://github.com/pymeasure/leco-protocol).
 
 The [reviewed branch](https://github.com/pymeasure/pyleco/tree/reviewed) contains reviewed code, which does not yet contain all necessary modules and classes.
 Development happens in the [main](https://github.com/pymeasure/pyleco/tree/main) branch.
 
 Note: LECO is still under development, such that the code and API might change.
 The LECO protocol branch [pyleco-state](https://github.com/pymeasure/leco-protocol/tree/pyleco-state) contains the assumptions used in this project, which are not yet accepted into the LECO main branch.
 These things might change, if LECO defines them differently.
 
-[![codecov](https://codecov.io/gh/pymeasure/pyleco/graph/badge.svg?token=9OB3GWDLRB)](https://codecov.io/gh/pymeasure/pyleco)
-[![pypi release](https://img.shields.io/pypi/v/pyleco.svg)](https://pypi.org/project/pyleco/)
-[![DOI](https://zenodo.org/badge/594982645.svg)](https://zenodo.org/doi/10.5281/zenodo.10837366)
-[![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
-
 For a tutorial on how to get started, see [GETTING_STARTED.md](https://github.com/pymeasure/pyleco/blob/main/GETTING_STARTED.md).
 
 
 ## Quick Start
 
 1. Install Python,
 2. Execute `pip install pyleco`,
```

### Comparing `pyleco-0.3.1/README.md` & `pyleco-0.3.2/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # PyLECO
 
+[![codecov](https://codecov.io/gh/pymeasure/pyleco/graph/badge.svg?token=9OB3GWDLRB)](https://codecov.io/gh/pymeasure/pyleco)
+[![pypi release](https://img.shields.io/pypi/v/pyleco.svg)](https://pypi.org/project/pyleco/)
+[![DOI](https://zenodo.org/badge/594982645.svg)](https://zenodo.org/doi/10.5281/zenodo.10837366)
+[![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
+
 Python reference implementation of the [Laboratory Experiment COntrol (LECO) protocol](https://github.com/pymeasure/leco-protocol).
 
 The [reviewed branch](https://github.com/pymeasure/pyleco/tree/reviewed) contains reviewed code, which does not yet contain all necessary modules and classes.
 Development happens in the [main](https://github.com/pymeasure/pyleco/tree/main) branch.
 
 Note: LECO is still under development, such that the code and API might change.
 The LECO protocol branch [pyleco-state](https://github.com/pymeasure/leco-protocol/tree/pyleco-state) contains the assumptions used in this project, which are not yet accepted into the LECO main branch.
 These things might change, if LECO defines them differently.
 
-[![codecov](https://codecov.io/gh/pymeasure/pyleco/graph/badge.svg?token=9OB3GWDLRB)](https://codecov.io/gh/pymeasure/pyleco)
-[![pypi release](https://img.shields.io/pypi/v/pyleco.svg)](https://pypi.org/project/pyleco/)
-[![DOI](https://zenodo.org/badge/594982645.svg)](https://zenodo.org/doi/10.5281/zenodo.10837366)
-[![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
-
 For a tutorial on how to get started, see [GETTING_STARTED.md](https://github.com/pymeasure/pyleco/blob/main/GETTING_STARTED.md).
 
 
 ## Quick Start
 
 1. Install Python,
 2. Execute `pip install pyleco`,
```

### Comparing `pyleco-0.3.1/docs/Makefile` & `pyleco-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/docs/conf.py` & `pyleco-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/docs/make.bat` & `pyleco-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/examples/measurement_script.py` & `pyleco-0.3.2/examples/measurement_script.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/examples/pymeasure_actor.py` & `pyleco-0.3.2/examples/pymeasure_actor.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/__init__.py` & `pyleco-0.3.2/pyleco/__init__.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/actors/actor.py` & `pyleco-0.3.2/pyleco/actors/actor.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/coordinators/coordinator.py` & `pyleco-0.3.2/pyleco/coordinators/coordinator.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/coordinators/proxy_server.py` & `pyleco-0.3.2/pyleco/coordinators/proxy_server.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/core/__init__.py` & `pyleco-0.3.2/pyleco/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/core/data_message.py` & `pyleco-0.3.2/pyleco/core/data_message.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/core/internal_protocols.py` & `pyleco-0.3.2/pyleco/core/internal_protocols.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/core/leco_protocols.py` & `pyleco-0.3.2/pyleco/core/leco_protocols.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/core/message.py` & `pyleco-0.3.2/pyleco/core/message.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/core/serialization.py` & `pyleco-0.3.2/pyleco/core/serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 from __future__ import annotations
+import datetime
 from enum import IntEnum, IntFlag
 import json
 from typing import Any, Optional, NamedTuple, Union
 
-from uuid_extensions import uuid7  # type: ignore  #  as long as uuid does not yet support UUIDv7
+# as long as uuid does not yet support UUIDv7 use uuid6
+from uuid6 import uuid7
 from ..json_utils.json_objects import (
     Request,
     ParamsRequest,
     ResultResponse,
     ErrorResponse,
     Notification,
     ParamsNotification,
@@ -148,15 +150,20 @@
 def deserialize_data(content: bytes) -> Any:
     """Turn received message content into python objects."""
     return json.loads(content.decode())
 
 
 def generate_conversation_id() -> bytes:
     """Generate a conversation_id."""
-    return uuid7(as_type="bytes")  # type: ignore
+    return uuid7().bytes
+
+
+def conversation_id_to_datetime(conversation_id: bytes) -> datetime.datetime:
+    seconds_since_epoch = int.from_bytes(conversation_id[:6], byteorder="big", signed=False) / 1000
+    return datetime.datetime.fromtimestamp(seconds_since_epoch, tz=datetime.timezone.utc)
 
 
 def _get_json_object_type(data: dict[str, Any]) -> JsonContentTypes:
     if isinstance(data, dict):
         if "method" in data.keys():
             return JsonContentTypes.REQUEST
         elif "result" in data.keys():
```

### Comparing `pyleco-0.3.1/pyleco/directors/coordinator_director.py` & `pyleco-0.3.2/pyleco/directors/coordinator_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/directors/data_logger_director.py` & `pyleco-0.3.2/pyleco/directors/data_logger_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/directors/director.py` & `pyleco-0.3.2/pyleco/directors/director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/directors/starter_director.py` & `pyleco-0.3.2/pyleco/directors/starter_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/directors/transparent_director.py` & `pyleco-0.3.2/pyleco/directors/transparent_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/errors.py` & `pyleco-0.3.2/pyleco/errors.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/json_utils/__init__.py` & `pyleco-0.3.2/pyleco/json_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/json_utils/errors.py` & `pyleco-0.3.2/pyleco/json_utils/errors.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/json_utils/json_objects.py` & `pyleco-0.3.2/pyleco/json_utils/json_objects.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/json_utils/rpc_generator.py` & `pyleco-0.3.2/pyleco/json_utils/rpc_generator.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/json_utils/rpc_server.py` & `pyleco-0.3.2/pyleco/json_utils/rpc_server.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/json_utils/rpc_server_definition.py` & `pyleco-0.3.2/pyleco/json_utils/rpc_server_definition.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/management/data_logger.py` & `pyleco-0.3.2/pyleco/management/data_logger.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/management/starter.py` & `pyleco-0.3.2/pyleco/management/starter.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/management/test_tasks/test_task.py` & `pyleco-0.3.2/pyleco/management/test_tasks/test_task.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/test.py` & `pyleco-0.3.2/pyleco/test.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/utils/base_communicator.py` & `pyleco-0.3.2/pyleco/utils/base_communicator.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/utils/communicator.py` & `pyleco-0.3.2/pyleco/utils/communicator.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         self._last_beat = now
         super().send_message(message=message)
 
     def poll(self, timeout: Optional[float] = None) -> int:
         """Check how many messages arrived."""
         if timeout is None:
             timeout = self.timeout
-        return self.socket.poll(timeout=timeout * 1000)  # in ms
+        return self.socket.poll(timeout=int(timeout * 1000))  # in ms
 
     def handle_not_signed_in(self):
         super().handle_not_signed_in()
         raise ConnectionResetError("Have not been signed in, signing in.")
 
     def ask_message(self, message: Message, timeout: Optional[float] = None) -> Message:
         """Send and read the answer, signing in if necessary."""
```

### Comparing `pyleco-0.3.1/pyleco/utils/coordinator_utils.py` & `pyleco-0.3.2/pyleco/utils/coordinator_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     @abstractmethod
     def close(self, timeout: int) -> None: ...  # pragma: no cover
 
     @abstractmethod
     def send_message(self, identity: bytes, message: Message) -> None: ...  # pragma: no cover
 
     @abstractmethod
-    def message_received(self, timeout: float = 0) -> bool: ...  # pragma: no cover
+    def message_received(self, timeout: int = 0) -> bool: ...  # pragma: no cover
 
     @abstractmethod
     def read_message(self) -> tuple[bytes, Message]: ...  # pragma: no cover
 
 
 class ZmqMultiSocket(MultiSocket):
     """A MultiSocket using a zmq ROUTER socket."""
@@ -96,15 +96,15 @@
 
     def close(self, timeout: int = 0) -> None:
         self._sock.close(linger=timeout)
 
     def send_message(self, identity: bytes, message: Message) -> None:
         self._sock.send_multipart((identity, *message.to_frames()))
 
-    def message_received(self, timeout: float = 0) -> bool:
+    def message_received(self, timeout: int = 0) -> bool:
         return bool(self._sock.poll(timeout=timeout))
 
     def read_message(self) -> tuple[bytes, Message]:
         identity, *response = self._sock.recv_multipart()
         return identity, Message.from_frames(*response)
 
 
@@ -122,15 +122,15 @@
 
     def close(self, timeout: int) -> None:
         self.closed = True  # pragma: no cover
 
     def send_message(self, identity: bytes, message: Message) -> None:
         self._messages_sent.append((identity, message))
 
-    def message_received(self, timeout: float = 0) -> bool:
+    def message_received(self, timeout: int = 0) -> bool:
         return len(self._messages_read) > 0  # pragma: no cover
 
     def read_message(self) -> tuple[bytes, Message]:
         return self._messages_read.pop(0)
 
 
 @dataclass
@@ -158,15 +158,15 @@
 
     def is_connected(self) -> bool:
         return False
 
     def send_message(self, message: Message) -> None:
         raise NotImplementedError("Implement in subclass")  # pragma: no cover
 
-    def message_received(self, timeout: float = 0) -> bool:
+    def message_received(self, timeout: int = 0) -> bool:
         raise NotImplementedError("Implement in subclass")  # pragma: no cover
 
     def read_message(self, timeout: int = 0) -> Message:
         raise NotImplementedError("Implement in subclass")  # pragma: no cover
 
 
 class ZmqNode(Node):
@@ -196,15 +196,15 @@
         except AttributeError:
             return False
 
     def send_message(self, message: Message) -> None:
         """Send a multipart message to the Coordinator."""
         self._dealer.send_multipart(message.to_frames())
 
-    def message_received(self, timeout: float = 0) -> bool:
+    def message_received(self, timeout: int = 0) -> bool:
         return bool(self._dealer.poll(timeout=timeout))
 
     def read_message(self, timeout: int = 0) -> Message:
         return Message.from_frames(*self._dealer.recv_multipart())
 
 
 class FakeNode(Node):
```

### Comparing `pyleco-0.3.1/pyleco/utils/data_publisher.py` & `pyleco-0.3.2/pyleco/utils/data_publisher.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/utils/events.py` & `pyleco-0.3.2/pyleco/utils/events.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/utils/extended_message_handler.py` & `pyleco-0.3.2/pyleco/utils/extended_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/utils/listener.py` & `pyleco-0.3.2/pyleco/utils/listener.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/utils/log_levels.py` & `pyleco-0.3.2/pyleco/utils/log_levels.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/utils/message_handler.py` & `pyleco-0.3.2/pyleco/utils/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/utils/parser.py` & `pyleco-0.3.2/pyleco/utils/parser.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/utils/pipe_handler.py` & `pyleco-0.3.2/pyleco/utils/pipe_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/utils/qt_listener.py` & `pyleco-0.3.2/pyleco/utils/qt_listener.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/utils/timers.py` & `pyleco-0.3.2/pyleco/utils/timers.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco/utils/zmq_log_handler.py` & `pyleco-0.3.2/pyleco/utils/zmq_log_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/pyleco.egg-info/PKG-INFO` & `pyleco-0.3.2/pyleco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyleco
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python reference implementation of the Laboratory Experiment COntrol (LECO) protocol
 Author: PyLECO Developers
 License: MIT License
         
         Copyright (c) 2023-2024 PyLECO Developers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,37 +36,37 @@
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
 Requires-Dist: pyzmq>=22.3.0
 Requires-Dist: openrpc>=8.1.0; python_version >= "3.9"
-Requires-Dist: uuid7>=0.1.0
+Requires-Dist: uuid6>=2024.1.12
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 
 # PyLECO
 
+[![codecov](https://codecov.io/gh/pymeasure/pyleco/graph/badge.svg?token=9OB3GWDLRB)](https://codecov.io/gh/pymeasure/pyleco)
+[![pypi release](https://img.shields.io/pypi/v/pyleco.svg)](https://pypi.org/project/pyleco/)
+[![DOI](https://zenodo.org/badge/594982645.svg)](https://zenodo.org/doi/10.5281/zenodo.10837366)
+[![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
+
 Python reference implementation of the [Laboratory Experiment COntrol (LECO) protocol](https://github.com/pymeasure/leco-protocol).
 
 The [reviewed branch](https://github.com/pymeasure/pyleco/tree/reviewed) contains reviewed code, which does not yet contain all necessary modules and classes.
 Development happens in the [main](https://github.com/pymeasure/pyleco/tree/main) branch.
 
 Note: LECO is still under development, such that the code and API might change.
 The LECO protocol branch [pyleco-state](https://github.com/pymeasure/leco-protocol/tree/pyleco-state) contains the assumptions used in this project, which are not yet accepted into the LECO main branch.
 These things might change, if LECO defines them differently.
 
-[![codecov](https://codecov.io/gh/pymeasure/pyleco/graph/badge.svg?token=9OB3GWDLRB)](https://codecov.io/gh/pymeasure/pyleco)
-[![pypi release](https://img.shields.io/pypi/v/pyleco.svg)](https://pypi.org/project/pyleco/)
-[![DOI](https://zenodo.org/badge/594982645.svg)](https://zenodo.org/doi/10.5281/zenodo.10837366)
-[![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
-
 For a tutorial on how to get started, see [GETTING_STARTED.md](https://github.com/pymeasure/pyleco/blob/main/GETTING_STARTED.md).
 
 
 ## Quick Start
 
 1. Install Python,
 2. Execute `pip install pyleco`,
```

### Comparing `pyleco-0.3.1/pyleco.egg-info/SOURCES.txt` & `pyleco-0.3.2/pyleco.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 AUTHORS.txt
 CHANGELOG.md
+CITATION.cff
 GETTING_STARTED.md
 LICENSE
 README.md
 codecov.yml
 environment.yml
 pyproject.toml
 .github/pytest.json
```

### Comparing `pyleco-0.3.1/pyproject.toml` & `pyleco-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Topic :: System :: Networking",
 ]
 
 requires-python = ">=3.8"
 dependencies = [
   "pyzmq >= 22.3.0",
   "openrpc >= 8.1.0; python_version >= '3.9'",
-  "uuid7 >= 0.1.0",
+  "uuid6 >= 2024.1.12",
 ]
 
 [project.optional-dependencies]
 dev = [
   'pytest',
   'pytest-cov',
   'sphinx',
```

### Comparing `pyleco-0.3.1/tests/acceptance_tests/test_coordinator_live.py` & `pyleco-0.3.2/tests/acceptance_tests/test_coordinator_live.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/acceptance_tests/test_director_actor.py` & `pyleco-0.3.2/tests/acceptance_tests/test_director_actor.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/acceptance_tests/test_proxy_server_live.py` & `pyleco-0.3.2/tests/acceptance_tests/test_proxy_server_live.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/acceptance_tests/test_starter_live.py` & `pyleco-0.3.2/tests/acceptance_tests/test_starter_live.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/actors/test_actor.py` & `pyleco-0.3.2/tests/actors/test_actor.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/coordinators/test_coordinator.py` & `pyleco-0.3.2/tests/coordinators/test_coordinator.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/core/test_data_message.py` & `pyleco-0.3.2/tests/core/test_data_message.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/core/test_internal_protocols.py` & `pyleco-0.3.2/tests/core/test_internal_protocols.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/core/test_message.py` & `pyleco-0.3.2/tests/core/test_message.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/core/test_serialization.py` & `pyleco-0.3.2/tests/core/test_serialization.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 
 from __future__ import annotations
+import datetime
+import uuid
 from typing import Any, Optional, Union
 
 import pytest
 from pyleco.json_utils.json_objects import Request
 
 from pyleco.core import serialization
 from pyleco.core.serialization import JsonContentTypes, get_json_content_type
@@ -104,14 +106,31 @@
 
     def test_UUID_version(self, conversation_id):
         assert conversation_id[6] >> 4 == 7
 
     def test_variant(self, conversation_id):
         assert conversation_id[8] >> 6 == 0b10
 
+    def test_correct_timestamp(self, conversation_id):
+        ts = serialization.conversation_id_to_datetime(conversation_id=conversation_id)
+        assert abs(ts - datetime.datetime.now(datetime.timezone.utc)) < datetime.timedelta(hours=1)
+
+
+def test_conversation_id_to_datetime_according_to_uuid_example():
+    """According to the draft https://datatracker.ietf.org/doc/draft-ietf-uuidrev-rfc4122bis/14/
+    017F22E2-79B0-7CC3-98C4-DC0C0C07398F should be a timestamp of
+    Tuesday, February 22, 2022 2:22:22.00 PM GMT-05:00, represented as 1645557742000
+    """
+    cid = uuid.UUID("017F22E2-79B0-7CC3-98C4-DC0C0C07398F").bytes
+    reference = datetime.datetime(
+        2022, 2, 22, 14, 22, 22, tzinfo=datetime.timezone(datetime.timedelta(hours=-5))
+    )
+    ts = serialization.conversation_id_to_datetime(cid)
+    assert reference - ts == datetime.timedelta(0)
+
 
 def test_json_type_result_is_response():
     assert JsonContentTypes.RESPONSE in JsonContentTypes.RESULT_RESPONSE
     assert JsonContentTypes.RESULT in JsonContentTypes.RESULT_RESPONSE
 
 
 def test_json_type_error_is_response():
```

### Comparing `pyleco-0.3.1/tests/directors/test_coordinator_director.py` & `pyleco-0.3.2/tests/directors/test_coordinator_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/directors/test_data_logger_director.py` & `pyleco-0.3.2/tests/directors/test_data_logger_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/directors/test_director.py` & `pyleco-0.3.2/tests/directors/test_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/directors/test_starter_director.py` & `pyleco-0.3.2/tests/directors/test_starter_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/directors/test_transparent_director.py` & `pyleco-0.3.2/tests/directors/test_transparent_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/json_utils/test_errors.py` & `pyleco-0.3.2/tests/json_utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/json_utils/test_json_objects.py` & `pyleco-0.3.2/tests/json_utils/test_json_objects.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/json_utils/test_rpc_generator.py` & `pyleco-0.3.2/tests/json_utils/test_rpc_generator.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/json_utils/test_rpc_server.py` & `pyleco-0.3.2/tests/json_utils/test_rpc_server.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/management/test_data_logger.py` & `pyleco-0.3.2/tests/management/test_data_logger.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/management/test_starter.py` & `pyleco-0.3.2/tests/management/test_starter.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/test_test.py` & `pyleco-0.3.2/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/utils/test_base_communicator.py` & `pyleco-0.3.2/tests/utils/test_base_communicator.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/utils/test_communicator.py` & `pyleco-0.3.2/tests/utils/test_communicator.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/utils/test_coordinator_utils.py` & `pyleco-0.3.2/tests/utils/test_coordinator_utils.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/utils/test_data_publisher.py` & `pyleco-0.3.2/tests/utils/test_data_publisher.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/utils/test_extended_message_handler.py` & `pyleco-0.3.2/tests/utils/test_extended_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/utils/test_listener.py` & `pyleco-0.3.2/tests/utils/test_listener.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/utils/test_log_levels.py` & `pyleco-0.3.2/tests/utils/test_log_levels.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/utils/test_message_handler.py` & `pyleco-0.3.2/tests/utils/test_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/utils/test_parser.py` & `pyleco-0.3.2/tests/utils/test_parser.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/utils/test_pipe_handler.py` & `pyleco-0.3.2/tests/utils/test_pipe_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/utils/test_qt_listener.py` & `pyleco-0.3.2/tests/utils/test_qt_listener.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.1/tests/utils/test_zmq_log_handler.py` & `pyleco-0.3.2/tests/utils/test_zmq_log_handler.py`

 * *Files identical despite different names*

