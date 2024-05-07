# Comparing `tmp/temporalio-1.5.1.tar.gz` & `tmp/temporalio-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temporalio-1.5.1.tar", max compression
+gzip compressed data, was "temporalio-1.6.0.tar", max compression
```

## Comparing `temporalio-1.5.1.tar` & `temporalio-1.6.0.tar`

### file list

```diff
@@ -1,495 +1,492 @@
--rw-r--r--   0        0        0     1108 2024-02-27 16:05:59.803463 temporalio-1.5.1/LICENSE
--rw-r--r--   0        0        0    69553 2024-02-27 16:05:59.807464 temporalio-1.5.1/README.md
--rw-r--r--   0        0        0      899 2024-02-27 16:05:59.807464 temporalio-1.5.1/build.py
--rw-r--r--   0        0        0     6172 2024-02-27 16:05:59.807464 temporalio-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      423 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/__init__.py
--rw-r--r--   0        0        0    17894 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/activity.py
--rw-r--r--   0        0        0       36 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/__init__.py
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/batch/__init__.py
--rw-r--r--   0        0        0      388 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/batch/v1/__init__.py
--rw-r--r--   0        0        0     6384 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/batch/v1/message_pb2.py
--rw-r--r--   0        0        0     9555 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/batch/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/cluster/__init__.py
--rw-r--r--   0        0        0      286 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/cluster/v1/__init__.py
--rw-r--r--   0        0        0     5853 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/cluster/v1/message_pb2.py
--rw-r--r--   0        0        0    11757 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/cluster/v1/message_pb2.pyi
--rw-r--r--   0        0        0      158 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/cluster/v1/message_pb2_grpc.py
--rw-r--r--   0        0        0     1185 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/cluster/v1/message_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/command/__init__.py
--rw-r--r--   0        0        0     1476 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/command/v1/__init__.py
--rw-r--r--   0        0        0    22775 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/command/v1/message_pb2.py
--rw-r--r--   0        0        0    45400 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/command/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/common/__init__.py
--rw-r--r--   0        0        0      642 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/common/v1/__init__.py
--rw-r--r--   0        0        0     1540 2024-02-27 16:05:59.807464 temporalio-1.5.1/temporalio/api/common/v1/grpc_status_pb2.py
--rw-r--r--   0        0        0     1462 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/common/v1/grpc_status_pb2.pyi
--rw-r--r--   0        0        0    14100 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/common/v1/message_pb2.py
--rw-r--r--   0        0        0    20923 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/common/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/__init__.py
--rw-r--r--   0        0        0     2118 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/__init__.py
--rw-r--r--   0        0        0     2704 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/batch_operation_pb2.py
--rw-r--r--   0        0        0     3906 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/batch_operation_pb2.pyi
--rw-r--r--   0        0        0     3050 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/command_type_pb2.py
--rw-r--r--   0        0        0     4307 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/command_type_pb2.pyi
--rw-r--r--   0        0        0     2980 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/common_pb2.py
--rw-r--r--   0        0        0     4571 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/common_pb2.pyi
--rw-r--r--   0        0        0     6437 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/event_type_pb2.py
--rw-r--r--   0        0        0    20495 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/event_type_pb2.pyi
--rw-r--r--   0        0        0     9816 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/failed_cause_pb2.py
--rw-r--r--   0        0        0    19397 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/failed_cause_pb2.pyi
--rw-r--r--   0        0        0     2747 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/namespace_pb2.py
--rw-r--r--   0        0        0     4174 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/namespace_pb2.pyi
--rw-r--r--   0        0        0     2353 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/query_pb2.py
--rw-r--r--   0        0        0     3983 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/query_pb2.pyi
--rw-r--r--   0        0        0     2817 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/reset_pb2.py
--rw-r--r--   0        0        0     5713 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/reset_pb2.pyi
--rw-r--r--   0        0        0     2149 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/schedule_pb2.py
--rw-r--r--   0        0        0     5644 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/schedule_pb2.pyi
--rw-r--r--   0        0        0     2849 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/task_queue_pb2.py
--rw-r--r--   0        0        0     7514 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/task_queue_pb2.pyi
--rw-r--r--   0        0        0     2676 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/update_pb2.py
--rw-r--r--   0        0        0     6448 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/update_pb2.pyi
--rw-r--r--   0        0        0     7735 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/workflow_pb2.py
--rw-r--r--   0        0        0    15052 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/enums/v1/workflow_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/errordetails/__init__.py
--rw-r--r--   0        0        0     1034 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/errordetails/v1/__init__.py
--rw-r--r--   0        0        0    12726 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/errordetails/v1/message_pb2.py
--rw-r--r--   0        0        0    10736 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/errordetails/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/export/__init__.py
--rw-r--r--   0        0        0      129 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/export/v1/__init__.py
--rw-r--r--   0        0        0     2609 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/export/v1/message_pb2.py
--rw-r--r--   0        0        0     3010 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/export/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/failure/__init__.py
--rw-r--r--   0        0        0      530 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/failure/v1/__init__.py
--rw-r--r--   0        0        0     9303 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/failure/v1/message_pb2.py
--rw-r--r--   0        0        0    16245 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/failure/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/filter/__init__.py
--rw-r--r--   0        0        0      236 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/filter/v1/__init__.py
--rw-r--r--   0        0        0     4015 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/filter/v1/message_pb2.py
--rw-r--r--   0        0        0     4131 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/filter/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/history/__init__.py
--rw-r--r--   0        0        0     4730 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/history/v1/__init__.py
--rw-r--r--   0        0        0    69546 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/history/v1/message_pb2.py
--rw-r--r--   0        0        0   156397 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/history/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/interaction/__init__.py
--rw-r--r--   0        0        0      129 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/interaction/v1/__init__.py
--rw-r--r--   0        0        0     4385 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/interaction/v1/message_pb2.py
--rw-r--r--   0        0        0     7155 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/interaction/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/namespace/__init__.py
--rw-r--r--   0        0        0      300 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/namespace/v1/__init__.py
--rw-r--r--   0        0        0    10181 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/namespace/v1/message_pb2.py
--rw-r--r--   0        0        0    12925 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/namespace/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/operatorservice/__init__.py
--rw-r--r--   0        0        0     1423 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/operatorservice/v1/__init__.py
--rw-r--r--   0        0        0    17707 2024-02-27 16:05:59.811464 temporalio-1.5.1/temporalio/api/operatorservice/v1/request_response_pb2.py
--rw-r--r--   0        0        0    15980 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/operatorservice/v1/request_response_pb2.pyi
--rw-r--r--   0        0        0      158 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/operatorservice/v1/request_response_pb2_grpc.py
--rw-r--r--   0        0        0     1185 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/operatorservice/v1/request_response_pb2_grpc.pyi
--rw-r--r--   0        0        0     3359 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/operatorservice/v1/service_pb2.py
--rw-r--r--   0        0        0     1274 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/operatorservice/v1/service_pb2.pyi
--rw-r--r--   0        0        0    17632 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/operatorservice/v1/service_pb2_grpc.py
--rw-r--r--   0        0        0     8793 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/operatorservice/v1/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/protocol/__init__.py
--rw-r--r--   0        0        0       63 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/protocol/v1/__init__.py
--rw-r--r--   0        0        0     2034 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/protocol/v1/message_pb2.py
--rw-r--r--   0        0        0     3657 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/protocol/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/query/__init__.py
--rw-r--r--   0        0        0      159 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/query/v1/__init__.py
--rw-r--r--   0        0        0     3696 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/query/v1/message_pb2.py
--rw-r--r--   0        0        0     5000 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/query/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/replication/__init__.py
--rw-r--r--   0        0        0      214 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/replication/v1/__init__.py
--rw-r--r--   0        0        0     3775 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/replication/v1/message_pb2.py
--rw-r--r--   0        0        0     4288 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/replication/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/schedule/__init__.py
--rw-r--r--   0        0        0      732 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/schedule/v1/__init__.py
--rw-r--r--   0        0        0    16020 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/schedule/v1/message_pb2.py
--rw-r--r--   0        0        0    39783 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/schedule/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/sdk/__init__.py
--rw-r--r--   0        0        0      329 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/sdk/v1/__init__.py
--rw-r--r--   0        0        0     2058 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/sdk/v1/task_complete_metadata_pb2.py
--rw-r--r--   0        0        0     5122 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/sdk/v1/task_complete_metadata_pb2.pyi
--rw-r--r--   0        0        0     3542 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/sdk/v1/workflow_metadata_pb2.py
--rw-r--r--   0        0        0     5971 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/sdk/v1/workflow_metadata_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/taskqueue/__init__.py
--rw-r--r--   0        0        0      530 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/taskqueue/v1/__init__.py
--rw-r--r--   0        0        0     8986 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/taskqueue/v1/message_pb2.py
--rw-r--r--   0        0        0    12733 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/taskqueue/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/testservice/__init__.py
--rw-r--r--   0        0        0      814 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/testservice/v1/__init__.py
--rw-r--r--   0        0        0     6584 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/testservice/v1/request_response_pb2.py
--rw-r--r--   0        0        0     4609 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/testservice/v1/request_response_pb2.pyi
--rw-r--r--   0        0        0      158 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/testservice/v1/request_response_pb2_grpc.py
--rw-r--r--   0        0        0     1185 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/testservice/v1/request_response_pb2_grpc.pyi
--rw-r--r--   0        0        0     2532 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/testservice/v1/service_pb2.py
--rw-r--r--   0        0        0     1274 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/testservice/v1/service_pb2.pyi
--rw-r--r--   0        0        0    14985 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/testservice/v1/service_pb2_grpc.py
--rw-r--r--   0        0        0     9065 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/testservice/v1/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/update/__init__.py
--rw-r--r--   0        0        0      308 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/update/v1/__init__.py
--rw-r--r--   0        0        0     7265 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/update/v1/message_pb2.py
--rw-r--r--   0        0        0    11509 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/update/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/version/__init__.py
--rw-r--r--   0        0        0      123 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/version/v1/__init__.py
--rw-r--r--   0        0        0     3528 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/version/v1/message_pb2.py
--rw-r--r--   0        0        0     5233 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/version/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/workflow/__init__.py
--rw-r--r--   0        0        0      476 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/workflow/v1/__init__.py
--rw-r--r--   0        0        0    11283 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/workflow/v1/message_pb2.py
--rw-r--r--   0        0        0    25439 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/workflow/v1/message_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/workflowservice/__init__.py
--rw-r--r--   0        0        0     8907 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/workflowservice/v1/__init__.py
--rw-r--r--   0        0        0   125363 2024-02-27 16:05:59.815465 temporalio-1.5.1/temporalio/api/workflowservice/v1/request_response_pb2.py
--rw-r--r--   0        0        0   205481 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/api/workflowservice/v1/request_response_pb2.pyi
--rw-r--r--   0        0        0      158 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/api/workflowservice/v1/request_response_pb2_grpc.py
--rw-r--r--   0        0        0     1185 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/api/workflowservice/v1/request_response_pb2_grpc.pyi
--rw-r--r--   0        0        0    27279 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/api/workflowservice/v1/service_pb2.py
--rw-r--r--   0        0        0     1274 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/api/workflowservice/v1/service_pb2.pyi
--rw-r--r--   0        0        0   136945 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/api/workflowservice/v1/service_pb2_grpc.py
--rw-r--r--   0        0        0    67952 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/api/workflowservice/v1/service_pb2_grpc.pyi
--rw-r--r--   0        0        0    79075 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/Cargo.lock
--rw-r--r--   0        0        0      902 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/Cargo.toml
--rw-r--r--   0        0        0      122 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/__init__.py
--rw-r--r--   0        0        0     3827 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/client.py
--rw-r--r--   0        0        0     3411 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/metric.py
--rw-r--r--   0        0        0      144 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/__init__.py
--rw-r--r--   0        0        0      336 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/activity_result/__init__.py
--rw-r--r--   0        0        0     6517 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/activity_result/activity_result_pb2.py
--rw-r--r--   0        0        0     9319 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/activity_result/activity_result_pb2.pyi
--rw-r--r--   0        0        0      171 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/activity_task/__init__.py
--rw-r--r--   0        0        0     5900 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/activity_task/activity_task_pb2.py
--rw-r--r--   0        0        0    11710 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/activity_task/activity_task_pb2.pyi
--rw-r--r--   0        0        0     1435 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/bridge/__init__.py
--rw-r--r--   0        0        0    33694 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/bridge/bridge_pb2.py
--rw-r--r--   0        0        0    35620 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/bridge/bridge_pb2.pyi
--rw-r--r--   0        0        0      407 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/child_workflow/__init__.py
--rw-r--r--   0        0        0     6028 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/child_workflow/child_workflow_pb2.py
--rw-r--r--   0        0        0     9065 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/child_workflow/child_workflow_pb2.pyi
--rw-r--r--   0        0        0      144 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/common/__init__.py
--rw-r--r--   0        0        0     2270 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/common/common_pb2.py
--rw-r--r--   0        0        0     3473 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/common/common_pb2.pyi
--rw-r--r--   0        0        0     4340 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/core_interface_pb2.py
--rw-r--r--   0        0        0     2437 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/core_interface_pb2.pyi
--rw-r--r--   0        0        0      158 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/core_interface_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/core_interface_pb2_grpc.pyi
--rw-r--r--   0        0        0      145 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/external_data/__init__.py
--rw-r--r--   0        0        0     2882 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/external_data/external_data_pb2.py
--rw-r--r--   0        0        0     4346 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/external_data/external_data_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/health/__init__.py
--rw-r--r--   0        0        0      132 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/health/v1/__init__.py
--rw-r--r--   0        0        0     3055 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/health/v1/health_pb2.py
--rw-r--r--   0        0        0     2546 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/health/v1/health_pb2.pyi
--rw-r--r--   0        0        0     1168 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/workflow_activation/__init__.py
--rw-r--r--   0        0        0    25113 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/workflow_activation/workflow_activation_pb2.py
--rw-r--r--   0        0        0    49936 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/workflow_activation/workflow_activation_pb2.pyi
--rw-r--r--   0        0        0     1360 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/workflow_commands/__init__.py
--rw-r--r--   0        0        0    35980 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/workflow_commands/workflow_commands_pb2.py
--rw-r--r--   0        0        0    63691 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/workflow_commands/workflow_commands_pb2.pyi
--rw-r--r--   0        0        0      165 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/workflow_completion/__init__.py
--rw-r--r--   0        0        0     3971 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/workflow_completion/workflow_completion_pb2.py
--rw-r--r--   0        0        0     4425 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/proto/workflow_completion/workflow_completion_pb2.pyi
--rw-r--r--   0        0        0     3682 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/runtime.py
--rw-r--r--   0        0        0      523 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/.cargo/config.toml
--rw-r--r--   0        0        0       39 2024-02-27 16:06:00.455564 temporalio-1.5.1/temporalio/bridge/sdk-core/.git
--rw-r--r--   0        0        0      833 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/.github/workflows/heavy.yml
--rw-r--r--   0        0        0     2504 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/.github/workflows/per-pr.yml
--rw-r--r--   0        0        0      281 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/.gitignore
--rw-r--r--   0        0        0     7880 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/ARCHITECTURE.md
--rw-r--r--   0        0        0       36 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/CODEOWNERS
--rw-r--r--   0        0        0      380 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/Cargo.toml
--rw-r--r--   0        0        0     1108 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/LICENSE.txt
--rw-r--r--   0        0        0     5250 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/README.md
--rw-r--r--   0        0        0      555 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/arch_docs/diagrams/README.md
--rw-r--r--   0        0        0     1029 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/arch_docs/diagrams/sticky_queues.puml
--rw-r--r--   0        0        0   102701 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/arch_docs/diagrams/workflow_internals.svg
--rw-r--r--   0        0        0     3212 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/arch_docs/sticky_queues.md
--rwxr-xr-x   0        0        0      109 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/cargo-tokio-console.sh
--rw-r--r--   0        0        0     1049 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/client/Cargo.toml
--rw-r--r--   0        0        0    58112 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/client/src/lib.rs
--rw-r--r--   0        0        0     6611 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/client/src/metrics.rs
--rw-r--r--   0        0        0    38359 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/client/src/raw.rs
--rw-r--r--   0        0        0    25119 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/client/src/retry.rs
--rw-r--r--   0        0        0     8602 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/client/src/worker_registry/mod.rs
--rw-r--r--   0        0        0     6950 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/client/src/workflow_handle/mod.rs
--rw-r--r--   0        0        0     4027 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/Cargo.toml
--rw-r--r--   0        0        0     2426 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/benches/workflow_replay.rs
--rw-r--r--   0        0        0      836 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/abstractions/take_cell.rs
--rw-r--r--   0        0        0     9733 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/abstractions.rs
--rw-r--r--   0        0        0    42206 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/activity_tasks.rs
--rw-r--r--   0        0        0     7987 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/child_workflows.rs
--rw-r--r--   0        0        0    10823 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/determinism.rs
--rw-r--r--   0        0        0    48589 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/local_activities.rs
--rw-r--r--   0        0        0     3140 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/mod.rs
--rw-r--r--   0        0        0    33815 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/queries.rs
--rw-r--r--   0        0        0     6292 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/replay_flag.rs
--rw-r--r--   0        0        0     2484 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/updates.rs
--rw-r--r--   0        0        0     9518 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/workers.rs
--rw-r--r--   0        0        0     4233 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/workflow_cancels.rs
--rw-r--r--   0        0        0   104545 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/workflow_tasks.rs
--rw-r--r--   0        0        0    22352 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/ephemeral_server/mod.rs
--rw-r--r--   0        0        0     8831 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/internal_flags.rs
--rw-r--r--   0        0        0     9669 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/lib.rs
--rw-r--r--   0        0        0     2515 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/pollers/mod.rs
--rw-r--r--   0        0        0    12106 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/pollers/poll_buffer.rs
--rw-r--r--   0        0        0    16106 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/protosext/mod.rs
--rw-r--r--   0        0        0     3235 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/protosext/protocol_messages.rs
--rw-r--r--   0        0        0     9405 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/replay/mod.rs
--rw-r--r--   0        0        0     6553 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/retry_logic.rs
--rw-r--r--   0        0        0    10387 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/telemetry/log_export.rs
--rw-r--r--   0        0        0    39823 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/telemetry/metrics.rs
--rw-r--r--   0        0        0    12130 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/telemetry/mod.rs
--rw-r--r--   0        0        0     2952 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/telemetry/prometheus_server.rs
--rw-r--r--   0        0        0    34497 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/test_help/mod.rs
--rw-r--r--   0        0        0    23136 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/activities/activity_heartbeat_manager.rs
--rw-r--r--   0        0        0     2467 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/activities/activity_task_poller_stream.rs
--rw-r--r--   0        0        0    53677 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/activities/local_activities.rs
--rw-r--r--   0        0        0    41780 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/activities.rs
--rw-r--r--   0        0        0     4580 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/client/mocks.rs
--rw-r--r--   0        0        0    14127 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/client.rs
--rw-r--r--   0        0        0    27894 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/mod.rs
--rw-r--r--   0        0        0     5330 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/slot_provider.rs
--rw-r--r--   0        0        0     3407 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/driven_workflow.rs
--rw-r--r--   0        0        0    73598 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/history_update.rs
--rw-r--r--   0        0        0    33691 2024-02-27 16:06:01.199590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/activity_state_machine.rs
--rw-r--r--   0        0        0    10894 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/cancel_external_state_machine.rs
--rw-r--r--   0        0        0     5875 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/cancel_workflow_state_machine.rs
--rw-r--r--   0        0        0    41586 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/child_workflow_state_machine.rs
--rw-r--r--   0        0        0     4187 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/complete_workflow_state_machine.rs
--rw-r--r--   0        0        0     5263 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/continue_as_new_workflow_state_machine.rs
--rw-r--r--   0        0        0     3903 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/fail_workflow_state_machine.rs
--rw-r--r--   0        0        0    58549 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/local_activity_state_machine.rs
--rw-r--r--   0        0        0    11681 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/mod.rs
--rw-r--r--   0        0        0     5759 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/modify_workflow_properties_state_machine.rs
--rw-r--r--   0        0        0    32183 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/patch_state_machine.rs
--rw-r--r--   0        0        0    16311 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/signal_external_state_machine.rs
--rw-r--r--   0        0        0    13484 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/timer_state_machine.rs
--rw-r--r--   0        0        0     7999 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/transition_coverage.rs
--rw-r--r--   0        0        0    14487 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/update_state_machine.rs
--rw-r--r--   0        0        0    15423 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/upsert_search_attributes_state_machine.rs
--rw-r--r--   0        0        0     3593 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/workflow_machines/local_acts.rs
--rw-r--r--   0        0        0    74513 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/workflow_machines.rs
--rw-r--r--   0        0        0     8693 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/workflow_task_state_machine.rs
--rw-r--r--   0        0        0    56953 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/managed_run.rs
--rw-r--r--   0        0        0    58800 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/mod.rs
--rw-r--r--   0        0        0     4402 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/run_cache.rs
--rw-r--r--   0        0        0     5437 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/wft_extraction.rs
--rw-r--r--   0        0        0     4212 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/wft_poller.rs
--rw-r--r--   0        0        0     4014 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/workflow_stream/saved_wf_inputs.rs
--rw-r--r--   0        0        0      509 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/workflow_stream/tonic_status_serde.rs
--rw-r--r--   0        0        0    30192 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/workflow_stream.rs
--rw-r--r--   0        0        0      972 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core-api/Cargo.toml
--rw-r--r--   0        0        0     2912 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core-api/src/errors.rs
--rw-r--r--   0        0        0     6298 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core-api/src/lib.rs
--rw-r--r--   0        0        0    10619 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core-api/src/telemetry/metrics.rs
--rw-r--r--   0        0        0     6282 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core-api/src/telemetry.rs
--rw-r--r--   0        0        0    10029 2024-02-27 16:06:01.195590 temporalio-1.5.1/temporalio/bridge/sdk-core/core-api/src/worker.rs
--rw-r--r--   0        0        0      963 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/docker/docker-compose-telem.yaml
--rw-r--r--   0        0        0      839 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/docker/docker-compose.yaml
--rw-r--r--   0        0        0     7987 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/etc/deps.svg
--rw-r--r--   0        0        0      332 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/etc/dynamic-config.yaml
--rw-r--r--   0        0        0      574 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/etc/otel-collector-config.yaml
--rw-r--r--   0        0        0      173 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/etc/prometheus.yaml
--rwxr-xr-x   0        0        0      204 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/etc/regen-depgraph.sh
--rw-r--r--   0        0        0      574 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/Cargo.toml
--rw-r--r--   0        0        0     1108 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/LICENSE.txt
--rw-r--r--   0        0        0      126 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/README.md
--rw-r--r--   0        0        0      623 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/Cargo.toml
--rw-r--r--   0        0        0     1108 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/LICENSE.txt
--rw-r--r--   0        0        0    26182 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/src/lib.rs
--rw-r--r--   0        0        0      191 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/progress.rs
--rw-r--r--   0        0        0      299 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/dupe_transitions_fail.rs
--rw-r--r--   0        0        0      387 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/dupe_transitions_fail.stderr
--rw-r--r--   0        0        0      892 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/dynamic_dest_pass.rs
--rw-r--r--   0        0        0      202 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/forgot_name_fail.rs
--rw-r--r--   0        0        0      331 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/forgot_name_fail.stderr
--rw-r--r--   0        0        0      686 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/handler_arg_pass.rs
--rw-r--r--   0        0        0      619 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/handler_pass.rs
--rw-r--r--   0        0        0      862 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/medium_complex_pass.rs
--rw-r--r--   0        0        0      584 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/no_handle_conversions_require_into_fail.rs
--rw-r--r--   0        0        0      694 2024-02-27 16:06:01.203590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/no_handle_conversions_require_into_fail.stderr
--rw-r--r--   0        0        0      649 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/simple_pass.rs
--rw-r--r--   0        0        0      307 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/struct_event_variant_fail.rs
--rw-r--r--   0        0        0      161 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/struct_event_variant_fail.stderr
--rw-r--r--   0        0        0      184 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/tuple_more_item_event_variant_fail.rs
--rw-r--r--   0        0        0      189 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/tuple_more_item_event_variant_fail.stderr
--rw-r--r--   0        0        0      176 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/tuple_zero_item_event_variant_fail.rs
--rw-r--r--   0        0        0      181 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/tuple_zero_item_event_variant_fail.stderr
--rw-r--r--   0        0        0      366 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_trait/Cargo.toml
--rw-r--r--   0        0        0     1108 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_trait/LICENSE.txt
--rw-r--r--   0        0        0     6524 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_trait/src/lib.rs
--rw-r--r--   0        0        0      103 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/src/lib.rs
--rw-r--r--   0        0        0     1206 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/histories/ends_empty_wft_complete.bin
--rw-r--r--   0        0        0     1853 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/histories/evict_while_la_running_no_interference-16_history.bin
--rw-r--r--   0        0        0     3277 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/histories/evict_while_la_running_no_interference-23_history.bin
--rw-r--r--   0        0        0     2532 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/histories/evict_while_la_running_no_interference-85_history.bin
--rw-r--r--   0        0        0      924 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/histories/fail_wf_task.bin
--rw-r--r--   0        0        0     1701 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/histories/old_change_marker_format.bin
--rw-r--r--   0        0        0      711 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/histories/timer_workflow_history.bin
--rwxr-xr-x   0        0        0      213 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/integ-with-otel.sh
--rw-r--r--   0        0        0       27 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/rustfmt.toml
--rw-r--r--   0        0        0     1275 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/Cargo.toml
--rw-r--r--   0        0        0     8019 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/activity_context.rs
--rw-r--r--   0        0        0      979 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/app_data.rs
--rw-r--r--   0        0        0     1789 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/interceptors.rs
--rw-r--r--   0        0        0    34783 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/lib.rs
--rw-r--r--   0        0        0      523 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/payload_converter.rs
--rw-r--r--   0        0        0    12104 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/workflow_context/options.rs
--rw-r--r--   0        0        0    25361 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/workflow_context.rs
--rw-r--r--   0        0        0    28088 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/workflow_future.rs
--rw-r--r--   0        0        0      912 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/Cargo.toml
--rw-r--r--   0        0        0     5393 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/build.rs
--rw-r--r--   0        0        0       57 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.buildkite/Dockerfile
--rw-r--r--   0        0        0      336 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.buildkite/docker-compose.yml
--rw-r--r--   0        0        0      223 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.buildkite/pipeline.yml
--rw-r--r--   0        0        0      234 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.github/CODEOWNERS
--rw-r--r--   0        0        0      227 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      587 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.github/workflows/publish-docs.yml
--rw-r--r--   0        0        0     1097 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.github/workflows/trigger-api-go-update.yml
--rw-r--r--   0        0        0       32 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.gitignore
--rw-r--r--   0        0        0     1108 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/LICENSE
--rw-r--r--   0        0        0     2882 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/Makefile
--rw-r--r--   0        0        0      151 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/README.md
--rw-r--r--   0        0        0     1760 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/api-linter.yaml
--rw-r--r--   0        0        0      470 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/buf.gen.yaml
--rw-r--r--   0        0        0      289 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/buf.lock
--rw-r--r--   0        0        0      333 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/buf.yaml
--rw-r--r--   0        0        0     1045 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/api/annotations.proto
--rw-r--r--   0        0        0    15159 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/api/http.proto
--rw-r--r--   0        0        0     6153 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/any.proto
--rw-r--r--   0        0        0    49556 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/descriptor.proto
--rw-r--r--   0        0        0     4891 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/duration.proto
--rw-r--r--   0        0        0     2363 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/empty.proto
--rw-r--r--   0        0        0     6448 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/timestamp.proto
--rw-r--r--   0        0        0     4043 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/wrappers.proto
--rw-r--r--   0        0        0     4369 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/batch/v1/message.proto
--rw-r--r--   0        0        0    12821 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/command/v1/message.proto
--rw-r--r--   0        0        0     7856 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/common/v1/message.proto
--rw-r--r--   0        0        0     1950 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/batch_operation.proto
--rw-r--r--   0        0        0     2465 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/command_type.proto
--rw-r--r--   0        0        0     2062 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/common.proto
--rw-r--r--   0        0        0    10063 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/event_type.proto
--rw-r--r--   0        0        0     7346 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/failed_cause.proto
--rw-r--r--   0        0        0     1944 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/namespace.proto
--rw-r--r--   0        0        0     2098 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/query.proto
--rw-r--r--   0        0        0     2848 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/reset.proto
--rw-r--r--   0        0        0     3212 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/schedule.proto
--rw-r--r--   0        0        0     3715 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/task_queue.proto
--rw-r--r--   0        0        0     3524 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/update.proto
--rw-r--r--   0        0        0     5083 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/workflow.proto
--rw-r--r--   0        0        0     3957 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/errordetails/v1/message.proto
--rw-r--r--   0        0        0     1884 2024-02-27 16:06:01.207590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/export/v1/message.proto
--rw-r--r--   0        0        0     4728 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/failure/v1/message.proto
--rw-r--r--   0        0        0     1965 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/filter/v1/message.proto
--rw-r--r--   0        0        0    42913 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/history/v1/message.proto
--rw-r--r--   0        0        0     3917 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/namespace/v1/message.proto
--rw-r--r--   0        0        0     4462 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/operatorservice/v1/request_response.proto
--rw-r--r--   0        0        0     4190 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/operatorservice/v1/service.proto
--rw-r--r--   0        0        0     2427 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/protocol/v1/message.proto
--rw-r--r--   0        0        0     2587 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/query/v1/message.proto
--rw-r--r--   0        0        0     2138 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/replication/v1/message.proto
--rw-r--r--   0        0        0    17755 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/schedule/v1/message.proto
--rw-r--r--   0        0        0     3871 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/sdk/v1/task_complete_metadata.proto
--rw-r--r--   0        0        0     3072 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/sdk/v1/workflow_metadata.proto
--rw-r--r--   0        0        0     4361 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/taskqueue/v1/message.proto
--rw-r--r--   0        0        0     3984 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/update/v1/message.proto
--rw-r--r--   0        0        0     2265 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/version/v1/message.proto
--rw-r--r--   0        0        0     7002 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/workflow/v1/message.proto
--rw-r--r--   0        0        0    61128 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/workflowservice/v1/request_response.proto
--rw-r--r--   0        0        0    30601 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/workflowservice/v1/service.proto
--rw-r--r--   0        0        0     2069 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/google/rpc/status.proto
--rw-r--r--   0        0        0     2416 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/grpc/health/v1/health.proto
--rw-r--r--   0        0        0     2716 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/activity_result/activity_result.proto
--rw-r--r--   0        0        0     3066 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/activity_task/activity_task.proto
--rw-r--r--   0        0        0     2322 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/child_workflow/child_workflow.proto
--rw-r--r--   0        0        0     1260 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/common/common.proto
--rw-r--r--   0        0        0     1313 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/core_interface.proto
--rw-r--r--   0        0        0     1726 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/external_data/external_data.proto
--rw-r--r--   0        0        0    15881 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/workflow_activation/workflow_activation.proto
--rw-r--r--   0        0        0    16340 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/workflow_commands/workflow_commands.proto
--rw-r--r--   0        0        0     1230 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/workflow_completion/workflow_completion.proto
--rw-r--r--   0        0        0     2139 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/Makefile
--rw-r--r--   0        0        0     1029 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/api-linter.yaml
--rw-r--r--   0        0        0      137 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/buf.yaml
--rw-r--r--   0        0        0     2043 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/temporal/api/testservice/v1/request_response.proto
--rw-r--r--   0        0        0     4494 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/temporal/api/testservice/v1/service.proto
--rw-r--r--   0        0        0      334 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/src/constants.rs
--rw-r--r--   0        0        0    23459 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/src/history_builder.rs
--rw-r--r--   0        0        0     9321 2024-02-27 16:06:01.211590 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/src/history_info.rs
--rw-r--r--   0        0        0    92827 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/src/lib.rs
--rw-r--r--   0        0        0     1289 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/src/task_token.rs
--rw-r--r--   0        0        0      844 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/src/utilities.rs
--rw-r--r--   0        0        0      916 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/test-utils/Cargo.toml
--rw-r--r--   0        0        0    48345 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/test-utils/src/canned_histories.rs
--rw-r--r--   0        0        0     1091 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/test-utils/src/histfetch.rs
--rw-r--r--   0        0        0     1366 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/test-utils/src/interceptors.rs
--rw-r--r--   0        0        0    28626 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/test-utils/src/lib.rs
--rw-r--r--   0        0        0     1617 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/test-utils/src/wf_input_saver.rs
--rw-r--r--   0        0        0     1148 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/test-utils/src/workflows.rs
--rw-r--r--   0        0        0     4751 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/fuzzy_workflow.rs
--rw-r--r--   0        0        0     8767 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/heavy_tests.rs
--rw-r--r--   0        0        0      118 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/activity_functions.rs
--rw-r--r--   0        0        0     1353 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/client_tests.rs
--rw-r--r--   0        0        0     5118 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/ephemeral_server_tests.rs
--rw-r--r--   0        0        0     8263 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/heartbeat_tests.rs
--rw-r--r--   0        0        0    17653 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/metrics_tests.rs
--rw-r--r--   0        0        0     3333 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/polling_tests.rs
--rw-r--r--   0        0        0    17683 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/queries_tests.rs
--rw-r--r--   0        0        0    31251 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/update_tests.rs
--rw-r--r--   0        0        0     5061 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/visibility_tests.rs
--rw-r--r--   0        0        0    36651 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/activities.rs
--rw-r--r--   0        0        0     1996 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/appdata_propagation.rs
--rw-r--r--   0        0        0     1713 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/cancel_external.rs
--rw-r--r--   0        0        0     1625 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/cancel_wf.rs
--rw-r--r--   0        0        0     6265 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/child_workflows.rs
--rw-r--r--   0        0        0     1986 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/continue_as_new.rs
--rw-r--r--   0        0        0     1628 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/determinism.rs
--rw-r--r--   0        0        0     2292 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/eager.rs
--rw-r--r--   0        0        0    24762 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/local_activities.rs
--rw-r--r--   0        0        0     1616 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/modify_wf_properties.rs
--rw-r--r--   0        0        0     7129 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/patches.rs
--rw-r--r--   0        0        0    10648 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/replay.rs
--rw-r--r--   0        0        0     3038 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/resets.rs
--rw-r--r--   0        0        0     5449 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/signals.rs
--rw-r--r--   0        0        0     3059 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/stickyness.rs
--rw-r--r--   0        0        0     3906 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/timers.rs
--rw-r--r--   0        0        0     2614 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/upsert_search_attrs.rs
--rw-r--r--   0        0        0    25151 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests.rs
--rw-r--r--   0        0        0     3401 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/main.rs
--rw-r--r--   0        0        0     4461 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/runner.rs
--rw-r--r--   0        0        0      850 2024-02-27 16:06:01.215591 temporalio-1.5.1/temporalio/bridge/sdk-core/tests/wf_input_replay.rs
--rw-r--r--   0        0        0    18493 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/src/client.rs
--rw-r--r--   0        0        0     3130 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/src/lib.rs
--rw-r--r--   0        0        0     9556 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/src/metric.rs
--rw-r--r--   0        0        0    13370 2024-02-27 16:05:59.819465 temporalio-1.5.1/temporalio/bridge/src/runtime.rs
--rw-r--r--   0        0        0     5587 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/bridge/src/testing.rs
--rw-r--r--   0        0        0    11247 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/bridge/src/worker.rs
--rw-r--r--   0        0        0     2384 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/bridge/testing.py
--rw-r--r--   0        0        0    13413 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/bridge/worker.py
--rw-r--r--   0        0        0   215552 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/client.py
--rw-r--r--   0        0        0    31286 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/common.py
--rw-r--r--   0        0        0       57 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/contrib/__init__.py
--rw-r--r--   0        0        0    27336 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/contrib/opentelemetry.py
--rw-r--r--   0        0        0    59296 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/converter.py
--rw-r--r--   0        0        0    10663 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/py.typed
--rw-r--r--   0        0        0    21661 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/runtime.py
--rw-r--r--   0        0        0    29986 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/service.py
--rw-r--r--   0        0        0      207 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/testing/__init__.py
--rw-r--r--   0        0        0     7345 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/testing/_activity.py
--rw-r--r--   0        0        0    23571 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/testing/_workflow.py
--rw-r--r--   0        0        0     4443 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/types.py
--rw-r--r--   0        0        0     1880 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/worker/__init__.py
--rw-r--r--   0        0        0    40083 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/worker/_activity.py
--rw-r--r--   0        0        0    13085 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/worker/_interceptor.py
--rw-r--r--   0        0        0    13086 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/worker/_replayer.py
--rw-r--r--   0        0        0    32680 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/worker/_worker.py
--rw-r--r--   0        0        0    16082 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/worker/_workflow.py
--rw-r--r--   0        0        0   102067 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/worker/_workflow_instance.py
--rw-r--r--   0        0        0     2481 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/worker/workflow_sandbox/__init__.py
--rw-r--r--   0        0        0    17707 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/worker/workflow_sandbox/_importer.py
--rw-r--r--   0        0        0     1817 2024-02-27 16:05:59.823466 temporalio-1.5.1/temporalio/worker/workflow_sandbox/_in_sandbox.py
--rw-r--r--   0        0        0    40485 2024-02-27 16:05:59.827467 temporalio-1.5.1/temporalio/worker/workflow_sandbox/_restrictions.py
--rw-r--r--   0        0        0     6571 2024-02-27 16:05:59.827467 temporalio-1.5.1/temporalio/worker/workflow_sandbox/_runner.py
--rw-r--r--   0        0        0   158288 2024-02-27 16:05:59.827467 temporalio-1.5.1/temporalio/workflow.py
--rw-r--r--   0        0        0    80749 1970-01-01 00:00:00.000000 temporalio-1.5.1/setup.py
--rw-r--r--   0        0        0    70833 1970-01-01 00:00:00.000000 temporalio-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1108 2024-05-07 14:04:43.407591 temporalio-1.6.0/LICENSE
+-rw-r--r--   0        0        0    70194 2024-05-07 14:04:43.407591 temporalio-1.6.0/README.md
+-rw-r--r--   0        0        0      899 2024-05-07 14:04:43.407591 temporalio-1.6.0/build.py
+-rw-r--r--   0        0        0     6392 2024-05-07 14:04:43.411591 temporalio-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      423 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/__init__.py
+-rw-r--r--   0        0        0    18671 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/activity.py
+-rw-r--r--   0        0        0       36 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/batch/__init__.py
+-rw-r--r--   0        0        0      388 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/batch/v1/__init__.py
+-rw-r--r--   0        0        0     6384 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/batch/v1/message_pb2.py
+-rw-r--r--   0        0        0     9555 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/batch/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/cluster/__init__.py
+-rw-r--r--   0        0        0      286 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/cluster/v1/__init__.py
+-rw-r--r--   0        0        0     5853 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/cluster/v1/message_pb2.py
+-rw-r--r--   0        0        0    11757 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/cluster/v1/message_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/cluster/v1/message_pb2_grpc.py
+-rw-r--r--   0        0        0     1185 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/cluster/v1/message_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/command/__init__.py
+-rw-r--r--   0        0        0     1476 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/command/v1/__init__.py
+-rw-r--r--   0        0        0    22775 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/command/v1/message_pb2.py
+-rw-r--r--   0        0        0    45400 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/command/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/common/__init__.py
+-rw-r--r--   0        0        0      642 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/common/v1/__init__.py
+-rw-r--r--   0        0        0     1540 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/common/v1/grpc_status_pb2.py
+-rw-r--r--   0        0        0     1462 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/common/v1/grpc_status_pb2.pyi
+-rw-r--r--   0        0        0    14100 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/common/v1/message_pb2.py
+-rw-r--r--   0        0        0    20923 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/common/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/enums/__init__.py
+-rw-r--r--   0        0        0     2118 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/enums/v1/__init__.py
+-rw-r--r--   0        0        0     2704 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/enums/v1/batch_operation_pb2.py
+-rw-r--r--   0        0        0     3906 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/enums/v1/batch_operation_pb2.pyi
+-rw-r--r--   0        0        0     3050 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/enums/v1/command_type_pb2.py
+-rw-r--r--   0        0        0     4307 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/enums/v1/command_type_pb2.pyi
+-rw-r--r--   0        0        0     2980 2024-05-07 14:04:43.411591 temporalio-1.6.0/temporalio/api/enums/v1/common_pb2.py
+-rw-r--r--   0        0        0     4571 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/common_pb2.pyi
+-rw-r--r--   0        0        0     6437 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/event_type_pb2.py
+-rw-r--r--   0        0        0    20495 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/event_type_pb2.pyi
+-rw-r--r--   0        0        0     9816 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/failed_cause_pb2.py
+-rw-r--r--   0        0        0    19397 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/failed_cause_pb2.pyi
+-rw-r--r--   0        0        0     2747 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/namespace_pb2.py
+-rw-r--r--   0        0        0     4174 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/namespace_pb2.pyi
+-rw-r--r--   0        0        0     2353 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/query_pb2.py
+-rw-r--r--   0        0        0     3983 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/query_pb2.pyi
+-rw-r--r--   0        0        0     2817 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/reset_pb2.py
+-rw-r--r--   0        0        0     5713 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/reset_pb2.pyi
+-rw-r--r--   0        0        0     2149 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/schedule_pb2.py
+-rw-r--r--   0        0        0     5644 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/schedule_pb2.pyi
+-rw-r--r--   0        0        0     2849 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/task_queue_pb2.py
+-rw-r--r--   0        0        0     7514 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/task_queue_pb2.pyi
+-rw-r--r--   0        0        0     2676 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/update_pb2.py
+-rw-r--r--   0        0        0     6448 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/update_pb2.pyi
+-rw-r--r--   0        0        0     7735 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/workflow_pb2.py
+-rw-r--r--   0        0        0    15052 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/enums/v1/workflow_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/errordetails/__init__.py
+-rw-r--r--   0        0        0     1034 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/errordetails/v1/__init__.py
+-rw-r--r--   0        0        0    12726 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/errordetails/v1/message_pb2.py
+-rw-r--r--   0        0        0    10736 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/errordetails/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/export/__init__.py
+-rw-r--r--   0        0        0      129 2024-05-07 14:04:43.415591 temporalio-1.6.0/temporalio/api/export/v1/__init__.py
+-rw-r--r--   0        0        0     2609 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/export/v1/message_pb2.py
+-rw-r--r--   0        0        0     3010 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/export/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/failure/__init__.py
+-rw-r--r--   0        0        0      530 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/failure/v1/__init__.py
+-rw-r--r--   0        0        0     9303 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/failure/v1/message_pb2.py
+-rw-r--r--   0        0        0    16245 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/failure/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/filter/__init__.py
+-rw-r--r--   0        0        0      236 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/filter/v1/__init__.py
+-rw-r--r--   0        0        0     4015 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/filter/v1/message_pb2.py
+-rw-r--r--   0        0        0     4131 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/filter/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/history/__init__.py
+-rw-r--r--   0        0        0     4730 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/history/v1/__init__.py
+-rw-r--r--   0        0        0    69546 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/history/v1/message_pb2.py
+-rw-r--r--   0        0        0   156397 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/history/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/interaction/__init__.py
+-rw-r--r--   0        0        0      129 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/interaction/v1/__init__.py
+-rw-r--r--   0        0        0     4385 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/interaction/v1/message_pb2.py
+-rw-r--r--   0        0        0     7155 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/interaction/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/namespace/__init__.py
+-rw-r--r--   0        0        0      300 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/namespace/v1/__init__.py
+-rw-r--r--   0        0        0    10181 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/namespace/v1/message_pb2.py
+-rw-r--r--   0        0        0    12925 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/namespace/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/operatorservice/__init__.py
+-rw-r--r--   0        0        0     1423 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/operatorservice/v1/__init__.py
+-rw-r--r--   0        0        0    17707 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/operatorservice/v1/request_response_pb2.py
+-rw-r--r--   0        0        0    15980 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/operatorservice/v1/request_response_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/operatorservice/v1/request_response_pb2_grpc.py
+-rw-r--r--   0        0        0     1185 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/operatorservice/v1/request_response_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3359 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/operatorservice/v1/service_pb2.py
+-rw-r--r--   0        0        0     1274 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/operatorservice/v1/service_pb2.pyi
+-rw-r--r--   0        0        0    17632 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/operatorservice/v1/service_pb2_grpc.py
+-rw-r--r--   0        0        0     8793 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/operatorservice/v1/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/protocol/__init__.py
+-rw-r--r--   0        0        0       63 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/protocol/v1/__init__.py
+-rw-r--r--   0        0        0     2034 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/protocol/v1/message_pb2.py
+-rw-r--r--   0        0        0     3657 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/protocol/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/query/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/query/v1/__init__.py
+-rw-r--r--   0        0        0     3696 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/query/v1/message_pb2.py
+-rw-r--r--   0        0        0     5000 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/query/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/replication/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/replication/v1/__init__.py
+-rw-r--r--   0        0        0     3775 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/replication/v1/message_pb2.py
+-rw-r--r--   0        0        0     4288 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/replication/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/schedule/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/schedule/v1/__init__.py
+-rw-r--r--   0        0        0    16020 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/schedule/v1/message_pb2.py
+-rw-r--r--   0        0        0    39783 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/schedule/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/sdk/__init__.py
+-rw-r--r--   0        0        0      329 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/sdk/v1/__init__.py
+-rw-r--r--   0        0        0     2058 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/sdk/v1/task_complete_metadata_pb2.py
+-rw-r--r--   0        0        0     5122 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/sdk/v1/task_complete_metadata_pb2.pyi
+-rw-r--r--   0        0        0     3542 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/sdk/v1/workflow_metadata_pb2.py
+-rw-r--r--   0        0        0     5971 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/sdk/v1/workflow_metadata_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/taskqueue/__init__.py
+-rw-r--r--   0        0        0      530 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/taskqueue/v1/__init__.py
+-rw-r--r--   0        0        0     8986 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/taskqueue/v1/message_pb2.py
+-rw-r--r--   0        0        0    12733 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/taskqueue/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/testservice/__init__.py
+-rw-r--r--   0        0        0      814 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/testservice/v1/__init__.py
+-rw-r--r--   0        0        0     6584 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/testservice/v1/request_response_pb2.py
+-rw-r--r--   0        0        0     4609 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/testservice/v1/request_response_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/testservice/v1/request_response_pb2_grpc.py
+-rw-r--r--   0        0        0     1185 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/testservice/v1/request_response_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2532 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/testservice/v1/service_pb2.py
+-rw-r--r--   0        0        0     1274 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/testservice/v1/service_pb2.pyi
+-rw-r--r--   0        0        0    14985 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/testservice/v1/service_pb2_grpc.py
+-rw-r--r--   0        0        0     9065 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/testservice/v1/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/update/__init__.py
+-rw-r--r--   0        0        0      308 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/update/v1/__init__.py
+-rw-r--r--   0        0        0     7265 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/update/v1/message_pb2.py
+-rw-r--r--   0        0        0    11509 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/update/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/version/__init__.py
+-rw-r--r--   0        0        0      123 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/version/v1/__init__.py
+-rw-r--r--   0        0        0     3528 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/version/v1/message_pb2.py
+-rw-r--r--   0        0        0     5233 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/version/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflow/__init__.py
+-rw-r--r--   0        0        0      476 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflow/v1/__init__.py
+-rw-r--r--   0        0        0    11283 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflow/v1/message_pb2.py
+-rw-r--r--   0        0        0    25439 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflow/v1/message_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflowservice/__init__.py
+-rw-r--r--   0        0        0     8907 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflowservice/v1/__init__.py
+-rw-r--r--   0        0        0   125363 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflowservice/v1/request_response_pb2.py
+-rw-r--r--   0        0        0   205481 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflowservice/v1/request_response_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflowservice/v1/request_response_pb2_grpc.py
+-rw-r--r--   0        0        0     1185 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflowservice/v1/request_response_pb2_grpc.pyi
+-rw-r--r--   0        0        0    27279 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflowservice/v1/service_pb2.py
+-rw-r--r--   0        0        0     1274 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflowservice/v1/service_pb2.pyi
+-rw-r--r--   0        0        0   136945 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflowservice/v1/service_pb2_grpc.py
+-rw-r--r--   0        0        0    67952 2024-05-07 14:04:43.419591 temporalio-1.6.0/temporalio/api/workflowservice/v1/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0    81780 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/Cargo.lock
+-rw-r--r--   0        0        0      880 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/Cargo.toml
+-rw-r--r--   0        0        0      122 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/__init__.py
+-rw-r--r--   0        0        0     4284 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/client.py
+-rw-r--r--   0        0        0     5177 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/metric.py
+-rw-r--r--   0        0        0      144 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/__init__.py
+-rw-r--r--   0        0        0      336 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/activity_result/__init__.py
+-rw-r--r--   0        0        0     6517 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/activity_result/activity_result_pb2.py
+-rw-r--r--   0        0        0     9319 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/activity_result/activity_result_pb2.pyi
+-rw-r--r--   0        0        0      171 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/activity_task/__init__.py
+-rw-r--r--   0        0        0     5900 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/activity_task/activity_task_pb2.py
+-rw-r--r--   0        0        0    11710 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/activity_task/activity_task_pb2.pyi
+-rw-r--r--   0        0        0     1435 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/bridge/__init__.py
+-rw-r--r--   0        0        0    33694 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/bridge/bridge_pb2.py
+-rw-r--r--   0        0        0    35620 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/bridge/bridge_pb2.pyi
+-rw-r--r--   0        0        0      407 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/child_workflow/__init__.py
+-rw-r--r--   0        0        0     6028 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/child_workflow/child_workflow_pb2.py
+-rw-r--r--   0        0        0     9065 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/child_workflow/child_workflow_pb2.pyi
+-rw-r--r--   0        0        0      144 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/common/__init__.py
+-rw-r--r--   0        0        0     2270 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/common/common_pb2.py
+-rw-r--r--   0        0        0     3473 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/common/common_pb2.pyi
+-rw-r--r--   0        0        0     4340 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/core_interface_pb2.py
+-rw-r--r--   0        0        0     2437 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/core_interface_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/core_interface_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/core_interface_pb2_grpc.pyi
+-rw-r--r--   0        0        0      145 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/external_data/__init__.py
+-rw-r--r--   0        0        0     2882 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/external_data/external_data_pb2.py
+-rw-r--r--   0        0        0     4346 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/external_data/external_data_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/health/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/health/v1/__init__.py
+-rw-r--r--   0        0        0     3055 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/health/v1/health_pb2.py
+-rw-r--r--   0        0        0     2546 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/health/v1/health_pb2.pyi
+-rw-r--r--   0        0        0     1168 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/workflow_activation/__init__.py
+-rw-r--r--   0        0        0    25113 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/workflow_activation/workflow_activation_pb2.py
+-rw-r--r--   0        0        0    49831 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/workflow_activation/workflow_activation_pb2.pyi
+-rw-r--r--   0        0        0     1360 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/workflow_commands/__init__.py
+-rw-r--r--   0        0        0    35980 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/workflow_commands/workflow_commands_pb2.py
+-rw-r--r--   0        0        0    63691 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/workflow_commands/workflow_commands_pb2.pyi
+-rw-r--r--   0        0        0      165 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/workflow_completion/__init__.py
+-rw-r--r--   0        0        0     3971 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/workflow_completion/workflow_completion_pb2.py
+-rw-r--r--   0        0        0     4425 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/proto/workflow_completion/workflow_completion_pb2.pyi
+-rw-r--r--   0        0        0     3792 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/runtime.py
+-rw-r--r--   0        0        0      361 2024-05-07 14:04:44.095594 temporalio-1.6.0/temporalio/bridge/sdk-core/.cargo/config.toml
+-rw-r--r--   0        0        0       39 2024-05-07 14:04:44.091594 temporalio-1.6.0/temporalio/bridge/sdk-core/.git
+-rw-r--r--   0        0        0      802 2024-05-07 14:04:44.095594 temporalio-1.6.0/temporalio/bridge/sdk-core/.github/workflows/heavy.yml
+-rw-r--r--   0        0        0     2552 2024-05-07 14:04:44.095594 temporalio-1.6.0/temporalio/bridge/sdk-core/.github/workflows/per-pr.yml
+-rw-r--r--   0        0        0      281 2024-05-07 14:04:44.095594 temporalio-1.6.0/temporalio/bridge/sdk-core/.gitignore
+-rw-r--r--   0        0        0     7880 2024-05-07 14:04:44.095594 temporalio-1.6.0/temporalio/bridge/sdk-core/ARCHITECTURE.md
+-rw-r--r--   0        0        0       36 2024-05-07 14:04:44.095594 temporalio-1.6.0/temporalio/bridge/sdk-core/CODEOWNERS
+-rw-r--r--   0        0        0      510 2024-05-07 14:04:44.095594 temporalio-1.6.0/temporalio/bridge/sdk-core/Cargo.toml
+-rw-r--r--   0        0        0     1108 2024-05-07 14:04:44.095594 temporalio-1.6.0/temporalio/bridge/sdk-core/LICENSE.txt
+-rw-r--r--   0        0        0     5050 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/README.md
+-rw-r--r--   0        0        0      555 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/arch_docs/diagrams/README.md
+-rw-r--r--   0        0        0     1029 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/arch_docs/diagrams/sticky_queues.puml
+-rw-r--r--   0        0        0   102701 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/arch_docs/diagrams/workflow_internals.svg
+-rw-r--r--   0        0        0     3212 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/arch_docs/sticky_queues.md
+-rwxr-xr-x   0        0        0      109 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/cargo-tokio-console.sh
+-rw-r--r--   0        0        0     1231 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/client/Cargo.toml
+-rw-r--r--   0        0        0    61131 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/client/src/lib.rs
+-rw-r--r--   0        0        0     6600 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/client/src/metrics.rs
+-rw-r--r--   0        0        0     2866 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/client/src/proxy.rs
+-rw-r--r--   0        0        0    38381 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/client/src/raw.rs
+-rw-r--r--   0        0        0    25119 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/client/src/retry.rs
+-rw-r--r--   0        0        0     8729 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/client/src/worker_registry/mod.rs
+-rw-r--r--   0        0        0     7048 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/client/src/workflow_handle/mod.rs
+-rw-r--r--   0        0        0     3957 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/Cargo.toml
+-rw-r--r--   0        0        0     2426 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/benches/workflow_replay.rs
+-rw-r--r--   0        0        0      857 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/abstractions/take_cell.rs
+-rw-r--r--   0        0        0     9524 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/abstractions.rs
+-rw-r--r--   0        0        0    42206 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/activity_tasks.rs
+-rw-r--r--   0        0        0     7987 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/child_workflows.rs
+-rw-r--r--   0        0        0    10831 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/determinism.rs
+-rw-r--r--   0        0        0    48596 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/local_activities.rs
+-rw-r--r--   0        0        0     3150 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/mod.rs
+-rw-r--r--   0        0        0    33815 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/queries.rs
+-rw-r--r--   0        0        0     6292 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/replay_flag.rs
+-rw-r--r--   0        0        0     2484 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/updates.rs
+-rw-r--r--   0        0        0     9470 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/workers.rs
+-rw-r--r--   0        0        0     4233 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/workflow_cancels.rs
+-rw-r--r--   0        0        0   104548 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/workflow_tasks.rs
+-rw-r--r--   0        0        0    17950 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/ephemeral_server/mod.rs
+-rw-r--r--   0        0        0     8887 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/internal_flags.rs
+-rw-r--r--   0        0        0     9731 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/lib.rs
+-rw-r--r--   0        0        0     2529 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/pollers/mod.rs
+-rw-r--r--   0        0        0    12136 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/pollers/poll_buffer.rs
+-rw-r--r--   0        0        0    16323 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/protosext/mod.rs
+-rw-r--r--   0        0        0     3033 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/protosext/protocol_messages.rs
+-rw-r--r--   0        0        0     9405 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/replay/mod.rs
+-rw-r--r--   0        0        0     6553 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/retry_logic.rs
+-rw-r--r--   0        0        0    10387 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/telemetry/log_export.rs
+-rw-r--r--   0        0        0    35566 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/telemetry/metrics.rs
+-rw-r--r--   0        0        0    11090 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/telemetry/mod.rs
+-rw-r--r--   0        0        0    12689 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/telemetry/otel.rs
+-rw-r--r--   0        0        0     3476 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/telemetry/prometheus_server.rs
+-rw-r--r--   0        0        0    34928 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/test_help/mod.rs
+-rw-r--r--   0        0        0    23123 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/activities/activity_heartbeat_manager.rs
+-rw-r--r--   0        0        0     2467 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/activities/activity_task_poller_stream.rs
+-rw-r--r--   0        0        0    54041 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/activities/local_activities.rs
+-rw-r--r--   0        0        0    41768 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/activities.rs
+-rw-r--r--   0        0        0     4640 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/client/mocks.rs
+-rw-r--r--   0        0        0    14527 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/client.rs
+-rw-r--r--   0        0        0    28623 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/mod.rs
+-rw-r--r--   0        0        0     5333 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/slot_provider.rs
+-rw-r--r--   0        0        0     3449 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/driven_workflow.rs
+-rw-r--r--   0        0        0    72595 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/history_update.rs
+-rw-r--r--   0        0        0    33245 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/activity_state_machine.rs
+-rw-r--r--   0        0        0    10536 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/cancel_external_state_machine.rs
+-rw-r--r--   0        0        0     5643 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/cancel_workflow_state_machine.rs
+-rw-r--r--   0        0        0    40852 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/child_workflow_state_machine.rs
+-rw-r--r--   0        0        0     3933 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/complete_workflow_state_machine.rs
+-rw-r--r--   0        0        0     5109 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/continue_as_new_workflow_state_machine.rs
+-rw-r--r--   0        0        0     3736 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/fail_workflow_state_machine.rs
+-rw-r--r--   0        0        0    58406 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/local_activity_state_machine.rs
+-rw-r--r--   0        0        0    11002 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/mod.rs
+-rw-r--r--   0        0        0     5581 2024-05-07 14:04:44.103594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/modify_workflow_properties_state_machine.rs
+-rw-r--r--   0        0        0    32030 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/patch_state_machine.rs
+-rw-r--r--   0        0        0    15974 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/signal_external_state_machine.rs
+-rw-r--r--   0        0        0    13256 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/timer_state_machine.rs
+-rw-r--r--   0        0        0     8040 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/transition_coverage.rs
+-rw-r--r--   0        0        0    14147 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/update_state_machine.rs
+-rw-r--r--   0        0        0    15153 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/upsert_search_attributes_state_machine.rs
+-rw-r--r--   0        0        0     3593 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/workflow_machines/local_acts.rs
+-rw-r--r--   0        0        0    74061 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/workflow_machines.rs
+-rw-r--r--   0        0        0     8305 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/workflow_task_state_machine.rs
+-rw-r--r--   0        0        0    58259 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/managed_run.rs
+-rw-r--r--   0        0        0    55739 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/mod.rs
+-rw-r--r--   0        0        0     4502 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/run_cache.rs
+-rw-r--r--   0        0        0     5539 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/wft_extraction.rs
+-rw-r--r--   0        0        0     4212 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/wft_poller.rs
+-rw-r--r--   0        0        0    28539 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/workflow_stream.rs
+-rw-r--r--   0        0        0      938 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core-api/Cargo.toml
+-rw-r--r--   0        0        0     3198 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core-api/src/errors.rs
+-rw-r--r--   0        0        0     6298 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core-api/src/lib.rs
+-rw-r--r--   0        0        0    13128 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core-api/src/telemetry/metrics.rs
+-rw-r--r--   0        0        0     6577 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core-api/src/telemetry.rs
+-rw-r--r--   0        0        0    10613 2024-05-07 14:04:44.099594 temporalio-1.6.0/temporalio/bridge/sdk-core/core-api/src/worker.rs
+-rw-r--r--   0        0        0      963 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/docker/docker-compose-telem.yaml
+-rw-r--r--   0        0        0      839 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/docker/docker-compose.yaml
+-rw-r--r--   0        0        0     7987 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/etc/deps.svg
+-rw-r--r--   0        0        0      332 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/etc/dynamic-config.yaml
+-rw-r--r--   0        0        0      574 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/etc/otel-collector-config.yaml
+-rw-r--r--   0        0        0      173 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/etc/prometheus.yaml
+-rwxr-xr-x   0        0        0      204 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/etc/regen-depgraph.sh
+-rw-r--r--   0        0        0      600 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/Cargo.toml
+-rw-r--r--   0        0        0     1108 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/LICENSE.txt
+-rw-r--r--   0        0        0      126 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/README.md
+-rw-r--r--   0        0        0      623 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/Cargo.toml
+-rw-r--r--   0        0        0     1108 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/LICENSE.txt
+-rw-r--r--   0        0        0    26182 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/src/lib.rs
+-rw-r--r--   0        0        0      191 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/progress.rs
+-rw-r--r--   0        0        0      299 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/dupe_transitions_fail.rs
+-rw-r--r--   0        0        0      387 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/dupe_transitions_fail.stderr
+-rw-r--r--   0        0        0      892 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/dynamic_dest_pass.rs
+-rw-r--r--   0        0        0      202 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/forgot_name_fail.rs
+-rw-r--r--   0        0        0      331 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/forgot_name_fail.stderr
+-rw-r--r--   0        0        0      686 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/handler_arg_pass.rs
+-rw-r--r--   0        0        0      619 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/handler_pass.rs
+-rw-r--r--   0        0        0      862 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/medium_complex_pass.rs
+-rw-r--r--   0        0        0      584 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/no_handle_conversions_require_into_fail.rs
+-rw-r--r--   0        0        0      733 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/no_handle_conversions_require_into_fail.stderr
+-rw-r--r--   0        0        0      649 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/simple_pass.rs
+-rw-r--r--   0        0        0      307 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/struct_event_variant_fail.rs
+-rw-r--r--   0        0        0      161 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/struct_event_variant_fail.stderr
+-rw-r--r--   0        0        0      184 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/tuple_more_item_event_variant_fail.rs
+-rw-r--r--   0        0        0      189 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/tuple_more_item_event_variant_fail.stderr
+-rw-r--r--   0        0        0      176 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/tuple_zero_item_event_variant_fail.rs
+-rw-r--r--   0        0        0      181 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/tuple_zero_item_event_variant_fail.stderr
+-rw-r--r--   0        0        0      366 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_trait/Cargo.toml
+-rw-r--r--   0        0        0     1108 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_trait/LICENSE.txt
+-rw-r--r--   0        0        0     6524 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_trait/src/lib.rs
+-rw-r--r--   0        0        0      103 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/src/lib.rs
+-rw-r--r--   0        0        0     1206 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/histories/ends_empty_wft_complete.bin
+-rw-r--r--   0        0        0     1853 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/histories/evict_while_la_running_no_interference-16_history.bin
+-rw-r--r--   0        0        0     3277 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/histories/evict_while_la_running_no_interference-23_history.bin
+-rw-r--r--   0        0        0     2532 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/histories/evict_while_la_running_no_interference-85_history.bin
+-rw-r--r--   0        0        0      924 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/histories/fail_wf_task.bin
+-rw-r--r--   0        0        0     1701 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/histories/old_change_marker_format.bin
+-rw-r--r--   0        0        0      711 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/histories/timer_workflow_history.bin
+-rwxr-xr-x   0        0        0      213 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/integ-with-otel.sh
+-rw-r--r--   0        0        0       27 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/rustfmt.toml
+-rw-r--r--   0        0        0     1242 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/Cargo.toml
+-rw-r--r--   0        0        0     8019 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/activity_context.rs
+-rw-r--r--   0        0        0     1000 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/app_data.rs
+-rw-r--r--   0        0        0     1789 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/interceptors.rs
+-rw-r--r--   0        0        0    34815 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/lib.rs
+-rw-r--r--   0        0        0    12111 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/workflow_context/options.rs
+-rw-r--r--   0        0        0    25442 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/workflow_context.rs
+-rw-r--r--   0        0        0    28095 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/workflow_future.rs
+-rw-r--r--   0        0        0      931 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/Cargo.toml
+-rw-r--r--   0        0        0     5052 2024-05-07 14:04:44.107594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/build.rs
+-rw-r--r--   0        0        0       57 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.buildkite/Dockerfile
+-rw-r--r--   0        0        0      336 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.buildkite/docker-compose.yml
+-rw-r--r--   0        0        0      223 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.buildkite/pipeline.yml
+-rw-r--r--   0        0        0      234 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.github/CODEOWNERS
+-rw-r--r--   0        0        0      227 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      587 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.github/workflows/publish-docs.yml
+-rw-r--r--   0        0        0     1097 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.github/workflows/trigger-api-go-update.yml
+-rw-r--r--   0        0        0       32 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.gitignore
+-rw-r--r--   0        0        0     1108 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/LICENSE
+-rw-r--r--   0        0        0     2882 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/Makefile
+-rw-r--r--   0        0        0      151 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/README.md
+-rw-r--r--   0        0        0     1760 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/api-linter.yaml
+-rw-r--r--   0        0        0      470 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/buf.gen.yaml
+-rw-r--r--   0        0        0      289 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/buf.lock
+-rw-r--r--   0        0        0      333 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/buf.yaml
+-rw-r--r--   0        0        0     1045 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/api/annotations.proto
+-rw-r--r--   0        0        0    15159 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/api/http.proto
+-rw-r--r--   0        0        0     6153 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/any.proto
+-rw-r--r--   0        0        0    49556 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/descriptor.proto
+-rw-r--r--   0        0        0     4891 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/duration.proto
+-rw-r--r--   0        0        0     2363 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/empty.proto
+-rw-r--r--   0        0        0     6448 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/timestamp.proto
+-rw-r--r--   0        0        0     4043 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/wrappers.proto
+-rw-r--r--   0        0        0     4369 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/batch/v1/message.proto
+-rw-r--r--   0        0        0    12821 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/command/v1/message.proto
+-rw-r--r--   0        0        0     7856 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/common/v1/message.proto
+-rw-r--r--   0        0        0     1950 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/batch_operation.proto
+-rw-r--r--   0        0        0     2465 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/command_type.proto
+-rw-r--r--   0        0        0     2062 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/common.proto
+-rw-r--r--   0        0        0    10063 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/event_type.proto
+-rw-r--r--   0        0        0     7346 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/failed_cause.proto
+-rw-r--r--   0        0        0     1944 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/namespace.proto
+-rw-r--r--   0        0        0     2098 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/query.proto
+-rw-r--r--   0        0        0     2848 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/reset.proto
+-rw-r--r--   0        0        0     3212 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/schedule.proto
+-rw-r--r--   0        0        0     3715 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/task_queue.proto
+-rw-r--r--   0        0        0     3524 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/update.proto
+-rw-r--r--   0        0        0     5083 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/workflow.proto
+-rw-r--r--   0        0        0     3957 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/errordetails/v1/message.proto
+-rw-r--r--   0        0        0     1884 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/export/v1/message.proto
+-rw-r--r--   0        0        0     4728 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/failure/v1/message.proto
+-rw-r--r--   0        0        0     1965 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/filter/v1/message.proto
+-rw-r--r--   0        0        0    42913 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/history/v1/message.proto
+-rw-r--r--   0        0        0     3917 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/namespace/v1/message.proto
+-rw-r--r--   0        0        0     4462 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/operatorservice/v1/request_response.proto
+-rw-r--r--   0        0        0     4190 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/operatorservice/v1/service.proto
+-rw-r--r--   0        0        0     2427 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/protocol/v1/message.proto
+-rw-r--r--   0        0        0     2587 2024-05-07 14:04:44.111594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/query/v1/message.proto
+-rw-r--r--   0        0        0     2138 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/replication/v1/message.proto
+-rw-r--r--   0        0        0    17755 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/schedule/v1/message.proto
+-rw-r--r--   0        0        0     3871 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/sdk/v1/task_complete_metadata.proto
+-rw-r--r--   0        0        0     3072 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/sdk/v1/workflow_metadata.proto
+-rw-r--r--   0        0        0     4361 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/taskqueue/v1/message.proto
+-rw-r--r--   0        0        0     3984 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/update/v1/message.proto
+-rw-r--r--   0        0        0     2265 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/version/v1/message.proto
+-rw-r--r--   0        0        0     7002 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/workflow/v1/message.proto
+-rw-r--r--   0        0        0    61128 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/workflowservice/v1/request_response.proto
+-rw-r--r--   0        0        0    30601 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/workflowservice/v1/service.proto
+-rw-r--r--   0        0        0     2069 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/google/rpc/status.proto
+-rw-r--r--   0        0        0     2416 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/grpc/health/v1/health.proto
+-rw-r--r--   0        0        0     2716 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/activity_result/activity_result.proto
+-rw-r--r--   0        0        0     3066 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/activity_task/activity_task.proto
+-rw-r--r--   0        0        0     2322 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/child_workflow/child_workflow.proto
+-rw-r--r--   0        0        0     1260 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/common/common.proto
+-rw-r--r--   0        0        0     1313 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/core_interface.proto
+-rw-r--r--   0        0        0     1726 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/external_data/external_data.proto
+-rw-r--r--   0        0        0    15760 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/workflow_activation/workflow_activation.proto
+-rw-r--r--   0        0        0    16340 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/workflow_commands/workflow_commands.proto
+-rw-r--r--   0        0        0     1230 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/workflow_completion/workflow_completion.proto
+-rw-r--r--   0        0        0     2139 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/Makefile
+-rw-r--r--   0        0        0     1029 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/api-linter.yaml
+-rw-r--r--   0        0        0      137 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/buf.yaml
+-rw-r--r--   0        0        0     2043 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/temporal/api/testservice/v1/request_response.proto
+-rw-r--r--   0        0        0     4494 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/temporal/api/testservice/v1/service.proto
+-rw-r--r--   0        0        0      334 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/src/constants.rs
+-rw-r--r--   0        0        0    23461 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/src/history_builder.rs
+-rw-r--r--   0        0        0     9321 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/src/history_info.rs
+-rw-r--r--   0        0        0    91944 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/src/lib.rs
+-rw-r--r--   0        0        0     1426 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/src/task_token.rs
+-rw-r--r--   0        0        0      844 2024-05-07 14:04:44.115594 temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/src/utilities.rs
+-rw-r--r--   0        0        0      984 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/test-utils/Cargo.toml
+-rw-r--r--   0        0        0    48345 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/test-utils/src/canned_histories.rs
+-rw-r--r--   0        0        0     1085 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/test-utils/src/histfetch.rs
+-rw-r--r--   0        0        0     1366 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/test-utils/src/interceptors.rs
+-rw-r--r--   0        0        0    29019 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/test-utils/src/lib.rs
+-rw-r--r--   0        0        0     1148 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/test-utils/src/workflows.rs
+-rw-r--r--   0        0        0     4751 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/fuzzy_workflow.rs
+-rw-r--r--   0        0        0     8767 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/heavy_tests.rs
+-rw-r--r--   0        0        0      125 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/activity_functions.rs
+-rw-r--r--   0        0        0     1341 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/client_tests.rs
+-rw-r--r--   0        0        0     4722 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/ephemeral_server_tests.rs
+-rw-r--r--   0        0        0     8263 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/heartbeat_tests.rs
+-rw-r--r--   0        0        0    19743 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/metrics_tests.rs
+-rw-r--r--   0        0        0     7518 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/polling_tests.rs
+-rw-r--r--   0        0        0    17683 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/queries_tests.rs
+-rw-r--r--   0        0        0    31235 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/update_tests.rs
+-rw-r--r--   0        0        0     5049 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/visibility_tests.rs
+-rw-r--r--   0        0        0    36658 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/activities.rs
+-rw-r--r--   0        0        0     2003 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/appdata_propagation.rs
+-rw-r--r--   0        0        0     1713 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/cancel_external.rs
+-rw-r--r--   0        0        0     1625 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/cancel_wf.rs
+-rw-r--r--   0        0        0     6265 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/child_workflows.rs
+-rw-r--r--   0        0        0     1986 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/continue_as_new.rs
+-rw-r--r--   0        0        0     1636 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/determinism.rs
+-rw-r--r--   0        0        0     2135 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/eager.rs
+-rw-r--r--   0        0        0    24790 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/local_activities.rs
+-rw-r--r--   0        0        0     1616 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/modify_wf_properties.rs
+-rw-r--r--   0        0        0     7152 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/patches.rs
+-rw-r--r--   0        0        0    10648 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/replay.rs
+-rw-r--r--   0        0        0     3038 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/resets.rs
+-rw-r--r--   0        0        0     5277 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/signals.rs
+-rw-r--r--   0        0        0     3059 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/stickyness.rs
+-rw-r--r--   0        0        0     3913 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/timers.rs
+-rw-r--r--   0        0        0     2614 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/upsert_search_attrs.rs
+-rw-r--r--   0        0        0    28694 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests.rs
+-rw-r--r--   0        0        0     3389 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/main.rs
+-rw-r--r--   0        0        0     4461 2024-05-07 14:04:44.119594 temporalio-1.6.0/temporalio/bridge/sdk-core/tests/runner.rs
+-rw-r--r--   0        0        0    19045 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/src/client.rs
+-rw-r--r--   0        0        0     3294 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/src/lib.rs
+-rw-r--r--   0        0        0    13298 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/src/metric.rs
+-rw-r--r--   0        0        0    13677 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/src/runtime.rs
+-rw-r--r--   0        0        0     5587 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/src/testing.rs
+-rw-r--r--   0        0        0    12359 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/src/worker.rs
+-rw-r--r--   0        0        0     2384 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/testing.py
+-rw-r--r--   0        0        0    13720 2024-05-07 14:04:43.423591 temporalio-1.6.0/temporalio/bridge/worker.py
+-rw-r--r--   0        0        0   220007 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/client.py
+-rw-r--r--   0        0        0    33982 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/common.py
+-rw-r--r--   0        0        0       57 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/contrib/__init__.py
+-rw-r--r--   0        0        0    27336 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/contrib/opentelemetry.py
+-rw-r--r--   0        0        0    59640 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/converter.py
+-rw-r--r--   0        0        0    10663 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/py.typed
+-rw-r--r--   0        0        0    23896 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/runtime.py
+-rw-r--r--   0        0        0    31406 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/service.py
+-rw-r--r--   0        0        0      207 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/testing/__init__.py
+-rw-r--r--   0        0        0     7345 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/testing/_activity.py
+-rw-r--r--   0        0        0    23571 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/testing/_workflow.py
+-rw-r--r--   0        0        0     4443 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/types.py
+-rw-r--r--   0        0        0     1880 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/worker/__init__.py
+-rw-r--r--   0        0        0    40083 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/worker/_activity.py
+-rw-r--r--   0        0        0    13085 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/worker/_interceptor.py
+-rw-r--r--   0        0        0    14261 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/worker/_replayer.py
+-rw-r--r--   0        0        0    36097 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/worker/_worker.py
+-rw-r--r--   0        0        0    18039 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/worker/_workflow.py
+-rw-r--r--   0        0        0   105905 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/worker/_workflow_instance.py
+-rw-r--r--   0        0        0     2481 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/worker/workflow_sandbox/__init__.py
+-rw-r--r--   0        0        0    17707 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/worker/workflow_sandbox/_importer.py
+-rw-r--r--   0        0        0     3336 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/worker/workflow_sandbox/_in_sandbox.py
+-rw-r--r--   0        0        0    40485 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/worker/workflow_sandbox/_restrictions.py
+-rw-r--r--   0        0        0     7034 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/worker/workflow_sandbox/_runner.py
+-rw-r--r--   0        0        0   159946 2024-05-07 14:04:43.427591 temporalio-1.6.0/temporalio/workflow.py
+-rw-r--r--   0        0        0    81320 1970-01-01 00:00:00.000000 temporalio-1.6.0/setup.py
+-rw-r--r--   0        0        0    71474 1970-01-01 00:00:00.000000 temporalio-1.6.0/PKG-INFO
```

### Comparing `temporalio-1.5.1/LICENSE` & `temporalio-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/README.md` & `temporalio-1.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -718,24 +718,32 @@
 * `continue_as_new()` - Async function to stop the workflow immediately and continue as new
 * `info()` - Returns information about the current workflow
 * `logger` - A logger for use in a workflow (properly skips logging on replay)
 * `now()` - Returns the "current time" from the workflow's perspective
 
 #### Exceptions
 
-* Workflows can raise exceptions to fail the workflow or the "workflow task" (i.e. suspend the workflow retrying).
+* Workflows/updates can raise exceptions to fail the workflow or the "workflow task" (i.e. suspend the workflow
+  in a retrying state).
 * Exceptions that are instances of `temporalio.exceptions.FailureError` will fail the workflow with that exception
   * For failing the workflow explicitly with a user exception, use `temporalio.exceptions.ApplicationError`. This can
     be marked non-retryable or include details as needed.
   * Other exceptions that come from activity execution, child execution, cancellation, etc are already instances of
     `FailureError` and will fail the workflow when uncaught.
 * All other exceptions fail the "workflow task" which means the workflow will continually retry until the workflow is
   fixed. This is helpful for bad code or other non-predictable exceptions. To actually fail the workflow, use an
   `ApplicationError` as mentioned above.
 
+This default can be changed by providing a list of exception types to `workflow_failure_exception_types` when creating a
+`Worker` or `failure_exception_types` on the `@workflow.defn` decorator. If a workflow-thrown exception is an instance
+of any type in either list, it will fail the workflow instead of the task. This means a value of `[Exception]` will
+cause every exception to fail the workflow instead of the task. Also, as a special case, if
+`temporalio.workflow.NondeterminismError` (or any superclass of it) is set, non-deterministic exceptions will fail the
+workflow. WARNING: These settings are experimental.
+
 #### External Workflows
 
 * `workflow.get_external_workflow_handle()` inside a workflow returns a handle to interact with another workflow
 * `workflow.get_external_workflow_handle_for()` can be used instead for a type safe handle
 * `await handle.signal()` can be called on the handle to signal the external workflow
 * `await handle.cancel()` can be called on the handle to send a cancel to the external workflow
```

### Comparing `temporalio-1.5.1/build.py` & `temporalio-1.6.0/build.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/pyproject.toml` & `temporalio-1.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "temporalio"
-version = "1.5.1"
+version = "1.6.0"
 description = "Temporal.io Python SDK"
 license = "MIT"
 authors = ["Temporal Technologies Inc <sdk@temporal.io>"]
 readme = "README.md"
 homepage = "https://github.com/temporalio/sdk-python"
 repository = "https://github.com/temporalio/sdk-python"
 documentation = "https://docs.temporal.io/docs/python"
@@ -38,15 +38,15 @@
 python = "^3.8"
 python-dateutil = { version = "^2.8.2", python = "<3.11" }
 types-protobuf = ">=3.20"
 typing-extensions = "^4.2.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
-cibuildwheel = "^2.16.0"
+cibuildwheel = "^2.17.0"
 grpcio-tools = "^1.48.0"
 isort = "^5.11.5"
 mypy = "^1.0.0"
 mypy-protobuf = "^3.3.0"
 protoc-wheel-0 = "^21.1"
 psutil = "^5.9.3"
 pydantic = "^1.9.1"
@@ -106,16 +106,19 @@
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 testpaths = ["tests"]
 timeout = 600
 timeout_func_only = true
 
 [tool.cibuildwheel]
-# We only want the 3.8 64-bit build of each type
-build = "cp38-win_amd64 cp38-manylinux_x86_64 cp38-manylinux_aarch64 cp38-macosx_x86_64 cp38-macosx_arm64"
+# We only want the 3.8 64-bit build of each type. However, due to
+# https://github.com/pypa/cibuildwheel/issues/1278, we have to build macOS as
+# 3.9 until that is fixed. Our fix-wheel process will rename it to 3.8 and we
+# have manually confirmed this works with 3.8.
+build = "cp38-win_amd64 cp38-manylinux_x86_64 cp38-manylinux_aarch64 cp38-macosx_x86_64 cp39-macosx_arm64"
 build-verbosity = "1"
 
 [tool.cibuildwheel.linux]
 before-all = "curl https://sh.rustup.rs -sSf | sh -s -- --default-toolchain stable -y && yum install -y openssl-devel"
 environment = { PATH = "$PATH:$HOME/.cargo/bin", CARGO_NET_GIT_FETCH_WITH_CLI = "true" }
 
 [tool.isort]
```

### Comparing `temporalio-1.5.1/temporalio/activity.py` & `temporalio-1.6.0/temporalio/activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -423,39 +423,54 @@
 class LoggerAdapter(logging.LoggerAdapter):
     """Adapter that adds details to the log about the running activity.
 
     Attributes:
         activity_info_on_message: Boolean for whether a string representation of
             a dict of some activity info will be appended to each message.
             Default is True.
-        activity_info_on_extra: Boolean for whether an ``activity_info`` value
-            will be added to the ``extra`` dictionary, making it present on the
-            ``LogRecord.__dict__`` for use by others.
+        activity_info_on_extra: Boolean for whether a ``temporal_activity``
+            dictionary value will be added to the ``extra`` dictionary with some
+            activity info, making it present on the ``LogRecord.__dict__`` for
+            use by others. Default is True.
+        full_activity_info_on_extra: Boolean for whether an ``activity_info``
+            value will be added to the ``extra`` dictionary with the entire
+            activity info, making it present on the ``LogRecord.__dict__`` for
+            use by others. Default is False.
     """
 
     def __init__(
         self, logger: logging.Logger, extra: Optional[Mapping[str, Any]]
     ) -> None:
         """Create the logger adapter."""
         super().__init__(logger, extra or {})
         self.activity_info_on_message = True
         self.activity_info_on_extra = True
+        self.full_activity_info_on_extra = False
 
     def process(
         self, msg: Any, kwargs: MutableMapping[str, Any]
     ) -> Tuple[Any, MutableMapping[str, Any]]:
         """Override to add activity details."""
-        if self.activity_info_on_message or self.activity_info_on_extra:
+        if (
+            self.activity_info_on_message
+            or self.activity_info_on_extra
+            or self.full_activity_info_on_extra
+        ):
             context = _current_context.get(None)
             if context:
                 if self.activity_info_on_message:
                     msg = f"{msg} ({context.logger_details})"
                 if self.activity_info_on_extra:
                     # Extra can be absent or None, this handles both
                     extra = kwargs.get("extra", None) or {}
+                    extra["temporal_activity"] = context._logger_details
+                    kwargs["extra"] = extra
+                if self.full_activity_info_on_extra:
+                    # Extra can be absent or None, this handles both
+                    extra = kwargs.get("extra", None) or {}
                     extra["activity_info"] = context.info()
                     kwargs["extra"] = extra
         return (msg, kwargs)
 
     @property
     def base_logger(self) -> logging.Logger:
         """Underlying logger usable for actions such as adding
```

### Comparing `temporalio-1.5.1/temporalio/api/batch/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/batch/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/batch/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/batch/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/cluster/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/cluster/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/cluster/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/cluster/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/cluster/v1/message_pb2_grpc.pyi` & `temporalio-1.6.0/temporalio/api/cluster/v1/message_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/command/v1/__init__.py` & `temporalio-1.6.0/temporalio/api/command/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/command/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/command/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/command/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/command/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/common/v1/__init__.py` & `temporalio-1.6.0/temporalio/api/common/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/common/v1/grpc_status_pb2.py` & `temporalio-1.6.0/temporalio/api/common/v1/grpc_status_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/common/v1/grpc_status_pb2.pyi` & `temporalio-1.6.0/temporalio/api/common/v1/grpc_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/common/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/common/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/common/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/common/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/__init__.py` & `temporalio-1.6.0/temporalio/api/enums/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/batch_operation_pb2.py` & `temporalio-1.6.0/temporalio/api/enums/v1/batch_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/batch_operation_pb2.pyi` & `temporalio-1.6.0/temporalio/api/enums/v1/batch_operation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/command_type_pb2.py` & `temporalio-1.6.0/temporalio/api/enums/v1/command_type_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/command_type_pb2.pyi` & `temporalio-1.6.0/temporalio/api/enums/v1/command_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/common_pb2.py` & `temporalio-1.6.0/temporalio/api/enums/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/common_pb2.pyi` & `temporalio-1.6.0/temporalio/api/enums/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/event_type_pb2.py` & `temporalio-1.6.0/temporalio/api/enums/v1/event_type_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/event_type_pb2.pyi` & `temporalio-1.6.0/temporalio/api/enums/v1/event_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/failed_cause_pb2.py` & `temporalio-1.6.0/temporalio/api/enums/v1/failed_cause_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/failed_cause_pb2.pyi` & `temporalio-1.6.0/temporalio/api/enums/v1/failed_cause_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/namespace_pb2.py` & `temporalio-1.6.0/temporalio/api/enums/v1/namespace_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/namespace_pb2.pyi` & `temporalio-1.6.0/temporalio/api/enums/v1/namespace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/query_pb2.py` & `temporalio-1.6.0/temporalio/api/enums/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/query_pb2.pyi` & `temporalio-1.6.0/temporalio/api/enums/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/reset_pb2.py` & `temporalio-1.6.0/temporalio/api/enums/v1/reset_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/reset_pb2.pyi` & `temporalio-1.6.0/temporalio/api/enums/v1/reset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/schedule_pb2.py` & `temporalio-1.6.0/temporalio/api/enums/v1/schedule_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/schedule_pb2.pyi` & `temporalio-1.6.0/temporalio/api/enums/v1/schedule_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/task_queue_pb2.py` & `temporalio-1.6.0/temporalio/api/enums/v1/task_queue_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/task_queue_pb2.pyi` & `temporalio-1.6.0/temporalio/api/enums/v1/task_queue_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/update_pb2.py` & `temporalio-1.6.0/temporalio/api/enums/v1/update_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/update_pb2.pyi` & `temporalio-1.6.0/temporalio/api/enums/v1/update_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/workflow_pb2.py` & `temporalio-1.6.0/temporalio/api/enums/v1/workflow_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/enums/v1/workflow_pb2.pyi` & `temporalio-1.6.0/temporalio/api/enums/v1/workflow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/errordetails/v1/__init__.py` & `temporalio-1.6.0/temporalio/api/errordetails/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/errordetails/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/errordetails/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/errordetails/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/errordetails/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/export/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/export/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/export/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/export/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/failure/v1/__init__.py` & `temporalio-1.6.0/temporalio/api/failure/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/failure/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/failure/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/failure/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/failure/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/filter/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/filter/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/filter/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/filter/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/history/v1/__init__.py` & `temporalio-1.6.0/temporalio/api/history/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/history/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/history/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/history/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/history/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/interaction/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/interaction/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/interaction/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/interaction/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/namespace/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/namespace/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/namespace/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/namespace/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/operatorservice/v1/__init__.py` & `temporalio-1.6.0/temporalio/api/operatorservice/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/operatorservice/v1/request_response_pb2.py` & `temporalio-1.6.0/temporalio/api/operatorservice/v1/request_response_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/operatorservice/v1/request_response_pb2.pyi` & `temporalio-1.6.0/temporalio/api/operatorservice/v1/request_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/operatorservice/v1/request_response_pb2_grpc.pyi` & `temporalio-1.6.0/temporalio/api/operatorservice/v1/request_response_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/operatorservice/v1/service_pb2.py` & `temporalio-1.6.0/temporalio/api/operatorservice/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/operatorservice/v1/service_pb2.pyi` & `temporalio-1.6.0/temporalio/api/operatorservice/v1/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/operatorservice/v1/service_pb2_grpc.py` & `temporalio-1.6.0/temporalio/api/operatorservice/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/operatorservice/v1/service_pb2_grpc.pyi` & `temporalio-1.6.0/temporalio/api/operatorservice/v1/service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/protocol/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/protocol/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/protocol/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/protocol/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/query/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/query/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/query/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/query/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/replication/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/replication/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/replication/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/replication/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/schedule/v1/__init__.py` & `temporalio-1.6.0/temporalio/api/schedule/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/schedule/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/schedule/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/schedule/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/schedule/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/sdk/v1/task_complete_metadata_pb2.py` & `temporalio-1.6.0/temporalio/api/sdk/v1/task_complete_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/sdk/v1/task_complete_metadata_pb2.pyi` & `temporalio-1.6.0/temporalio/api/sdk/v1/task_complete_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/sdk/v1/workflow_metadata_pb2.py` & `temporalio-1.6.0/temporalio/api/sdk/v1/workflow_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/sdk/v1/workflow_metadata_pb2.pyi` & `temporalio-1.6.0/temporalio/api/sdk/v1/workflow_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/taskqueue/v1/__init__.py` & `temporalio-1.6.0/temporalio/api/taskqueue/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/taskqueue/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/taskqueue/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/taskqueue/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/taskqueue/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/testservice/v1/__init__.py` & `temporalio-1.6.0/temporalio/api/testservice/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/testservice/v1/request_response_pb2.py` & `temporalio-1.6.0/temporalio/api/testservice/v1/request_response_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/testservice/v1/request_response_pb2.pyi` & `temporalio-1.6.0/temporalio/api/testservice/v1/request_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/testservice/v1/request_response_pb2_grpc.pyi` & `temporalio-1.6.0/temporalio/api/testservice/v1/request_response_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/testservice/v1/service_pb2.py` & `temporalio-1.6.0/temporalio/api/testservice/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/testservice/v1/service_pb2.pyi` & `temporalio-1.6.0/temporalio/api/testservice/v1/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/testservice/v1/service_pb2_grpc.py` & `temporalio-1.6.0/temporalio/api/testservice/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/testservice/v1/service_pb2_grpc.pyi` & `temporalio-1.6.0/temporalio/api/testservice/v1/service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/update/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/update/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/update/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/update/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/version/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/version/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/version/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/version/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/workflow/v1/message_pb2.py` & `temporalio-1.6.0/temporalio/api/workflow/v1/message_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/workflow/v1/message_pb2.pyi` & `temporalio-1.6.0/temporalio/api/workflow/v1/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/workflowservice/v1/__init__.py` & `temporalio-1.6.0/temporalio/api/workflowservice/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/workflowservice/v1/request_response_pb2.py` & `temporalio-1.6.0/temporalio/api/workflowservice/v1/request_response_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/workflowservice/v1/request_response_pb2.pyi` & `temporalio-1.6.0/temporalio/api/workflowservice/v1/request_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/workflowservice/v1/request_response_pb2_grpc.pyi` & `temporalio-1.6.0/temporalio/api/workflowservice/v1/request_response_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/workflowservice/v1/service_pb2.py` & `temporalio-1.6.0/temporalio/api/workflowservice/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/workflowservice/v1/service_pb2.pyi` & `temporalio-1.6.0/temporalio/api/workflowservice/v1/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/workflowservice/v1/service_pb2_grpc.py` & `temporalio-1.6.0/temporalio/api/workflowservice/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/api/workflowservice/v1/service_pb2_grpc.pyi` & `temporalio-1.6.0/temporalio/api/workflowservice/v1/service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/Cargo.lock` & `temporalio-1.6.0/temporalio/bridge/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -52,24 +52,24 @@
 [[package]]
 name = "allocator-api2"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
 
 [[package]]
-name = "anyhow"
-version = "1.0.79"
+name = "anstyle"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "080e9890a082662b09c1ad45f567faeeb47f22b5fb23895fbe1e651e718e25ca"
+checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
 
 [[package]]
-name = "arc-swap"
-version = "1.6.0"
+name = "anyhow"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
+checksum = "080e9890a082662b09c1ad45f567faeeb47f22b5fb23895fbe1e651e718e25ca"
 
 [[package]]
 name = "async-stream"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd56dd203fef61ac097dd65721a419ddccb106b2d2b70ba60a6b529f03961a51"
 dependencies = [
@@ -113,17 +113,17 @@
 checksum = "3b829e4e32b91e643de6eafe82b1d90675f5874230191a4ffbc1b336dec4d6bf"
 dependencies = [
  "async-trait",
  "axum-core",
  "bitflags 1.3.2",
  "bytes",
  "futures-util",
- "http",
- "http-body",
- "hyper",
+ "http 0.2.11",
+ "http-body 0.4.6",
+ "hyper 0.14.28",
  "itoa",
  "matchit",
  "memchr",
  "mime",
  "percent-encoding",
  "pin-project-lite",
  "rustversion",
@@ -139,16 +139,16 @@
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "759fa577a247914fd3f7f76d62972792636412fbfd634cd452f6a385a74d2d2c"
 dependencies = [
  "async-trait",
  "bytes",
  "futures-util",
- "http",
- "http-body",
+ "http 0.2.11",
+ "http-body 0.4.6",
  "mime",
  "rustversion",
  "tower-layer",
  "tower-service",
 ]
 
 [[package]]
@@ -175,17 +175,17 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
-version = "0.21.6"
+version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c79fed4cdb43e993fcdadc7e58a09fd0e3e649c4436fa11da71c9f1f3ee7feb9"
+checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "base64ct"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
 
@@ -262,14 +262,20 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "cfg_aliases"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
+
+[[package]]
 name = "chrono"
 version = "0.4.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f2c685bad3eb3d45a01354cedb7d5faa66194d1d58ba6e267a8de788f79db38"
 dependencies = [
  "num-traits",
  "serde",
@@ -363,45 +369,45 @@
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
 name = "darling"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
+checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
 dependencies = [
  "darling_core",
  "darling_macro",
 ]
 
 [[package]]
 name = "darling_core"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "109c1ca6e6b7f82cc233a97004ea8ed7ca123a9af07a8230878fcfda9b158bf0"
+checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
- "syn 1.0.109",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "darling_macro"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
+checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
 dependencies = [
  "darling_core",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "dashmap"
 version = "5.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978747c1d849a7d2ee5e8adc0159961c48fb7e5db2f06af6723b80123bb53856"
@@ -420,41 +426,41 @@
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
 
 [[package]]
 name = "derive_builder"
-version = "0.12.0"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d67778784b508018359cbc8696edb3db78160bab2c2a28ba7f56ef6932997f8"
+checksum = "0350b5cb0331628a5916d6c5c0b72e97393b8b6b03b47a9284f4e7f5a405ffd7"
 dependencies = [
  "derive_builder_macro",
 ]
 
 [[package]]
 name = "derive_builder_core"
-version = "0.12.0"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c11bdc11a0c47bc7d37d582b5285da6849c96681023680b906673c5707af7b0f"
+checksum = "d48cda787f839151732d396ac69e3473923d54312c070ee21e9effcaa8ca0b1d"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "derive_builder_macro"
-version = "0.12.0"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ebcda35c7a396850a55ffeac740804b40ffec779b98fffbb1738f4033f0ee79e"
+checksum = "206868b8242f27cecce124c19fd88157fbd0dd334df2587f36417bafbc85097b"
 dependencies = [
  "derive_builder_core",
- "syn 1.0.109",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
@@ -463,20 +469,14 @@
  "proc-macro2",
  "quote",
  "rustc_version",
  "syn 1.0.109",
 ]
 
 [[package]]
-name = "difflib"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6184e33543162437515c2e2b48714794e37845ec9851711914eec9d308f6ebe8"
-
-[[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
@@ -502,26 +502,26 @@
 checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "enum-iterator"
-version = "1.4.1"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7add3873b5dd076766ee79c8e406ad1a472c385476b9e38849f8eec24f1be689"
+checksum = "600536cfe9e2da0820aa498e570f6b2b9223eec3ce2f835c8ae4861304fa4794"
 dependencies = [
  "enum-iterator-derive",
 ]
 
 [[package]]
 name = "enum-iterator-derive"
-version = "1.2.1"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eecf8589574ce9b895052fa12d69af7a233f99e6107f5cb8dd1044f2a17bfdcb"
+checksum = "03cdc46ec28bd728e67540c528013c6a10eb69a02eb31078a1bda695438cbfb8"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
@@ -592,23 +592,14 @@
 checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
-name = "float-cmp"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98de4bbd547a563b716d8dfa9aad1cb19bfab00f4fa09a6a4ed21dbcf44ce9c4"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "form_urlencoded"
@@ -780,24 +771,43 @@
  "quanta",
  "rand",
  "smallvec",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.22"
+version = "0.3.24"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bb2c4422095b67ee78da96fbb51a4cc413b3b25883c7717ff7ca1ab31022c9c9"
+dependencies = [
+ "bytes",
+ "fnv",
+ "futures-core",
+ "futures-sink",
+ "futures-util",
+ "http 0.2.11",
+ "indexmap 2.1.0",
+ "slab",
+ "tokio",
+ "tokio-util",
+ "tracing",
+]
+
+[[package]]
+name = "h2"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d6250322ef6e60f93f9a2162799302cd6f68f79f6e5d85c8c16f14d1d958178"
+checksum = "31d030e59af851932b72ceebadf4a2b5986dba4c3b99dd2493f8273a0f151943"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
- "http",
+ "http 1.1.0",
  "indexmap 2.1.0",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
@@ -855,21 +865,55 @@
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
+name = "http"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
+]
+
+[[package]]
 name = "http-body"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
 dependencies = [
  "bytes",
- "http",
+ "http 0.2.11",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "http-body"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cac85db508abc24a2e48553ba12a996e87244a0395ce011e62b37158745d643"
+dependencies = [
+ "bytes",
+ "http 1.1.0",
+]
+
+[[package]]
+name = "http-body-util"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0475f8b2ac86659c21b64320d5d653f9efe42acd2a4e560073ec61a155a34f1d"
+dependencies = [
+ "bytes",
+ "futures-core",
+ "http 1.1.0",
+ "http-body 1.0.0",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -887,55 +931,91 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
- "h2",
- "http",
- "http-body",
+ "h2 0.3.24",
+ "http 0.2.11",
+ "http-body 0.4.6",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
  "socket2",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
+name = "hyper"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "186548d73ac615b32a73aafe38fb4f56c0d340e110e5a200bcadbaf2e199263a"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-util",
+ "h2 0.4.2",
+ "http 1.1.0",
+ "http-body 1.0.0",
+ "httparse",
+ "httpdate",
+ "itoa",
+ "pin-project-lite",
+ "smallvec",
+ "tokio",
+]
+
+[[package]]
 name = "hyper-rustls"
 version = "0.24.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec3efd23720e2049821a693cbc7e65ea87c72f1c58ff2f9522ff332b1491e590"
 dependencies = [
  "futures-util",
- "http",
- "hyper",
- "rustls",
+ "http 0.2.11",
+ "hyper 0.14.28",
+ "rustls 0.21.10",
  "tokio",
- "tokio-rustls",
+ "tokio-rustls 0.24.1",
 ]
 
 [[package]]
 name = "hyper-timeout"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbb958482e8c7be4bc3cf272a766a2b0bf1a6755e7a6ae777f017a31d11b13b1"
 dependencies = [
- "hyper",
+ "hyper 0.14.28",
  "pin-project-lite",
  "tokio",
  "tokio-io-timeout",
 ]
 
 [[package]]
+name = "hyper-util"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
+dependencies = [
+ "bytes",
+ "futures-util",
+ "http 1.1.0",
+ "http-body 1.0.0",
+ "hyper 1.2.0",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+]
+
+[[package]]
 name = "ident_case"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
 
 [[package]]
 name = "idna"
@@ -1001,26 +1081,26 @@
 name = "ipnet"
 version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
 
 [[package]]
 name = "itertools"
-version = "0.10.5"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itertools"
-version = "0.11.0"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
 version = "1.0.10"
@@ -1049,17 +1129,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.152"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4cd1a83af159aa67994778be9070f0ae1bd732942279cabb14f86f986a21456"
 
@@ -1077,17 +1157,17 @@
 name = "log"
 version = "0.4.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
 
 [[package]]
 name = "lru"
-version = "0.11.1"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4a83fb7698b3643a0e34f9ae6f2e8f0178c0fd42f8b59d493aa271ff3a5bf21"
+checksum = "d3262e75e648fce39813cb56ac41f3c3e3f65217ebf3844d818d1f9398cfb0dc"
 dependencies = [
  "hashbrown 0.14.3",
 ]
 
 [[package]]
 name = "mach2"
 version = "0.4.2"
@@ -1151,53 +1231,54 @@
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "mockall"
-version = "0.11.4"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c84490118f2ee2d74570d114f3d0493cbf02790df303d2707606c3e14e07c96"
+checksum = "43766c2b5203b10de348ffe19f7e54564b64f3d6018ff7648d1e2d6d3a0f0a48"
 dependencies = [
  "cfg-if",
  "downcast",
  "fragile",
  "lazy_static",
  "mockall_derive",
  "predicates",
  "predicates-tree",
 ]
 
 [[package]]
 name = "mockall_derive"
-version = "0.11.4"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22ce75669015c4f47b289fd4d4f56e894e4c96003ffdf3ac51313126f94c6cbb"
+checksum = "af7cbce79ec385a1d4f54baa90a76401eb15d9cab93685f62e7e9f942aa00ae2"
 dependencies = [
  "cfg-if",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "multimap"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
 
 [[package]]
 name = "nix"
-version = "0.27.1"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2eb04e9c688eff1c89d72b407f168cf79bb9e867a9d3323ed6c01519eb9cc053"
+checksum = "ab2156c4fce2f8df6c499cc1c763e4394b7482525bf2a9701c9d79d215f519e4"
 dependencies = [
  "bitflags 2.4.1",
  "cfg-if",
+ "cfg_aliases",
  "libc",
 ]
 
 [[package]]
 name = "no-std-compat"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1206,20 +1287,14 @@
 [[package]]
 name = "nonzero_ext"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38bf9645c8b145698bb0b18a4637dcacbc421ea49bef2317e4fd8065a387cf21"
 
 [[package]]
-name = "normalize-line-endings"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61807f77802ff30975e01f4f071c8ba10c022052f98b3294119f3e615d13e5be"
-
-[[package]]
 name = "nu-ansi-term"
 version = "0.46.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
 dependencies = [
  "overload",
  "winapi",
@@ -1263,86 +1338,82 @@
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "opentelemetry"
-version = "0.21.0"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e32339a5dc40459130b3bd269e9892439f55b33e772d2a9d402a789baaf4e8a"
+checksum = "900d57987be3f2aeb70d385fff9b27fb74c5723cc9a52d904d4f9c807a0667bf"
 dependencies = [
  "futures-core",
  "futures-sink",
- "indexmap 2.1.0",
  "js-sys",
  "once_cell",
  "pin-project-lite",
  "thiserror",
  "urlencoding",
 ]
 
 [[package]]
 name = "opentelemetry-otlp"
-version = "0.14.0"
+version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f24cda83b20ed2433c68241f918d0f6fdec8b1d43b7a9590ab4420c5095ca930"
+checksum = "1a016b8d9495c639af2145ac22387dcb88e44118e45320d9238fbf4e7889abcb"
 dependencies = [
  "async-trait",
  "futures-core",
- "http",
+ "http 0.2.11",
  "opentelemetry",
  "opentelemetry-proto",
  "opentelemetry-semantic-conventions",
  "opentelemetry_sdk",
  "prost",
  "thiserror",
  "tokio",
  "tonic",
 ]
 
 [[package]]
 name = "opentelemetry-prometheus"
-version = "0.14.1"
+version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f8f082da115b0dcb250829e3ed0b8792b8f963a1ad42466e48422fbe6a079bd"
+checksum = "30bbcf6341cab7e2193e5843f0ac36c446a5b3fccb28747afaeda17996dcd02e"
 dependencies = [
  "once_cell",
  "opentelemetry",
  "opentelemetry_sdk",
  "prometheus",
  "protobuf",
 ]
 
 [[package]]
 name = "opentelemetry-proto"
-version = "0.4.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2e155ce5cc812ea3d1dffbd1539aed653de4bf4882d60e6e04dcf0901d674e1"
+checksum = "3a8fddc9b68f5b80dae9d6f510b88e02396f006ad48cac349411fbecc80caae4"
 dependencies = [
  "opentelemetry",
  "opentelemetry_sdk",
  "prost",
  "tonic",
 ]
 
 [[package]]
 name = "opentelemetry-semantic-conventions"
-version = "0.13.0"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f5774f1ef1f982ef2a447f6ee04ec383981a3ab99c8e77a1a7b30182e65bbc84"
-dependencies = [
- "opentelemetry",
-]
+checksum = "f9ab5bd6c42fb9349dcf28af2ba9a0667f697f9bdcca045d39f2cec5543e2910"
 
 [[package]]
 name = "opentelemetry_sdk"
-version = "0.21.2"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2f16aec8a98a457a52664d69e0091bac3a0abd18ead9b641cb00202ba4e0efe4"
+checksum = "9e90c7113be649e31e9a0f8b5ee24ed7a16923b322c3c5ab6367469c049d6b7e"
 dependencies = [
  "async-trait",
  "crossbeam-channel",
  "futures-channel",
  "futures-executor",
  "futures-util",
  "glob",
@@ -1481,24 +1552,20 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "predicates"
-version = "2.1.5"
+version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59230a63c37f3e18569bdb90e4a89cbf5bf8b06fea0b84e65ea10cc4df47addd"
+checksum = "68b87bfd4605926cdfefc1c3b5f8fe560e3feca9d5552cf68c466d3d8236c7e8"
 dependencies = [
- "difflib",
- "float-cmp",
- "itertools 0.10.5",
- "normalize-line-endings",
+ "anstyle",
  "predicates-core",
- "regex",
 ]
 
 [[package]]
 name = "predicates-core"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b794032607612e7abeb4db69adb4e33590fa6cf1149e95fd7cb00e634b92f174"
@@ -1511,20 +1578,20 @@
 dependencies = [
  "predicates-core",
  "termtree",
 ]
 
 [[package]]
 name = "prettyplease"
-version = "0.1.25"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c8646e95016a7a6c4adea95bafa8a16baab64b583356217f2c85db4a39d9a86"
+checksum = "a41cf62165e97c7f814d2221421dbb9afcbcdb0a88068e5ea206e19951c2cbb5"
 dependencies = [
  "proc-macro2",
- "syn 1.0.109",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "proc-macro2"
 version = "1.0.76"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95fc56cda0b5c3325f5fbbd7ff9fda9e02bb00bb3dac51252d2f1bfa1cb8cc8c"
@@ -1545,99 +1612,99 @@
  "parking_lot",
  "protobuf",
  "thiserror",
 ]
 
 [[package]]
 name = "prost"
-version = "0.11.9"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b82eaa1d779e9a4bc1c3217db8ffbeabaae1dca241bf70183242128d48681cd"
+checksum = "146c289cda302b98a28d40c8b3b90498d6e526dd24ac2ecea73e4e491685b94a"
 dependencies = [
  "bytes",
  "prost-derive",
 ]
 
 [[package]]
 name = "prost-build"
-version = "0.11.9"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "119533552c9a7ffacc21e099c24a0ac8bb19c2a2a3f363de84cd9b844feab270"
+checksum = "c55e02e35260070b6f716a2423c2ff1c3bb1642ddca6f99e1f26d06268a0e2d2"
 dependencies = [
  "bytes",
  "heck",
- "itertools 0.10.5",
- "lazy_static",
+ "itertools 0.11.0",
  "log",
  "multimap",
+ "once_cell",
  "petgraph",
  "prettyplease",
  "prost",
  "prost-types",
  "regex",
- "syn 1.0.109",
+ "syn 2.0.48",
  "tempfile",
  "which",
 ]
 
 [[package]]
 name = "prost-derive"
-version = "0.11.9"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5d2d8d10f3c6ded6da8b05b5fb3b8a5082514344d56c9f871412d29b4e075b4"
+checksum = "efb6c9a1dd1def8e2124d17e83a20af56f1570d6c2d2bd9e266ccb768df3840e"
 dependencies = [
  "anyhow",
- "itertools 0.10.5",
+ "itertools 0.11.0",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "prost-types"
-version = "0.11.9"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "213622a1460818959ac1181aaeb2dc9c7f63df720db7d788b3e24eacd1983e13"
+checksum = "193898f59edcf43c26227dcd4c8427f00d99d61e95dcde58dabd49fa291d470e"
 dependencies = [
  "prost",
 ]
 
 [[package]]
 name = "prost-wkt"
-version = "0.4.2"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "562788060bcf2bfabe055194bd991ed2442457661744c88e0a0828ff9a08c08b"
+checksum = "4d8ef9c3f0f1dab910d2b7e2c24a8e4322e122eba6d7a1921eeebcebbc046c40"
 dependencies = [
  "chrono",
  "inventory",
  "prost",
  "serde",
  "serde_derive",
  "serde_json",
  "typetag",
 ]
 
 [[package]]
 name = "prost-wkt-build"
-version = "0.4.2"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4dca8bcead3b728a6a7da017cc95e7f4cb2320ec4f6896bc593a1c4700f7328"
+checksum = "5b31cae9a54ca84fee1504740a82eebf2479532905e106f63ca0c3bc8d780321"
 dependencies = [
  "heck",
  "prost",
  "prost-build",
  "prost-types",
  "quote",
 ]
 
 [[package]]
 name = "prost-wkt-types"
-version = "0.4.2"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2377c5680f2342871823045052e791b4487f7c90aae17e0feaee24cf59578a34"
+checksum = "435be4a8704091b4c5fb1d79799de7f2dbff53af05edf29385237f8cf7ab37ee"
 dependencies = [
  "chrono",
  "prost",
  "prost-build",
  "prost-types",
  "prost-wkt",
  "prost-wkt-build",
@@ -1860,34 +1927,34 @@
 checksum = "37b1ae8d9ac08420c66222fb9096fc5de435c3c48542bc5336c51892cffafb41"
 dependencies = [
  "base64",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
- "h2",
- "http",
- "http-body",
- "hyper",
+ "h2 0.3.24",
+ "http 0.2.11",
+ "http-body 0.4.6",
+ "hyper 0.14.28",
  "hyper-rustls",
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls",
- "rustls-pemfile",
+ "rustls 0.21.10",
+ "rustls-pemfile 1.0.4",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "system-configuration",
  "tokio",
- "tokio-rustls",
+ "tokio-rustls 0.24.1",
  "tokio-util",
  "tower-service",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "wasm-streams",
  "web-sys",
@@ -1973,50 +2040,92 @@
 name = "rustls"
 version = "0.21.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
 dependencies = [
  "log",
  "ring",
- "rustls-webpki",
+ "rustls-webpki 0.101.7",
  "sct",
 ]
 
 [[package]]
+name = "rustls"
+version = "0.22.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e87c9956bd9807afa1f77e0f7594af32566e830e088a5576d27c5b6f30f49d41"
+dependencies = [
+ "log",
+ "ring",
+ "rustls-pki-types",
+ "rustls-webpki 0.102.2",
+ "subtle",
+ "zeroize",
+]
+
+[[package]]
 name = "rustls-native-certs"
-version = "0.6.3"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9aace74cb666635c918e9c12bc0d348266037aa8eb599b5cba565709a8dff00"
+checksum = "8f1fb85efa936c42c6d5fc28d2629bb51e4b2f4b8a5211e297d599cc5a093792"
 dependencies = [
  "openssl-probe",
- "rustls-pemfile",
+ "rustls-pemfile 2.1.1",
+ "rustls-pki-types",
  "schannel",
  "security-framework",
 ]
 
 [[package]]
 name = "rustls-pemfile"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
 dependencies = [
  "base64",
 ]
 
 [[package]]
+name = "rustls-pemfile"
+version = "2.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f48172685e6ff52a556baa527774f61fcaa884f59daf3375c62a3f1cd2549dab"
+dependencies = [
+ "base64",
+ "rustls-pki-types",
+]
+
+[[package]]
+name = "rustls-pki-types"
+version = "1.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ede67b28608b4c60685c7d54122d4400d90f62b40caee7700e700380a390fa8"
+
+[[package]]
 name = "rustls-webpki"
 version = "0.101.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
+name = "rustls-webpki"
+version = "0.102.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
+dependencies = [
+ "ring",
+ "rustls-pki-types",
+ "untrusted",
+]
+
+[[package]]
 name = "rustversion"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "ryu"
@@ -2183,17 +2292,17 @@
 checksum = "dbff4acf519f630b3a3ddcfaea6c06b42174d9a44bc70c620e9ed1649d58b82a"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.2"
+version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dccd0940a2dcdf68d092b8cbab7dc0ad8fa938bf95787e1b916b0e3d0e8e970"
+checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
 
 [[package]]
 name = "socket2"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
 dependencies = [
@@ -2301,21 +2410,22 @@
 [[package]]
 name = "temporal-client"
 version = "0.1.0"
 dependencies = [
  "anyhow",
  "async-trait",
  "backoff",
+ "base64",
  "derive_builder",
  "derive_more",
  "futures",
  "futures-retry",
- "http",
+ "http 0.2.11",
+ "hyper 0.14.28",
  "once_cell",
- "opentelemetry",
  "parking_lot",
  "prost-types",
  "slotmap",
  "temporal-sdk-core-api",
  "temporal-sdk-core-protos",
  "thiserror",
  "tokio",
@@ -2329,15 +2439,14 @@
 [[package]]
 name = "temporal-sdk-bridge"
 version = "0.1.0"
 dependencies = [
  "futures",
  "log",
  "once_cell",
- "parking_lot",
  "prost",
  "prost-types",
  "pyo3",
  "pyo3-asyncio",
  "pythonize",
  "temporal-client",
  "temporal-sdk-core",
@@ -2351,32 +2460,31 @@
 ]
 
 [[package]]
 name = "temporal-sdk-core"
 version = "0.1.0"
 dependencies = [
  "anyhow",
- "arc-swap",
  "async-trait",
  "base64",
  "crossbeam-channel",
  "crossbeam-queue",
  "dashmap",
  "derive_builder",
  "derive_more",
  "enum-iterator",
  "enum_dispatch",
  "flate2",
  "futures",
  "futures-util",
  "governor",
- "http",
- "hyper",
- "itertools 0.11.0",
- "lazy_static",
+ "http-body-util",
+ "hyper 1.2.0",
+ "hyper-util",
+ "itertools 0.12.1",
  "log",
  "lru",
  "mockall",
  "nix",
  "once_cell",
  "opentelemetry",
  "opentelemetry-otlp",
@@ -2402,15 +2510,14 @@
  "thiserror",
  "tokio",
  "tokio-stream",
  "tokio-util",
  "tonic",
  "tonic-build",
  "tracing",
- "tracing-futures",
  "tracing-subscriber",
  "url",
  "uuid",
  "zip",
 ]
 
 [[package]]
@@ -2418,19 +2525,17 @@
 version = "0.1.0"
 dependencies = [
  "async-trait",
  "derive_builder",
  "derive_more",
  "opentelemetry",
  "prost-types",
- "serde",
  "serde_json",
  "temporal-sdk-core-protos",
  "thiserror",
- "tokio",
  "tonic",
  "tracing-core",
  "url",
 ]
 
 [[package]]
 name = "temporal-sdk-core-protos"
@@ -2563,15 +2668,26 @@
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
 dependencies = [
- "rustls",
+ "rustls 0.21.10",
+ "tokio",
+]
+
+[[package]]
+name = "tokio-rustls"
+version = "0.25.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "775e0c0f0adb3a2f22a00c4745d728b479985fc15ee7ca6a2608388c5569860f"
+dependencies = [
+ "rustls 0.22.2",
+ "rustls-pki-types",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-stream"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2594,55 +2710,54 @@
  "pin-project-lite",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "tonic"
-version = "0.9.2"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3082666a3a6433f7f511c7192923fa1fe07c69332d3c6a2e6bb040b569199d5a"
+checksum = "76c4eb7a4e9ef9d4763600161f12f5070b92a578e1b634db88a6887844c91a13"
 dependencies = [
  "async-stream",
  "async-trait",
  "axum",
  "base64",
  "bytes",
- "futures-core",
- "futures-util",
- "h2",
- "http",
- "http-body",
- "hyper",
+ "h2 0.3.24",
+ "http 0.2.11",
+ "http-body 0.4.6",
+ "hyper 0.14.28",
  "hyper-timeout",
  "percent-encoding",
  "pin-project",
  "prost",
  "rustls-native-certs",
- "rustls-pemfile",
+ "rustls-pemfile 2.1.1",
+ "rustls-pki-types",
  "tokio",
- "tokio-rustls",
+ "tokio-rustls 0.25.0",
  "tokio-stream",
  "tower",
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
 name = "tonic-build"
-version = "0.9.2"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6fdaae4c2c638bb70fe42803a26fbd6fc6ac8c72f5c59f67ecc2a2dcabf4b07"
+checksum = "be4ef6dd70a610078cb4e338a0f79d06bc759ff1b22d2120c2ff02ae264ba9c2"
 dependencies = [
  "prettyplease",
  "proc-macro2",
  "prost-build",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "tower"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
@@ -2703,24 +2818,14 @@
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
  "valuable",
 ]
 
 [[package]]
-name = "tracing-futures"
-version = "0.2.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97d095ae15e245a057c8e8451bab9b3ee1e1f68e9ba2b4fbc18d0ac5237835f2"
-dependencies = [
- "pin-project",
- "tracing",
-]
-
-[[package]]
 name = "tracing-log"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee855f1f400bd0e5c02d150ae5de3840039a3f54b025156404e34c23c03f47c3"
 dependencies = [
  "log",
  "once_cell",
@@ -3167,14 +3272,20 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
+name = "zeroize"
+version = "1.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
+
+[[package]]
 name = "zip"
 version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "760394e246e4c28189f19d488c058bf16f564016aefac5d32bb1f3b51d5e9261"
 dependencies = [
  "aes",
  "byteorder",
```

### Comparing `temporalio-1.5.1/temporalio/bridge/Cargo.toml` & `temporalio-1.6.0/temporalio/bridge/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,27 @@
 [lib]
 name = "temporal_sdk_bridge"
 crate-type = ["cdylib"]
 
 [dependencies]
 futures = "0.3"
 log = "0.4"
-once_cell = "1.16.0"
-parking_lot = "0.12"
-prost = "0.11"
-prost-types = "0.11"
+once_cell = "1.16"
+prost = "0.12"
+prost-types = "0.12"
 pyo3 = { version = "0.19", features = ["extension-module", "abi3-py38"] }
 pyo3-asyncio = { version = "0.19", features = ["tokio-runtime"] }
 pythonize = "0.19"
 temporal-client = { version = "0.1.0", path = "./sdk-core/client" }
 temporal-sdk-core = { version = "0.1.0", path = "./sdk-core/core", features = ["ephemeral-server"] }
 temporal-sdk-core-api = { version = "0.1.0", path = "./sdk-core/core-api" }
 temporal-sdk-core-protos = { version = "0.1.0", path = "./sdk-core/sdk-core-protos" }
 tokio = "1.26"
 tokio-stream = "0.1"
-tonic = "0.9"
+tonic = "0.11"
 tracing = "0.1"
 url = "2.2"
 
 [profile.release]
 opt-level = 3
 debug = false
 lto = true
```

### Comparing `temporalio-1.5.1/temporalio/bridge/client.py` & `temporalio-1.6.0/temporalio/bridge/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Nothing in this module should be considered stable. The API may change.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import timedelta
-from typing import Mapping, Optional, Type, TypeVar
+from typing import Mapping, Optional, Tuple, Type, TypeVar
 
 import google.protobuf.message
 
 import temporalio.bridge.runtime
 import temporalio.bridge.temporal_sdk_bridge
 from temporalio.bridge.temporal_sdk_bridge import RPCError
 
@@ -43,25 +43,35 @@
     """Python representation of the Rust struct for configuring keep alive."""
 
     interval_millis: int
     timeout_millis: int
 
 
 @dataclass
+class ClientHttpConnectProxyConfig:
+    """Python representation of the Rust struct for configuring HTTP proxy."""
+
+    target_host: str
+    basic_auth: Optional[Tuple[str, str]]
+
+
+@dataclass
 class ClientConfig:
     """Python representation of the Rust struct for configuring the client."""
 
     target_url: str
     metadata: Mapping[str, str]
+    api_key: Optional[str]
     identity: str
     tls_config: Optional[ClientTlsConfig]
     retry_config: Optional[ClientRetryConfig]
     keep_alive_config: Optional[ClientKeepAliveConfig]
     client_name: str
     client_version: str
+    http_connect_proxy_config: Optional[ClientHttpConnectProxyConfig]
 
 
 @dataclass
 class RpcCall:
     """Python representation of the Rust struct for an RPC call."""
 
     rpc: str
@@ -98,14 +108,18 @@
         self._runtime = runtime
         self._ref = ref
 
     def update_metadata(self, metadata: Mapping[str, str]) -> None:
         """Update underlying metadata on Core client."""
         self._ref.update_metadata(metadata)
 
+    def update_api_key(self, api_key: Optional[str]) -> None:
+        """Update underlying API key on Core client."""
+        self._ref.update_api_key(api_key)
+
     async def call(
         self,
         *,
         service: str,
         rpc: str,
         req: google.protobuf.message.Message,
         resp_type: Type[ProtoMessage],
```

### Comparing `temporalio-1.5.1/temporalio/bridge/metric.py` & `temporalio-1.6.0/temporalio/bridge/metric.py`

 * *Files 22% similar despite different names*

```diff
@@ -71,14 +71,54 @@
     def record(self, value: int, attrs: MetricAttributes) -> None:
         """Record value on histogram."""
         if value < 0:
             raise ValueError("Metric value must be non-negative value")
         self._ref.record(value, attrs._ref)
 
 
+class MetricHistogramFloat:
+    """Metric histogram using SDK Core."""
+
+    def __init__(
+        self,
+        meter: MetricMeter,
+        name: str,
+        description: Optional[str],
+        unit: Optional[str],
+    ) -> None:
+        """Initialize histogram."""
+        self._ref = meter._ref.new_histogram_float(name, description, unit)
+
+    def record(self, value: float, attrs: MetricAttributes) -> None:
+        """Record value on histogram."""
+        if value < 0:
+            raise ValueError("Metric value must be non-negative value")
+        self._ref.record(value, attrs._ref)
+
+
+class MetricHistogramDuration:
+    """Metric histogram using SDK Core."""
+
+    def __init__(
+        self,
+        meter: MetricMeter,
+        name: str,
+        description: Optional[str],
+        unit: Optional[str],
+    ) -> None:
+        """Initialize histogram."""
+        self._ref = meter._ref.new_histogram_duration(name, description, unit)
+
+    def record(self, value_ms: int, attrs: MetricAttributes) -> None:
+        """Record value on histogram."""
+        if value_ms < 0:
+            raise ValueError("Metric value must be non-negative value")
+        self._ref.record(value_ms, attrs._ref)
+
+
 class MetricGauge:
     """Metric gauge using SDK Core."""
 
     def __init__(
         self,
         meter: MetricMeter,
         name: str,
@@ -91,14 +131,34 @@
     def set(self, value: int, attrs: MetricAttributes) -> None:
         """Set value on gauge."""
         if value < 0:
             raise ValueError("Metric value must be non-negative value")
         self._ref.set(value, attrs._ref)
 
 
+class MetricGaugeFloat:
+    """Metric gauge using SDK Core."""
+
+    def __init__(
+        self,
+        meter: MetricMeter,
+        name: str,
+        description: Optional[str],
+        unit: Optional[str],
+    ) -> None:
+        """Initialize gauge."""
+        self._ref = meter._ref.new_gauge_float(name, description, unit)
+
+    def set(self, value: float, attrs: MetricAttributes) -> None:
+        """Set value on gauge."""
+        if value < 0:
+            raise ValueError("Metric value must be non-negative value")
+        self._ref.set(value, attrs._ref)
+
+
 class MetricAttributes:
     """Metric attributes using SDK Core."""
 
     def __init__(
         self,
         meter: MetricMeter,
         ref: temporalio.bridge.temporal_sdk_bridge.MetricAttributesRef,
```

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/activity_result/activity_result_pb2.py` & `temporalio-1.6.0/temporalio/bridge/proto/activity_result/activity_result_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/activity_result/activity_result_pb2.pyi` & `temporalio-1.6.0/temporalio/bridge/proto/activity_result/activity_result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/activity_task/activity_task_pb2.py` & `temporalio-1.6.0/temporalio/bridge/proto/activity_task/activity_task_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/activity_task/activity_task_pb2.pyi` & `temporalio-1.6.0/temporalio/bridge/proto/activity_task/activity_task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/bridge/__init__.py` & `temporalio-1.6.0/temporalio/bridge/proto/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/bridge/bridge_pb2.py` & `temporalio-1.6.0/temporalio/bridge/proto/bridge/bridge_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/bridge/bridge_pb2.pyi` & `temporalio-1.6.0/temporalio/bridge/proto/bridge/bridge_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/child_workflow/child_workflow_pb2.py` & `temporalio-1.6.0/temporalio/bridge/proto/child_workflow/child_workflow_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/child_workflow/child_workflow_pb2.pyi` & `temporalio-1.6.0/temporalio/bridge/proto/child_workflow/child_workflow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/common/common_pb2.py` & `temporalio-1.6.0/temporalio/bridge/proto/common/common_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/common/common_pb2.pyi` & `temporalio-1.6.0/temporalio/bridge/proto/common/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/core_interface_pb2.py` & `temporalio-1.6.0/temporalio/bridge/proto/core_interface_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/core_interface_pb2.pyi` & `temporalio-1.6.0/temporalio/bridge/proto/core_interface_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/external_data/external_data_pb2.py` & `temporalio-1.6.0/temporalio/bridge/proto/external_data/external_data_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/external_data/external_data_pb2.pyi` & `temporalio-1.6.0/temporalio/bridge/proto/external_data/external_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/health/v1/health_pb2.py` & `temporalio-1.6.0/temporalio/bridge/proto/health/v1/health_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/health/v1/health_pb2.pyi` & `temporalio-1.6.0/temporalio/bridge/proto/health/v1/health_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/workflow_activation/__init__.py` & `temporalio-1.6.0/temporalio/bridge/proto/workflow_activation/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/workflow_activation/workflow_activation_pb2.py` & `temporalio-1.6.0/temporalio/bridge/proto/workflow_activation/workflow_activation_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/workflow_activation/workflow_activation_pb2.pyi` & `temporalio-1.6.0/temporalio/bridge/proto/workflow_activation/workflow_activation_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,30 +40,29 @@
     `patches -> signals/updates -> other -> queries -> evictions`
 
     This is because:
     * Patches are expected to apply to the entire activation
     * Signal and update handlers should be invoked before workflow routines are iterated. That is to
       say before the users' main workflow function and anything spawned by it is allowed to continue.
     * Queries always go last (and, in fact, always come in their own activation)
+    * Evictions also always come in their own activation
 
     The downside of this reordering is that a signal or update handler may not observe that some
     other event had already happened (ex: an activity completed) when it is first invoked, though it
     will subsequently when workflow routines are driven. Core only does this reordering to make life
     easier for languages that cannot explicitly control when workflow routines are iterated.
     Languages that can explicitly control such iteration should prefer to apply all the jobs to state
     (by resolving promises/futures, invoking handlers, etc as they iterate over the jobs) and then
     only *after* that is done, drive the workflow routines.
 
     ## Evictions
 
-    Activations that contain only a `remove_from_cache` job should not cause the workflow code
-    to be invoked and may be responded to with an empty command list. Eviction jobs may also
-    appear with other jobs, but will always appear last in the job list. In this case it is
-    expected that the workflow code will be invoked, and the response produced as normal, but
-    the caller should evict the run after doing so.
+    Evictions appear as an activations that contains only a `remove_from_cache` job. Such activations
+    should not cause the workflow code to be invoked and may be responded to with an empty command
+    list.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RUN_ID_FIELD_NUMBER: builtins.int
     TIMESTAMP_FIELD_NUMBER: builtins.int
     IS_REPLAYING_FIELD_NUMBER: builtins.int
@@ -176,15 +175,17 @@
     def fire_timer(self) -> global___FireTimer:
         """A timer has fired, allowing whatever was waiting on it (if anything) to proceed"""
     @property
     def update_random_seed(self) -> global___UpdateRandomSeed:
         """Workflow was reset. The randomness seed must be updated."""
     @property
     def query_workflow(self) -> global___QueryWorkflow:
-        """A request to query the workflow was received."""
+        """A request to query the workflow was received. It is guaranteed that queries (one or more)
+        always come in their own activation after other mutating jobs.
+        """
     @property
     def cancel_workflow(self) -> global___CancelWorkflow:
         """A request to cancel the workflow was received."""
     @property
     def signal_workflow(self) -> global___SignalWorkflow:
         """A request to signal the workflow was received."""
     @property
@@ -217,19 +218,17 @@
     ) -> global___ResolveRequestCancelExternalWorkflow:
         """An attempt to cancel an external workflow resolved"""
     @property
     def do_update(self) -> global___DoUpdate:
         """A request to handle a workflow update."""
     @property
     def remove_from_cache(self) -> global___RemoveFromCache:
-        """Remove the workflow identified by the [WorkflowActivation] containing this job from the cache
-        after performing the activation.
-
-        If other job variant are present in the list, this variant will be the last job in the
-        job list. The string value is a reason for eviction.
+        """Remove the workflow identified by the [WorkflowActivation] containing this job from the
+        cache after performing the activation. It is guaranteed that this will be the only job
+        in the activation if present.
         """
     def __init__(
         self,
         *,
         start_workflow: global___StartWorkflow | None = ...,
         fire_timer: global___FireTimer | None = ...,
         update_random_seed: global___UpdateRandomSeed | None = ...,
```

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/workflow_commands/__init__.py` & `temporalio-1.6.0/temporalio/bridge/proto/workflow_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/workflow_commands/workflow_commands_pb2.py` & `temporalio-1.6.0/temporalio/bridge/proto/workflow_commands/workflow_commands_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/workflow_commands/workflow_commands_pb2.pyi` & `temporalio-1.6.0/temporalio/bridge/proto/workflow_commands/workflow_commands_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/workflow_completion/workflow_completion_pb2.py` & `temporalio-1.6.0/temporalio/bridge/proto/workflow_completion/workflow_completion_pb2.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/proto/workflow_completion/workflow_completion_pb2.pyi` & `temporalio-1.6.0/temporalio/bridge/proto/workflow_completion/workflow_completion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/runtime.py` & `temporalio-1.6.0/temporalio/bridge/runtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,17 @@
             thread_id, exc_type
         )
 
     def __init__(self, *, telemetry: TelemetryConfig) -> None:
         """Create SDK Core runtime."""
         self._ref = temporalio.bridge.temporal_sdk_bridge.init_runtime(telemetry)
 
-    def retrieve_buffered_metrics(self) -> Sequence[Any]:
+    def retrieve_buffered_metrics(self, durations_as_seconds: bool) -> Sequence[Any]:
         """Get buffered metrics."""
-        return self._ref.retrieve_buffered_metrics()
+        return self._ref.retrieve_buffered_metrics(durations_as_seconds)
 
     def write_test_info_log(self, message: str, extra_data: str) -> None:
         """Write a test core log at INFO level."""
         self._ref.write_test_info_log(message, extra_data)
 
     def write_test_debug_log(self, message: str, extra_data: str) -> None:
         """Write a test core log at DEBUG level."""
@@ -64,23 +64,25 @@
 class OpenTelemetryConfig:
     """Python representation of the Rust struct for OpenTelemetry config."""
 
     url: str
     headers: Mapping[str, str]
     metric_periodicity_millis: Optional[int]
     metric_temporality_delta: bool
+    durations_as_seconds: bool
 
 
 @dataclass(frozen=True)
 class PrometheusConfig:
     """Python representation of the Rust struct for Prometheus config."""
 
     bind_address: str
     counters_total_suffix: bool
     unit_suffix: bool
+    durations_as_seconds: bool
 
 
 @dataclass(frozen=True)
 class TelemetryConfig:
     """Python representation of the Rust struct for telemetry config."""
 
     logging: Optional[LoggingConfig]
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/.github/workflows/heavy.yml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/.github/workflows/heavy.yml`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,8 @@
         with:
           version: '3.x'
           repo-token: ${{ secrets.GITHUB_TOKEN }}
 
       - uses: actions-rs/cargo@v1
         with:
           command: integ-test
-          args: -c "--release" -c "--features=save_wf_inputs" -t heavy_tests -- --test-threads 1
+          args: -c "--release" -t heavy_tests -- --test-threads 1
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/.github/workflows/per-pr.yml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/.github/workflows/per-pr.yml`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.ref }}
   cancel-in-progress: true
 
 jobs:
   build-and-test:
     name: "Format, docs, and lint"
-    timeout-minutes: 20
+    timeout-minutes: 10
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
         with:
           submodules: recursive
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
-          toolchain: 1.74.0
+          toolchain: 1.77.0
           override: true
       - name: Install protoc
         uses: arduino/setup-protoc@v1
         with:
           version: '3.x'
           repo-token: ${{ secrets.GITHUB_TOKEN }}
       - run: rustup component add rustfmt clippy
@@ -44,21 +44,22 @@
           command: lint
       - uses: actions-rs/cargo@v1
         with:
           command: test-lint
 
   test:
     name: Unit Tests
+    timeout-minutes: 10
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
-          toolchain: 1.74.0
+          toolchain: 1.77.0
           override: true
       - name: Install protoc
         uses: arduino/setup-protoc@v1
         with:
           version: '3.x'
           repo-token: ${{ secrets.GITHUB_TOKEN }}
       - uses: Swatinem/rust-cache@v2
@@ -73,21 +74,22 @@
       - uses: actions/upload-artifact@v3
         with:
           name: state-machine-coverage
           path: machine_coverage/
 
   fmt:
     name: Integ tests
+    timeout-minutes: 20
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
-          toolchain: 1.74.0
+          toolchain: 1.77.0
           override: true
       - name: Install protoc
         uses: arduino/setup-protoc@v1
         with:
           version: '3.x'
           repo-token: ${{ secrets.GITHUB_TOKEN }}
       - uses: Swatinem/rust-cache@v2
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/ARCHITECTURE.md` & `temporalio-1.6.0/temporalio/bridge/sdk-core/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/LICENSE.txt` & `temporalio-1.6.0/temporalio/bridge/sdk-core/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/README.md` & `temporalio-1.6.0/temporalio/bridge/sdk-core/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-[![Build status](https://badge.buildkite.com/c23f47f4a827f04daece909963bd3a248496f0cdbabfbecee4.svg?branch=master)](https://buildkite.com/temporal/core-sdk?branch=master)
-
 # Temporal Core SDK
 
 Core SDK that can be used as a base for other Temporal SDKs. It is currently used as the base of:
 
 - [TypeScript SDK](https://github.com/temporalio/sdk-typescript/)
 - [Python SDK](https://github.com/temporalio/sdk-python/)
 - [.NET SDK](https://github.com/temporalio/sdk-dotnet/)
@@ -30,15 +28,15 @@
 
 - temporal-sdk-core-protos `./sdk-core-protos` - Holds the generated proto code and extensions
 - temporal-client `./client` - Defines client(s) for interacting with the Temporal gRPC service
 - temporal-sdk-core-api `./core-api` - Defines the API surface exposed by Core
 - temporal-sdk-core `./core` - The Core implementation
 - temporal-sdk `./sdk` - A (currently prototype) Rust SDK built on top of Core. Used for testing.
 - rustfsm `./fsm` - Implements a procedural macro used by core for defining state machines
-    (contains subcrates). It is temporal agnostic.
+  (contains subcrates). It is temporal agnostic.
 
 Visualized (dev dependencies are in blue):
 
 ![Crate dependency graph](./etc/deps.svg)
 
 All the following commands are enforced for each pull request:
 
@@ -47,15 +45,15 @@
 You can build and test the project using cargo:
 `cargo build`
 `cargo test`
 
 Run integ tests with `cargo integ-test`. By default it will start an ephemeral server. You can also
 use an already-running server by passing `-s external`.
 
-Run load tests with `cargo test --features=save_wf_inputs --test heavy_tests`.
+Run load tests with `cargo test --test heavy_tests`.
 
 ## Formatting
 
 To format all code run:
 `cargo fmt --all`
 
 ## Linting
@@ -82,16 +80,16 @@
 `docker-compose -f docker/docker-compose.yaml -f docker/docker-compose-telem.yaml up`
 
 If you are working on a language SDK, you are expected to initialize tracing early in your `main`
 equivalent.
 
 ## Proto files
 
-This repo uses a subtree for upstream protobuf files. The path `sdk-core-protos/protos/api_upstream` is a
-subtree. To update it, use:
+This repo uses a subtree for upstream protobuf files. The path `sdk-core-protos/protos/api_upstream`
+is a subtree. To update it, use:
 
 `git pull --squash --rebase=false -s subtree ssh://git@github.com/temporalio/api.git master --allow-unrelated-histories`
 
 Do not question why this git command is the way it is. It is not our place to interpret git's ways.
 
 The java testserver protos are also pulled from the sdk-java repo, but since we only need a
 subdirectory of that repo, we just copy the files with read-tree:
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/arch_docs/diagrams/README.md` & `temporalio-1.6.0/temporalio/bridge/sdk-core/arch_docs/diagrams/README.md`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/arch_docs/diagrams/sticky_queues.puml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/arch_docs/diagrams/sticky_queues.puml`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/arch_docs/diagrams/workflow_internals.svg` & `temporalio-1.6.0/temporalio/bridge/sdk-core/arch_docs/diagrams/workflow_internals.svg`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/arch_docs/sticky_queues.md` & `temporalio-1.6.0/temporalio/bridge/sdk-core/arch_docs/sticky_queues.md`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/client/Cargo.toml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/client/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,32 @@
 license-file = { workspace = true }
 description = "Clients for interacting with Temporal Clusters"
 homepage = "https://temporal.io/"
 repository = "https://github.com/temporalio/sdk-core"
 keywords = ["temporal", "workflow"]
 categories = ["development-tools"]
 
+[features]
+telemetry = ["dep:opentelemetry"]
+
 [dependencies]
 anyhow = "1.0"
 async-trait = "0.1"
 backoff = "0.4"
-derive_builder = "0.12"
+base64 = "0.21.7"
+derive_builder = { workspace = true }
 derive_more = "0.99"
 futures = "0.3"
 futures-retry = "0.6.0"
 http = "0.2"
-once_cell = "1.13"
-opentelemetry = { workspace = true, features = ["metrics"] }
+hyper = { version = "0.14.28" }
+once_cell = { workspace = true }
+opentelemetry = { workspace = true, features = ["metrics"], optional = true  }
 parking_lot = "0.12"
-prost-types = "0.11"
+prost-types = { workspace = true }
 slotmap = "1.0"
 thiserror = "1.0"
 tokio = "1.1"
 tonic = { workspace = true, features = ["tls", "tls-roots"] }
 tower = "0.4"
 tracing = "0.1"
 url = "2.2"
@@ -36,8 +41,11 @@
 path = "../sdk-core-protos"
 
 [dependencies.temporal-sdk-core-api]
 path = "../core-api"
 
 [dev-dependencies]
 assert_matches = "1"
-mockall = "0.11"
+mockall = "0.12"
+
+[lints]
+workspace = true
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/client/src/lib.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/client/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,36 @@
 //!
 //! It implements auto-retry behavior and metrics collection.
 
 #[macro_use]
 extern crate tracing;
 
 mod metrics;
+mod proxy;
 mod raw;
 mod retry;
 mod worker_registry;
 mod workflow_handle;
 
+pub use crate::proxy::HttpConnectProxyOptions;
 pub use crate::retry::{CallType, RetryClient, RETRYABLE_ERROR_CODES};
 pub use raw::{HealthService, OperatorService, TestService, WorkflowService};
 pub use temporal_sdk_core_protos::temporal::api::{
     enums::v1::ArchivalState,
     filter::v1::{StartTimeFilter, StatusFilter, WorkflowExecutionFilter, WorkflowTypeFilter},
     workflowservice::v1::{
         list_closed_workflow_executions_request::Filters as ListClosedFilters,
         list_open_workflow_executions_request::Filters as ListOpenFilters,
     },
 };
 pub use tonic;
 pub use worker_registry::{Slot, SlotManager, SlotProvider, WorkerKey};
-pub use workflow_handle::{WorkflowExecutionInfo, WorkflowExecutionResult};
+pub use workflow_handle::{
+    GetWorkflowResultOpts, WorkflowExecutionInfo, WorkflowExecutionResult, WorkflowHandle,
+};
 
 use crate::{
     metrics::{GrpcMetricSvc, MetricsContext},
     raw::{sealed::RawClientLike, AttachMetricLabels},
     sealed::WfHandleClient,
     workflow_handle::UntypedWorkflowHandle,
 };
@@ -63,15 +67,15 @@
     },
     TaskToken,
 };
 use tonic::{
     body::BoxBody,
     client::GrpcService,
     codegen::InterceptedService,
-    metadata::{MetadataKey, MetadataValue},
+    metadata::{MetadataKey, MetadataMap, MetadataValue},
     service::Interceptor,
     transport::{Certificate, Channel, Endpoint, Identity},
     Code, Status,
 };
 use tower::ServiceBuilder;
 use url::Url;
 use uuid::Uuid;
@@ -129,14 +133,27 @@
     /// override.
     #[builder(default)]
     pub override_origin: Option<Uri>,
 
     /// If set (which it is by default), HTTP2 gRPC keep alive will be enabled.
     #[builder(default = "Some(ClientKeepAliveConfig::default())")]
     pub keep_alive: Option<ClientKeepAliveConfig>,
+
+    /// HTTP headers to include on every RPC call.
+    #[builder(default)]
+    pub headers: Option<HashMap<String, String>>,
+
+    /// API key which is set as the "Authorization" header with "Bearer " prepended. This will only
+    /// be applied if the headers don't already have an "Authorization" header.
+    #[builder(default)]
+    pub api_key: Option<String>,
+
+    /// HTTP CONNECT proxy to use for this client.
+    #[builder(default)]
+    pub http_connect_proxy: Option<HttpConnectProxyOptions>,
 }
 
 /// Configuration options for TLS
 #[derive(Clone, Debug, Default)]
 pub struct TlsConfig {
     /// Bytes representing the root CA certificate used by the server. If not set, and the server's
     /// cert is issued by someone the operating system trusts, verification will still work (ex:
@@ -196,15 +213,15 @@
 }
 
 impl Default for RetryConfig {
     fn default() -> Self {
         Self {
             initial_interval: Duration::from_millis(100), // 100 ms wait by default.
             randomization_factor: 0.2,                    // +-20% jitter.
-            multiplier: 1.5, // each next retry delay will increase by 50%
+            multiplier: 1.7, // each next retry delay will increase by 70%
             max_interval: Duration::from_secs(5), // until it reaches 5 seconds.
             max_elapsed_time: Some(Duration::from_secs(10)), // 10 seconds total allocated time for all retries.
             max_retries: 10,
         }
     }
 }
 
@@ -275,25 +292,29 @@
 
 /// A client with [ClientOptions] attached, which can be passed to initialize workers,
 /// or can be used directly. Is cheap to clone.
 #[derive(Clone, Debug)]
 pub struct ConfiguredClient<C> {
     client: C,
     options: Arc<ClientOptions>,
-    headers: Arc<RwLock<HashMap<String, String>>>,
+    headers: Arc<RwLock<ClientHeaders>>,
     /// Capabilities as read from the `get_system_info` RPC call made on client connection
     capabilities: Option<get_system_info_response::Capabilities>,
     workers: Arc<SlotManager>,
 }
 
 impl<C> ConfiguredClient<C> {
     /// Set HTTP request headers overwriting previous headers
     pub fn set_headers(&self, headers: HashMap<String, String>) {
-        let mut guard = self.headers.write();
-        *guard = headers;
+        self.headers.write().user_headers = headers;
+    }
+
+    /// Set API key, overwriting previous
+    pub fn set_api_key(&self, api_key: Option<String>) {
+        self.headers.write().api_key = api_key;
     }
 
     /// Returns the options the client is configured with
     pub fn options(&self) -> &ClientOptions {
         &self.options
     }
 
@@ -305,14 +326,42 @@
 
     /// Returns a cloned reference to a registry with workers using this client instance
     pub fn workers(&self) -> Arc<SlotManager> {
         self.workers.clone()
     }
 }
 
+#[derive(Debug)]
+struct ClientHeaders {
+    user_headers: HashMap<String, String>,
+    api_key: Option<String>,
+}
+
+impl ClientHeaders {
+    fn apply_to_metadata(&self, metadata: &mut MetadataMap) {
+        for (key, val) in self.user_headers.iter() {
+            // Only if not already present
+            if !metadata.contains_key(key) {
+                // Ignore invalid keys/values
+                if let (Ok(key), Ok(val)) = (MetadataKey::from_str(key), val.parse()) {
+                    metadata.insert(key, val);
+                }
+            }
+        }
+        if let Some(api_key) = &self.api_key {
+            // Only if not already present
+            if !metadata.contains_key("authorization") {
+                if let Ok(val) = format!("Bearer {}", api_key).parse() {
+                    metadata.insert("authorization", val);
+                }
+            }
+        }
+    }
+}
+
 // The configured client is effectively a "smart" (dumb) pointer
 impl<C> Deref for ConfiguredClient<C> {
     type Target = C;
 
     fn deref(&self) -> &Self::Target {
         &self.client
     }
@@ -327,33 +376,28 @@
 impl ClientOptions {
     /// Attempt to establish a connection to the Temporal server in a specific namespace. The
     /// returned client is bound to that namespace.
     pub async fn connect(
         &self,
         namespace: impl Into<String>,
         metrics_meter: Option<TemporalMeter>,
-        headers: Option<Arc<RwLock<HashMap<String, String>>>>,
     ) -> Result<RetryClient<Client>, ClientInitError> {
-        let client = self
-            .connect_no_namespace(metrics_meter, headers)
-            .await?
-            .into_inner();
+        let client = self.connect_no_namespace(metrics_meter).await?.into_inner();
         let client = Client::new(client, namespace.into());
         let retry_client = RetryClient::new(client, self.retry_config.clone());
         Ok(retry_client)
     }
 
     /// Attempt to establish a connection to the Temporal server and return a gRPC client which is
     /// intercepted with retry, default headers functionality, and metrics if provided.
     ///
     /// See [RetryClient] for more
     pub async fn connect_no_namespace(
         &self,
         metrics_meter: Option<TemporalMeter>,
-        headers: Option<Arc<RwLock<HashMap<String, String>>>>,
     ) -> Result<RetryClient<ConfiguredClient<TemporalServiceClientWithMetrics>>, ClientInitError>
     {
         let channel = Channel::from_shared(self.target_url.to_string())?;
         let channel = self.add_tls_to_channel(channel).await?;
         let channel = if let Some(keep_alive) = self.keep_alive.as_ref() {
             channel
                 .keep_alive_while_idle(true)
@@ -363,22 +407,30 @@
             channel
         };
         let channel = if let Some(origin) = self.override_origin.clone() {
             channel.origin(origin)
         } else {
             channel
         };
-        let channel = channel.connect().await?;
+        // If there is a proxy, we have to connect that way
+        let channel = if let Some(proxy) = self.http_connect_proxy.as_ref() {
+            proxy.connect_endpoint(&channel).await?
+        } else {
+            channel.connect().await?
+        };
         let service = ServiceBuilder::new()
             .layer_fn(move |channel| GrpcMetricSvc {
                 inner: channel,
                 metrics: metrics_meter.clone().map(MetricsContext::new),
             })
             .service(channel);
-        let headers = headers.unwrap_or_default();
+        let headers = Arc::new(RwLock::new(ClientHeaders {
+            user_headers: self.headers.clone().unwrap_or_default(),
+            api_key: self.api_key.clone(),
+        }));
         let interceptor = ServiceCallInterceptor {
             opts: self.clone(),
             headers: headers.clone(),
         };
         let svc = InterceptedService::new(service, interceptor);
 
         let mut client = ConfiguredClient {
@@ -438,15 +490,15 @@
 }
 
 /// Interceptor which attaches common metadata (like "client-name") to every outgoing call
 #[derive(Clone)]
 pub struct ServiceCallInterceptor {
     opts: ClientOptions,
     /// Only accessed as a reader
-    headers: Arc<RwLock<HashMap<String, String>>>,
+    headers: Arc<RwLock<ClientHeaders>>,
 }
 
 impl Interceptor for ServiceCallInterceptor {
     /// This function will get called on each outbound request. Returning a `Status` here will
     /// cancel the request and have that status returned to the caller.
     fn call(&mut self, mut request: tonic::Request<()>) -> Result<tonic::Request<()>, Status> {
         let metadata = request.metadata_mut();
@@ -464,24 +516,15 @@
                 CLIENT_VERSION_HEADER_KEY,
                 self.opts
                     .client_version
                     .parse()
                     .unwrap_or_else(|_| MetadataValue::from_static("")),
             );
         }
-        let headers = &*self.headers.read();
-        for (k, v) in headers {
-            if metadata.contains_key(k) {
-                // Don't overwrite per-request specified headers
-                continue;
-            }
-            if let (Ok(k), Ok(v)) = (MetadataKey::from_str(k), v.parse()) {
-                metadata.insert(k, v);
-            }
-        }
+        self.headers.read().apply_to_metadata(metadata);
         if !metadata.contains_key("grpc-timeout") {
             request.set_timeout(OTHER_CALL_TIMEOUT);
         }
 
         Ok(request)
     }
 }
@@ -1555,33 +1598,72 @@
 impl<T> WfClientExt for T where T: WfHandleClient + Clone + Sized {}
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
-    fn respects_per_call_headers() {
+    fn applies_headers() {
         let opts = ClientOptionsBuilder::default()
             .identity("enchicat".to_string())
             .target_url(Url::parse("https://smolkitty").unwrap())
             .client_name("cute-kitty".to_string())
             .client_version("0.1.0".to_string())
             .build()
             .unwrap();
 
-        let mut static_headers = HashMap::new();
-        static_headers.insert("enchi".to_string(), "kitty".to_string());
-        let mut iceptor = ServiceCallInterceptor {
+        // Initial header set
+        let headers = Arc::new(RwLock::new(ClientHeaders {
+            user_headers: HashMap::new(),
+            api_key: Some("my-api-key".to_owned()),
+        }));
+        headers
+            .clone()
+            .write()
+            .user_headers
+            .insert("my-meta-key".to_owned(), "my-meta-val".to_owned());
+        let mut interceptor = ServiceCallInterceptor {
             opts,
-            headers: Arc::new(RwLock::new(static_headers)),
+            headers: headers.clone(),
         };
+
+        // Confirm on metadata
+        let req = interceptor.call(tonic::Request::new(())).unwrap();
+        assert_eq!(req.metadata().get("my-meta-key").unwrap(), "my-meta-val");
+        assert_eq!(
+            req.metadata().get("authorization").unwrap(),
+            "Bearer my-api-key"
+        );
+
+        // Overwrite at request time
         let mut req = tonic::Request::new(());
-        req.metadata_mut().insert("enchi", "cat".parse().unwrap());
-        let next_req = iceptor.call(req).unwrap();
-        assert_eq!(next_req.metadata().get("enchi").unwrap(), "cat");
+        req.metadata_mut()
+            .insert("my-meta-key", "my-meta-val2".parse().unwrap());
+        req.metadata_mut()
+            .insert("authorization", "my-api-key2".parse().unwrap());
+        let req = interceptor.call(req).unwrap();
+        assert_eq!(req.metadata().get("my-meta-key").unwrap(), "my-meta-val2");
+        assert_eq!(req.metadata().get("authorization").unwrap(), "my-api-key2");
+
+        // Overwrite auth on header
+        headers
+            .clone()
+            .write()
+            .user_headers
+            .insert("authorization".to_owned(), "my-api-key3".to_owned());
+        let req = interceptor.call(tonic::Request::new(())).unwrap();
+        assert_eq!(req.metadata().get("my-meta-key").unwrap(), "my-meta-val");
+        assert_eq!(req.metadata().get("authorization").unwrap(), "my-api-key3");
+
+        // Remove headers and auth and confirm gone
+        headers.clone().write().user_headers.clear();
+        headers.clone().write().api_key.take();
+        let req = interceptor.call(tonic::Request::new(())).unwrap();
+        assert!(!req.metadata().contains_key("my-meta-key"));
+        assert!(!req.metadata().contains_key("authorization"));
     }
 
     #[test]
     fn keep_alive_defaults() {
         let mut builder = ClientOptionsBuilder::default();
         builder
             .identity("enchicat".to_string())
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/client/src/metrics.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/client/src/metrics.rs`

 * *Files 15% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 use futures::{future::BoxFuture, FutureExt};
 use std::{
     sync::Arc,
     task::{Context, Poll},
     time::{Duration, Instant},
 };
 use temporal_sdk_core_api::telemetry::metrics::{
-    CoreMeter, Counter, Histogram, MetricAttributes, MetricKeyValue, MetricParameters,
+    CoreMeter, Counter, HistogramDuration, MetricAttributes, MetricKeyValue, MetricParameters,
     TemporalMeter,
 };
 use tonic::{body::BoxBody, transport::Channel};
 use tower::Service;
 
 /// Used to track context associated with metrics, and record/update them
 // Possible improvement: make generic over some type tag so that methods are only exposed if the
 // appropriate k/vs have already been set.
 #[derive(Clone, derive_more::DebugCustom)]
 #[debug(fmt = "MetricsContext {{ attribs: {kvs:?}, poll_is_long: {poll_is_long} }}")]
-pub struct MetricsContext {
+pub(crate) struct MetricsContext {
     meter: Arc<dyn CoreMeter>,
     kvs: MetricAttributes,
     poll_is_long: bool,
 
     svc_request: Arc<dyn Counter>,
     svc_request_failed: Arc<dyn Counter>,
     long_svc_request: Arc<dyn Counter>,
     long_svc_request_failed: Arc<dyn Counter>,
 
-    svc_request_latency: Arc<dyn Histogram>,
-    long_svc_request_latency: Arc<dyn Histogram>,
+    svc_request_latency: Arc<dyn HistogramDuration>,
+    long_svc_request_latency: Arc<dyn HistogramDuration>,
 }
 
 impl MetricsContext {
     pub(crate) fn new(tm: TemporalMeter) -> Self {
         let meter = tm.inner;
         Self {
             kvs: meter.new_attributes(tm.default_attribs),
@@ -53,22 +53,22 @@
                 unit: "".into(),
             }),
             long_svc_request_failed: meter.counter(MetricParameters {
                 name: "long_request_failure".into(),
                 description: "Count of long-poll request failures by rpc name".into(),
                 unit: "".into(),
             }),
-            svc_request_latency: meter.histogram(MetricParameters {
+            svc_request_latency: meter.histogram_duration(MetricParameters {
                 name: "request_latency".into(),
-                unit: "ms".into(),
+                unit: "duration".into(),
                 description: "Histogram of client request latencies".into(),
             }),
-            long_svc_request_latency: meter.histogram(MetricParameters {
+            long_svc_request_latency: meter.histogram_duration(MetricParameters {
                 name: "long_request_latency".into(),
-                unit: "ms".into(),
+                unit: "duration".into(),
                 description: "Histogram of client long-poll request latencies".into(),
             }),
             meter,
         }
     }
 
     /// Mutate this metrics context with new attributes
@@ -99,19 +99,17 @@
             self.svc_request_failed.add(1, &self.kvs);
         }
     }
 
     /// Record service request latency
     pub(crate) fn record_svc_req_latency(&self, dur: Duration) {
         if self.poll_is_long {
-            self.long_svc_request_latency
-                .record(dur.as_millis() as u64, &self.kvs);
+            self.long_svc_request_latency.record(dur, &self.kvs);
         } else {
-            self.svc_request_latency
-                .record(dur.as_millis() as u64, &self.kvs);
+            self.svc_request_latency.record(dur, &self.kvs);
         }
     }
 }
 
 const KEY_NAMESPACE: &str = "namespace";
 const KEY_SVC_METHOD: &str = "operation";
 const KEY_TASK_QUEUE: &str = "task_queue";
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/client/src/raw.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/client/src/raw.rs`

 * *Files 0% similar despite different names*

```diff
@@ -295,27 +295,27 @@
 }
 
 #[derive(Debug)]
 pub(super) struct AttachMetricLabels {
     pub(super) labels: Vec<MetricKeyValue>,
 }
 impl AttachMetricLabels {
-    pub fn new(kvs: impl Into<Vec<MetricKeyValue>>) -> Self {
+    pub(super) fn new(kvs: impl Into<Vec<MetricKeyValue>>) -> Self {
         Self { labels: kvs.into() }
     }
-    pub fn namespace(ns: impl Into<String>) -> Self {
+    pub(super) fn namespace(ns: impl Into<String>) -> Self {
         AttachMetricLabels::new(vec![namespace_kv(ns.into())])
     }
-    pub fn task_q(&mut self, tq: Option<TaskQueue>) -> &mut Self {
+    pub(super) fn task_q(&mut self, tq: Option<TaskQueue>) -> &mut Self {
         if let Some(tq) = tq {
             self.task_q_str(tq.name);
         }
         self
     }
-    pub fn task_q_str(&mut self, tq: impl Into<String>) -> &mut Self {
+    pub(super) fn task_q_str(&mut self, tq: impl Into<String>) -> &mut Self {
         self.labels.push(task_queue_kv(tq.into()));
         self
     }
 }
 
 // Blanket impl the trait for all raw-client-like things. Since the trait default-implements
 // everything, there's nothing to actually implement.
@@ -1011,15 +1011,15 @@
         operatorservice::v1::DeleteNamespaceRequest, workflowservice::v1::ListNamespacesRequest,
     };
 
     // Just to help make sure some stuff compiles. Not run.
     #[allow(dead_code)]
     async fn raw_client_retry_compiles() {
         let opts = ClientOptionsBuilder::default().build().unwrap();
-        let raw_client = opts.connect_no_namespace(None, None).await.unwrap();
+        let raw_client = opts.connect_no_namespace(None).await.unwrap();
         let mut retry_client = RetryClient::new(raw_client, opts.retry_config);
 
         let list_ns_req = ListNamespacesRequest::default();
         let fact = |c: &mut RetryClient<_>, req| {
             let mut c = c.workflow_client_mut().clone();
             async move { c.list_namespaces(req).await }.boxed()
         };
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/client/src/retry.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/client/src/retry.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/client/src/worker_registry/mod.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/client/src/worker_registry/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -91,17 +91,19 @@
             Some(self.index.insert(key))
         } else {
             warn!("Ignoring registration for worker: {key:?}.");
             None
         }
     }
 
-    fn unregister(&mut self, id: WorkerKey) {
+    fn unregister(&mut self, id: WorkerKey) -> Option<Box<dyn SlotProvider + Send + Sync>> {
         if let Some(key) = self.index.remove(id) {
-            self.providers.remove(&key);
+            self.providers.remove(&key)
+        } else {
+            None
         }
     }
 
     #[cfg(test)]
     fn num_providers(&self) -> (usize, usize) {
         (self.index.len(), self.providers.len())
     }
@@ -136,15 +138,15 @@
 
     /// Register a local worker that can provide WFT processing slots.
     pub fn register(&self, provider: Box<dyn SlotProvider + Send + Sync>) -> Option<WorkerKey> {
         self.manager.write().register(provider)
     }
 
     /// Unregister a provider, typically when its worker starts shutdown.
-    pub fn unregister(&self, id: WorkerKey) {
+    pub fn unregister(&self, id: WorkerKey) -> Option<Box<dyn SlotProvider + Send + Sync>> {
         self.manager.write().unregister(id)
     }
 
     #[cfg(test)]
     /// Returns (num_providers, num_buckets), where a bucket key is namespace+task_queue.
     /// There is only one provider per bucket so `num_providers` should be equal to `num_buckets`.
     pub fn num_providers(&self) -> (usize, usize) {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/client/src/workflow_handle/mod.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/client/src/workflow_handle/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         CT: RawClientLike<SvcType = InterceptedMetricsSvc> + Clone,
     {
         UntypedWorkflowHandle::new(client, self)
     }
 }
 
 /// A workflow handle to a workflow with unknown types. Uses raw payloads.
-pub type UntypedWorkflowHandle<CT> = WorkflowHandle<CT, Vec<Payload>>;
+pub(crate) type UntypedWorkflowHandle<CT> = WorkflowHandle<CT, Vec<Payload>>;
 
 impl<CT, RT> WorkflowHandle<CT, RT>
 where
     CT: RawClientLike<SvcType = InterceptedMetricsSvc> + Clone,
     // TODO: Make more generic, capable of (de)serialization w/ serde
     RT: FromPayloadsExt,
 {
@@ -87,18 +87,20 @@
         Self {
             client,
             info,
             _res_type: PhantomData::<RT>,
         }
     }
 
+    /// Get the workflow execution info
     pub fn info(&self) -> &WorkflowExecutionInfo {
         &self.info
     }
 
+    /// Await the result of the workflow execution
     pub async fn get_workflow_result(
         &self,
         opts: GetWorkflowResultOpts,
     ) -> Result<WorkflowExecutionResult<RT>, anyhow::Error> {
         let mut next_page_tok = vec![];
         let mut run_id = self.info.run_id.clone().unwrap_or_default();
         loop {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/Cargo.toml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -9,72 +9,67 @@
 repository = "https://github.com/temporalio/sdk-core"
 keywords = ["temporal", "workflow"]
 categories = ["development-tools"]
 
 [lib]
 
 [features]
-default = []
-# Do not enable this feature when building production SDKs. If we ever want a user in the field to
-# record WF input data, we can build them a custom SDK or they can build - it adds significant extra
-# code size in the form of [de]serializers.
-save_wf_inputs = ["rmp-serde", "temporal-sdk-core-protos/serde_serialize"]
+default = ["otel"]
+otel = ["dep:opentelemetry", "dep:opentelemetry_sdk", "dep:opentelemetry-otlp",
+    "dep:opentelemetry-prometheus", "dep:hyper", "dep:hyper-util", "dep:http-body-util"]
 tokio-console = ["console-subscriber"]
 ephemeral-server = ["dep:flate2", "dep:nix", "dep:reqwest", "dep:tar", "dep:zip"]
 
 [dependencies]
 anyhow = "1.0"
-arc-swap = "1.3"
 async-trait = "0.1"
 base64 = "0.21"
-console-subscriber = { version = "0.1", optional = true }
+console-subscriber = { version = "0.2", optional = true }
 crossbeam-channel = "0.5"
 crossbeam-queue = "0.3"
 dashmap = "5.5"
-derive_builder = "0.12"
+derive_builder = { workspace = true }
 derive_more = { workspace = true }
 enum_dispatch = "0.3"
-enum-iterator = "1.4"
+enum-iterator = "2"
 flate2 = { version = "1.0", optional = true }
 futures = "0.3"
 futures-util = "0.3"
 governor = "0.6"
-http = "0.2"
-hyper = "0.14"
-itertools = "0.11"
-lazy_static = "1.4"
-lru = "0.11"
-mockall = "0.11"
-nix = { version = "0.27", optional = true, features = ["process", "signal"] }
-once_cell = "1.5"
-opentelemetry = { workspace = true, features = ["metrics"] }
-opentelemetry_sdk = { version = "0.21", features = ["rt-tokio", "metrics"] }
-opentelemetry-otlp = { version = "0.14", features = ["tokio", "metrics"] }
-opentelemetry-prometheus = "0.14"
+http-body-util = { version = "0.1", optional = true }
+hyper = { version = "1.2", optional = true }
+hyper-util = { version = "0.1", features = ["server", "http1", "http2", "tokio"], optional = true }
+itertools = "0.12"
+lru = "0.12"
+mockall = "0.12"
+nix = { version = "0.28", optional = true, features = ["process", "signal"] }
+once_cell = { workspace = true }
+opentelemetry = { workspace = true, features = ["metrics"], optional = true }
+opentelemetry_sdk = { version = "0.22", features = ["rt-tokio", "metrics"], optional = true }
+opentelemetry-otlp = { version = "0.15", features = ["tokio", "metrics"], optional = true }
+opentelemetry-prometheus = { version = "0.15", optional = true }
 parking_lot = { version = "0.12", features = ["send_guard"] }
 pin-project = "1.0"
 prometheus = "0.13"
-prost = "0.11"
-prost-types = { version = "0.4", package = "prost-wkt-types" }
+prost = { workspace = true }
+prost-types = { version = "0.5", package = "prost-wkt-types" }
 rand = "0.8.3"
 reqwest = { version = "0.11", features = ["json", "stream", "rustls-tls", "tokio-rustls"], default-features = false, optional = true }
 ringbuf = "0.3"
-rmp-serde = { version = "1.1", optional = true }
 serde = "1.0"
 serde_json = "1.0"
 siphasher = "1.0"
 slotmap = "1.0"
 tar = { version = "0.4", optional = true }
 thiserror = "1.0"
 tokio = { version = "1.26", features = ["rt", "rt-multi-thread", "parking_lot", "time", "fs", "process"] }
 tokio-util = { version = "0.7", features = ["io", "io-util"] }
 tokio-stream = "0.1"
 tonic = { workspace = true, features = ["tls", "tls-roots"] }
 tracing = "0.1"
-tracing-futures = "0.2"
 tracing-subscriber = { version = "0.3", features = ["parking_lot", "env-filter", "registry"] }
 url = "2.2"
 uuid = { version = "1.1", features = ["v4"] }
 zip = { version = "0.6.3", optional = true }
 log = "0.4.20"
 
 # 1st party local deps
@@ -94,14 +89,15 @@
 
 [dev-dependencies]
 assert_matches = "1.4"
 bimap = "0.6.1"
 clap = { version = "4.0", features = ["derive"] }
 criterion = "0.5"
 rstest = "0.18"
+sysinfo = "0.30"
 temporal-sdk-core-test-utils = { path = "../test-utils" }
 temporal-sdk = { path = "../sdk" }
 
 [build-dependencies]
 tonic-build = { workspace = true }
 
 [[test]]
@@ -111,23 +107,20 @@
 # `cargo test --test integ_tests`
 test = false
 
 [[test]]
 name = "heavy_tests"
 path = "../tests/heavy_tests.rs"
 test = false
-required-features = ["save_wf_inputs"]
 
 [[bench]]
 name = "workflow_replay"
 harness = false
 
 # This is maybe a bit hacky, but we call the runner an "example" because that gets it compiling with
 # the dev-dependencies, which we want.
 [[example]]
 name = "integ_runner"
 path = "../tests/runner.rs"
 
-[[example]]
-name = "wf_input_replay"
-path = "../tests/wf_input_replay.rs"
-required-features = ["save_wf_inputs"]
+[lints]
+workspace = true
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/benches/workflow_replay.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/benches/workflow_replay.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/abstractions/take_cell.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/abstractions/take_cell.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 use parking_lot::Mutex;
 use std::sync::atomic::{AtomicBool, Ordering};
 
 /// Implements something a bit like a `OnceCell`, but starts already initialized and allows you
 /// to take everything out of it only once in a thread-safe way. This isn't optimized for super
 /// fast-path usage.
-pub struct TakeCell<T> {
+pub(crate) struct TakeCell<T> {
     taken: AtomicBool,
     data: Mutex<Option<T>>,
 }
 
 impl<T> TakeCell<T> {
-    pub fn new(val: T) -> Self {
+    pub(crate) fn new(val: T) -> Self {
         Self {
             taken: AtomicBool::new(false),
             data: Mutex::new(Some(val)),
         }
     }
 
     /// If the cell has not already been taken from, takes the value and returns it
-    pub fn take_once(&self) -> Option<T> {
+    pub(crate) fn take_once(&self) -> Option<T> {
         if self.taken.load(Ordering::Acquire) {
             return None;
         }
         self.taken.store(true, Ordering::Release);
         self.data.lock().take()
     }
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/abstractions.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/abstractions.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 //! This module contains very generic helpers that can be used codebase-wide
 
-pub mod take_cell;
+pub(crate) mod take_cell;
 
 use crate::MetricsContext;
 use derive_more::DebugCustom;
 use std::{
     fmt::{Debug, Formatter},
     sync::{
         atomic::{AtomicBool, AtomicUsize, Ordering},
@@ -25,42 +25,42 @@
     /// isn't used in the sense the user expects until we actually also get the corresponding task.
     unused_claimants: Arc<AtomicUsize>,
     metrics_ctx: MetricsContext,
     record_fn: fn(&MetricsContext, usize),
 }
 
 impl MeteredSemaphore {
-    pub fn new(
+    pub(crate) fn new(
         inital_permits: usize,
         metrics_ctx: MetricsContext,
         record_fn: fn(&MetricsContext, usize),
     ) -> Self {
         Self {
             sem: Arc::new(Semaphore::new(inital_permits)),
             unused_claimants: Arc::new(AtomicUsize::new(0)),
             metrics_ctx,
             record_fn,
         }
     }
 
-    pub fn available_permits(&self) -> usize {
+    pub(crate) fn available_permits(&self) -> usize {
         self.sem.available_permits()
     }
 
     #[cfg(test)]
-    pub fn unused_permits(&self) -> usize {
+    pub(crate) fn unused_permits(&self) -> usize {
         self.sem.available_permits() + self.unused_claimants.load(Ordering::Acquire)
     }
 
-    pub async fn acquire_owned(&self) -> Result<OwnedMeteredSemPermit, AcquireError> {
+    pub(crate) async fn acquire_owned(&self) -> Result<OwnedMeteredSemPermit, AcquireError> {
         let res = self.sem.clone().acquire_owned().await?;
         Ok(self.build_owned(res))
     }
 
-    pub fn try_acquire_owned(&self) -> Result<OwnedMeteredSemPermit, TryAcquireError> {
+    pub(crate) fn try_acquire_owned(&self) -> Result<OwnedMeteredSemPermit, TryAcquireError> {
         let res = self.sem.clone().try_acquire_owned()?;
         Ok(self.build_owned(res))
     }
 
     fn build_owned(&self, res: OwnedSemaphorePermit) -> OwnedMeteredSemPermit {
         self.unused_claimants.fetch_add(1, Ordering::Release);
         self.record();
@@ -102,45 +102,45 @@
     inner: Arc<MeteredSemaphore>,
     outstanding_permits: AtomicUsize,
     close_requested: AtomicBool,
     close_complete_token: CancellationToken,
 }
 
 impl ClosableMeteredSemaphore {
-    pub fn new_arc(sem: Arc<MeteredSemaphore>) -> Arc<Self> {
+    pub(crate) fn new_arc(sem: Arc<MeteredSemaphore>) -> Arc<Self> {
         Arc::new(Self {
             inner: sem,
             outstanding_permits: Default::default(),
             close_requested: AtomicBool::new(false),
             close_complete_token: CancellationToken::new(),
         })
     }
 }
 
 impl ClosableMeteredSemaphore {
     #[cfg(test)]
-    pub fn unused_permits(&self) -> usize {
+    pub(crate) fn unused_permits(&self) -> usize {
         self.inner.unused_permits()
     }
 
     /// Request to close the semaphore and prevent new permits from being acquired.
-    pub fn close(&self) {
+    pub(crate) fn close(&self) {
         self.close_requested.store(true, Ordering::Release);
         if self.outstanding_permits.load(Ordering::Acquire) == 0 {
             self.close_complete_token.cancel();
         }
     }
 
     /// Returns after close has been requested and all outstanding permits have been returned.
-    pub async fn close_complete(&self) {
+    pub(crate) async fn close_complete(&self) {
         self.close_complete_token.cancelled().await;
     }
 
     /// Acquire a permit if one is available and close was not requested.
-    pub fn try_acquire_owned(
+    pub(crate) fn try_acquire_owned(
         self: &Arc<Self>,
     ) -> Result<TrackedOwnedMeteredSemPermit, TryAcquireError> {
         if self.close_requested.load(Ordering::Acquire) {
             return Err(TryAcquireError::Closed);
         }
         self.outstanding_permits.fetch_add(1, Ordering::Release);
         let res = self.inner.try_acquire_owned();
@@ -217,27 +217,18 @@
             (self.record_fn)(false)
         }
         UsedMeteredSemPermit(self)
     }
 }
 
 #[derive(Debug)]
-pub(crate) struct UsedMeteredSemPermit(OwnedMeteredSemPermit);
-impl UsedMeteredSemPermit {
-    #[cfg(feature = "save_wf_inputs")]
-    pub(crate) fn fake_deserialized() -> Self {
-        let sem = Arc::new(Semaphore::new(1));
-        let inner = sem.try_acquire_owned().unwrap();
-        Self(OwnedMeteredSemPermit {
-            inner,
-            unused_claimants: None,
-            record_fn: Box::new(|_| {}),
-        })
-    }
-}
+pub(crate) struct UsedMeteredSemPermit(
+    // Field isn't read, but we need to hold on to it.
+    #[allow(dead_code)] OwnedMeteredSemPermit,
+);
 
 macro_rules! dbg_panic {
   ($($arg:tt)*) => {
       error!($($arg)*);
       debug_assert!(false, $($arg)*);
   };
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/activity_tasks.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/activity_tasks.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/child_workflows.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/child_workflows.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/determinism.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/determinism.rs`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,16 @@
         enums::v1::{EventType, WorkflowTaskFailedCause},
         failure::v1::Failure,
     },
     TestHistoryBuilder, DEFAULT_ACTIVITY_TYPE,
 };
 
 static DID_FAIL: AtomicBool = AtomicBool::new(false);
-pub async fn timer_wf_fails_once(ctx: WfContext) -> WorkflowResult<()> {
+
+pub(crate) async fn timer_wf_fails_once(ctx: WfContext) -> WorkflowResult<()> {
     ctx.timer(Duration::from_secs(1)).await;
     if DID_FAIL
         .compare_exchange(false, true, Ordering::Relaxed, Ordering::Relaxed)
         .is_ok()
     {
         panic!("Ahh");
     }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/local_activities.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/local_activities.rs`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             WorkflowOptions::default(),
         )
         .await
         .unwrap();
     worker.run_until_done().await.unwrap();
 }
 
-pub async fn local_act_fanout_wf(ctx: WfContext) -> WorkflowResult<()> {
+pub(crate) async fn local_act_fanout_wf(ctx: WfContext) -> WorkflowResult<()> {
     let las: Vec<_> = (1..=50)
         .map(|i| {
             ctx.local_activity(LocalActivityOptions {
                 activity_type: "echo".to_string(),
                 input: format!("Hi {i}")
                     .as_json_payload()
                     .expect("serializes fine"),
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/mod.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 use crate::{
     errors::{PollActivityError, PollWfError},
     test_help::{build_mock_pollers, canned_histories, mock_worker, test_worker_cfg, MockPollCfg},
     worker::client::mocks::{mock_manual_workflow_client, mock_workflow_client},
     Worker,
 };
 use futures::FutureExt;
+use once_cell::sync::Lazy;
 use std::time::Duration;
 use temporal_sdk_core_api::Worker as WorkerTrait;
 use temporal_sdk_core_protos::coresdk::workflow_completion::WorkflowActivationCompletion;
 use tokio::{sync::Barrier, time::sleep};
 
 #[tokio::test]
 async fn after_shutdown_server_is_not_polled() {
@@ -41,17 +42,16 @@
         worker.poll_workflow_activation().await.unwrap_err(),
         PollWfError::ShutDown
     );
     worker.finalize_shutdown().await;
 }
 
 // Better than cloning a billion arcs...
-lazy_static::lazy_static! {
-    static ref BARR: Barrier = Barrier::new(3);
-}
+static BARR: Lazy<Barrier> = Lazy::new(|| Barrier::new(3));
+
 #[tokio::test]
 async fn shutdown_interrupts_both_polls() {
     let mut mock_client = mock_manual_workflow_client();
     mock_client
         .expect_poll_activity_task()
         .times(1)
         .returning(move |_, _| {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/queries.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/queries.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/replay_flag.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/replay_flag.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/updates.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/updates.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/workers.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/workers.rs`

 * *Files 1% similar despite different names*

```diff
@@ -171,35 +171,34 @@
     let res = core.poll_workflow_activation().await.unwrap();
     assert_eq!(res.jobs.len(), 1);
 
     let complete_order = RefCell::new(vec![]);
     // Initiate shutdown before completing the activation
     let shutdown_fut = async {
         core.shutdown().await;
-        complete_order.borrow_mut().push(3);
+        complete_order.borrow_mut().push(2);
     };
     let poll_fut = async {
         // This will return shutdown once the completion goes through
         assert_matches!(
             core.poll_workflow_activation().await.unwrap_err(),
             PollWfError::ShutDown
         );
-        complete_order.borrow_mut().push(2);
     };
     let complete_fut = async {
         core.complete_workflow_activation(WorkflowActivationCompletion::from_cmds(
             res.run_id,
             vec![start_timer_cmd(1, Duration::from_secs(1))],
         ))
         .await
         .unwrap();
         complete_order.borrow_mut().push(1);
     };
     tokio::join!(shutdown_fut, poll_fut, complete_fut);
-    assert_eq!(&complete_order.into_inner(), &[1, 2, 3])
+    assert_eq!(&complete_order.into_inner(), &[1, 2])
 }
 
 #[tokio::test]
 async fn complete_eviction_after_shutdown_doesnt_panic() {
     let t = canned_histories::single_timer("1");
     let mut mh = build_mock_pollers(MockPollCfg::from_resp_batches(
         "fakeid",
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/workflow_cancels.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/workflow_cancels.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/core_tests/workflow_tasks.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/core_tests/workflow_tasks.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1527,15 +1527,15 @@
         let activation = worker.poll_workflow_activation().await.unwrap();
         assert_matches!(
             activation.jobs.as_slice(),
             [WorkflowActivationJob {
                 variant: Some(workflow_activation_job::Variant::RemoveFromCache(_)),
             },]
         );
-        run_id = activation.run_id.clone();
+        run_id.clone_from(&activation.run_id);
         worker
             .complete_workflow_activation(WorkflowActivationCompletion::empty(activation.run_id))
             .await
             .unwrap();
     }
     assert_eq!(worker.outstanding_workflow_tasks().await, 0);
     // We should be "out of work" because the mock service thinks we didn't complete the last task,
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/ephemeral_server/mod.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/ephemeral_server/mod.rs`

 * *Files 11% similar despite different names*

```diff
@@ -18,107 +18,14 @@
 use url::Url;
 use zip::read::read_zipfile_from_stream;
 
 #[cfg(target_family = "unix")]
 use std::os::unix::fs::OpenOptionsExt;
 use std::process::Stdio;
 
-/// Configuration for Temporalite.
-/// Will be removed eventually as its successor, Temporal CLI matures.
-/// We don't care for the duplication between this struct and [TemporalDevServerConfig] and prefer that over another
-/// abstraction since the existence of this struct is temporary.
-#[derive(Debug, Clone, derive_builder::Builder)]
-pub struct TemporaliteConfig {
-    /// Required path to executable or download info.
-    pub exe: EphemeralExe,
-    /// Namespace to use.
-    #[builder(default = "\"default\".to_owned()")]
-    pub namespace: String,
-    /// IP to bind to.
-    #[builder(default = "\"127.0.0.1\".to_owned()")]
-    pub ip: String,
-    /// Port to use or obtains a free one if none given.
-    #[builder(default)]
-    pub port: Option<u16>,
-    /// Sqlite DB filename if persisting or non-persistent if none.
-    #[builder(default)]
-    pub db_filename: Option<String>,
-    /// Whether to enable the UI.
-    #[builder(default)]
-    pub ui: bool,
-    /// Log format and level
-    #[builder(default = "(\"pretty\".to_owned(), \"warn\".to_owned())")]
-    pub log: (String, String),
-    /// Additional arguments to Temporalite.
-    #[builder(default)]
-    pub extra_args: Vec<String>,
-}
-
-impl TemporaliteConfig {
-    /// Start a Temporalite server.
-    pub async fn start_server(&self) -> anyhow::Result<EphemeralServer> {
-        self.start_server_with_output(Stdio::inherit(), Stdio::inherit())
-            .await
-    }
-
-    /// Start a Temporalite server with configurable stdout destination.
-    pub async fn start_server_with_output(
-        &self,
-        output: Stdio,
-        err_output: Stdio,
-    ) -> anyhow::Result<EphemeralServer> {
-        // Get exe path
-        let exe_path = self
-            .exe
-            .get_or_download("temporalite", "temporalite", None)
-            .await?;
-
-        // Get free port if not already given
-        let port = self.port.unwrap_or_else(|| get_free_port(&self.ip));
-
-        // Build arg set
-        let mut args = vec![
-            "start".to_owned(),
-            "--port".to_owned(),
-            port.to_string(),
-            "--namespace".to_owned(),
-            self.namespace.clone(),
-            "--ip".to_owned(),
-            self.ip.clone(),
-            "--log-format".to_owned(),
-            self.log.0.clone(),
-            "--log-level".to_owned(),
-            self.log.1.clone(),
-            "--dynamic-config-value".to_owned(),
-            "frontend.enableServerVersionCheck=false".to_owned(),
-        ];
-        if let Some(db_filename) = &self.db_filename {
-            args.push("--filename".to_owned());
-            args.push(db_filename.clone());
-        } else {
-            args.push("--ephemeral".to_owned());
-        }
-        if !self.ui {
-            args.push("--headless".to_owned());
-        }
-        args.extend(self.extra_args.clone());
-
-        // Start
-        EphemeralServer::start(EphemeralServerConfig {
-            exe_path,
-            port,
-            args,
-            has_test_service: false,
-            output,
-            err_output,
-        })
-        .await
-    }
-}
-
 /// Configuration for Temporal CLI dev server.
 #[derive(Debug, Clone, derive_builder::Builder)]
 pub struct TemporalDevServerConfig {
     /// Required path to executable or download info.
     pub exe: EphemeralExe,
     /// Namespace to use.
     #[builder(default = "\"default\".to_owned()")]
@@ -303,65 +210,38 @@
             .identity("online_checker".to_owned())
             .target_url(Url::parse(&target_url)?)
             .client_name("online-checker".to_owned())
             .client_version("0.1.0".to_owned())
             .build()?;
         for _ in 0..50 {
             sleep(Duration::from_millis(100)).await;
-            if client_options
-                .connect_no_namespace(None, None)
-                .await
-                .is_ok()
-            {
+            if client_options.connect_no_namespace(None).await.is_ok() {
                 return success;
             }
         }
         Err(anyhow!("Failed connecting to test server after 5 seconds"))
     }
 
     /// Shutdown the server (i.e. kill the child process). This does not attempt
     /// a kill if the child process appears completed, but such a check is not
     /// atomic so a kill could still fail as completed if completed just before
     /// kill.
-    #[cfg(not(target_family = "unix"))]
     pub async fn shutdown(&mut self) -> anyhow::Result<()> {
         // Only kill if there is a PID
         if self.child.id().is_some() {
             Ok(self.child.kill().await?)
         } else {
             Ok(())
         }
     }
 
-    /// Shutdown the server (i.e. kill the child process). This does not attempt
-    /// a kill if the child process appears completed, but such a check is not
-    /// atomic so a kill could still fail as completed if completed just before
-    /// kill.
-    #[cfg(target_family = "unix")]
-    pub async fn shutdown(&mut self) -> anyhow::Result<()> {
-        // For whatever reason, Tokio is not properly waiting on result
-        // after sending kill in some cases which is causing defunct zombie
-        // processes to remain and kill() to hang. Therefore, we are sending
-        // SIGKILL and waiting on the process ourselves using a low-level call.
-        //
-        // WARNING: This is based on empirical evidence starting a Python test
-        // run on Linux with Python 3.7 (does not happen on Python 3.10 nor does
-        // it happen on Temporalite nor does it happen in Rust integration
-        // tests). Don't alter without running that scenario. EX: SIGINT works but not SIGKILL
-        if let Some(pid) = self.child.id() {
-            let nix_pid = nix::unistd::Pid::from_raw(pid as i32);
-            Ok(spawn_blocking(move || {
-                nix::sys::signal::kill(nix_pid, nix::sys::signal::Signal::SIGINT)?;
-                nix::sys::wait::waitpid(Some(nix_pid), None)
-            })
-            .await?
-            .map(|_| ())?)
-        } else {
-            Ok(())
-        }
+    /// Get the process ID of the child. This will be None if the process is
+    /// considered to be complete.
+    pub fn child_process_id(&self) -> Option<u32> {
+        self.child.id()
     }
 }
 
 /// Where to find an executable. Can be a path or download.
 #[derive(Debug, Clone)]
 pub enum EphemeralExe {
     /// Existing path on the filesystem for the executable.
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/internal_flags.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/internal_flags.rs`

 * *Files 8% similar despite different names*

```diff
@@ -39,54 +39,54 @@
         core_since_last_complete: HashSet<CoreInternalFlags>,
         lang_since_last_complete: HashSet<u32>,
     },
     Disabled,
 }
 
 impl InternalFlags {
-    pub fn new(server_capabilities: &get_system_info_response::Capabilities) -> Self {
+    pub(crate) fn new(server_capabilities: &get_system_info_response::Capabilities) -> Self {
         match server_capabilities.sdk_metadata {
             true => Self::Enabled {
                 core: Default::default(),
                 lang: Default::default(),
                 core_since_last_complete: Default::default(),
                 lang_since_last_complete: Default::default(),
             },
             false => Self::Disabled,
         }
     }
 
-    pub fn add_from_complete(&mut self, e: &WorkflowTaskCompletedEventAttributes) {
+    pub(crate) fn add_from_complete(&mut self, e: &WorkflowTaskCompletedEventAttributes) {
         if let Self::Enabled { core, lang, .. } = self {
             if let Some(metadata) = e.sdk_metadata.as_ref() {
                 core.extend(
                     metadata
                         .core_used_flags
                         .iter()
                         .map(|u| CoreInternalFlags::from_u32(*u)),
                 );
                 lang.extend(metadata.lang_used_flags.iter());
             }
         }
     }
 
-    pub fn add_lang_used(&mut self, flags: impl IntoIterator<Item = u32>) {
+    pub(crate) fn add_lang_used(&mut self, flags: impl IntoIterator<Item = u32>) {
         if let Self::Enabled {
             lang_since_last_complete,
             ..
         } = self
         {
             lang_since_last_complete.extend(flags);
         }
     }
 
     /// Returns true if this flag may currently be used. If `should_record` is true, always returns
     /// true and records the flag as being used, for taking later via
     /// [Self::gather_for_wft_complete].
-    pub fn try_use(&mut self, core_patch: CoreInternalFlags, should_record: bool) -> bool {
+    pub(crate) fn try_use(&mut self, core_patch: CoreInternalFlags, should_record: bool) -> bool {
         match self {
             Self::Enabled {
                 core,
                 core_since_last_complete,
                 ..
             } => {
                 if should_record {
@@ -100,28 +100,28 @@
             // any internal flags since they can't be recorded for future use
             Self::Disabled => false,
         }
     }
 
     /// Writes all known core flags to the set which should be recorded in the current WFT if not
     /// already known. Must only be called if not replaying.
-    pub fn write_all_known(&mut self) {
+    pub(crate) fn write_all_known(&mut self) {
         if let Self::Enabled {
             core_since_last_complete,
             ..
         } = self
         {
             core_since_last_complete.extend(CoreInternalFlags::all_except_too_high());
         }
     }
 
     /// Wipes the recorded flags used during the current WFT and returns a partially filled
     /// sdk metadata message that can be combined with any existing data before sending the WFT
     /// complete
-    pub fn gather_for_wft_complete(&mut self) -> WorkflowTaskCompletedMetadata {
+    pub(crate) fn gather_for_wft_complete(&mut self) -> WorkflowTaskCompletedMetadata {
         match self {
             Self::Enabled {
                 core_since_last_complete,
                 lang_since_last_complete,
                 core,
                 lang,
             } => {
@@ -144,15 +144,15 @@
                     sdk_version: "".to_string(),
                 }
             }
             Self::Disabled => WorkflowTaskCompletedMetadata::default(),
         }
     }
 
-    pub fn all_lang(&self) -> impl Iterator<Item = u32> + '_ {
+    pub(crate) fn all_lang(&self) -> impl Iterator<Item = u32> + '_ {
         match self {
             Self::Enabled { lang, .. } => Either::Left(lang.iter().copied()),
             Self::Disabled => Either::Right(iter::empty()),
         }
     }
 }
 
@@ -161,15 +161,15 @@
         match v {
             1 => Self::IdAndTypeDeterminismChecks,
             2 => Self::UpsertSearchAttributeOnPatch,
             _ => Self::TooHigh,
         }
     }
 
-    pub fn all_except_too_high() -> impl Iterator<Item = CoreInternalFlags> {
+    pub(crate) fn all_except_too_high() -> impl Iterator<Item = CoreInternalFlags> {
         enum_iterator::all::<CoreInternalFlags>()
             .filter(|f| !matches!(f, CoreInternalFlags::TooHigh))
     }
 }
 
 #[cfg(test)]
 mod tests {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/lib.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,14 @@
     Client, ClientOptions, ClientOptionsBuilder, ClientTlsConfig, RetryClient, RetryConfig,
     TlsConfig, WorkflowClientTrait,
 };
 pub use temporal_sdk_core_api as api;
 pub use temporal_sdk_core_protos as protos;
 pub use temporal_sdk_core_protos::TaskToken;
 pub use url::Url;
-#[cfg(feature = "save_wf_inputs")]
-pub use worker::replay_wf_state_inputs;
 pub use worker::{Worker, WorkerConfig, WorkerConfigBuilder};
 
 use crate::{
     replay::{HistoryForReplay, ReplayWorkerInput},
     telemetry::{
         metrics::MetricsContext, remove_trace_subscriber_for_current_thread,
         set_trace_subscriber_for_current_thread, telemetry_init, TelemetryInstance,
@@ -75,22 +73,15 @@
     runtime: &CoreRuntime,
     worker_config: WorkerConfig,
     client: CT,
 ) -> Result<Worker, anyhow::Error>
 where
     CT: Into<sealed::AnyClient>,
 {
-    let client = {
-        let ll = client.into().into_inner();
-        let mut client = Client::new(*ll, worker_config.namespace.clone());
-        if let Some(ref id_override) = worker_config.client_identity_override {
-            client.options_mut().identity = id_override.clone();
-        }
-        RetryClient::new(client, RetryConfig::default())
-    };
+    let client = init_worker_client(&worker_config, *client.into().into_inner());
     if client.namespace() != worker_config.namespace {
         panic!("Passed in client is not bound to the same namespace as the worker");
     }
     let client_ident = client.get_options().identity.clone();
     let sticky_q = sticky_q_name_for_worker(&client_ident, &worker_config);
     let client_bag = Arc::new(WorkerClientBag::new(
         client,
@@ -121,14 +112,25 @@
     info!(
         task_queue = rwi.config.task_queue.as_str(),
         "Registering replay worker"
     );
     rwi.into_core_worker()
 }
 
+pub(crate) fn init_worker_client(
+    config: &WorkerConfig,
+    client: ConfiguredClient<TemporalServiceClientWithMetrics>,
+) -> RetryClient<Client> {
+    let mut client = Client::new(client, config.namespace.clone());
+    if let Some(ref id_override) = config.client_identity_override {
+        client.options_mut().identity.clone_from(id_override);
+    }
+    RetryClient::new(client, RetryConfig::default())
+}
+
 /// Creates a unique sticky queue name for a worker, iff the config allows for 1 or more cached
 /// workflows.
 pub(crate) fn sticky_q_name_for_worker(
     process_identity: &str,
     config: &WorkerConfig,
 ) -> Option<String> {
     if config.max_cached_workflows > 0 {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/pollers/mod.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/pollers/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 };
 
 #[cfg(test)]
 use futures::Future;
 #[cfg(test)]
 pub(crate) use poll_buffer::MockPermittedPollBuffer;
 
-pub type Result<T, E = tonic::Status> = std::result::Result<T, E>;
+pub(crate) type Result<T, E = tonic::Status> = std::result::Result<T, E>;
 
 /// A trait for things that poll the server. Hides complexity of concurrent polling or polling
 /// on sticky/nonsticky queues simultaneously.
 #[cfg_attr(test, mockall::automock)]
 #[cfg_attr(test, allow(unused))]
 #[async_trait::async_trait]
-pub trait Poller<PollResult>
+pub(crate) trait Poller<PollResult>
 where
     PollResult: Send + Sync + 'static,
 {
     async fn poll(&self) -> Option<Result<PollResult>>;
     fn notify_shutdown(&self);
     async fn shutdown(self);
     /// Need a separate shutdown to be able to consume boxes :(
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/pollers/poll_buffer.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/pollers/poll_buffer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         mpsc::{unbounded_channel, UnboundedReceiver},
         Mutex,
     },
     task::JoinHandle,
 };
 use tokio_util::sync::CancellationToken;
 
-pub struct LongPollBuffer<T> {
+pub(crate) struct LongPollBuffer<T> {
     buffered_polls: Mutex<UnboundedReceiver<pollers::Result<(T, OwnedMeteredSemPermit)>>>,
     shutdown: CancellationToken,
     join_handles: FuturesUnordered<JoinHandle<()>>,
     /// Pollers won't actually start polling until initialized & value is sent
     starter: broadcast::Sender<()>,
     did_start: AtomicBool,
 }
@@ -179,15 +179,15 @@
         let this = *self;
         this.shutdown().await;
     }
 }
 
 /// A poller capable of polling on a sticky and a nonsticky queue simultaneously for workflow tasks.
 #[derive(derive_more::Constructor)]
-pub struct WorkflowTaskPoller {
+pub(crate) struct WorkflowTaskPoller {
     normal_poller: PollWorkflowTaskBuffer,
     sticky_poller: Option<PollWorkflowTaskBuffer>,
 }
 
 #[async_trait::async_trait]
 impl Poller<(PollWorkflowTaskQueueResponse, OwnedMeteredSemPermit)> for WorkflowTaskPoller {
     async fn poll(
@@ -219,15 +219,16 @@
 
     async fn shutdown_box(self: Box<Self>) {
         let this = *self;
         this.shutdown().await;
     }
 }
 
-pub type PollWorkflowTaskBuffer = LongPollBuffer<PollWorkflowTaskQueueResponse>;
+pub(crate) type PollWorkflowTaskBuffer = LongPollBuffer<PollWorkflowTaskQueueResponse>;
+
 pub(crate) fn new_workflow_task_buffer(
     client: Arc<dyn WorkerClient>,
     task_queue: TaskQueue,
     concurrent_pollers: usize,
     semaphore: Arc<MeteredSemaphore>,
     shutdown: CancellationToken,
     num_pollers_handler: Option<impl Fn(usize) + Send + Sync + 'static>,
@@ -242,15 +243,16 @@
         concurrent_pollers,
         shutdown,
         num_pollers_handler,
         None::<fn() -> BoxFuture<'static, ()>>,
     )
 }
 
-pub type PollActivityTaskBuffer = LongPollBuffer<PollActivityTaskQueueResponse>;
+pub(crate) type PollActivityTaskBuffer = LongPollBuffer<PollActivityTaskQueueResponse>;
+
 #[allow(clippy::too_many_arguments)]
 pub(crate) fn new_activity_task_buffer(
     client: Arc<dyn WorkerClient>,
     task_queue: String,
     concurrent_pollers: usize,
     semaphore: Arc<MeteredSemaphore>,
     max_tps: Option<f64>,
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/protosext/mod.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/protosext/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -41,31 +41,31 @@
     },
     utilities::TryIntoOrNone,
 };
 
 /// A validated version of a [PollWorkflowTaskQueueResponse]
 #[derive(Clone, PartialEq)]
 #[allow(clippy::manual_non_exhaustive)] // Clippy doesn't understand it's only for *in* this crate
-pub struct ValidPollWFTQResponse {
-    pub task_token: TaskToken,
-    pub task_queue: String,
-    pub workflow_execution: WorkflowExecution,
-    pub workflow_type: String,
-    pub history: History,
-    pub next_page_token: Vec<u8>,
-    pub attempt: u32,
-    pub previous_started_event_id: i64,
-    pub started_event_id: i64,
+pub(crate) struct ValidPollWFTQResponse {
+    pub(crate) task_token: TaskToken,
+    pub(crate) task_queue: String,
+    pub(crate) workflow_execution: WorkflowExecution,
+    pub(crate) workflow_type: String,
+    pub(crate) history: History,
+    pub(crate) next_page_token: Vec<u8>,
+    pub(crate) attempt: u32,
+    pub(crate) previous_started_event_id: i64,
+    pub(crate) started_event_id: i64,
     /// If this is present, `history` will be empty. This is not a very "tight" design, but it's
     /// enforced at construction time. From the `query` field.
-    pub legacy_query: Option<WorkflowQuery>,
+    pub(crate) legacy_query: Option<WorkflowQuery>,
     /// Query requests from the `queries` field
-    pub query_requests: Vec<QueryWorkflow>,
+    pub(crate) query_requests: Vec<QueryWorkflow>,
     /// Protocol messages
-    pub messages: Vec<IncomingProtocolMessage>,
+    pub(crate) messages: Vec<IncomingProtocolMessage>,
 
     /// Zero-size field to prevent explicit construction
     _cant_construct_me: (),
 }
 
 impl Debug for ValidPollWFTQResponse {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
@@ -249,16 +249,16 @@
         } else {
             None
         }
     }
 }
 
 pub(crate) struct CompleteLocalActivityData {
-    pub marker_dat: LocalActivityMarkerData,
-    pub result: Result<Payload, Failure>,
+    pub(crate) marker_dat: LocalActivityMarkerData,
+    pub(crate) result: Result<Payload, Failure>,
 }
 
 pub(crate) fn validate_activity_completion(
     status: &activity_execution_result::Status,
 ) -> Result<(), CompleteActivityError> {
     match status {
         Status::Completed(c) if c.result.is_none() => {
@@ -299,40 +299,40 @@
     }
 }
 
 /// Validated version of [ScheduleLocalActivity]. See it for field docs.
 /// One or both of `schedule_to_close_timeout` and `start_to_close_timeout` are guaranteed to exist.
 #[derive(Debug, Clone)]
 #[cfg_attr(test, derive(Default))]
-pub struct ValidScheduleLA {
-    pub seq: u32,
-    pub activity_id: String,
-    pub activity_type: String,
-    pub attempt: u32,
-    pub original_schedule_time: Option<SystemTime>,
-    pub headers: HashMap<String, Payload>,
-    pub arguments: Vec<Payload>,
-    pub schedule_to_start_timeout: Option<Duration>,
-    pub close_timeouts: LACloseTimeouts,
-    pub retry_policy: RetryPolicy,
-    pub local_retry_threshold: Duration,
-    pub cancellation_type: ActivityCancellationType,
+pub(crate) struct ValidScheduleLA {
+    pub(crate) seq: u32,
+    pub(crate) activity_id: String,
+    pub(crate) activity_type: String,
+    pub(crate) attempt: u32,
+    pub(crate) original_schedule_time: Option<SystemTime>,
+    pub(crate) headers: HashMap<String, Payload>,
+    pub(crate) arguments: Vec<Payload>,
+    pub(crate) schedule_to_start_timeout: Option<Duration>,
+    pub(crate) close_timeouts: LACloseTimeouts,
+    pub(crate) retry_policy: RetryPolicy,
+    pub(crate) local_retry_threshold: Duration,
+    pub(crate) cancellation_type: ActivityCancellationType,
 }
 
 #[derive(Debug, Clone, Copy)]
-pub enum LACloseTimeouts {
+pub(crate) enum LACloseTimeouts {
     ScheduleOnly(Duration),
     StartOnly(Duration),
     Both { sched: Duration, start: Duration },
 }
 
 impl LACloseTimeouts {
     /// Splits into (schedule_to_close, start_to_close) options, one or both of which is guaranteed
     /// to be populated
-    pub fn into_sched_and_start(self) -> (Option<Duration>, Option<Duration>) {
+    pub(crate) fn into_sched_and_start(self) -> (Option<Duration>, Option<Duration>) {
         match self {
             LACloseTimeouts::ScheduleOnly(x) => (Some(x), None),
             LACloseTimeouts::StartOnly(x) => (None, Some(x)),
             LACloseTimeouts::Both { sched, start } => (Some(sched), Some(start)),
         }
     }
 }
@@ -341,15 +341,15 @@
 impl Default for LACloseTimeouts {
     fn default() -> Self {
         LACloseTimeouts::ScheduleOnly(Duration::from_secs(100))
     }
 }
 
 impl ValidScheduleLA {
-    pub fn from_schedule_la(v: ScheduleLocalActivity) -> Result<Self, anyhow::Error> {
+    pub(crate) fn from_schedule_la(v: ScheduleLocalActivity) -> Result<Self, anyhow::Error> {
         let original_schedule_time = v
             .original_schedule_time
             .map(|x| {
                 x.try_into()
                     .map_err(|_| anyhow!("Could not convert original_schedule_time"))
             })
             .transpose()?;
@@ -402,15 +402,15 @@
         };
         let retry_policy = v.retry_policy.unwrap_or_default();
         let local_retry_threshold = v
             .local_retry_threshold
             .clone()
             .try_into_or_none()
             .unwrap_or_else(|| Duration::from_secs(60));
-        let cancellation_type = ActivityCancellationType::from_i32(v.cancellation_type)
+        let cancellation_type = ActivityCancellationType::try_from(v.cancellation_type)
             .unwrap_or(ActivityCancellationType::WaitCancellationCompleted);
         Ok(ValidScheduleLA {
             seq: v.seq,
             activity_id: v.activity_id,
             activity_type: v.activity_type,
             attempt: v.attempt,
             original_schedule_time,
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/protosext/protocol_messages.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/protosext/protocol_messages.rs`

 * *Files 15% similar despite different names*

```diff
@@ -4,33 +4,31 @@
     common::v1::Payload,
     protocol::v1::{message::SequencingId, Message},
     update,
 };
 
 /// A decoded & verified of a [Message] that came with a WFT.
 #[derive(Debug, Clone, PartialEq)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
-pub struct IncomingProtocolMessage {
-    pub id: String,
-    pub protocol_instance_id: String,
-    pub sequencing_id: Option<SequencingId>,
-    pub body: IncomingProtocolMessageBody,
+pub(crate) struct IncomingProtocolMessage {
+    pub(crate) id: String,
+    pub(crate) protocol_instance_id: String,
+    pub(crate) sequencing_id: Option<SequencingId>,
+    pub(crate) body: IncomingProtocolMessageBody,
 }
+
 impl IncomingProtocolMessage {
-    pub fn processable_after_event_id(&self) -> Option<i64> {
+    pub(crate) fn processable_after_event_id(&self) -> Option<i64> {
         match self.sequencing_id {
             None => Some(0),
             Some(SequencingId::EventId(id)) => Some(id),
             Some(SequencingId::CommandIndex(_)) => None,
         }
     }
 }
+
 impl TryFrom<Message> for IncomingProtocolMessage {
     type Error = anyhow::Error;
 
     fn try_from(m: Message) -> Result<Self, Self::Error> {
         let body = m.body.try_into()?;
         Ok(Self {
             id: m.id,
@@ -40,19 +38,15 @@
         })
     }
 }
 
 /// All the protocol [Message] bodies Core understands that might come to us when receiving a new
 /// WFT.
 #[derive(Debug, Clone, PartialEq)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
-pub enum IncomingProtocolMessageBody {
+pub(crate) enum IncomingProtocolMessageBody {
     UpdateRequest(UpdateRequest),
 }
 
 impl TryFrom<Option<prost_types::Any>> for IncomingProtocolMessageBody {
     type Error = anyhow::Error;
 
     fn try_from(v: Option<prost_types::Any>) -> Result<Self, Self::Error> {
@@ -67,23 +61,19 @@
             }
             o => bail!("Could not understand protocol message type {}", o),
         })
     }
 }
 
 #[derive(Debug, Clone, PartialEq)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
-pub struct UpdateRequest {
-    pub name: String,
-    pub headers: HashMap<String, Payload>,
-    pub input: Vec<Payload>,
-    pub meta: update::v1::Meta,
+pub(crate) struct UpdateRequest {
+    pub(crate) name: String,
+    pub(crate) headers: HashMap<String, Payload>,
+    pub(crate) input: Vec<Payload>,
+    pub(crate) meta: update::v1::Meta,
 }
 
 impl TryFrom<update::v1::Request> for UpdateRequest {
     type Error = anyhow::Error;
 
     fn try_from(r: update::v1::Request) -> Result<Self, Self::Error> {
         let inp = r
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/replay/mod.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/replay/mod.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/retry_logic.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/retry_logic.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/telemetry/log_export.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/telemetry/log_export.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/telemetry/metrics.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/telemetry/metrics.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,22 @@
-use crate::{
-    abstractions::dbg_panic,
-    telemetry::{
-        default_resource, metric_temporality_to_selector, prometheus_server::PromServer,
-        TelemetryInstance, TELEM_SERVICE_NAME,
-    },
-};
-use opentelemetry::{
-    self,
-    metrics::{Meter, MeterProvider as MeterProviderT, Unit},
-    KeyValue,
-};
-use opentelemetry_otlp::WithExportConfig;
-use opentelemetry_sdk::{
-    metrics::{
-        new_view,
-        reader::{AggregationSelector, DefaultAggregationSelector},
-        Aggregation, Instrument, InstrumentKind, MeterProvider, MeterProviderBuilder,
-        PeriodicReader, View,
-    },
-    runtime, AttributeSet,
+use crate::{abstractions::dbg_panic, telemetry::TelemetryInstance};
+
+use std::{
+    fmt::{Debug, Display},
+    iter::Iterator,
+    sync::Arc,
+    time::Duration,
 };
-use parking_lot::RwLock;
-use std::{collections::HashMap, fmt::Debug, net::SocketAddr, sync::Arc, time::Duration};
-use temporal_sdk_core_api::telemetry::{
-    metrics::{
-        BufferAttributes, BufferInstrumentRef, CoreMeter, Counter, Gauge, Histogram,
-        LazyBufferInstrument, MetricAttributes, MetricCallBufferer, MetricEvent, MetricKeyValue,
-        MetricKind, MetricParameters, MetricUpdateVal, NewAttributes, NoOpCoreMeter,
-    },
-    OtelCollectorOptions, PrometheusExporterOptions,
+use temporal_sdk_core_api::telemetry::metrics::{
+    BufferAttributes, BufferInstrumentRef, CoreMeter, Counter, Gauge, GaugeF64, Histogram,
+    HistogramDuration, HistogramF64, LazyBufferInstrument, MetricAttributes, MetricCallBufferer,
+    MetricEvent, MetricKeyValue, MetricKind, MetricParameters, MetricUpdateVal, NewAttributes,
+    NoOpCoreMeter,
 };
-use tokio::task::AbortHandle;
-use tonic::metadata::MetadataMap;
+use temporal_sdk_core_protos::temporal::api::enums::v1::WorkflowTaskFailedCause;
 
 /// Used to track context associated with metrics, and record/update them
 ///
 /// Possible improvement: make generic over some type tag so that methods are only exposed if the
 /// appropriate k/vs have already been set.
 #[derive(Clone)]
 pub(crate) struct MetricsContext {
@@ -45,26 +26,26 @@
 }
 
 struct Instruments {
     wf_completed_counter: Arc<dyn Counter>,
     wf_canceled_counter: Arc<dyn Counter>,
     wf_failed_counter: Arc<dyn Counter>,
     wf_cont_counter: Arc<dyn Counter>,
-    wf_e2e_latency: Arc<dyn Histogram>,
+    wf_e2e_latency: Arc<dyn HistogramDuration>,
     wf_task_queue_poll_empty_counter: Arc<dyn Counter>,
     wf_task_queue_poll_succeed_counter: Arc<dyn Counter>,
     wf_task_execution_failure_counter: Arc<dyn Counter>,
-    wf_task_sched_to_start_latency: Arc<dyn Histogram>,
-    wf_task_replay_latency: Arc<dyn Histogram>,
-    wf_task_execution_latency: Arc<dyn Histogram>,
+    wf_task_sched_to_start_latency: Arc<dyn HistogramDuration>,
+    wf_task_replay_latency: Arc<dyn HistogramDuration>,
+    wf_task_execution_latency: Arc<dyn HistogramDuration>,
     act_poll_no_task: Arc<dyn Counter>,
     act_task_received_counter: Arc<dyn Counter>,
     act_execution_failed: Arc<dyn Counter>,
-    act_sched_to_start_latency: Arc<dyn Histogram>,
-    act_exec_latency: Arc<dyn Histogram>,
+    act_sched_to_start_latency: Arc<dyn HistogramDuration>,
+    act_exec_latency: Arc<dyn HistogramDuration>,
     worker_registered: Arc<dyn Counter>,
     num_pollers: Arc<dyn Gauge>,
     task_slots_available: Arc<dyn Gauge>,
     sticky_cache_hit: Arc<dyn Counter>,
     sticky_cache_miss: Arc<dyn Counter>,
     sticky_cache_size: Arc<dyn Gauge>,
     sticky_cache_evictions: Arc<dyn Counter>,
@@ -152,38 +133,36 @@
     /// A workflow continued as new
     pub(crate) fn wf_continued_as_new(&self) {
         self.instruments.wf_cont_counter.add(1, &self.kvs);
     }
 
     /// Record workflow total execution time in milliseconds
     pub(crate) fn wf_e2e_latency(&self, dur: Duration) {
-        self.instruments
-            .wf_e2e_latency
-            .record(dur.as_millis() as u64, &self.kvs);
+        self.instruments.wf_e2e_latency.record(dur, &self.kvs);
     }
 
     /// Record workflow task schedule to start time in millis
     pub(crate) fn wf_task_sched_to_start_latency(&self, dur: Duration) {
         self.instruments
             .wf_task_sched_to_start_latency
-            .record(dur.as_millis() as u64, &self.kvs);
+            .record(dur, &self.kvs);
     }
 
     /// Record workflow task execution time in milliseconds
     pub(crate) fn wf_task_latency(&self, dur: Duration) {
         self.instruments
             .wf_task_execution_latency
-            .record(dur.as_millis() as u64, &self.kvs);
+            .record(dur, &self.kvs);
     }
 
     /// Record time it takes to catch up on replaying a WFT
     pub(crate) fn wf_task_replay_latency(&self, dur: Duration) {
         self.instruments
             .wf_task_replay_latency
-            .record(dur.as_millis() as u64, &self.kvs);
+            .record(dur, &self.kvs);
     }
 
     /// An activity long poll timed out
     pub(crate) fn act_poll_timeout(&self) {
         self.instruments.act_poll_no_task.add(1, &self.kvs);
     }
 
@@ -197,23 +176,21 @@
         self.instruments.act_execution_failed.add(1, &self.kvs);
     }
 
     /// Record activity task schedule to start time in millis
     pub(crate) fn act_sched_to_start_latency(&self, dur: Duration) {
         self.instruments
             .act_sched_to_start_latency
-            .record(dur.as_millis() as u64, &self.kvs);
+            .record(dur, &self.kvs);
     }
 
     /// Record time it took to complete activity execution, from the time core generated the
     /// activity task, to the time lang responded with a completion (failure or success).
     pub(crate) fn act_execution_latency(&self, dur: Duration) {
-        self.instruments
-            .act_exec_latency
-            .record(dur.as_millis() as u64, &self.kvs);
+        self.instruments.act_exec_latency.record(dur, &self.kvs);
     }
 
     /// A worker was registered
     pub(crate) fn worker_registered(&self) {
         self.instruments.worker_registered.add(1, &self.kvs);
     }
 
@@ -269,17 +246,17 @@
                 unit: "".into(),
             }),
             wf_cont_counter: meter.counter(MetricParameters {
                 name: "workflow_continue_as_new".into(),
                 description: "Count of continued-as-new workflows".into(),
                 unit: "".into(),
             }),
-            wf_e2e_latency: meter.histogram(MetricParameters {
+            wf_e2e_latency: meter.histogram_duration(MetricParameters {
                 name: WF_E2E_LATENCY_NAME.into(),
-                unit: "ms".into(),
+                unit: "duration".into(),
                 description: "Histogram of total workflow execution latencies".into(),
             }),
             wf_task_queue_poll_empty_counter: meter.counter(MetricParameters {
                 name: "workflow_task_queue_poll_empty".into(),
                 description: "Count of workflow task queue poll timeouts (no new task)".into(),
                 unit: "".into(),
             }),
@@ -289,27 +266,27 @@
                 unit: "".into(),
             }),
             wf_task_execution_failure_counter: meter.counter(MetricParameters {
                 name: "workflow_task_execution_failed".into(),
                 description: "Count of workflow task execution failures".into(),
                 unit: "".into(),
             }),
-            wf_task_sched_to_start_latency: meter.histogram(MetricParameters {
+            wf_task_sched_to_start_latency: meter.histogram_duration(MetricParameters {
                 name: WF_TASK_SCHED_TO_START_LATENCY_NAME.into(),
-                unit: "ms".into(),
+                unit: "duration".into(),
                 description: "Histogram of workflow task schedule-to-start latencies".into(),
             }),
-            wf_task_replay_latency: meter.histogram(MetricParameters {
+            wf_task_replay_latency: meter.histogram_duration(MetricParameters {
                 name: WF_TASK_REPLAY_LATENCY_NAME.into(),
-                unit: "ms".into(),
+                unit: "duration".into(),
                 description: "Histogram of workflow task replay latencies".into(),
             }),
-            wf_task_execution_latency: meter.histogram(MetricParameters {
+            wf_task_execution_latency: meter.histogram_duration(MetricParameters {
                 name: WF_TASK_EXECUTION_LATENCY_NAME.into(),
-                unit: "ms".into(),
+                unit: "duration".into(),
                 description: "Histogram of workflow task execution (not replay) latencies".into(),
             }),
             act_poll_no_task: meter.counter(MetricParameters {
                 name: "activity_poll_no_task".into(),
                 description: "Count of activity task queue poll timeouts (no new task)".into(),
                 unit: "".into(),
             }),
@@ -319,22 +296,22 @@
                 unit: "".into(),
             }),
             act_execution_failed: meter.counter(MetricParameters {
                 name: "activity_execution_failed".into(),
                 description: "Count of activity task execution failures".into(),
                 unit: "".into(),
             }),
-            act_sched_to_start_latency: meter.histogram(MetricParameters {
+            act_sched_to_start_latency: meter.histogram_duration(MetricParameters {
                 name: ACT_SCHED_TO_START_LATENCY_NAME.into(),
-                unit: "ms".into(),
+                unit: "duration".into(),
                 description: "Histogram of activity schedule-to-start latencies".into(),
             }),
-            act_exec_latency: meter.histogram(MetricParameters {
+            act_exec_latency: meter.histogram_duration(MetricParameters {
                 name: ACT_EXEC_LATENCY_NAME.into(),
-                unit: "ms".into(),
+                unit: "duration".into(),
                 description: "Histogram of activity execution latencies".into(),
             }),
             // name kept as worker start for compat with old sdk / what users expect
             worker_registered: meter.counter(MetricParameters {
                 name: "worker_start".into(),
                 description: "Count of the number of initialized workers".into(),
                 unit: "".into(),
@@ -379,14 +356,15 @@
 const KEY_NAMESPACE: &str = "namespace";
 const KEY_WF_TYPE: &str = "workflow_type";
 const KEY_TASK_QUEUE: &str = "task_queue";
 const KEY_ACT_TYPE: &str = "activity_type";
 const KEY_POLLER_TYPE: &str = "poller_type";
 const KEY_WORKER_TYPE: &str = "worker_type";
 const KEY_EAGER: &str = "eager";
+const KEY_TASK_FAILURE_TYPE: &str = "failure_reason";
 
 pub(crate) fn workflow_poller() -> MetricKeyValue {
     MetricKeyValue::new(KEY_POLLER_TYPE, "workflow_task")
 }
 pub(crate) fn workflow_sticky_poller() -> MetricKeyValue {
     MetricKeyValue::new(KEY_POLLER_TYPE, "sticky_workflow_task")
 }
@@ -410,225 +388,122 @@
 }
 pub(crate) fn local_activity_worker_type() -> MetricKeyValue {
     MetricKeyValue::new(KEY_WORKER_TYPE, "LocalActivityWorker")
 }
 pub(crate) fn eager(is_eager: bool) -> MetricKeyValue {
     MetricKeyValue::new(KEY_EAGER, is_eager)
 }
-
-const WF_E2E_LATENCY_NAME: &str = "workflow_endtoend_latency";
-const WF_TASK_SCHED_TO_START_LATENCY_NAME: &str = "workflow_task_schedule_to_start_latency";
-const WF_TASK_REPLAY_LATENCY_NAME: &str = "workflow_task_replay_latency";
-const WF_TASK_EXECUTION_LATENCY_NAME: &str = "workflow_task_execution_latency";
-const ACT_SCHED_TO_START_LATENCY_NAME: &str = "activity_schedule_to_start_latency";
-const ACT_EXEC_LATENCY_NAME: &str = "activity_execution_latency";
-const NUM_POLLERS_NAME: &str = "num_pollers";
-const TASK_SLOTS_AVAILABLE_NAME: &str = "worker_task_slots_available";
-const STICKY_CACHE_SIZE_NAME: &str = "sticky_cache_size";
-
-/// Artisanal, handcrafted latency buckets for workflow e2e latency which should expose a useful
-/// set of buckets for < 1 day runtime workflows. Beyond that, this metric probably isn't very
-/// helpful
-static WF_LATENCY_MS_BUCKETS: &[f64] = &[
-    100.,
-    500.,
-    1000.,
-    1500.,
-    2000.,
-    5000.,
-    10_000.,
-    30_000.,
-    60_000.,
-    120_000.,
-    300_000.,
-    600_000.,
-    1_800_000.,  // 30 min
-    3_600_000.,  //  1 hr
-    30_600_000., // 10 hrs
-    8.64e7,      // 24 hrs
-];
-
-/// Task latencies are expected to be fast, no longer than a second which was generally the deadlock
-/// timeout in old SDKs. Here it's a bit different since a WFT may represent multiple activations.
-static WF_TASK_MS_BUCKETS: &[f64] = &[1., 10., 20., 50., 100., 200., 500., 1000.];
-
-/// Activity are generally expected to take at least a little time, and sometimes quite a while,
-/// since they're doing side-effecty things, etc.
-static ACT_EXE_MS_BUCKETS: &[f64] = &[50., 100., 500., 1000., 5000., 10_000., 60_000.];
-
-/// Schedule-to-start latency buckets for both WFT and AT
-static TASK_SCHED_TO_START_MS_BUCKETS: &[f64] =
-    &[100., 500., 1000., 5000., 10_000., 100_000., 1_000_000.];
-
-/// Default buckets. Should never really be used as they will be meaningless for many things, but
-/// broadly it's trying to represent latencies in millis.
-pub(super) static DEFAULT_MS_BUCKETS: &[f64] = &[50., 100., 500., 1000., 2500., 10_000.];
-
-/// Returns the default histogram buckets that lang should use for a given metric name if they
-/// have not been overridden by the user.
-///
-/// The name must *not* be prefixed with `temporal_`
-pub fn default_buckets_for(histo_name: &str) -> &'static [f64] {
-    match histo_name {
-        WF_E2E_LATENCY_NAME => WF_LATENCY_MS_BUCKETS,
-        WF_TASK_EXECUTION_LATENCY_NAME | WF_TASK_REPLAY_LATENCY_NAME => WF_TASK_MS_BUCKETS,
-        WF_TASK_SCHED_TO_START_LATENCY_NAME | ACT_SCHED_TO_START_LATENCY_NAME => {
-            TASK_SCHED_TO_START_MS_BUCKETS
-        }
-        ACT_EXEC_LATENCY_NAME => ACT_EXE_MS_BUCKETS,
-        _ => DEFAULT_MS_BUCKETS,
+pub(crate) enum FailureReason {
+    Nondeterminism,
+    Workflow,
+}
+impl Display for FailureReason {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        let str = match self {
+            FailureReason::Nondeterminism => "NonDeterminismError",
+            FailureReason::Workflow => "WorkflowError",
+        };
+        write!(f, "{}", str)
     }
 }
-
-/// Chooses appropriate aggregators for our metrics
-#[derive(Debug, Clone, Default)]
-pub struct SDKAggSelector {
-    default: DefaultAggregationSelector,
-}
-impl AggregationSelector for SDKAggSelector {
-    fn aggregation(&self, kind: InstrumentKind) -> Aggregation {
-        match kind {
-            InstrumentKind::Histogram => Aggregation::ExplicitBucketHistogram {
-                boundaries: DEFAULT_MS_BUCKETS.to_vec(),
-                record_min_max: true,
-            },
-            _ => self.default.aggregation(kind),
+impl From<WorkflowTaskFailedCause> for FailureReason {
+    fn from(v: WorkflowTaskFailedCause) -> Self {
+        match v {
+            WorkflowTaskFailedCause::NonDeterministicError => FailureReason::Nondeterminism,
+            _ => FailureReason::Workflow,
         }
     }
 }
-
-fn histo_view(
-    metric_name: &'static str,
-    buckets: &[f64],
-) -> opentelemetry::metrics::Result<Box<dyn View>> {
-    new_view(
-        Instrument::new().name(format!("*{metric_name}")),
-        opentelemetry_sdk::metrics::Stream::new().aggregation(
-            Aggregation::ExplicitBucketHistogram {
-                boundaries: buckets.to_vec(),
-                record_min_max: true,
-            },
-        ),
-    )
-}
-
-pub(super) fn augment_meter_provider_with_defaults(
-    mpb: MeterProviderBuilder,
-    global_tags: &HashMap<String, String>,
-) -> opentelemetry::metrics::Result<MeterProviderBuilder> {
-    // Some histograms are actually gauges, but we have to use histograms otherwise they forget
-    // their value between collections since we don't use callbacks.
-    Ok(mpb
-        .with_view(histo_view(WF_E2E_LATENCY_NAME, WF_LATENCY_MS_BUCKETS)?)
-        .with_view(histo_view(
-            WF_TASK_EXECUTION_LATENCY_NAME,
-            WF_TASK_MS_BUCKETS,
-        )?)
-        .with_view(histo_view(WF_TASK_REPLAY_LATENCY_NAME, WF_TASK_MS_BUCKETS)?)
-        .with_view(histo_view(
-            WF_TASK_SCHED_TO_START_LATENCY_NAME,
-            TASK_SCHED_TO_START_MS_BUCKETS,
-        )?)
-        .with_view(histo_view(
-            ACT_SCHED_TO_START_LATENCY_NAME,
-            TASK_SCHED_TO_START_MS_BUCKETS,
-        )?)
-        .with_view(histo_view(ACT_EXEC_LATENCY_NAME, ACT_EXE_MS_BUCKETS)?)
-        .with_resource(default_resource(global_tags)))
-}
-
-/// OTel has no built-in synchronous Gauge. Histograms used to be able to serve that purpose, but
-/// they broke that. Lovely. So, we need to implement one by hand.
-pub(crate) struct MemoryGaugeU64 {
-    labels_to_values: Arc<RwLock<HashMap<AttributeSet, u64>>>,
-}
-
-impl MemoryGaugeU64 {
-    fn new(params: MetricParameters, meter: &Meter) -> Self {
-        let gauge = meter
-            .u64_observable_gauge(params.name)
-            .with_unit(Unit::new(params.unit))
-            .with_description(params.description)
-            .init();
-        let map = Arc::new(RwLock::new(HashMap::<AttributeSet, u64>::new()));
-        let map_c = map.clone();
-        meter
-            .register_callback(&[gauge.as_any()], move |o| {
-                // This whole thing is... extra stupid.
-                // See https://github.com/open-telemetry/opentelemetry-rust/issues/1181
-                // The performance is likely bad here, but, given this is only called when metrics
-                // are exported it should be livable for now.
-                let map_rlock = map_c.read();
-                for (kvs, val) in map_rlock.iter() {
-                    let kvs: Vec<_> = kvs
-                        .iter()
-                        .map(|(k, v)| KeyValue::new(k.clone(), v.clone()))
-                        .collect();
-                    o.observe_u64(&gauge, *val, kvs.as_slice())
-                }
-            })
-            .expect("instrument must exist we just created it");
-        MemoryGaugeU64 {
-            labels_to_values: map,
+pub(crate) fn failure_reason(reason: FailureReason) -> MetricKeyValue {
+    MetricKeyValue::new(KEY_TASK_FAILURE_TYPE, reason.to_string())
+}
+
+pub(super) const WF_E2E_LATENCY_NAME: &str = "workflow_endtoend_latency";
+pub(super) const WF_TASK_SCHED_TO_START_LATENCY_NAME: &str =
+    "workflow_task_schedule_to_start_latency";
+pub(super) const WF_TASK_REPLAY_LATENCY_NAME: &str = "workflow_task_replay_latency";
+pub(super) const WF_TASK_EXECUTION_LATENCY_NAME: &str = "workflow_task_execution_latency";
+pub(super) const ACT_SCHED_TO_START_LATENCY_NAME: &str = "activity_schedule_to_start_latency";
+pub(super) const ACT_EXEC_LATENCY_NAME: &str = "activity_execution_latency";
+pub(super) const NUM_POLLERS_NAME: &str = "num_pollers";
+pub(super) const TASK_SLOTS_AVAILABLE_NAME: &str = "worker_task_slots_available";
+pub(super) const STICKY_CACHE_SIZE_NAME: &str = "sticky_cache_size";
+
+/// Helps define buckets once in terms of millis, but also generates a seconds version
+macro_rules! define_latency_buckets {
+    ($(($metric_name:pat, $name:ident, $sec_name:ident, [$($bucket:expr),*])),*) => {
+        $(
+            pub(super) static $name: &[f64] = &[$($bucket,)*];
+            pub(super) static $sec_name: &[f64] = &[$( $bucket / 1000.0, )*];
+        )*
+
+        /// Returns the default histogram buckets that lang should use for a given metric name if
+        /// they have not been overridden by the user. If `use_seconds` is true, returns buckets
+        /// in terms of seconds rather than milliseconds.
+        ///
+        /// The name must *not* be prefixed with `temporal_`
+        pub fn default_buckets_for(histo_name: &str, use_seconds: bool) -> &'static [f64] {
+            match histo_name {
+                $(
+                    $metric_name => { if use_seconds { &$sec_name } else { &$name } },
+                )*
+            }
         }
-    }
-    fn record(&self, val: u64, kvs: &[KeyValue]) {
-        self.labels_to_values
-            .write()
-            .insert(AttributeSet::from(kvs), val);
-    }
+    };
 }
 
-/// Create an OTel meter that can be used as a [CoreMeter] to export metrics over OTLP.
-pub fn build_otlp_metric_exporter(
-    opts: OtelCollectorOptions,
-) -> Result<CoreOtelMeter, anyhow::Error> {
-    let exporter = opentelemetry_otlp::TonicExporterBuilder::default()
-        .with_endpoint(opts.url.to_string())
-        .with_metadata(MetadataMap::from_headers((&opts.headers).try_into()?))
-        .build_metrics_exporter(
-            Box::<SDKAggSelector>::default(),
-            Box::new(metric_temporality_to_selector(opts.metric_temporality)),
-        )?;
-    let reader = PeriodicReader::builder(exporter, runtime::Tokio)
-        .with_interval(opts.metric_periodicity)
-        .build();
-    let mp = augment_meter_provider_with_defaults(
-        MeterProvider::builder().with_reader(reader),
-        &opts.global_tags,
-    )?
-    .build();
-    Ok::<_, anyhow::Error>(CoreOtelMeter(mp.meter(TELEM_SERVICE_NAME)))
-}
-
-pub struct StartedPromServer {
-    pub meter: Arc<CoreOtelMeter>,
-    pub bound_addr: SocketAddr,
-    pub abort_handle: AbortHandle,
-}
-
-/// Builds and runs a prometheus endpoint which can be scraped by prom instances for metrics export.
-/// Returns the meter that can be used as a [CoreMeter].
-pub fn start_prometheus_metric_exporter(
-    opts: PrometheusExporterOptions,
-) -> Result<StartedPromServer, anyhow::Error> {
-    let (srv, exporter) = PromServer::new(&opts, SDKAggSelector::default())?;
-    let meter_provider = augment_meter_provider_with_defaults(
-        MeterProvider::builder().with_reader(exporter),
-        &opts.global_tags,
-    )?
-    .build();
-    let bound_addr = srv.bound_addr();
-    let handle = tokio::spawn(async move { srv.run().await });
-    Ok(StartedPromServer {
-        meter: Arc::new(CoreOtelMeter(meter_provider.meter(TELEM_SERVICE_NAME))),
-        bound_addr,
-        abort_handle: handle.abort_handle(),
-    })
-}
+define_latency_buckets!(
+    (
+        WF_E2E_LATENCY_NAME,
+        WF_LATENCY_MS_BUCKETS,
+        WF_LATENCY_S_BUCKETS,
+        [
+            100.,
+            500.,
+            1000.,
+            1500.,
+            2000.,
+            5000.,
+            10_000.,
+            30_000.,
+            60_000.,
+            120_000.,
+            300_000.,
+            600_000.,
+            1_800_000.,  // 30 min
+            3_600_000.,  //  1 hr
+            30_600_000., // 10 hrs
+            8.64e7       // 24 hrs
+        ]
+    ),
+    (
+        WF_TASK_EXECUTION_LATENCY_NAME | WF_TASK_REPLAY_LATENCY_NAME,
+        WF_TASK_MS_BUCKETS,
+        WF_TASK_S_BUCKETS,
+        [1., 10., 20., 50., 100., 200., 500., 1000.]
+    ),
+    (
+        ACT_EXEC_LATENCY_NAME,
+        ACT_EXE_MS_BUCKETS,
+        ACT_EXE_S_BUCKETS,
+        [50., 100., 500., 1000., 5000., 10_000., 60_000.]
+    ),
+    (
+        WF_TASK_SCHED_TO_START_LATENCY_NAME | ACT_SCHED_TO_START_LATENCY_NAME,
+        TASK_SCHED_TO_START_MS_BUCKETS,
+        TASK_SCHED_TO_START_S_BUCKETS,
+        [100., 500., 1000., 5000., 10_000., 100_000., 1_000_000.]
+    ),
+    (
+        _,
+        DEFAULT_MS_BUCKETS,
+        DEFAULT_S_BUCKETS,
+        [50., 100., 500., 1000., 2500., 10_000.]
+    )
+);
 
 /// Buffers [MetricEvent]s for periodic consumption by lang
 #[derive(Debug)]
 pub struct MetricsCallBuffer<I>
 where
     I: BufferInstrumentRef,
 {
@@ -664,15 +539,14 @@
         let hole = LazyBufferInstrument::hole();
         self.calls_tx.send(MetricEvent::Create {
             params,
             kind,
             populate_into: hole.clone(),
         });
         BufferInstrument {
-            kind,
             instrument_ref: hole,
             tx: self.calls_tx.clone(),
         }
     }
 }
 
 impl<I> CoreMeter for MetricsCallBuffer<I>
@@ -712,131 +586,105 @@
         Arc::new(self.new_instrument(params, MetricKind::Counter))
     }
 
     fn histogram(&self, params: MetricParameters) -> Arc<dyn Histogram> {
         Arc::new(self.new_instrument(params, MetricKind::Histogram))
     }
 
+    fn histogram_f64(&self, params: MetricParameters) -> Arc<dyn HistogramF64> {
+        Arc::new(self.new_instrument(params, MetricKind::HistogramF64))
+    }
+
+    fn histogram_duration(&self, params: MetricParameters) -> Arc<dyn HistogramDuration> {
+        Arc::new(self.new_instrument(params, MetricKind::HistogramDuration))
+    }
+
     fn gauge(&self, params: MetricParameters) -> Arc<dyn Gauge> {
         Arc::new(self.new_instrument(params, MetricKind::Gauge))
     }
+
+    fn gauge_f64(&self, params: MetricParameters) -> Arc<dyn GaugeF64> {
+        Arc::new(self.new_instrument(params, MetricKind::GaugeF64))
+    }
 }
 impl<I> MetricCallBufferer<I> for MetricsCallBuffer<I>
 where
     I: Send + Sync + BufferInstrumentRef,
 {
     fn retrieve(&self) -> Vec<MetricEvent<I>> {
         self.calls_rx.try_iter().collect()
     }
 }
 
 struct BufferInstrument<I: BufferInstrumentRef> {
-    kind: MetricKind,
     instrument_ref: LazyBufferInstrument<I>,
     tx: LogErrOnFullSender<MetricEvent<I>>,
 }
 impl<I> BufferInstrument<I>
 where
     I: Clone + BufferInstrumentRef,
 {
-    fn send(&self, value: u64, attributes: &MetricAttributes) {
+    fn send(&self, value: MetricUpdateVal, attributes: &MetricAttributes) {
         let attributes = match attributes {
             MetricAttributes::Buffer(l) => l.clone(),
             _ => panic!("MetricsCallBuffer only works with MetricAttributes::Lang"),
         };
         self.tx.send(MetricEvent::Update {
             instrument: self.instrument_ref.clone(),
-            update: match self.kind {
-                MetricKind::Counter => MetricUpdateVal::Delta(value),
-                MetricKind::Gauge | MetricKind::Histogram => MetricUpdateVal::Value(value),
-            },
+            update: value,
             attributes: attributes.clone(),
         });
     }
 }
 impl<I> Counter for BufferInstrument<I>
 where
     I: BufferInstrumentRef + Send + Sync + Clone,
 {
     fn add(&self, value: u64, attributes: &MetricAttributes) {
-        self.send(value, attributes)
+        self.send(MetricUpdateVal::Delta(value), attributes)
     }
 }
 impl<I> Gauge for BufferInstrument<I>
 where
     I: BufferInstrumentRef + Send + Sync + Clone,
 {
     fn record(&self, value: u64, attributes: &MetricAttributes) {
-        self.send(value, attributes)
+        self.send(MetricUpdateVal::Value(value), attributes)
+    }
+}
+impl<I> GaugeF64 for BufferInstrument<I>
+where
+    I: BufferInstrumentRef + Send + Sync + Clone,
+{
+    fn record(&self, value: f64, attributes: &MetricAttributes) {
+        self.send(MetricUpdateVal::ValueF64(value), attributes)
     }
 }
 impl<I> Histogram for BufferInstrument<I>
 where
     I: BufferInstrumentRef + Send + Sync + Clone,
 {
     fn record(&self, value: u64, attributes: &MetricAttributes) {
-        self.send(value, attributes)
+        self.send(MetricUpdateVal::Value(value), attributes)
     }
 }
-
-#[derive(Debug)]
-pub struct CoreOtelMeter(Meter);
-impl CoreMeter for CoreOtelMeter {
-    fn new_attributes(&self, attribs: NewAttributes) -> MetricAttributes {
-        MetricAttributes::OTel {
-            kvs: Arc::new(attribs.attributes.into_iter().map(KeyValue::from).collect()),
-        }
-    }
-
-    fn extend_attributes(
-        &self,
-        existing: MetricAttributes,
-        attribs: NewAttributes,
-    ) -> MetricAttributes {
-        if let MetricAttributes::OTel { mut kvs } = existing {
-            Arc::make_mut(&mut kvs).extend(attribs.attributes.into_iter().map(Into::into));
-            MetricAttributes::OTel { kvs }
-        } else {
-            dbg_panic!("Must use OTel attributes with an OTel metric implementation");
-            existing
-        }
-    }
-
-    fn counter(&self, params: MetricParameters) -> Arc<dyn Counter> {
-        Arc::new(
-            self.0
-                .u64_counter(params.name)
-                .with_unit(Unit::new(params.unit))
-                .with_description(params.description)
-                .init(),
-        )
-    }
-
-    fn histogram(&self, params: MetricParameters) -> Arc<dyn Histogram> {
-        Arc::new(
-            self.0
-                .u64_histogram(params.name)
-                .with_unit(Unit::new(params.unit))
-                .with_description(params.description)
-                .init(),
-        )
-    }
-
-    fn gauge(&self, params: MetricParameters) -> Arc<dyn Gauge> {
-        Arc::new(MemoryGaugeU64::new(params, &self.0))
+impl<I> HistogramF64 for BufferInstrument<I>
+where
+    I: BufferInstrumentRef + Send + Sync + Clone,
+{
+    fn record(&self, value: f64, attributes: &MetricAttributes) {
+        self.send(MetricUpdateVal::ValueF64(value), attributes)
     }
 }
-
-impl Gauge for MemoryGaugeU64 {
-    fn record(&self, value: u64, attributes: &MetricAttributes) {
-        if let MetricAttributes::OTel { kvs } = attributes {
-            self.record(value, kvs);
-        } else {
-            dbg_panic!("Must use OTel attributes with an OTel metric implementation");
-        }
+impl<I> HistogramDuration for BufferInstrument<I>
+where
+    I: BufferInstrumentRef + Send + Sync + Clone,
+{
+    fn record(&self, value: Duration, attributes: &MetricAttributes) {
+        self.send(MetricUpdateVal::Duration(value), attributes)
     }
 }
 
 #[derive(Debug, derive_more::Constructor)]
 pub(crate) struct PrefixedMetricsMeter<CM> {
     prefix: String,
     meter: CM,
@@ -860,18 +708,33 @@
     }
 
     fn histogram(&self, mut params: MetricParameters) -> Arc<dyn Histogram> {
         params.name = (self.prefix.clone() + &*params.name).into();
         self.meter.histogram(params)
     }
 
+    fn histogram_f64(&self, mut params: MetricParameters) -> Arc<dyn HistogramF64> {
+        params.name = (self.prefix.clone() + &*params.name).into();
+        self.meter.histogram_f64(params)
+    }
+
+    fn histogram_duration(&self, mut params: MetricParameters) -> Arc<dyn HistogramDuration> {
+        params.name = (self.prefix.clone() + &*params.name).into();
+        self.meter.histogram_duration(params)
+    }
+
     fn gauge(&self, mut params: MetricParameters) -> Arc<dyn Gauge> {
         params.name = (self.prefix.clone() + &*params.name).into();
         self.meter.gauge(params)
     }
+
+    fn gauge_f64(&self, mut params: MetricParameters) -> Arc<dyn GaugeF64> {
+        params.name = (self.prefix.clone() + &*params.name).into();
+        self.meter.gauge_f64(params)
+    }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use std::any::Any;
     use temporal_sdk_core_api::telemetry::{
@@ -966,17 +829,18 @@
         );
         a2.set(Arc::new(DummyCustomAttrs(2))).unwrap();
         assert_matches!(
             &events[1],
             MetricEvent::Update {
                 instrument,
                 attributes,
-                update: MetricUpdateVal::Value(1000) // milliseconds
+                update: MetricUpdateVal::Duration(d)
             }
             if DummyCustomAttrs::as_id(attributes) == 2 && instrument.get().0 == 11
+               && d == &Duration::from_secs(1)
         );
     }
 
     #[test]
     fn metric_buffer() {
         let call_buffer = MetricsCallBuffer::new(10);
         let ctr = call_buffer.counter(MetricParameters {
@@ -990,23 +854,29 @@
             unit: "flubarbs".into(),
         });
         let gauge = call_buffer.gauge(MetricParameters {
             name: "gauge".into(),
             description: "a counter".into(),
             unit: "bleezles".into(),
         });
+        let histo_dur = call_buffer.histogram_duration(MetricParameters {
+            name: "histo_dur".into(),
+            description: "a duration histogram".into(),
+            unit: "seconds".into(),
+        });
         let attrs_1 = call_buffer.new_attributes(NewAttributes {
             attributes: vec![MetricKeyValue::new("hi", "yo")],
         });
         let attrs_2 = call_buffer.new_attributes(NewAttributes {
             attributes: vec![MetricKeyValue::new("run", "fast")],
         });
         ctr.add(1, &attrs_1);
         histo.record(2, &attrs_1);
         gauge.record(3, &attrs_2);
+        histo_dur.record(Duration::from_secs_f64(1.2), &attrs_1);
 
         let mut calls = call_buffer.retrieve();
         calls.reverse();
         let ctr_1 = assert_matches!(
             calls.pop(),
             Some(MetricEvent::Create {
                 params,
@@ -1035,14 +905,25 @@
                 populate_into,
                 kind: MetricKind::Gauge
             })
             if params.name == "gauge"
             => populate_into
         );
         gauge_3.set(Arc::new(DummyInstrumentRef(3))).unwrap();
+        let hist_4 = assert_matches!(
+            calls.pop(),
+            Some(MetricEvent::Create {
+                params,
+                populate_into,
+                kind: MetricKind::HistogramDuration
+            })
+            if params.name == "histo_dur"
+            => populate_into
+        );
+        hist_4.set(Arc::new(DummyInstrumentRef(4))).unwrap();
         let a1 = assert_matches!(
             calls.pop(),
             Some(MetricEvent::CreateAttributes {
                 populate_into,
                 append_from: None,
                 attributes
             })
@@ -1082,11 +963,21 @@
         assert_matches!(
             calls.pop(),
             Some(MetricEvent::Update{
                 instrument,
                 attributes,
                 update: MetricUpdateVal::Value(3)
             })
-            if DummyCustomAttrs::as_id(&attributes) == 2&& instrument.get().0 == 3
+            if DummyCustomAttrs::as_id(&attributes) == 2 && instrument.get().0 == 3
+        );
+        assert_matches!(
+            calls.pop(),
+            Some(MetricEvent::Update{
+                instrument,
+                attributes,
+                update: MetricUpdateVal::Duration(d)
+            })
+            if DummyCustomAttrs::as_id(&attributes) == 1 && instrument.get().0 == 4
+               && d == Duration::from_secs_f64(1.2)
         );
     }
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/telemetry/mod.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/telemetry/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 //! This module helps with the initialization and management of telemetry. IE: Metrics and tracing.
 //! Logs from core are all traces, which may be exported to the console, in memory, or externally.
 
 mod log_export;
 pub(crate) mod metrics;
+#[cfg(feature = "otel")]
+mod otel;
+#[cfg(feature = "otel")]
 mod prometheus_server;
 
-pub use metrics::{
-    build_otlp_metric_exporter, default_buckets_for, start_prometheus_metric_exporter,
-    MetricsCallBuffer,
-};
+#[cfg(feature = "otel")]
+pub use metrics::{default_buckets_for, MetricsCallBuffer};
+#[cfg(feature = "otel")]
+pub use otel::{build_otlp_metric_exporter, start_prometheus_metric_exporter};
 
 pub use log_export::{CoreLogBuffer, CoreLogBufferedConsumer, CoreLogStreamConsumer};
 
 use crate::telemetry::{log_export::CoreLogConsumerLayer, metrics::PrefixedMetricsMeter};
 use itertools::Itertools;
-use once_cell::sync::OnceCell;
-use opentelemetry::KeyValue;
-use opentelemetry_sdk::{
-    metrics::{data::Temporality, reader::TemporalitySelector, InstrumentKind},
-    Resource,
-};
 use parking_lot::Mutex;
 use std::{
     cell::RefCell,
-    collections::{HashMap, VecDeque},
+    collections::VecDeque,
     env,
     sync::{
         atomic::{AtomicBool, Ordering},
         Arc,
     },
 };
 use temporal_sdk_core_api::telemetry::{
     metrics::{CoreMeter, MetricKeyValue, NewAttributes, TemporalMeter},
-    CoreLog, CoreTelemetry, Logger, MetricTemporality, TelemetryOptions,
+    CoreLog, CoreTelemetry, Logger, TelemetryOptions,
 };
 use tracing::{Level, Subscriber};
 use tracing_subscriber::{layer::SubscriberExt, EnvFilter, Layer};
 
 const TELEM_SERVICE_NAME: &str = "temporal-core-sdk";
 
 const FORWARD_LOG_BUFFER_SIZE: usize = 2048;
@@ -120,15 +117,16 @@
         } else {
             vec![]
         }
     }
 }
 
 thread_local! {
-    static SUB_GUARD: RefCell<Option<tracing::subscriber::DefaultGuard>> = RefCell::new(None);
+    static SUB_GUARD: RefCell<Option<tracing::subscriber::DefaultGuard>> =
+        const { RefCell::new(None) };
 }
 /// Set the trace subscriber for the current thread. This must be done in every thread which uses
 /// core stuff, otherwise traces/logs will not be collected on that thread. For example, if using
 /// a multithreaded Tokio runtime, you should ensure that said runtime uses
 /// [on_thread_start](https://docs.rs/tokio/latest/tokio/runtime/struct.Builder.html#method.on_thread_start)
 /// or a similar mechanism to call this for each thread within the runtime.
 pub fn set_trace_subscriber_for_current_thread(sub: impl Subscriber + Send + Sync + 'static) {
@@ -248,39 +246,14 @@
         if let Some(ts) = ti.trace_subscriber() {
             tracing::subscriber::set_global_default(ts)?;
         }
     }
     Ok(())
 }
 
-fn default_resource_kvs() -> &'static [KeyValue] {
-    static INSTANCE: OnceCell<[KeyValue; 1]> = OnceCell::new();
-    INSTANCE.get_or_init(|| [KeyValue::new("service.name", TELEM_SERVICE_NAME)])
-}
-
-fn default_resource(override_values: &HashMap<String, String>) -> Resource {
-    let override_kvs = override_values
-        .iter()
-        .map(|(k, v)| KeyValue::new(k.clone(), v.clone()));
-    Resource::new(default_resource_kvs().iter().cloned()).merge(&Resource::new(override_kvs))
-}
-
-#[derive(Clone)]
-struct ConstantTemporality(Temporality);
-impl TemporalitySelector for ConstantTemporality {
-    fn temporality(&self, _: InstrumentKind) -> Temporality {
-        self.0
-    }
-}
-fn metric_temporality_to_selector(t: MetricTemporality) -> impl TemporalitySelector + Clone {
-    match t {
-        MetricTemporality::Cumulative => ConstantTemporality(Temporality::Cumulative),
-        MetricTemporality::Delta => ConstantTemporality(Temporality::Delta),
-    }
-}
 #[cfg(test)]
 pub use test_initters::*;
 
 /// A trait for using [Display] on the contents of vecs, etc, which don't implement it.
 ///
 /// Dislike this, but, there doesn't seem to be a great alternative. Calling itertools format
 /// inline in an `event!` macro can panic because it gets evaluated twice somehow.
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/telemetry/prometheus_server.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/telemetry/prometheus_server.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-use hyper::{
-    header::CONTENT_TYPE,
-    server::conn::AddrIncoming,
-    service::{make_service_fn, service_fn},
-    Body, Method, Request, Response, Server,
+use http_body_util::Full;
+use hyper::{body::Bytes, header::CONTENT_TYPE, service::service_fn, Method, Request, Response};
+use hyper_util::{
+    rt::{TokioExecutor, TokioIo},
+    server::conn::auto,
 };
 use opentelemetry_prometheus::PrometheusExporter;
 use opentelemetry_sdk::metrics::reader::AggregationSelector;
 use prometheus::{Encoder, Registry, TextEncoder};
-use std::{convert::Infallible, net::SocketAddr};
+use std::net::{SocketAddr, TcpListener};
 use temporal_sdk_core_api::telemetry::PrometheusExporterOptions;
+use tokio::io;
 
 /// Exposes prometheus metrics for scraping
 pub(super) struct PromServer {
-    bound_addr: AddrIncoming,
+    listener: TcpListener,
     registry: Registry,
 }
 
 impl PromServer {
-    pub fn new(
+    pub(super) fn new(
         opts: &PrometheusExporterOptions,
-        aggregation: impl AggregationSelector + Send + Sync + 'static,
+        aggregation: impl AggregationSelector + 'static,
     ) -> Result<(Self, PrometheusExporter), anyhow::Error> {
         let registry = Registry::new();
         let exporter = opentelemetry_prometheus::exporter()
             .with_aggregation_selector(aggregation)
             .without_scope_info()
             .with_registry(registry.clone());
         let exporter = if !opts.counters_total_suffix {
@@ -32,58 +33,70 @@
             exporter
         };
         let exporter = if !opts.unit_suffix {
             exporter.without_units()
         } else {
             exporter
         };
-        let bound_addr = AddrIncoming::bind(&opts.socket_addr)?;
         Ok((
             Self {
-                bound_addr,
+                listener: TcpListener::bind(opts.socket_addr)?,
                 registry,
             },
             exporter.build()?,
         ))
     }
 
-    pub async fn run(self) -> hyper::Result<()> {
+    pub(super) async fn run(self) -> Result<(), anyhow::Error> {
         // Spin up hyper server to serve metrics for scraping. We use hyper since we already depend
         // on it via Tonic.
-        let svc = make_service_fn(move |_conn| {
+        self.listener.set_nonblocking(true)?;
+        let listener = tokio::net::TcpListener::from_std(self.listener)?;
+        loop {
+            let (stream, _) = listener.accept().await?;
+            let io = TokioIo::new(stream);
             let regclone = self.registry.clone();
-            async move { Ok::<_, Infallible>(service_fn(move |req| metrics_req(req, regclone.clone()))) }
-        });
-        let server = Server::builder(self.bound_addr).serve(svc);
-        server.await
+            tokio::task::spawn(async move {
+                let server = auto::Builder::new(TokioExecutor::new());
+                if let Err(e) = server
+                    .serve_connection(
+                        io,
+                        service_fn(move |req| metrics_req(req, regclone.clone())),
+                    )
+                    .await
+                {
+                    warn!("Error serving metrics connection: {:?}", e);
+                }
+            });
+        }
     }
 
-    pub fn bound_addr(&self) -> SocketAddr {
-        self.bound_addr.local_addr()
+    pub(super) fn bound_addr(&self) -> io::Result<SocketAddr> {
+        self.listener.local_addr()
     }
 }
 
 /// Serves prometheus metrics in the expected format for scraping
 async fn metrics_req(
-    req: Request<Body>,
+    req: Request<hyper::body::Incoming>,
     registry: Registry,
-) -> Result<Response<Body>, hyper::Error> {
+) -> Result<Response<Full<Bytes>>, hyper::Error> {
     let response = match (req.method(), req.uri().path()) {
         (&Method::GET, "/metrics") => {
             let mut buffer = vec![];
             let encoder = TextEncoder::new();
             let metric_families = registry.gather();
             encoder.encode(&metric_families, &mut buffer).unwrap();
 
             Response::builder()
                 .status(200)
                 .header(CONTENT_TYPE, encoder.format_type())
-                .body(Body::from(buffer))
+                .body(buffer.into())
                 .unwrap()
         }
         _ => Response::builder()
             .status(404)
-            .body(Body::empty())
+            .body(vec![].into())
             .expect("Can't fail to construct empty resp"),
     };
     Ok(response)
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/test_help/mod.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/test_help/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 use temporal_sdk::interceptors::FailOnNondeterminismInterceptor;
 use temporal_sdk_core_api::{
     errors::{PollActivityError, PollWfError},
     Worker as WorkerTrait,
 };
 use temporal_sdk_core_protos::{
     coresdk::{
-        workflow_activation::WorkflowActivation,
+        workflow_activation::{workflow_activation_job, WorkflowActivation},
         workflow_commands::workflow_command,
         workflow_completion::{self, workflow_activation_completion, WorkflowActivationCompletion},
     },
     temporal::api::{
         common::v1::WorkflowExecution,
         enums::v1::WorkflowTaskFailedCause,
         failure::v1::Failure,
@@ -51,66 +51,69 @@
         },
     },
 };
 use temporal_sdk_core_test_utils::TestWorker;
 use tokio::sync::{mpsc::unbounded_channel, Notify};
 use tokio_stream::wrappers::UnboundedReceiverStream;
 
-pub const TEST_Q: &str = "q";
+pub(crate) const TEST_Q: &str = "q";
 
-pub fn test_worker_cfg() -> WorkerConfigBuilder {
+pub(crate) fn test_worker_cfg() -> WorkerConfigBuilder {
     let mut wcb = WorkerConfigBuilder::default();
     wcb.namespace("default")
         .task_queue(TEST_Q)
         .worker_build_id("test_bin_id")
         .ignore_evicts_on_shutdown(true)
         // Serial polling since it makes mocking much easier.
         .max_concurrent_wft_polls(1_usize);
     wcb
 }
 
 /// When constructing responses for mocks, indicates how a given response should be built
 #[derive(derive_more::From)]
 #[allow(clippy::large_enum_variant)] // Test only code, whatever.
-pub enum ResponseType {
+pub(crate) enum ResponseType {
     ToTaskNum(usize),
     /// Returns just the history after the WFT completed of the provided task number - 1, through to
     /// the next WFT started. Simulating the incremental history for just the provided task number
     #[from(ignore)]
     OneTask(usize),
     /// Waits until the future resolves before responding as `ToTaskNum` with the provided number
     UntilResolved(BoxFuture<'static, ()>, usize),
     /// Waits until the future resolves before responding with the provided response
     UntilResolvedRaw(BoxFuture<'static, ()>, PollWorkflowTaskQueueResponse),
     AllHistory,
     Raw(PollWorkflowTaskQueueResponse),
 }
+
 #[derive(Eq, PartialEq, Hash)]
-pub enum HashableResponseType {
+pub(crate) enum HashableResponseType {
     ToTaskNum(usize),
     OneTask(usize),
     UntilResolved(usize),
     UntilResolvedRaw(TaskToken),
     AllHistory,
     Raw(TaskToken),
 }
+
 impl ResponseType {
-    pub fn hashable(&self) -> HashableResponseType {
+    fn hashable(&self) -> HashableResponseType {
         match self {
             ResponseType::ToTaskNum(x) => HashableResponseType::ToTaskNum(*x),
             ResponseType::OneTask(x) => HashableResponseType::OneTask(*x),
             ResponseType::AllHistory => HashableResponseType::AllHistory,
             ResponseType::Raw(r) => HashableResponseType::Raw(r.task_token.clone().into()),
             ResponseType::UntilResolved(_, x) => HashableResponseType::UntilResolved(*x),
             ResponseType::UntilResolvedRaw(_, r) => {
                 HashableResponseType::UntilResolvedRaw(r.task_token.clone().into())
             }
         }
     }
 }
+
 impl From<&usize> for ResponseType {
     fn from(u: &usize) -> Self {
         Self::ToTaskNum(*u)
     }
 }
 
 /// Given identifiers for a workflow/run, and a test history builder, construct an instance of
@@ -135,15 +138,18 @@
         0,
     );
     mock_worker(mock_holder)
 }
 
 pub(crate) fn build_fake_sdk(mock_cfg: MockPollCfg) -> temporal_sdk::Worker {
     let mut mock = build_mock_pollers(mock_cfg);
-    mock.worker_cfg(|c| c.max_cached_workflows = 1);
+    mock.worker_cfg(|c| {
+        c.max_cached_workflows = 1;
+        c.ignore_evicts_on_shutdown = false;
+    });
     let core = mock_worker(mock);
     let mut worker = temporal_sdk::Worker::new_from_core(Arc::new(core), "replay_q".to_string());
     worker.set_worker_interceptor(FailOnNondeterminismInterceptor {});
     worker
 }
 
 pub(crate) fn mock_worker(mocks: MocksHolder) -> Worker {
@@ -175,55 +181,57 @@
     poll_cfg.using_rust_sdk = true;
     let mut mock = build_mock_pollers(poll_cfg);
     mock.worker_cfg(mutator);
     let core = mock_worker(mock);
     TestWorker::new(Arc::new(core), TEST_Q.to_string())
 }
 
-pub struct FakeWfResponses {
-    pub wf_id: String,
-    pub hist: TestHistoryBuilder,
-    pub response_batches: Vec<ResponseType>,
+pub(crate) struct FakeWfResponses {
+    pub(crate) wf_id: String,
+    pub(crate) hist: TestHistoryBuilder,
+    pub(crate) response_batches: Vec<ResponseType>,
 }
 
 // TODO: Should be all-internal to this module
-pub struct MocksHolder {
+pub(crate) struct MocksHolder {
     client: Arc<dyn WorkerClient>,
     inputs: MockWorkerInputs,
-    pub outstanding_task_map: Option<OutstandingWFTMap>,
+    pub(crate) outstanding_task_map: Option<OutstandingWFTMap>,
 }
 
 impl MocksHolder {
-    pub fn worker_cfg(&mut self, mutator: impl FnOnce(&mut WorkerConfig)) {
+    pub(crate) fn worker_cfg(&mut self, mutator: impl FnOnce(&mut WorkerConfig)) {
         mutator(&mut self.inputs.config);
     }
-    pub fn set_act_poller(&mut self, poller: BoxedPoller<PollActivityTaskQueueResponse>) {
+
+    pub(crate) fn set_act_poller(&mut self, poller: BoxedPoller<PollActivityTaskQueueResponse>) {
         self.inputs.act_poller = Some(poller);
     }
+
     /// Can be used for tests that need to avoid auto-shutdown due to running out of mock responses
-    pub fn make_wft_stream_interminable(&mut self) {
+    pub(crate) fn make_wft_stream_interminable(&mut self) {
         let old_stream = std::mem::replace(&mut self.inputs.wft_stream, stream::pending().boxed());
         self.inputs.wft_stream = old_stream.chain(stream::pending()).boxed();
     }
 }
 
-pub struct MockWorkerInputs {
-    pub wft_stream: BoxStream<'static, Result<ValidPollWFTQResponse, tonic::Status>>,
-    pub act_poller: Option<BoxedPoller<PollActivityTaskQueueResponse>>,
-    pub config: WorkerConfig,
+pub(crate) struct MockWorkerInputs {
+    pub(crate) wft_stream: BoxStream<'static, Result<ValidPollWFTQResponse, tonic::Status>>,
+    pub(crate) act_poller: Option<BoxedPoller<PollActivityTaskQueueResponse>>,
+    pub(crate) config: WorkerConfig,
 }
 
 impl Default for MockWorkerInputs {
     fn default() -> Self {
         Self::new(stream::empty().boxed())
     }
 }
 
 impl MockWorkerInputs {
-    pub fn new(
+    pub(crate) fn new(
         wft_stream: BoxStream<'static, Result<ValidPollWFTQResponse, tonic::Status>>,
     ) -> Self {
         Self {
             wft_stream,
             act_poller: None,
             config: test_worker_cfg().build().unwrap(),
         }
@@ -309,25 +317,25 @@
         } else {
             async { None }.boxed()
         }
     });
     Box::new(mock_poller) as BoxedPoller<T>
 }
 
-pub fn mock_poller<T>() -> MockPoller<T>
+pub(crate) fn mock_poller<T>() -> MockPoller<T>
 where
     T: Send + Sync + 'static,
 {
     let mut mock_poller = MockPoller::new();
     mock_poller.expect_shutdown_box().return_const(());
     mock_poller.expect_notify_shutdown().return_const(());
     mock_poller
 }
 
-pub fn mock_manual_poller<T>() -> MockManualPoller<T>
+pub(crate) fn mock_manual_poller<T>() -> MockManualPoller<T>
 where
     T: Send + Sync + 'static,
 {
     let mut mock_poller = MockManualPoller::new();
     mock_poller
         .expect_shutdown_box()
         .returning(|| async {}.boxed());
@@ -368,33 +376,33 @@
     let mut mh = MockPollCfg::from_resp_batches(wf_id, t, response_batches, mock_client);
     mh.enforce_correct_number_of_polls = enforce_num_polls;
     build_mock_pollers(mh)
 }
 
 #[allow(clippy::type_complexity)]
 pub(crate) struct MockPollCfg {
-    pub hists: Vec<FakeWfResponses>,
-    pub enforce_correct_number_of_polls: bool,
-    pub num_expected_fails: usize,
-    pub num_expected_legacy_query_resps: usize,
-    pub mock_client: MockWorkerClient,
+    pub(crate) hists: Vec<FakeWfResponses>,
+    pub(crate) enforce_correct_number_of_polls: bool,
+    pub(crate) num_expected_fails: usize,
+    pub(crate) num_expected_legacy_query_resps: usize,
+    pub(crate) mock_client: MockWorkerClient,
     /// All calls to fail WFTs must match this predicate
-    pub expect_fail_wft_matcher:
+    pub(crate) expect_fail_wft_matcher:
         Box<dyn Fn(&TaskToken, &WorkflowTaskFailedCause, &Option<Failure>) -> bool + Send>,
-    pub completion_asserts: Option<Box<dyn FnMut(&WorkflowTaskCompletion) + Send>>,
-    pub num_expected_completions: Option<TimesRange>,
+    pub(crate) completion_asserts: Option<Box<dyn FnMut(&WorkflowTaskCompletion) + Send>>,
+    pub(crate) num_expected_completions: Option<TimesRange>,
     /// If being used with the Rust SDK, this is set true. It ensures pollers will not error out
     /// early with no work, since we cannot know the exact number of times polling will happen.
     /// Instead, they will just block forever.
-    pub using_rust_sdk: bool,
-    pub make_poll_stream_interminable: bool,
+    pub(crate) using_rust_sdk: bool,
+    pub(crate) make_poll_stream_interminable: bool,
 }
 
 impl MockPollCfg {
-    pub fn new(
+    pub(crate) fn new(
         hists: Vec<FakeWfResponses>,
         enforce_correct_number_of_polls: bool,
         num_expected_fails: usize,
     ) -> Self {
         Self {
             hists,
             enforce_correct_number_of_polls,
@@ -406,28 +414,28 @@
             num_expected_completions: None,
             using_rust_sdk: false,
             make_poll_stream_interminable: false,
         }
     }
 
     /// Builds a config which will hand out each WFT in the history builder one by one
-    pub fn from_hist_builder(t: TestHistoryBuilder) -> Self {
+    pub(crate) fn from_hist_builder(t: TestHistoryBuilder) -> Self {
         let full_hist_info = t.get_full_history_info().unwrap();
         let tasks = 1..=full_hist_info.wf_task_count();
         Self::from_resp_batches("fake_wf_id", t, tasks, mock_workflow_client())
     }
 
-    pub fn from_resps(
+    pub(crate) fn from_resps(
         t: TestHistoryBuilder,
         resps: impl IntoIterator<Item = impl Into<ResponseType>>,
     ) -> Self {
         Self::from_resp_batches("fake_wf_id", t, resps, mock_workflow_client())
     }
 
-    pub fn from_resp_batches(
+    pub(crate) fn from_resp_batches(
         wf_id: &str,
         t: TestHistoryBuilder,
         resps: impl IntoIterator<Item = impl Into<ResponseType>>,
         mock_client: MockWorkerClient,
     ) -> Self {
         Self {
             hists: vec![FakeWfResponses {
@@ -443,15 +451,15 @@
             completion_asserts: None,
             num_expected_completions: None,
             using_rust_sdk: false,
             make_poll_stream_interminable: false,
         }
     }
 
-    pub fn completion_asserts_from_expectations(
+    pub(crate) fn completion_asserts_from_expectations(
         &mut self,
         builder_fn: impl FnOnce(CompletionAssertsBuilder<'_>),
     ) {
         let builder = CompletionAssertsBuilder {
             dest: &mut self.completion_asserts,
             assertions: Default::default(),
         };
@@ -460,56 +468,63 @@
 }
 
 #[allow(clippy::type_complexity)]
 pub(crate) struct CompletionAssertsBuilder<'a> {
     dest: &'a mut Option<Box<dyn FnMut(&WorkflowTaskCompletion) + Send>>,
     assertions: VecDeque<Box<dyn FnOnce(&WorkflowTaskCompletion) + Send>>,
 }
+
 impl CompletionAssertsBuilder<'_> {
-    pub fn then(
+    pub(crate) fn then(
         &mut self,
         assert: impl FnOnce(&WorkflowTaskCompletion) + Send + 'static,
     ) -> &mut Self {
         self.assertions.push_back(Box::new(assert));
         self
     }
 }
+
 impl Drop for CompletionAssertsBuilder<'_> {
     fn drop(&mut self) {
         let mut asserts = std::mem::take(&mut self.assertions);
         *self.dest = Some(Box::new(move |wtc| {
             if let Some(fun) = asserts.pop_front() {
                 fun(wtc)
             }
         }));
     }
 }
 
 #[derive(Default, Clone)]
-pub struct OutstandingWFTMap {
+pub(crate) struct OutstandingWFTMap {
     map: Arc<RwLock<BiMap<String, TaskToken>>>,
     waker: Arc<Notify>,
     all_work_delivered: Arc<AtomicBool>,
 }
+
 impl OutstandingWFTMap {
     fn has_run(&self, run_id: &str) -> bool {
         self.map.read().contains_left(run_id)
     }
+
     fn put_token(&self, run_id: String, token: TaskToken) {
         self.map.write().insert(run_id, token);
     }
+
     fn release_token(&self, token: &TaskToken) {
         self.map.write().remove_by_right(token);
         self.waker.notify_one();
     }
-    pub fn release_run(&self, run_id: &str) {
+
+    pub(crate) fn release_run(&self, run_id: &str) {
         self.map.write().remove_by_left(run_id);
         self.waker.notify_waiters();
     }
-    pub fn all_work_delivered(&self) -> bool {
+
+    pub(crate) fn all_work_delivered(&self) -> bool {
         self.all_work_delivered.load(Ordering::Acquire)
     }
 }
 
 struct EnsuresWorkDoneWFTStream {
     inner: UnboundedReceiverStream<ValidPollWFTQResponse>,
     all_work_was_completed: Arc<AtomicBool>,
@@ -686,18 +701,19 @@
     };
     if cfg.make_poll_stream_interminable {
         mh.make_wft_stream_interminable();
     }
     mh
 }
 
-pub struct QueueResponse<T> {
-    pub resp: T,
-    pub delay_until: Option<BoxFuture<'static, ()>>,
+pub(crate) struct QueueResponse<T> {
+    pub(crate) resp: T,
+    pub(crate) delay_until: Option<BoxFuture<'static, ()>>,
 }
+
 impl<T> From<T> for QueueResponse<T> {
     fn from(resp: T) -> Self {
         QueueResponse {
             resp,
             delay_until: None,
         }
     }
@@ -728,15 +744,15 @@
     T: Debug,
 {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         self.resp.fmt(f)
     }
 }
 
-pub fn hist_to_poll_resp(
+pub(crate) fn hist_to_poll_resp(
     t: &TestHistoryBuilder,
     wf_id: impl Into<String>,
     response_type: ResponseType,
 ) -> QueueResponse<PollWorkflowTaskQueueResponse> {
     let run_id = t.get_orig_run_id();
     let wf = WorkflowExecution {
         workflow_id: wf_id.into(),
@@ -824,26 +840,31 @@
             let complete_is_failure = !reply.is_success();
             // Only send activation failures once
             if executed_failures.contains(&i) {
                 continue;
             }
 
             let mut res = worker.poll_workflow_activation().await.unwrap();
-            let contains_eviction = res.eviction_index();
+            if res.jobs.iter().any(|j| {
+                matches!(
+                    j.variant,
+                    Some(workflow_activation_job::Variant::RemoveFromCache(_))
+                )
+            }) && res.jobs.len() > 1
+            {
+                panic!("Saw an activation with an eviction & other work! {res:?}");
+            }
+            let is_eviction = res.is_only_eviction();
 
             let mut do_release = false;
-            if let Some(eviction_job_ix) = contains_eviction {
-                // If the job list has an eviction, make sure it was the last item in the list
-                // then remove it, since in the tests we don't explicitly specify evict assertions
-                assert_eq!(
-                    eviction_job_ix,
-                    res.jobs.len() - 1,
-                    "Eviction job was not last job in job list"
-                );
-                res.jobs.remove(eviction_job_ix);
+
+            if is_eviction {
+                // If the job is an eviction, clear it, since in the tests we don't explicitly
+                // specify evict assertions
+                res.jobs.clear();
                 do_release = true;
             }
 
             // TODO: Can remove this if?
             if !res.jobs.is_empty() {
                 asserter(&res);
             }
@@ -866,15 +887,15 @@
             if do_release {
                 if let Some(omap) = outstanding_map.as_ref() {
                     omap.release_run(&res.run_id);
                 }
             }
             // Restart assertions from the beginning if it was an eviction (and workflow execution
             // isn't over)
-            if contains_eviction.is_some() && !ends_execution {
+            if is_eviction && !ends_execution {
                 continue 'outer;
             }
 
             if complete_is_failure {
                 executed_failures.insert(i);
             }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/activities/activity_heartbeat_manager.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/activities/activity_heartbeat_manager.rs`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,19 @@
         on_complete: Arc<Notify>,
     },
     CompleteReport(TaskToken),
     CompleteThrottle(TaskToken),
 }
 
 #[derive(Debug)]
-pub struct ValidActivityHeartbeat {
-    pub task_token: TaskToken,
-    pub details: Vec<Payload>,
-    pub throttle_interval: Duration,
-    pub timeout_resetter: Option<Arc<Notify>>,
+struct ValidActivityHeartbeat {
+    task_token: TaskToken,
+    details: Vec<Payload>,
+    throttle_interval: Duration,
+    timeout_resetter: Option<Arc<Notify>>,
 }
 
 #[derive(Debug)]
 enum HeartbeatExecutorAction {
     /// Heartbeats are throttled for this task token, sleep until duration or wait to be cancelled
     Sleep(TaskToken, Duration, CancellationToken),
     /// Report heartbeat to the server
@@ -61,15 +61,15 @@
         task_token: TaskToken,
         details: Vec<Payload>,
     },
 }
 
 /// Errors thrown when heartbeating
 #[derive(thiserror::Error, Debug)]
-pub enum ActivityHeartbeatError {
+pub(crate) enum ActivityHeartbeatError {
     /// Heartbeat referenced an activity that we don't think exists. It may have completed already.
     #[error("Heartbeat has been sent for activity that either completed or never started on this worker.")]
     UnknownActivity,
     /// There was a set heartbeat timeout, but it was not parseable. A valid timeout is requried
     /// to heartbeat.
     #[error("Unable to parse activity heartbeat timeout.")]
     InvalidHeartbeatTimeout,
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/activities/activity_task_poller_stream.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/activities/activity_task_poller_stream.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/activities/local_activities.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/activities/local_activities.rs`

 * *Files 2% similar despite different names*

```diff
@@ -43,26 +43,22 @@
     /// Send the activity task to lang
     Dispatch(ActivityTask),
     /// The worker must re-feed this completion back through the machines. Includes timeouts.
     Autocomplete(LACompleteAction),
 }
 
 #[derive(Debug)]
-pub(crate) struct LocalInFlightActInfo {
-    pub la_info: NewLocalAct,
-    pub dispatch_time: Instant,
-    pub attempt: u32,
+struct LocalInFlightActInfo {
+    la_info: NewLocalAct,
+    dispatch_time: Instant,
+    attempt: u32,
     _permit: UsedMeteredSemPermit,
 }
 
 #[derive(Debug, Clone)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 pub(crate) enum LocalActivityExecutionResult {
     Completed(Success),
     Failed(ActFail),
     TimedOut(ActFail),
     Cancelled(Cancellation),
 }
 impl LocalActivityExecutionResult {
@@ -93,41 +89,38 @@
                             Some(failure::FailureInfo::TimeoutFailureInfo(TimeoutFailureInfo {
                                 timeout_type,
                                 ..
                             })),
                         ..
                     }),
                 ..
-            }) => TimeoutType::from_i32(*timeout_type),
+            }) => TimeoutType::try_from(*timeout_type).ok(),
             _ => None,
         }
     }
 }
 
 #[derive(Debug, Clone)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 pub(crate) struct LocalActivityResolution {
-    pub seq: u32,
-    pub result: LocalActivityExecutionResult,
-    pub runtime: Duration,
-    pub attempt: u32,
-    pub backoff: Option<prost_types::Duration>,
-    pub original_schedule_time: Option<SystemTime>,
+    pub(crate) seq: u32,
+    pub(crate) result: LocalActivityExecutionResult,
+    pub(crate) runtime: Duration,
+    pub(crate) attempt: u32,
+    pub(crate) backoff: Option<prost_types::Duration>,
+    pub(crate) original_schedule_time: Option<SystemTime>,
 }
 
 #[derive(Clone)]
 pub(crate) struct NewLocalAct {
-    pub schedule_cmd: ValidScheduleLA,
-    pub workflow_type: String,
-    pub workflow_exec_info: WorkflowExecution,
-    pub schedule_time: SystemTime,
+    pub(crate) schedule_cmd: ValidScheduleLA,
+    pub(crate) workflow_type: String,
+    pub(crate) workflow_exec_info: WorkflowExecution,
+    pub(crate) schedule_time: SystemTime,
 }
+
 impl Debug for NewLocalAct {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "LocalActivity({}, {})",
             self.schedule_cmd.seq, self.schedule_cmd.activity_type
         )
@@ -150,16 +143,16 @@
     /// certain run id
     #[from(ignore)]
     IndicateWorkflowTaskCompleted(String),
 }
 
 #[derive(Debug, Clone, Eq, PartialEq, Hash)]
 pub(crate) struct ExecutingLAId {
-    pub run_id: String,
-    pub seq_num: u32,
+    pub(crate) run_id: String,
+    pub(crate) seq_num: u32,
 }
 
 pub(crate) struct LocalActivityManager {
     /// Just so we can provide activity tasks the same namespace as the worker
     namespace: String,
     /// Sink for new activity execution requests
     act_req_tx: UnboundedSender<NewOrRetry>,
@@ -382,15 +375,27 @@
 
     /// Returns the next pending local-activity related action, or None if shutdown has initiated
     /// and there are no more remaining actions to take.
     pub(crate) async fn next_pending(&self) -> Option<NextPendingLAAction> {
         let (new_or_retry, permit) = match self.rcvs.lock().await.next().await? {
             NewOrCancel::Cancel(c) => {
                 return match c {
-                    CancelOrTimeout::Cancel(c) => Some(NextPendingLAAction::Dispatch(c)),
+                    CancelOrTimeout::Cancel(c) => {
+                        if self
+                            .dat
+                            .lock()
+                            .outstanding_activity_tasks
+                            .contains_key(c.task_token.as_slice())
+                        {
+                            Some(NextPendingLAAction::Dispatch(c))
+                        } else {
+                            // Don't dispatch cancels for things we've already stopped tracking
+                            None
+                        }
+                    }
                     CancelOrTimeout::Timeout { run_id, resolution } => {
                         let tt = self
                             .dat
                             .lock()
                             .la_info
                             .get(&ExecutingLAId {
                                 run_id,
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/activities.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/activities.rs`

 * *Files 1% similar despite different names*

```diff
@@ -69,49 +69,49 @@
     task_token: TaskToken,
     reason: ActivityCancelReason,
     /// Set true if we should assume the server has already forgotten about this activity
     consider_not_found: bool,
 }
 
 impl PendingActivityCancel {
-    pub fn new(task_token: TaskToken, reason: ActivityCancelReason) -> Self {
+    fn new(task_token: TaskToken, reason: ActivityCancelReason) -> Self {
         Self {
             task_token,
             reason,
             consider_not_found: false,
         }
     }
 }
 
 /// Contains details that core wants to store while an activity is running.
 #[derive(Debug)]
 struct InFlightActInfo {
-    pub activity_type: String,
-    pub workflow_type: String,
+    activity_type: String,
+    workflow_type: String,
     /// Only kept for logging reasons
-    pub workflow_id: String,
+    workflow_id: String,
     /// Only kept for logging reasons
-    pub workflow_run_id: String,
+    workflow_run_id: String,
     start_time: Instant,
 }
 
 /// Augments [InFlightActInfo] with details specific to remote activities
 struct RemoteInFlightActInfo {
-    pub base: InFlightActInfo,
+    base: InFlightActInfo,
     /// Used to calculate aggregation delay between activity heartbeats.
-    pub heartbeat_timeout: Option<prost_types::Duration>,
+    heartbeat_timeout: Option<prost_types::Duration>,
     /// Set if we have already issued a cancellation activation to lang for this activity, with
     /// the original reason we issued the cancel.
-    pub issued_cancel_to_lang: Option<ActivityCancelReason>,
+    issued_cancel_to_lang: Option<ActivityCancelReason>,
     /// Set to true if we have already learned from the server this activity doesn't exist. EX:
     /// we have learned from heartbeating and issued a cancel task, in which case we may simply
     /// discard the reply.
-    pub known_not_found: bool,
+    known_not_found: bool,
     /// Handle to the task containing local timeout tracking, if any.
-    pub local_timeouts_task: Option<JoinHandle<()>>,
+    local_timeouts_task: Option<JoinHandle<()>>,
     /// Used to reset the local heartbeat timeout every time we record a heartbeat
     timeout_resetter: Option<Arc<Notify>>,
     /// The permit from the max concurrent semaphore
     _permit: UsedMeteredSemPermit,
 }
 impl RemoteInFlightActInfo {
     fn new(poll_resp: &PollActivityTaskQueueResponse, permit: UsedMeteredSemPermit) -> Self {
@@ -662,22 +662,22 @@
             self.tx.send(t).expect("Receive half cannot be dropped");
         }
     }
 }
 
 #[derive(Debug)]
 pub(crate) struct PermittedTqResp {
-    pub permit: OwnedMeteredSemPermit,
-    pub resp: PollActivityTaskQueueResponse,
+    pub(crate) permit: OwnedMeteredSemPermit,
+    pub(crate) resp: PollActivityTaskQueueResponse,
 }
 
 #[derive(Debug)]
 pub(crate) struct TrackedPermittedTqResp {
-    pub permit: TrackedOwnedMeteredSemPermit,
-    pub resp: PollActivityTaskQueueResponse,
+    pub(crate) permit: TrackedOwnedMeteredSemPermit,
+    pub(crate) resp: PollActivityTaskQueueResponse,
 }
 
 fn worker_shutdown_failure() -> Failure {
     Failure {
         message: "Worker is shutting down and this activity did not complete in time".to_string(),
         source: "".to_string(),
         stack_trace: "".to_string(),
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/client/mocks.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/client/mocks.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 use super::*;
 use futures::Future;
-use lazy_static::lazy_static;
+use once_cell::sync::Lazy;
 use std::sync::Arc;
 use temporal_client::SlotManager;
 
-lazy_static! {
-    pub(crate) static ref DEFAULT_WORKERS_REGISTRY: Arc<SlotManager> = Arc::new(SlotManager::new());
-}
+static DEFAULT_WORKERS_REGISTRY: Lazy<Arc<SlotManager>> =
+    Lazy::new(|| Arc::new(SlotManager::new()));
 
 pub(crate) static DEFAULT_TEST_CAPABILITIES: &Capabilities = &Capabilities {
     signal_and_query_header: true,
     internal_error_differentiation: true,
     activity_failure_include_heartbeat: true,
     supports_schedules: true,
     encoded_failure_attributes: true,
@@ -22,26 +21,26 @@
 };
 
 #[cfg(test)]
 /// Create a mock client primed with basic necessary expectations
 pub(crate) fn mock_workflow_client() -> MockWorkerClient {
     let mut r = MockWorkerClient::new();
     r.expect_capabilities()
-        .returning(|| Some(DEFAULT_TEST_CAPABILITIES));
+        .returning(|| Some(DEFAULT_TEST_CAPABILITIES.clone()));
     r.expect_workers()
         .returning(|| DEFAULT_WORKERS_REGISTRY.clone());
     r.expect_is_mock().returning(|| true);
     r
 }
 
 /// Create a mock manual client primed with basic necessary expectations
 pub(crate) fn mock_manual_workflow_client() -> MockManualWorkerClient {
     let mut r = MockManualWorkerClient::new();
     r.expect_capabilities()
-        .returning(|| Some(DEFAULT_TEST_CAPABILITIES));
+        .returning(|| Some(DEFAULT_TEST_CAPABILITIES.clone()));
     r.expect_workers()
         .returning(|| DEFAULT_WORKERS_REGISTRY.clone());
     r.expect_is_mock().returning(|| true);
     r
 }
 
 // Need a version of the mock that can return futures so we can return potentially pending
@@ -112,14 +111,16 @@
         fn respond_legacy_query<'a, 'b>(
             &self,
             task_token: TaskToken,
             query_result: QueryResult,
         ) -> impl Future<Output = Result<RespondQueryTaskCompletedResponse>> + Send + 'b
             where 'a: 'b, Self: 'b;
 
-        fn capabilities(&self) -> Option<&'static get_system_info_response::Capabilities>;
+        fn replace_client(&self, new_client: RetryClient<Client>);
+
+        fn capabilities(&self) -> Option<get_system_info_response::Capabilities>;
 
         fn workers(&self) -> Arc<SlotManager>;
 
         fn is_mock(&self) -> bool;
     }
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/client.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/client.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 //! Worker-specific client needs
 
 pub(crate) mod mocks;
+use parking_lot::RwLock;
 use std::sync::Arc;
 use temporal_client::{Client, RetryClient, SlotManager, WorkflowService};
 use temporal_sdk_core_protos::{
     coresdk::workflow_commands::QueryResult,
     temporal::api::{
         command::v1::Command,
         common::v1::{
@@ -22,40 +23,44 @@
     TaskToken,
 };
 
 type Result<T, E = tonic::Status> = std::result::Result<T, E>;
 
 /// Contains everything a worker needs to interact with the server
 pub(crate) struct WorkerClientBag {
-    client: RetryClient<Client>,
+    replaceable_client: RwLock<RetryClient<Client>>,
     namespace: String,
     identity: String,
     worker_build_id: String,
     use_versioning: bool,
 }
 
 impl WorkerClientBag {
-    pub fn new(
+    pub(crate) fn new(
         client: RetryClient<Client>,
         namespace: String,
         identity: String,
         worker_build_id: String,
         use_versioning: bool,
     ) -> Self {
         Self {
-            client,
+            replaceable_client: RwLock::new(client),
             namespace,
             identity,
             worker_build_id,
             use_versioning,
         }
     }
 
+    fn cloned_client(&self) -> RetryClient<Client> {
+        self.replaceable_client.read().clone()
+    }
+
     fn default_capabilities(&self) -> Capabilities {
-        self.capabilities().cloned().unwrap_or_default()
+        self.capabilities().unwrap_or_default()
     }
 
     fn binary_checksum(&self) -> String {
         if self.default_capabilities().build_id_based_versioning {
             "".to_string()
         } else {
             self.worker_build_id.clone()
@@ -138,16 +143,16 @@
     ) -> Result<GetWorkflowExecutionHistoryResponse>;
     async fn respond_legacy_query(
         &self,
         task_token: TaskToken,
         query_result: QueryResult,
     ) -> Result<RespondQueryTaskCompletedResponse>;
 
-    #[allow(clippy::needless_lifetimes)] // Clippy is wrong here
-    fn capabilities<'a>(&'a self) -> Option<&'a get_system_info_response::Capabilities>;
+    fn replace_client(&self, new_client: RetryClient<Client>);
+    fn capabilities(&self) -> Option<get_system_info_response::Capabilities>;
     fn workers(&self) -> Arc<SlotManager>;
     fn is_mock(&self) -> bool;
 }
 
 #[async_trait::async_trait]
 impl WorkerClient for WorkerClientBag {
     async fn poll_workflow_task(
@@ -159,16 +164,15 @@
             task_queue: Some(task_queue),
             identity: self.identity.clone(),
             binary_checksum: self.binary_checksum(),
             worker_version_capabilities: self.worker_version_capabilities(),
         };
 
         Ok(self
-            .client
-            .clone()
+            .cloned_client()
             .poll_workflow_task_queue(request)
             .await?
             .into_inner())
     }
 
     async fn poll_activity_task(
         &self,
@@ -186,16 +190,15 @@
             task_queue_metadata: max_tasks_per_sec.map(|tps| TaskQueueMetadata {
                 max_tasks_per_second: Some(tps),
             }),
             worker_version_capabilities: self.worker_version_capabilities(),
         };
 
         Ok(self
-            .client
-            .clone()
+            .cloned_client()
             .poll_activity_task_queue(request)
             .await?
             .into_inner())
     }
 
     async fn complete_workflow_task(
         &self,
@@ -227,29 +230,27 @@
                 })
                 .collect(),
             namespace: self.namespace.clone(),
             sdk_metadata: Some(request.sdk_metadata),
             metering_metadata: Some(request.metering_metadata),
         };
         Ok(self
-            .client
-            .clone()
+            .cloned_client()
             .respond_workflow_task_completed(request)
             .await?
             .into_inner())
     }
 
     async fn complete_activity_task(
         &self,
         task_token: TaskToken,
         result: Option<Payloads>,
     ) -> Result<RespondActivityTaskCompletedResponse> {
         Ok(self
-            .client
-            .clone()
+            .cloned_client()
             .respond_activity_task_completed(RespondActivityTaskCompletedRequest {
                 task_token: task_token.0,
                 result,
                 identity: self.identity.clone(),
                 namespace: self.namespace.clone(),
                 worker_version: self.worker_version_stamp(),
             })
@@ -259,16 +260,15 @@
 
     async fn record_activity_heartbeat(
         &self,
         task_token: TaskToken,
         details: Option<Payloads>,
     ) -> Result<RecordActivityTaskHeartbeatResponse> {
         Ok(self
-            .client
-            .clone()
+            .cloned_client()
             .record_activity_task_heartbeat(RecordActivityTaskHeartbeatRequest {
                 task_token: task_token.0,
                 details,
                 identity: self.identity.clone(),
                 namespace: self.namespace.clone(),
             })
             .await?
@@ -277,16 +277,15 @@
 
     async fn cancel_activity_task(
         &self,
         task_token: TaskToken,
         details: Option<Payloads>,
     ) -> Result<RespondActivityTaskCanceledResponse> {
         Ok(self
-            .client
-            .clone()
+            .cloned_client()
             .respond_activity_task_canceled(RespondActivityTaskCanceledRequest {
                 task_token: task_token.0,
                 details,
                 identity: self.identity.clone(),
                 namespace: self.namespace.clone(),
                 worker_version: self.worker_version_stamp(),
             })
@@ -296,16 +295,15 @@
 
     async fn fail_activity_task(
         &self,
         task_token: TaskToken,
         failure: Option<Failure>,
     ) -> Result<RespondActivityTaskFailedResponse> {
         Ok(self
-            .client
-            .clone()
+            .cloned_client()
             .respond_activity_task_failed(RespondActivityTaskFailedRequest {
                 task_token: task_token.0,
                 failure,
                 identity: self.identity.clone(),
                 namespace: self.namespace.clone(),
                 // TODO: Implement - https://github.com/temporalio/sdk-core/issues/293
                 last_heartbeat_details: None,
@@ -328,30 +326,28 @@
             identity: self.identity.clone(),
             binary_checksum: self.binary_checksum(),
             namespace: self.namespace.clone(),
             messages: vec![],
             worker_version: self.worker_version_stamp(),
         };
         Ok(self
-            .client
-            .clone()
+            .cloned_client()
             .respond_workflow_task_failed(request)
             .await?
             .into_inner())
     }
 
     async fn get_workflow_execution_history(
         &self,
         workflow_id: String,
         run_id: Option<String>,
         page_token: Vec<u8>,
     ) -> Result<GetWorkflowExecutionHistoryResponse> {
         Ok(self
-            .client
-            .clone()
+            .cloned_client()
             .get_workflow_execution_history(GetWorkflowExecutionHistoryRequest {
                 namespace: self.namespace.clone(),
                 execution: Some(WorkflowExecution {
                     workflow_id,
                     run_id: run_id.unwrap_or_default(),
                 }),
                 next_page_token: page_token,
@@ -364,56 +360,62 @@
     async fn respond_legacy_query(
         &self,
         task_token: TaskToken,
         query_result: QueryResult,
     ) -> Result<RespondQueryTaskCompletedResponse> {
         let (_, completed_type, query_result, error_message) = query_result.into_components();
         Ok(self
-            .client
-            .clone()
+            .cloned_client()
             .respond_query_task_completed(RespondQueryTaskCompletedRequest {
                 task_token: task_token.into(),
                 completed_type: completed_type as i32,
                 query_result,
                 error_message,
                 namespace: self.namespace.clone(),
             })
             .await?
             .into_inner())
     }
 
-    fn capabilities(&self) -> Option<&Capabilities> {
-        self.client.get_client().inner().capabilities()
+    fn replace_client(&self, new_client: RetryClient<Client>) {
+        let mut replaceable_client = self.replaceable_client.write();
+        *replaceable_client = new_client;
+    }
+
+    fn capabilities(&self) -> Option<Capabilities> {
+        let client = self.replaceable_client.read();
+        client.get_client().inner().capabilities().cloned()
     }
 
     fn workers(&self) -> Arc<SlotManager> {
-        self.client.get_client().inner().workers()
+        let client = self.replaceable_client.read();
+        client.get_client().inner().workers()
     }
 
     fn is_mock(&self) -> bool {
         false
     }
 }
 
 /// A version of [RespondWorkflowTaskCompletedRequest] that will finish being filled out by the
 /// server client
 #[derive(Debug, Clone, PartialEq)]
 pub(crate) struct WorkflowTaskCompletion {
     /// The task token that would've been received from polling for a workflow activation
-    pub task_token: TaskToken,
+    pub(crate) task_token: TaskToken,
     /// A list of new commands to send to the server, such as starting a timer.
-    pub commands: Vec<Command>,
+    pub(crate) commands: Vec<Command>,
     /// A list of protocol messages to send to the server.
-    pub messages: Vec<ProtocolMessage>,
+    pub(crate) messages: Vec<ProtocolMessage>,
     /// If set, indicate that next task should be queued on sticky queue with given attributes.
-    pub sticky_attributes: Option<StickyExecutionAttributes>,
+    pub(crate) sticky_attributes: Option<StickyExecutionAttributes>,
     /// Responses to queries in the `queries` field of the workflow task.
-    pub query_responses: Vec<QueryResult>,
+    pub(crate) query_responses: Vec<QueryResult>,
     /// Indicate that the task completion should return a new WFT if one is available
-    pub return_new_workflow_task: bool,
+    pub(crate) return_new_workflow_task: bool,
     /// Force a new WFT to be created after this completion
-    pub force_create_new_workflow_task: bool,
+    pub(crate) force_create_new_workflow_task: bool,
     /// SDK-specific metadata to send
-    pub sdk_metadata: WorkflowTaskCompletedMetadata,
+    pub(crate) sdk_metadata: WorkflowTaskCompletedMetadata,
     /// Metering info
-    pub metering_metadata: MeteringMetadata,
+    pub(crate) metering_metadata: MeteringMetadata,
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/mod.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 mod activities;
 pub(crate) mod client;
 mod slot_provider;
 mod workflow;
 
 pub use temporal_sdk_core_api::worker::{WorkerConfig, WorkerConfigBuilder};
-#[cfg(feature = "save_wf_inputs")]
-pub use workflow::replay_wf_state_inputs;
 
 pub(crate) use activities::{
     ExecutingLAId, LocalActRequest, LocalActivityExecutionResult, LocalActivityResolution,
     NewLocalAct,
 };
 pub(crate) use workflow::{wft_poller::new_wft_poller, LEGACY_QUERY_ID};
 
-use temporal_client::WorkerKey;
+use temporal_client::{ConfiguredClient, TemporalServiceClientWithMetrics, WorkerKey};
 
 use crate::{
     abstractions::{dbg_panic, MeteredSemaphore},
     errors::CompleteWfError,
     pollers::{
         new_activity_task_buffer, new_workflow_task_buffer, BoxedActPoller, WorkflowTaskPoller,
     },
@@ -34,14 +32,15 @@
         client::WorkerClient,
         workflow::{LAReqSink, LocalResolution, WorkflowBasics, Workflows},
     },
     ActivityHeartbeat, CompleteActivityError, PollActivityError, PollWfError, WorkerTrait,
 };
 use activities::WorkerActivityTasks;
 use futures_util::{stream, StreamExt};
+use parking_lot::Mutex;
 use slot_provider::SlotProvider;
 use std::{
     convert::TryInto,
     future,
     sync::{
         atomic::{AtomicBool, Ordering},
         Arc,
@@ -77,15 +76,15 @@
 };
 
 /// A worker polls on a certain task queue
 pub struct Worker {
     config: WorkerConfig,
     wf_client: Arc<dyn WorkerClient>,
     /// Registration key to enable eager workflow start for this worker
-    worker_key: Option<WorkerKey>,
+    worker_key: Mutex<Option<WorkerKey>>,
     /// Manages all workflows and WFT processing
     workflows: Workflows,
     /// Manages activity tasks for this worker/task queue
     at_task_mgr: Option<WorkerActivityTasks>,
     /// Manages local activities
     local_act_mgr: Arc<LocalActivityManager>,
     /// Has shutdown been called?
@@ -165,15 +164,15 @@
                 task_queue=%self.config.task_queue,
                 namespace=%self.config.namespace,
                 "Initiated shutdown",
             );
         }
         self.shutdown_token.cancel();
         // First, disable Eager Workflow Start
-        if let Some(key) = self.worker_key {
+        if let Some(key) = *self.worker_key.lock() {
             self.wf_client.workers().unregister(key);
         }
         // Second, we want to stop polling of both activity and workflow tasks
         if let Some(atm) = self.at_task_mgr.as_ref() {
             atm.initiate_shutdown();
         }
         // Let the manager know that shutdown has been initiated to try to unblock the local
@@ -213,14 +212,26 @@
             sticky_queue_name,
             client,
             TaskPollers::Real,
             telem_instance,
         )
     }
 
+    /// Replace client and return a new client. For eager workflow purposes, this new client will
+    /// now apply to future eager start requests and the older client will not.
+    pub fn replace_client(&self, new_client: ConfiguredClient<TemporalServiceClientWithMetrics>) {
+        // Unregister worker from current client, register in new client at the end
+        let mut worker_key = self.worker_key.lock();
+        let slot_provider = (*worker_key).and_then(|k| self.wf_client.workers().unregister(k));
+        self.wf_client
+            .replace_client(super::init_worker_client(&self.config, new_client));
+        *worker_key = slot_provider
+            .and_then(|slot_provider| self.wf_client.workers().register(slot_provider));
+    }
+
     #[cfg(test)]
     pub(crate) fn new_test(config: WorkerConfig, client: impl WorkerClient + 'static) -> Self {
         Self::new(config, None, Arc::new(client), None)
     }
 
     #[allow(clippy::too_many_arguments)] // Not much worth combining here
     pub(crate) fn new_with_pollers(
@@ -364,31 +375,31 @@
                 config.local_timeout_buffer_for_activities,
             )
         });
         let poll_on_non_local_activities = at_task_mgr.is_some();
         if !poll_on_non_local_activities {
             info!("Activity polling is disabled for this worker");
         };
-        let la_sink = LAReqSink::new(local_act_mgr.clone(), config.wf_state_inputs.clone());
+        let la_sink = LAReqSink::new(local_act_mgr.clone());
         let provider = SlotProvider::new(
             config.namespace.clone(),
             config.task_queue.clone(),
             wft_semaphore.clone(),
             external_wft_tx,
         );
-        let worker_key = client.workers().register(Box::new(provider));
+        let worker_key = Mutex::new(client.workers().register(Box::new(provider)));
         Self {
             worker_key,
             wf_client: client.clone(),
             workflows: Workflows::new(
                 build_wf_basics(
                     config.clone(),
                     metrics,
                     shutdown_token.child_token(),
-                    client.capabilities().cloned().unwrap_or_default(),
+                    client.capabilities().clone().unwrap_or_default(),
                 ),
                 sticky_queue_name.map(|sq| StickyExecutionAttributes {
                     worker_task_queue: Some(TaskQueue {
                         name: sq,
                         kind: TaskQueueKind::Sticky as i32,
                         normal_name: config.task_queue.clone(),
                     }),
@@ -655,18 +666,17 @@
     }
 
     fn notify_local_result(&self, run_id: &str, res: LocalResolution) {
         self.workflows.notify_of_local_result(run_id, res);
     }
 }
 
-pub struct PostActivateHookData<'a> {
-    pub run_id: &'a str,
-    pub most_recent_event: usize,
-    pub replaying: bool,
+pub(crate) struct PostActivateHookData<'a> {
+    pub(crate) run_id: &'a str,
+    pub(crate) replaying: bool,
 }
 
 fn build_wf_basics(
     config: WorkerConfig,
     metrics: MetricsContext,
     shutdown_token: CancellationToken,
     server_capabilities: get_system_info_response::Capabilities,
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/slot_provider.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/slot_provider.rs`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 use temporal_sdk_core_protos::temporal::api::workflowservice::v1::PollWorkflowTaskQueueResponse;
 use tokio::sync::mpsc::UnboundedSender;
 use tonic::Status;
 
 type WFTStreamSender =
     UnboundedSender<Result<(ValidPollWFTQResponse, OwnedMeteredSemPermit), Status>>;
 
-pub struct Slot {
+struct Slot {
     permit: OwnedMeteredSemPermit,
     external_wft_tx: WFTStreamSender,
 }
 
 impl Slot {
     fn new(permit: OwnedMeteredSemPermit, external_wft_tx: WFTStreamSender) -> Self {
         Self {
@@ -40,23 +40,23 @@
         self.external_wft_tx.send(Ok((wft, self.permit)))?;
         Ok(())
     }
 }
 
 #[derive(derive_more::DebugCustom)]
 #[debug(fmt = "SlotProvider {{ namespace:{namespace}, task_queue: {task_queue} }}")]
-pub struct SlotProvider {
+pub(super) struct SlotProvider {
     namespace: String,
     task_queue: String,
     wft_semaphore: Arc<MeteredSemaphore>,
     external_wft_tx: WFTStreamSender,
 }
 
 impl SlotProvider {
-    pub(crate) fn new(
+    pub(super) fn new(
         namespace: String,
         task_queue: String,
         wft_semaphore: Arc<MeteredSemaphore>,
         external_wft_tx: WFTStreamSender,
     ) -> Self {
         Self {
             namespace,
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/driven_workflow.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/driven_workflow.rs`

 * *Files 11% similar despite different names*

```diff
@@ -8,35 +8,35 @@
     coresdk::workflow_activation::{start_workflow_from_attribs, WorkflowActivationJob},
     temporal::api::history::v1::WorkflowExecutionStartedEventAttributes,
     utilities::TryIntoOrNone,
 };
 
 /// Represents a connection to a lang side workflow that can have activations fed into it and
 /// command responses pulled out.
-pub struct DrivenWorkflow {
+pub(crate) struct DrivenWorkflow {
     started_attrs: Option<WorkflowStartedInfo>,
     incoming_commands: Receiver<Vec<WFCommand>>,
     /// Outgoing activation jobs that need to be sent to the lang sdk
     outgoing_wf_activation_jobs: Vec<OutgoingJob>,
 }
 
 impl DrivenWorkflow {
-    pub fn new() -> (Self, Sender<Vec<WFCommand>>) {
+    pub(super) fn new() -> (Self, Sender<Vec<WFCommand>>) {
         let (tx, rx) = mpsc::channel();
         (
             Self {
                 started_attrs: None,
                 incoming_commands: rx,
                 outgoing_wf_activation_jobs: vec![],
             },
             tx,
         )
     }
     /// Start the workflow
-    pub fn start(
+    pub(super) fn start(
         &mut self,
         workflow_id: String,
         randomness_seed: u64,
         start_time: Timestamp,
         attribs: WorkflowExecutionStartedEventAttributes,
     ) {
         debug!(run_id = %attribs.original_execution_run_id, "Driven WF start");
@@ -49,40 +49,40 @@
         self.send_job(
             start_workflow_from_attribs(attribs, workflow_id, randomness_seed, start_time).into(),
         );
         self.started_attrs = Some(started_info);
     }
 
     /// Return the attributes from the workflow execution started event if this workflow has started
-    pub fn get_started_info(&self) -> Option<&WorkflowStartedInfo> {
+    pub(super) fn get_started_info(&self) -> Option<&WorkflowStartedInfo> {
         self.started_attrs.as_ref()
     }
 
     /// Enqueue a new job to be sent to the driven workflow
     pub(super) fn send_job(&mut self, job: OutgoingJob) {
         self.outgoing_wf_activation_jobs.push(job);
     }
 
     /// Observe pending jobs
     pub(super) fn peek_pending_jobs(&self) -> &[OutgoingJob] {
         self.outgoing_wf_activation_jobs.as_slice()
     }
 
     /// Drain all pending jobs, so that they may be sent to the driven workflow
-    pub fn drain_jobs(&mut self) -> Vec<WorkflowActivationJob> {
+    pub(super) fn drain_jobs(&mut self) -> Vec<WorkflowActivationJob> {
         self.outgoing_wf_activation_jobs
             .drain(..)
             .map(Into::into)
             .collect()
     }
 
     /// Obtain any output from the workflow's recent execution(s). Because the lang sdk is
     /// responsible for calling workflow code as a result of receiving tasks from
     /// [crate::Core::poll_task], we cannot directly iterate it here. Commands are simply pulled
     /// from a buffer that the language side sinks into when it calls [crate::Core::complete_task]
-    pub fn fetch_workflow_iteration_output(&mut self) -> Vec<WFCommand> {
+    pub(super) fn fetch_workflow_iteration_output(&mut self) -> Vec<WFCommand> {
         let in_cmds = self.incoming_commands.try_recv();
         let in_cmds = in_cmds.unwrap_or_else(|_| vec![WFCommand::NoCommandsFromLang]);
         debug!(in_cmds = %in_cmds.display(), "wf bridge iteration fetch");
         in_cmds
     }
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/history_update.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/history_update.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     worker::{
         client::WorkerClient,
         workflow::{CacheMissFetchReq, PermittedWFT, PreparedWFT},
     },
 };
 use futures::{future::BoxFuture, FutureExt, Stream};
 use itertools::Itertools;
+use once_cell::sync::Lazy;
 use std::{
     collections::VecDeque,
     fmt::Debug,
     future::Future,
     mem,
     mem::transmute,
     pin::Pin,
@@ -19,41 +20,37 @@
 };
 use temporal_sdk_core_protos::temporal::api::{
     enums::v1::EventType,
     history::v1::{history_event, History, HistoryEvent, WorkflowTaskCompletedEventAttributes},
 };
 use tracing::Instrument;
 
-lazy_static::lazy_static! {
-    static ref EMPTY_FETCH_ERR: tonic::Status
-        = tonic::Status::unknown("Fetched empty history page");
-    static ref EMPTY_TASK_ERR: tonic::Status
-        = tonic::Status::unknown("Received an empty workflow task with no queries or history");
-}
+static EMPTY_FETCH_ERR: Lazy<tonic::Status> =
+    Lazy::new(|| tonic::Status::unknown("Fetched empty history page"));
+static EMPTY_TASK_ERR: Lazy<tonic::Status> = Lazy::new(|| {
+    tonic::Status::unknown("Received an empty workflow task with no queries or history")
+});
 
 /// Represents one or more complete WFT sequences. History events are expected to be consumed from
 /// it and applied to the state machines via [HistoryUpdate::take_next_wft_sequence]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
-pub struct HistoryUpdate {
+pub(crate) struct HistoryUpdate {
     events: Vec<HistoryEvent>,
     /// The event ID of the last started WFT, as according to the WFT which this update was
     /// extracted from. Hence, while processing multiple logical WFTs during replay which were part
     /// of one large history fetched from server, multiple updates may have the same value here.
-    pub previous_wft_started_id: i64,
+    pub(crate) previous_wft_started_id: i64,
     /// The `started_event_id` field from the WFT which this update is tied to. Multiple updates
     /// may have the same value if they're associated with the same WFT.
-    pub wft_started_id: i64,
+    pub(crate) wft_started_id: i64,
     /// True if this update contains the final WFT in history, and no more attempts to extract
     /// additional updates should be made.
     has_last_wft: bool,
     wft_count: usize,
 }
+
 impl Debug for HistoryUpdate {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         if self.is_real() {
             write!(
                 f,
                 "HistoryUpdate(previous_started_event_id: {}, started_id: {}, \
                  length: {}, first_event_id: {:?})",
@@ -65,48 +62,39 @@
         } else {
             write!(f, "DummyHistoryUpdate")
         }
     }
 }
 
 #[derive(Debug)]
-pub enum NextWFT {
+pub(crate) enum NextWFT {
     ReplayOver,
     WFT(Vec<HistoryEvent>, bool),
     NeedFetch,
 }
 
 #[derive(derive_more::DebugCustom)]
 #[debug(fmt = "HistoryPaginator(run_id: {run_id})")]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize),
-    serde(default = "HistoryPaginator::fake_deserialized")
-)]
-pub struct HistoryPaginator {
+pub(crate) struct HistoryPaginator {
     pub(crate) wf_id: String,
     pub(crate) run_id: String,
     pub(crate) previous_wft_started_id: i64,
     pub(crate) wft_started_event_id: i64,
     id_of_last_event_in_last_extracted_update: Option<i64>,
 
-    #[cfg_attr(feature = "save_wf_inputs", serde(skip))]
     client: Arc<dyn WorkerClient>,
-    #[cfg_attr(feature = "save_wf_inputs", serde(skip))]
     event_queue: VecDeque<HistoryEvent>,
-    #[cfg_attr(feature = "save_wf_inputs", serde(skip))]
     next_page_token: NextPageToken,
     /// These are events that should be returned once pagination has finished. This only happens
     /// during cache misses, where we got a partial task but need to fetch history from the start.
-    #[cfg_attr(feature = "save_wf_inputs", serde(skip))]
     final_events: Vec<HistoryEvent>,
 }
 
 #[derive(Clone, Debug)]
-pub enum NextPageToken {
+pub(crate) enum NextPageToken {
     /// There is no page token, we need to fetch history from the beginning
     FetchFromStart,
     /// There is a page token
     Next(Vec<u8>),
     /// There is no page token, we are done fetching history
     Done,
 }
@@ -220,30 +208,14 @@
             final_events,
             previous_wft_started_id,
             wft_started_event_id,
             id_of_last_event_in_last_extracted_update: None,
         }
     }
 
-    #[cfg(feature = "save_wf_inputs")]
-    pub(super) fn fake_deserialized() -> HistoryPaginator {
-        use crate::worker::client::mocks::mock_manual_workflow_client;
-        HistoryPaginator {
-            client: Arc::new(mock_manual_workflow_client()),
-            event_queue: Default::default(),
-            wf_id: "".to_string(),
-            run_id: "".to_string(),
-            next_page_token: NextPageToken::FetchFromStart,
-            final_events: vec![],
-            previous_wft_started_id: -2,
-            wft_started_event_id: -2,
-            id_of_last_event_in_last_extracted_update: None,
-        }
-    }
-
     /// Return at least the next two WFT sequences (as determined by the passed-in ID) as a
     /// [HistoryUpdate]. Two sequences supports the required peek-ahead during replay without
     /// unnecessary back-and-forth.
     ///
     /// If there are already enough events buffered in memory, they will all be returned. Including
     /// possibly (likely, during replay) more than just the next two WFTs.
     ///
@@ -405,15 +377,15 @@
     #[pin]
     open_history_request: Option<BoxFuture<'static, Result<(), tonic::Status>>>,
 }
 
 impl StreamingHistoryPaginator {
     // Kept since can be used for history downloading
     #[cfg(test)]
-    pub fn new(inner: HistoryPaginator) -> Self {
+    fn new(inner: HistoryPaginator) -> Self {
         Self {
             inner,
             open_history_request: None,
         }
     }
 }
 
@@ -447,27 +419,29 @@
         }
     }
 }
 
 impl HistoryUpdate {
     /// Sometimes it's useful to take an update out of something without needing to use an option
     /// field. Use this to replace the field with an empty update.
-    pub fn dummy() -> Self {
+    pub(crate) fn dummy() -> Self {
         Self {
             events: vec![],
             previous_wft_started_id: -1,
             wft_started_id: -1,
             has_last_wft: false,
             wft_count: 0,
         }
     }
-    pub fn is_real(&self) -> bool {
+
+    pub(crate) fn is_real(&self) -> bool {
         self.previous_wft_started_id >= 0
     }
-    pub fn first_event_id(&self) -> Option<i64> {
+
+    pub(crate) fn first_event_id(&self) -> Option<i64> {
         self.events.first().map(|e| e.event_id)
     }
 
     #[cfg(debug_assertions)]
     fn assert_contiguous(&self) -> bool {
         use crate::abstractions::dbg_panic;
 
@@ -481,15 +455,15 @@
         true
     }
 
     /// Create an instance of an update directly from events. If the passed in event iterator has a
     /// partial WFT sequence at the end, all events after the last complete WFT sequence (ending
     /// with WFT started) are returned back to the caller, since the history update only works in
     /// terms of complete WFT sequences.
-    pub fn from_events<I: IntoIterator<Item = HistoryEvent>>(
+    pub(crate) fn from_events<I: IntoIterator<Item = HistoryEvent>>(
         events: I,
         previous_wft_started_id: i64,
         wft_started_id: i64,
         has_last_wft: bool,
     ) -> (Self, Vec<HistoryEvent>)
     where
         <I as IntoIterator>::IntoIter: Send + 'static,
@@ -562,15 +536,15 @@
         )
     }
 
     /// Create an instance of an update directly from events. The passed in events *must* consist
     /// of one or more complete WFT sequences. IE: The event iterator must not end in the middle
     /// of a WFT sequence.
     #[cfg(test)]
-    pub fn new_from_events<I: IntoIterator<Item = HistoryEvent>>(
+    fn new_from_events<I: IntoIterator<Item = HistoryEvent>>(
         events: I,
         previous_wft_started_id: i64,
         wft_started_id: i64,
     ) -> Self
     where
         <I as IntoIterator>::IntoIter: Send + 'static,
     {
@@ -586,15 +560,15 @@
     /// Given a workflow task started id, return all events starting at that number (exclusive) to
     /// the next WFT started event (inclusive).
     ///
     /// Events are *consumed* by this process, to keep things efficient in workflow machines.
     ///
     /// If we are out of WFT sequences that can be yielded by this update, it will return an empty
     /// vec, indicating more pages will need to be fetched.
-    pub fn take_next_wft_sequence(&mut self, from_wft_started_id: i64) -> NextWFT {
+    pub(crate) fn take_next_wft_sequence(&mut self, from_wft_started_id: i64) -> NextWFT {
         // First, drop any events from the queue which are earlier than the passed-in id.
         if let Some(ix_first_relevant) = self.starting_index_after_skipping(from_wft_started_id) {
             self.events.drain(0..ix_first_relevant);
         }
         let next_wft_ix =
             find_end_index_of_next_wft_seq(&self.events, from_wft_started_id, self.has_last_wft);
         match next_wft_ix {
@@ -625,15 +599,15 @@
         )
     }
 
     /// Lets the caller peek ahead at the next WFT sequence that will be returned by
     /// [take_next_wft_sequence]. Will always return the first available WFT sequence if that has
     /// not been called first. May also return an empty iterator or incomplete sequence if we are at
     /// the end of history.
-    pub fn peek_next_wft_sequence(&self, from_wft_started_id: i64) -> &[HistoryEvent] {
+    pub(crate) fn peek_next_wft_sequence(&self, from_wft_started_id: i64) -> &[HistoryEvent] {
         let ix_first_relevant = self
             .starting_index_after_skipping(from_wft_started_id)
             .unwrap_or_default();
         let relevant_events = &self.events[ix_first_relevant..];
         if relevant_events.is_empty() {
             return relevant_events;
         }
@@ -641,28 +615,28 @@
             find_end_index_of_next_wft_seq(relevant_events, from_wft_started_id, self.has_last_wft)
                 .index();
         &relevant_events[0..=ix_end]
     }
 
     /// Returns true if this update has the next needed WFT sequence, false if events will need to
     /// be fetched in order to create a complete update with the entire next WFT sequence.
-    pub fn can_take_next_wft_sequence(&self, from_wft_started_id: i64) -> bool {
+    pub(crate) fn can_take_next_wft_sequence(&self, from_wft_started_id: i64) -> bool {
         let next_wft_ix =
             find_end_index_of_next_wft_seq(&self.events, from_wft_started_id, self.has_last_wft);
         if let NextWFTSeqEndIndex::Incomplete(_) = next_wft_ix {
             if !self.has_last_wft {
                 return false;
             }
         }
         true
     }
 
     /// Returns the next WFT completed event attributes, if any, starting at (inclusive) the
     /// `from_id`
-    pub fn peek_next_wft_completed(
+    pub(crate) fn peek_next_wft_completed(
         &self,
         from_id: i64,
     ) -> Option<&WorkflowTaskCompletedEventAttributes> {
         self.events
             .iter()
             .skip_while(|e| e.event_id < from_id)
             .find_map(|e| match &e.attributes {
@@ -772,15 +746,15 @@
         }
     }
 
     NextWFTSeqEndIndex::Incomplete(last_index)
 }
 
 #[cfg(test)]
-pub mod tests {
+mod tests {
     use super::*;
     use crate::{
         replay::{HistoryInfo, TestHistoryBuilder},
         test_help::{canned_histories, hist_to_poll_resp, mock_sdk_cfg, MockPollCfg, ResponseType},
         worker::client::mocks::mock_workflow_client,
     };
     use futures::StreamExt;
@@ -802,15 +776,15 @@
                 v.events().to_vec(),
                 v.previous_started_event_id(),
                 v.workflow_task_started_event_id(),
             )
         }
     }
 
-    pub trait TestHBExt {
+    trait TestHBExt {
         fn as_history_update(&self) -> HistoryUpdate;
     }
 
     impl TestHBExt for TestHistoryBuilder {
         fn as_history_update(&self) -> HistoryUpdate {
             self.get_full_history_info().unwrap().into()
         }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/activity_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/activity_state_machine.rs`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         },
         common::v1::{ActivityType, Payload, Payloads},
         enums::v1::{CommandType, EventType, RetryState},
         failure::v1::{failure::FailureInfo, ActivityFailureInfo, CanceledFailureInfo, Failure},
         history::v1::{
             history_event, ActivityTaskCanceledEventAttributes,
             ActivityTaskCompletedEventAttributes, ActivityTaskFailedEventAttributes,
-            ActivityTaskTimedOutEventAttributes, HistoryEvent,
+            ActivityTaskTimedOutEventAttributes,
         },
     },
 };
 
 fsm! {
     pub(super) name ActivityMachine;
     command ActivityMachineCommand;
@@ -113,16 +113,16 @@
         attrs: ScheduleActivity,
         internal_flags: InternalFlagsRef,
         use_compatible_version: bool,
     ) -> NewMachineWithCommand {
         let mut s = Self::from_parts(
             Created {}.into(),
             SharedState {
-                cancellation_type: ActivityCancellationType::from_i32(attrs.cancellation_type)
-                    .unwrap(),
+                cancellation_type: ActivityCancellationType::try_from(attrs.cancellation_type)
+                    .unwrap_or(ActivityCancellationType::TryCancel),
                 attrs,
                 internal_flags,
                 scheduled_event_id: 0,
                 started_event_id: 0,
                 cancelled_before_sent: false,
             },
         );
@@ -282,27 +282,14 @@
                 self.machine_responses_from_cancel_request(c)
             }
             ActivityMachineCommand::Cancel(attrs) => {
                 vec![self.create_cancelation_resolve(attrs).into()]
             }
         })
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        matches!(
-            event.event_type(),
-            EventType::ActivityTaskScheduled
-                | EventType::ActivityTaskStarted
-                | EventType::ActivityTaskCompleted
-                | EventType::ActivityTaskFailed
-                | EventType::ActivityTaskTimedOut
-                | EventType::ActivityTaskCancelRequested
-                | EventType::ActivityTaskCanceled
-        )
-    }
 }
 
 impl TryFrom<CommandType> for ActivityMachineEvents {
     type Error = ();
 
     fn try_from(c: CommandType) -> Result<Self, Self::Error> {
         Ok(match c {
@@ -777,15 +764,15 @@
             attrs.started_event_id,
             attrs.scheduled_event_id,
         )),
         ..Default::default()
     }
 }
 
-pub fn activity_fail_info(
+pub(super) fn activity_fail_info(
     act_type: String,
     act_id: String,
     identity: Option<String>,
     retry_state: RetryState,
     started_event_id: i64,
     scheduled_event_id: i64,
 ) -> FailureInfo {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/cancel_external_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/cancel_external_state_machine.rs`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         common::NamespacedWorkflowExecution,
         workflow_activation::ResolveRequestCancelExternalWorkflow,
     },
     temporal::api::{
         command::v1::{command, Command, RequestCancelExternalWorkflowExecutionCommandAttributes},
         enums::v1::{CancelExternalWorkflowExecutionFailedCause, CommandType, EventType},
         failure::v1::{failure::FailureInfo, ApplicationFailureInfo, Failure},
-        history::v1::{history_event, HistoryEvent},
+        history::v1::history_event,
     },
 };
 
 fsm! {
     pub(super)
     name CancelExternalMachine;
     command CancelExternalCommand;
@@ -206,23 +206,14 @@
                         ..Default::default()
                     }),
                 }
                 .into()]
             }
         })
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        matches!(
-            event.event_type(),
-            EventType::ExternalWorkflowExecutionCancelRequested
-                | EventType::RequestCancelExternalWorkflowExecutionFailed
-                | EventType::RequestCancelExternalWorkflowExecutionInitiated
-        )
-    }
 }
 
 impl Cancellable for CancelExternalMachine {}
 
 #[cfg(test)]
 mod tests {
     use super::*;
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/cancel_workflow_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/cancel_workflow_state_machine.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use super::{
-    workflow_machines::MachineResponse, Cancellable, EventInfo, HistoryEvent,
-    NewMachineWithCommand, OnEventWrapper, WFMachinesAdapter, WFMachinesError,
+    workflow_machines::MachineResponse, Cancellable, EventInfo, NewMachineWithCommand,
+    OnEventWrapper, WFMachinesAdapter, WFMachinesError,
 };
 use crate::worker::workflow::machines::HistEventData;
 use rustfsm::{fsm, StateMachine, TransitionResult};
 use std::convert::TryFrom;
 use temporal_sdk_core_protos::{
     coresdk::workflow_commands::CancelWorkflowExecution,
     temporal::api::{
@@ -23,17 +23,14 @@
 
     CancelWorkflowCommandCreated --(CommandCancelWorkflowExecution)
         --> CancelWorkflowCommandCreated;
     CancelWorkflowCommandCreated --(WorkflowExecutionCanceled)
         --> CancelWorkflowCommandRecorded;
 }
 
-#[derive(thiserror::Error, Debug)]
-pub(super) enum CancelWorkflowMachineError {}
-
 #[derive(Debug, derive_more::Display)]
 pub(super) enum CancelWorkflowCommand {}
 
 pub(super) fn cancel_workflow(attribs: CancelWorkflowExecution) -> NewMachineWithCommand {
     let mut machine = CancelWorkflowMachine::from_parts(Created {}.into(), ());
     OnEventWrapper::on_event_mut(&mut machine, CancelWorkflowMachineEvents::Schedule)
         .expect("Scheduling continue as new machine doesn't fail");
@@ -71,16 +68,16 @@
 }
 
 impl TryFrom<HistEventData> for CancelWorkflowMachineEvents {
     type Error = WFMachinesError;
 
     fn try_from(e: HistEventData) -> Result<Self, Self::Error> {
         let e = e.event;
-        Ok(match EventType::from_i32(e.event_type) {
-            Some(EventType::WorkflowExecutionCanceled) => Self::WorkflowExecutionCanceled,
+        Ok(match EventType::try_from(e.event_type) {
+            Ok(EventType::WorkflowExecutionCanceled) => Self::WorkflowExecutionCanceled,
             _ => {
                 return Err(WFMachinesError::Nondeterminism(format!(
                     "Cancel workflow machine does not handle this event: {e}"
                 )))
             }
         })
     }
@@ -101,18 +98,14 @@
     fn adapt_response(
         &self,
         _my_command: Self::Command,
         _event_info: Option<EventInfo>,
     ) -> Result<Vec<MachineResponse>, WFMachinesError> {
         Ok(vec![])
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        event.event_type() == EventType::WorkflowExecutionCanceled
-    }
 }
 
 impl Cancellable for CancelWorkflowMachine {}
 
 #[cfg(test)]
 mod tests {
     use super::*;
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/child_workflow_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/child_workflow_state_machine.rs`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         enums::v1::{
             CommandType, EventType, RetryState, StartChildWorkflowExecutionFailedCause, TimeoutType,
         },
         failure::v1::{self as failure, failure::FailureInfo, Failure},
         history::v1::{
             history_event, ChildWorkflowExecutionCompletedEventAttributes,
             ChildWorkflowExecutionFailedEventAttributes,
-            ChildWorkflowExecutionStartedEventAttributes, HistoryEvent,
+            ChildWorkflowExecutionStartedEventAttributes,
             StartChildWorkflowExecutionFailedEventAttributes,
         },
     },
 };
 
 fsm! {
     pub(super) name ChildWorkflowMachine;
@@ -94,15 +94,15 @@
         shared on_child_workflow_execution_terminated) --> Cancelled;
     Failed --(Cancel) --> Failed;
     StartFailed --(Cancel) --> StartFailed;
     TimedOut --(Cancel) --> TimedOut;
     Completed --(Cancel) --> Completed;
 }
 
-pub struct ChildWorkflowExecutionStartedEvent {
+pub(super) struct ChildWorkflowExecutionStartedEvent {
     workflow_execution: WorkflowExecution,
     started_event_id: i64,
 }
 
 #[derive(Debug, derive_more::Display)]
 pub(super) enum ChildWorkflowCommand {
     #[display(fmt = "Start")]
@@ -279,15 +279,15 @@
 impl StartEventRecorded {
     pub(super) fn on_child_workflow_execution_started(
         self,
         state: &mut SharedState,
         event: ChildWorkflowExecutionStartedEvent,
     ) -> ChildWorkflowMachineTransition<Started> {
         state.started_event_id = event.started_event_id;
-        state.run_id = event.workflow_execution.run_id.clone();
+        state.run_id.clone_from(&event.workflow_execution.run_id);
         ChildWorkflowMachineTransition::commands(vec![ChildWorkflowCommand::Start(
             event.workflow_execution,
         )])
     }
     pub(super) fn on_start_child_workflow_execution_failed(
         self,
         cause: StartChildWorkflowExecutionFailedCause,
@@ -494,16 +494,16 @@
 
 impl TryFrom<HistEventData> for ChildWorkflowMachineEvents {
     type Error = WFMachinesError;
 
     fn try_from(e: HistEventData) -> Result<Self, Self::Error> {
         let last_task_in_history = e.current_task_is_last_in_history;
         let e = e.event;
-        Ok(match EventType::from_i32(e.event_type) {
-            Some(EventType::StartChildWorkflowExecutionInitiated) => {
+        Ok(match EventType::try_from(e.event_type) {
+            Ok(EventType::StartChildWorkflowExecutionInitiated) => {
                 if let Some(
                     history_event::Attributes::StartChildWorkflowExecutionInitiatedEventAttributes(
                         attrs,
                     ),
                 ) = e.attributes
                 {
                     Self::StartChildWorkflowExecutionInitiated(ChildWorkflowInitiatedData {
@@ -514,37 +514,35 @@
                     })
                 } else {
                     return Err(WFMachinesError::Fatal(
                         "StartChildWorkflowExecutionInitiated attributes were unset".to_string(),
                     ));
                 }
             }
-            Some(EventType::StartChildWorkflowExecutionFailed) => {
+            Ok(EventType::StartChildWorkflowExecutionFailed) => {
                 if let Some(
                     history_event::Attributes::StartChildWorkflowExecutionFailedEventAttributes(
                         StartChildWorkflowExecutionFailedEventAttributes { cause, .. },
                     ),
                 ) = e.attributes
                 {
                     Self::StartChildWorkflowExecutionFailed(
-                        StartChildWorkflowExecutionFailedCause::from_i32(cause).ok_or_else(
-                            || {
-                                WFMachinesError::Fatal(
-                                    "Invalid StartChildWorkflowExecutionFailedCause".to_string(),
-                                )
-                            },
-                        )?,
+                        StartChildWorkflowExecutionFailedCause::try_from(cause).map_err(|_| {
+                            WFMachinesError::Fatal(
+                                "Invalid StartChildWorkflowExecutionFailedCause".to_string(),
+                            )
+                        })?,
                     )
                 } else {
                     return Err(WFMachinesError::Fatal(
                         "StartChildWorkflowExecutionFailed attributes were unset".to_string(),
                     ));
                 }
             }
-            Some(EventType::ChildWorkflowExecutionStarted) => {
+            Ok(EventType::ChildWorkflowExecutionStarted) => {
                 if let Some(
                     history_event::Attributes::ChildWorkflowExecutionStartedEventAttributes(
                         ChildWorkflowExecutionStartedEventAttributes {
                             workflow_execution: Some(we),
                             ..
                         },
                     ),
@@ -557,60 +555,58 @@
                 } else {
                     return Err(WFMachinesError::Fatal(
                         "ChildWorkflowExecutionStarted attributes were unset or malformed"
                             .to_string(),
                     ));
                 }
             }
-            Some(EventType::ChildWorkflowExecutionCompleted) => {
+            Ok(EventType::ChildWorkflowExecutionCompleted) => {
                 if let Some(
                     history_event::Attributes::ChildWorkflowExecutionCompletedEventAttributes(
                         ChildWorkflowExecutionCompletedEventAttributes { result, .. },
                     ),
                 ) = e.attributes
                 {
                     Self::ChildWorkflowExecutionCompleted(result)
                 } else {
                     return Err(WFMachinesError::Fatal(
                         "ChildWorkflowExecutionCompleted attributes were unset or malformed"
                             .to_string(),
                     ));
                 }
             }
-            Some(EventType::ChildWorkflowExecutionFailed) => {
+            Ok(EventType::ChildWorkflowExecutionFailed) => {
                 if let Some(
                     history_event::Attributes::ChildWorkflowExecutionFailedEventAttributes(attrs),
                 ) = e.attributes
                 {
                     Self::ChildWorkflowExecutionFailed(attrs)
                 } else {
                     return Err(WFMachinesError::Fatal(
                         "ChildWorkflowExecutionFailed attributes were unset".to_string(),
                     ));
                 }
             }
-            Some(EventType::ChildWorkflowExecutionTimedOut) => {
+            Ok(EventType::ChildWorkflowExecutionTimedOut) => {
                 if let Some(
                     history_event::Attributes::ChildWorkflowExecutionTimedOutEventAttributes(atts),
                 ) = e.attributes
                 {
                     Self::ChildWorkflowExecutionTimedOut(atts.retry_state())
                 } else {
                     return Err(WFMachinesError::Fatal(
                         "ChildWorkflowExecutionTimedOut attributes were unset or malformed"
                             .to_string(),
                     ));
                 }
             }
-            Some(EventType::ChildWorkflowExecutionTerminated) => {
+            Ok(EventType::ChildWorkflowExecutionTerminated) => {
                 Self::ChildWorkflowExecutionTerminated
             }
-            Some(EventType::ChildWorkflowExecutionCanceled) => {
-                Self::ChildWorkflowExecutionCancelled
-            }
+            Ok(EventType::ChildWorkflowExecutionCanceled) => Self::ChildWorkflowExecutionCancelled,
             _ => {
                 return Err(WFMachinesError::Nondeterminism(format!(
                     "Child workflow machine does not handle this event: {e:?}"
                 )))
             }
         })
     }
@@ -704,28 +700,14 @@
                 ) {
                     resps.push(self.resolve_cancelled_msg().into())
                 }
                 resps
             }
         })
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        matches!(
-            event.event_type(),
-            EventType::StartChildWorkflowExecutionInitiated
-                | EventType::StartChildWorkflowExecutionFailed
-                | EventType::ChildWorkflowExecutionStarted
-                | EventType::ChildWorkflowExecutionCompleted
-                | EventType::ChildWorkflowExecutionFailed
-                | EventType::ChildWorkflowExecutionTimedOut
-                | EventType::ChildWorkflowExecutionTerminated
-                | EventType::ChildWorkflowExecutionCanceled
-        )
-    }
 }
 
 impl TryFrom<CommandType> for ChildWorkflowMachineEvents {
     type Error = ();
 
     fn try_from(c: CommandType) -> Result<Self, Self::Error> {
         Ok(match c {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/complete_workflow_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/complete_workflow_state_machine.rs`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 use rustfsm::{fsm, StateMachine, TransitionResult};
 use std::convert::TryFrom;
 use temporal_sdk_core_protos::{
     coresdk::workflow_commands::CompleteWorkflowExecution,
     temporal::api::{
         command::v1::Command,
         enums::v1::{CommandType, EventType},
-        history::v1::HistoryEvent,
     },
 };
 
 fsm! {
     pub(super)
     name CompleteWorkflowMachine;
     command CompleteWFCommand;
@@ -99,17 +98,14 @@
             command_type: CommandType::CompleteWorkflowExecution as i32,
             attributes: Some(self.attribs.into()),
         };
         TransitionResult::commands(vec![CompleteWFCommand::AddCommand(cmd)])
     }
 }
 
-#[derive(thiserror::Error, Debug)]
-pub(super) enum CompleteWorkflowMachineError {}
-
 #[derive(Default, Clone)]
 pub(super) struct CompleteWorkflowCommandCreated {}
 
 #[derive(Default, Clone)]
 pub(super) struct CompleteWorkflowCommandRecorded {}
 
 impl From<CompleteWorkflowCommandCreated> for CompleteWorkflowCommandRecorded {
@@ -122,14 +118,10 @@
     fn adapt_response(
         &self,
         _my_command: Self::Command,
         _event_info: Option<EventInfo>,
     ) -> Result<Vec<MachineResponse>, WFMachinesError> {
         Ok(vec![])
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        event.event_type() == EventType::WorkflowExecutionCompleted
-    }
 }
 
 impl Cancellable for CompleteWorkflowMachine {}
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/continue_as_new_workflow_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/continue_as_new_workflow_state_machine.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use super::{
-    Cancellable, EventInfo, HistoryEvent, MachineResponse, NewMachineWithCommand, OnEventWrapper,
+    Cancellable, EventInfo, MachineResponse, NewMachineWithCommand, OnEventWrapper,
     WFMachinesAdapter, WFMachinesError,
 };
 use crate::worker::workflow::machines::HistEventData;
 use rustfsm::{fsm, StateMachine, TransitionResult};
 use std::convert::TryFrom;
 use temporal_sdk_core_protos::{
     coresdk::workflow_commands::ContinueAsNewWorkflowExecution,
@@ -103,18 +103,14 @@
     fn adapt_response(
         &self,
         _my_command: Self::Command,
         _event_info: Option<EventInfo>,
     ) -> Result<Vec<MachineResponse>, WFMachinesError> {
         Ok(vec![])
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        event.event_type() == EventType::WorkflowExecutionContinuedAsNew
-    }
 }
 
 impl Cancellable for ContinueAsNewWorkflowMachine {}
 
 #[cfg(test)]
 mod tests {
     use super::*;
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/fail_workflow_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/fail_workflow_state_machine.rs`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 use rustfsm::{fsm, StateMachine, TransitionResult};
 use std::convert::TryFrom;
 use temporal_sdk_core_protos::{
     coresdk::workflow_commands::FailWorkflowExecution,
     temporal::api::{
         command::v1::Command as ProtoCommand,
         enums::v1::{CommandType, EventType},
-        history::v1::HistoryEvent,
     },
 };
 
 fsm! {
     pub(super) name FailWorkflowMachine;
     command FailWFCommand;
     error WFMachinesError;
@@ -113,14 +112,10 @@
     fn adapt_response(
         &self,
         _my_command: Self::Command,
         _event_info: Option<EventInfo>,
     ) -> Result<Vec<MachineResponse>, WFMachinesError> {
         Ok(vec![])
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        event.event_type() == EventType::WorkflowExecutionFailed
-    }
 }
 
 impl Cancellable for FailWorkflowMachine {}
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/local_activity_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/local_activity_state_machine.rs`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         workflow_activation::ResolveActivity,
         workflow_commands::ActivityCancellationType,
     },
     temporal::api::{
         command::v1::{command, RecordMarkerCommandAttributes},
         enums::v1::{CommandType, EventType, RetryState},
         failure::v1::{failure::FailureInfo, Failure},
-        history::v1::HistoryEvent,
     },
     utilities::TryIntoOrNone,
 };
 
 fsm! {
     pub(super) name LocalActivityMachine;
     command LocalActivityCommand;
@@ -795,18 +794,14 @@
             LocalActivityCommand::RequestCancel => {
                 Ok(vec![MachineResponse::RequestCancelLocalActivity(
                     self.shared_state.attrs.seq,
                 )])
             }
         }
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        event.is_local_activity_marker()
-    }
 }
 
 impl TryFrom<CommandType> for LocalActivityMachineEvents {
     type Error = ();
 
     fn try_from(c: CommandType) -> Result<Self, Self::Error> {
         Ok(match c {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/mod.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -80,19 +80,14 @@
 #[enum_dispatch::enum_dispatch(Machines)]
 trait TemporalStateMachine {
     fn handle_command(
         &mut self,
         command_type: CommandType,
     ) -> Result<Vec<MachineResponse>, WFMachinesError>;
 
-    /// Returns true if this machine is compatible with the provided event. Provides a way to know
-    /// ahead of time if it's worth trying to call [TemporalStateMachine::handle_event] without
-    /// requiring mutable access.
-    fn matches_event(&self, event: &HistoryEvent) -> bool;
-
     /// Tell the state machine to handle some event. Returns a list of responses that can be used
     /// to update the overall state of the workflow. EX: To issue outgoing WF activations.
     fn handle_event(
         &mut self,
         event: HistEventData,
     ) -> Result<Vec<MachineResponse>, WFMachinesError>;
 
@@ -146,18 +141,14 @@
                 "Unexpected command {:?} generated by a {:?} machine",
                 command_type,
                 self.name()
             )))
         }
     }
 
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        self.matches_event(event)
-    }
-
     fn handle_event(
         &mut self,
         event_dat: HistEventData,
     ) -> Result<Vec<MachineResponse>, WFMachinesError> {
         trace!(
             event = %event_dat.event,
             machine_name = %self.name(),
@@ -236,19 +227,14 @@
     /// processed, perform any handling that needs inform the [WorkflowMachines] instance of some
     /// action to be taken in response to that command.
     fn adapt_response(
         &self,
         my_command: Self::Command,
         event_info: Option<EventInfo>,
     ) -> Result<Vec<MachineResponse>, WFMachinesError>;
-
-    /// Returns true if this machine is compatible with the provided event. Provides a way to know
-    /// ahead of time if it's worth trying to call [TemporalStateMachine::handle_event] without
-    /// requiring mutable access.
-    fn matches_event(&self, event: &HistoryEvent) -> bool;
 }
 
 /// Wraps a history event with extra relevant data that a machine might care about while the event
 /// is being applied to it.
 #[derive(Debug, derive_more::Display)]
 #[display(fmt = "{event}")]
 struct HistEventData {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/modify_workflow_properties_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/modify_workflow_properties_state_machine.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 };
 use rustfsm::{fsm, StateMachine, TransitionResult};
 use temporal_sdk_core_protos::{
     coresdk::workflow_commands::ModifyWorkflowProperties,
     temporal::api::{
         command::v1::Command,
         enums::v1::{CommandType, EventType},
-        history::v1::HistoryEvent,
     },
 };
 
 fsm! {
     pub(super) name ModifyWorkflowPropertiesMachine;
     command ModifyWorkflowPropertiesMachineCommand;
     error WFMachinesError;
@@ -59,18 +58,14 @@
         _my_command: Self::Command,
         _event_info: Option<EventInfo>,
     ) -> Result<Vec<MachineResponse>, Self::Error> {
         Err(Self::Error::Nondeterminism(
             "ModifyWorkflowProperties does not use state machine commands".to_string(),
         ))
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        matches!(event.event_type(), EventType::WorkflowPropertiesModified)
-    }
 }
 
 impl Cancellable for ModifyWorkflowPropertiesMachine {}
 
 impl TryFrom<HistEventData> for ModifyWorkflowPropertiesMachineEvents {
     type Error = WFMachinesError;
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/patch_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/patch_state_machine.rs`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     coresdk::{common::build_has_change_marker_details, AsJsonPayloadExt},
     temporal::api::{
         command::v1::{
             Command, RecordMarkerCommandAttributes, UpsertWorkflowSearchAttributesCommandAttributes,
         },
         common::v1::SearchAttributes,
         enums::v1::CommandType,
-        history::v1::HistoryEvent,
     },
 };
 
 pub(crate) const VERSION_SEARCH_ATTR_KEY: &str = "TemporalChangeVersion";
 
 fsm! {
     pub(super) name PatchMachine;
@@ -233,18 +232,14 @@
     fn adapt_response(
         &self,
         _my_command: Self::Command,
         _event_info: Option<EventInfo>,
     ) -> Result<Vec<MachineResponse>, WFMachinesError> {
         panic!("Patch machine does not produce commands")
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        event.get_patch_marker_details().is_some()
-    }
 }
 
 impl Cancellable for PatchMachine {}
 
 impl TryFrom<CommandType> for PatchMachineEvents {
     type Error = ();
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/signal_external_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/signal_external_state_machine.rs`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         IntoPayloadsExt,
     },
     temporal::api::{
         command::v1::{command, Command, SignalExternalWorkflowExecutionCommandAttributes},
         common::v1::WorkflowExecution as UpstreamWE,
         enums::v1::{CommandType, EventType, SignalExternalWorkflowExecutionFailedCause},
         failure::v1::{failure::FailureInfo, ApplicationFailureInfo, CanceledFailureInfo, Failure},
-        history::v1::{history_event, HistoryEvent},
+        history::v1::history_event,
     },
 };
 
 const SIG_CANCEL_MSG: &str = "Signal was cancelled before being sent";
 
 fsm! {
     pub(super) name SignalExternalMachine;
@@ -256,23 +256,14 @@
                 .into()]
             }
             SignalExternalCommand::Cancelled => {
                 panic!("Cancelled command not expected as part of non-cancel transition")
             }
         })
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        matches!(
-            event.event_type(),
-            EventType::ExternalWorkflowExecutionSignaled
-                | EventType::SignalExternalWorkflowExecutionInitiated
-                | EventType::SignalExternalWorkflowExecutionFailed
-        )
-    }
 }
 
 impl Cancellable for SignalExternalMachine {
     fn cancel(&mut self) -> Result<Vec<MachineResponse>, MachineError<Self::Error>> {
         let res = OnEventWrapper::on_event_mut(self, SignalExternalMachineEvents::Cancel)?;
         let mut ret = vec![];
         match res.first() {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/timer_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/timer_state_machine.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         workflow_activation::FireTimer,
         workflow_commands::{CancelTimer, StartTimer},
         HistoryEventId,
     },
     temporal::api::{
         command::v1::Command,
         enums::v1::{CommandType, EventType},
-        history::v1::{history_event, HistoryEvent, TimerFiredEventAttributes},
+        history::v1::{history_event, TimerFiredEventAttributes},
     },
 };
 
 fsm! {
     pub(super) name TimerMachine;
     command TimerMachineCommand;
     error WFMachinesError;
@@ -229,21 +229,14 @@
             TimerMachineCommand::Complete => vec![FireTimer {
                 seq: self.shared_state.attrs.seq,
             }
             .into()],
             TimerMachineCommand::IssueCancelCmd(c) => vec![MachineResponse::IssueNewCommand(c)],
         })
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        matches!(
-            event.event_type(),
-            EventType::TimerStarted | EventType::TimerCanceled | EventType::TimerFired
-        )
-    }
 }
 
 impl Cancellable for TimerMachine {
     fn cancel(&mut self) -> Result<Vec<MachineResponse>, MachineError<Self::Error>> {
         Ok(
             match OnEventWrapper::on_event_mut(self, TimerMachineEvents::Cancel)?.pop() {
                 Some(TimerMachineCommand::IssueCancelCmd(cmd)) => {
@@ -306,16 +299,16 @@
     #[tokio::test]
     async fn mismatched_timer_ids_errors() {
         let t = canned_histories::single_timer("badid");
         let mut mock_cfg = MockPollCfg::from_hist_builder(t);
         mock_cfg.num_expected_fails = 1;
         mock_cfg.expect_fail_wft_matcher = Box::new(move |_, cause, f| {
             matches!(cause, WorkflowTaskFailedCause::NonDeterministicError)
-                && matches!(f, Some(Failure { source, .. }) 
-            if source.contains("Timer fired event did not have expected timer id 1"))
+                && matches!(f, Some(Failure {message, .. })
+            if message.contains("Timer fired event did not have expected timer id 1"))
         });
         let mut worker = build_fake_sdk(mock_cfg);
         worker.register_wf(DEFAULT_WORKFLOW_TYPE, |ctx: WfContext| async move {
             ctx.timer(Duration::from_secs(5)).await;
             Ok(().into())
         });
         worker.run().await.unwrap();
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/transition_coverage.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/transition_coverage.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 //! Look, I'm not happy about the code in here, and you shouldn't be either. This is all an awful,
 //! dirty hack to work around the fact that there's no such thing as "run this after all unit tests"
 //! in stable Rust. Don't do the things in here. They're bad. This is test only code, and should
 //! never ever be removed from behind `#[cfg(test)]` compilation.
 
 use dashmap::{mapref::entry::Entry, DashMap, DashSet};
+use once_cell::sync::Lazy;
 use std::{
     path::PathBuf,
     sync::{
         mpsc::{sync_channel, SyncSender},
         Mutex,
     },
     thread::JoinHandle,
     time::Duration,
 };
 
 // During test we want to know about which transitions we've covered in state machines
-lazy_static::lazy_static! {
-    static ref COVERED_TRANSITIONS: DashMap<String, DashSet<CoveredTransition>>
-        = DashMap::new();
-    static ref COVERAGE_SENDER: SyncSender<(String, CoveredTransition)> =
-        spawn_save_coverage_at_end();
-    static ref THREAD_HANDLE: Mutex<Option<JoinHandle<()>>> = Mutex::new(None);
-}
+static COVERED_TRANSITIONS: Lazy<DashMap<String, DashSet<CoveredTransition>>> =
+    Lazy::new(DashMap::new);
+static COVERAGE_SENDER: Lazy<SyncSender<(String, CoveredTransition)>> =
+    Lazy::new(spawn_save_coverage_at_end);
+static THREAD_HANDLE: Lazy<Mutex<Option<JoinHandle<()>>>> = Lazy::new(|| Mutex::new(None));
 
 #[derive(Eq, PartialEq, Hash, Debug)]
 struct CoveredTransition {
     from_state: String,
     to_state: String,
     event: String,
 }
 
-pub fn add_coverage(machine_name: String, from_state: String, to_state: String, event: String) {
+pub(super) fn add_coverage(
+    machine_name: String,
+    from_state: String,
+    to_state: String,
+    event: String,
+) {
     let ct = CoveredTransition {
         from_state,
         to_state,
         event,
     };
     let _ = COVERAGE_SENDER.send((machine_name, ct));
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/update_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/update_state_machine.rs`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
         workflow_commands::{update_response, UpdateResponse},
     },
     temporal::api::{
         command::v1::{command, ProtocolMessageCommandAttributes},
         common::v1::Payload,
         enums::v1::{CommandType, EventType},
         failure::v1::Failure,
-        history::v1::HistoryEvent,
         protocol::v1::Message as ProtocolMessage,
         update::v1::{outcome, Acceptance, Outcome, Rejection, Response},
     },
     utilities::pack_any,
 };
 
 fsm! {
@@ -267,23 +266,14 @@
                     outcome: Some(Outcome {
                         value: Some(outcome::Value::Failure(f)),
                     }),
                 }),
             )?,
         })
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        matches!(
-            event.event_type(),
-            EventType::WorkflowExecutionUpdateAccepted
-                | EventType::WorkflowExecutionUpdateRejected
-                | EventType::WorkflowExecutionUpdateCompleted
-        )
-    }
 }
 
 impl TryFrom<CommandType> for UpdateMachineEvents {
     type Error = ();
 
     fn try_from(c: CommandType) -> Result<Self, Self::Error> {
         Ok(match c {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/upsert_search_attributes_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/upsert_search_attributes_state_machine.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 };
 use rustfsm::{fsm, StateMachine, TransitionResult};
 use temporal_sdk_core_protos::{
     coresdk::workflow_commands::UpsertWorkflowSearchAttributes,
     temporal::api::{
         command::v1::{command, Command, UpsertWorkflowSearchAttributesCommandAttributes},
         common::v1::SearchAttributes,
-        enums::v1::{CommandType, EventType},
-        history::v1::{history_event, HistoryEvent},
+        enums::v1::CommandType,
+        history::v1::history_event,
     },
 };
 
 /// By default the server permits SA values under 2k.
 pub(crate) const MAX_SEARCH_ATTR_PAYLOAD_SIZE: usize = 2048;
 
 fsm! {
@@ -133,22 +133,14 @@
         _event_info: Option<EventInfo>,
     ) -> Result<Vec<MachineResponse>, Self::Error> {
         // No implementation needed until this state machine emits state machine commands
         Err(Self::Error::Nondeterminism(
             "UpsertWorkflowSearchAttributesMachine does not use commands".to_string(),
         ))
     }
-
-    /// Filters for EventType::UpsertWorkflowSearchAttributes
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        matches!(
-            event.event_type(),
-            EventType::UpsertWorkflowSearchAttributes
-        )
-    }
 }
 
 impl Cancellable for UpsertSearchAttributesMachine {}
 
 // Converts the generic history event with type EventType::UpsertWorkflowSearchAttributes into the
 // UpsertSearchAttributesMachine-specific event type
 // UpsertSearchAttributesMachineEvents::CommandRecorded.
@@ -210,16 +202,18 @@
         coresdk::{
             workflow_activation::{workflow_activation_job, WorkflowActivationJob},
             workflow_commands::SetPatchMarker,
             workflow_completion::WorkflowActivationCompletion,
             AsJsonPayloadExt,
         },
         temporal::api::{
-            command::v1::command::Attributes, common::v1::Payload,
-            history::v1::UpsertWorkflowSearchAttributesEventAttributes,
+            command::v1::command::Attributes,
+            common::v1::Payload,
+            enums::v1::EventType,
+            history::v1::{HistoryEvent, UpsertWorkflowSearchAttributesEventAttributes},
         },
         DEFAULT_WORKFLOW_TYPE,
     };
     use temporal_sdk_core_test_utils::WorkerTestHelpers;
 
     #[tokio::test]
     async fn upsert_search_attrs_from_workflow() {
@@ -287,15 +281,14 @@
             attributes: Some(
                 history_event::Attributes::UpsertWorkflowSearchAttributesEventAttributes(
                     sa_attribs,
                 ),
             ),
             ..Default::default()
         };
-        assert!(sm.matches_event(&recorded_history_event));
         let cmd_recorded_sm_event = HistEventData {
             event: recorded_history_event,
             replaying: false,
             current_task_is_last_in_history: true,
         }
         .try_into()
         .unwrap();
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/workflow_machines/local_acts.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/workflow_machines/local_acts.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/workflow_machines.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/workflow_machines.rs`

 * *Files 2% similar despite different names*

```diff
@@ -88,26 +88,26 @@
     /// The event id of the next workflow task started event that the machines need to process.
     /// Eventually, this number should reach the started id in the latest history update, but
     /// we must incrementally apply the history while communicating with lang.
     next_started_event_id: i64,
     /// The event id of the most recent event processed. It's possible in some situations (ex legacy
     /// queries) to receive a history with no new workflow tasks. If the last history we processed
     /// also had no new tasks, we need a way to know not to apply the same events over again.
-    pub last_processed_event: i64,
+    pub(crate) last_processed_event: i64,
     /// True if the workflow is replaying from history
-    pub replaying: bool,
+    pub(crate) replaying: bool,
     /// Workflow identifier
-    pub workflow_id: String,
+    pub(crate) workflow_id: String,
     /// Workflow type identifier. (Function name, class, etc)
-    pub workflow_type: String,
+    pub(crate) workflow_type: String,
     /// Identifies the current run
-    pub run_id: String,
+    pub(crate) run_id: String,
     /// Is set to true once we've seen the final event in workflow history, to avoid accidentally
     /// re-applying the final workflow task.
-    pub have_seen_terminal_event: bool,
+    pub(crate) have_seen_terminal_event: bool,
     /// The time the workflow execution began, as told by the WEStarted event
     workflow_start_time: Option<SystemTime>,
     /// The time the workflow execution finished, as determined by when the machines handled
     /// a terminal workflow command. If this is `Some`, you know the workflow is ended.
     workflow_end_time: Option<SystemTime>,
     /// The WFT start time if it has been established
     wft_start_time: Option<SystemTime>,
@@ -153,15 +153,15 @@
     /// Contains extra local-activity related data
     local_activity_data: LocalActivityData,
 
     /// The workflow that is being driven by this instance of the machines
     drive_me: DrivenWorkflow,
 
     /// Metrics context
-    pub metrics: MetricsContext,
+    pub(crate) metrics: MetricsContext,
     worker_config: Arc<WorkerConfig>,
 }
 
 #[derive(Debug, derive_more::Display)]
 #[display(fmt = "Cmd&Machine({command})")]
 struct CommandAndMachine {
     command: MachineAssociatedCommand,
@@ -372,15 +372,14 @@
 
     pub(crate) fn prepare_for_wft_response(&mut self) -> MachinesWFTResponseContent {
         MachinesWFTResponseContent {
             replaying: self.replaying,
             has_pending_jobs: self.has_pending_jobs(),
             have_seen_terminal_event: self.have_seen_terminal_event,
             have_pending_la_resolutions: self.has_pending_la_resolutions(),
-            last_processed_event: self.last_processed_event,
             me: self,
         }
     }
 
     /// Fetches commands which are ready for processing from the state machines, generally to be
     /// sent off to the server. They are not removed from the internal queue, that happens when
     /// corresponding history events from the server are being handled.
@@ -901,16 +900,16 @@
 
         Ok(EventHandlingOutcome::Normal)
     }
 
     fn handle_non_stateful_event(&mut self, event_dat: HistEventData) -> Result<()> {
         trace!(event = %event_dat.event, "handling non-stateful event");
         let event_id = event_dat.event.event_id;
-        match EventType::from_i32(event_dat.event.event_type) {
-            Some(EventType::WorkflowExecutionStarted) => {
+        match EventType::try_from(event_dat.event.event_type) {
+            Ok(EventType::WorkflowExecutionStarted) => {
                 if let Some(history_event::Attributes::WorkflowExecutionStartedEventAttributes(
                     attrs,
                 )) = event_dat.event.attributes
                 {
                     if let Some(st) = event_dat.event.event_time.clone() {
                         let as_systime: SystemTime = st.try_into()?;
                         self.workflow_start_time = Some(as_systime);
@@ -928,32 +927,32 @@
                     );
                 } else {
                     return Err(WFMachinesError::Fatal(format!(
                         "WorkflowExecutionStarted event did not have appropriate attributes: {event_dat}"
                     )));
                 }
             }
-            Some(EventType::WorkflowTaskScheduled) => {
+            Ok(EventType::WorkflowTaskScheduled) => {
                 let wf_task_sm = WorkflowTaskMachine::new(self.next_started_event_id);
                 let key = self.all_machines.insert(wf_task_sm.into());
                 self.submachine_handle_event(key, event_dat)?;
                 self.machines_by_event_id.insert(event_id, key);
             }
-            Some(EventType::WorkflowExecutionSignaled) => {
+            Ok(EventType::WorkflowExecutionSignaled) => {
                 if let Some(history_event::Attributes::WorkflowExecutionSignaledEventAttributes(
                     attrs,
                 )) = event_dat.event.attributes
                 {
                     self.drive_me
                         .send_job(workflow_activation::SignalWorkflow::from(attrs).into());
                 } else {
                     // err
                 }
             }
-            Some(EventType::WorkflowExecutionCancelRequested) => {
+            Ok(EventType::WorkflowExecutionCancelRequested) => {
                 if let Some(
                     history_event::Attributes::WorkflowExecutionCancelRequestedEventAttributes(
                         attrs,
                     ),
                 ) = event_dat.event.attributes
                 {
                     self.drive_me
@@ -1289,40 +1288,28 @@
                 WFCommand::RequestCancelActivity(attrs) => {
                     self.process_cancellation(CommandID::Activity(attrs.seq))?;
                 }
                 WFCommand::RequestCancelLocalActivity(attrs) => {
                     self.process_cancellation(CommandID::LocalActivity(attrs.seq))?;
                 }
                 WFCommand::CompleteWorkflow(attrs) => {
-                    if !self.replaying {
-                        self.metrics.wf_completed();
-                    }
                     self.add_terminal_command(complete_workflow(attrs));
                 }
                 WFCommand::FailWorkflow(attrs) => {
-                    if !self.replaying {
-                        self.metrics.wf_failed();
-                    }
                     self.add_terminal_command(fail_workflow(attrs));
                 }
                 WFCommand::ContinueAsNew(attrs) => {
-                    if !self.replaying {
-                        self.metrics.wf_continued_as_new();
-                    }
                     let attrs = self.augment_continue_as_new_with_current_values(attrs);
                     let use_compat = self.determine_use_compatible_flag(
                         attrs.versioning_intent(),
                         &attrs.task_queue,
                     );
                     self.add_terminal_command(continue_as_new(attrs, use_compat));
                 }
                 WFCommand::CancelWorkflow(attrs) => {
-                    if !self.replaying {
-                        self.metrics.wf_canceled();
-                    }
                     self.add_terminal_command(cancel_workflow(attrs));
                 }
                 WFCommand::SetPatchMarker(attrs) => {
                     // Do not create commands for change IDs that we have already created commands
                     // for.
                     let encountered_entry = self.encountered_patch_markers.get(&attrs.patch_id);
                     if !matches!(encountered_entry,
@@ -1531,15 +1518,15 @@
                 attrs.search_attributes = started_info
                     .search_attrs
                     .clone()
                     .map(Into::into)
                     .unwrap_or_default();
             }
             if attrs.retry_policy.is_none() {
-                attrs.retry_policy = started_info.retry_policy.clone();
+                attrs.retry_policy.clone_from(&started_info.retry_policy);
             }
         }
         attrs
     }
 
     /// Given a user's versioning intent for a command and that command's target task queue,
     /// returns whether or not the command should set the flag for attempting to stick within the
@@ -1556,33 +1543,36 @@
         }
     }
 }
 
 /// Contains everything workflow machine internals need to bubble up when we're getting ready to
 /// respond with a WFT completion. Allows for lazy mutation of the machine, since mutation is not
 /// desired unless we are actually going to respond to the WFT, which may not always happen.
-pub struct MachinesWFTResponseContent<'a> {
+pub(crate) struct MachinesWFTResponseContent<'a> {
     me: &'a mut WorkflowMachines,
-    pub replaying: bool,
-    pub has_pending_jobs: bool,
-    pub have_seen_terminal_event: bool,
-    pub have_pending_la_resolutions: bool,
-    pub last_processed_event: i64,
+    pub(crate) replaying: bool,
+    pub(crate) has_pending_jobs: bool,
+    pub(crate) have_seen_terminal_event: bool,
+    pub(crate) have_pending_la_resolutions: bool,
 }
+
 impl<'a> MachinesWFTResponseContent<'a> {
-    pub fn commands(&self) -> Peekable<impl Iterator<Item = ProtoCommand> + '_> {
+    pub(crate) fn commands(&self) -> Peekable<impl Iterator<Item = ProtoCommand> + '_> {
         self.me.get_commands().peekable()
     }
-    pub fn has_messages(&self) -> bool {
+
+    pub(crate) fn has_messages(&self) -> bool {
         !self.me.message_outbox.is_empty()
     }
-    pub fn messages(&mut self) -> Vec<ProtocolMessage> {
+
+    pub(crate) fn messages(&mut self) -> Vec<ProtocolMessage> {
         self.me.message_outbox.drain(..).collect()
     }
-    pub fn metadata_for_complete(&mut self) -> WorkflowTaskCompletedMetadata {
+
+    pub(crate) fn metadata_for_complete(&mut self) -> WorkflowTaskCompletedMetadata {
         self.me.get_metadata_for_wft_complete()
     }
 }
 
 fn str_to_randomness_seed(run_id: &str) -> u64 {
     // This was originally `DefaultHasher` but that is potentially unstable across Rust releases.
     // This must forever be `SipHasher13` now or we risk breaking history compat.
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/workflow_task_state_machine.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/machines/workflow_task_state_machine.rs`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 use rustfsm::{fsm, StateMachine, TransitionResult};
 use std::{
     convert::{TryFrom, TryInto},
     time::SystemTime,
 };
 use temporal_sdk_core_protos::temporal::api::{
     enums::v1::{CommandType, EventType, WorkflowTaskFailedCause},
-    history::v1::{history_event::Attributes::WorkflowTaskFailedEventAttributes, HistoryEvent},
+    history::v1::history_event::Attributes::WorkflowTaskFailedEventAttributes,
 };
 
 fsm! {
     pub(super) name WorkflowTaskMachine;
     command WFTaskMachineCommand;
     error WFMachinesError;
     shared_state SharedState;
@@ -84,25 +84,14 @@
                 }])
             }
             WFTaskMachineCommand::RunIdOnWorkflowResetUpdate { run_id } => {
                 Ok(vec![MachineResponse::UpdateRunIdOnWorkflowReset { run_id }])
             }
         }
     }
-
-    fn matches_event(&self, event: &HistoryEvent) -> bool {
-        matches!(
-            event.event_type(),
-            EventType::WorkflowTaskScheduled
-                | EventType::WorkflowTaskStarted
-                | EventType::WorkflowTaskTimedOut
-                | EventType::WorkflowTaskCompleted
-                | EventType::WorkflowTaskFailed
-        )
-    }
 }
 
 impl TryFrom<HistEventData> for WorkflowTaskMachineEvents {
     type Error = WFMachinesError;
 
     fn try_from(e: HistEventData) -> Result<Self, Self::Error> {
         let e = e.event;
@@ -132,17 +121,17 @@
             EventType::WorkflowTaskTimedOut => Self::WorkflowTaskTimedOut,
             EventType::WorkflowTaskCompleted => Self::WorkflowTaskCompleted,
             EventType::WorkflowTaskFailed => {
                 if let Some(attributes) = e.attributes {
                     Self::WorkflowTaskFailed(WFTFailedDat {
                         new_run_id: match attributes {
                             WorkflowTaskFailedEventAttributes(a) => {
-                                let cause = WorkflowTaskFailedCause::from_i32(a.cause);
+                                let cause = WorkflowTaskFailedCause::try_from(a.cause);
                                 match cause {
-                                    Some(WorkflowTaskFailedCause::ResetWorkflow) => {
+                                    Ok(WorkflowTaskFailedCause::ResetWorkflow) => {
                                         Some(a.new_run_id)
                                     }
                                     _ => None,
                                 }
                             }
                             _ => None,
                         },
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/managed_run.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/managed_run.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use crate::{
     abstractions::dbg_panic,
     protosext::{protocol_messages::IncomingProtocolMessage, WorkflowActivationExt},
+    telemetry::metrics,
     worker::{
         workflow::{
             history_update::HistoryPaginator,
             machines::{MachinesWFTResponseContent, WorkflowMachines},
             ActivationAction, ActivationCompleteOutcome, ActivationCompleteResult,
             ActivationOrAuto, BufferedTasks, DrivenWorkflow, EvictionRequestResult,
             FailedActivationWFTReport, HeartbeatTimeoutMsg, HistoryUpdate,
@@ -19,27 +20,31 @@
 };
 use futures_util::future::AbortHandle;
 use std::{
     collections::HashSet,
     mem,
     ops::Add,
     rc::Rc,
-    sync::mpsc::Sender,
+    sync::{mpsc::Sender, Arc},
     time::{Duration, Instant},
 };
+use temporal_sdk_core_api::{errors::WorkflowErrorType, worker::WorkerConfig};
 use temporal_sdk_core_protos::{
     coresdk::{
         workflow_activation::{
             create_evict_activation, query_to_job, remove_from_cache::EvictionReason,
-            workflow_activation_job, RemoveFromCache, WorkflowActivation,
+            workflow_activation_job, WorkflowActivation,
         },
-        workflow_commands::QueryResult,
+        workflow_commands::{FailWorkflowExecution, QueryResult},
         workflow_completion,
     },
-    temporal::api::{enums::v1::WorkflowTaskFailedCause, failure::v1::Failure},
+    temporal::api::{
+        command::v1::command::Attributes as CmdAttribs, enums::v1::WorkflowTaskFailedCause,
+        failure::v1::Failure,
+    },
     TaskToken,
 };
 use tokio::sync::oneshot;
 use tracing::Span;
 
 type Result<T, E = WFMachinesError> = std::result::Result<T, E>;
 pub(super) type RunUpdateAct = Option<ActivationOrAuto>;
@@ -88,36 +93,39 @@
     /// duplicating field values. Remove this once https://github.com/tokio-rs/tracing/issues/2334
     /// is fixed.
     recorded_span_ids: HashSet<tracing::Id>,
     metrics: MetricsContext,
     /// We store the paginator used for our own run's history fetching
     paginator: Option<HistoryPaginator>,
     completion_waiting_on_page_fetch: Option<RunActivationCompletion>,
+    config: Arc<WorkerConfig>,
 }
 impl ManagedRun {
     pub(super) fn new(
         basics: RunBasics,
         wft: PermittedWFT,
         local_activity_request_sink: Rc<dyn LocalActivityRequestSink>,
     ) -> (Self, RunUpdateAct) {
         let metrics = basics.metrics.clone();
+        let config = basics.worker_config.clone();
         let wfm = WorkflowManager::new(basics);
         let mut me = Self {
             wfm,
             local_activity_request_sink,
             waiting_on_la: None,
             am_broken: false,
             wft: None,
             activation: None,
             task_buffer: Default::default(),
             trying_to_evict: None,
             recorded_span_ids: Default::default(),
             metrics,
             paginator: None,
             completion_waiting_on_page_fetch: None,
+            config,
         };
         let rua = me.incoming_wft(wft);
         (me, rua)
     }
 
     /// Returns true if there are pending jobs that need to be sent to lang.
     pub(super) fn more_pending_work(&self) -> bool {
@@ -336,23 +344,16 @@
                 if has_pending_queries {
                     return Ok(Some(ActivationOrAuto::ReadyForQueries(
                         self.wfm.machines.get_wf_activation(),
                     )));
                 }
             }
             if let Some(wte) = self.trying_to_evict.clone() {
-                let mut act = self.wfm.machines.get_wf_activation();
-                // No other jobs make any sense to send if we encountered an error.
-                if self.am_broken {
-                    act.jobs = vec![];
-                }
-                act.append_evict_job(RemoveFromCache {
-                    message: wte.message,
-                    reason: wte.reason as i32,
-                });
+                let act =
+                    create_evict_activation(self.run_id().to_string(), wte.message, wte.reason);
                 Ok(Some(ActivationOrAuto::LangActivation(act)))
             } else {
                 Ok(None)
             }
         }
     }
 
@@ -364,15 +365,15 @@
     /// the completion can proceed.
     pub(super) fn successful_completion(
         &mut self,
         mut commands: Vec<WFCommand>,
         used_flags: Vec<u32>,
         resp_chan: Option<oneshot::Sender<ActivationCompleteResult>>,
     ) -> Result<RunUpdateAct, NextPageReq> {
-        let activation_was_only_eviction = self.activation_has_only_eviction();
+        let activation_was_only_eviction = self.activation_is_eviction();
         let (task_token, has_pending_query, start_time) = if let Some(entry) = self.wft.as_ref() {
             (
                 entry.info.task_token.clone(),
                 !entry.pending_queries.is_empty(),
                 entry.start_time,
             )
         } else {
@@ -433,23 +434,22 @@
                     } else {
                         Some(x)
                     }
                 })
                 .collect();
 
             if activation_was_only_eviction && !commands.is_empty() {
-                dbg_panic!("Reply to an eviction only containing an eviction included commands");
+                dbg_panic!("Reply to an eviction included commands");
             }
 
             let rac = RunActivationCompletion {
                 task_token,
                 start_time,
                 commands,
-                activation_was_eviction: self.activation_has_eviction(),
-                activation_was_only_eviction,
+                activation_was_eviction: self.activation_is_eviction(),
                 has_pending_query,
                 query_responses,
                 used_flags,
                 resp_chan,
             };
 
             // Verify we can actually apply the next workflow task, which will happen as part of
@@ -530,15 +530,14 @@
                 "No workflow task for run id {} found when trying to fail activation",
                 self.run_id()
             );
             self.reply_to_complete(ActivationCompleteOutcome::DoNothing, resp_chan);
             return None;
         };
 
-        self.metrics.wf_task_failed();
         let message = format!("Workflow activation completion failed: {:?}", &failure);
         // We don't want to fail queries that could otherwise be retried
         let is_no_report_query_fail = self.pending_work_is_legacy_query()
             && is_auto_fail
             && matches!(
                 reason,
                 EvictionReason::Unspecified | EvictionReason::PaginationOrHistoryFetch
@@ -566,20 +565,45 @@
                 ActivationCompleteOutcome::WFTFailedDontReport
             } else {
                 ActivationCompleteOutcome::ReportWFTFail(
                     FailedActivationWFTReport::ReportLegacyQueryFailure(tt, failure),
                 )
             }
         } else if should_report {
-            ActivationCompleteOutcome::ReportWFTFail(FailedActivationWFTReport::Report(
-                tt, cause, failure,
-            ))
+            // Check if we should fail the workflow instead of the WFT because of user's preferences
+            if matches!(cause, WorkflowTaskFailedCause::NonDeterministicError)
+                && self.config.should_fail_workflow(
+                    &self.wfm.machines.workflow_type,
+                    &WorkflowErrorType::Nondeterminism,
+                )
+            {
+                warn!(failure=?failure, "Failing workflow due to nondeterminism error");
+                return self
+                    .successful_completion(
+                        vec![WFCommand::FailWorkflow(FailWorkflowExecution {
+                            failure: failure.failure,
+                        })],
+                        vec![],
+                        resp_chan,
+                    )
+                    .unwrap_or_else(|e| {
+                        dbg_panic!("Got next page request when auto-failing workflow: {e:?}");
+                        None
+                    });
+            } else {
+                ActivationCompleteOutcome::ReportWFTFail(FailedActivationWFTReport::Report(
+                    tt, cause, failure,
+                ))
+            }
         } else {
             ActivationCompleteOutcome::WFTFailedDontReport
         };
+        self.metrics
+            .with_new_attrs([metrics::failure_reason(cause.into())])
+            .wf_task_failed();
         self.reply_to_complete(outcome, resp_chan);
         rur
     }
 
     /// Must be called after the processing of the activation completion and WFT reporting.
     ///
     /// It will delete the currently tracked workflow activation (if there is one) and `pred`
@@ -590,15 +614,16 @@
     /// out-of-date.
     pub(super) fn finish_activation(
         &mut self,
         pred: impl FnOnce(&OutstandingActivation) -> bool,
     ) -> (bool, BufferedTasks) {
         let evict = if self.activation().map(pred).unwrap_or_default() {
             let act = self.activation.take();
-            act.map(|a| a.has_eviction()).unwrap_or_default()
+            act.map(|a| matches!(a, OutstandingActivation::Eviction))
+                .unwrap_or_default()
         } else {
             false
         };
         let buffered = if evict {
             mem::take(&mut self.task_buffer)
         } else {
             Default::default()
@@ -622,22 +647,22 @@
         completion: RunActivationCompletion,
         update_from_new_page: Option<HistoryUpdate>,
     ) -> Result<Option<FulfillableActivationComplete>, RunUpdateErr> {
         let data = CompletionDataForWFT {
             task_token: completion.task_token,
             query_responses: completion.query_responses,
             has_pending_query: completion.has_pending_query,
-            activation_was_only_eviction: completion.activation_was_only_eviction,
+            activation_was_eviction: completion.activation_was_eviction,
         };
 
         self.wfm.machines.add_lang_used_flags(completion.used_flags);
 
-        // If this is just bookkeeping after a reply to an only-eviction activation, we can bypass
+        // If this is just bookkeeping after a reply to an eviction activation, we can bypass
         // everything, since there is no reason to continue trying to update machines.
-        if completion.activation_was_only_eviction {
+        if completion.activation_was_eviction {
             return Ok(Some(self.prepare_complete_resp(
                 completion.resp_chan,
                 data,
                 false,
             )));
         }
 
@@ -760,19 +785,17 @@
     pub(super) fn has_any_pending_work(&self, ignore_evicts: bool, ignore_buffered: bool) -> bool {
         let evict_work = if ignore_evicts {
             false
         } else {
             self.trying_to_evict.is_some()
         };
         let act_work = if ignore_evicts {
-            if let Some(ref act) = self.activation {
-                !act.has_only_eviction()
-            } else {
-                false
-            }
+            self.activation
+                .map(|a| !matches!(a, OutstandingActivation::Eviction))
+                .unwrap_or_default()
         } else {
             self.activation.is_some()
         };
         let buffered = if ignore_buffered {
             false
         } else {
             self.task_buffer.has_tasks()
@@ -821,15 +844,15 @@
                 Failure::application_failure(info.message, false).into(),
                 true,
                 c.resp_chan,
             );
             return EvictionRequestResult::EvictionRequested(attempts, run_upd);
         }
 
-        if !self.activation_has_eviction() && self.trying_to_evict.is_none() {
+        if !self.activation_is_eviction() && self.trying_to_evict.is_none() {
             debug!(run_id=%info.run_id, reason=%info.message, "Eviction requested");
             self.trying_to_evict = Some(info);
             EvictionRequestResult::EvictionRequested(attempts, self.check_more_activations())
         } else {
             // Always store the most recent eviction reason
             self.trying_to_evict = Some(info);
             EvictionRequestResult::EvictionAlreadyRequested(attempts)
@@ -935,19 +958,18 @@
                 let rur = if let Some(resp_chan) = fail.complete_resp_chan {
                     // Automatically fail the workflow task in the event we couldn't update machines
                     let fail_cause = if matches!(&fail.source, WFMachinesError::Nondeterminism(_)) {
                         WorkflowTaskFailedCause::NonDeterministicError
                     } else {
                         WorkflowTaskFailedCause::Unspecified
                     };
-                    let wft_fail_str = format!("{:?}", fail.source);
                     self.failed_completion(
                         fail_cause,
                         fail.source.evict_reason(),
-                        Failure::application_failure(wft_fail_str, false).into(),
+                        fail.source.as_failure(),
                         true,
                         Some(resp_chan),
                     )
                 } else {
                     warn!(error=?fail.source, "Error while updating workflow");
                     Some(ActivationOrAuto::AutoFail {
                         run_id: self.run_id().to_owned(),
@@ -958,21 +980,20 @@
             }
         }
     }
 
     fn insert_outstanding_activation(&mut self, act: &ActivationOrAuto) {
         let act_type = match &act {
             ActivationOrAuto::LangActivation(act) | ActivationOrAuto::ReadyForQueries(act) => {
-                if act.is_legacy_query() {
+                if act.is_only_eviction() {
+                    OutstandingActivation::Eviction
+                } else if act.is_legacy_query() {
                     OutstandingActivation::LegacyQuery
                 } else {
-                    OutstandingActivation::Normal {
-                        contains_eviction: act.eviction_index().is_some(),
-                        num_jobs: act.jobs.len(),
-                    }
+                    OutstandingActivation::Normal
                 }
             }
             ActivationOrAuto::Autocomplete { .. } | ActivationOrAuto::AutoFail { .. } => {
                 OutstandingActivation::Autocomplete
             }
         };
         if let Some(old_act) = self.activation {
@@ -989,15 +1010,15 @@
     fn prepare_complete_resp(
         &mut self,
         resp_chan: Option<oneshot::Sender<ActivationCompleteResult>>,
         data: CompletionDataForWFT,
         due_to_heartbeat_timeout: bool,
     ) -> FulfillableActivationComplete {
         let mut machines_wft_response = self.wfm.prepare_for_wft_response();
-        if data.activation_was_only_eviction
+        if data.activation_was_eviction
             && (machines_wft_response.commands().peek().is_some()
                 || machines_wft_response.has_messages())
             && !self.am_broken
         {
             dbg_panic!(
                 "There should not be any outgoing commands or messages when preparing a completion \
                  response if the activation was only an eviction. This is an SDK bug."
@@ -1013,36 +1034,55 @@
         // activations and we are caught up on replay. We don't want to complete a wft if we already
         // saw the final event in the workflow, or if we are playing back for the express purpose of
         // fulfilling a query. If the activation we sent was *only* an eviction, don't send that
         // either.
         let should_respond = !(machines_wft_response.has_pending_jobs
             || machines_wft_response.replaying
             || is_query_playback
-            || data.activation_was_only_eviction
+            || data.activation_was_eviction
             || machines_wft_response.have_seen_terminal_event);
         // If there are pending LA resolutions, and we're responding to a query here,
         // we want to make sure to force a new task, as otherwise once we tell lang about
         // the LA resolution there wouldn't be any task to reply to with the result of iterating
         // the workflow.
         if has_query_responses && machines_wft_response.have_pending_la_resolutions {
             force_new_wft = true;
         }
 
         let outcome = if should_respond || has_query_responses {
             // If we broke there could be commands or messages in the pipe that we didn't
             // get a chance to handle properly during replay. Don't send them.
-            let (commands, messages) = if self.am_broken && data.activation_was_only_eviction {
+            let (commands, messages) = if self.am_broken && data.activation_was_eviction {
                 (vec![], vec![])
             } else {
                 (
                     machines_wft_response.commands().collect(),
                     machines_wft_response.messages(),
                 )
             };
 
+            // Record metrics for any outgoing terminal commands
+            for cmd in commands.iter() {
+                match cmd.attributes.as_ref() {
+                    Some(CmdAttribs::CompleteWorkflowExecutionCommandAttributes(_)) => {
+                        self.metrics.wf_completed();
+                    }
+                    Some(CmdAttribs::FailWorkflowExecutionCommandAttributes(_)) => {
+                        self.metrics.wf_failed();
+                    }
+                    Some(CmdAttribs::ContinueAsNewWorkflowExecutionCommandAttributes(_)) => {
+                        self.metrics.wf_continued_as_new();
+                    }
+                    Some(CmdAttribs::CancelWorkflowExecutionCommandAttributes(_)) => {
+                        self.metrics.wf_canceled();
+                    }
+                    _ => (),
+                }
+            }
+
             ActivationCompleteOutcome::ReportWFTSuccess(ServerCommandsWithWorkflowInfo {
                 task_token: data.task_token,
                 action: ActivationAction::WftComplete {
                     force_new_wft,
                     commands,
                     messages,
                     query_responses,
@@ -1051,15 +1091,14 @@
             })
         } else {
             ActivationCompleteOutcome::DoNothing
         };
         FulfillableActivationComplete {
             result: ActivationCompleteResult {
                 outcome,
-                most_recently_processed_event: machines_wft_response.last_processed_event as usize,
                 replaying: machines_wft_response.replaying,
             },
             resp_chan,
         }
     }
 
     /// Pump some local activity requests into the sink, applying any immediate results to the
@@ -1081,16 +1120,14 @@
         outcome: ActivationCompleteOutcome,
         chan: Option<oneshot::Sender<ActivationCompleteResult>>,
     ) {
         if let Some(chan) = chan {
             if chan
                 .send(ActivationCompleteResult {
                     outcome,
-                    most_recently_processed_event: self.most_recently_processed_event_number()
-                        as usize,
                     replaying: self.wfm.machines.replaying,
                 })
                 .is_err()
             {
                 let warnstr = "The workflow task completer went missing! This likely indicates an \
                                SDK bug, please report."
                     .to_string();
@@ -1117,23 +1154,17 @@
                 .unwrap_or_default()
     }
 
     fn most_recently_processed_event_number(&self) -> i64 {
         self.wfm.machines.last_processed_event
     }
 
-    fn activation_has_eviction(&mut self) -> bool {
+    fn activation_is_eviction(&mut self) -> bool {
         self.activation
-            .map(OutstandingActivation::has_eviction)
-            .unwrap_or_default()
-    }
-
-    fn activation_has_only_eviction(&mut self) -> bool {
-        self.activation
-            .map(OutstandingActivation::has_only_eviction)
+            .map(|a| matches!(a, OutstandingActivation::Eviction))
             .unwrap_or_default()
     }
 
     fn run_id(&self) -> &str {
         &self.wfm.machines.run_id
     }
 }
@@ -1194,15 +1225,15 @@
     hb_timeout_handle: AbortHandle,
 }
 #[derive(Debug)]
 struct CompletionDataForWFT {
     task_token: TaskToken,
     query_responses: Vec<QueryResult>,
     has_pending_query: bool,
-    activation_was_only_eviction: bool,
+    activation_was_eviction: bool,
 }
 
 /// Manages an instance of a [WorkflowMachines], which is not thread-safe, as well as other data
 /// associated with that specific workflow run.
 struct WorkflowManager {
     machines: WorkflowMachines,
     /// Is always `Some` in normal operation. Optional to allow for unit testing with the test
@@ -1334,15 +1365,14 @@
 
 #[derive(Debug)]
 struct RunActivationCompletion {
     task_token: TaskToken,
     start_time: Instant,
     commands: Vec<WFCommand>,
     activation_was_eviction: bool,
-    activation_was_only_eviction: bool,
     has_pending_query: bool,
     query_responses: Vec<QueryResult>,
     used_flags: Vec<u32>,
     /// Used to notify the worker when the completion is done processing and the completion can
     /// unblock. Must always be `Some` when initialized.
     resp_chan: Option<oneshot::Sender<ActivationCompleteResult>>,
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/mod.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 mod machines;
 mod managed_run;
 mod run_cache;
 mod wft_extraction;
 pub(crate) mod wft_poller;
 mod workflow_stream;
 
-#[cfg(feature = "save_wf_inputs")]
-pub use workflow_stream::replay_wf_state_inputs;
-
 pub(crate) use driven_workflow::DrivenWorkflow;
 pub(crate) use history_update::HistoryUpdate;
 
 use crate::{
     abstractions::{
         dbg_panic, take_cell::TakeCell, MeteredSemaphore, TrackedOwnedMeteredSemPermit,
         UsedMeteredSemPermit,
@@ -127,28 +124,28 @@
     /// Ensures we stay at or below this worker's maximum concurrent workflow task limit
     wft_semaphore: Arc<MeteredSemaphore>,
     local_act_mgr: Arc<LocalActivityManager>,
     ever_polled: AtomicBool,
 }
 
 pub(crate) struct WorkflowBasics {
-    pub worker_config: Arc<WorkerConfig>,
-    pub shutdown_token: CancellationToken,
-    pub metrics: MetricsContext,
-    pub server_capabilities: get_system_info_response::Capabilities,
+    pub(crate) worker_config: Arc<WorkerConfig>,
+    pub(crate) shutdown_token: CancellationToken,
+    pub(crate) metrics: MetricsContext,
+    pub(crate) server_capabilities: get_system_info_response::Capabilities,
 }
 
 pub(crate) struct RunBasics<'a> {
-    pub worker_config: Arc<WorkerConfig>,
-    pub workflow_id: String,
-    pub workflow_type: String,
-    pub run_id: String,
-    pub history: HistoryUpdate,
-    pub metrics: MetricsContext,
-    pub capabilities: &'a get_system_info_response::Capabilities,
+    pub(crate) worker_config: Arc<WorkerConfig>,
+    pub(crate) workflow_id: String,
+    pub(crate) workflow_type: String,
+    pub(crate) run_id: String,
+    pub(crate) history: HistoryUpdate,
+    pub(crate) metrics: MetricsContext,
+    pub(crate) capabilities: &'a get_system_info_response::Capabilities,
 }
 
 impl Workflows {
     #[allow(clippy::too_many_arguments)] // Not much worth combining here
     pub(super) fn new(
         basics: WorkflowBasics,
         sticky_attrs: Option<StickyExecutionAttributes>,
@@ -287,15 +284,15 @@
                 ActivationOrAuto::AutoFail {
                     run_id,
                     machines_err,
                 } => {
                     self.activation_completed(
                         WorkflowActivationCompletion {
                             run_id,
-                            status: Some(auto_fail_to_complete_status(machines_err)),
+                            status: Some(machines_err.as_failure().into()),
                         },
                         true,
                         Option::<Box<dyn Fn(PostActivateHookData) + Send>>::None,
                     )
                     .await?;
                 }
             }
@@ -454,15 +451,14 @@
         } else {
             None
         };
 
         if let Some(h) = post_activate_hook {
             h(PostActivateHookData {
                 run_id: &run_id,
-                most_recent_event: completion_outcome.most_recently_processed_event,
                 replaying: completion_outcome.replaying,
             });
         }
 
         self.post_activation(PostActivationMsg {
             run_id,
             wft_report_status,
@@ -754,152 +750,109 @@
         machines_err: WFMachinesError,
     },
 }
 
 /// A WFT which is considered to be using a slot for metrics purposes and being or about to be
 /// applied to workflow state.
 #[derive(derive_more::DebugCustom)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 #[debug(fmt = "PermittedWft({work:?})")]
 pub(crate) struct PermittedWFT {
     work: PreparedWFT,
-    #[cfg_attr(
-        feature = "save_wf_inputs",
-        serde(skip, default = "UsedMeteredSemPermit::fake_deserialized")
-    )]
     permit: UsedMeteredSemPermit,
-    #[cfg_attr(
-        feature = "save_wf_inputs",
-        serde(skip, default = "HistoryPaginator::fake_deserialized")
-    )]
     paginator: HistoryPaginator,
 }
 /// A WFT without a permit
 #[derive(Debug)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 struct WFTWithPaginator {
     wft: PreparedWFT,
     paginator: HistoryPaginator,
 }
 
 /// A WFT which has been validated and had a history update extracted from it.
 #[derive(Debug)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 struct PreparedWFT {
     task_token: TaskToken,
     attempt: u32,
     execution: WorkflowExecution,
     workflow_type: String,
     legacy_query: Option<WorkflowQuery>,
     query_requests: Vec<QueryWorkflow>,
     update: HistoryUpdate,
     messages: Vec<IncomingProtocolMessage>,
 }
+
 impl PreparedWFT {
     /// Returns true if the contained history update is incremental (IE: expects to hit a cached
     /// workflow)
-    pub fn is_incremental(&self) -> bool {
+    fn is_incremental(&self) -> bool {
         let start_event_id = self.update.first_event_id();
         let poll_resp_is_incremental = start_event_id.map(|eid| eid > 1).unwrap_or_default();
         poll_resp_is_incremental || start_event_id.is_none()
     }
 
     fn is_query_only(&self) -> bool {
         let no_new_history = self.update.wft_started_id == 0;
         no_new_history && self.legacy_query.is_some()
     }
 }
 
 #[derive(Debug)]
-pub(crate) struct OutstandingTask {
-    pub info: WorkflowTaskInfo,
+struct OutstandingTask {
+    info: WorkflowTaskInfo,
     /// Set if the outstanding task has quer(ies) which must be fulfilled upon finishing replay
-    pub pending_queries: Vec<QueryWorkflow>,
-    pub start_time: Instant,
+    pending_queries: Vec<QueryWorkflow>,
+    start_time: Instant,
     /// The WFT permit owned by this task, ensures we don't exceed max concurrent WFT, and makes
     /// sure the permit is automatically freed when we delete the task.
-    pub permit: UsedMeteredSemPermit,
+    permit: UsedMeteredSemPermit,
 }
 
 impl OutstandingTask {
-    pub fn has_pending_legacy_query(&self) -> bool {
+    fn has_pending_legacy_query(&self) -> bool {
         self.pending_queries
             .iter()
             .any(|q| q.query_id == LEGACY_QUERY_ID)
     }
 }
 
 #[derive(Copy, Clone, Debug)]
 pub(crate) enum OutstandingActivation {
     /// A normal activation with a joblist
-    Normal {
-        /// True if there is an eviction in the joblist
-        contains_eviction: bool,
-        /// Number of jobs in the activation
-        num_jobs: usize,
-    },
+    Normal,
+    /// An eviction job
+    Eviction,
     /// An activation for a legacy query
     LegacyQuery,
     /// A fake activation which is never sent to lang, but used internally
     Autocomplete,
 }
 
-impl OutstandingActivation {
-    pub(crate) const fn has_only_eviction(self) -> bool {
-        matches!(
-            self,
-            OutstandingActivation::Normal {
-                contains_eviction: true,
-                num_jobs: nj
-            }
-        if nj == 1)
-    }
-    pub(crate) const fn has_eviction(self) -> bool {
-        matches!(
-            self,
-            OutstandingActivation::Normal {
-                contains_eviction: true,
-                ..
-            }
-        )
-    }
-}
-
 /// Contains important information about a given workflow task that we need to memorize while
 /// lang handles it.
 #[derive(Clone, Debug)]
-pub struct WorkflowTaskInfo {
-    pub task_token: TaskToken,
-    pub attempt: u32,
+struct WorkflowTaskInfo {
+    task_token: TaskToken,
+    attempt: u32,
     /// Exists to allow easy tagging of spans with workflow ids. Is duplicative of info inside the
     /// run machines themselves, but that can't be accessed easily. Would be nice to somehow have a
     /// shared repository, or refcounts, or whatever, for strings like these that get duped all
     /// sorts of places.
-    pub wf_id: String,
+    wf_id: String,
 }
 
 #[derive(Debug)]
-pub enum FailedActivationWFTReport {
+enum FailedActivationWFTReport {
     Report(TaskToken, WorkflowTaskFailedCause, Failure),
     ReportLegacyQueryFailure(TaskToken, Failure),
 }
 
 #[derive(Debug)]
-pub(crate) struct ServerCommandsWithWorkflowInfo {
-    pub task_token: TaskToken,
-    pub action: ActivationAction,
+struct ServerCommandsWithWorkflowInfo {
+    task_token: TaskToken,
+    action: ActivationAction,
 }
 
 #[derive(Debug)]
 pub(crate) enum ActivationAction {
     /// We should respond that the workflow task is complete
     WftComplete {
         commands: Vec<ProtoCommand>,
@@ -927,53 +880,36 @@
         }
     }
 }
 
 #[derive(Debug)]
 #[allow(dead_code)] // Not always used in non-test
 pub(crate) struct WorkflowStateInfo {
-    pub cached_workflows: usize,
-    pub outstanding_wft: usize,
+    pub(crate) cached_workflows: usize,
+    pub(crate) outstanding_wft: usize,
 }
 
 #[derive(Debug)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 struct WFActCompleteMsg {
     completion: ValidatedCompletion,
-    #[cfg_attr(feature = "save_wf_inputs", serde(skip))]
     response_tx: Option<oneshot::Sender<ActivationCompleteResult>>,
 }
 #[derive(Debug)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 struct LocalResolutionMsg {
     run_id: String,
     res: LocalResolution,
 }
 #[derive(Debug)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 struct PostActivationMsg {
     run_id: String,
     wft_report_status: WFTReportStatus,
     wft_from_complete: Option<WFTWithPaginator>,
     is_autocomplete: bool,
 }
 #[derive(Debug, Clone)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 struct RequestEvictMsg {
     run_id: String,
     message: String,
     reason: EvictionReason,
     /// If set, we requested eviction because something went wrong processing a brand new poll task,
     /// which means we won't have stored the WFT and we need to track the task token separately so
     /// we can reply with a failure to server after the evict goes through.
@@ -988,18 +924,18 @@
 struct GetStateInfoMsg {
     response_tx: oneshot::Sender<WorkflowStateInfo>,
 }
 
 /// Each activation completion produces one of these
 #[derive(Debug)]
 struct ActivationCompleteResult {
-    most_recently_processed_event: usize,
     replaying: bool,
     outcome: ActivationCompleteOutcome,
 }
+
 /// What needs to be done after calling [Workflows::activation_completed]
 #[derive(Debug)]
 #[allow(clippy::large_enum_variant)]
 enum ActivationCompleteOutcome {
     /// The WFT must be reported as successful to the server using the contained information.
     ReportWFTSuccess(ServerCommandsWithWorkflowInfo),
     /// The WFT must be reported as failed to the server using the contained information.
@@ -1008,18 +944,14 @@
     DoNothing,
     /// The workflow task failed, but we shouldn't report it. EX: We have failed 2 or more attempts
     /// in a row.
     WFTFailedDontReport,
 }
 /// Did we report, or not, completion of a WFT to server?
 #[derive(Debug, Copy, Clone)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 enum WFTReportStatus {
     Reported {
         reset_last_started_to: Option<i64>,
     },
     /// The WFT completion was not reported when finishing the activation, because there's still
     /// work to be done. EX: Running LAs.
     NotReported,
@@ -1142,18 +1074,14 @@
             reason: "Workflow completion had empty status field".to_owned(),
             run_id: completion.run_id,
         }),
     }
 }
 
 #[derive(Debug)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 #[allow(clippy::large_enum_variant)]
 enum ValidatedCompletion {
     Success {
         run_id: String,
         commands: Vec<WFCommand>,
         used_flags: Vec<u32>,
     },
@@ -1161,53 +1089,45 @@
         run_id: String,
         failure: Failure,
         is_autocomplete: bool,
     },
 }
 
 impl ValidatedCompletion {
-    pub fn run_id(&self) -> &str {
+    fn run_id(&self) -> &str {
         match self {
             ValidatedCompletion::Success { run_id, .. } => run_id,
             ValidatedCompletion::Fail { run_id, .. } => run_id,
         }
     }
 }
 
 #[derive(Debug)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 pub(crate) enum LocalResolution {
     LocalActivity(LocalActivityResolution),
 }
 impl LocalResolution {
-    pub fn is_la_cancel_confirmation(&self) -> bool {
+    fn is_la_cancel_confirmation(&self) -> bool {
         match self {
             LocalResolution::LocalActivity(lar) => {
                 matches!(lar.result, LocalActivityExecutionResult::Cancelled(_))
             }
         }
     }
 }
 
 #[derive(thiserror::Error, Debug, derive_more::From)]
 #[error("Lang provided workflow command with empty variant")]
-pub struct EmptyWorkflowCommandErr;
+struct EmptyWorkflowCommandErr;
 
 /// [DrivenWorkflow]s respond with these when called, to indicate what they want to do next.
 /// EX: Create a new timer, complete the workflow, etc.
 #[derive(Debug, derive_more::From, derive_more::Display)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 #[allow(clippy::large_enum_variant)]
-pub enum WFCommand {
+enum WFCommand {
     /// Returned when we need to wait for the lang sdk to send us something
     NoCommandsFromLang,
     AddActivity(ScheduleActivity),
     AddLocalActivity(ScheduleLocalActivity),
     RequestCancelActivity(RequestCancelActivity),
     RequestCancelLocalActivity(RequestCancelLocalActivity),
     AddTimer(StartTimer),
@@ -1277,15 +1197,15 @@
 
 impl WFCommand {
     /// Returns true if the command is one which ends the workflow:
     /// * Completed
     /// * Failed
     /// * Cancelled
     /// * Continue-as-new
-    pub fn is_terminal(&self) -> bool {
+    fn is_terminal(&self) -> bool {
         matches!(
             self,
             WFCommand::CompleteWorkflow(_)
                 | WFCommand::FailWorkflow(_)
                 | WFCommand::CancelWorkflow(_)
                 | WFCommand::ContinueAsNew(_)
         )
@@ -1301,15 +1221,15 @@
     SignalExternal(u32),
     CancelExternal(u32),
 }
 
 /// Details remembered from the workflow execution started event that we may need to recall later.
 /// Is a subset of `WorkflowExecutionStartedEventAttributes`, but avoids holding on to huge fields.
 #[derive(Debug, Clone)]
-pub struct WorkflowStartedInfo {
+struct WorkflowStartedInfo {
     workflow_task_timeout: Option<Duration>,
     memo: Option<Memo>,
     search_attrs: Option<SearchAttributes>,
     retry_policy: Option<RetryPolicy>,
 }
 
 /// Wraps outgoing activation job protos with some internal details core might care about
@@ -1343,78 +1263,61 @@
     #[error("[TMPRL1100] Nondeterminism error: {0}")]
     Nondeterminism(String),
     #[error("Fatal error in workflow machines: {0}")]
     Fatal(String),
 }
 
 impl WFMachinesError {
-    pub fn evict_reason(&self) -> EvictionReason {
+    fn evict_reason(&self) -> EvictionReason {
         match self {
             WFMachinesError::Nondeterminism(_) => EvictionReason::Nondeterminism,
             WFMachinesError::Fatal(_) => EvictionReason::Fatal,
         }
     }
+
+    fn as_failure(&self) -> Failure {
+        Failure {
+            failure: Some(
+                temporal_sdk_core_protos::temporal::api::failure::v1::Failure::application_failure(
+                    self.to_string(),
+                    false,
+                ),
+            ),
+            force_cause: WorkflowTaskFailedCause::from(self.evict_reason()) as i32,
+        }
+    }
 }
 
 impl From<TimestampError> for WFMachinesError {
     fn from(_: TimestampError) -> Self {
         Self::Fatal("Could not decode timestamp".to_string())
     }
 }
 
 impl From<anyhow::Error> for WFMachinesError {
     fn from(value: anyhow::Error) -> Self {
         WFMachinesError::Fatal(value.to_string())
     }
 }
 
-fn auto_fail_to_complete_status(err: WFMachinesError) -> workflow_activation_completion::Status {
-    workflow_activation_completion::Status::Failed(Failure {
-        failure: Some(
-            temporal_sdk_core_protos::temporal::api::failure::v1::Failure {
-                message: "Error while processing workflow task".to_string(),
-                source: err.to_string(),
-                stack_trace: "".to_string(),
-                encoded_attributes: None,
-                cause: None,
-                failure_info: None,
-            },
-        ),
-        force_cause: WorkflowTaskFailedCause::from(err.evict_reason()) as i32,
-    })
-}
-
 pub(crate) trait LocalActivityRequestSink: Send + Sync + 'static {
     fn sink_reqs(&self, reqs: Vec<LocalActRequest>) -> Vec<LocalActivityResolution>;
 }
 
 #[derive(derive_more::Constructor)]
 pub(super) struct LAReqSink {
     lam: Arc<LocalActivityManager>,
-    /// If we're recording WF inputs, we also need to store immediate resolutions so they're
-    /// available on replay.
-    #[allow(dead_code)] // sometimes appears unused due to feature flagging
-    recorder: Option<UnboundedSender<Vec<u8>>>,
 }
 
 impl LocalActivityRequestSink for LAReqSink {
     fn sink_reqs(&self, reqs: Vec<LocalActRequest>) -> Vec<LocalActivityResolution> {
         if reqs.is_empty() {
             return vec![];
         }
-
-        #[allow(clippy::let_and_return)] // When feature is off clippy doesn't like this
-        let res = self.lam.enqueue(reqs);
-
-        // We always save when there are any reqs, even if the response might be empty, so that
-        // calls/responses are 1:1
-        #[cfg(feature = "save_wf_inputs")]
-        self.write_req(&res);
-
-        res
+        self.lam.enqueue(reqs)
     }
 }
 
 /// Sorts jobs in an activation to be in the order lang expects, and confirms any invariants
 /// activations must uphold.
 ///
 /// ## Ordering
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/run_cache.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/run_cache.rs`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     runs: LruCache<String, ManagedRun>,
     local_activity_request_sink: Rc<dyn LocalActivityRequestSink>,
 
     metrics: MetricsContext,
 }
 
 impl RunCache {
-    pub fn new(
+    pub(super) fn new(
         worker_config: Arc<WorkerConfig>,
         server_capabilities: get_system_info_response::Capabilities,
         local_activity_request_sink: impl LocalActivityRequestSink,
         metrics: MetricsContext,
     ) -> Self {
         // The cache needs room for at least one run, otherwise we couldn't do anything. In
         // "0" size mode, the run is evicted once the workflow task is complete.
@@ -42,15 +42,15 @@
                 NonZeroUsize::new(lru_size).expect("LRU size is guaranteed positive"),
             ),
             local_activity_request_sink: Rc::new(local_activity_request_sink),
             metrics,
         }
     }
 
-    pub fn instantiate_or_update(&mut self, pwft: PermittedWFT) -> RunUpdateAct {
+    pub(super) fn instantiate_or_update(&mut self, pwft: PermittedWFT) -> RunUpdateAct {
         let cur_num_cached_runs = self.runs.len();
         let run_id = pwft.work.execution.run_id.clone();
 
         if let Some(run_handle) = self.runs.get_mut(&run_id) {
             let rur = run_handle.incoming_wft(pwft);
             self.metrics.cache_size(cur_num_cached_runs as u64);
             return rur;
@@ -76,48 +76,57 @@
         );
         if self.runs.push(run_id, mrh).is_some() {
             panic!("Overflowed run cache! Cache owner is expected to avoid this!");
         }
         self.metrics.cache_size(cur_num_cached_runs as u64 + 1);
         rur
     }
-    pub fn remove(&mut self, k: &str) -> Option<ManagedRun> {
+
+    pub(super) fn remove(&mut self, k: &str) -> Option<ManagedRun> {
         let r = self.runs.pop(k);
         self.metrics.cache_size(self.len() as u64);
         self.metrics.cache_eviction();
         r
     }
 
-    pub fn get_mut(&mut self, k: &str) -> Option<&mut ManagedRun> {
+    pub(super) fn get_mut(&mut self, k: &str) -> Option<&mut ManagedRun> {
         self.runs.get_mut(k)
     }
-    pub fn get(&mut self, k: &str) -> Option<&ManagedRun> {
+
+    pub(super) fn get(&mut self, k: &str) -> Option<&ManagedRun> {
         self.runs.get(k)
     }
 
     /// Returns the current least-recently-used run. Returns `None` when cache empty.
-    pub fn current_lru_run(&self) -> Option<&str> {
+    pub(super) fn current_lru_run(&self) -> Option<&str> {
         self.runs.peek_lru().map(|(run_id, _)| run_id.as_str())
     }
+
     /// Returns an iterator yielding cached runs in LRU order
-    pub fn runs_lru_order(&self) -> impl Iterator<Item = (&str, &ManagedRun)> {
+    pub(super) fn runs_lru_order(&self) -> impl Iterator<Item = (&str, &ManagedRun)> {
         self.runs.iter().rev().map(|(k, v)| (k.as_str(), v))
     }
-    pub fn peek(&self, k: &str) -> Option<&ManagedRun> {
+
+    pub(super) fn peek(&self, k: &str) -> Option<&ManagedRun> {
         self.runs.peek(k)
     }
-    pub fn has_run(&self, k: &str) -> bool {
+
+    pub(super) fn has_run(&self, k: &str) -> bool {
         self.runs.contains(k)
     }
-    pub fn handles(&self) -> impl Iterator<Item = &ManagedRun> {
+
+    pub(super) fn handles(&self) -> impl Iterator<Item = &ManagedRun> {
         self.runs.iter().map(|(_, v)| v)
     }
-    pub fn is_full(&self) -> bool {
+
+    pub(super) fn is_full(&self) -> bool {
         self.runs.cap().get() == self.runs.len()
     }
-    pub fn len(&self) -> usize {
+
+    pub(super) fn len(&self) -> usize {
         self.runs.len()
     }
-    pub fn cache_capacity(&self) -> usize {
+
+    pub(super) fn cache_capacity(&self) -> usize {
         self.worker_config.max_cached_workflows
     }
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/wft_extraction.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/wft_extraction.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,19 @@
 
 /// Transforms incoming validated WFTs and history fetching requests into [PermittedWFT]s ready
 /// for application to workflow state
 pub(super) struct WFTExtractor {}
 
 pub(super) enum WFTExtractorOutput {
     NewWFT(PermittedWFT),
-    FetchResult(PermittedWFT, Arc<HistfetchRC>),
+    FetchResult(
+        PermittedWFT,
+        // Field isn't read, but we need to hold on to it.
+        #[allow(dead_code)] Arc<HistfetchRC>,
+    ),
     NextPage {
         paginator: HistoryPaginator,
         update: HistoryUpdate,
         span: Span,
         rc: Arc<HistfetchRC>,
     },
     FailedFetch {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/wft_poller.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/wft_poller.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core/src/worker/workflow/workflow_stream.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core/src/worker/workflow/workflow_stream.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-#[cfg(feature = "save_wf_inputs")]
-mod saved_wf_inputs;
-#[cfg(feature = "save_wf_inputs")]
-mod tonic_status_serde;
-
-#[cfg(feature = "save_wf_inputs")]
-pub use saved_wf_inputs::replay_wf_state_inputs;
-
 use crate::{
     abstractions::dbg_panic,
     worker::workflow::{
         managed_run::RunUpdateAct,
         run_cache::RunCache,
         wft_extraction::{HistfetchRC, HistoryFetchReq, WFTExtractorOutput},
         *,
@@ -37,17 +29,14 @@
     runs_needing_fetching: VecDeque<HistoryFetchReq>,
 
     history_fetch_refcounter: Arc<HistfetchRC>,
     shutdown_token: CancellationToken,
     ignore_evicts_on_shutdown: bool,
 
     metrics: MetricsContext,
-
-    #[cfg(feature = "save_wf_inputs")]
-    wf_state_inputs: Option<UnboundedSender<Vec<u8>>>,
 }
 impl WFStream {
     /// Constructs workflow state management and returns a stream which outputs activations.
     ///
     /// * `wft_stream` is a stream of validated poll responses and fetched history pages as returned
     ///    by a poller (or mock), via [WFTExtractor].
     /// * `local_rx` is a stream of actions that workflow state needs to see. Things like
@@ -101,26 +90,20 @@
                 basics.metrics.clone(),
             ),
             shutdown_token: basics.shutdown_token,
             ignore_evicts_on_shutdown: basics.worker_config.ignore_evicts_on_shutdown,
             metrics: basics.metrics,
             runs_needing_fetching: Default::default(),
             history_fetch_refcounter: Arc::new(HistfetchRC {}),
-
-            #[cfg(feature = "save_wf_inputs")]
-            wf_state_inputs: basics.worker_config.wf_state_inputs.clone(),
         };
         all_inputs
             .map(move |action: WFStreamInput| {
                 let span = span!(Level::DEBUG, "new_stream_input", action=?action);
                 let _span_g = span.enter();
 
-                #[cfg(feature = "save_wf_inputs")]
-                let maybe_write = state.prep_input(&action);
-
                 let mut activations = vec![];
                 let maybe_act = match action {
                     WFStreamInput::NewWft(pwft) => {
                         debug!(run_id=%pwft.work.execution.run_id, "New WFT");
                         state.instantiate_or_update(pwft)
                     }
                     WFStreamInput::Local(local_input) => {
@@ -184,22 +167,14 @@
                         return Err(PollWfError::TonicError(e));
                     }
                 };
 
                 activations.extend(maybe_act);
                 activations.extend(state.reconcile_buffered());
 
-                // Always flush *after* actually handling the input, as this allows LA sink
-                // responses to be recorded before the input, so they can be read and buffered to be
-                // replayed during the handling of the input itself.
-                #[cfg(feature = "save_wf_inputs")]
-                if let Some(write) = maybe_write {
-                    state.flush_write(write);
-                }
-
                 if state.shutdown_done() {
                     info!("Workflow shutdown is done");
                     return Err(PollWfError::ShutDown);
                 }
 
                 Ok(WFStreamOutput {
                     activations: activations.into(),
@@ -567,81 +542,57 @@
             info!(run_id, "Run not found");
         }
     }
 }
 
 /// All possible inputs to the [WFStream]
 #[derive(derive_more::From, Debug)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 enum WFStreamInput {
     NewWft(PermittedWFT),
     Local(LocalInput),
     /// The stream given to us which represents the poller (or a mock) terminated.
     PollerDead,
     /// The stream given to us which represents the poller (or a mock) encountered a non-retryable
     /// error while polling
-    PollerError(
-        #[cfg_attr(
-            feature = "save_wf_inputs",
-            serde(with = "tonic_status_serde::SerdeStatus")
-        )]
-        tonic::Status,
-    ),
+    PollerError(tonic::Status),
     FailedFetch {
         run_id: String,
-        #[cfg_attr(
-            feature = "save_wf_inputs",
-            serde(with = "tonic_status_serde::SerdeStatus")
-        )]
         err: tonic::Status,
         auto_reply_fail_tt: Option<TaskToken>,
     },
 }
 
 /// A non-poller-received input to the [WFStream]
 #[derive(derive_more::DebugCustom)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 #[debug(fmt = "LocalInput {{ {input:?} }}")]
 pub(super) struct LocalInput {
-    pub input: LocalInputs,
-    #[cfg_attr(feature = "save_wf_inputs", serde(skip, default = "Span::current"))]
-    pub span: Span,
+    pub(super) input: LocalInputs,
+    pub(super) span: Span,
 }
 impl From<HeartbeatTimeoutMsg> for LocalInput {
     fn from(hb: HeartbeatTimeoutMsg) -> Self {
         Self {
             input: LocalInputs::HeartbeatTimeout(hb.run_id),
             span: hb.span,
         }
     }
 }
 /// Everything that _isn't_ a poll which may affect workflow state. Always higher priority than
 /// new polls.
 #[derive(Debug, derive_more::From)]
-#[cfg_attr(
-    feature = "save_wf_inputs",
-    derive(serde::Serialize, serde::Deserialize)
-)]
 pub(super) enum LocalInputs {
     Completion(WFActCompleteMsg),
     FetchedPageCompletion {
         paginator: HistoryPaginator,
         update: HistoryUpdate,
     },
     LocalResolution(LocalResolutionMsg),
     PostActivation(PostActivationMsg),
     RequestEviction(RequestEvictMsg),
     HeartbeatTimeout(String),
-    #[cfg_attr(feature = "save_wf_inputs", serde(skip))]
     GetStateInfo(GetStateInfoMsg),
 }
 impl LocalInputs {
     fn run_id(&self) -> Option<&str> {
         Some(match self {
             LocalInputs::Completion(c) => c.completion.run_id(),
             LocalInputs::FetchedPageCompletion { paginator, .. } => &paginator.run_id,
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core-api/src/errors.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core-api/src/errors.rs`

 * *Files 6% similar despite different names*

```diff
@@ -56,7 +56,15 @@
     MalformedActivityCompletion {
         /// Reason the completion was malformed
         reason: String,
         /// The completion, which may not be included to avoid unnecessary copies.
         completion: Option<ActivityExecutionResult>,
     },
 }
+
+/// Errors we can encounter during workflow processing which we may treat as either WFT failures
+/// or whole-workflow failures depending on user preference.
+#[derive(Clone, Debug, Eq, PartialEq, Hash)]
+pub enum WorkflowErrorType {
+    /// A nondeterminism error
+    Nondeterminism,
+}
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core-api/src/lib.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core-api/src/lib.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core-api/src/telemetry/metrics.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core-api/src/telemetry/metrics.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use std::{
     any::Any,
     borrow::Cow,
     fmt::Debug,
     sync::{Arc, OnceLock},
+    time::Duration,
 };
 
 /// Implementors of this trait are expected to be defined in each language's bridge.
 /// The implementor is responsible for the allocation/instantiation of new metric meters which
 /// Core has requested.
 pub trait CoreMeter: Send + Sync + Debug {
     /// Given some k/v pairs, create a return a new instantiated instance of metric attributes.
@@ -19,15 +20,22 @@
     fn extend_attributes(
         &self,
         existing: MetricAttributes,
         attribs: NewAttributes,
     ) -> MetricAttributes;
     fn counter(&self, params: MetricParameters) -> Arc<dyn Counter>;
     fn histogram(&self, params: MetricParameters) -> Arc<dyn Histogram>;
+    fn histogram_f64(&self, params: MetricParameters) -> Arc<dyn HistogramF64>;
+    /// Create a histogram which records Durations. Implementations should choose to emit in
+    /// either milliseconds or seconds depending on how they have been configured.
+    /// [MetricParameters::unit] should be overwritten by implementations to be `ms` or `s`
+    /// accordingly.
+    fn histogram_duration(&self, params: MetricParameters) -> Arc<dyn HistogramDuration>;
     fn gauge(&self, params: MetricParameters) -> Arc<dyn Gauge>;
+    fn gauge_f64(&self, params: MetricParameters) -> Arc<dyn GaugeF64>;
 }
 
 #[derive(Debug, Clone, derive_builder::Builder)]
 pub struct MetricParameters {
     /// The name for the new metric/instrument
     #[builder(setter(into))]
     pub name: Cow<'static, str>,
@@ -70,17 +78,30 @@
 
     fn counter(&self, params: MetricParameters) -> Arc<dyn Counter> {
         self.as_ref().counter(params)
     }
     fn histogram(&self, params: MetricParameters) -> Arc<dyn Histogram> {
         self.as_ref().histogram(params)
     }
+
+    fn histogram_f64(&self, params: MetricParameters) -> Arc<dyn HistogramF64> {
+        self.as_ref().histogram_f64(params)
+    }
+
+    fn histogram_duration(&self, params: MetricParameters) -> Arc<dyn HistogramDuration> {
+        self.as_ref().histogram_duration(params)
+    }
+
     fn gauge(&self, params: MetricParameters) -> Arc<dyn Gauge> {
         self.as_ref().gauge(params)
     }
+
+    fn gauge_f64(&self, params: MetricParameters) -> Arc<dyn GaugeF64> {
+        self.as_ref().gauge_f64(params)
+    }
 }
 
 /// Attributes which are provided every time a call to record a specific metric is made.
 /// Implementors must be very cheap to clone, as these attributes will be re-used frequently.
 #[derive(Clone, Debug)]
 #[non_exhaustive]
 pub enum MetricAttributes {
@@ -154,30 +175,42 @@
     fn add(&self, value: u64, attributes: &MetricAttributes);
 }
 
 pub trait Histogram: Send + Sync {
     // When referring to durations, this value is in millis
     fn record(&self, value: u64, attributes: &MetricAttributes);
 }
+pub trait HistogramF64: Send + Sync {
+    // When referring to durations, this value is in seconds
+    fn record(&self, value: f64, attributes: &MetricAttributes);
+}
+pub trait HistogramDuration: Send + Sync {
+    fn record(&self, value: Duration, attributes: &MetricAttributes);
+}
 
 pub trait Gauge: Send + Sync {
     // When referring to durations, this value is in millis
     fn record(&self, value: u64, attributes: &MetricAttributes);
 }
+pub trait GaugeF64: Send + Sync {
+    // When referring to durations, this value is in seconds
+    fn record(&self, value: f64, attributes: &MetricAttributes);
+}
 
 #[derive(Debug, Clone)]
 pub enum MetricEvent<I: BufferInstrumentRef> {
     Create {
         params: MetricParameters,
-        /// One you receive this event, call `set` on this with the initialized instrument reference
+        /// Once you receive this event, call `set` on this with the initialized instrument
+        /// reference
         populate_into: LazyBufferInstrument<I>,
         kind: MetricKind,
     },
     CreateAttributes {
-        /// One you receive this event, call `set` on this with the initialized attributes
+        /// Once you receive this event, call `set` on this with the initialized attributes
         populate_into: BufferAttributes,
         /// If not `None`, use these already-initialized attributes as the base (extended with
         /// `attributes`) for the ones you are about to initialize.
         append_from: Option<BufferAttributes>,
         attributes: Vec<MetricKeyValue>,
     },
     Update {
@@ -186,22 +219,26 @@
         update: MetricUpdateVal,
     },
 }
 #[derive(Debug, Clone, Copy)]
 pub enum MetricKind {
     Counter,
     Gauge,
+    GaugeF64,
     Histogram,
+    HistogramF64,
+    HistogramDuration,
 }
 #[derive(Debug, Clone, Copy)]
 pub enum MetricUpdateVal {
-    // Currently all deltas are natural numbers
     Delta(u64),
-    // Currently all values are natural numbers
+    DeltaF64(f64),
     Value(u64),
+    ValueF64(f64),
+    Duration(Duration),
 }
 
 pub trait MetricCallBufferer<I: BufferInstrumentRef>: Send + Sync {
     fn retrieve(&self) -> Vec<MetricEvent<I>>;
 }
 
 /// A lazy reference to some metrics buffer attributes
@@ -256,29 +293,50 @@
         Arc::new(NoOpInstrument)
     }
 
     fn histogram(&self, _: MetricParameters) -> Arc<dyn Histogram> {
         Arc::new(NoOpInstrument)
     }
 
+    fn histogram_f64(&self, _: MetricParameters) -> Arc<dyn HistogramF64> {
+        Arc::new(NoOpInstrument)
+    }
+
+    fn histogram_duration(&self, _: MetricParameters) -> Arc<dyn HistogramDuration> {
+        Arc::new(NoOpInstrument)
+    }
+
     fn gauge(&self, _: MetricParameters) -> Arc<dyn Gauge> {
         Arc::new(NoOpInstrument)
     }
+
+    fn gauge_f64(&self, _: MetricParameters) -> Arc<dyn GaugeF64> {
+        Arc::new(NoOpInstrument)
+    }
 }
 
 pub struct NoOpInstrument;
 impl Counter for NoOpInstrument {
     fn add(&self, _: u64, _: &MetricAttributes) {}
 }
 impl Histogram for NoOpInstrument {
     fn record(&self, _: u64, _: &MetricAttributes) {}
 }
+impl HistogramF64 for NoOpInstrument {
+    fn record(&self, _: f64, _: &MetricAttributes) {}
+}
+impl HistogramDuration for NoOpInstrument {
+    fn record(&self, _: Duration, _: &MetricAttributes) {}
+}
 impl Gauge for NoOpInstrument {
     fn record(&self, _: u64, _: &MetricAttributes) {}
 }
+impl GaugeF64 for NoOpInstrument {
+    fn record(&self, _: f64, _: &MetricAttributes) {}
+}
 
 #[derive(Debug, Clone)]
 pub struct NoOpAttributes;
 impl CustomMetricAttributes for NoOpAttributes {
     fn as_any(self: Arc<Self>) -> Arc<dyn Any + Send + Sync> {
         self as Arc<dyn Any + Send + Sync>
     }
@@ -324,11 +382,24 @@
             if let MetricAttributes::OTel { kvs } = attributes {
                 self.record(value, kvs);
             } else {
                 debug_assert!(
                     false,
                     "Must use OTel attributes with an OTel metric implementation"
                 );
+            }
+        }
+    }
+
+    impl HistogramF64 for metrics::Histogram<f64> {
+        fn record(&self, value: f64, attributes: &MetricAttributes) {
+            if let MetricAttributes::OTel { kvs } = attributes {
+                self.record(value, kvs);
+            } else {
+                debug_assert!(
+                    false,
+                    "Must use OTel attributes with an OTel metric implementation"
+                );
             }
         }
     }
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core-api/src/telemetry.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core-api/src/telemetry.rs`

 * *Files 4% similar despite different names*

```diff
@@ -57,17 +57,20 @@
     pub headers: HashMap<String, String>,
     /// Optionally specify how frequently metrics should be exported. Defaults to 1 second.
     #[builder(default = "Duration::from_secs(1)")]
     pub metric_periodicity: Duration,
     /// Specifies the aggregation temporality for metric export. Defaults to cumulative.
     #[builder(default = "MetricTemporality::Cumulative")]
     pub metric_temporality: MetricTemporality,
-    // A map of tags to be applied to all metrics
+    /// A map of tags to be applied to all metrics
     #[builder(default)]
     pub global_tags: HashMap<String, String>,
+    /// If set to true, use f64 seconds for durations instead of u64 milliseconds
+    #[builder(default)]
+    pub use_seconds_for_durations: bool,
 }
 
 /// Options for exporting metrics to Prometheus
 #[derive(Debug, Clone, derive_builder::Builder)]
 pub struct PrometheusExporterOptions {
     pub socket_addr: SocketAddr,
     // A map of tags to be applied to all metrics
@@ -76,14 +79,17 @@
     /// If set true, all counters will include a "_total" suffix
     #[builder(default = "false")]
     pub counters_total_suffix: bool,
     /// If set true, all histograms will include the unit in their name as a suffix.
     /// Ex: "_milliseconds".
     #[builder(default = "false")]
     pub unit_suffix: bool,
+    /// If set to true, use f64 seconds for durations instead of u64 milliseconds
+    #[builder(default)]
+    pub use_seconds_for_durations: bool,
 }
 
 /// Control where logs go
 #[derive(Debug, Clone)]
 pub enum Logger {
     /// Log directly to console.
     Console {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/core-api/src/worker.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/core-api/src/worker.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-use std::time::Duration;
-use tokio::sync::mpsc::UnboundedSender;
+use crate::errors::WorkflowErrorType;
+use std::{
+    collections::{HashMap, HashSet},
+    time::Duration,
+};
 
 const MAX_OUTSTANDING_WFT_DEFAULT: usize = 100;
 const MAX_CONCURRENT_WFT_POLLS_DEFAULT: usize = 5;
 
 /// Defines per-worker configuration options
-#[derive(Debug, Clone, derive_builder::Builder, serde::Serialize, serde::Deserialize)]
+#[derive(Debug, Clone, derive_builder::Builder)]
 #[builder(setter(into), build_fn(validate = "Self::validate"))]
 #[non_exhaustive]
 pub struct WorkerConfig {
     /// The Temporal service namespace this worker is bound to
     pub namespace: String,
     /// What task queue will this worker poll from? This task queue name will be used for both
     /// workflow and activity polling.
@@ -111,44 +114,60 @@
     pub ignore_evicts_on_shutdown: bool,
 
     /// Maximum number of next page (or initial) history event listing requests we'll make
     /// concurrently. I don't this it's worth exposing this to users until we encounter a reason.
     #[builder(default = "5")]
     pub fetching_concurrency: usize,
 
-    // TODO: Move this out - dependency on tokio should not exist just for this
-    /// If set, and the `save_wf_inputs` feature is enabled in core, will be sent a serialized
-    /// instance of every input to workflow state in order. This is for testing purposes, SDK
-    /// implementations never need to care about it.
-    #[builder(default)]
-    #[serde(skip)]
-    pub wf_state_inputs: Option<UnboundedSender<Vec<u8>>>,
-
     /// If set, core will issue cancels for all outstanding activities after shutdown has been
     /// initiated and this amount of time has elapsed.
     #[builder(default)]
     pub graceful_shutdown_period: Option<Duration>,
 
     /// The amount of time core will wait before timing out activities using its own local timers
     /// after one of them elapses. This is to avoid racing with server's own tracking of the
     /// timeout.
     #[builder(default = "Duration::from_secs(5)")]
     pub local_timeout_buffer_for_activities: Duration,
+
+    /// Any error types listed here will cause any workflow being processed by this worker to fail,
+    /// rather than simply failing the workflow task.
+    #[builder(default)]
+    pub workflow_failure_errors: HashSet<WorkflowErrorType>,
+
+    /// Like [WorkerConfig::workflow_failure_errors], but specific to certain workflow types (the
+    /// map key).
+    #[builder(default)]
+    pub workflow_types_to_failure_errors: HashMap<String, HashSet<WorkflowErrorType>>,
 }
 
 impl WorkerConfig {
     pub fn max_nonsticky_polls(&self) -> usize {
         ((self.max_concurrent_wft_polls as f32 * self.nonsticky_to_sticky_poll_ratio) as usize)
             .max(1)
     }
     pub fn max_sticky_polls(&self) -> usize {
         self.max_concurrent_wft_polls
             .saturating_sub(self.max_nonsticky_polls())
             .max(1)
     }
+    /// Returns true if the configuration specifies we should fail a workflow on a certain error
+    /// type rather than failing the workflow task.
+    pub fn should_fail_workflow(
+        &self,
+        workflow_type: &str,
+        error_type: &WorkflowErrorType,
+    ) -> bool {
+        self.workflow_failure_errors.contains(error_type)
+            || self
+                .workflow_types_to_failure_errors
+                .get(workflow_type)
+                .map(|s| s.contains(error_type))
+                .unwrap_or(false)
+    }
 }
 
 impl WorkerConfigBuilder {
     fn validate(&self) -> Result<(), String> {
         if self.max_concurrent_wft_polls == Some(0) {
             return Err("`max_concurrent_wft_polls` must be at least 1".to_owned());
         }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/docker/docker-compose-telem.yaml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/docker/docker-compose-telem.yaml`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/docker/docker-compose.yaml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/docker/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/etc/deps.svg` & `temporalio-1.6.0/temporalio/bridge/sdk-core/etc/deps.svg`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/etc/otel-collector-config.yaml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/etc/otel-collector-config.yaml`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/Cargo.toml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/Cargo.toml`

 * *Files 25% similar despite different names*

```diff
@@ -12,7 +12,10 @@
 
 [dependencies]
 rustfsm_procmacro = { version = "0.1", path = "rustfsm_procmacro" }
 rustfsm_trait = { version = "0.1", path = "rustfsm_trait" }
 
 [package.metadata.workspaces]
 independent = true
+
+[lints]
+workspace = true
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/LICENSE.txt` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/Cargo.toml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/Cargo.toml`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/LICENSE.txt` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/src/lib.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/src/lib.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/dynamic_dest_pass.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/dynamic_dest_pass.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/handler_arg_pass.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/handler_arg_pass.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/handler_pass.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/handler_pass.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/medium_complex_pass.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/medium_complex_pass.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/no_handle_conversions_require_into_fail.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/no_handle_conversions_require_into_fail.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/no_handle_conversions_require_into_fail.stderr` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/no_handle_conversions_require_into_fail.stderr`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 error[E0277]: the trait bound `One: From<Two>` is not satisfied
   --> tests/trybuild/no_handle_conversions_require_into_fail.rs:11:5
    |
 11 |     Two --(B)--> One;
-   |     ^^^ the trait `From<Two>` is not implemented for `One`
+   |     ^^^ the trait `From<Two>` is not implemented for `One`, which is required by `Two: Into<One>`
    |
    = note: required for `Two` to implement `Into<One>`
 note: required by a bound in `TransitionResult::<Sm, Ds>::from`
   --> $WORKSPACE/fsm/rustfsm_trait/src/lib.rs
    |
    |     pub fn from<CurrentState>(current_state: CurrentState) -> Self
    |            ---- required by a bound in this associated function
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/simple_pass.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_procmacro/tests/trybuild/simple_pass.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_trait/LICENSE.txt` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_trait/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/fsm/rustfsm_trait/src/lib.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/fsm/rustfsm_trait/src/lib.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/histories/ends_empty_wft_complete.bin` & `temporalio-1.6.0/temporalio/bridge/sdk-core/histories/ends_empty_wft_complete.bin`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/histories/evict_while_la_running_no_interference-16_history.bin` & `temporalio-1.6.0/temporalio/bridge/sdk-core/histories/evict_while_la_running_no_interference-16_history.bin`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/histories/evict_while_la_running_no_interference-23_history.bin` & `temporalio-1.6.0/temporalio/bridge/sdk-core/histories/evict_while_la_running_no_interference-23_history.bin`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/histories/evict_while_la_running_no_interference-85_history.bin` & `temporalio-1.6.0/temporalio/bridge/sdk-core/histories/evict_while_la_running_no_interference-85_history.bin`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/histories/fail_wf_task.bin` & `temporalio-1.6.0/temporalio/bridge/sdk-core/histories/fail_wf_task.bin`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/histories/old_change_marker_format.bin` & `temporalio-1.6.0/temporalio/bridge/sdk-core/histories/old_change_marker_format.bin`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/histories/timer_workflow_history.bin` & `temporalio-1.6.0/temporalio/bridge/sdk-core/histories/timer_workflow_history.bin`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/Cargo.toml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/test-utils/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 [package]
-name = "temporal-sdk"
-version = "0.1.0-alpha.1"
-edition = "2021"
+name = "temporal-sdk-core-test-utils"
+version = "0.1.0"
 authors = ["Spencer Judge <spencer@temporal.io>"]
+edition = "2021"
 license-file = { workspace = true }
-description = "Temporal Rust SDK"
-homepage = "https://temporal.io/"
-repository = "https://github.com/temporalio/sdk-core"
-keywords = ["temporal", "workflow"]
-categories = ["development-tools"]
 
-# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
+[[bin]]
+name = "histfetch"
+path = "src/histfetch.rs"
+
+[features]
+default = ["ephemeral-server"]
+ephemeral-server = ["temporal-sdk-core/ephemeral-server"]
 
 [dependencies]
-async-trait = "0.1"
-thiserror = "1.0"
 anyhow = "1.0"
+async-trait = "0.1"
 base64 = "0.21"
-crossbeam-channel = "0.5"
-derive_more = { workspace = true }
+bytes = "1.3"
 futures = "0.3"
-once_cell = "1.10"
-parking_lot = { version = "0.12", features = ["send_guard"] }
-prost-types = { version = "0.4", package = "prost-wkt-types" }
-sha2 = "0.10"
-serde = "1.0"
-tokio = { version = "1.26", features = ["rt", "rt-multi-thread", "parking_lot", "time", "fs"] }
+log = "0.4"
+once_cell = { workspace = true }
+parking_lot = "0.12"
+prost = { workspace = true }
+prost-types = { workspace = true }
+rand = "0.8"
+rmp-serde = "1.1"
+serde_json = "1.0"
+temporal-client = { path = "../client" }
+temporal-sdk = { path = "../sdk" }
+temporal-sdk-core = { path = "../core" }
+temporal-sdk-core-api = { path = "../core-api" }
+thiserror = "1.0"
+tokio = "1.1"
 tokio-util = { version = "0.7" }
-tokio-stream = "0.1"
-tonic = { workspace = true }
 tracing = "0.1"
-
-[dependencies.temporal-sdk-core]
-path = "../core"
-version = "0.1"
+url = "2.2"
+uuid = "1.1"
 
 [dependencies.temporal-sdk-core-protos]
 path = "../sdk-core-protos"
 version = "0.1"
 
-[dependencies.temporal-sdk-core-api]
-path = "../core-api"
-version = "0.1"
-
-[dependencies.temporal-client]
-path = "../client"
-version = "0.1"
+[lints]
+workspace = true
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/activity_context.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/activity_context.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/app_data.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/app_data.rs`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,28 @@
     any::{Any, TypeId},
     collections::HashMap,
     fmt,
 };
 
 /// A Wrapper Type for workflow and activity app data
 #[derive(Default)]
-pub struct AppData {
+pub(crate) struct AppData {
     map: HashMap<TypeId, Box<dyn Any + Send + Sync>>,
 }
 
 impl AppData {
     /// Insert an item, overwritting duplicates
-    pub fn insert<T: Send + Sync + 'static>(&mut self, val: T) -> Option<T> {
+    pub(crate) fn insert<T: Send + Sync + 'static>(&mut self, val: T) -> Option<T> {
         self.map
             .insert(TypeId::of::<T>(), Box::new(val))
             .and_then(downcast_owned)
     }
 
     /// Get a reference to a type in the map
-    pub fn get<T: 'static>(&self) -> Option<&T> {
+    pub(crate) fn get<T: 'static>(&self) -> Option<&T> {
         self.map
             .get(&TypeId::of::<T>())
             .and_then(|boxed| boxed.downcast_ref())
     }
 }
 
 impl fmt::Debug for AppData {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/interceptors.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/interceptors.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/lib.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 //! use temporal_sdk_core::{init_worker, Url, CoreRuntime};
 //! use temporal_sdk_core_api::{worker::WorkerConfigBuilder, telemetry::TelemetryOptionsBuilder};
 //!
 //! #[tokio::main]
 //! async fn main() -> Result<(), Box<dyn std::error::Error>> {
 //!     let server_options = sdk_client_options(Url::from_str("http://localhost:7233")?).build()?;
 //!
-//!     let client = server_options.connect("default", None, None).await?;
+//!     let client = server_options.connect("default", None).await?;
 //!
 //!     let telemetry_options = TelemetryOptionsBuilder::default().build()?;
 //!     let runtime = CoreRuntime::new_assume_tokio(telemetry_options)?;
 //!
 //!     let worker_config = WorkerConfigBuilder::default()
 //!         .namespace("default")
 //!         .task_queue("task_queue")
@@ -44,15 +44,14 @@
 
 #[macro_use]
 extern crate tracing;
 
 mod activity_context;
 mod app_data;
 pub mod interceptors;
-mod payload_converter;
 mod workflow_context;
 mod workflow_future;
 
 pub use activity_context::ActContext;
 pub use temporal_client::Namespace;
 pub use workflow_context::{
     ActivityOptions, CancellableFuture, ChildWorkflow, ChildWorkflowOptions, LocalActivityOptions,
@@ -517,15 +516,18 @@
                             result: Some(result),
                         })
                         .await?;
                     Ok::<_, anyhow::Error>(())
                 });
             }
             Some(activity_task::Variant::Cancel(_)) => {
-                if let Some(ct) = self.task_tokens_to_cancels.get(&activity.task_token.into()) {
+                if let Some(ct) = self
+                    .task_tokens_to_cancels
+                    .get(activity.task_token.as_slice())
+                {
                     ct.cancel();
                 }
             }
             None => bail!("Undefined activity task variant"),
         }
         Ok(())
     }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/workflow_context/options.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/workflow_context/options.rs`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         common::v1::{Payload, RetryPolicy},
         enums::v1::ParentClosePolicy,
     },
 };
 
 // TODO: Before release, probably best to avoid using proto types entirely here. They're awkward.
 
-pub trait IntoWorkflowCommand {
+pub(crate) trait IntoWorkflowCommand {
     type WFCommandType;
 
     /// Produces a workflow command from some options
     fn into_command(self, seq: u32) -> Self::WFCommandType;
 }
 
 /// Options for scheduling an activity
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/workflow_context.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/workflow_context.rs`

 * *Files 1% similar despite different names*

```diff
@@ -94,19 +94,19 @@
         seq
     }
 }
 
 #[derive(Clone, Debug, Default)]
 pub(crate) struct WfContextSharedData {
     /// Maps change ids -> resolved status
-    pub changes: HashMap<String, bool>,
-    pub is_replaying: bool,
-    pub wf_time: Option<SystemTime>,
-    pub history_length: u32,
-    pub current_build_id: Option<String>,
+    pub(crate) changes: HashMap<String, bool>,
+    pub(crate) is_replaying: bool,
+    pub(crate) wf_time: Option<SystemTime>,
+    pub(crate) history_length: u32,
+    pub(crate) current_build_id: Option<String>,
 }
 
 // TODO: Dataconverter type interface to replace Payloads here. Possibly just use serde
 //    traits.
 impl WfContext {
     /// Create a new wf context, returning the context itself and a receiver which outputs commands
     /// sent from the workflow.
@@ -200,15 +200,15 @@
 
     /// Request to run an activity
     pub fn activity(
         &self,
         mut opts: ActivityOptions,
     ) -> impl CancellableFuture<ActivityResolution> {
         if opts.task_queue.is_empty() {
-            opts.task_queue = self.task_queue.clone()
+            opts.task_queue.clone_from(&self.task_queue);
         }
         let seq = self.seq_nums.write().next_activity_seq();
         let (cmd, unblocker) = CancellableWFCommandFut::new(CancellableID::Activity(seq));
         self.send(
             CommandCreateRequest {
                 cmd: opts.into_command(seq).into(),
                 unblocker,
@@ -569,15 +569,16 @@
             return match tf.poll_unpin(cx) {
                 Poll::Ready(tr) => {
                     self.timer_fut = None;
                     // Schedule next LA if this timer wasn't cancelled
                     if let TimerResult::Fired = tr {
                         let mut opts = self.la_opts.clone();
                         opts.attempt = Some(self.next_attempt);
-                        opts.original_schedule_time = self.next_sched_time.clone();
+                        opts.original_schedule_time
+                            .clone_from(&self.next_sched_time);
                         self.current_fut = Box::pin(self.ctx.local_activity_no_timer_retry(opts));
                         Poll::Pending
                     } else {
                         Poll::Ready(ActivityResolution {
                             status: Some(
                                 activity_resolution::Status::Cancelled(Default::default()),
                             ),
@@ -604,15 +605,15 @@
                         .clone()
                         .expect("Duration is set")
                         .try_into()
                         .expect("duration converts ok"),
                 );
                 self.timer_fut = Some(Box::pin(timer_f));
                 self.next_attempt = b.attempt;
-                self.next_sched_time = b.original_schedule_time.clone();
+                self.next_sched_time.clone_from(&b.original_schedule_time);
                 return Poll::Pending;
             }
         }
         poll_res
     }
 }
 impl<'a> CancellableFuture<ActivityResolution> for LATimerBackoffFut<'a> {
@@ -627,15 +628,15 @@
 
 /// A stub representing an unstarted child workflow.
 #[derive(Default, Debug, Clone)]
 pub struct ChildWorkflow {
     opts: ChildWorkflowOptions,
 }
 
-pub struct ChildWfCommon {
+pub(crate) struct ChildWfCommon {
     workflow_id: String,
     result_future: CancellableWFCommandFut<ChildWorkflowResult, ()>,
 }
 
 /// Child workflow in pending state
 pub struct PendingChildWorkflow {
     /// The status of the child workflow start
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk/src/workflow_future.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk/src/workflow_future.rs`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 //   production-ready SDK design, or if desired to allow dynamic signal registration, prevent this
 //   from growing unbounded if being sent lots of unhandled signals.
 enum SigChanOrBuffer {
     Chan(UnboundedSender<SignalData>),
     Buffer(Vec<SignalData>),
 }
 
-pub struct WorkflowFuture {
+pub(crate) struct WorkflowFuture {
     /// Future produced by calling the workflow function
     inner: BoxFuture<'static, WorkflowResult<Payload>>,
     /// Commands produced inside user's wf code
     incoming_commands: Receiver<RustWfCmd>,
     /// Once blocked or the workflow has finished or errored out, the result is sent here
     outgoing_completions: UnboundedSender<WorkflowActivationCompletion>,
     /// Activations from core
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/Cargo.toml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 homepage = "https://temporal.io/"
 repository = "https://github.com/temporalio/sdk-core"
 keywords = ["temporal", "workflow"]
 categories = ["development-tools"]
 
 [features]
 history_builders = ["uuid", "rand"]
-serde_serialize = []
 
 [dependencies]
 anyhow = "1.0"
 base64 = "0.21"
 derive_more = { workspace = true }
-prost = "0.11"
-prost-wkt = "0.4"
-prost-wkt-types = "0.4"
+prost = { workspace = true }
+prost-wkt = "0.5"
+prost-wkt-types = "0.5"
 rand = { version = "0.8", optional = true }
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
 thiserror = "1.0"
 tonic = { workspace = true }
 uuid = { version = "1.1", features = ["v4"], optional = true }
 
 [build-dependencies]
 tonic-build = { workspace = true }
-prost-wkt-build = "0.4"
+prost-wkt-build = "0.5"
+
+[lints]
+workspace = true
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/build.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/build.rs`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             ".google.protobuf.Duration",
             "::prost_wkt_types::Duration"
         )
         .extern_path(
             ".google.protobuf.Value",
             "::prost_wkt_types::Value"
         )
-        .file_descriptor_set_path(#[allow(clippy::needless_borrow)] &descriptor_file)
+        .file_descriptor_set_path(descriptor_file)
         .compile(
             &[
                 "./protos/local/temporal/sdk/core/core_interface.proto",
                 "./protos/api_upstream/temporal/api/workflowservice/v1/service.proto",
                 "./protos/api_upstream/temporal/api/operatorservice/v1/service.proto",
                 "./protos/testsrv_upstream/temporal/api/testservice/v1/service.proto",
                 "./protos/grpc/health/v1/health.proto",
@@ -125,18 +125,9 @@
                 "./protos/api_upstream",
                 "./protos/local",
                 "./protos/testsrv_upstream",
                 "./protos/grpc",
             ],
         )?;
 
-    #[cfg(feature = "serde_serialize")]
-    {
-        use prost_wkt_build::{FileDescriptorSet, Message};
-
-        let descriptor_bytes = std::fs::read(descriptor_file)?;
-        let descriptor = FileDescriptorSet::decode(&descriptor_bytes[..])?;
-        prost_wkt_build::add_serde(out, descriptor);
-    }
-
     Ok(())
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.github/workflows/publish-docs.yml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.github/workflows/publish-docs.yml`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.github/workflows/trigger-api-go-update.yml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/.github/workflows/trigger-api-go-update.yml`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/LICENSE` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/LICENSE`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/Makefile` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/Makefile`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/api-linter.yaml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/api-linter.yaml`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/api/annotations.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/api/http.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/any.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/descriptor.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/duration.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/duration.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/empty.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/empty.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/timestamp.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/timestamp.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/wrappers.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/google/protobuf/wrappers.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/batch/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/batch/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/command/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/command/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/common/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/common/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/batch_operation.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/batch_operation.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/command_type.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/command_type.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/common.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/common.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/event_type.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/event_type.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/failed_cause.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/failed_cause.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/namespace.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/namespace.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/query.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/query.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/reset.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/reset.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/schedule.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/schedule.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/task_queue.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/task_queue.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/update.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/update.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/workflow.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/enums/v1/workflow.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/errordetails/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/errordetails/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/export/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/export/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/failure/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/failure/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/filter/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/filter/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/history/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/history/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/namespace/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/namespace/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/operatorservice/v1/request_response.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/operatorservice/v1/request_response.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/operatorservice/v1/service.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/operatorservice/v1/service.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/protocol/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/protocol/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/query/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/query/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/replication/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/replication/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/schedule/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/schedule/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/sdk/v1/task_complete_metadata.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/sdk/v1/task_complete_metadata.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/sdk/v1/workflow_metadata.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/sdk/v1/workflow_metadata.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/taskqueue/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/taskqueue/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/update/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/update/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/version/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/version/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/workflow/v1/message.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/workflow/v1/message.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/workflowservice/v1/request_response.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/workflowservice/v1/request_response.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/workflowservice/v1/service.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/api_upstream/temporal/api/workflowservice/v1/service.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/google/rpc/status.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/grpc/health/v1/health.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/grpc/health/v1/health.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/activity_result/activity_result.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/activity_result/activity_result.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/activity_task/activity_task.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/activity_task/activity_task.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/child_workflow/child_workflow.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/child_workflow/child_workflow.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/common/common.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/common/common.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/core_interface.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/core_interface.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/external_data/external_data.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/external_data/external_data.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/workflow_activation/workflow_activation.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/workflow_activation/workflow_activation.proto`

 * *Files 4% similar despite different names*

```diff
@@ -26,30 +26,29 @@
 // `patches -> signals/updates -> other -> queries -> evictions`
 //
 // This is because:
 // * Patches are expected to apply to the entire activation
 // * Signal and update handlers should be invoked before workflow routines are iterated. That is to
 //   say before the users' main workflow function and anything spawned by it is allowed to continue.
 // * Queries always go last (and, in fact, always come in their own activation)
+// * Evictions also always come in their own activation
 //
 // The downside of this reordering is that a signal or update handler may not observe that some
 // other event had already happened (ex: an activity completed) when it is first invoked, though it
 // will subsequently when workflow routines are driven. Core only does this reordering to make life
 // easier for languages that cannot explicitly control when workflow routines are iterated.
 // Languages that can explicitly control such iteration should prefer to apply all the jobs to state
 // (by resolving promises/futures, invoking handlers, etc as they iterate over the jobs) and then
 // only *after* that is done, drive the workflow routines.
 //
 // ## Evictions
 //
-// Activations that contain only a `remove_from_cache` job should not cause the workflow code
-// to be invoked and may be responded to with an empty command list. Eviction jobs may also
-// appear with other jobs, but will always appear last in the job list. In this case it is
-// expected that the workflow code will be invoked, and the response produced as normal, but
-// the caller should evict the run after doing so.
+// Evictions appear as an activations that contains only a `remove_from_cache` job. Such activations
+// should not cause the workflow code to be invoked and may be responded to with an empty command
+// list.
 message WorkflowActivation {
     // The id of the currently active run of the workflow. Also used as a cache key. There may
     // only ever be one active workflow task (and hence activation) of a run at one time.
     string run_id = 1;
     // The current time as understood by the workflow, which is set by workflow task started events
     google.protobuf.Timestamp timestamp = 2;
     // Whether or not the activation is replaying past events
@@ -77,15 +76,16 @@
     oneof variant {
         // Begin a workflow for the first time
         StartWorkflow start_workflow = 1;
         // A timer has fired, allowing whatever was waiting on it (if anything) to proceed
         FireTimer fire_timer = 2;
         // Workflow was reset. The randomness seed must be updated.
         UpdateRandomSeed update_random_seed = 4;
-        // A request to query the workflow was received.
+        // A request to query the workflow was received. It is guaranteed that queries (one or more)
+        // always come in their own activation after other mutating jobs.
         QueryWorkflow query_workflow = 5;
         // A request to cancel the workflow was received.
         CancelWorkflow cancel_workflow = 6;
         // A request to signal the workflow was received.
         SignalWorkflow signal_workflow = 7;
         // An activity was resolved, result could be completed, failed or cancelled
         ResolveActivity resolve_activity = 8;
@@ -99,19 +99,17 @@
         ResolveChildWorkflowExecution resolve_child_workflow_execution = 11;
         // An attempt to signal an external workflow resolved
         ResolveSignalExternalWorkflow resolve_signal_external_workflow = 12;
         // An attempt to cancel an external workflow resolved
         ResolveRequestCancelExternalWorkflow resolve_request_cancel_external_workflow = 13;
         // A request to handle a workflow update.
         DoUpdate do_update = 14;
-        // Remove the workflow identified by the [WorkflowActivation] containing this job from the cache
-        // after performing the activation.
-        //
-        // If other job variant are present in the list, this variant will be the last job in the
-        // job list. The string value is a reason for eviction.
+        // Remove the workflow identified by the [WorkflowActivation] containing this job from the
+        // cache after performing the activation. It is guaranteed that this will be the only job
+        // in the activation if present.
         RemoveFromCache remove_from_cache = 50;
     }
 }
 
 // Start a new workflow
 message StartWorkflow {
     // The identifier the lang-specific sdk uses to execute workflow code
@@ -204,15 +202,15 @@
     string workflow_type = 2;
     child_workflow.StartChildWorkflowExecutionFailedCause cause = 3;
 }
 
 // `failure` should be ChildWorkflowFailure with cause set to CancelledFailure.
 // The failure is constructed in core for lang's convenience.
 message ResolveChildWorkflowExecutionStartCancelled {
-  temporal.api.failure.v1.Failure failure = 1;
+    temporal.api.failure.v1.Failure failure = 1;
 }
 
 // Notify a workflow that a child workflow execution has been resolved
 message ResolveChildWorkflowExecution {
     // Sequence number as provided by lang in the corresponding StartChildWorkflowExecution command
     uint32 seq = 1;
     child_workflow.ChildWorkflowResult result = 2;
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/workflow_commands/workflow_commands.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/workflow_commands/workflow_commands.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/workflow_completion/workflow_completion.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/local/temporal/sdk/core/workflow_completion/workflow_completion.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/Makefile` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/Makefile`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/api-linter.yaml` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/api-linter.yaml`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/temporal/api/testservice/v1/request_response.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/temporal/api/testservice/v1/request_response.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/temporal/api/testservice/v1/service.proto` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/protos/testsrv_upstream/temporal/api/testservice/v1/service.proto`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/src/history_builder.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/src/history_builder.rs`

 * *Files 0% similar despite different names*

```diff
@@ -594,15 +594,15 @@
         if let Some(Attributes::WorkflowExecutionStartedEventAttributes(
             WorkflowExecutionStartedEventAttributes {
                 original_execution_run_id,
                 ..
             },
         )) = &evt.attributes
         {
-            self.original_run_id = original_execution_run_id.clone();
+            self.original_run_id.clone_from(original_execution_run_id);
         };
         self.events.push(evt);
         self.current_event_id
     }
 }
 
 fn default_attribs(et: EventType) -> Result<Attributes> {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/src/history_info.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/src/history_info.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/src/lib.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -360,31 +360,36 @@
 
         // Buncha hullaballoo because prost types aren't serde compat.
         // See https://github.com/tokio-rs/prost/issues/75 which hilariously Chad opened ages ago
 
         #[derive(Serialize, Deserialize)]
         #[serde(remote = "Timestamp")]
         struct TimestampDef {
-            pub seconds: i64,
-            pub nanos: i32,
+            seconds: i64,
+            nanos: i32,
         }
         mod opt_timestamp {
             use super::*;
 
-            pub fn serialize<S>(value: &Option<Timestamp>, serializer: S) -> Result<S::Ok, S::Error>
+            pub(super) fn serialize<S>(
+                value: &Option<Timestamp>,
+                serializer: S,
+            ) -> Result<S::Ok, S::Error>
             where
                 S: Serializer,
             {
                 #[derive(Serialize)]
                 struct Helper<'a>(#[serde(with = "TimestampDef")] &'a Timestamp);
 
                 value.as_ref().map(Helper).serialize(serializer)
             }
 
-            pub fn deserialize<'de, D>(deserializer: D) -> Result<Option<Timestamp>, D::Error>
+            pub(super) fn deserialize<'de, D>(
+                deserializer: D,
+            ) -> Result<Option<Timestamp>, D::Error>
             where
                 D: Deserializer<'de>,
             {
                 #[derive(Deserialize)]
                 struct Helper(#[serde(with = "TimestampDef")] Timestamp);
 
                 let helper = Option::deserialize(deserializer)?;
@@ -392,31 +397,34 @@
             }
         }
 
         // Luckily Duration is also stored the exact same way
         #[derive(Serialize, Deserialize)]
         #[serde(remote = "Duration")]
         struct DurationDef {
-            pub seconds: i64,
-            pub nanos: i32,
+            seconds: i64,
+            nanos: i32,
         }
         mod opt_duration {
             use super::*;
 
-            pub fn serialize<S>(value: &Option<Duration>, serializer: S) -> Result<S::Ok, S::Error>
+            pub(super) fn serialize<S>(
+                value: &Option<Duration>,
+                serializer: S,
+            ) -> Result<S::Ok, S::Error>
             where
                 S: Serializer,
             {
                 #[derive(Serialize)]
                 struct Helper<'a>(#[serde(with = "DurationDef")] &'a Duration);
 
                 value.as_ref().map(Helper).serialize(serializer)
             }
 
-            pub fn deserialize<'de, D>(deserializer: D) -> Result<Option<Duration>, D::Error>
+            pub(super) fn deserialize<'de, D>(deserializer: D) -> Result<Option<Duration>, D::Error>
             where
                 D: Deserializer<'de>,
             {
                 #[derive(Deserialize)]
                 struct Helper(#[serde(with = "DurationDef")] Duration);
 
                 let helper = Option::deserialize(deserializer)?;
@@ -479,60 +487,36 @@
                 query_type: q.query_type,
                 arguments: Vec::from_payloads(q.query_args),
                 headers: q.header.map(|h| h.into()).unwrap_or_default(),
             }
         }
 
         impl WorkflowActivation {
-            /// Returns the index of the eviction job if this activation contains one. If present
-            /// it should always be the last job in the list.
-            pub fn eviction_index(&self) -> Option<usize> {
-                self.jobs.iter().position(|j| {
-                    matches!(
-                        j,
-                        WorkflowActivationJob {
-                            variant: Some(workflow_activation_job::Variant::RemoveFromCache(_))
-                        }
-                    )
-                })
-            }
-
-            /// Returns true if the only job is eviction
+            /// Returns true if the only job in the activation is eviction
             pub fn is_only_eviction(&self) -> bool {
-                self.jobs.len() == 1 && self.eviction_index().is_some()
+                matches!(
+                    self.jobs.as_slice(),
+                    [WorkflowActivationJob {
+                        variant: Some(workflow_activation_job::Variant::RemoveFromCache(_))
+                    }]
+                )
             }
 
-            /// Returns eviction reason if this activation has an evict job
+            /// Returns eviction reason if this activation is an eviction
             pub fn eviction_reason(&self) -> Option<EvictionReason> {
                 self.jobs.iter().find_map(|j| {
                     if let Some(workflow_activation_job::Variant::RemoveFromCache(ref rj)) =
                         j.variant
                     {
-                        EvictionReason::from_i32(rj.reason)
+                        EvictionReason::try_from(rj.reason).ok()
                     } else {
                         None
                     }
                 })
             }
-
-            /// Append an eviction job to the joblist
-            pub fn append_evict_job(&mut self, evict_job: RemoveFromCache) {
-                if let Some(last_job) = self.jobs.last() {
-                    if matches!(
-                        last_job.variant,
-                        Some(workflow_activation_job::Variant::RemoveFromCache(_))
-                    ) {
-                        return;
-                    }
-                }
-                let evict_job = WorkflowActivationJob::from(
-                    workflow_activation_job::Variant::RemoveFromCache(evict_job),
-                );
-                self.jobs.push(evict_job);
-            }
         }
 
         impl Display for EvictionReason {
             fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
                 write!(f, "{self:?}")
             }
         }
@@ -1490,15 +1474,15 @@
                             _ => unimplemented!(),
                         }
                     }
                 }
 
                 impl Display for Command {
                     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
-                        let ct = CommandType::from_i32(self.command_type)
+                        let ct = CommandType::try_from(self.command_type)
                             .unwrap_or(CommandType::Unspecified);
                         write!(f, "{:?}", ct)
                     }
                 }
 
                 impl From<workflow_commands::StartTimer> for command::Attributes {
                     fn from(s: workflow_commands::StartTimer) -> Self {
@@ -1826,15 +1810,15 @@
                         bail!("First event is not WorkflowExecutionStarted?!?")
                     }
                 }
 
                 impl HistoryEvent {
                     /// Returns true if this is an event created to mirror a command
                     pub fn is_command_event(&self) -> bool {
-                        EventType::from_i32(self.event_type).map_or(false, |et| match et {
+                        EventType::try_from(self.event_type).map_or(false, |et| match et {
                             EventType::ActivityTaskScheduled
                             | EventType::ActivityTaskCancelRequested
                             | EventType::MarkerRecorded
                             | EventType::RequestCancelExternalWorkflowExecutionInitiated
                             | EventType::SignalExternalWorkflowExecutionInitiated
                             | EventType::StartChildWorkflowExecutionInitiated
                             | EventType::TimerCanceled
@@ -1925,15 +1909,15 @@
 
                 impl Display for HistoryEvent {
                     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
                         write!(
                             f,
                             "HistoryEvent(id: {}, {:?})",
                             self.event_id,
-                            EventType::from_i32(self.event_type)
+                            EventType::try_from(self.event_type)
                         )
                     }
                 }
 
                 impl Attributes {
                     pub fn event_type(&self) -> EventType {
                         // I just absolutely _love_ this
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/src/task_token.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/src/task_token.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 use base64::{prelude::BASE64_STANDARD, Engine};
-use std::fmt::{Debug, Display, Formatter};
+use std::{
+    borrow::Borrow,
+    fmt::{Debug, Display, Formatter},
+};
 
 static LOCAL_ACT_TASK_TOKEN_PREFIX: &[u8] = b"local_act_";
 
 #[derive(
     Hash,
     Eq,
     PartialEq,
@@ -39,10 +42,16 @@
 
 impl Debug for TaskToken {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         f.write_str(&format!("TaskToken({})", fmt_tt(&self.0)))
     }
 }
 
-pub fn fmt_tt(tt: &[u8]) -> String {
+impl Borrow<[u8]> for TaskToken {
+    fn borrow(&self) -> &[u8] {
+        self.0.as_slice()
+    }
+}
+
+pub(crate) fn fmt_tt(tt: &[u8]) -> String {
     BASE64_STANDARD.encode(tt)
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/sdk-core-protos/src/utilities.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/sdk-core-protos/src/utilities.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/test-utils/src/canned_histories.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/test-utils/src/canned_histories.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/test-utils/src/histfetch.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/test-utils/src/histfetch.rs`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 use prost::Message;
 use temporal_client::WorkflowClientTrait;
 use temporal_sdk_core_test_utils::get_integ_server_options;
 
 #[tokio::main]
 async fn main() -> Result<(), anyhow::Error> {
     let gw_opts = get_integ_server_options();
-    let client = gw_opts.connect("default", None, None).await?;
+    let client = gw_opts.connect("default", None).await?;
     let wf_id = std::env::args()
         .nth(1)
         .expect("must provide workflow id as only argument");
     let run_id = std::env::args().nth(2);
     let hist = client
         .get_workflow_execution_history(wf_id.clone(), run_id, vec![])
         .await?
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/test-utils/src/interceptors.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/test-utils/src/interceptors.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/test-utils/src/lib.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/test-utils/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,20 @@
 //! or even when testing workflows written in SDKs that use Core.
 
 #[macro_use]
 extern crate tracing;
 
 pub mod canned_histories;
 pub mod interceptors;
-pub mod wf_input_saver;
 pub mod workflows;
 
-use anyhow::Context;
 pub use temporal_sdk_core::replay::HistoryForReplay;
 
-use crate::{
-    stream::{Stream, TryStreamExt},
-    wf_input_saver::stream_to_file,
-};
+use crate::stream::{Stream, TryStreamExt};
+use anyhow::{Context, Error};
 use base64::{prelude::BASE64_STANDARD, Engine};
 use futures::{future, stream, stream::FuturesUnordered, StreamExt};
 use parking_lot::Mutex;
 use prost::Message;
 use rand::{distributions::Standard, Rng};
 use std::{
     convert::TryFrom, env, future::Future, net::SocketAddr, path::PathBuf, sync::Arc,
@@ -47,27 +43,28 @@
         metrics::CoreMeter, Logger, OtelCollectorOptionsBuilder, PrometheusExporterOptionsBuilder,
         TelemetryOptions, TelemetryOptionsBuilder,
     },
     Worker as CoreWorker,
 };
 use temporal_sdk_core_protos::{
     coresdk::{
+        workflow_activation::WorkflowActivation,
         workflow_commands::{
             workflow_command, ActivityCancellationType, CompleteWorkflowExecution, QueryResult,
             QuerySuccess, ScheduleActivity, ScheduleLocalActivity, StartTimer,
         },
         workflow_completion::WorkflowActivationCompletion,
     },
     temporal::api::{
         common::v1::Payload, history::v1::History,
         workflowservice::v1::StartWorkflowExecutionResponse,
     },
     DEFAULT_ACTIVITY_TYPE,
 };
-use tokio::sync::{mpsc::unbounded_channel, OnceCell};
+use tokio::sync::OnceCell;
 use url::Url;
 
 pub const NAMESPACE: &str = "default";
 pub const TEST_Q: &str = "q";
 /// The env var used to specify where the integ tests should point
 pub const INTEG_SERVER_TARGET_ENV_VAR: &str = "TEMPORAL_SERVICE_ADDRESS";
 pub const INTEG_NAMESPACE_ENV_VAR: &str = "TEMPORAL_NAMESPACE";
@@ -145,35 +142,35 @@
     path.push("..");
     path.push(path_from_root);
     let bytes = tokio::fs::read(path).await?;
     Ok(History::decode(&*bytes)?)
 }
 
 static INTEG_TESTS_RT: once_cell::sync::OnceCell<CoreRuntime> = once_cell::sync::OnceCell::new();
-pub fn init_integ_telem() {
+pub fn init_integ_telem() -> &'static CoreRuntime {
     INTEG_TESTS_RT.get_or_init(|| {
         let telemetry_options = get_integ_telem_options();
         let rt =
             CoreRuntime::new_assume_tokio(telemetry_options).expect("Core runtime inits cleanly");
         if let Some(sub) = rt.telemetry().trace_subscriber() {
             let _ = tracing::subscriber::set_global_default(sub);
         }
         rt
-    });
+    })
 }
 
 /// Implements a builder pattern to help integ tests initialize core and create workflows
 pub struct CoreWfStarter {
     /// Used for both the task queue and workflow id
     task_queue_name: String,
     pub worker_config: WorkerConfigBuilder,
     /// Options to use when starting workflow(s)
     pub workflow_options: WorkflowOptions,
     initted_worker: OnceCell<InitializedWorker>,
-    runtime_override: Option<CoreRuntime>,
+    runtime_override: Option<Arc<CoreRuntime>>,
 }
 struct InitializedWorker {
     worker: Arc<dyn CoreWorker>,
     client: Arc<RetryClient<Client>>,
 }
 
 impl CoreWfStarter {
@@ -197,26 +194,26 @@
             .worker_build_id("test_build_id")
             .max_cached_workflows(1000_usize);
         Self {
             task_queue_name: task_queue,
             worker_config,
             initted_worker: OnceCell::new(),
             workflow_options: Default::default(),
-            runtime_override,
+            runtime_override: runtime_override.map(Arc::new),
         }
     }
 
     /// Create a new starter with no initialized worker or runtime override. Useful for starting a
     /// new worker on the same queue.
     pub fn clone_no_worker(&self) -> Self {
         Self {
             task_queue_name: self.task_queue_name.clone(),
             worker_config: self.worker_config.clone(),
             workflow_options: self.workflow_options.clone(),
-            runtime_override: None,
+            runtime_override: self.runtime_override.clone(),
             initted_worker: Default::default(),
         }
     }
 
     pub async fn worker(&mut self) -> TestWorker {
         let w = self.get_worker().await;
         let tq = w.get_config().task_queue.clone();
@@ -239,14 +236,15 @@
     }
 
     /// Start the workflow defined by the builder and return run id
     pub async fn start_wf(&mut self) -> String {
         self.start_wf_with_id(self.task_queue_name.clone()).await
     }
 
+    /// Starts the workflow using the worker, returns run id.
     pub async fn start_with_worker(
         &self,
         wf_name: impl Into<String>,
         worker: &mut TestWorker,
     ) -> String {
         worker
             .submit_wf(
@@ -355,34 +353,24 @@
     }
 
     pub fn no_remote_activities(&mut self) -> &mut Self {
         self.worker_config.no_remote_activities(true);
         self
     }
 
-    pub fn enable_wf_state_input_recording(&mut self) -> &mut Self {
-        let (ser_tx, ser_rx) = unbounded_channel();
-        let worker_cfg_clone = self.worker_config.build().unwrap();
-        tokio::spawn(async move {
-            stream_to_file(&worker_cfg_clone, ser_rx).await.unwrap();
-        });
-        self.worker_config.wf_state_inputs(Some(ser_tx));
-        self
-    }
-
     async fn get_or_init(&mut self) -> &InitializedWorker {
         self.initted_worker
             .get_or_init(|| async {
                 let cfg = self
                     .worker_config
                     .build()
                     .expect("Worker config must be valid");
                 let client = Arc::new(
                     get_integ_server_options()
-                        .connect(cfg.namespace.clone(), None, None)
+                        .connect(cfg.namespace.clone(), None)
                         .await
                         .expect("Must connect"),
                 );
                 let rt = if let Some(ref rto) = self.runtime_override {
                     rto
                 } else {
                     INTEG_TESTS_RT.get().unwrap()
@@ -506,15 +494,28 @@
             namespace: c.namespace().to_string(),
             workflow_id: wfid,
             run_id: Some(res.run_id.clone()),
         });
         Ok(res)
     }
 
-    /// Runs until all expected workflows have completed
+    pub fn expect_workflow_completion(&self, wf_id: impl Into<String>, run_id: Option<String>) {
+        self.started_workflows.lock().push(WorkflowExecutionInfo {
+            namespace: self
+                .client
+                .as_ref()
+                .map(|c| c.namespace())
+                .unwrap_or(NAMESPACE)
+                .to_owned(),
+            workflow_id: wf_id.into(),
+            run_id,
+        });
+    }
+
+    /// Runs until all expected workflows have completed and then shuts down the worker
     pub async fn run_until_done(&mut self) -> Result<(), anyhow::Error> {
         self.run_until_done_intercepted(Option::<TestWorkerCompletionIceptor>::None)
             .await
     }
 
     /// See [Self::run_until_done], but allows configuration of some low-level interception.
     pub async fn run_until_done_intercepted(
@@ -600,14 +601,20 @@
     }
 
     fn on_shutdown(&self, sdk_worker: &Worker) {
         if let Some(n) = self.next.as_ref() {
             n.on_shutdown(sdk_worker);
         }
     }
+    async fn on_workflow_activation(&self, a: &WorkflowActivation) -> Result<(), Error> {
+        if let Some(n) = self.next.as_ref() {
+            n.on_workflow_activation(a).await?;
+        }
+        Ok(())
+    }
 }
 
 /// Returns the client options used to connect to the server used for integration tests.
 pub fn get_integ_server_options() -> ClientOptions {
     let temporal_server_address = match env::var(INTEG_SERVER_TARGET_ENV_VAR) {
         Ok(addr) => addr,
         Err(_) => "http://localhost:7233".to_owned(),
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/test-utils/src/workflows.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/test-utils/src/workflows.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/fuzzy_workflow.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/fuzzy_workflow.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/heavy_tests.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/heavy_tests.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/client_tests.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/client_tests.rs`

 * *Files 0% similar despite different names*

```diff
@@ -13,24 +13,24 @@
         tokio::time::sleep(Duration::from_millis(10)).await;
     }
 }
 
 #[tokio::test]
 async fn can_use_retry_raw_client() {
     let opts = get_integ_server_options();
-    let raw_client = opts.connect_no_namespace(None, None).await.unwrap();
+    let raw_client = opts.connect_no_namespace(None).await.unwrap();
     let mut retry_client = RetryClient::new(raw_client, opts.retry_config);
     retry_client
         .describe_namespace(DescribeNamespaceRequest {
             namespace: NAMESPACE.to_string(),
             ..Default::default()
         })
         .await
         .unwrap();
 }
 
 #[tokio::test]
 async fn calls_get_system_info() {
     let opts = get_integ_server_options();
-    let raw_client = opts.connect_no_namespace(None, None).await.unwrap();
+    let raw_client = opts.connect_no_namespace(None).await.unwrap();
     assert!(raw_client.get_client().capabilities().is_some());
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/ephemeral_server_tests.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/ephemeral_server_tests.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,49 @@
 use std::time::{SystemTime, UNIX_EPOCH};
 use temporal_client::{ClientOptionsBuilder, TestService, WorkflowService};
 use temporal_sdk_core::ephemeral_server::{
     EphemeralExe, EphemeralExeVersion, EphemeralServer, TemporalDevServerConfigBuilder,
-    TemporaliteConfigBuilder, TestServerConfigBuilder,
+    TestServerConfigBuilder,
 };
 use temporal_sdk_core_protos::temporal::api::workflowservice::v1::DescribeNamespaceRequest;
 use temporal_sdk_core_test_utils::{default_cached_download, NAMESPACE};
 use url::Url;
 
 #[tokio::test]
 async fn temporal_cli_default() {
     let config = TemporalDevServerConfigBuilder::default()
         .exe(default_cached_download())
         .build()
         .unwrap();
     let mut server = config.start_server().await.unwrap();
     assert_ephemeral_server(&server).await;
+
+    // Make sure process is there on start and not there after shutdown
+    let pid = sysinfo::Pid::from_u32(server.child_process_id().unwrap());
+    assert!(sysinfo::System::new_all().process(pid).is_some());
     server.shutdown().await.unwrap();
+    assert!(sysinfo::System::new_all().process(pid).is_none());
 }
 
 #[tokio::test]
 async fn temporal_cli_fixed() {
     let config = TemporalDevServerConfigBuilder::default()
         .exe(fixed_cached_download("v0.4.0"))
         .build()
         .unwrap();
     let mut server = config.start_server().await.unwrap();
     assert_ephemeral_server(&server).await;
     server.shutdown().await.unwrap();
 }
 
 #[tokio::test]
-async fn temporalite_default() {
-    let config = TemporaliteConfigBuilder::default()
-        .exe(default_cached_download())
-        .build()
-        .unwrap();
-    let mut server = config.start_server().await.unwrap();
-    assert_ephemeral_server(&server).await;
-    server.shutdown().await.unwrap();
-}
-
-#[tokio::test]
-async fn temporalite_fixed() {
-    let config = TemporaliteConfigBuilder::default()
-        .exe(fixed_cached_download("v0.2.0"))
-        .build()
-        .unwrap();
-    let mut server = config.start_server().await.unwrap();
-    assert_ephemeral_server(&server).await;
-    server.shutdown().await.unwrap();
-}
-
-#[tokio::test]
-async fn temporalite_shutdown_port_reuse() {
+async fn temporal_cli_shutdown_port_reuse() {
     // Start, test shutdown, do again immediately on same port to ensure we can
     // reuse after shutdown
-    let config = TemporaliteConfigBuilder::default()
+    let config = TemporalDevServerConfigBuilder::default()
         .exe(default_cached_download())
         .port(Some(10123))
         .build()
         .unwrap();
     let mut server = config.start_server().await.unwrap();
     assert_ephemeral_server(&server).await;
     server.shutdown().await.unwrap();
@@ -120,15 +103,15 @@
     let mut client = ClientOptionsBuilder::default()
         .identity("integ_tester".to_string())
         .target_url(Url::try_from(&*format!("http://{}", server.target)).unwrap())
         .client_name("temporal-core".to_string())
         .client_version("0.1.0".to_string())
         .build()
         .unwrap()
-        .connect_no_namespace(None, None)
+        .connect_no_namespace(None)
         .await
         .unwrap();
     let resp = client
         .describe_namespace(DescribeNamespaceRequest {
             namespace: NAMESPACE.to_string(),
             ..Default::default()
         })
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/heartbeat_tests.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/heartbeat_tests.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/metrics_tests.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/metrics_tests.rs`

 * *Files 10% similar despite different names*

```diff
@@ -30,53 +30,60 @@
 use temporal_sdk_core_test_utils::{
     get_integ_server_options, get_integ_telem_options, CoreWfStarter, NAMESPACE,
 };
 use tokio::{join, sync::Barrier, task::AbortHandle};
 
 static ANY_PORT: &str = "127.0.0.1:0";
 
-async fn get_text(endpoint: String) -> String {
+pub(crate) async fn get_text(endpoint: String) -> String {
     reqwest::get(endpoint).await.unwrap().text().await.unwrap()
 }
 
-struct AbortOnDrop {
+pub(crate) struct AbortOnDrop {
     ah: AbortHandle,
 }
+
 impl Drop for AbortOnDrop {
     fn drop(&mut self) {
         self.ah.abort();
     }
 }
 
-fn prom_metrics() -> (TelemetryOptions, SocketAddr, AbortOnDrop) {
+pub(crate) fn prom_metrics(
+    use_seconds: bool,
+    show_units: bool,
+) -> (TelemetryOptions, SocketAddr, AbortOnDrop) {
     let mut telemopts = get_integ_telem_options();
     let prom_info = start_prometheus_metric_exporter(
         PrometheusExporterOptionsBuilder::default()
             .socket_addr(ANY_PORT.parse().unwrap())
+            .use_seconds_for_durations(use_seconds)
+            .unit_suffix(show_units)
             .build()
             .unwrap(),
     )
     .unwrap();
     telemopts.metrics = Some(prom_info.meter as Arc<dyn CoreMeter>);
     (
         telemopts,
         prom_info.bound_addr,
         AbortOnDrop {
             ah: prom_info.abort_handle,
         },
     )
 }
 
+#[rstest::rstest]
 #[tokio::test]
-async fn prometheus_metrics_exported() {
-    let (telemopts, addr, _aborter) = prom_metrics();
+async fn prometheus_metrics_exported(#[values(true, false)] use_seconds_latency: bool) {
+    let (telemopts, addr, _aborter) = prom_metrics(use_seconds_latency, false);
     let rt = CoreRuntime::new_assume_tokio(telemopts).unwrap();
     let opts = get_integ_server_options();
     let mut raw_client = opts
-        .connect_no_namespace(rt.telemetry().get_temporal_metric_meter(), None)
+        .connect_no_namespace(rt.telemetry().get_temporal_metric_meter())
         .await
         .unwrap();
     assert!(raw_client.get_client().capabilities().is_some());
 
     let _ = raw_client
         .list_namespaces(ListNamespacesRequest::default())
         .await
@@ -85,14 +92,25 @@
     let body = get_text(format!("http://{addr}/metrics")).await;
     assert!(body.contains(
         "temporal_request_latency_count{operation=\"ListNamespaces\",service_name=\"temporal-core-sdk\"} 1"
     ));
     assert!(body.contains(
         "temporal_request_latency_count{operation=\"GetSystemInfo\",service_name=\"temporal-core-sdk\"} 1"
     ));
+    if use_seconds_latency {
+        assert!(body.contains(
+            "temporal_request_latency_bucket{\
+             operation=\"GetSystemInfo\",service_name=\"temporal-core-sdk\",le=\"0.05\"}"
+        ));
+    } else {
+        assert!(body.contains(
+            "temporal_request_latency_bucket{\
+             operation=\"GetSystemInfo\",service_name=\"temporal-core-sdk\",le=\"50\"}"
+        ));
+    }
     // Verify counter names are appropriate (don't end w/ '_total')
     assert!(body.contains("temporal_request{"));
     // Verify non-temporal metrics meter does not prefix
     let mm = rt.telemetry().get_metric_meter().unwrap();
     let g = mm.inner.gauge(MetricParameters::from("mygauge"));
     g.record(
         42,
@@ -102,15 +120,15 @@
     );
     let body = get_text(format!("http://{addr}/metrics")).await;
     assert!(body.contains("\nmygauge 42"));
 }
 
 #[tokio::test]
 async fn one_slot_worker_reports_available_slot() {
-    let (telemopts, addr, _aborter) = prom_metrics();
+    let (telemopts, addr, _aborter) = prom_metrics(false, false);
     let tq = "one_slot_worker_tq";
     let rt = CoreRuntime::new_assume_tokio(telemopts).unwrap();
 
     let worker_cfg = WorkerConfigBuilder::default()
         .namespace(NAMESPACE)
         .task_queue(tq)
         .worker_build_id("test_build_id")
@@ -121,15 +139,15 @@
         .max_outstanding_workflow_tasks(2_usize)
         .max_concurrent_wft_polls(1_usize)
         .build()
         .unwrap();
 
     let client = Arc::new(
         get_integ_server_options()
-            .connect(worker_cfg.namespace.clone(), None, None)
+            .connect(worker_cfg.namespace.clone(), None)
             .await
             .expect("Must connect"),
     );
     let worker = init_worker(&rt, worker_cfg, client.clone()).expect("Worker inits cleanly");
     let wf_task_barr = Barrier::new(2);
     let act_task_barr = Barrier::new(2);
 
@@ -314,15 +332,15 @@
             failure: Some(Failure::application_failure("I'm ded".to_string(), false)),
         }.into(),
         ContinueAsNewWorkflowExecution::default().into(),
         CancelWorkflowExecution { }.into()
     )]
     completion: workflow_command::Variant,
 ) {
-    let (telemopts, addr, _aborter) = prom_metrics();
+    let (telemopts, addr, _aborter) = prom_metrics(false, false);
     let rt = CoreRuntime::new_assume_tokio(telemopts).unwrap();
     let mut starter =
         CoreWfStarter::new_with_runtime("query_of_closed_workflow_doesnt_tick_terminal_metric", rt);
     // Disable cache to ensure replay happens completely
     starter.max_cached_workflows(0);
     let worker = starter.get_worker().await;
     let run_id = starter.start_wf().await;
@@ -443,25 +461,65 @@
     let mut rt = CoreRuntime::new(
         get_integ_telem_options(),
         tokio::runtime::Builder::new_multi_thread(),
     )
     .unwrap();
     let handle = rt.tokio_handle();
     let _rt = handle.enter();
-    let (telemopts, addr, _aborter) = prom_metrics();
+    let (telemopts, addr, _aborter) = prom_metrics(false, false);
     rt.telemetry_mut()
         .attach_late_init_metrics(telemopts.metrics.unwrap());
     let opts = get_integ_server_options();
     handle.block_on(async {
         let mut raw_client = opts
-            .connect_no_namespace(rt.telemetry().get_temporal_metric_meter(), None)
+            .connect_no_namespace(rt.telemetry().get_temporal_metric_meter())
             .await
             .unwrap();
         assert!(raw_client.get_client().capabilities().is_some());
         let _ = raw_client
             .list_namespaces(ListNamespacesRequest::default())
             .await
             .unwrap();
         let body = get_text(format!("http://{addr}/metrics")).await;
         assert!(body.contains("temporal_request"));
     });
 }
+
+#[rstest::rstest]
+#[tokio::test]
+async fn latency_metrics(
+    #[values(true, false)] use_seconds_latency: bool,
+    #[values(true, false)] show_units: bool,
+) {
+    let (telemopts, addr, _aborter) = prom_metrics(use_seconds_latency, show_units);
+    let rt = CoreRuntime::new_assume_tokio(telemopts).unwrap();
+    let mut starter = CoreWfStarter::new_with_runtime("latency_metrics", rt);
+    let worker = starter.get_worker().await;
+    starter.start_wf().await;
+    // Immediately finish workflow
+    let task = worker.poll_workflow_activation().await.unwrap();
+    worker
+        .complete_workflow_activation(WorkflowActivationCompletion::from_cmd(
+            task.run_id,
+            CompleteWorkflowExecution { result: None }.into(),
+        ))
+        .await
+        .unwrap();
+
+    let body = get_text(format!("http://{addr}/metrics")).await;
+    let matching_line = body
+        .lines()
+        .find(|l| l.starts_with("temporal_workflow_endtoend_latency"))
+        .unwrap();
+
+    if use_seconds_latency {
+        if show_units {
+            assert!(matching_line.contains("temporal_workflow_endtoend_latency_seconds"));
+        }
+        assert!(matching_line.contains("le=\"0.1\""));
+    } else {
+        if show_units {
+            assert!(matching_line.contains("temporal_workflow_endtoend_latency_milliseconds"));
+        }
+        assert!(matching_line.contains("le=\"100\""));
+    }
+}
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/polling_tests.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/main.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,96 @@
-use assert_matches::assert_matches;
-use std::time::Duration;
-use temporal_sdk_core_protos::coresdk::{
-    activity_task::activity_task as act_task,
-    workflow_activation::{workflow_activation_job, FireTimer, WorkflowActivationJob},
-    workflow_commands::{ActivityCancellationType, RequestCancelActivity, StartTimer},
-    workflow_completion::WorkflowActivationCompletion,
-    IntoCompletion,
-};
-use temporal_sdk_core_test_utils::{
-    init_core_and_create_wf, schedule_activity_cmd, WorkerTestHelpers,
-};
-use tokio::time::timeout;
-
-#[tokio::test]
-async fn out_of_order_completion_doesnt_hang() {
-    let mut starter = init_core_and_create_wf("out_of_order_completion_doesnt_hang").await;
-    let core = starter.get_worker().await;
-    let task_q = starter.get_task_queue();
-    let activity_id = "act-1";
-    let task = core.poll_workflow_activation().await.unwrap();
-    // Complete workflow task and schedule activity and a timer that fires immediately
-    core.complete_workflow_activation(
-        vec![
-            schedule_activity_cmd(
-                0,
-                task_q,
-                activity_id,
-                ActivityCancellationType::TryCancel,
-                Duration::from_secs(60),
-                Duration::from_secs(60),
-            ),
-            StartTimer {
-                seq: 1,
-                start_to_fire_timeout: Some(prost_dur!(from_millis(50))),
-            }
-            .into(),
-        ]
-        .into_completion(task.run_id),
-    )
-    .await
-    .unwrap();
-    // Poll activity and verify that it's been scheduled, we don't expect to complete it in this
-    // test as activity is try-cancelled.
-    let activity_task = core.poll_activity_task().await.unwrap();
-    assert_matches!(activity_task.variant, Some(act_task::Variant::Start(_)));
-    // Poll workflow task and verify that activity has failed.
-    let task = core.poll_workflow_activation().await.unwrap();
-    assert_matches!(
-        task.jobs.as_slice(),
-        [
-            WorkflowActivationJob {
-                variant: Some(workflow_activation_job::Variant::FireTimer(
-                    FireTimer { seq: t_seq }
-                )),
-            },
-        ] => {
-            assert_eq!(*t_seq, 1);
-        }
-    );
-
-    // Start polling again *before* we complete the WFT
-    let cc = core.clone();
-    let jh = tokio::spawn(async move {
-        // We want to fail the test if this takes too long -- we should not hit long poll timeout
-        let task = timeout(Duration::from_secs(1), cc.poll_workflow_activation())
+//! Integration tests
+
+#[macro_use]
+extern crate rstest;
+#[macro_use]
+extern crate temporal_sdk_core_test_utils;
+
+#[cfg(test)]
+mod integ_tests {
+    mod activity_functions;
+    mod client_tests;
+    mod ephemeral_server_tests;
+    mod heartbeat_tests;
+    mod metrics_tests;
+    mod polling_tests;
+    mod queries_tests;
+    mod update_tests;
+    mod visibility_tests;
+    mod workflow_tests;
+
+    use std::str::FromStr;
+    use temporal_client::WorkflowService;
+    use temporal_sdk_core::{
+        init_worker, ClientOptionsBuilder, ClientTlsConfig, CoreRuntime, TlsConfig,
+        WorkflowClientTrait,
+    };
+    use temporal_sdk_core_api::worker::WorkerConfigBuilder;
+    use temporal_sdk_core_protos::temporal::api::workflowservice::v1::ListNamespacesRequest;
+    use temporal_sdk_core_test_utils::{
+        get_integ_server_options, get_integ_telem_options, init_integ_telem,
+    };
+    use url::Url;
+
+    // Create a worker like a bridge would (unwraps aside)
+    #[tokio::test]
+    #[ignore] // Really a compile time check more than anything
+    async fn lang_bridge_example() {
+        let opts = get_integ_server_options();
+        let runtime = CoreRuntime::new_assume_tokio(get_integ_telem_options()).unwrap();
+        let mut retrying_client = opts
+            .connect_no_namespace(runtime.telemetry().get_temporal_metric_meter())
             .await
-            .expect("Poll should come back right away")
             .unwrap();
-        assert_matches!(
-            task.jobs.as_slice(),
-            [WorkflowActivationJob {
-                variant: Some(workflow_activation_job::Variant::ResolveActivity(_)),
-            }]
+
+        let _worker = init_worker(
+            &runtime,
+            WorkerConfigBuilder::default()
+                .namespace("default")
+                .task_queue("Wheee!")
+                .build()
+                .unwrap(),
+            // clone the client if you intend to use it later. Strip off the retry wrapper since
+            // worker will assert its own
+            retrying_client.clone(),
         );
-        cc.complete_execution(&task.run_id).await;
-    });
 
-    tokio::time::sleep(Duration::from_millis(100)).await;
-    // Then complete the (last) WFT with a request to cancel the AT, which should produce a
-    // pending activation, unblocking the (already started) poll
-    core.complete_workflow_activation(WorkflowActivationCompletion::from_cmds(
-        task.run_id,
-        vec![RequestCancelActivity { seq: 0 }.into()],
-    ))
-    .await
-    .unwrap();
+        // Do things with worker or client
+        let _ = retrying_client
+            .list_namespaces(ListNamespacesRequest::default())
+            .await;
+    }
 
-    jh.await.unwrap();
+    // Manually run to verify tls works against cloud. You will need certs in place in the
+    // indicated directory.
+    #[tokio::test]
+    #[ignore]
+    async fn tls_test() {
+        init_integ_telem();
+        let root = tokio::fs::read("../.cloud_certs/ca.pem").await.unwrap();
+        let client_cert = tokio::fs::read("../.cloud_certs/client.pem").await.unwrap();
+        let client_private_key = tokio::fs::read("../.cloud_certs/client.key").await.unwrap();
+        let sgo = ClientOptionsBuilder::default()
+            .target_url(Url::from_str("https://spencer.temporal-dev.tmprl.cloud:7233").unwrap())
+            .client_name("tls_tester")
+            .client_version("clientver")
+            .tls_cfg(TlsConfig {
+                server_root_ca_cert: Some(root),
+                // Not necessary, but illustrates functionality for people using proxies, etc.
+                domain: Some("spencer.temporal-dev.tmprl.cloud".to_string()),
+                client_tls_config: Some(ClientTlsConfig {
+                    client_cert,
+                    client_private_key,
+                }),
+            })
+            .build()
+            .unwrap();
+        let con = sgo
+            .connect("spencer.temporal-dev".to_string(), None)
+            .await
+            .unwrap();
+        dbg!(con
+            .list_workflow_executions(100, vec![], "".to_string())
+            .await
+            .unwrap());
+    }
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/queries_tests.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/queries_tests.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/update_tests.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/update_tests.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use anyhow::{anyhow, bail};
 use assert_matches::assert_matches;
 use futures_util::{future, future::join_all, StreamExt};
-use lazy_static::lazy_static;
+use once_cell::sync::Lazy;
 use std::{
     sync::atomic::{AtomicBool, AtomicUsize, Ordering},
     time::Duration,
 };
 use temporal_client::WorkflowClientTrait;
 use temporal_sdk::{ActContext, ActivityOptions, LocalActivityOptions, UpdateContext, WfContext};
 use temporal_sdk_core::replay::HistoryForReplay;
@@ -813,17 +813,15 @@
 #[tokio::test]
 async fn worker_restarted_in_middle_of_update() {
     let wf_name = "worker_restarted_in_middle_of_update";
     let mut starter = CoreWfStarter::new(wf_name);
     let mut worker = starter.worker().await;
     let client = starter.get_client().await;
 
-    lazy_static! {
-        static ref BARR: Barrier = Barrier::new(2);
-    }
+    static BARR: Lazy<Barrier> = Lazy::new(|| Barrier::new(2));
     static ACT_RAN: AtomicBool = AtomicBool::new(false);
     worker.register_wf(wf_name.to_owned(), |ctx: WfContext| async move {
         ctx.update_handler(
             "update",
             |_: &_, _: ()| Ok(()),
             move |ctx: UpdateContext, _: ()| async move {
                 ctx.wf_ctx
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/visibility_tests.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/visibility_tests.rs`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     assert!(passed);
 }
 
 #[tokio::test]
 async fn client_create_namespace() {
     let client = Arc::new(
         get_integ_server_options()
-            .connect(NAMESPACE.to_owned(), None, None)
+            .connect(NAMESPACE.to_owned(), None)
             .await
             .expect("Must connect"),
     );
 
     let register_options = RegisterNamespaceOptions::builder()
         .namespace("test-create-namespace")
         .description("it's alive")
@@ -134,15 +134,15 @@
     }
 }
 
 #[tokio::test]
 async fn client_describe_namespace() {
     let client = Arc::new(
         get_integ_server_options()
-            .connect(NAMESPACE.to_owned(), None, None)
+            .connect(NAMESPACE.to_owned(), None)
             .await
             .expect("Must connect"),
     );
 
     let namespace_result = client
         .describe_namespace(Namespace::Name(NAMESPACE.to_owned()))
         .await
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/activities.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/activities.rs`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 };
 use temporal_sdk_core_test_utils::{
     drain_pollers_and_shutdown, init_core_and_create_wf, schedule_activity_cmd, CoreWfStarter,
     WorkerTestHelpers,
 };
 use tokio::{join, sync::Semaphore, time::sleep};
 
-pub async fn one_activity_wf(ctx: WfContext) -> WorkflowResult<()> {
+pub(crate) async fn one_activity_wf(ctx: WfContext) -> WorkflowResult<()> {
     ctx.activity(ActivityOptions {
         activity_type: "echo_activity".to_string(),
         start_to_close_timeout: Some(Duration::from_secs(5)),
         input: "hi!".as_json_payload().expect("serializes fine"),
         ..Default::default()
     })
     .await;
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/appdata_propagation.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/appdata_propagation.rs`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 const TEST_APPDATA_MESSAGE: &str = "custom app data, yay";
 
 struct Data {
     message: String,
 }
 
-pub async fn appdata_activity_wf(ctx: WfContext) -> WorkflowResult<()> {
+pub(crate) async fn appdata_activity_wf(ctx: WfContext) -> WorkflowResult<()> {
     ctx.activity(ActivityOptions {
         activity_type: "echo_activity".to_string(),
         start_to_close_timeout: Some(Duration::from_secs(5)),
         input: "hi!".as_json_payload().expect("serializes fine"),
         ..Default::default()
     })
     .await;
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/cancel_external.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/cancel_external.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/cancel_wf.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/cancel_wf.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/child_workflows.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/child_workflows.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/continue_as_new.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/continue_as_new.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/determinism.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/determinism.rs`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
     sync::atomic::{AtomicUsize, Ordering},
     time::Duration,
 };
 use temporal_sdk::{ActivityOptions, WfContext, WorkflowResult};
 use temporal_sdk_core_test_utils::CoreWfStarter;
 
 static RUN_CT: AtomicUsize = AtomicUsize::new(1);
-pub async fn timer_wf_nondeterministic(ctx: WfContext) -> WorkflowResult<()> {
+
+pub(crate) async fn timer_wf_nondeterministic(ctx: WfContext) -> WorkflowResult<()> {
     let run_ct = RUN_CT.fetch_add(1, Ordering::Relaxed);
 
     match run_ct {
         1 | 3 => {
             // If we have not run yet or are on the third attempt, schedule a timer
             ctx.timer(Duration::from_secs(1)).await;
             if run_ct == 1 {
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/eager.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/eager.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::time::Duration;
-use temporal_client::{WorkflowClientTrait, WorkflowExecutionInfo};
+use temporal_client::WorkflowClientTrait;
 use temporal_sdk::{WfContext, WorkflowResult};
 use temporal_sdk_core_test_utils::{get_integ_server_options, CoreWfStarter, NAMESPACE};
 
-pub async fn eager_wf(_context: WfContext) -> WorkflowResult<()> {
+pub(crate) async fn eager_wf(_context: WfContext) -> WorkflowResult<()> {
     Ok(().into())
 }
 
 #[tokio::test]
 async fn eager_wf_start() {
     let wf_name = "eager_wf_start";
     let mut starter = CoreWfStarter::new(wf_name);
@@ -29,15 +29,15 @@
     // hang the test if wf task needs retry
     starter.workflow_options.task_timeout = Some(Duration::from_secs(1500));
     starter.no_remote_activities();
     let mut worker = starter.worker().await;
     worker.register_wf(wf_name.to_owned(), eager_wf);
 
     let client = get_integ_server_options()
-        .connect(NAMESPACE.to_string(), None, None)
+        .connect(NAMESPACE.to_string(), None)
         .await
         .expect("Should connect");
     let w = starter.get_worker().await;
     let res = client
         .start_workflow(
             vec![],
             w.get_config().task_queue.clone(), // task_queue
@@ -48,14 +48,10 @@
         )
         .await
         .unwrap();
     // different clients means no eager_wf_start.
     assert!(res.eager_workflow_task.is_none());
 
     //wf task delivered through default path
-    worker.started_workflows.lock().push(WorkflowExecutionInfo {
-        namespace: NAMESPACE.to_string(),
-        workflow_id: wf_name.to_string(),
-        run_id: Some(res.run_id.clone()),
-    });
+    worker.expect_workflow_completion(wf_name, Some(res.run_id));
     worker.run_until_done().await.unwrap();
 }
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/local_activities.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/local_activities.rs`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     TestHistoryBuilder,
 };
 use temporal_sdk_core_test_utils::{
     history_from_proto_binary, replay_sdk_worker, workflows::la_problem_workflow, CoreWfStarter,
 };
 use tokio_util::sync::CancellationToken;
 
-pub async fn one_local_activity_wf(ctx: WfContext) -> WorkflowResult<()> {
+pub(crate) async fn one_local_activity_wf(ctx: WfContext) -> WorkflowResult<()> {
     let initial_workflow_time = ctx.workflow_time().expect("Workflow time should be set");
     ctx.local_activity(LocalActivityOptions {
         activity_type: "echo_activity".to_string(),
         input: "hi!".as_json_payload().expect("serializes fine"),
         ..Default::default()
     })
     .await;
@@ -47,15 +47,15 @@
     worker.register_wf(wf_name.to_owned(), one_local_activity_wf);
     worker.register_activity("echo_activity", echo);
 
     starter.start_with_worker(wf_name, &mut worker).await;
     worker.run_until_done().await.unwrap();
 }
 
-pub async fn local_act_concurrent_with_timer_wf(ctx: WfContext) -> WorkflowResult<()> {
+pub(crate) async fn local_act_concurrent_with_timer_wf(ctx: WfContext) -> WorkflowResult<()> {
     let la = ctx.local_activity(LocalActivityOptions {
         activity_type: "echo_activity".to_string(),
         input: "hi!".as_json_payload().expect("serializes fine"),
         ..Default::default()
     });
     let timer = ctx.timer(Duration::from_secs(1));
     tokio::join!(la, timer);
@@ -70,15 +70,15 @@
     worker.register_wf(wf_name.to_owned(), local_act_concurrent_with_timer_wf);
     worker.register_activity("echo_activity", echo);
 
     starter.start_with_worker(wf_name, &mut worker).await;
     worker.run_until_done().await.unwrap();
 }
 
-pub async fn local_act_then_timer_then_wait(ctx: WfContext) -> WorkflowResult<()> {
+pub(crate) async fn local_act_then_timer_then_wait(ctx: WfContext) -> WorkflowResult<()> {
     let la = ctx.local_activity(LocalActivityOptions {
         activity_type: "echo_activity".to_string(),
         input: "hi!".as_json_payload().expect("serializes fine"),
         ..Default::default()
     });
     ctx.timer(Duration::from_secs(1)).await;
     let res = la.await;
@@ -110,15 +110,15 @@
         Ok(str)
     });
 
     starter.start_with_worker(wf_name, &mut worker).await;
     worker.run_until_done().await.unwrap();
 }
 
-pub async fn local_act_fanout_wf(ctx: WfContext) -> WorkflowResult<()> {
+pub(crate) async fn local_act_fanout_wf(ctx: WfContext) -> WorkflowResult<()> {
     let las: Vec<_> = (1..=50)
         .map(|i| {
             ctx.local_activity(LocalActivityOptions {
                 activity_type: "echo_activity".to_string(),
                 input: format!("Hi {i}")
                     .as_json_payload()
                     .expect("serializes fine"),
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/modify_wf_properties.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/modify_wf_properties.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/patches.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/patches.rs`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 use tokio_stream::StreamExt;
 
 use temporal_sdk::{WfContext, WorkflowResult};
 use temporal_sdk_core_test_utils::CoreWfStarter;
 
 const MY_PATCH_ID: &str = "integ_test_change_name";
 
-pub async fn changes_wf(ctx: WfContext) -> WorkflowResult<()> {
+pub(crate) async fn changes_wf(ctx: WfContext) -> WorkflowResult<()> {
     if ctx.patched(MY_PATCH_ID) {
         ctx.timer(Duration::from_millis(100)).await;
     } else {
         ctx.timer(Duration::from_millis(200)).await;
     }
     ctx.timer(Duration::from_millis(200)).await;
     if ctx.patched(MY_PATCH_ID) {
@@ -40,15 +40,16 @@
     starter.start_with_worker(wf_name, &mut worker).await;
     worker.run_until_done().await.unwrap();
 }
 
 /// This one simulates a run as if the worker had the "old" code, then it fails at the end as
 /// a cheapo way of being re-run, at which point it runs with change checks and the "new" code.
 static DID_DIE: AtomicBool = AtomicBool::new(false);
-pub async fn no_change_then_change_wf(ctx: WfContext) -> WorkflowResult<()> {
+
+pub(crate) async fn no_change_then_change_wf(ctx: WfContext) -> WorkflowResult<()> {
     if DID_DIE.load(Ordering::Acquire) {
         assert!(!ctx.patched(MY_PATCH_ID));
     }
     ctx.timer(Duration::from_millis(200)).await;
     ctx.timer(Duration::from_millis(200)).await;
     if DID_DIE.load(Ordering::Acquire) {
         assert!(!ctx.patched(MY_PATCH_ID));
@@ -71,15 +72,16 @@
     worker.register_wf(wf_name.to_owned(), no_change_then_change_wf);
 
     starter.start_with_worker(wf_name, &mut worker).await;
     worker.run_until_done().await.unwrap();
 }
 
 static DID_DIE_2: AtomicBool = AtomicBool::new(false);
-pub async fn replay_with_change_marker_wf(ctx: WfContext) -> WorkflowResult<()> {
+
+pub(crate) async fn replay_with_change_marker_wf(ctx: WfContext) -> WorkflowResult<()> {
     assert!(ctx.patched(MY_PATCH_ID));
     ctx.timer(Duration::from_millis(200)).await;
     if !DID_DIE_2.load(Ordering::Acquire) {
         DID_DIE_2.store(true, Ordering::Release);
         ctx.force_task_fail(anyhow::anyhow!("i'm ded"));
     }
     Ok(().into())
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/replay.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/replay.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/resets.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/resets.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/signals.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/signals.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 use std::collections::HashMap;
 
 use futures::StreamExt;
-use temporal_client::{
-    SignalWithStartOptions, WorkflowClientTrait, WorkflowExecutionInfo, WorkflowOptions,
-};
+use temporal_client::{SignalWithStartOptions, WorkflowClientTrait, WorkflowOptions};
 use temporal_sdk::{
     ChildWorkflowOptions, Signal, SignalWorkflowOptions, WfContext, WorkflowResult,
 };
 use temporal_sdk_core_protos::{coresdk::IntoPayloadsExt, temporal::api::common::v1::Payload};
 use temporal_sdk_core_test_utils::CoreWfStarter;
 use uuid::Uuid;
 
@@ -119,20 +117,15 @@
         .build()
         .unwrap();
     let res = client
         .signal_with_start_workflow_execution(options, WorkflowOptions::default())
         .await
         .expect("request succeeds.qed");
 
-    worker.started_workflows.lock().push(WorkflowExecutionInfo {
-        namespace: client.namespace().to_string(),
-        workflow_id: "sends_signal_with_create_wf".to_owned(),
-        run_id: Some(res.run_id.clone()),
-    });
-
+    worker.expect_workflow_completion("sends_signal_with_create_wf", Some(res.run_id));
     worker.run_until_done().await.unwrap();
 }
 
 async fn signals_child(ctx: WfContext) -> WorkflowResult<()> {
     let started_child = ctx
         .child_workflow(ChildWorkflowOptions {
             workflow_id: "my_precious_child".to_string(),
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/stickyness.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/stickyness.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/timers.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/timers.rs`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     workflow_completion::WorkflowActivationCompletion,
 };
 use temporal_sdk_core_test_utils::{
     drain_pollers_and_shutdown, init_core_and_create_wf, start_timer_cmd, CoreWfStarter,
     WorkerTestHelpers,
 };
 
-pub async fn timer_wf(command_sink: WfContext) -> WorkflowResult<()> {
+pub(crate) async fn timer_wf(command_sink: WfContext) -> WorkflowResult<()> {
     command_sink.timer(Duration::from_secs(1)).await;
     Ok(().into())
 }
 
 #[tokio::test]
 async fn timer_workflow_workflow_driver() {
     let wf_name = "timer_wf_new";
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/upsert_search_attrs.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests/upsert_search_attrs.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/integ_tests/workflow_tests.rs`

 * *Files 25% similar despite different names*

```diff
@@ -12,40 +12,46 @@
 mod replay;
 mod resets;
 mod signals;
 mod stickyness;
 mod timers;
 mod upsert_search_attrs;
 
-use crate::integ_tests::activity_functions::echo;
+use crate::integ_tests::{activity_functions::echo, metrics_tests};
 use assert_matches::assert_matches;
 use futures::{channel::mpsc::UnboundedReceiver, future, SinkExt, StreamExt};
 use std::{
-    collections::HashMap,
+    collections::{HashMap, HashSet},
     sync::{
         atomic::{AtomicUsize, Ordering},
         Arc,
     },
     time::Duration,
 };
 use temporal_client::{WorkflowClientTrait, WorkflowOptions};
 use temporal_sdk::{interceptors::WorkerInterceptor, ActivityOptions, WfContext, WorkflowResult};
-use temporal_sdk_core::replay::HistoryForReplay;
-use temporal_sdk_core_api::{errors::PollWfError, Worker};
+use temporal_sdk_core::{replay::HistoryForReplay, CoreRuntime};
+use temporal_sdk_core_api::{
+    errors::{PollWfError, WorkflowErrorType},
+    Worker,
+};
 use temporal_sdk_core_protos::{
     coresdk::{
         activity_result::ActivityExecutionResult,
         workflow_activation::{workflow_activation_job, WorkflowActivation, WorkflowActivationJob},
         workflow_commands::{
             ActivityCancellationType, FailWorkflowExecution, QueryResult, QuerySuccess, StartTimer,
         },
         workflow_completion::WorkflowActivationCompletion,
         ActivityTaskCompletion, AsJsonPayloadExt, IntoCompletion,
     },
-    temporal::api::{failure::v1::Failure, history::v1::history_event, query::v1::WorkflowQuery},
+    temporal::api::{
+        enums::v1::EventType, failure::v1::Failure, history::v1::history_event,
+        query::v1::WorkflowQuery,
+    },
 };
 use temporal_sdk_core_test_utils::{
     drain_pollers_and_shutdown, history_from_proto_binary, init_core_and_create_wf,
     init_core_replay_preloaded, schedule_activity_cmd, CoreWfStarter, WorkerTestHelpers,
 };
 use tokio::{join, time::sleep};
 use uuid::Uuid;
@@ -105,15 +111,16 @@
     for handle in handles {
         handle.await.unwrap()
     }
     drain_pollers_and_shutdown(&core).await;
 }
 
 static RUN_CT: AtomicUsize = AtomicUsize::new(0);
-pub async fn cache_evictions_wf(command_sink: WfContext) -> WorkflowResult<()> {
+
+pub(crate) async fn cache_evictions_wf(command_sink: WfContext) -> WorkflowResult<()> {
     RUN_CT.fetch_add(1, Ordering::SeqCst);
     command_sink.timer(Duration::from_secs(1)).await;
     Ok(().into())
 }
 
 #[tokio::test]
 async fn workflow_lru_cache_evictions() {
@@ -726,7 +733,96 @@
         .await
         .unwrap();
 
     let res = core.poll_workflow_activation().await.unwrap();
     assert_eq!(res.build_id_for_current_task, "2.0");
     core.complete_execution(&res.run_id).await;
 }
+
+#[rstest::rstest]
+#[tokio::test]
+async fn nondeterminism_errors_fail_workflow_when_configured_to(
+    #[values(true, false)] whole_worker: bool,
+) {
+    let (telemopts, addr, _aborter) = metrics_tests::prom_metrics(false, false);
+    let rt = CoreRuntime::new_assume_tokio(telemopts).unwrap();
+    let wf_name = "nondeterminism_errors_fail_workflow_when_configured_to";
+    let mut starter = CoreWfStarter::new_with_runtime(wf_name, rt);
+    starter.no_remote_activities();
+    let typeset = HashSet::from([WorkflowErrorType::Nondeterminism]);
+    if whole_worker {
+        starter.worker_config.workflow_failure_errors(typeset);
+    } else {
+        starter
+            .worker_config
+            .workflow_types_to_failure_errors(HashMap::from([(wf_name.to_owned(), typeset)]));
+    }
+    let wf_id = starter.get_task_queue().to_owned();
+    let mut worker = starter.worker().await;
+    worker.fetch_results = false;
+
+    worker.register_wf(wf_name.to_owned(), move |ctx: WfContext| async move {
+        ctx.timer(Duration::from_secs(1000)).await;
+        Ok(().into())
+    });
+    let client = starter.get_client().await;
+    let core_worker = worker.core_worker.clone();
+    starter.start_with_worker(wf_name, &mut worker).await;
+
+    let stopper = async {
+        // Wait for the timer to show up in history and then stop the worker
+        loop {
+            let hist = client
+                .get_workflow_execution_history(wf_id.clone(), None, vec![])
+                .await
+                .unwrap()
+                .history
+                .unwrap();
+            let has_timer_event = hist
+                .events
+                .iter()
+                .any(|e| matches!(e.event_type(), EventType::TimerStarted));
+            if has_timer_event {
+                break;
+            }
+            tokio::time::sleep(Duration::from_millis(100)).await;
+        }
+        core_worker.initiate_shutdown();
+    };
+    let runner = async {
+        worker.run_until_done().await.unwrap();
+    };
+    join!(stopper, runner);
+
+    // Restart the worker with a new, incompatible wf definition which will cause nondeterminism
+    let mut starter = starter.clone_no_worker();
+    let mut worker = starter.worker().await;
+    worker.register_wf(wf_name.to_owned(), move |ctx: WfContext| async move {
+        ctx.activity(ActivityOptions {
+            activity_type: "echo_activity".to_string(),
+            start_to_close_timeout: Some(Duration::from_secs(5)),
+            ..Default::default()
+        })
+        .await;
+        Ok(().into())
+    });
+    // We need to generate a task so that we'll encounter the error (first avoid WFT timeout)
+    client
+        .reset_sticky_task_queue(wf_id.clone(), "".to_string())
+        .await
+        .unwrap();
+    client
+        .signal_workflow_execution(wf_id.clone(), "".to_string(), "hi".to_string(), None, None)
+        .await
+        .unwrap();
+    worker.expect_workflow_completion(&wf_id, None);
+    // If we don't fail the workflow on nondeterminism, we'll get stuck here retrying the WFT
+    worker.run_until_done().await.unwrap();
+
+    let body = metrics_tests::get_text(format!("http://{addr}/metrics")).await;
+    let match_this = format!(
+        "temporal_workflow_failed{{namespace=\"default\",\
+         service_name=\"temporal-core-sdk\",\
+         task_queue=\"{wf_id}\",workflow_type=\"{wf_name}\"}} 1"
+    );
+    assert!(body.contains(&match_this));
+}
```

### Comparing `temporalio-1.5.1/temporalio/bridge/sdk-core/tests/runner.rs` & `temporalio-1.6.0/temporalio/bridge/sdk-core/tests/runner.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/src/client.rs` & `temporalio-1.6.0/temporalio/bridge/src/client.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-use parking_lot::RwLock;
 use pyo3::exceptions::{PyException, PyRuntimeError, PyValueError};
 use pyo3::prelude::*;
 use std::collections::HashMap;
 use std::str::FromStr;
-use std::sync::Arc;
 use std::time::Duration;
 use temporal_client::{
     ClientKeepAliveConfig as CoreClientKeepAliveConfig, ClientOptions, ClientOptionsBuilder,
-    ConfiguredClient, HealthService, OperatorService, RetryClient, RetryConfig,
-    TemporalServiceClientWithMetrics, TestService, TlsConfig, WorkflowService,
+    ConfiguredClient, HealthService, HttpConnectProxyOptions, OperatorService, RetryClient,
+    RetryConfig, TemporalServiceClientWithMetrics, TestService, TlsConfig, WorkflowService,
 };
 use tonic::metadata::MetadataKey;
 use url::Url;
 
 use crate::runtime;
 
 pyo3::create_exception!(temporal_sdk_bridge, RPCError, PyException);
@@ -27,18 +25,20 @@
 
 #[derive(FromPyObject)]
 pub struct ClientConfig {
     target_url: String,
     client_name: String,
     client_version: String,
     metadata: HashMap<String, String>,
+    api_key: Option<String>,
     identity: String,
     tls_config: Option<ClientTlsConfig>,
     retry_config: Option<ClientRetryConfig>,
     keep_alive_config: Option<ClientKeepAliveConfig>,
+    http_connect_proxy_config: Option<ClientHttpConnectProxyConfig>,
 }
 
 #[derive(FromPyObject)]
 struct ClientTlsConfig {
     server_root_ca_cert: Option<Vec<u8>>,
     domain: Option<String>,
     client_cert: Option<Vec<u8>>,
@@ -58,41 +58,39 @@
 #[derive(FromPyObject)]
 struct ClientKeepAliveConfig {
     pub interval_millis: u64,
     pub timeout_millis: u64,
 }
 
 #[derive(FromPyObject)]
+struct ClientHttpConnectProxyConfig {
+    pub target_host: String,
+    pub basic_auth: Option<(String, String)>,
+}
+
+#[derive(FromPyObject)]
 struct RpcCall {
     rpc: String,
     req: Vec<u8>,
     retry: bool,
     metadata: HashMap<String, String>,
     timeout_millis: Option<u64>,
 }
 
 pub fn connect_client<'a>(
     py: Python<'a>,
     runtime_ref: &runtime::RuntimeRef,
     config: ClientConfig,
 ) -> PyResult<&'a PyAny> {
-    let headers = if config.metadata.is_empty() {
-        None
-    } else {
-        Some(Arc::new(RwLock::new(config.metadata.clone())))
-    };
     let opts: ClientOptions = config.try_into()?;
     let runtime = runtime_ref.runtime.clone();
     runtime_ref.runtime.future_into_py(py, async move {
         Ok(ClientRef {
             retry_client: opts
-                .connect_no_namespace(
-                    runtime.core.telemetry().get_temporal_metric_meter(),
-                    headers,
-                )
+                .connect_no_namespace(runtime.core.telemetry().get_temporal_metric_meter())
                 .await
                 .map_err(|err| {
                     PyRuntimeError::new_err(format!("Failed client connect: {}", err))
                 })?,
             runtime,
         })
     })
@@ -110,14 +108,18 @@
 
 #[pymethods]
 impl ClientRef {
     fn update_metadata(&self, headers: HashMap<String, String>) {
         self.retry_client.get_client().set_headers(headers);
     }
 
+    fn update_api_key(&self, api_key: Option<String>) {
+        self.retry_client.get_client().set_api_key(api_key);
+    }
+
     fn call_workflow_service<'p>(&self, py: Python<'p>, call: RpcCall) -> PyResult<&'p PyAny> {
         let mut retry_client = self.retry_client.clone();
         self.runtime.future_into_py(py, async move {
             let bytes = match call.rpc.as_str() {
                 "count_workflow_executions" => {
                     rpc_call!(retry_client, call, count_workflow_executions)
                 }
@@ -392,15 +394,18 @@
             .client_name(opts.client_name)
             .client_version(opts.client_version)
             .identity(opts.identity)
             .retry_config(
                 opts.retry_config
                     .map_or(RetryConfig::default(), |c| c.into()),
             )
-            .keep_alive(opts.keep_alive_config.map(Into::into));
+            .keep_alive(opts.keep_alive_config.map(Into::into))
+            .http_connect_proxy(opts.http_connect_proxy_config.map(Into::into))
+            .headers(Some(opts.metadata))
+            .api_key(opts.api_key);
         // Builder does not allow us to set option here, so we have to make
         // a conditional to even call it
         if let Some(tls_config) = opts.tls_config {
             gateway_opts.tls_cfg(tls_config.try_into()?);
         }
         return gateway_opts
             .build()
@@ -450,7 +455,16 @@
     fn from(conf: ClientKeepAliveConfig) -> Self {
         CoreClientKeepAliveConfig {
             interval: Duration::from_millis(conf.interval_millis),
             timeout: Duration::from_millis(conf.timeout_millis),
         }
     }
 }
+
+impl From<ClientHttpConnectProxyConfig> for HttpConnectProxyOptions {
+    fn from(conf: ClientHttpConnectProxyConfig) -> Self {
+        HttpConnectProxyOptions {
+            target_addr: conf.target_host,
+            basic_auth: conf.basic_auth,
+        }
+    }
+}
```

### Comparing `temporalio-1.5.1/temporalio/bridge/src/lib.rs` & `temporalio-1.6.0/temporalio/bridge/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,18 @@
     m.add_function(wrap_pyfunction!(connect_client, m)?)?;
 
     // Metric stuff
     m.add_class::<metric::MetricMeterRef>()?;
     m.add_class::<metric::MetricAttributesRef>()?;
     m.add_class::<metric::MetricCounterRef>()?;
     m.add_class::<metric::MetricHistogramRef>()?;
+    m.add_class::<metric::MetricHistogramFloatRef>()?;
+    m.add_class::<metric::MetricHistogramDurationRef>()?;
     m.add_class::<metric::MetricGaugeRef>()?;
+    m.add_class::<metric::MetricGaugeFloatRef>()?;
     m.add_class::<metric::BufferedMetricUpdate>()?;
     m.add_class::<metric::BufferedMetric>()?;
     m.add_function(wrap_pyfunction!(new_metric_meter, m)?)?;
 
     // Runtime stuff
     m.add_class::<runtime::RuntimeRef>()?;
     m.add_class::<runtime::BufferedLogEntry>()?;
```

### Comparing `temporalio-1.5.1/temporalio/bridge/src/runtime.rs` & `temporalio-1.6.0/temporalio/bridge/src/runtime.rs`

 * *Files 4% similar despite different names*

```diff
@@ -70,21 +70,23 @@
 
 #[derive(FromPyObject)]
 pub struct OpenTelemetryConfig {
     url: String,
     headers: HashMap<String, String>,
     metric_periodicity_millis: Option<u64>,
     metric_temporality_delta: bool,
+    durations_as_seconds: bool,
 }
 
 #[derive(FromPyObject)]
 pub struct PrometheusConfig {
     bind_address: String,
     counters_total_suffix: bool,
     unit_suffix: bool,
+    durations_as_seconds: bool,
 }
 
 const FORWARD_LOG_BUFFER_SIZE: usize = 2048;
 const FORWARD_LOG_MAX_FREQ_MS: u64 = 10;
 
 pub fn init_runtime(telemetry_config: TelemetryConfig) -> PyResult<RuntimeRef> {
     // Have to build/start telemetry config pieces
@@ -199,22 +201,27 @@
             handle.abort();
         }
     }
 }
 
 #[pymethods]
 impl RuntimeRef {
-    fn retrieve_buffered_metrics<'p>(&self, py: Python<'p>) -> Vec<BufferedMetricUpdate> {
+    fn retrieve_buffered_metrics<'p>(
+        &self,
+        py: Python<'p>,
+        durations_as_seconds: bool,
+    ) -> Vec<BufferedMetricUpdate> {
         convert_metric_events(
             py,
             self.runtime
                 .metrics_call_buffer
                 .as_ref()
                 .expect("Attempting to retrieve buffered metrics without buffer")
                 .retrieve(),
+            durations_as_seconds,
         )
     }
 
     fn write_test_info_log(&self, message: &str, extra_data: &str) {
         let _g = tracing::subscriber::set_default(
             self.runtime
                 .core
@@ -301,15 +308,16 @@
             let mut build = OtelCollectorOptionsBuilder::default();
             build
                 .url(
                     Url::parse(&otel_conf.url).map_err(|err| {
                         PyValueError::new_err(format!("Invalid OTel URL: {}", err))
                     })?,
                 )
-                .headers(otel_conf.headers);
+                .headers(otel_conf.headers)
+                .use_seconds_for_durations(otel_conf.durations_as_seconds);
             if let Some(period) = otel_conf.metric_periodicity_millis {
                 build.metric_periodicity(Duration::from_millis(period));
             }
             if otel_conf.metric_temporality_delta {
                 build.metric_temporality(MetricTemporality::Delta);
             }
             if let Some(global_tags) = conf.global_tags {
@@ -327,15 +335,16 @@
             build
                 .socket_addr(
                     SocketAddr::from_str(&prom_conf.bind_address).map_err(|err| {
                         PyValueError::new_err(format!("Invalid Prometheus address: {}", err))
                     })?,
                 )
                 .counters_total_suffix(prom_conf.counters_total_suffix)
-                .unit_suffix(prom_conf.unit_suffix);
+                .unit_suffix(prom_conf.unit_suffix)
+                .use_seconds_for_durations(prom_conf.durations_as_seconds);
             if let Some(global_tags) = conf.global_tags {
                 build.global_tags(global_tags);
             }
             let prom_options = build.build().map_err(|err| {
                 PyValueError::new_err(format!("Invalid Prometheus config: {}", err))
             })?;
             Ok(start_prometheus_metric_exporter(prom_options)
```

### Comparing `temporalio-1.5.1/temporalio/bridge/src/testing.rs` & `temporalio-1.6.0/temporalio/bridge/src/testing.rs`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/src/worker.rs` & `temporalio-1.6.0/temporalio/bridge/src/worker.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 use prost::Message;
 use pyo3::exceptions::{PyException, PyRuntimeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::{PyBytes, PyTuple};
+use std::collections::HashMap;
+use std::collections::HashSet;
 use std::sync::Arc;
 use std::time::Duration;
 use temporal_sdk_core::api::errors::{PollActivityError, PollWfError};
 use temporal_sdk_core::replay::{HistoryForReplay, ReplayWorkerInput};
+use temporal_sdk_core_api::errors::WorkflowErrorType;
 use temporal_sdk_core_api::Worker;
 use temporal_sdk_core_protos::coresdk::workflow_completion::WorkflowActivationCompletion;
 use temporal_sdk_core_protos::coresdk::{ActivityHeartbeat, ActivityTaskCompletion};
 use temporal_sdk_core_protos::temporal::api::history::v1::History;
 use tokio::sync::mpsc::{channel, Sender};
 use tokio_stream::wrappers::ReceiverStream;
 
@@ -41,14 +44,16 @@
     sticky_queue_schedule_to_start_timeout_millis: u64,
     max_heartbeat_throttle_interval_millis: u64,
     default_heartbeat_throttle_interval_millis: u64,
     max_activities_per_second: Option<f64>,
     max_task_queue_activities_per_second: Option<f64>,
     graceful_shutdown_period_millis: u64,
     use_worker_versioning: bool,
+    nondeterminism_as_workflow_fail: bool,
+    nondeterminism_as_workflow_fail_for_types: HashSet<String>,
 }
 
 macro_rules! enter_sync {
     ($runtime:expr) => {
         if let Some(subscriber) = $runtime.core.telemetry().trace_subscriber() {
             temporal_sdk_core::telemetry::set_trace_subscriber_for_current_thread(subscriber);
         }
@@ -175,14 +180,21 @@
         self.worker
             .as_ref()
             .unwrap()
             .request_workflow_eviction(run_id);
         Ok(())
     }
 
+    fn replace_client(&self, client: &client::ClientRef) {
+        self.worker
+            .as_ref()
+            .expect("missing worker")
+            .replace_client(client.retry_client.clone().into_inner());
+    }
+
     fn initiate_shutdown(&self) -> PyResult<()> {
         let worker = self.worker.as_ref().unwrap().clone();
         worker.initiate_shutdown();
         Ok(())
     }
 
     fn finalize_shutdown<'p>(&mut self, py: Python<'p>) -> PyResult<&'p PyAny> {
@@ -230,14 +242,30 @@
             .max_worker_activities_per_second(conf.max_activities_per_second)
             .max_task_queue_activities_per_second(conf.max_task_queue_activities_per_second)
             // Even though grace period is optional, if it is not set then the
             // auto-cancel-activity behavior of shutdown will not occur, so we
             // always set it even if 0.
             .graceful_shutdown_period(Duration::from_millis(conf.graceful_shutdown_period_millis))
             .use_worker_versioning(conf.use_worker_versioning)
+            .workflow_failure_errors(if conf.nondeterminism_as_workflow_fail {
+                HashSet::from([WorkflowErrorType::Nondeterminism])
+            } else {
+                HashSet::new()
+            })
+            .workflow_types_to_failure_errors(
+                conf.nondeterminism_as_workflow_fail_for_types
+                    .iter()
+                    .map(|s| {
+                        (
+                            s.to_owned(),
+                            HashSet::from([WorkflowErrorType::Nondeterminism]),
+                        )
+                    })
+                    .collect::<HashMap<String, HashSet<WorkflowErrorType>>>(),
+            )
             .build()
             .map_err(|err| PyValueError::new_err(format!("Invalid worker config: {}", err)))
     }
 }
 
 /// For feeding histories into core during replay
 #[pyclass]
```

### Comparing `temporalio-1.5.1/temporalio/bridge/testing.py` & `temporalio-1.6.0/temporalio/bridge/testing.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/bridge/worker.py` & `temporalio-1.6.0/temporalio/bridge/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,24 @@
 
 Nothing in this module should be considered stable. The API may change.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Awaitable, Callable, List, Optional, Sequence, Tuple
+from typing import (
+    TYPE_CHECKING,
+    Awaitable,
+    Callable,
+    List,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+)
 
 import google.protobuf.internal.containers
 from typing_extensions import TypeAlias
 
 import temporalio.api.common.v1
 import temporalio.api.history.v1
 import temporalio.bridge.client
@@ -44,14 +53,16 @@
     sticky_queue_schedule_to_start_timeout_millis: int
     max_heartbeat_throttle_interval_millis: int
     default_heartbeat_throttle_interval_millis: int
     max_activities_per_second: Optional[float]
     max_task_queue_activities_per_second: Optional[float]
     graceful_shutdown_period_millis: int
     use_worker_versioning: bool
+    nondeterminism_as_workflow_fail: bool
+    nondeterminism_as_workflow_fail_for_types: Set[str]
 
 
 class Worker:
     """SDK Core worker."""
 
     @staticmethod
     def create(client: temporalio.bridge.client.Client, config: WorkerConfig) -> Worker:
@@ -117,14 +128,18 @@
         """Record an activity heartbeat."""
         self._ref.record_activity_heartbeat(comp.SerializeToString())
 
     def request_workflow_eviction(self, run_id: str) -> None:
         """Request a workflow be evicted."""
         self._ref.request_workflow_eviction(run_id)
 
+    def replace_client(self, client: temporalio.bridge.client.Client) -> None:
+        """Replace the worker client."""
+        self._ref.replace_client(client._ref)
+
     def initiate_shutdown(self) -> None:
         """Start shutdown of the worker."""
         self._ref.initiate_shutdown()
 
     async def finalize_shutdown(self) -> None:
         """Finalize the worker.
```

### Comparing `temporalio-1.5.1/temporalio/client.py` & `temporalio-1.6.0/temporalio/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 import temporalio.common
 import temporalio.converter
 import temporalio.exceptions
 import temporalio.runtime
 import temporalio.service
 import temporalio.workflow
 from temporalio.service import (
+    HttpConnectProxyConfig,
     KeepAliveConfig,
     RetryConfig,
     RPCError,
     RPCStatusCode,
     TLSConfig,
 )
 
@@ -93,33 +94,38 @@
     """
 
     @staticmethod
     async def connect(
         target_host: str,
         *,
         namespace: str = "default",
+        api_key: Optional[str] = None,
         data_converter: temporalio.converter.DataConverter = temporalio.converter.DataConverter.default,
         interceptors: Sequence[Interceptor] = [],
         default_workflow_query_reject_condition: Optional[
             temporalio.common.QueryRejectCondition
         ] = None,
         tls: Union[bool, TLSConfig] = False,
         retry_config: Optional[RetryConfig] = None,
         keep_alive_config: Optional[KeepAliveConfig] = KeepAliveConfig.default,
         rpc_metadata: Mapping[str, str] = {},
         identity: Optional[str] = None,
         lazy: bool = False,
         runtime: Optional[temporalio.runtime.Runtime] = None,
+        http_connect_proxy_config: Optional[HttpConnectProxyConfig] = None,
     ) -> Client:
         """Connect to a Temporal server.
 
         Args:
             target_host: ``host:port`` for the Temporal server. For local
                 development, this is often "localhost:7233".
             namespace: Namespace to use for client calls.
+            api_key: API key for Temporal. This becomes the "Authorization"
+                HTTP header with "Bearer " prepended. This is only set if RPC
+                metadata doesn't already have an "authorization" key.
             data_converter: Data converter to use for all data conversions
                 to/from payloads.
             interceptors: Set of interceptors that are chained together to allow
                 intercepting of client calls. The earlier interceptors wrap the
                 later ones.
 
                 Any interceptors that also implement
@@ -145,24 +151,27 @@
                 can be overriden by per-call RPC metadata keys.
             identity: Identity for this client. If unset, a default is created
                 based on the version of the SDK.
             lazy: If true, the client will not connect until the first call is
                 attempted or a worker is created with it. Lazy clients cannot be
                 used for workers.
             runtime: The runtime for this client, or the default if unset.
+            http_connect_proxy_config: Configuration for HTTP CONNECT proxy.
         """
         connect_config = temporalio.service.ConnectConfig(
             target_host=target_host,
+            api_key=api_key,
             tls=tls,
             retry_config=retry_config,
             keep_alive_config=keep_alive_config,
             rpc_metadata=rpc_metadata,
             identity=identity or "",
             lazy=lazy,
             runtime=runtime,
+            http_connect_proxy_config=http_connect_proxy_config,
         )
         return Client(
             await temporalio.service.ServiceClient.connect(connect_config),
             namespace=namespace,
             data_converter=data_converter,
             interceptors=interceptors,
             default_workflow_query_reject_condition=default_workflow_query_reject_condition,
@@ -257,14 +266,30 @@
         Do not mutate this mapping after set. Rather, set an entirely new
         mapping if changes are needed.
         """
         # Update config and perform update
         self.service_client.config.rpc_metadata = value
         self.service_client.update_rpc_metadata(value)
 
+    @property
+    def api_key(self) -> Optional[str]:
+        """API key for every call made by this client."""
+        return self.service_client.config.api_key
+
+    @api_key.setter
+    def api_key(self, value: Optional[str]) -> None:
+        """Update the API key for this client.
+
+        This is only set if RPCmetadata doesn't already have an "authorization"
+        key.
+        """
+        # Update config and perform update
+        self.service_client.config.api_key = value
+        self.service_client.update_api_key(value)
+
     # Overload for no-param workflow
     @overload
     async def start_workflow(
         self,
         workflow: MethodAsyncNoParam[SelfType, ReturnType],
         *,
         id: str,
@@ -437,16 +462,15 @@
             retry_policy: Retry policy for the workflow.
             cron_schedule: See https://docs.temporal.io/docs/content/what-is-a-temporal-cron-job/
             memo: Memo for the workflow.
             search_attributes: Search attributes for the workflow. The
                 dictionary form of this is deprecated, use
                 :py:class:`temporalio.common.TypedSearchAttributes`.
             start_delay: Amount of time to wait before starting the workflow.
-                This does not work with ``cron_schedule``. This is currently
-                experimental.
+                This does not work with ``cron_schedule``.
             start_signal: If present, this signal is sent as signal-with-start
                 instead of traditional workflow start.
             start_signal_args: Arguments for start_signal if start_signal
                 present.
             rpc_metadata: Headers used on the RPC call. Keys here override
                 client-level RPC metadata keys.
             rpc_timeout: Optional RPC deadline to set for the RPC call.
@@ -791,14 +815,38 @@
                 page_size=page_size,
                 next_page_token=next_page_token,
                 rpc_metadata=rpc_metadata,
                 rpc_timeout=rpc_timeout,
             )
         )
 
+    async def count_workflows(
+        self,
+        query: Optional[str] = None,
+        rpc_metadata: Mapping[str, str] = {},
+        rpc_timeout: Optional[timedelta] = None,
+    ) -> WorkflowExecutionCount:
+        """Count workflows.
+
+        Args:
+            query: A Temporal visibility filter. See Temporal documentation
+                concerning visibility list filters.
+            rpc_metadata: Headers used on each RPC call. Keys here override
+                client-level RPC metadata keys.
+            rpc_timeout: Optional RPC deadline to set for each RPC call.
+
+        Returns:
+            Count of workflows.
+        """
+        return await self._impl.count_workflows(
+            CountWorkflowsInput(
+                query=query, rpc_metadata=rpc_metadata, rpc_timeout=rpc_timeout
+            )
+        )
+
     @overload
     def get_async_activity_handle(
         self, *, workflow_id: str, run_id: Optional[str], activity_id: str
     ) -> AsyncActivityHandle:
         pass
 
     @overload
@@ -2282,14 +2330,65 @@
         temporalio.api.enums.v1.WorkflowExecutionStatus.WORKFLOW_EXECUTION_STATUS_CONTINUED_AS_NEW
     )
     TIMED_OUT = int(
         temporalio.api.enums.v1.WorkflowExecutionStatus.WORKFLOW_EXECUTION_STATUS_TIMED_OUT
     )
 
 
+@dataclass
+class WorkflowExecutionCount:
+    """Representation of a count from a count workflows call."""
+
+    count: int
+    """Approximate number of workflows matching the original query.
+    
+    If the query had a group-by clause, this is simply the sum of all the counts
+    in py:attr:`groups`.
+    """
+
+    groups: Sequence[WorkflowExecutionCountAggregationGroup]
+    """Groups if the query had a group-by clause, or empty if not."""
+
+    @staticmethod
+    def _from_raw(
+        raw: temporalio.api.workflowservice.v1.CountWorkflowExecutionsResponse,
+    ) -> WorkflowExecutionCount:
+        return WorkflowExecutionCount(
+            count=raw.count,
+            groups=[
+                WorkflowExecutionCountAggregationGroup._from_raw(g) for g in raw.groups
+            ],
+        )
+
+
+@dataclass
+class WorkflowExecutionCountAggregationGroup:
+    """Aggregation group if the workflow count query had a group-by clause."""
+
+    count: int
+    """Approximate number of workflows matching the original query for this
+    group.
+    """
+
+    group_values: Sequence[temporalio.common.SearchAttributeValue]
+    """Search attribute values for this group."""
+
+    @staticmethod
+    def _from_raw(
+        raw: temporalio.api.workflowservice.v1.CountWorkflowExecutionsResponse.AggregationGroup,
+    ) -> WorkflowExecutionCountAggregationGroup:
+        return WorkflowExecutionCountAggregationGroup(
+            count=raw.count,
+            group_values=[
+                temporalio.converter._decode_search_attribute_value(v)
+                for v in raw.group_values
+            ],
+        )
+
+
 class WorkflowExecutionAsyncIterator:
     """Asynchronous iterator for :py:class:`WorkflowExecution` values.
 
     Most users should use ``async for`` on this iterator and not call any of the
     methods within. To consume the workflows as histories, call
     :py:meth:`map_histories`.
     """
@@ -4346,14 +4445,23 @@
     page_size: int
     next_page_token: Optional[bytes]
     rpc_metadata: Mapping[str, str]
     rpc_timeout: Optional[timedelta]
 
 
 @dataclass
+class CountWorkflowsInput:
+    """Input for :py:meth:`OutboundInterceptor.count_workflows`."""
+
+    query: Optional[str]
+    rpc_metadata: Mapping[str, str]
+    rpc_timeout: Optional[timedelta]
+
+
+@dataclass
 class QueryWorkflowInput:
     """Input for :py:meth:`OutboundInterceptor.query_workflow`."""
 
     id: str
     run_id: Optional[str]
     query: str
     args: Sequence[Any]
@@ -4641,14 +4749,20 @@
 
     def list_workflows(
         self, input: ListWorkflowsInput
     ) -> WorkflowExecutionAsyncIterator:
         """Called for every :py:meth:`Client.list_workflows` call."""
         return self.next.list_workflows(input)
 
+    async def count_workflows(
+        self, input: CountWorkflowsInput
+    ) -> WorkflowExecutionCount:
+        """Called for every :py:meth:`Client.count_workflows` call."""
+        return await self.next.count_workflows(input)
+
     async def query_workflow(self, input: QueryWorkflowInput) -> Any:
         """Called for every :py:meth:`WorkflowHandle.query` call."""
         return await self.next.query_workflow(input)
 
     async def signal_workflow(self, input: SignalWorkflowInput) -> None:
         """Called for every :py:meth:`WorkflowHandle.signal` call."""
         await self.next.signal_workflow(input)
@@ -4900,14 +5014,29 @@
         return WorkflowHistoryEventAsyncIterator(self._client, input)
 
     def list_workflows(
         self, input: ListWorkflowsInput
     ) -> WorkflowExecutionAsyncIterator:
         return WorkflowExecutionAsyncIterator(self._client, input)
 
+    async def count_workflows(
+        self, input: CountWorkflowsInput
+    ) -> WorkflowExecutionCount:
+        return WorkflowExecutionCount._from_raw(
+            await self._client.workflow_service.count_workflow_executions(
+                temporalio.api.workflowservice.v1.CountWorkflowExecutionsRequest(
+                    namespace=self._client.namespace,
+                    query=input.query or "",
+                ),
+                retry=True,
+                metadata=input.rpc_metadata,
+                timeout=input.rpc_timeout,
+            )
+        )
+
     async def query_workflow(self, input: QueryWorkflowInput) -> Any:
         req = temporalio.api.workflowservice.v1.QueryWorkflowRequest(
             namespace=self._client.namespace,
             execution=temporalio.api.common.v1.WorkflowExecution(
                 workflow_id=input.id,
                 run_id=input.run_id or "",
             ),
```

### Comparing `temporalio-1.5.1/temporalio/common.py` & `temporalio-1.6.0/temporalio/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     TypeVar,
     Union,
     get_type_hints,
     overload,
 )
 
 import google.protobuf.internal.containers
-from typing_extensions import ClassVar, NamedTuple, TypeAlias, get_origin
+from typing_extensions import ClassVar, NamedTuple, Self, TypeAlias, get_origin
 
 import temporalio.api.common.v1
 import temporalio.api.enums.v1
 import temporalio.types
 
 
 @dataclass
@@ -574,14 +574,49 @@
 
         Returns:
             Histogram metric.
         """
         ...
 
     @abstractmethod
+    def create_histogram_float(
+        self, name: str, description: Optional[str] = None, unit: Optional[str] = None
+    ) -> MetricHistogramFloat:
+        """Create a histogram metric for recording values.
+
+        Args:
+            name: Name for the metric.
+            description: Optional description for the metric.
+            unit: Optional unit for the metric.
+
+        Returns:
+            Histogram metric.
+        """
+        ...
+
+    @abstractmethod
+    def create_histogram_timedelta(
+        self, name: str, description: Optional[str] = None, unit: Optional[str] = None
+    ) -> MetricHistogramTimedelta:
+        """Create a histogram metric for recording values.
+
+        Note, duration precision is millisecond. Also note, if "unit" is set as
+        "duration", it will be converted to "ms" or "s" on the way out.
+
+        Args:
+            name: Name for the metric.
+            description: Optional description for the metric.
+            unit: Optional unit for the metric.
+
+        Returns:
+            Histogram metric.
+        """
+        ...
+
+    @abstractmethod
     def create_gauge(
         self, name: str, description: Optional[str] = None, unit: Optional[str] = None
     ) -> MetricGauge:
         """Create a gauge metric for setting values.
 
         Args:
             name: Name for the metric.
@@ -590,14 +625,30 @@
 
         Returns:
             Gauge metric.
         """
         ...
 
     @abstractmethod
+    def create_gauge_float(
+        self, name: str, description: Optional[str] = None, unit: Optional[str] = None
+    ) -> MetricGaugeFloat:
+        """Create a gauge metric for setting values.
+
+        Args:
+            name: Name for the metric.
+            description: Optional description for the metric.
+            unit: Optional unit for the metric.
+
+        Returns:
+            Gauge metric.
+        """
+        ...
+
+    @abstractmethod
     def with_additional_attributes(
         self, additional_attributes: MetricAttributes
     ) -> MetricMeter:
         """Create a new metric meter with the given attributes appended to the
         current set.
 
         Args:
@@ -609,16 +660,16 @@
 
         Raises:
             TypeError: Attribute values are not the expected type.
         """
         ...
 
 
-class MetricCounter(ABC):
-    """Counter metric created by a metric meter."""
+class MetricCommon(ABC):
+    """Base for all metrics."""
 
     @property
     @abstractmethod
     def name(self) -> str:
         """Name for the metric."""
         ...
 
@@ -631,71 +682,57 @@
     @property
     @abstractmethod
     def unit(self) -> Optional[str]:
         """Unit for the metric if any."""
         ...
 
     @abstractmethod
-    def add(
-        self, value: int, additional_attributes: Optional[MetricAttributes] = None
-    ) -> None:
-        """Add a value to the counter.
+    def with_additional_attributes(
+        self, additional_attributes: MetricAttributes
+    ) -> Self:
+        """Create a new metric with the given attributes appended to the
+        current set.
 
         Args:
-            value: A non-negative integer to add.
             additional_attributes: Additional attributes to append to the
                 current set.
 
+        Returns:
+            New metric.
+
         Raises:
-            ValueError: Value is negative.
             TypeError: Attribute values are not the expected type.
         """
         ...
 
+
+class MetricCounter(MetricCommon):
+    """Counter metric created by a metric meter."""
+
     @abstractmethod
-    def with_additional_attributes(
-        self, additional_attributes: MetricAttributes
-    ) -> MetricCounter:
-        """Create a new counter with the given attributes appended to the
-        current set.
+    def add(
+        self, value: int, additional_attributes: Optional[MetricAttributes] = None
+    ) -> None:
+        """Add a value to the counter.
 
         Args:
+            value: A non-negative integer to add.
             additional_attributes: Additional attributes to append to the
                 current set.
 
-        Returns:
-            New counter.
-
         Raises:
+            ValueError: Value is negative.
             TypeError: Attribute values are not the expected type.
         """
         ...
 
 
-class MetricHistogram(ABC):
+class MetricHistogram(MetricCommon):
     """Histogram metric created by a metric meter."""
 
-    @property
-    @abstractmethod
-    def name(self) -> str:
-        """Name for the metric."""
-        ...
-
-    @property
-    @abstractmethod
-    def description(self) -> Optional[str]:
-        """Description for the metric if any."""
-        ...
-
-    @property
-    @abstractmethod
-    def unit(self) -> Optional[str]:
-        """Unit for the metric if any."""
-        ...
-
     @abstractmethod
     def record(
         self, value: int, additional_attributes: Optional[MetricAttributes] = None
     ) -> None:
         """Record a value on the histogram.
 
         Args:
@@ -705,55 +742,62 @@
 
         Raises:
             ValueError: Value is negative.
             TypeError: Attribute values are not the expected type.
         """
         ...
 
+
+class MetricHistogramFloat(MetricCommon):
+    """Histogram metric created by a metric meter."""
+
     @abstractmethod
-    def with_additional_attributes(
-        self, additional_attributes: MetricAttributes
-    ) -> MetricHistogram:
-        """Create a new histogram with the given attributes appended to the
-        current set.
+    def record(
+        self, value: float, additional_attributes: Optional[MetricAttributes] = None
+    ) -> None:
+        """Record a value on the histogram.
 
         Args:
+            value: A non-negative float to record.
             additional_attributes: Additional attributes to append to the
                 current set.
 
-        Returns:
-            New histogram.
-
         Raises:
+            ValueError: Value is negative.
             TypeError: Attribute values are not the expected type.
         """
         ...
 
 
-class MetricGauge(ABC):
-    """Gauge metric created by a metric meter."""
+class MetricHistogramTimedelta(MetricCommon):
+    """Histogram metric created by a metric meter."""
 
-    @property
     @abstractmethod
-    def name(self) -> str:
-        """Name for the metric."""
-        ...
+    def record(
+        self, value: timedelta, additional_attributes: Optional[MetricAttributes] = None
+    ) -> None:
+        """Record a value on the histogram.
 
-    @property
-    @abstractmethod
-    def description(self) -> Optional[str]:
-        """Description for the metric if any."""
-        ...
+        Note, duration precision is millisecond.
 
-    @property
-    @abstractmethod
-    def unit(self) -> Optional[str]:
-        """Unit for the metric if any."""
+        Args:
+            value: A non-negative timedelta to record.
+            additional_attributes: Additional attributes to append to the
+                current set.
+
+        Raises:
+            ValueError: Value is negative.
+            TypeError: Attribute values are not the expected type.
+        """
         ...
 
+
+class MetricGauge(MetricCommon):
+    """Gauge metric created by a metric meter."""
+
     @abstractmethod
     def set(
         self, value: int, additional_attributes: Optional[MetricAttributes] = None
     ) -> None:
         """Set a value on the gauge.
 
         Args:
@@ -763,29 +807,31 @@
 
         Raises:
             ValueError: Value is negative.
             TypeError: Attribute values are not the expected type.
         """
         ...
 
+
+class MetricGaugeFloat(MetricCommon):
+    """Gauge metric created by a metric meter."""
+
     @abstractmethod
-    def with_additional_attributes(
-        self, additional_attributes: MetricAttributes
-    ) -> MetricGauge:
-        """Create a new gauge with the given attributes appended to the
-        current set.
+    def set(
+        self, value: float, additional_attributes: Optional[MetricAttributes] = None
+    ) -> None:
+        """Set a value on the gauge.
 
         Args:
+            value: A non-negative float to set.
             additional_attributes: Additional attributes to append to the
                 current set.
 
-        Returns:
-            New gauge.
-
         Raises:
+            ValueError: Value is negative.
             TypeError: Attribute values are not the expected type.
         """
         ...
 
 
 class _NoopMetricMeter(MetricMeter):
     def create_counter(
@@ -794,26 +840,41 @@
         return _NoopMetricCounter(name, description, unit)
 
     def create_histogram(
         self, name: str, description: Optional[str] = None, unit: Optional[str] = None
     ) -> MetricHistogram:
         return _NoopMetricHistogram(name, description, unit)
 
+    def create_histogram_float(
+        self, name: str, description: Optional[str] = None, unit: Optional[str] = None
+    ) -> MetricHistogramFloat:
+        return _NoopMetricHistogramFloat(name, description, unit)
+
+    def create_histogram_timedelta(
+        self, name: str, description: Optional[str] = None, unit: Optional[str] = None
+    ) -> MetricHistogramTimedelta:
+        return _NoopMetricHistogramTimedelta(name, description, unit)
+
     def create_gauge(
         self, name: str, description: Optional[str] = None, unit: Optional[str] = None
     ) -> MetricGauge:
         return _NoopMetricGauge(name, description, unit)
 
+    def create_gauge_float(
+        self, name: str, description: Optional[str] = None, unit: Optional[str] = None
+    ) -> MetricGaugeFloat:
+        return _NoopMetricGaugeFloat(name, description, unit)
+
     def with_additional_attributes(
         self, additional_attributes: MetricAttributes
     ) -> MetricMeter:
         return self
 
 
-class _NoopMetric:
+class _NoopMetric(MetricCommon):
     def __init__(
         self, name: str, description: Optional[str], unit: Optional[str]
     ) -> None:
         self._name = name
         self._description = description
         self._unit = unit
 
@@ -825,49 +886,60 @@
     def description(self) -> Optional[str]:
         return self._description
 
     @property
     def unit(self) -> Optional[str]:
         return self._unit
 
+    def with_additional_attributes(
+        self, additional_attributes: MetricAttributes
+    ) -> Self:
+        return self
 
-class _NoopMetricCounter(_NoopMetric, MetricCounter):
+
+class _NoopMetricCounter(MetricCounter, _NoopMetric):
     def add(
         self, value: int, additional_attributes: Optional[MetricAttributes] = None
     ) -> None:
         pass
 
-    def with_additional_attributes(
-        self, additional_attributes: MetricAttributes
-    ) -> MetricCounter:
-        return self
-
 
-class _NoopMetricHistogram(_NoopMetric, MetricHistogram):
+class _NoopMetricHistogram(MetricHistogram, _NoopMetric):
     def record(
         self, value: int, additional_attributes: Optional[MetricAttributes] = None
     ) -> None:
         pass
 
-    def with_additional_attributes(
-        self, additional_attributes: MetricAttributes
-    ) -> MetricHistogram:
-        return self
+
+class _NoopMetricHistogramFloat(MetricHistogramFloat, _NoopMetric):
+    def record(
+        self, value: float, additional_attributes: Optional[MetricAttributes] = None
+    ) -> None:
+        pass
+
+
+class _NoopMetricHistogramTimedelta(MetricHistogramTimedelta, _NoopMetric):
+    def record(
+        self, value: timedelta, additional_attributes: Optional[MetricAttributes] = None
+    ) -> None:
+        pass
 
 
-class _NoopMetricGauge(_NoopMetric, MetricGauge):
+class _NoopMetricGauge(MetricGauge, _NoopMetric):
     def set(
         self, value: int, additional_attributes: Optional[MetricAttributes] = None
     ) -> None:
         pass
 
-    def with_additional_attributes(
-        self, additional_attributes: MetricAttributes
-    ) -> MetricGauge:
-        return self
+
+class _NoopMetricGaugeFloat(MetricGaugeFloat, _NoopMetric):
+    def set(
+        self, value: float, additional_attributes: Optional[MetricAttributes] = None
+    ) -> None:
+        pass
 
 
 MetricMeter.noop = _NoopMetricMeter()
 
 # Should be set as the "arg" argument for _arg_or_args checks where the argument
 # is unset. This is different than None which is a legitimate argument.
 _arg_unset = object()
```

### Comparing `temporalio-1.5.1/temporalio/contrib/opentelemetry.py` & `temporalio-1.6.0/temporalio/contrib/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/converter.py` & `temporalio-1.6.0/temporalio/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1337,14 +1337,23 @@
             val = parser(val)
         # If the value isn't the right type, we need to ignore
         if isinstance(val, key.origin_value_type):
             pairs.append(temporalio.common.SearchAttributePair(key, val))
     return temporalio.common.TypedSearchAttributes(pairs)
 
 
+def _decode_search_attribute_value(
+    payload: temporalio.api.common.v1.Payload,
+) -> temporalio.common.SearchAttributeValue:
+    val = default().payload_converter.from_payload(payload)
+    if isinstance(val, str) and payload.metadata.get("type") == b"Datetime":
+        val = _get_iso_datetime_parser()(val)
+    return val  # type: ignore
+
+
 def value_to_type(
     hint: Type,
     value: Any,
     custom_converters: Sequence[JSONTypeConverter] = [],
 ) -> Any:
     """Convert a given value to the given type hint.
```

### Comparing `temporalio-1.5.1/temporalio/exceptions.py` & `temporalio-1.6.0/temporalio/exceptions.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/runtime.py` & `temporalio-1.6.0/temporalio/runtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,26 @@
 from __future__ import annotations
 
 import logging
 import time
 from dataclasses import dataclass, field
 from datetime import timedelta
 from enum import Enum
-from typing import ClassVar, Mapping, NewType, Optional, Sequence, Union
+from typing import (
+    ClassVar,
+    Generic,
+    Mapping,
+    NewType,
+    Optional,
+    Sequence,
+    TypeVar,
+    Union,
+)
 
-from typing_extensions import Protocol
+from typing_extensions import Protocol, Self
 
 import temporalio.bridge.metric
 import temporalio.bridge.runtime
 import temporalio.common
 
 _default_runtime: Optional[Runtime] = None
 
@@ -245,81 +254,105 @@
 
     url: str
     headers: Optional[Mapping[str, str]] = None
     metric_periodicity: Optional[timedelta] = None
     metric_temporality: OpenTelemetryMetricTemporality = (
         OpenTelemetryMetricTemporality.CUMULATIVE
     )
+    durations_as_seconds: bool = False
 
     def _to_bridge_config(self) -> temporalio.bridge.runtime.OpenTelemetryConfig:
         return temporalio.bridge.runtime.OpenTelemetryConfig(
             url=self.url,
             headers=self.headers or {},
             metric_periodicity_millis=None
             if not self.metric_periodicity
             else round(self.metric_periodicity.total_seconds() * 1000),
             metric_temporality_delta=self.metric_temporality
             == OpenTelemetryMetricTemporality.DELTA,
+            durations_as_seconds=self.durations_as_seconds,
         )
 
 
 @dataclass(frozen=True)
 class PrometheusConfig:
     """Configuration for Prometheus metrics endpoint."""
 
     bind_address: str
     counters_total_suffix: bool = False
     unit_suffix: bool = False
+    durations_as_seconds: bool = False
 
     def _to_bridge_config(self) -> temporalio.bridge.runtime.PrometheusConfig:
         return temporalio.bridge.runtime.PrometheusConfig(
             bind_address=self.bind_address,
             counters_total_suffix=self.counters_total_suffix,
             unit_suffix=self.unit_suffix,
+            durations_as_seconds=self.durations_as_seconds,
         )
 
 
+class MetricBufferDurationFormat(Enum):
+    """How durations are represented for metrics buffers."""
+
+    MILLISECONDS = 1
+    """Durations are millisecond integers."""
+
+    SECONDS = 2
+    """Durations are second floats."""
+
+
 class MetricBuffer:
     """A buffer that can be set on :py:class:`TelemetryConfig` to record
     metrics instead of ignoring/exporting them.
 
     .. warning::
         It is important that the buffer size is set to a high number and that
         :py:meth:`retrieve_updates` is called regularly to drain the buffer. If
         the buffer is full, metric updates will be dropped and an error will be
         logged.
     """
 
-    def __init__(self, buffer_size: int) -> None:
+    def __init__(
+        self,
+        buffer_size: int,
+        duration_format: MetricBufferDurationFormat = MetricBufferDurationFormat.MILLISECONDS,
+    ) -> None:
         """Create a buffer with the given size.
 
         .. warning::
             It is important that the buffer size is set to a high number and is
             drained regularly. See :py:class:`MetricBuffer` warning.
 
         Args:
             buffer_size: Size of the buffer. Set this to a large value. A value
                 in the tens of thousands or higher is plenty reasonable.
+            duration_format: Which duration format to use.
         """
         self._buffer_size = buffer_size
         self._runtime: Optional[Runtime] = None
+        self._durations_as_seconds = (
+            duration_format == MetricBufferDurationFormat.SECONDS
+        )
 
     def retrieve_updates(self) -> Sequence[BufferedMetricUpdate]:
         """Drain the buffer and return all metric updates.
 
         .. warning::
             It is important that this is called regularly. See
             :py:class:`MetricBuffer` warning.
 
         Returns:
             A sequence of metric updates.
         """
         if not self._runtime:
             raise RuntimeError("Attempting to retrieve updates before runtime created")
-        return self._runtime._core_runtime.retrieve_buffered_metrics()
+        return self._runtime._core_runtime.retrieve_buffered_metrics(
+            self._durations_as_seconds
+        )
 
 
 @dataclass(frozen=True)
 class TelemetryConfig:
     """Configuration for Core telemetry."""
 
     logging: Optional[LoggingConfig] = LoggingConfig.default
@@ -477,43 +510,85 @@
             unit,
             temporalio.bridge.metric.MetricHistogram(
                 self._core_meter, name, description, unit
             ),
             self._core_attrs,
         )
 
+    def create_histogram_float(
+        self, name: str, description: Optional[str] = None, unit: Optional[str] = None
+    ) -> temporalio.common.MetricHistogramFloat:
+        return _MetricHistogramFloat(
+            name,
+            description,
+            unit,
+            temporalio.bridge.metric.MetricHistogramFloat(
+                self._core_meter, name, description, unit
+            ),
+            self._core_attrs,
+        )
+
+    def create_histogram_timedelta(
+        self, name: str, description: Optional[str] = None, unit: Optional[str] = None
+    ) -> temporalio.common.MetricHistogramTimedelta:
+        return _MetricHistogramTimedelta(
+            name,
+            description,
+            unit,
+            temporalio.bridge.metric.MetricHistogramDuration(
+                self._core_meter, name, description, unit
+            ),
+            self._core_attrs,
+        )
+
     def create_gauge(
         self, name: str, description: Optional[str] = None, unit: Optional[str] = None
     ) -> temporalio.common.MetricGauge:
         return _MetricGauge(
             name,
             description,
             unit,
             temporalio.bridge.metric.MetricGauge(
                 self._core_meter, name, description, unit
             ),
             self._core_attrs,
         )
 
+    def create_gauge_float(
+        self, name: str, description: Optional[str] = None, unit: Optional[str] = None
+    ) -> temporalio.common.MetricGaugeFloat:
+        return _MetricGaugeFloat(
+            name,
+            description,
+            unit,
+            temporalio.bridge.metric.MetricGaugeFloat(
+                self._core_meter, name, description, unit
+            ),
+            self._core_attrs,
+        )
+
     def with_additional_attributes(
         self, additional_attributes: temporalio.common.MetricAttributes
     ) -> temporalio.common.MetricMeter:
         return _MetricMeter(
             self._core_meter,
             self._core_attrs.with_additional_attributes(additional_attributes),
         )
 
 
-class _MetricCounter(temporalio.common.MetricCounter):
+_CoreMetricType = TypeVar("_CoreMetricType")
+
+
+class _MetricCommon(temporalio.common.MetricCommon, Generic[_CoreMetricType]):
     def __init__(
         self,
         name: str,
         description: Optional[str],
         unit: Optional[str],
-        core_metric: temporalio.bridge.metric.MetricCounter,
+        core_metric: _CoreMetricType,
         core_attrs: temporalio.bridge.metric.MetricAttributes,
     ) -> None:
         self._name = name
         self._description = description
         self._unit = unit
         self._core_metric = core_metric
         self._core_attrs = core_attrs
@@ -526,131 +601,123 @@
     def description(self) -> Optional[str]:
         return self._description
 
     @property
     def unit(self) -> Optional[str]:
         return self._unit
 
-    def add(
-        self,
-        value: int,
-        additional_attributes: Optional[temporalio.common.MetricAttributes] = None,
-    ) -> None:
-        if value < 0:
-            raise ValueError("Metric value cannot be negative")
-        core_attrs = self._core_attrs
-        if additional_attributes:
-            core_attrs = core_attrs.with_additional_attributes(additional_attributes)
-        self._core_metric.add(value, core_attrs)
-
     def with_additional_attributes(
         self, additional_attributes: temporalio.common.MetricAttributes
-    ) -> temporalio.common.MetricCounter:
-        return _MetricCounter(
+    ) -> Self:
+        return self.__class__(
             self._name,
             self._description,
             self._unit,
             self._core_metric,
             self._core_attrs.with_additional_attributes(additional_attributes),
         )
 
 
-class _MetricHistogram(temporalio.common.MetricHistogram):
-    def __init__(
+class _MetricCounter(
+    temporalio.common.MetricCounter,
+    _MetricCommon[temporalio.bridge.metric.MetricCounter],
+):
+    def add(
         self,
-        name: str,
-        description: Optional[str],
-        unit: Optional[str],
-        core_metric: temporalio.bridge.metric.MetricHistogram,
-        core_attrs: temporalio.bridge.metric.MetricAttributes,
+        value: int,
+        additional_attributes: Optional[temporalio.common.MetricAttributes] = None,
     ) -> None:
-        self._name = name
-        self._description = description
-        self._unit = unit
-        self._core_metric = core_metric
-        self._core_attrs = core_attrs
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @property
-    def description(self) -> Optional[str]:
-        return self._description
+        if value < 0:
+            raise ValueError("Metric value cannot be negative")
+        core_attrs = self._core_attrs
+        if additional_attributes:
+            core_attrs = core_attrs.with_additional_attributes(additional_attributes)
+        self._core_metric.add(value, core_attrs)
 
-    @property
-    def unit(self) -> Optional[str]:
-        return self._unit
 
+class _MetricHistogram(
+    temporalio.common.MetricHistogram,
+    _MetricCommon[temporalio.bridge.metric.MetricHistogram],
+):
     def record(
         self,
         value: int,
         additional_attributes: Optional[temporalio.common.MetricAttributes] = None,
     ) -> None:
         if value < 0:
             raise ValueError("Metric value cannot be negative")
         core_attrs = self._core_attrs
         if additional_attributes:
             core_attrs = core_attrs.with_additional_attributes(additional_attributes)
         self._core_metric.record(value, core_attrs)
 
-    def with_additional_attributes(
-        self, additional_attributes: temporalio.common.MetricAttributes
-    ) -> temporalio.common.MetricHistogram:
-        return _MetricHistogram(
-            self._name,
-            self._description,
-            self._unit,
-            self._core_metric,
-            self._core_attrs.with_additional_attributes(additional_attributes),
-        )
 
-
-class _MetricGauge(temporalio.common.MetricGauge):
-    def __init__(
+class _MetricHistogramFloat(
+    temporalio.common.MetricHistogramFloat,
+    _MetricCommon[temporalio.bridge.metric.MetricHistogramFloat],
+):
+    def record(
         self,
-        name: str,
-        description: Optional[str],
-        unit: Optional[str],
-        core_metric: temporalio.bridge.metric.MetricGauge,
-        core_attrs: temporalio.bridge.metric.MetricAttributes,
+        value: float,
+        additional_attributes: Optional[temporalio.common.MetricAttributes] = None,
     ) -> None:
-        self._name = name
-        self._description = description
-        self._unit = unit
-        self._core_metric = core_metric
-        self._core_attrs = core_attrs
+        if value < 0:
+            raise ValueError("Metric value cannot be negative")
+        core_attrs = self._core_attrs
+        if additional_attributes:
+            core_attrs = core_attrs.with_additional_attributes(additional_attributes)
+        self._core_metric.record(value, core_attrs)
 
-    @property
-    def name(self) -> str:
-        return self._name
 
-    @property
-    def description(self) -> Optional[str]:
-        return self._description
+class _MetricHistogramTimedelta(
+    temporalio.common.MetricHistogramTimedelta,
+    _MetricCommon[temporalio.bridge.metric.MetricHistogramDuration],
+):
+    def record(
+        self,
+        value: timedelta,
+        additional_attributes: Optional[temporalio.common.MetricAttributes] = None,
+    ) -> None:
+        if value.days < 0:
+            raise ValueError("Metric value cannot be negative")
+        core_attrs = self._core_attrs
+        if additional_attributes:
+            core_attrs = core_attrs.with_additional_attributes(additional_attributes)
+        self._core_metric.record(
+            (value.days * 86400 * 1000)
+            + (value.seconds * 1000)
+            + (value.microseconds // 1000),
+            core_attrs,
+        )
 
-    @property
-    def unit(self) -> Optional[str]:
-        return self._unit
 
+class _MetricGauge(
+    temporalio.common.MetricGauge, _MetricCommon[temporalio.bridge.metric.MetricGauge]
+):
     def set(
         self,
         value: int,
         additional_attributes: Optional[temporalio.common.MetricAttributes] = None,
     ) -> None:
         if value < 0:
             raise ValueError("Metric value cannot be negative")
         core_attrs = self._core_attrs
         if additional_attributes:
             core_attrs = core_attrs.with_additional_attributes(additional_attributes)
         self._core_metric.set(value, core_attrs)
 
-    def with_additional_attributes(
-        self, additional_attributes: temporalio.common.MetricAttributes
-    ) -> temporalio.common.MetricGauge:
-        return _MetricGauge(
-            self._name,
-            self._description,
-            self._unit,
-            self._core_metric,
-            self._core_attrs.with_additional_attributes(additional_attributes),
-        )
+
+class _MetricGaugeFloat(
+    temporalio.common.MetricGaugeFloat,
+    _MetricCommon[temporalio.bridge.metric.MetricGaugeFloat],
+):
+    def set(
+        self,
+        value: float,
+        additional_attributes: Optional[temporalio.common.MetricAttributes] = None,
+    ) -> None:
+        if value < 0:
+            raise ValueError("Metric value cannot be negative")
+        core_attrs = self._core_attrs
+        if additional_attributes:
+            core_attrs = core_attrs.with_additional_attributes(additional_attributes)
+        self._core_metric.set(value, core_attrs)
```

### Comparing `temporalio-1.5.1/temporalio/service.py` & `temporalio-1.6.0/temporalio/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 import os
 import socket
 import warnings
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from datetime import timedelta
 from enum import IntEnum
-from typing import ClassVar, Generic, Mapping, Optional, Type, TypeVar, Union
+from typing import ClassVar, Generic, Mapping, Optional, Tuple, Type, TypeVar, Union
 
 import google.protobuf.empty_pb2
 import google.protobuf.message
 
 import temporalio.api.common.v1
 import temporalio.api.operatorservice.v1
 import temporalio.api.testservice.v1
 import temporalio.api.workflowservice.v1
 import temporalio.bridge.client
 import temporalio.bridge.proto.health.v1
 import temporalio.exceptions
 import temporalio.runtime
 
-__version__ = "1.5.1"
+__version__ = "1.6.0"
 
 ServiceRequest = TypeVar("ServiceRequest", bound=google.protobuf.message.Message)
 ServiceResponse = TypeVar("ServiceResponse", bound=google.protobuf.message.Message)
 
 logger = logging.getLogger(__name__)
 
 # Set to true to log all requests and responses
@@ -111,26 +111,46 @@
             timeout_millis=self.timeout_millis,
         )
 
 
 KeepAliveConfig.default = KeepAliveConfig()
 
 
+@dataclass(frozen=True)
+class HttpConnectProxyConfig:
+    """Configuration for HTTP CONNECT proxy for client connections."""
+
+    target_host: str
+    """Target host:port for the HTTP CONNECT proxy."""
+    basic_auth: Optional[Tuple[str, str]] = None
+    """Basic auth for the HTTP CONNECT proxy if any as a user/pass tuple."""
+
+    def _to_bridge_config(
+        self,
+    ) -> temporalio.bridge.client.ClientHttpConnectProxyConfig:
+        return temporalio.bridge.client.ClientHttpConnectProxyConfig(
+            target_host=self.target_host,
+            basic_auth=self.basic_auth,
+        )
+
+
 @dataclass
 class ConnectConfig:
     """Config for connecting to the server."""
 
     target_host: str
+    api_key: Optional[str] = None
     tls: Union[bool, TLSConfig] = False
     retry_config: Optional[RetryConfig] = None
     keep_alive_config: Optional[KeepAliveConfig] = KeepAliveConfig.default
     rpc_metadata: Mapping[str, str] = field(default_factory=dict)
     identity: str = ""
     lazy: bool = False
     runtime: Optional[temporalio.runtime.Runtime] = None
+    http_connect_proxy_config: Optional[HttpConnectProxyConfig] = None
 
     def __post_init__(self) -> None:
         """Set extra defaults on unset properties."""
         if not self.identity:
             self.identity = f"{os.getpid()}@{socket.gethostname()}"
 
     def _to_bridge_config(self) -> temporalio.bridge.client.ClientConfig:
@@ -157,25 +177,29 @@
             tls_config = TLSConfig()._to_bridge_config()
         else:
             target_url = f"http://{self.target_host}"
             tls_config = None
 
         return temporalio.bridge.client.ClientConfig(
             target_url=target_url,
+            api_key=self.api_key,
             tls_config=tls_config,
             retry_config=self.retry_config._to_bridge_config()
             if self.retry_config
             else None,
             keep_alive_config=self.keep_alive_config._to_bridge_config()
             if self.keep_alive_config
             else None,
             metadata=self.rpc_metadata,
             identity=self.identity,
             client_name="temporal-python",
             client_version=__version__,
+            http_connect_proxy_config=self.http_connect_proxy_config._to_bridge_config()
+            if self.http_connect_proxy_config
+            else None,
         )
 
 
 class ServiceClient(ABC):
     """Direct client to Temporal services."""
 
     @staticmethod
@@ -235,14 +259,19 @@
 
     @abstractmethod
     def update_rpc_metadata(self, metadata: Mapping[str, str]) -> None:
         """Update service client's RPC metadata."""
         raise NotImplementedError
 
     @abstractmethod
+    def update_api_key(self, api_key: Optional[str]) -> None:
+        """Update service client's API key."""
+        raise NotImplementedError
+
+    @abstractmethod
     async def _rpc_call(
         self,
         rpc: str,
         req: google.protobuf.message.Message,
         resp_type: Type[ServiceResponse],
         *,
         service: str,
@@ -736,14 +765,22 @@
         """Update Core client metadata."""
         # Mutate the bridge config and then only mutate the running client
         # metadata if already connected
         self._bridge_config.metadata = metadata
         if self._bridge_client:
             self._bridge_client.update_metadata(metadata)
 
+    def update_api_key(self, api_key: Optional[str]) -> None:
+        """Update Core client API key."""
+        # Mutate the bridge config and then only mutate the running client
+        # metadata if already connected
+        self._bridge_config.api_key = api_key
+        if self._bridge_client:
+            self._bridge_client.update_api_key(api_key)
+
     async def _rpc_call(
         self,
         rpc: str,
         req: google.protobuf.message.Message,
         resp_type: Type[ServiceResponse],
         *,
         service: str,
```

### Comparing `temporalio-1.5.1/temporalio/testing/_activity.py` & `temporalio-1.6.0/temporalio/testing/_activity.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/testing/_workflow.py` & `temporalio-1.6.0/temporalio/testing/_workflow.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/types.py` & `temporalio-1.6.0/temporalio/types.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/worker/__init__.py` & `temporalio-1.6.0/temporalio/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/worker/_activity.py` & `temporalio-1.6.0/temporalio/worker/_activity.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/worker/_interceptor.py` & `temporalio-1.6.0/temporalio/worker/_interceptor.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/worker/_replayer.py` & `temporalio-1.6.0/temporalio/worker/_replayer.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,16 +39,18 @@
         workflow_runner: WorkflowRunner = SandboxedWorkflowRunner(),
         unsandboxed_workflow_runner: WorkflowRunner = UnsandboxedWorkflowRunner(),
         namespace: str = "ReplayNamespace",
         data_converter: temporalio.converter.DataConverter = temporalio.converter.DataConverter.default,
         interceptors: Sequence[Interceptor] = [],
         build_id: Optional[str] = None,
         identity: Optional[str] = None,
+        workflow_failure_exception_types: Sequence[Type[BaseException]] = [],
         debug_mode: bool = False,
         runtime: Optional[temporalio.runtime.Runtime] = None,
+        disable_safe_workflow_eviction: bool = False,
     ) -> None:
         """Create a replayer to replay workflows from history.
 
         See :py:meth:`temporalio.worker.Worker.__init__` for a description of
         most of the arguments. The same arguments need to be passed to the
         replayer that were passed to the worker when the workflow originally
         ran.
@@ -61,16 +63,18 @@
             workflow_runner=workflow_runner,
             unsandboxed_workflow_runner=unsandboxed_workflow_runner,
             namespace=namespace,
             data_converter=data_converter,
             interceptors=interceptors,
             build_id=build_id,
             identity=identity,
+            workflow_failure_exception_types=workflow_failure_exception_types,
             debug_mode=debug_mode,
             runtime=runtime,
+            disable_safe_workflow_eviction=disable_safe_workflow_eviction,
         )
 
     def config(self) -> ReplayerConfig:
         """Config, as a dictionary, used to create this replayer.
 
         Returns:
             Configuration, shallow-copied.
@@ -147,43 +151,14 @@
         Args:
             histories: The histories to replay, from an async iterator.
 
         Returns:
             An async iterator that returns replayed workflow results as they are
             replayed.
         """
-        # Create bridge worker
-        task_queue = f"replay-{self._config['build_id']}"
-        runtime = self._config["runtime"] or temporalio.runtime.Runtime.default()
-        bridge_worker, pusher = temporalio.bridge.worker.Worker.for_replay(
-            runtime._core_runtime,
-            temporalio.bridge.worker.WorkerConfig(
-                namespace=self._config["namespace"],
-                task_queue=task_queue,
-                build_id=self._config["build_id"] or load_default_build_id(),
-                identity_override=self._config["identity"],
-                # All values below are ignored but required by Core
-                max_cached_workflows=2,
-                max_outstanding_workflow_tasks=2,
-                max_outstanding_activities=1,
-                max_outstanding_local_activities=1,
-                max_concurrent_workflow_task_polls=1,
-                nonsticky_to_sticky_poll_ratio=1,
-                max_concurrent_activity_task_polls=1,
-                no_remote_activities=True,
-                sticky_queue_schedule_to_start_timeout_millis=1000,
-                max_heartbeat_throttle_interval_millis=1000,
-                default_heartbeat_throttle_interval_millis=1000,
-                max_activities_per_second=None,
-                max_task_queue_activities_per_second=None,
-                graceful_shutdown_period_millis=0,
-                use_worker_versioning=False,
-            ),
-        )
-
         try:
             last_replay_failure: Optional[Exception]
             last_replay_complete = asyncio.Event()
 
             # Create eviction hook
             def on_eviction_hook(
                 run_id: str,
@@ -206,34 +181,70 @@
                     last_replay_failure = RuntimeError(
                         f"{remove_job.reason}: {remove_job.message}"
                     )
                 else:
                     last_replay_failure = None
                 last_replay_complete.set()
 
-            # Start the worker
-            workflow_worker_task = asyncio.create_task(
-                _WorkflowWorker(
-                    bridge_worker=lambda: bridge_worker,
+            # Create worker referencing bridge worker
+            bridge_worker: temporalio.bridge.worker.Worker
+            task_queue = f"replay-{self._config['build_id']}"
+            runtime = self._config["runtime"] or temporalio.runtime.Runtime.default()
+            workflow_worker = _WorkflowWorker(
+                bridge_worker=lambda: bridge_worker,
+                namespace=self._config["namespace"],
+                task_queue=task_queue,
+                workflows=self._config["workflows"],
+                workflow_task_executor=self._config["workflow_task_executor"],
+                workflow_runner=self._config["workflow_runner"],
+                unsandboxed_workflow_runner=self._config["unsandboxed_workflow_runner"],
+                data_converter=self._config["data_converter"],
+                interceptors=self._config["interceptors"],
+                workflow_failure_exception_types=self._config[
+                    "workflow_failure_exception_types"
+                ],
+                debug_mode=self._config["debug_mode"],
+                metric_meter=runtime.metric_meter,
+                on_eviction_hook=on_eviction_hook,
+                disable_eager_activity_execution=False,
+                disable_safe_eviction=self._config["disable_safe_workflow_eviction"],
+            )
+            # Create bridge worker
+            bridge_worker, pusher = temporalio.bridge.worker.Worker.for_replay(
+                runtime._core_runtime,
+                temporalio.bridge.worker.WorkerConfig(
                     namespace=self._config["namespace"],
                     task_queue=task_queue,
-                    workflows=self._config["workflows"],
-                    workflow_task_executor=self._config["workflow_task_executor"],
-                    workflow_runner=self._config["workflow_runner"],
-                    unsandboxed_workflow_runner=self._config[
-                        "unsandboxed_workflow_runner"
-                    ],
-                    data_converter=self._config["data_converter"],
-                    interceptors=self._config["interceptors"],
-                    debug_mode=self._config["debug_mode"],
-                    metric_meter=runtime.metric_meter,
-                    on_eviction_hook=on_eviction_hook,
-                    disable_eager_activity_execution=False,
-                ).run()
+                    build_id=self._config["build_id"] or load_default_build_id(),
+                    identity_override=self._config["identity"],
+                    # Need to tell core whether we want to consider all
+                    # non-determinism exceptions as workflow fail, and whether we do
+                    # per workflow type
+                    nondeterminism_as_workflow_fail=workflow_worker.nondeterminism_as_workflow_fail(),
+                    nondeterminism_as_workflow_fail_for_types=workflow_worker.nondeterminism_as_workflow_fail_for_types(),
+                    # All values below are ignored but required by Core
+                    max_cached_workflows=2,
+                    max_outstanding_workflow_tasks=2,
+                    max_outstanding_activities=1,
+                    max_outstanding_local_activities=1,
+                    max_concurrent_workflow_task_polls=1,
+                    nonsticky_to_sticky_poll_ratio=1,
+                    max_concurrent_activity_task_polls=1,
+                    no_remote_activities=True,
+                    sticky_queue_schedule_to_start_timeout_millis=1000,
+                    max_heartbeat_throttle_interval_millis=1000,
+                    default_heartbeat_throttle_interval_millis=1000,
+                    max_activities_per_second=None,
+                    max_task_queue_activities_per_second=None,
+                    graceful_shutdown_period_millis=0,
+                    use_worker_versioning=False,
+                ),
             )
+            # Start worker
+            workflow_worker_task = asyncio.create_task(workflow_worker.run())
 
             # Yield iterator
             async def replay_iterator() -> AsyncIterator[WorkflowReplayResult]:
                 async for history in histories:
                     # Clear last complete and push history
                     last_replay_complete.clear()
                     await pusher.push_history(
@@ -292,16 +303,18 @@
     workflow_runner: WorkflowRunner
     unsandboxed_workflow_runner: WorkflowRunner
     namespace: str
     data_converter: temporalio.converter.DataConverter
     interceptors: Sequence[Interceptor]
     build_id: Optional[str]
     identity: Optional[str]
+    workflow_failure_exception_types: Sequence[Type[BaseException]]
     debug_mode: bool
     runtime: Optional[temporalio.runtime.Runtime]
+    disable_safe_workflow_eviction: bool
 
 
 @dataclass(frozen=True)
 class WorkflowReplayResult:
     """Single workflow replay result."""
 
     history: temporalio.client.WorkflowHistory
```

### Comparing `temporalio-1.5.1/temporalio/worker/_worker.py` & `temporalio-1.6.0/temporalio/worker/_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,19 +69,21 @@
         no_remote_activities: bool = False,
         sticky_queue_schedule_to_start_timeout: timedelta = timedelta(seconds=10),
         max_heartbeat_throttle_interval: timedelta = timedelta(seconds=60),
         default_heartbeat_throttle_interval: timedelta = timedelta(seconds=30),
         max_activities_per_second: Optional[float] = None,
         max_task_queue_activities_per_second: Optional[float] = None,
         graceful_shutdown_timeout: timedelta = timedelta(),
+        workflow_failure_exception_types: Sequence[Type[BaseException]] = [],
         shared_state_manager: Optional[SharedStateManager] = None,
         debug_mode: bool = False,
         disable_eager_activity_execution: bool = False,
         on_fatal_error: Optional[Callable[[BaseException], Awaitable[None]]] = None,
         use_worker_versioning: bool = False,
+        disable_safe_workflow_eviction: bool = False,
     ) -> None:
         """Create a worker to process workflows and/or activities.
 
         Args:
             client: Client to use for this worker. This is required and must be
                 the :py:class:`temporalio.client.Client` instance or have a
                 worker_service_client attribute with reference to the original
@@ -162,14 +164,21 @@
                 server-side. Note that this only takes effect upon an activity
                 poll request. If multiple workers on the same queue have
                 different values set, they will thrash with the last poller
                 winning.
             graceful_shutdown_timeout: Amount of time after shutdown is called
                 that activities are given to complete before their tasks are
                 cancelled.
+            workflow_failure_exception_types: The types of exceptions that, if a
+                workflow-thrown exception extends, will cause the
+                workflow/update to fail instead of suspending the workflow via
+                task failure. These are applied in addition to ones set on the
+                ``workflow.defn`` decorator. If ``Exception`` is set, it
+                effectively will fail a workflow/update in all user exception
+                cases. WARNING: This setting is experimental.
             shared_state_manager: Used for obtaining cross-process friendly
                 synchronization primitives. This is required for non-async
                 activities where the activity_executor is not a
                 :py:class:`concurrent.futures.ThreadPoolExecutor`. Reuse of
                 these across workers is encouraged.
             debug_mode: If true, will disable deadlock detection and may disable
                 sandboxing in order to make using a debugger easier. If false
@@ -179,19 +188,27 @@
                 activity execution. Eager activity execution is an optimization
                 on some servers that sends activities back to the same worker as
                 the calling workflow if they can run there. This setting is
                 experimental and may be removed in a future release.
             on_fatal_error: An async function that can handle a failure before
                 the worker shutdown commences. This cannot stop the shutdown and
                 any exception raised is logged and ignored.
-            use_worker_versioning: If true, the `build_id` argument must be specified, and this
-                worker opts into the worker versioning feature. This ensures it only receives
-                workflow tasks for workflows which it claims to be compatible with.
-
-                For more information, see https://docs.temporal.io/workers#worker-versioning
+            use_worker_versioning: If true, the `build_id` argument must be
+                specified, and this worker opts into the worker versioning
+                feature. This ensures it only receives workflow tasks for
+                workflows which it claims to be compatible with. For more
+                information, see
+                https://docs.temporal.io/workers#worker-versioning.
+            disable_safe_workflow_eviction: If true, instead of letting the
+                workflow collect its tasks properly, the worker will simply let
+                the Python garbage collector collect the tasks. WARNING: Users
+                should not set this value to true. The garbage collector will
+                throw ``GeneratorExit`` in coroutines causing them to to wake up
+                in different threads and run ``finally`` and other code in the
+                wrong workflow environment.
         """
         if not activities and not workflows:
             raise ValueError("At least one activity or workflow must be specified")
         if use_worker_versioning and not build_id:
             raise ValueError(
                 "build_id must be specified when use_worker_versioning is True"
             )
@@ -200,31 +217,16 @@
         client_config = client.config()
         interceptors_from_client = cast(
             List[Interceptor],
             [i for i in client_config["interceptors"] if isinstance(i, Interceptor)],
         )
         interceptors = interceptors_from_client + list(interceptors)
 
-        # Extract the bridge service client. We try the service on the client
-        # first, then we support a worker_service_client on the client's service
-        # to return underlying service client we can use.
-        bridge_client: temporalio.service._BridgeServiceClient
-        if isinstance(client.service_client, temporalio.service._BridgeServiceClient):
-            bridge_client = client.service_client
-        elif hasattr(client.service_client, "worker_service_client"):
-            bridge_client = client.service_client.worker_service_client
-            if not isinstance(bridge_client, temporalio.service._BridgeServiceClient):
-                raise TypeError(
-                    "Client's worker_service_client cannot be used for a worker"
-                )
-        else:
-            raise TypeError(
-                "Client cannot be used for a worker. "
-                + "Use the original client's service or set worker_service_client on the wrapped service with the original service client."
-            )
+        # Extract the bridge service client
+        bridge_client = _extract_bridge_client_for_worker(client)
 
         # Store the config for tracking
         self._config = WorkerConfig(
             client=client,
             task_queue=task_queue,
             activities=activities,
             workflows=workflows,
@@ -245,30 +247,34 @@
             no_remote_activities=no_remote_activities,
             sticky_queue_schedule_to_start_timeout=sticky_queue_schedule_to_start_timeout,
             max_heartbeat_throttle_interval=max_heartbeat_throttle_interval,
             default_heartbeat_throttle_interval=default_heartbeat_throttle_interval,
             max_activities_per_second=max_activities_per_second,
             max_task_queue_activities_per_second=max_task_queue_activities_per_second,
             graceful_shutdown_timeout=graceful_shutdown_timeout,
+            workflow_failure_exception_types=workflow_failure_exception_types,
             shared_state_manager=shared_state_manager,
             debug_mode=debug_mode,
             disable_eager_activity_execution=disable_eager_activity_execution,
             on_fatal_error=on_fatal_error,
             use_worker_versioning=use_worker_versioning,
+            disable_safe_workflow_eviction=disable_safe_workflow_eviction,
         )
         self._started = False
         self._shutdown_event = asyncio.Event()
         self._shutdown_complete_event = asyncio.Event()
         self._async_context_inner_task: Optional[asyncio.Task] = None
         self._async_context_run_task: Optional[asyncio.Task] = None
         self._async_context_run_exception: Optional[BaseException] = None
 
         # Create activity and workflow worker
         self._activity_worker: Optional[_ActivityWorker] = None
-        runtime = bridge_client.config.runtime or temporalio.runtime.Runtime.default()
+        self._runtime = (
+            bridge_client.config.runtime or temporalio.runtime.Runtime.default()
+        )
         if activities:
             # Issue warning here if executor max_workers is lower than max
             # concurrent activities. We do this here instead of in
             # _ActivityWorker so the stack level is predictable.
             max_workers = getattr(activity_executor, "_max_workers", None)
             if isinstance(max_workers, int) and max_workers < max_concurrent_activities:
                 warnings.warn(
@@ -281,53 +287,45 @@
                 bridge_worker=lambda: self._bridge_worker,
                 task_queue=task_queue,
                 activities=activities,
                 activity_executor=activity_executor,
                 shared_state_manager=shared_state_manager,
                 data_converter=client_config["data_converter"],
                 interceptors=interceptors,
-                metric_meter=runtime.metric_meter,
+                metric_meter=self._runtime.metric_meter,
             )
         self._workflow_worker: Optional[_WorkflowWorker] = None
         if workflows:
             self._workflow_worker = _WorkflowWorker(
                 bridge_worker=lambda: self._bridge_worker,
                 namespace=client.namespace,
                 task_queue=task_queue,
                 workflows=workflows,
                 workflow_task_executor=workflow_task_executor,
                 workflow_runner=workflow_runner,
                 unsandboxed_workflow_runner=unsandboxed_workflow_runner,
                 data_converter=client_config["data_converter"],
                 interceptors=interceptors,
+                workflow_failure_exception_types=workflow_failure_exception_types,
                 debug_mode=debug_mode,
                 disable_eager_activity_execution=disable_eager_activity_execution,
-                metric_meter=runtime.metric_meter,
+                metric_meter=self._runtime.metric_meter,
                 on_eviction_hook=None,
+                disable_safe_eviction=disable_safe_workflow_eviction,
             )
 
-        # We need an already connected client
-        # TODO(cretz): How to connect to client inside constructor here? In the
-        # meantime, we disallow lazy clients from being used for workers. We
-        # could check whether the connected client is present which means
-        # lazy-but-already-connected clients would work, but that is confusing
-        # to users that the client only works if they already made a call on it.
-        if bridge_client.config.lazy:
-            raise RuntimeError("Lazy clients cannot be used for workers")
-        raw_bridge_client = bridge_client._bridge_client
-        assert raw_bridge_client
-
         # Create bridge worker last. We have empirically observed that if it is
         # created before an error is raised from the activity worker
         # constructor, a deadlock/hang will occur presumably while trying to
         # free it.
         # TODO(cretz): Why does this cause a test hang when an exception is
         # thrown after it?
+        assert bridge_client._bridge_client
         self._bridge_worker = temporalio.bridge.worker.Worker.create(
-            raw_bridge_client,
+            bridge_client._bridge_client,
             temporalio.bridge.worker.WorkerConfig(
                 namespace=client.namespace,
                 task_queue=task_queue,
                 build_id=build_id or load_default_build_id(),
                 identity_override=identity,
                 max_cached_workflows=max_cached_workflows,
                 max_outstanding_workflow_tasks=max_concurrent_workflow_tasks,
@@ -351,14 +349,22 @@
                 ),
                 max_activities_per_second=max_activities_per_second,
                 max_task_queue_activities_per_second=max_task_queue_activities_per_second,
                 graceful_shutdown_period_millis=int(
                     1000 * graceful_shutdown_timeout.total_seconds()
                 ),
                 use_worker_versioning=use_worker_versioning,
+                # Need to tell core whether we want to consider all
+                # non-determinism exceptions as workflow fail, and whether we do
+                # per workflow type
+                nondeterminism_as_workflow_fail=self._workflow_worker is not None
+                and self._workflow_worker.nondeterminism_as_workflow_fail(),
+                nondeterminism_as_workflow_fail_for_types=self._workflow_worker.nondeterminism_as_workflow_fail_for_types()
+                if self._workflow_worker
+                else set(),
             ),
         )
 
     def config(self) -> WorkerConfig:
         """Config, as a dictionary, used to create this worker.
 
         Returns:
@@ -371,14 +377,37 @@
 
     @property
     def task_queue(self) -> str:
         """Task queue this worker is on."""
         return self._config["task_queue"]
 
     @property
+    def client(self) -> temporalio.client.Client:
+        """Client currently set on the worker."""
+        return self._config["client"]
+
+    @client.setter
+    def client(self, value: temporalio.client.Client) -> None:
+        """Update the client associated with the worker.
+
+        Changing the client will make sure the worker starts using it for the
+        next calls it makes. However, outstanding client calls will still
+        complete with the existing client. The new client cannot be "lazy" and
+        must be using the same runtime as the current client.
+        """
+        bridge_client = _extract_bridge_client_for_worker(value)
+        if self._runtime is not bridge_client.config.runtime:
+            raise ValueError(
+                "New client is not on the same runtime as the existing client"
+            )
+        assert bridge_client._bridge_client
+        self._bridge_worker.replace_client(bridge_client._bridge_client)
+        self._config["client"] = value
+
+    @property
     def is_running(self) -> bool:
         """Whether the worker is running.
 
         This is only ``True`` if the worker has been started and not yet
         shut down.
         """
         return self._started and not self.is_shutdown
@@ -469,17 +498,19 @@
             else:
                 assert self._workflow_worker
                 tasks[1] = asyncio.create_task(self._workflow_worker.drain_poll_queue())
         if len(tasks) > 2 and tasks[2].done() and tasks[2].exception():
             assert self._workflow_worker
             tasks[2] = asyncio.create_task(self._workflow_worker.drain_poll_queue())
 
-        # Set worker-shutdown event
+        # Notify shutdown occurring
         if self._activity_worker:
             self._activity_worker.notify_shutdown()
+        if self._workflow_worker:
+            self._workflow_worker.notify_shutdown()
 
         # Wait for all tasks to complete (i.e. for poller loops to stop)
         await asyncio.wait(tasks)
         # Sometimes both workers throw an exception and since we only take the
         # first, Python may complain with "Task exception was never retrieved"
         # if we don't get the others. Therefore we call cancel on each task
         # which suppresses this.
@@ -588,19 +619,21 @@
     no_remote_activities: bool
     sticky_queue_schedule_to_start_timeout: timedelta
     max_heartbeat_throttle_interval: timedelta
     default_heartbeat_throttle_interval: timedelta
     max_activities_per_second: Optional[float]
     max_task_queue_activities_per_second: Optional[float]
     graceful_shutdown_timeout: timedelta
+    workflow_failure_exception_types: Sequence[Type[BaseException]]
     shared_state_manager: Optional[SharedStateManager]
     debug_mode: bool
     disable_eager_activity_execution: bool
     on_fatal_error: Optional[Callable[[BaseException], Awaitable[None]]]
     use_worker_versioning: bool
+    disable_safe_workflow_eviction: bool
 
 
 _default_build_id: Optional[str] = None
 
 
 def load_default_build_id(*, memoize: bool = True) -> str:
     """Load the default worker build ID.
@@ -677,9 +710,41 @@
         with open(sys.modules[mod_name].__cached__, "rb") as f:
             return f.read()
     except Exception:
         pass
     return None
 
 
+def _extract_bridge_client_for_worker(
+    client: temporalio.client.Client,
+) -> temporalio.service._BridgeServiceClient:
+    # Extract the bridge service client. We try the service on the client first,
+    # then we support a worker_service_client on the client's service to return
+    # underlying service client we can use.
+    bridge_client: temporalio.service._BridgeServiceClient
+    if isinstance(client.service_client, temporalio.service._BridgeServiceClient):
+        bridge_client = client.service_client
+    elif hasattr(client.service_client, "worker_service_client"):
+        bridge_client = client.service_client.worker_service_client
+        if not isinstance(bridge_client, temporalio.service._BridgeServiceClient):
+            raise TypeError(
+                "Client's worker_service_client cannot be used for a worker"
+            )
+    else:
+        raise TypeError(
+            "Client cannot be used for a worker. "
+            + "Use the original client's service or set worker_service_client on the wrapped service with the original service client."
+        )
+
+    # We need an already connected client
+    # TODO(cretz): How to connect to client inside Worker constructor here? In
+    # the meantime, we disallow lazy clients from being used for workers. We
+    # could check whether the connected client is present which means
+    # lazy-but-already-connected clients would work, but that is confusing
+    # to users that the client only works if they already made a call on it.
+    if bridge_client.config.lazy:
+        raise RuntimeError("Lazy clients cannot be used for workers")
+    return bridge_client
+
+
 class _ShutdownRequested(RuntimeError):
     pass
```

### Comparing `temporalio-1.5.1/temporalio/worker/_workflow.py` & `temporalio-1.6.0/temporalio/worker/_workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 import asyncio
 import concurrent.futures
 import logging
 import os
 from datetime import timezone
-from typing import Callable, Dict, List, MutableMapping, Optional, Sequence, Type
+from typing import Callable, Dict, List, MutableMapping, Optional, Sequence, Set, Type
 
 import temporalio.activity
 import temporalio.api.common.v1
 import temporalio.bridge.client
 import temporalio.bridge.proto.workflow_activation
 import temporalio.bridge.proto.workflow_completion
 import temporalio.bridge.worker
@@ -48,22 +48,24 @@
         task_queue: str,
         workflows: Sequence[Type],
         workflow_task_executor: Optional[concurrent.futures.ThreadPoolExecutor],
         workflow_runner: WorkflowRunner,
         unsandboxed_workflow_runner: WorkflowRunner,
         data_converter: temporalio.converter.DataConverter,
         interceptors: Sequence[Interceptor],
+        workflow_failure_exception_types: Sequence[Type[BaseException]],
         debug_mode: bool,
         disable_eager_activity_execution: bool,
         metric_meter: temporalio.common.MetricMeter,
         on_eviction_hook: Optional[
             Callable[
                 [str, temporalio.bridge.proto.workflow_activation.RemoveFromCache], None
             ]
         ],
+        disable_safe_eviction: bool,
     ) -> None:
         self._bridge_worker = bridge_worker
         self._namespace = namespace
         self._task_queue = task_queue
         self._workflow_task_executor = (
             workflow_task_executor
             or concurrent.futures.ThreadPoolExecutor(
@@ -84,25 +86,35 @@
         for i in interceptors:
             interceptor_class = i.workflow_interceptor_class(interceptor_class_input)
             if interceptor_class:
                 self._interceptor_classes.append(interceptor_class)
         self._extern_functions.update(
             **_WorkflowExternFunctions(__temporal_get_metric_meter=lambda: metric_meter)
         )
+        self._workflow_failure_exception_types = workflow_failure_exception_types
         self._running_workflows: Dict[str, WorkflowInstance] = {}
         self._disable_eager_activity_execution = disable_eager_activity_execution
         self._on_eviction_hook = on_eviction_hook
+        self._disable_safe_eviction = disable_safe_eviction
         self._throw_after_activation: Optional[Exception] = None
 
         # If there's a debug mode or a truthy TEMPORAL_DEBUG env var, disable
         # deadlock detection, otherwise set to 2 seconds
         self._deadlock_timeout_seconds = (
             None if debug_mode or os.environ.get("TEMPORAL_DEBUG") else 2
         )
 
+        # Keep track of workflows that could not be evicted
+        self._could_not_evict_count = 0
+
+        # Set the worker-level failure exception types into the runner
+        workflow_runner.set_worker_level_failure_exception_types(
+            workflow_failure_exception_types
+        )
+
         # Validate and build workflow dict
         self._workflows: Dict[str, temporalio.workflow._Definition] = {}
         self._dynamic_workflow: Optional[temporalio.workflow._Definition] = None
         for workflow in workflows:
             defn = temporalio.workflow._Definition.must_from_class(workflow)
             # Confirm name unique
             if defn.name in self._workflows:
@@ -151,14 +163,21 @@
             # Shutdown the thread pool executor if we created it
             if not self._workflow_task_executor_user_provided:
                 self._workflow_task_executor.shutdown()
 
         if self._throw_after_activation:
             raise self._throw_after_activation
 
+    def notify_shutdown(self) -> None:
+        if self._could_not_evict_count:
+            logger.warn(
+                f"Shutting down workflow worker, but {self._could_not_evict_count} "
+                + "workflow(s) could not be evicted previously, so the shutdown will hang"
+            )
+
     # Only call this if run() raised an error
     async def drain_poll_queue(self) -> None:
         while True:
             try:
                 # Just take all tasks and say we can't handle them
                 act = await self._bridge_worker().poll_workflow_activation()
                 completion = temporalio.bridge.proto.workflow_completion.WorkflowActivationCompletion(
@@ -178,50 +197,51 @@
         cache_remove_job = None
         start_job = None
         for job in act.jobs:
             if job.HasField("remove_from_cache"):
                 cache_remove_job = job.remove_from_cache
             elif job.HasField("start_workflow"):
                 start_job = job.start_workflow
-        cache_remove_only_activation = len(act.jobs) == 1 and cache_remove_job
 
         # Build default success completion (e.g. remove-job-only activations)
         completion = (
             temporalio.bridge.proto.workflow_completion.WorkflowActivationCompletion()
         )
         completion.successful.SetInParent()
         try:
-            # Decode the activation if there's a codec and it's not a
-            # cache-remove-only activation
-            if self._data_converter.payload_codec and not cache_remove_only_activation:
+            # Decode the activation if there's a codec and not cache remove job
+            if self._data_converter.payload_codec and not cache_remove_job:
                 await temporalio.bridge.worker.decode_activation(
                     act, self._data_converter.payload_codec
                 )
 
             if LOG_PROTOS:
                 logger.debug("Received workflow activation:\n%s", act)
 
-            # We only have to run if there are any non-remove-from-cache jobs
-            if not cache_remove_only_activation:
-                # If the workflow is not running yet, create it
+            # If the workflow is not running yet and this isn't a cache remove
+            # job, create it. We do not even fetch a workflow if it's a cache
+            # remove job and safe evictions are enabled
+            workflow = None
+            if not cache_remove_job or not self._disable_safe_eviction:
                 workflow = self._running_workflows.get(act.run_id)
-                if not workflow:
-                    # Must have a start job to create instance
-                    if not start_job:
-                        raise RuntimeError(
-                            "Missing start workflow, workflow could have unexpectedly been removed from cache"
-                        )
-                    workflow = self._create_workflow_instance(act, start_job)
-                    self._running_workflows[act.run_id] = workflow
-                elif start_job:
-                    # This should never happen
-                    logger.warn("Cache already exists for activation with start job")
-
-                # Run activation in separate thread so we can check if it's
-                # deadlocked
+            if not workflow and not cache_remove_job:
+                # Must have a start job to create instance
+                if not start_job:
+                    raise RuntimeError(
+                        "Missing start workflow, workflow could have unexpectedly been removed from cache"
+                    )
+                workflow = self._create_workflow_instance(act, start_job)
+                self._running_workflows[act.run_id] = workflow
+            elif start_job:
+                # This should never happen
+                logger.warn("Cache already exists for activation with start job")
+
+            # Run activation in separate thread so we can check if it's
+            # deadlocked
+            if workflow:
                 activate_task = asyncio.get_running_loop().run_in_executor(
                     self._workflow_task_executor,
                     workflow.activate,
                     act,
                 )
 
                 # Wait for deadlock timeout and set commands if successful
@@ -230,14 +250,25 @@
                         activate_task, self._deadlock_timeout_seconds
                     )
                 except asyncio.TimeoutError:
                     raise RuntimeError(
                         f"[TMPRL1101] Potential deadlock detected, workflow didn't yield within {self._deadlock_timeout_seconds} second(s)"
                     )
         except Exception as err:
+            # We cannot fail a cache eviction, we must just log and not complete
+            # the activation (failed or otherwise). This should only happen in
+            # cases of deadlock or tasks not properly completing, and yes this
+            # means that a slot is forever taken.
+            # TODO(cretz): Should we build a complex mechanism to continually
+            # try the eviction until it succeeds?
+            if cache_remove_job:
+                logger.exception("Failed running eviction job, not evicting")
+                self._could_not_evict_count += 1
+                return
+
             logger.exception(
                 "Failed handling activation on workflow with run ID %s", act.run_id
             )
             # Set completion failure
             completion.failed.failure.SetInParent()
             try:
                 self._data_converter.failure_converter.to_failure(
@@ -253,33 +284,28 @@
                 completion.failed.failure.message = (
                     f"Failed converting activation exception: {inner_err}"
                 )
 
         # Always set the run ID on the completion
         completion.run_id = act.run_id
 
-        # If there is a remove-from-cache job, do so
+        # If there is a remove-from-cache job, do so. We don't need to log a
+        # warning if there's not, because create workflow failing for
+        # unregistered workflow still triggers cache remove job
         if cache_remove_job:
             if act.run_id in self._running_workflows:
                 logger.debug(
                     "Evicting workflow with run ID %s, message: %s",
                     act.run_id,
                     cache_remove_job.message,
                 )
                 del self._running_workflows[act.run_id]
-            else:
-                logger.warn(
-                    "Eviction request on unknown workflow with run ID %s, message: %s",
-                    act.run_id,
-                    cache_remove_job.message,
-                )
 
-        # Encode the completion if there's a codec and it's not a
-        # cache-remove-only activation
-        if self._data_converter.payload_codec and not cache_remove_only_activation:
+        # Encode the completion if there's a codec and not cache remove job
+        if self._data_converter.payload_codec and not cache_remove_job:
             try:
                 await temporalio.bridge.worker.encode_completion(
                     completion, self._data_converter.payload_codec
                 )
             except Exception as err:
                 logger.exception(
                     "Failed encoding completion on workflow with run ID %s", act.run_id
@@ -366,12 +392,29 @@
             failure_converter_class=self._data_converter.failure_converter_class,
             interceptor_classes=self._interceptor_classes,
             defn=defn,
             info=info,
             randomness_seed=start.randomness_seed,
             extern_functions=self._extern_functions,
             disable_eager_activity_execution=self._disable_eager_activity_execution,
+            worker_level_failure_exception_types=self._workflow_failure_exception_types,
         )
         if defn.sandboxed:
             return self._workflow_runner.create_instance(det)
         else:
             return self._unsandboxed_workflow_runner.create_instance(det)
+
+    def nondeterminism_as_workflow_fail(self) -> bool:
+        return any(
+            issubclass(temporalio.workflow.NondeterminismError, typ)
+            for typ in self._workflow_failure_exception_types
+        )
+
+    def nondeterminism_as_workflow_fail_for_types(self) -> Set[str]:
+        return set(
+            k
+            for k, v in self._workflows.items()
+            if any(
+                issubclass(temporalio.workflow.NondeterminismError, typ)
+                for typ in v.failure_exception_types
+            )
+        )
```

### Comparing `temporalio-1.5.1/temporalio/worker/_workflow_instance.py` & `temporalio-1.6.0/temporalio/worker/_workflow_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Any,
     Awaitable,
     Callable,
     Coroutine,
     Deque,
     Dict,
     Generator,
+    Generic,
     Iterator,
     List,
     Mapping,
     MutableMapping,
     NoReturn,
     Optional,
     Sequence,
@@ -34,15 +35,15 @@
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
-from typing_extensions import TypeAlias, TypedDict
+from typing_extensions import Self, TypeAlias, TypedDict
 
 import temporalio.activity
 import temporalio.api.common.v1
 import temporalio.api.enums.v1
 import temporalio.bridge.proto.activity_result
 import temporalio.bridge.proto.child_workflow
 import temporalio.bridge.proto.workflow_activation
@@ -66,14 +67,17 @@
     StartLocalActivityInput,
     WorkflowInboundInterceptor,
     WorkflowOutboundInterceptor,
 )
 
 logger = logging.getLogger(__name__)
 
+# Set to true to log all cases where we're ignoring things during delete
+LOG_IGNORE_DURING_DELETE = False
+
 
 class WorkflowRunner(ABC):
     """Abstract runner for workflows that creates workflow instances to run.
 
     :py:class:`UnsandboxedWorkflowRunner` is an implementation that locally runs
     the workflow.
     """
@@ -99,27 +103,39 @@
             det: Details that can be used to create the instance.
 
         Returns:
             Workflow instance that can handle activations.
         """
         raise NotImplementedError
 
+    def set_worker_level_failure_exception_types(
+        self, types: Sequence[Type[BaseException]]
+    ) -> None:
+        """Set worker-level failure exception types that will be used to
+        validate in the sandbox when calling ``prepare_workflow``.
+
+        Args:
+            types: Exception types.
+        """
+        pass
+
 
 @dataclass(frozen=True)
 class WorkflowInstanceDetails:
     """Immutable details for creating a workflow instance."""
 
     payload_converter_class: Type[temporalio.converter.PayloadConverter]
     failure_converter_class: Type[temporalio.converter.FailureConverter]
     interceptor_classes: Sequence[Type[WorkflowInboundInterceptor]]
     defn: temporalio.workflow._Definition
     info: temporalio.workflow.Info
     randomness_seed: int
     extern_functions: Mapping[str, Callable]
     disable_eager_activity_execution: bool
+    worker_level_failure_exception_types: Sequence[Type[BaseException]]
 
 
 class WorkflowInstance(ABC):
     """Instance of a workflow that can handle activations."""
 
     @abstractmethod
     def activate(
@@ -169,14 +185,17 @@
         temporalio.workflow._Runtime.__init__(self)
         self._payload_converter = det.payload_converter_class()
         self._failure_converter = det.failure_converter_class()
         self._defn = det.defn
         self._info = det.info
         self._extern_functions = det.extern_functions
         self._disable_eager_activity_execution = det.disable_eager_activity_execution
+        self._worker_level_failure_exception_types = (
+            det.worker_level_failure_exception_types
+        )
         self._primary_task: Optional[asyncio.Task[None]] = None
         self._time_ns = 0
         self._cancel_requested = False
         self._current_build_id = ""
         self._current_history_length = 0
         self._current_history_size = 0
         self._continue_as_new_suggested = False
@@ -250,27 +269,21 @@
         finally:
             # Remove our runtime from the loop
             temporalio.workflow._Runtime.set_on_loop(asyncio.get_running_loop(), None)
 
         # Set ourselves on our own loop
         temporalio.workflow._Runtime.set_on_loop(self, self)
 
-        # After GC, Python raises GeneratorExit calls from all awaiting tasks.
-        # Then in a finally of such an await, another exception can swallow
-        # these causing even more issues. We will set ourselves as deleted so we
-        # can check in some places to swallow these errors on tear down.
+        # When we evict, we have to mark the workflow as deleting so we don't
+        # add any commands and we swallow exceptions on tear down
         self._deleting = False
 
         # We only create the metric meter lazily
         self._metric_meter: Optional[_ReplaySafeMetricMeter] = None
 
-    def __del__(self) -> None:
-        # We have confirmed there are no super() versions of __del__
-        self._deleting = True
-
     #### Activation functions ####
     # These are in alphabetical order and besides "activate", all other calls
     # are "_apply_" + the job field name.
 
     def activate(
         self, act: temporalio.bridge.proto.workflow_activation.WorkflowActivation
     ) -> temporalio.bridge.proto.workflow_completion.WorkflowActivationCompletion:
@@ -312,28 +325,51 @@
                     # Let errors bubble out of these to the caller to fail the task
                     self._apply(job)
 
                 # Run one iteration of the loop. We do not allow conditions to
                 # be checked in patch jobs (first index) or query jobs (last
                 # index).
                 self._run_once(check_conditions=index == 1 or index == 2)
-        except temporalio.exceptions.FailureError as err:
-            # We want failure errors during activation, like those that can
-            # happen during payload conversion, to fail the workflow not the
-            # task
-            try:
-                self._set_workflow_failure(err)
-            except Exception as inner_err:
-                activation_err = inner_err
         except Exception as err:
-            activation_err = err
+            # We want some errors during activation, like those that can happen
+            # during payload conversion, to be able to fail the workflow not the
+            # task
+            if self._is_workflow_failure_exception(err):
+                try:
+                    self._set_workflow_failure(err)
+                except Exception as inner_err:
+                    activation_err = inner_err
+            else:
+                # Otherwise all exceptions are activation errors
+                activation_err = err
+            # If we're deleting, swallow any activation error
+            if self._deleting:
+                if LOG_IGNORE_DURING_DELETE:
+                    logger.debug(
+                        "Ignoring exception while deleting workflow", exc_info=True
+                    )
+                activation_err = None
+
+        # If we're deleting, there better be no more tasks. It is important for
+        # the integrity of the system that we check this. If there are tasks
+        # remaining, they and any associated coroutines will get garbage
+        # collected which can trigger a GeneratorExit exception thrown in the
+        # coroutine which can cause it to wakeup on a different thread which may
+        # have a different workflow/event-loop going.
+        if self._deleting and self._tasks:
+            raise RuntimeError(
+                f"Cache removal processed, but {len(self._tasks)} tasks remain. "
+                + f"Stack traces below:\n\n{self._stack_trace()}"
+            )
+
         if activation_err:
             logger.warning(
                 f"Failed activation on workflow {self._info.workflow_type} with ID {self._info.workflow_id} and run ID {self._info.run_id}",
                 exc_info=activation_err,
+                extra={"temporal_workflow": self._info._logger_details()},
             )
             # Set completion failure
             self._current_completion.failed.failure.SetInParent()
             try:
                 self._failure_converter.to_failure(
                     activation_err,
                     self._payload_converter,
@@ -377,16 +413,15 @@
         elif job.HasField("fire_timer"):
             self._apply_fire_timer(job.fire_timer)
         elif job.HasField("query_workflow"):
             self._apply_query_workflow(job.query_workflow)
         elif job.HasField("notify_has_patch"):
             self._apply_notify_has_patch(job.notify_has_patch)
         elif job.HasField("remove_from_cache"):
-            # Ignore, handled externally
-            pass
+            self._apply_remove_from_cache(job.remove_from_cache)
         elif job.HasField("resolve_activity"):
             self._apply_resolve_activity(job.resolve_activity)
         elif job.HasField("resolve_child_workflow_execution"):
             self._apply_resolve_child_workflow_execution(
                 job.resolve_child_workflow_execution
             )
         elif job.HasField("resolve_child_workflow_execution_start"):
@@ -491,20 +526,18 @@
                     err = temporalio.exceptions.CancelledError(
                         f"Cancellation raised within update {err}"
                     )
                 # Read-only issues during validation should fail the task
                 if isinstance(err, temporalio.workflow.ReadOnlyContextError):
                     self._current_activation_error = err
                     return
-                # Temporal errors always fail the update. Other errors fail it during validation, but the task during
-                # handling.
-                if (
-                    isinstance(err, temporalio.exceptions.FailureError)
-                    or not past_validation
-                ):
+                # Validation failures are always update failures. We reuse
+                # workflow failure logic to decide task failure vs update
+                # failure after validation.
+                if not past_validation or self._is_workflow_failure_exception(err):
                     if command is None:
                         command = self._add_command()
                         command.update_response.protocol_instance_id = (
                             job.protocol_instance_id
                         )
                     command.update_response.rejected.SetInParent()
                     self._failure_converter.to_failure(
@@ -512,27 +545,21 @@
                         self._payload_converter,
                         command.update_response.rejected,
                     )
                 else:
                     self._current_activation_error = err
                     return
             except BaseException as err:
-                # During tear down, generator exit and no-runtime exceptions can appear
-                if not self._deleting:
-                    raise
-                if not isinstance(
-                    err,
-                    (
-                        GeneratorExit,
-                        temporalio.workflow._NotInWorkflowEventLoopError,
-                    ),
-                ):
-                    logger.debug(
-                        "Ignoring exception while deleting workflow", exc_info=True
-                    )
+                if self._deleting:
+                    if LOG_IGNORE_DURING_DELETE:
+                        logger.debug(
+                            "Ignoring exception while deleting workflow", exc_info=True
+                        )
+                    return
+                raise
 
         self.create_task(
             run_update(),
             name=f"update: {job.name}",
         )
 
     def _apply_fire_timer(
@@ -601,14 +628,23 @@
         self.create_task(run_query(), name=f"query: {job.query_type}")
 
     def _apply_notify_has_patch(
         self, job: temporalio.bridge.proto.workflow_activation.NotifyHasPatch
     ) -> None:
         self._patches_notified.add(job.patch_id)
 
+    def _apply_remove_from_cache(
+        self, job: temporalio.bridge.proto.workflow_activation.RemoveFromCache
+    ) -> None:
+        self._deleting = True
+        self._cancel_requested = True
+        # Cancel everything
+        for task in self._tasks:
+            task.cancel()
+
     def _apply_resolve_activity(
         self, job: temporalio.bridge.proto.workflow_activation.ResolveActivity
     ) -> None:
         handle = self._pending_activities.pop(job.seq, None)
         if not handle:
             raise RuntimeError(f"Failed finding activity handle for sequence {job.seq}")
         if job.result.HasField("completed"):
@@ -770,25 +806,22 @@
                 result_payloads = self._payload_converter.to_payloads([result])
                 if len(result_payloads) != 1:
                     raise ValueError(
                         f"Expected 1 result payload, got {len(result_payloads)}"
                     )
                 command = self._add_command()
                 command.complete_workflow_execution.result.CopyFrom(result_payloads[0])
-            except BaseException as err:
-                # During tear down, generator exit and event loop exceptions can occur
-                if not self._deleting:
-                    raise
-                if not isinstance(
-                    err,
-                    (GeneratorExit, temporalio.workflow._NotInWorkflowEventLoopError),
-                ):
-                    logger.debug(
-                        "Ignoring exception while deleting workflow", exc_info=True
-                    )
+            except Exception:
+                if self._deleting:
+                    if LOG_IGNORE_DURING_DELETE:
+                        logger.debug(
+                            "Ignoring exception while deleting workflow", exc_info=True
+                        )
+                    return
+                raise
 
         # Set arg types, using raw values for dynamic
         arg_types = self._defn.arg_types
         if not self._defn.name:
             # Dynamic is just the raw value for each input value
             arg_types = [temporalio.common.RawValue] * len(job.arguments)
         args = self._convert_payloads(job.arguments, arg_types)
@@ -1473,15 +1506,19 @@
         prev_val = self._read_only
         self._read_only = True
         try:
             yield None
         finally:
             self._read_only = prev_val
 
-    def _assert_not_read_only(self, action_attempted: str) -> None:
+    def _assert_not_read_only(
+        self, action_attempted: str, *, allow_during_delete: bool = False
+    ) -> None:
+        if self._deleting and not allow_during_delete:
+            raise RuntimeError(f"Ignoring {action_attempted} while deleting")
         if self._read_only:
             raise temporalio.workflow.ReadOnlyContextError(
                 f"While in read-only function, action attempted: {action_attempted}"
             )
 
     async def _cancel_external_workflow(
         self,
@@ -1521,14 +1558,27 @@
             )
         except temporalio.exceptions.FailureError:
             # Don't wrap payload conversion errors that would fail the workflow
             raise
         except Exception as err:
             raise RuntimeError("Failed decoding arguments") from err
 
+    def _is_workflow_failure_exception(self, err: BaseException) -> bool:
+        # An exception is a failure instead of a task fail if it's already a
+        # failure error or if it is an instance of any of the failure types in
+        # the worker or workflow-level setting
+        return (
+            isinstance(err, temporalio.exceptions.FailureError)
+            or any(isinstance(err, typ) for typ in self._defn.failure_exception_types)
+            or any(
+                isinstance(err, typ)
+                for typ in self._worker_level_failure_exception_types
+            )
+        )
+
     def _next_seq(self, type: str) -> int:
         seq = self._curr_seqs.get(type, 0) + 1
         self._curr_seqs[type] = seq
         return seq
 
     def _process_handler_args(
         self,
@@ -1616,17 +1666,17 @@
             # Run while there is anything ready
             while self._ready:
                 # Run and remove all ready ones
                 while self._ready:
                     handle = self._ready.popleft()
                     handle._run()
 
-                    # Must throw here. Only really set inside
+                    # Must throw here if not deleting. Only really set inside
                     # _run_top_level_workflow_function.
-                    if self._current_activation_error:
+                    if self._current_activation_error and not self._deleting:
                         raise self._current_activation_error
 
                 # Check conditions which may add to the ready list. Also remove
                 # conditions whose futures have already cancelled (e.g. when
                 # timed out).
                 if check_conditions:
                     self._conditions[:] = [
@@ -1641,20 +1691,31 @@
     # order to apply common exception handling to each
     async def _run_top_level_workflow_function(self, coro: Awaitable[None]) -> None:
         try:
             await coro
         except _ContinueAsNewError as err:
             logger.debug("Workflow requested continue as new")
             err._apply_command(self._add_command())
-
-        # Note in some Python versions, cancelled error does not extend
-        # exception
-        # TODO(cretz): Should I fail the task on BaseException too (e.g.
-        # KeyboardInterrupt)?
         except (Exception, asyncio.CancelledError) as err:
+            # During tear down we can ignore exceptions. Technically the
+            # command-adding done later would throw a not-in-workflow exception
+            # we'd ignore later, but it's better to preempt it
+            if self._deleting:
+                if LOG_IGNORE_DURING_DELETE:
+                    logger.debug(
+                        "Ignoring exception while deleting workflow", exc_info=True
+                    )
+                return
+
+            # Handle continue as new
+            if isinstance(err, _ContinueAsNewError):
+                logger.debug("Workflow requested continue as new")
+                err._apply_command(self._add_command())
+                return
+
             logger.debug(
                 f"Workflow raised failure with run ID {self._info.run_id}",
                 exc_info=True,
             )
 
             # All asyncio cancelled errors become Temporal cancelled errors
             if isinstance(err, asyncio.CancelledError):
@@ -1666,32 +1727,22 @@
             # cancel later on will show the workflow as cancelled. But this is
             # a Temporal limitation in that cancellation is a state not an
             # event.
             if self._cancel_requested and temporalio.exceptions.is_cancelled_exception(
                 err
             ):
                 self._add_command().cancel_workflow_execution.SetInParent()
-            elif isinstance(err, temporalio.exceptions.FailureError):
+            elif self._is_workflow_failure_exception(err):
                 # All other failure errors fail the workflow
                 self._set_workflow_failure(err)
             else:
                 # All other exceptions fail the task
                 self._current_activation_error = err
-        except BaseException as err:
-            # During tear down, generator exit and no-runtime exceptions can appear
-            if not self._deleting:
-                raise
-            if not isinstance(
-                err, (GeneratorExit, temporalio.workflow._NotInWorkflowEventLoopError)
-            ):
-                logger.debug(
-                    "Ignoring exception while deleting workflow", exc_info=True
-                )
 
-    def _set_workflow_failure(self, err: temporalio.exceptions.FailureError) -> None:
+    def _set_workflow_failure(self, err: BaseException) -> None:
         # All other failure errors fail the workflow
         failure = self._add_command().fail_workflow_execution.failure
         failure.SetInParent()
         try:
             self._failure_converter.to_failure(err, self._payload_converter, failure)
         except Exception as inner_err:
             raise ValueError("Failed converting workflow exception") from inner_err
@@ -1748,15 +1799,17 @@
 
     def call_soon(
         self,
         callback: Callable[..., Any],
         *args: Any,
         context: Optional[contextvars.Context] = None,
     ) -> asyncio.Handle:
-        self._assert_not_read_only("schedule task")
+        # We need to allow this during delete because this is how tasks schedule
+        # entire cancellation calls
+        self._assert_not_read_only("schedule task", allow_during_delete=True)
         handle = asyncio.Handle(callback, args, self, context)
         self._ready.append(handle)
         return handle
 
     def call_later(
         self,
         delay: float,
@@ -1852,14 +1905,17 @@
             else:
                 value = repr(value)
             log_lines.append(f"{key}: {value}")
 
         logger.error("\n".join(log_lines), exc_info=exc_info)
 
     def call_exception_handler(self, context: _Context) -> None:
+        # Do nothing with any uncaught exceptions while deleting
+        if self._deleting:
+            return
         # Copied and slightly modified from
         # asyncio.BaseEventLoop.call_exception_handler
         if self._exception_handler is None:
             try:
                 self.default_exception_handler(context)
             except (SystemExit, KeyboardInterrupt):
                 raise
@@ -2041,20 +2097,23 @@
         self._seq = instance._next_seq("activity")
         self._input = input
         self._result_fut = instance.create_future()
         self._started = False
         instance._register_task(self, name=f"activity: {input.activity}")
 
     def cancel(self, msg: Optional[Any] = None) -> bool:
-        self._instance._assert_not_read_only("cancel activity handle")
-        # We override this because if it's not yet started and not done, we need
-        # to send a cancel command because the async function won't run to trap
-        # the cancel (i.e. cancelled before started)
-        if not self._started and not self.done():
-            self._apply_cancel_command(self._instance._add_command())
+        # Allow the cancel to go through for the task even if we're deleting,
+        # just don't do any commands
+        if not self._instance._deleting:
+            self._instance._assert_not_read_only("cancel activity handle")
+            # We override this because if it's not yet started and not done, we need
+            # to send a cancel command because the async function won't run to trap
+            # the cancel (i.e. cancelled before started)
+            if not self._started and not self.done():
+                self._apply_cancel_command(self._instance._add_command())
         # Message not supported in older versions
         if sys.version_info < (3, 9):
             return super().cancel()
         return super().cancel(msg)
 
     def _resolve_success(self, result: Any) -> None:
         # We intentionally let this error if already done
@@ -2412,116 +2471,146 @@
     def create_histogram(
         self, name: str, description: Optional[str] = None, unit: Optional[str] = None
     ) -> temporalio.common.MetricHistogram:
         return _ReplaySafeMetricHistogram(
             self._underlying.create_histogram(name, description, unit)
         )
 
+    def create_histogram_float(
+        self, name: str, description: Optional[str] = None, unit: Optional[str] = None
+    ) -> temporalio.common.MetricHistogramFloat:
+        return _ReplaySafeMetricHistogramFloat(
+            self._underlying.create_histogram_float(name, description, unit)
+        )
+
+    def create_histogram_timedelta(
+        self, name: str, description: Optional[str] = None, unit: Optional[str] = None
+    ) -> temporalio.common.MetricHistogramTimedelta:
+        return _ReplaySafeMetricHistogramTimedelta(
+            self._underlying.create_histogram_timedelta(name, description, unit)
+        )
+
     def create_gauge(
         self, name: str, description: Optional[str] = None, unit: Optional[str] = None
     ) -> temporalio.common.MetricGauge:
         return _ReplaySafeMetricGauge(
             self._underlying.create_gauge(name, description, unit)
         )
 
+    def create_gauge_float(
+        self, name: str, description: Optional[str] = None, unit: Optional[str] = None
+    ) -> temporalio.common.MetricGaugeFloat:
+        return _ReplaySafeMetricGaugeFloat(
+            self._underlying.create_gauge_float(name, description, unit)
+        )
+
     def with_additional_attributes(
         self, additional_attributes: temporalio.common.MetricAttributes
     ) -> temporalio.common.MetricMeter:
         return _ReplaySafeMetricMeter(
             self._underlying.with_additional_attributes(additional_attributes)
         )
 
 
-class _ReplaySafeMetricCounter(temporalio.common.MetricCounter):
-    def __init__(self, underlying: temporalio.common.MetricCounter) -> None:
+_MetricType = TypeVar("_MetricType", bound=temporalio.common.MetricCommon)
+
+
+class _ReplaySafeMetricCommon(temporalio.common.MetricCommon, Generic[_MetricType]):
+    def __init__(self, underlying: _MetricType) -> None:
         self._underlying = underlying
 
     @property
     def name(self) -> str:
         return self._underlying.name
 
     @property
     def description(self) -> Optional[str]:
         return self._underlying.description
 
     @property
     def unit(self) -> Optional[str]:
         return self._underlying.unit
 
+    def with_additional_attributes(
+        self, additional_attributes: temporalio.common.MetricAttributes
+    ) -> Self:
+        return self.__class__(
+            self._underlying.with_additional_attributes(additional_attributes)
+        )
+
+
+class _ReplaySafeMetricCounter(
+    temporalio.common.MetricCounter,
+    _ReplaySafeMetricCommon[temporalio.common.MetricCounter],
+):
     def add(
         self,
         value: int,
         additional_attributes: Optional[temporalio.common.MetricAttributes] = None,
     ) -> None:
         if not temporalio.workflow.unsafe.is_replaying():
             self._underlying.add(value, additional_attributes)
 
-    def with_additional_attributes(
-        self, additional_attributes: temporalio.common.MetricAttributes
-    ) -> temporalio.common.MetricCounter:
-        return _ReplaySafeMetricCounter(
-            self._underlying.with_additional_attributes(additional_attributes)
-        )
-
-
-class _ReplaySafeMetricHistogram(temporalio.common.MetricHistogram):
-    def __init__(self, underlying: temporalio.common.MetricHistogram) -> None:
-        self._underlying = underlying
-
-    @property
-    def name(self) -> str:
-        return self._underlying.name
-
-    @property
-    def description(self) -> Optional[str]:
-        return self._underlying.description
-
-    @property
-    def unit(self) -> Optional[str]:
-        return self._underlying.unit
 
+class _ReplaySafeMetricHistogram(
+    temporalio.common.MetricHistogram,
+    _ReplaySafeMetricCommon[temporalio.common.MetricHistogram],
+):
     def record(
         self,
         value: int,
         additional_attributes: Optional[temporalio.common.MetricAttributes] = None,
     ) -> None:
         if not temporalio.workflow.unsafe.is_replaying():
             self._underlying.record(value, additional_attributes)
 
-    def with_additional_attributes(
-        self, additional_attributes: temporalio.common.MetricAttributes
-    ) -> temporalio.common.MetricHistogram:
-        return _ReplaySafeMetricHistogram(
-            self._underlying.with_additional_attributes(additional_attributes)
-        )
-
 
-class _ReplaySafeMetricGauge(temporalio.common.MetricGauge):
-    def __init__(self, underlying: temporalio.common.MetricGauge) -> None:
-        self._underlying = underlying
+class _ReplaySafeMetricHistogramFloat(
+    temporalio.common.MetricHistogramFloat,
+    _ReplaySafeMetricCommon[temporalio.common.MetricHistogramFloat],
+):
+    def record(
+        self,
+        value: float,
+        additional_attributes: Optional[temporalio.common.MetricAttributes] = None,
+    ) -> None:
+        if not temporalio.workflow.unsafe.is_replaying():
+            self._underlying.record(value, additional_attributes)
 
-    @property
-    def name(self) -> str:
-        return self._underlying.name
 
-    @property
-    def description(self) -> Optional[str]:
-        return self._underlying.description
+class _ReplaySafeMetricHistogramTimedelta(
+    temporalio.common.MetricHistogramTimedelta,
+    _ReplaySafeMetricCommon[temporalio.common.MetricHistogramTimedelta],
+):
+    def record(
+        self,
+        value: timedelta,
+        additional_attributes: Optional[temporalio.common.MetricAttributes] = None,
+    ) -> None:
+        if not temporalio.workflow.unsafe.is_replaying():
+            self._underlying.record(value, additional_attributes)
 
-    @property
-    def unit(self) -> Optional[str]:
-        return self._underlying.unit
 
+class _ReplaySafeMetricGauge(
+    temporalio.common.MetricGauge,
+    _ReplaySafeMetricCommon[temporalio.common.MetricGauge],
+):
     def set(
         self,
         value: int,
         additional_attributes: Optional[temporalio.common.MetricAttributes] = None,
     ) -> None:
         if not temporalio.workflow.unsafe.is_replaying():
             self._underlying.set(value, additional_attributes)
 
-    def with_additional_attributes(
-        self, additional_attributes: temporalio.common.MetricAttributes
-    ) -> temporalio.common.MetricGauge:
-        return _ReplaySafeMetricGauge(
-            self._underlying.with_additional_attributes(additional_attributes)
-        )
+
+class _ReplaySafeMetricGaugeFloat(
+    temporalio.common.MetricGaugeFloat,
+    _ReplaySafeMetricCommon[temporalio.common.MetricGaugeFloat],
+):
+    def set(
+        self,
+        value: float,
+        additional_attributes: Optional[temporalio.common.MetricAttributes] = None,
+    ) -> None:
+        if not temporalio.workflow.unsafe.is_replaying():
+            self._underlying.set(value, additional_attributes)
```

### Comparing `temporalio-1.5.1/temporalio/worker/workflow_sandbox/__init__.py` & `temporalio-1.6.0/temporalio/worker/workflow_sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/worker/workflow_sandbox/_importer.py` & `temporalio-1.6.0/temporalio/worker/workflow_sandbox/_importer.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/worker/workflow_sandbox/_restrictions.py` & `temporalio-1.6.0/temporalio/worker/workflow_sandbox/_restrictions.py`

 * *Files identical despite different names*

### Comparing `temporalio-1.5.1/temporalio/worker/workflow_sandbox/_runner.py` & `temporalio-1.6.0/temporalio/worker/workflow_sandbox/_runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 .. warning::
     This API for this module is considered unstable and may change in future.
 """
 
 from __future__ import annotations
 
 from datetime import datetime, timedelta, timezone
-from typing import Any, Type
+from typing import Any, Sequence, Type
 
 import temporalio.bridge.proto.workflow_activation
 import temporalio.bridge.proto.workflow_completion
 import temporalio.common
 import temporalio.converter
 import temporalio.worker._workflow_instance
 import temporalio.workflow
@@ -64,14 +64,15 @@
             runner_class: The class for underlying runner the sandbox will
                 instantiate and  use to run workflows. Note, this class is
                 re-imported and instantiated for *each* workflow run.
         """
         super().__init__()
         self._runner_class = runner_class
         self._restrictions = restrictions
+        self._worker_level_failure_exception_types: Sequence[type[BaseException]] = []
 
     def prepare_workflow(self, defn: temporalio.workflow._Definition) -> None:
         """Implements :py:meth:`WorkflowRunner.prepare_workflow`."""
         # Just create with fake info which validates
         self.create_instance(
             WorkflowInstanceDetails(
                 payload_converter_class=temporalio.converter.DataConverter.default.payload_converter_class,
@@ -79,21 +80,28 @@
                 interceptor_classes=[],
                 defn=defn,
                 # Just use fake info during validation
                 info=_fake_info,
                 randomness_seed=-1,
                 extern_functions={},
                 disable_eager_activity_execution=False,
+                worker_level_failure_exception_types=self._worker_level_failure_exception_types,
             ),
         )
 
     def create_instance(self, det: WorkflowInstanceDetails) -> WorkflowInstance:
         """Implements :py:meth:`WorkflowRunner.create_instance`."""
         return _Instance(det, self._runner_class, self._restrictions)
 
+    def set_worker_level_failure_exception_types(
+        self, types: Sequence[type[BaseException]]
+    ) -> None:
+        """Implements :py:meth:`WorkflowRunner.set_worker_level_failure_exception_types`."""
+        self._worker_level_failure_exception_types = types
+
 
 # Implements in_sandbox._ExternEnvironment. Some of these calls are called from
 # within the sandbox.
 class _Instance(WorkflowInstance):
     def __init__(
         self,
         instance_details: WorkflowInstanceDetails,
```

### Comparing `temporalio-1.5.1/temporalio/workflow.py` & `temporalio-1.6.0/temporalio/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,18 @@
 @overload
 def defn(cls: ClassType) -> ClassType:
     ...
 
 
 @overload
 def defn(
-    *, name: Optional[str] = None, sandboxed: bool = True
+    *,
+    name: Optional[str] = None,
+    sandboxed: bool = True,
+    failure_exception_types: Sequence[Type[BaseException]] = [],
 ) -> Callable[[ClassType], ClassType]:
     ...
 
 
 @overload
 def defn(
     *, sandboxed: bool = True, dynamic: bool = False
@@ -97,14 +100,15 @@
 
 def defn(
     cls: Optional[ClassType] = None,
     *,
     name: Optional[str] = None,
     sandboxed: bool = True,
     dynamic: bool = False,
+    failure_exception_types: Sequence[Type[BaseException]] = [],
 ):
     """Decorator for workflow classes.
 
     This must be set on any registered workflow class (it is ignored if on a
     base class).
 
     Args:
@@ -112,22 +116,29 @@
         name: Name to use for the workflow. Defaults to class ``__name__``. This
             cannot be set if dynamic is set.
         sandboxed: Whether the workflow should run in a sandbox. Default is
             true.
         dynamic: If true, this activity will be dynamic. Dynamic workflows have
             to accept a single 'Sequence[RawValue]' parameter. This cannot be
             set to true if name is present.
+        failure_exception_types: The types of exceptions that, if a
+            workflow-thrown exception extends, will cause the workflow/update to
+            fail instead of suspending the workflow via task failure. These are
+            applied in addition to ones set on the worker constructor. If
+            ``Exception`` is set, it effectively will fail a workflow/update in
+            all user exception cases. WARNING: This setting is experimental.
     """
 
     def decorator(cls: ClassType) -> ClassType:
         # This performs validation
         _Definition._apply_to_class(
             cls,
             workflow_name=name or cls.__name__ if not dynamic else None,
             sandboxed=sandboxed,
+            failure_exception_types=failure_exception_types,
         )
         return cls
 
     if cls is not None:
         return decorator(cls)
     return decorator
 
@@ -1081,42 +1092,57 @@
 class LoggerAdapter(logging.LoggerAdapter):
     """Adapter that adds details to the log about the running workflow.
 
     Attributes:
         workflow_info_on_message: Boolean for whether a string representation of
             a dict of some workflow info will be appended to each message.
             Default is True.
-        workflow_info_on_extra: Boolean for whether a ``workflow_info`` value
-            will be added to the ``extra`` dictionary, making it present on the
-            ``LogRecord.__dict__`` for use by others.
+        workflow_info_on_extra: Boolean for whether a ``temporal_workflow``
+            dictionary value will be added to the ``extra`` dictionary with some
+            workflow info, making it present on the ``LogRecord.__dict__`` for
+            use by others. Default is True.
+        full_workflow_info_on_extra: Boolean for whether a ``workflow_info``
+            value will be added to the ``extra`` dictionary with the entire
+            workflow info, making it present on the ``LogRecord.__dict__`` for
+            use by others. Default is False.
         log_during_replay: Boolean for whether logs should occur during replay.
             Default is False.
     """
 
     def __init__(
         self, logger: logging.Logger, extra: Optional[Mapping[str, Any]]
     ) -> None:
         """Create the logger adapter."""
         super().__init__(logger, extra or {})
         self.workflow_info_on_message = True
         self.workflow_info_on_extra = True
+        self.full_workflow_info_on_extra = False
         self.log_during_replay = False
 
     def process(
         self, msg: Any, kwargs: MutableMapping[str, Any]
     ) -> Tuple[Any, MutableMapping[str, Any]]:
         """Override to add workflow details."""
-        if self.workflow_info_on_message or self.workflow_info_on_extra:
+        if (
+            self.workflow_info_on_message
+            or self.workflow_info_on_extra
+            or self.full_workflow_info_on_extra
+        ):
             runtime = _Runtime.maybe_current()
             if runtime:
                 if self.workflow_info_on_message:
                     msg = f"{msg} ({runtime.logger_details})"
                 if self.workflow_info_on_extra:
                     # Extra can be absent or None, this handles both
                     extra = kwargs.get("extra", None) or {}
+                    extra["temporal_workflow"] = runtime.logger_details
+                    kwargs["extra"] = extra
+                if self.full_workflow_info_on_extra:
+                    # Extra can be absent or None, this handles both
+                    extra = kwargs.get("extra", None) or {}
                     extra["workflow_info"] = runtime.workflow_info()
                     kwargs["extra"] = extra
         return (msg, kwargs)
 
     def isEnabledFor(self, level: int) -> bool:
         """Override to ignore replay logs."""
         if not self.log_during_replay and unsafe.is_replaying():
@@ -1143,14 +1169,15 @@
     name: Optional[str]
     cls: Type
     run_fn: Callable[..., Awaitable]
     signals: Mapping[Optional[str], _SignalDefinition]
     queries: Mapping[Optional[str], _QueryDefinition]
     updates: Mapping[Optional[str], _UpdateDefinition]
     sandboxed: bool
+    failure_exception_types: Sequence[Type[BaseException]]
     # Types loaded on post init if both are None
     arg_types: Optional[List[Type]] = None
     ret_type: Optional[Type] = None
 
     @staticmethod
     def from_class(cls: Type) -> Optional[_Definition]:
         # We make sure to only return it if it's on _this_ class
@@ -1181,15 +1208,19 @@
         fn_name = getattr(fn, "__qualname__", "<unknown>")
         raise ValueError(
             f"Function {fn_name} missing attributes, was it decorated with @workflow.run and was its class decorated with @workflow.defn?"
         )
 
     @staticmethod
     def _apply_to_class(
-        cls: Type, *, workflow_name: Optional[str], sandboxed: bool
+        cls: Type,
+        *,
+        workflow_name: Optional[str],
+        sandboxed: bool,
+        failure_exception_types: Sequence[Type[BaseException]],
     ) -> None:
         # Check it's not being doubly applied
         if _Definition.from_class(cls):
             raise ValueError("Class already contains workflow definition")
         issues: List[str] = []
 
         # Collect run fn and all signal/query/update fns
@@ -1304,14 +1335,15 @@
             name=workflow_name,
             cls=cls,
             run_fn=run_fn,
             signals=signals,
             queries=queries,
             updates=updates,
             sandboxed=sandboxed,
+            failure_exception_types=failure_exception_types,
         )
         setattr(cls, "__temporal_workflow_definition", defn)
         setattr(run_fn, "__temporal_workflow_definition", defn)
 
     def __post_init__(self) -> None:
         if self.arg_types is None and self.ret_type is None:
             dynamic = self.name is None
@@ -3843,15 +3875,15 @@
             temporalio.common.SearchAttributes, temporalio.common.TypedSearchAttributes
         ]
     ] = None,
     versioning_intent: Optional[VersioningIntent] = None,
 ) -> Any:
     """Start a child workflow and wait for completion.
 
-    This is a shortcut for ``await`` :py:meth:`start_child_workflow`.
+    This is a shortcut for ``await (await`` :py:meth:`start_child_workflow` ``)``.
     """
     temporalio.common._warn_on_deprecated_search_attributes(search_attributes)
     # We call the runtime directly instead of top-level start_child_workflow to
     # ensure we don't miss new parameters
     handle = await _Runtime.current().workflow_start_child_workflow(
         workflow,
         *temporalio.common._arg_or_args(arg, args),
```

### Comparing `temporalio-1.5.1/setup.py` & `temporalio-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
                        'sdk-core/core/src/test_help/*',
                        'sdk-core/core/src/worker/*',
                        'sdk-core/core/src/worker/activities/*',
                        'sdk-core/core/src/worker/client/*',
                        'sdk-core/core/src/worker/workflow/*',
                        'sdk-core/core/src/worker/workflow/machines/*',
                        'sdk-core/core/src/worker/workflow/machines/workflow_machines/*',
-                       'sdk-core/core/src/worker/workflow/workflow_stream/*',
                        'sdk-core/docker/*',
                        'sdk-core/etc/*',
                        'sdk-core/fsm/*',
                        'sdk-core/fsm/rustfsm_procmacro/*',
                        'sdk-core/fsm/rustfsm_procmacro/src/*',
                        'sdk-core/fsm/rustfsm_procmacro/tests/*',
                        'sdk-core/fsm/rustfsm_procmacro/tests/trybuild/*',
@@ -172,17 +171,17 @@
 {':python_version < "3.11"': ['python-dateutil>=2.8.2,<3.0.0'],
  'grpc': ['grpcio>=1.59.0,<2.0.0'],
  'opentelemetry': ['opentelemetry-api>=1.11.1,<2.0.0',
                    'opentelemetry-sdk>=1.11.1,<2.0.0']}
 
 setup_kwargs = {
     'name': 'temporalio',
-    'version': '1.5.1',
+    'version': '1.6.0',
     'description': 'Temporal.io Python SDK',
-    'long_description': '![Temporal Python SDK](https://assets.temporal.io/w/py-banner.svg)\n\n[![Python 3.8+](https://img.shields.io/pypi/pyversions/temporalio.svg?style=for-the-badge)](https://pypi.org/project/temporalio)\n[![PyPI](https://img.shields.io/pypi/v/temporalio.svg?style=for-the-badge)](https://pypi.org/project/temporalio)\n[![MIT](https://img.shields.io/pypi/l/temporalio.svg?style=for-the-badge)](LICENSE)\n\n[Temporal](https://temporal.io/) is a distributed, scalable, durable, and highly available orchestration engine used to\nexecute asynchronous, long-running business logic in a scalable and resilient way.\n\n"Temporal Python SDK" is the framework for authoring workflows and activities using the Python programming language.\n\nAlso see:\n* [Application Development Guide](https://docs.temporal.io/application-development?lang=python) - Once you\'ve tried our\n  [Quick Start](#quick-start), check out our guide on how to use Temporal in your Python applications, including\n  information around Temporal core concepts.\n* [Python Code Samples](https://github.com/temporalio/samples-python)\n* [API Documentation](https://python.temporal.io) - Complete Temporal Python SDK Package reference.\n\nIn addition to features common across all Temporal SDKs, the Python SDK also has the following interesting features:\n\n**Type Safe**\n\nThis library uses the latest typing and MyPy support with generics to ensure all calls can be typed. For example,\nstarting a workflow with an `int` parameter when it accepts a `str` parameter would cause MyPy to fail.\n\n**Different Activity Types**\n\nThe activity worker has been developed to work with `async def`, threaded, and multiprocess activities. While\n`async def` activities are the easiest and recommended, care has been taken to make heartbeating and cancellation also\nwork across threads/processes.\n\n**Custom `asyncio` Event Loop**\n\nThe workflow implementation basically turns `async def` functions into workflows backed by a distributed, fault-tolerant\nevent loop. This means task management, sleep, cancellation, etc have all been developed to seamlessly integrate with\n`asyncio` concepts.\n\nSee the [blog post](https://temporal.io/blog/durable-distributed-asyncio-event-loop) introducing the Python SDK for an\ninformal introduction to the features and their implementation.\n\n---\n\n<!-- START doctoc generated TOC please keep comment here to allow auto update -->\n<!-- DON\'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->\n**Contents**\n\n- [Quick Start](#quick-start)\n  - [Installation](#installation)\n  - [Implementing a Workflow](#implementing-a-workflow)\n  - [Running a Workflow](#running-a-workflow)\n  - [Next Steps](#next-steps)\n- [Usage](#usage)\n    - [Client](#client)\n      - [Data Conversion](#data-conversion)\n        - [Custom Type Data Conversion](#custom-type-data-conversion)\n    - [Workers](#workers)\n    - [Workflows](#workflows)\n      - [Definition](#definition)\n      - [Running](#running)\n      - [Invoking Activities](#invoking-activities)\n      - [Invoking Child Workflows](#invoking-child-workflows)\n      - [Timers](#timers)\n      - [Conditions](#conditions)\n      - [Asyncio and Cancellation](#asyncio-and-cancellation)\n      - [Workflow Utilities](#workflow-utilities)\n      - [Exceptions](#exceptions)\n      - [External Workflows](#external-workflows)\n      - [Testing](#testing)\n        - [Automatic Time Skipping](#automatic-time-skipping)\n        - [Manual Time Skipping](#manual-time-skipping)\n        - [Mocking Activities](#mocking-activities)\n      - [Workflow Sandbox](#workflow-sandbox)\n        - [How the Sandbox Works](#how-the-sandbox-works)\n        - [Avoiding the Sandbox](#avoiding-the-sandbox)\n        - [Customizing the Sandbox](#customizing-the-sandbox)\n          - [Passthrough Modules](#passthrough-modules)\n          - [Invalid Module Members](#invalid-module-members)\n        - [Known Sandbox Issues](#known-sandbox-issues)\n          - [Global Import/Builtins](#global-importbuiltins)\n          - [Sandbox is not Secure](#sandbox-is-not-secure)\n          - [Sandbox Performance](#sandbox-performance)\n          - [Extending Restricted Classes](#extending-restricted-classes)\n          - [Certain Standard Library Calls on Restricted Objects](#certain-standard-library-calls-on-restricted-objects)\n          - [is_subclass of ABC-based Restricted Classes](#is_subclass-of-abc-based-restricted-classes)\n          - [Compiled Pydantic Sometimes Using Wrong Types](#compiled-pydantic-sometimes-using-wrong-types)\n    - [Activities](#activities)\n      - [Definition](#definition-1)\n      - [Types of Activities](#types-of-activities)\n        - [Synchronous Activities](#synchronous-activities)\n          - [Synchronous Multithreaded Activities](#synchronous-multithreaded-activities)\n          - [Synchronous Multiprocess/Other Activities](#synchronous-multiprocessother-activities)\n        - [Asynchronous Activities](#asynchronous-activities)\n      - [Activity Context](#activity-context)\n        - [Heartbeating and Cancellation](#heartbeating-and-cancellation)\n        - [Worker Shutdown](#worker-shutdown)\n      - [Testing](#testing-1)\n    - [Workflow Replay](#workflow-replay)\n    - [OpenTelemetry Support](#opentelemetry-support)\n    - [Protobuf 3.x vs 4.x](#protobuf-3x-vs-4x)\n    - [Known Compatibility Issues](#known-compatibility-issues)\n      - [gevent Patching](#gevent-patching)\n- [Development](#development)\n    - [Building](#building)\n      - [Prepare](#prepare)\n      - [Build](#build)\n      - [Use](#use)\n    - [Local SDK development environment](#local-sdk-development-environment)\n      - [Testing](#testing-2)\n      - [Proto Generation and Testing](#proto-generation-and-testing)\n    - [Style](#style)\n\n<!-- END doctoc generated TOC please keep comment here to allow auto update -->\n\n# Quick Start\n\nWe will guide you through the Temporal basics to create a "hello, world!" script on your machine. It is not intended as\none of the ways to use Temporal, but in reality it is very simplified and decidedly not "the only way" to use Temporal.\nFor more information, check out the docs references in "Next Steps" below the quick start.\n\n## Installation\n\nInstall the `temporalio` package from [PyPI](https://pypi.org/project/temporalio).\n\nThese steps can be followed to use with a virtual environment and `pip`:\n\n* [Create a virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments)\n* Update `pip` - `python -m pip install -U pip`\n  * Needed because older versions of `pip` may not pick the right wheel\n* Install Temporal SDK - `python -m pip install temporalio`\n\nThe SDK is now ready for use. To build from source, see "Building" near the end of this documentation.\n\n**NOTE: This README is for the current branch and not necessarily what\'s released on `PyPI`.**\n\n## Implementing a Workflow\n\nCreate the following in `activities.py`:\n\n```python\nfrom temporalio import activity\n\n@activity.defn\ndef say_hello(name: str) -> str:\n    return f"Hello, {name}!"\n```\n\nCreate the following in `workflows.py`:\n\n```python\nfrom datetime import timedelta\nfrom temporalio import workflow\n\n# Import our activity, passing it through the sandbox\nwith workflow.unsafe.imports_passed_through():\n    from .activities import say_hello\n\n@workflow.defn\nclass SayHello:\n    @workflow.run\n    async def run(self, name: str) -> str:\n        return await workflow.execute_activity(\n            say_hello, name, schedule_to_close_timeout=timedelta(seconds=5)\n        )\n```\n\nCreate the following in `run_worker.py`:\n\n```python\nimport asyncio\nimport concurrent.futures\nfrom temporalio.client import Client\nfrom temporalio.worker import Worker\n\n# Import the activity and workflow from our other files\nfrom .activities import say_hello\nfrom .workflows import SayHello\n\nasync def main():\n    # Create client connected to server at the given address\n    client = await Client.connect("localhost:7233")\n\n    # Run the worker\n    with concurrent.futures.ThreadPoolExecutor(max_workers=100) as activity_executor:\n        worker = Worker(\n          client,\n          task_queue="my-task-queue",\n          workflows=[SayHello],\n          activities=[say_hello],\n          activity_executor=activity_executor,\n        )\n        await worker.run()\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nAssuming you have a [Temporal server running on localhost](https://docs.temporal.io/docs/server/quick-install/), this\nwill run the worker:\n\n    python run_worker.py\n\n## Running a Workflow\n\nCreate the following script at `run_workflow.py`:\n\n```python\nimport asyncio\nfrom temporalio.client import Client\n\n# Import the workflow from the previous code\nfrom .workflows import SayHello\n\nasync def main():\n    # Create client connected to server at the given address\n    client = await Client.connect("localhost:7233")\n\n    # Execute a workflow\n    result = await client.execute_workflow(SayHello.run, "my name", id="my-workflow-id", task_queue="my-task-queue")\n\n    print(f"Result: {result}")\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nAssuming you have `run_worker.py` running from before, this will run the workflow:\n\n    python run_workflow.py\n\nThe output will be:\n\n    Result: Hello, my-name!\n\n## Next Steps\n\nTemporal can be implemented in your code in many different ways, to suit your application\'s needs. The links below will\ngive you much more information about how Temporal works with Python:\n\n* [Code Samples](https://github.com/temporalio/samples-python) - If you want to start with some code, we have provided\n  some pre-built samples.\n* [Application Development Guide](https://docs.temporal.io/application-development?lang=python) Our Python specific\n  Developer\'s Guide will give you much more information on how to build with Temporal in your Python applications than\n  our SDK README ever could (or should).\n* [API Documentation](https://python.temporal.io) - Full Temporal Python SDK package documentation.\n\n---\n\n# Usage\n\nFrom here, you will find reference documentation about specific pieces of the Temporal Python SDK that were built around\nTemporal concepts. *This section is not intended as a how-to guide* -- For more how-to oriented information, check out\nthe links in the [Next Steps](#next-steps) section above.\n\n### Client\n\nA client can be created and used to start a workflow like so:\n\n```python\nfrom temporalio.client import Client\n\nasync def main():\n    # Create client connected to server at the given address and namespace\n    client = await Client.connect("localhost:7233", namespace="my-namespace")\n\n    # Start a workflow\n    handle = await client.start_workflow(MyWorkflow.run, "some arg", id="my-workflow-id", task_queue="my-task-queue")\n\n    # Wait for result\n    result = await handle.result()\n    print(f"Result: {result}")\n```\n\nSome things to note about the above code:\n\n* A `Client` does not have an explicit "close"\n* To enable TLS, the `tls` argument to `connect` can be set to `True` or a `TLSConfig` object\n* A single positional argument can be passed to `start_workflow`. If there are multiple arguments, only the\n  non-type-safe form of `start_workflow` can be used (i.e. the one accepting a string workflow name) and it must be in\n  the `args` keyword argument.\n* The `handle` represents the workflow that was started and can be used for more than just getting the result\n* Since we are just getting the handle and waiting on the result, we could have called `client.execute_workflow` which\n  does the same thing\n* Clients can have many more options not shown here (e.g. data converters and interceptors)\n* A string can be used instead of the method reference to call a workflow by name (e.g. if defined in another language)\n* Clients do not work across forks\n\nClients also provide a shallow copy of their config for use in making slightly different clients backed by the same\nconnection. For instance, given the `client` above, this is how to have a client in another namespace:\n\n```python\nconfig = client.config()\nconfig["namespace"] = "my-other-namespace"\nother_ns_client = Client(**config)\n```\n\n#### Data Conversion\n\nData converters are used to convert raw Temporal payloads to/from actual Python types. A custom data converter of type\n`temporalio.converter.DataConverter` can be set via the `data_converter` client parameter. Data converters are a\ncombination of payload converters, payload codecs, and failure converters. Payload converters convert Python values\nto/from serialized bytes. Payload codecs convert bytes to bytes (e.g. for compression or encryption). Failure converters\nconvert exceptions to/from serialized failures.\n\nThe default data converter supports converting multiple types including:\n\n* `None`\n* `bytes`\n* `google.protobuf.message.Message` - As JSON when encoding, but has ability to decode binary proto from other languages\n* Anything that can be converted to JSON including:\n  * Anything that [`json.dump`](https://docs.python.org/3/library/json.html#json.dump) supports natively\n  * [dataclasses](https://docs.python.org/3/library/dataclasses.html)\n  * Iterables including ones JSON dump may not support by default, e.g. `set`\n  * Any class with a `dict()` method and a static `parse_obj()` method, e.g.\n    [Pydantic models](https://pydantic-docs.helpmanual.io/usage/models)\n    * The default data converter is deprecated for Pydantic models and will warn if used since not all fields work.\n      See [this sample](https://github.com/temporalio/samples-python/tree/main/pydantic_converter) for the recommended\n      approach.\n  * [IntEnum, StrEnum](https://docs.python.org/3/library/enum.html) based enumerates\n  * [UUID](https://docs.python.org/3/library/uuid.html)\n\nThis notably doesn\'t include any `date`, `time`, or `datetime` objects as they may not work across SDKs.\n\nUsers are strongly encouraged to use a single `dataclass` for parameter and return types so fields with defaults can be\neasily added without breaking compatibility.\n\nClasses with generics may not have the generics properly resolved. The current implementation does not have generic\ntype resolution. Users should use concrete types.\n\n##### Custom Type Data Conversion\n\nFor converting from JSON, the workflow/activity type hint is taken into account to convert to the proper type. Care has\nbeen taken to support all common typings including `Optional`, `Union`, all forms of iterables and mappings, `NewType`,\netc in addition to the regular JSON values mentioned before.\n\nData converters contain a reference to a payload converter class that is used to convert to/from payloads/values. This\nis a class and not an instance because it is instantiated on every workflow run inside the sandbox. The payload\nconverter is usually a `CompositePayloadConverter` which contains a multiple `EncodingPayloadConverter`s it uses to try\nto serialize/deserialize payloads. Upon serialization, each `EncodingPayloadConverter` is tried until one succeeds. The\n`EncodingPayloadConverter` provides an "encoding" string serialized onto the payload so that, upon deserialization, the\nspecific `EncodingPayloadConverter` for the given "encoding" is used.\n\nThe default data converter uses the `DefaultPayloadConverter` which is simply a `CompositePayloadConverter` with a known\nset of default `EncodingPayloadConverter`s. To implement a custom encoding for a custom type, a new\n`EncodingPayloadConverter` can be created for the new type. For example, to support `IPv4Address` types:\n\n```python\nclass IPv4AddressEncodingPayloadConverter(EncodingPayloadConverter):\n    @property\n    def encoding(self) -> str:\n        return "text/ipv4-address"\n\n    def to_payload(self, value: Any) -> Optional[Payload]:\n        if isinstance(value, ipaddress.IPv4Address):\n            return Payload(\n                metadata={"encoding": self.encoding.encode()},\n                data=str(value).encode(),\n            )\n        else:\n            return None\n\n    def from_payload(self, payload: Payload, type_hint: Optional[Type] = None) -> Any:\n        assert not type_hint or type_hint is ipaddress.IPv4Address\n        return ipaddress.IPv4Address(payload.data.decode())\n\nclass IPv4AddressPayloadConverter(CompositePayloadConverter):\n    def __init__(self) -> None:\n        # Just add ours as first before the defaults\n        super().__init__(\n            IPv4AddressEncodingPayloadConverter(),\n            *DefaultPayloadConverter.default_encoding_payload_converters,\n        )\n\nmy_data_converter = dataclasses.replace(\n    DataConverter.default,\n    payload_converter_class=IPv4AddressPayloadConverter,\n)\n```\n\nImports are left off for brevity.\n\nThis is good for many custom types. However, sometimes you want to override the behavior of the just the existing JSON\nencoding payload converter to support a new type. It is already the last encoding data converter in the list, so it\'s\nthe fall-through behavior for any otherwise unknown type. Customizing the existing JSON converter has the benefit of\nmaking the type work in lists, unions, etc.\n\nThe `JSONPlainPayloadConverter` uses the Python [json](https://docs.python.org/3/library/json.html) library with an\nadvanced JSON encoder by default and a custom value conversion method to turn `json.load`ed values to their type hints.\nThe conversion can be customized for serialization with a custom `json.JSONEncoder` and deserialization with a custom\n`JSONTypeConverter`. For example, to support `IPv4Address` types in existing JSON conversion:\n\n```python\nclass IPv4AddressJSONEncoder(AdvancedJSONEncoder):\n    def default(self, o: Any) -> Any:\n        if isinstance(o, ipaddress.IPv4Address):\n            return str(o)\n        return super().default(o)\nclass IPv4AddressJSONTypeConverter(JSONTypeConverter):\n    def to_typed_value(\n        self, hint: Type, value: Any\n    ) -> Union[Optional[Any], _JSONTypeConverterUnhandled]:\n        if issubclass(hint, ipaddress.IPv4Address):\n            return ipaddress.IPv4Address(value)\n        return JSONTypeConverter.Unhandled\n\nclass IPv4AddressPayloadConverter(CompositePayloadConverter):\n    def __init__(self) -> None:\n        # Replace default JSON plain with our own that has our encoder and type\n        # converter\n        json_converter = JSONPlainPayloadConverter(\n            encoder=IPv4AddressJSONEncoder,\n            custom_type_converters=[IPv4AddressJSONTypeConverter()],\n        )\n        super().__init__(\n            *[\n                c if not isinstance(c, JSONPlainPayloadConverter) else json_converter\n                for c in DefaultPayloadConverter.default_encoding_payload_converters\n            ]\n        )\n\nmy_data_converter = dataclasses.replace(\n    DataConverter.default,\n    payload_converter_class=IPv4AddressPayloadConverter,\n)\n```\n\nNow `IPv4Address` can be used in type hints including collections, optionals, etc.\n\n### Workers\n\nWorkers host workflows and/or activities. Here\'s how to run a worker:\n\n```python\nimport asyncio\nimport logging\nfrom temporalio.client import Client\nfrom temporalio.worker import Worker\n# Import your own workflows and activities\nfrom my_workflow_package import MyWorkflow, my_activity\n\nasync def run_worker(stop_event: asyncio.Event):\n    # Create client connected to server at the given address\n    client = await Client.connect("localhost:7233", namespace="my-namespace")\n\n    # Run the worker until the event is set\n    worker = Worker(client, task_queue="my-task-queue", workflows=[MyWorkflow], activities=[my_activity])\n    async with worker:\n        await stop_event.wait()\n```\n\nSome things to note about the above code:\n\n* This creates/uses the same client that is used for starting workflows\n* While this example accepts a stop event and uses `async with`, `run()` and `shutdown()` may be used instead\n* Workers can have many more options not shown here (e.g. data converters and interceptors)\n\n### Workflows\n\n#### Definition\n\nWorkflows are defined as classes decorated with `@workflow.defn`. The method invoked for the workflow is decorated with\n`@workflow.run`. Methods for signals, queries, and updates are decorated with `@workflow.signal`, `@workflow.query`\nand `@workflow.update` respectively. Here\'s an example of a workflow:\n\n```python\nimport asyncio\nfrom datetime import timedelta\nfrom temporalio import workflow\n\n# Pass the activities through the sandbox\nwith workflow.unsafe.imports_passed_through():\n    from .my_activities import GreetingInfo, create_greeting_activity\n\n@workflow.defn\nclass GreetingWorkflow:\n    def __init__(self) -> None:\n        self._current_greeting = "<unset>"\n        self._greeting_info = GreetingInfo()\n        self._greeting_info_update = asyncio.Event()\n        self._complete = asyncio.Event()\n\n    @workflow.run\n    async def run(self, name: str) -> str:\n        self._greeting_info.name = name\n        while True:\n            # Store greeting\n            self._current_greeting = await workflow.execute_activity(\n                create_greeting_activity,\n                self._greeting_info,\n                start_to_close_timeout=timedelta(seconds=5),\n            )\n            workflow.logger.debug("Greeting set to %s", self._current_greeting)\n            \n            # Wait for salutation update or complete signal (this can be\n            # cancelled)\n            await asyncio.wait(\n                [\n                    asyncio.create_task(self._greeting_info_update.wait()),\n                    asyncio.create_task(self._complete.wait()),\n                ],\n                return_when=asyncio.FIRST_COMPLETED,\n            )\n            if self._complete.is_set():\n                return self._current_greeting\n            self._greeting_info_update.clear()\n\n    @workflow.signal\n    async def update_salutation(self, salutation: str) -> None:\n        self._greeting_info.salutation = salutation\n        self._greeting_info_update.set()\n\n    @workflow.signal\n    async def complete_with_greeting(self) -> None:\n        self._complete.set()\n\n    @workflow.query\n    def current_greeting(self) -> str:\n        return self._current_greeting\n    \n    @workflow.update\n    def set_and_get_greeting(self, greeting: str) -> str:\n      old = self._current_greeting\n      self._current_greeting = greeting\n      return old\n\n```\n\nThis assumes there\'s an activity in `my_activities.py` like:\n\n```python\nfrom dataclasses import dataclass\nfrom temporalio import workflow\n\n@dataclass\nclass GreetingInfo:\n    salutation: str = "Hello"\n    name: str = "<unknown>"\n\n@activity.defn\ndef create_greeting_activity(info: GreetingInfo) -> str:\n    return f"{info.salutation}, {info.name}!"\n```\n\nSome things to note about the above workflow code:\n\n* Workflows run in a sandbox by default.\n  * Users are encouraged to define workflows in files with no side effects or other complicated code or unnecessary\n    imports to other third party libraries.\n  * Non-standard-library, non-`temporalio` imports should usually be "passed through" the sandbox. See the\n    [Workflow Sandbox](#workflow-sandbox) section for more details.\n* This workflow continually updates the queryable current greeting when signalled and can complete with the greeting on\n  a different signal\n* Workflows are always classes and must have a single `@workflow.run` which is an `async def` function\n* Workflow code must be deterministic. This means no threading, no randomness, no external calls to processes, no\n  network IO, and no global state mutation. All code must run in the implicit `asyncio` event loop and be deterministic.\n* `@activity.defn` is explained in a later section. For normal simple string concatenation, this would just be done in\n  the workflow. The activity is for demonstration purposes only.\n* `workflow.execute_activity(create_greeting_activity, ...` is actually a typed signature, and MyPy will fail if the\n  `self._greeting_info` parameter is not a `GreetingInfo`\n\nHere are the decorators that can be applied:\n\n* `@workflow.defn` - Defines a workflow class\n  * Must be defined on the class given to the worker (ignored if present on a base class)\n  * Can have a `name` param to customize the workflow name, otherwise it defaults to the unqualified class name\n  * Can have `dynamic=True` which means all otherwise unhandled workflows fall through to this. If present, cannot have\n    `name` argument, and run method must accept a single parameter of `Sequence[temporalio.common.RawValue]` type. The\n    payload of the raw value can be converted via `workflow.payload_converter().from_payload`.\n* `@workflow.run` - Defines the primary workflow run method\n  * Must be defined on the same class as `@workflow.defn`, not a base class (but can _also_ be defined on the same\n    method of a base class)\n  * Exactly one method name must have this decorator, no more or less\n  * Must be defined on an `async def` method\n  * The method\'s arguments are the workflow\'s arguments\n  * The first parameter must be `self`, followed by positional arguments. Best practice is to only take a single\n    argument that is an object/dataclass of fields that can be added to as needed.\n* `@workflow.signal` - Defines a method as a signal\n  * Can be defined on an `async` or non-`async` function at any hierarchy depth, but if decorated method is overridden,\n    the override must also be decorated\n  * The method\'s arguments are the signal\'s arguments\n  * Can have a `name` param to customize the signal name, otherwise it defaults to the unqualified method name\n  * Can have `dynamic=True` which means all otherwise unhandled signals fall through to this. If present, cannot have\n    `name` argument, and method parameters must be `self`, a string signal name, and a\n    `Sequence[temporalio.common.RawValue]`.\n  * Non-dynamic method can only have positional arguments. Best practice is to only take a single argument that is an\n    object/dataclass of fields that can be added to as needed.\n  * Return value is ignored\n* `@workflow.query` - Defines a method as a query\n  * All the same constraints as `@workflow.signal` but should return a value\n  * Should not be `async`\n  * Temporal queries should never mutate anything in the workflow or call any calls that would mutate the workflow\n* `@workflow.update` - Defines a method as an update\n  * May both accept as input and return a value\n  * May be `async` or non-`async`\n  * May mutate workflow state, and make calls to other workflow APIs like starting activities, etc.\n  * Also accepts the `name` and `dynamic` parameters like signals and queries, with the same semantics.\n  * Update handlers may optionally define a validator method by decorating it with `@update_handler_method.validator`.\n    To reject an update before any events are written to history, throw an exception in a validator. Validators cannot \n    be `async`, cannot mutate workflow state, and return nothing.\n\n#### Running\n\nTo start a locally-defined workflow from a client, you can simply reference its method like so:\n\n```python\nfrom temporalio.client import Client\nfrom my_workflow_package import GreetingWorkflow\n\nasync def create_greeting(client: Client) -> str:\n    # Start the workflow\n    handle = await client.start_workflow(GreetingWorkflow.run, "my name", id="my-workflow-id", task_queue="my-task-queue")\n    # Change the salutation\n    await handle.signal(GreetingWorkflow.update_salutation, "Aloha")\n    # Tell it to complete\n    await handle.signal(GreetingWorkflow.complete_with_greeting)\n    # Wait and return result\n    return await handle.result()\n```\n\nSome things to note about the above code:\n\n* This uses the `GreetingWorkflow` from the previous section\n* The result of calling this function is `"Aloha, my name!"`\n* `id` and `task_queue` are required for running a workflow\n* `client.start_workflow` is typed, so MyPy would fail if `"my name"` were something besides a string\n* `handle.signal` is typed, so MyPy would fail if `"Aloha"` were something besides a string or if we provided a\n  parameter to the parameterless `complete_with_greeting`\n* `handle.result` is typed to the workflow itself, so MyPy would fail if we said this `create_greeting` returned\n  something besides a string\n\n#### Invoking Activities\n\n* Activities are started with non-async `workflow.start_activity()` which accepts either an activity function reference\n  or a string name.\n* A single argument to the activity is positional. Multiple arguments are not supported in the type-safe form of\n  start/execute activity and must be supplied via the `args` keyword argument.\n* Activity options are set as keyword arguments after the activity arguments. At least one of `start_to_close_timeout`\n  or `schedule_to_close_timeout` must be provided.\n* The result is an activity handle which is an `asyncio.Task` and supports basic task features\n* An async `workflow.execute_activity()` helper is provided which takes the same arguments as\n  `workflow.start_activity()` and `await`s on the result. This should be used in most cases unless advanced task\n  capabilities are needed.\n* Local activities work very similarly except the functions are `workflow.start_local_activity()` and\n  `workflow.execute_local_activity()`\n  * ⚠️Local activities are currently experimental\n* Activities can be methods of a class. Invokers should use `workflow.start_activity_method()`,\n  `workflow.execute_activity_method()`, `workflow.start_local_activity_method()`, and\n  `workflow.execute_local_activity_method()` instead.\n* Activities can callable classes (i.e. that define `__call__`). Invokers should use `workflow.start_activity_class()`,\n  `workflow.execute_activity_class()`, `workflow.start_local_activity_class()`, and\n  `workflow.execute_local_activity_class()` instead.\n\n#### Invoking Child Workflows\n\n* Child workflows are started with async `workflow.start_child_workflow()` which accepts either a workflow run method\n  reference or a string name. The arguments to the workflow are positional.\n* A single argument to the child workflow is positional. Multiple arguments are not supported in the type-safe form of\n  start/execute child workflow and must be supplied via the `args` keyword argument.\n* Child workflow options are set as keyword arguments after the arguments. At least `id` must be provided.\n* The `await` of the start does not complete until the start has been accepted by the server\n* The result is a child workflow handle which is an `asyncio.Task` and supports basic task features. The handle also has\n  some child info and supports signalling the child workflow\n* An async `workflow.execute_child_workflow()` helper is provided which takes the same arguments as\n  `workflow.start_child_workflow()` and `await`s on the result. This should be used in most cases unless advanced task\n  capabilities are needed.\n\n#### Timers\n\n* A timer is represented by normal `asyncio.sleep()`\n* Timers are also implicitly started on any `asyncio` calls with timeouts (e.g. `asyncio.wait_for`)\n* Timers are Temporal server timers, not local ones, so sub-second resolution rarely has value\n* Calls that use a specific point in time, e.g. `call_at` or `timeout_at`, should be based on the current loop time\n  (i.e. `workflow.time()`) and not an actual point in time. This is because fixed times are translated to relative ones\n  by subtracting the current loop time which may not be the actual current time.\n\n#### Conditions\n\n* `workflow.wait_condition` is an async function that doesn\'t return until a provided callback returns true\n* A `timeout` can optionally be provided which will throw a `asyncio.TimeoutError` if reached (internally backed by\n  `asyncio.wait_for` which uses a timer)\n\n#### Asyncio and Cancellation\n\nWorkflows are backed by a custom [asyncio](https://docs.python.org/3/library/asyncio.html) event loop. This means many\nof the common `asyncio` calls work as normal. Some asyncio features are disabled such as:\n\n* Thread related calls such as `to_thread()`, `run_coroutine_threadsafe()`, `loop.run_in_executor()`, etc\n* Calls that alter the event loop such as `loop.close()`, `loop.stop()`, `loop.run_forever()`,\n  `loop.set_task_factory()`, etc\n* Calls that use anything external such as networking, subprocesses, disk IO, etc\n\nCancellation is done the same way as `asyncio`. Specifically, a task can be requested to be cancelled but does not\nnecessarily have to respect that cancellation immediately. This also means that `asyncio.shield()` can be used to\nprotect against cancellation. The following tasks, when cancelled, perform a Temporal cancellation:\n\n* Activities - when the task executing an activity is cancelled, a cancellation request is sent to the activity\n* Child workflows - when the task starting or executing a child workflow is cancelled, a cancellation request is sent to\n  cancel the child workflow\n* Timers - when the task executing a timer is cancelled (whether started via sleep or timeout), the timer is cancelled\n\nWhen the workflow itself is requested to cancel, `Task.cancel` is called on the main workflow task. Therefore,\n`asyncio.CancelledError` can be caught in order to handle the cancel gracefully.\n\nWorkflows follow `asyncio` cancellation rules exactly which can cause confusion among Python developers. Cancelling a\ntask doesn\'t always cancel the thing it created. For example, given\n`task = asyncio.create_task(workflow.start_child_workflow(...`, calling `task.cancel` does not cancel the child\nworkflow, it only cancels the starting of it, which has no effect if it has already started. However, cancelling the\nresult of `handle = await workflow.start_child_workflow(...` or\n`task = asyncio.create_task(workflow.execute_child_workflow(...` _does_ cancel the child workflow.\n\nAlso, due to Temporal rules, a cancellation request is a state not an event. Therefore, repeated cancellation requests\nare not delivered, only the first. If the workflow chooses swallow a cancellation, it cannot be requested again.\n\n#### Workflow Utilities\n\nWhile running in a workflow, in addition to features documented elsewhere, the following items are available from the\n`temporalio.workflow` package:\n\n* `continue_as_new()` - Async function to stop the workflow immediately and continue as new\n* `info()` - Returns information about the current workflow\n* `logger` - A logger for use in a workflow (properly skips logging on replay)\n* `now()` - Returns the "current time" from the workflow\'s perspective\n\n#### Exceptions\n\n* Workflows can raise exceptions to fail the workflow or the "workflow task" (i.e. suspend the workflow retrying).\n* Exceptions that are instances of `temporalio.exceptions.FailureError` will fail the workflow with that exception\n  * For failing the workflow explicitly with a user exception, use `temporalio.exceptions.ApplicationError`. This can\n    be marked non-retryable or include details as needed.\n  * Other exceptions that come from activity execution, child execution, cancellation, etc are already instances of\n    `FailureError` and will fail the workflow when uncaught.\n* All other exceptions fail the "workflow task" which means the workflow will continually retry until the workflow is\n  fixed. This is helpful for bad code or other non-predictable exceptions. To actually fail the workflow, use an\n  `ApplicationError` as mentioned above.\n\n#### External Workflows\n\n* `workflow.get_external_workflow_handle()` inside a workflow returns a handle to interact with another workflow\n* `workflow.get_external_workflow_handle_for()` can be used instead for a type safe handle\n* `await handle.signal()` can be called on the handle to signal the external workflow\n* `await handle.cancel()` can be called on the handle to send a cancel to the external workflow\n\n#### Testing\n\nWorkflow testing can be done in an integration-test fashion against a real server, however it is hard to simulate\ntimeouts and other long time-based code. Using the time-skipping workflow test environment can help there.\n\nThe time-skipping `temporalio.testing.WorkflowEnvironment` can be created via the static async `start_time_skipping()`.\nThis internally downloads the Temporal time-skipping test server to a temporary directory if it doesn\'t already exist,\nthen starts the test server which has special APIs for skipping time.\n\n**NOTE:** The time-skipping test environment does not work on ARM. The SDK will try to download the x64 binary on macOS\nfor use with the Intel emulator, but for Linux or Windows ARM there is no proper time-skipping test server at this time.\n\n##### Automatic Time Skipping\n\nAnytime a workflow result is waited on, the time-skipping server automatically advances to the next event it can. To\nmanually advance time before waiting on the result of a workflow, the `WorkflowEnvironment.sleep` method can be used.\n\nHere\'s a simple example of a workflow that sleeps for 24 hours:\n\n```python\nimport asyncio\nfrom temporalio import workflow\n\n@workflow.defn\nclass WaitADayWorkflow:\n    @workflow.run\n    async def run(self) -> str:\n        await asyncio.sleep(24 * 60 * 60)\n        return "all done"\n```\n\nAn integration test of this workflow would be way too slow. However the time-skipping server automatically skips to the\nnext event when we wait on the result. Here\'s a test for that workflow:\n\n```python\nfrom temporalio.testing import WorkflowEnvironment\nfrom temporalio.worker import Worker\n\nasync def test_wait_a_day_workflow():\n    async with await WorkflowEnvironment.start_time_skipping() as env:\n        async with Worker(env.client, task_queue="tq1", workflows=[WaitADayWorkflow]):\n            assert "all done" == await env.client.execute_workflow(WaitADayWorkflow.run, id="wf1", task_queue="tq1")\n```\n\nThat test will run almost instantly. This is because by calling `execute_workflow` on our client, we have asked the\nenvironment to automatically skip time as much as it can (basically until the end of the workflow or until an activity\nis run).\n\nTo disable automatic time-skipping while waiting for a workflow result, run code inside a\n`with env.auto_time_skipping_disabled():` block.\n\n##### Manual Time Skipping\n\nUntil a workflow is waited on, all time skipping in the time-skipping environment is done manually via\n`WorkflowEnvironment.sleep`.\n\nHere\'s workflow that waits for a signal or times out:\n\n```python\nimport asyncio\nfrom temporalio import workflow\n\n@workflow.defn\nclass SignalWorkflow:\n    def __init__(self) -> None:\n        self.signal_received = False\n\n    @workflow.run\n    async def run(self) -> str:\n        # Wait for signal or timeout in 45 seconds\n        try:\n            await workflow.wait_condition(lambda: self.signal_received, timeout=45)\n            return "got signal"\n        except asyncio.TimeoutError:\n            return "got timeout"\n\n    @workflow.signal\n    def some_signal(self) -> None:\n        self.signal_received = True\n```\n\nTo test a normal signal, you might:\n\n```python\nfrom temporalio.testing import WorkflowEnvironment\nfrom temporalio.worker import Worker\n\nasync def test_signal_workflow():\n    async with await WorkflowEnvironment.start_time_skipping() as env:\n        async with Worker(env.client, task_queue="tq1", workflows=[SignalWorkflow]):\n            # Start workflow, send signal, check result\n            handle = await env.client.start_workflow(SignalWorkflow.run, id="wf1", task_queue="tq1")\n            await handle.signal(SignalWorkflow.some_signal)\n            assert "got signal" == await handle.result()\n```\n\nBut how would you test the timeout part? Like so:\n\n```python\nfrom temporalio.testing import WorkflowEnvironment\nfrom temporalio.worker import Worker\n\nasync def test_signal_workflow_timeout():\n    async with await WorkflowEnvironment.start_time_skipping() as env:\n        async with Worker(env.client, task_queue="tq1", workflows=[SignalWorkflow]):\n            # Start workflow, advance time past timeout, check result\n            handle = await env.client.start_workflow(SignalWorkflow.run, id="wf1", task_queue="tq1")\n            await env.sleep(50)\n            assert "got timeout" == await handle.result()\n```\n\nAlso, the current time of the workflow environment can be obtained via the async `WorkflowEnvironment.get_current_time`\nmethod.\n\n##### Mocking Activities\n\nActivities are just functions decorated with `@activity.defn`. Simply write different ones and pass those to the worker\nto have different activities called during the test.\n\n#### Workflow Sandbox\n\nBy default workflows are run in a sandbox to help avoid non-deterministic code. If a call that is known to be\nnon-deterministic is performed, an exception will be thrown in the workflow which will "fail the task" which means the\nworkflow will not progress until fixed.\n\nThe sandbox is not foolproof and non-determinism can still occur. It is simply a best-effort way to catch bad code\nearly. Users are encouraged to define their workflows in files with no other side effects.\n\nThe sandbox offers a mechanism to pass through modules from outside the sandbox. By default this already includes all\nstandard library modules and Temporal modules. **For performance and behavior reasons, users are encouraged to pass\nthrough all third party modules whose calls will be deterministic.** This includes modules containing the activities to\nbe referenced in workflows. See "Passthrough Modules" below on how to do this.\n\nIf you are getting an error like:\n\n> temporalio.worker.workflow_sandbox._restrictions.RestrictedWorkflowAccessError: Cannot access\n> http.client.IncompleteRead.\\_\\_mro_entries\\_\\_ from inside a workflow. If this is code from a module not used in a\n> workflow or known to only be used deterministically from a workflow, mark the import as pass through.\n\nThen you are either using an invalid construct from the workflow, this is a known limitation of the sandbox, or most\ncommonly this is from a module that is safe to pass through (see "Passthrough Modules" section below).\n\n##### How the Sandbox Works\n\nThe sandbox is made up of two components that work closely together:\n\n* Global state isolation\n* Restrictions preventing known non-deterministic library calls\n\nGlobal state isolation is performed by using `exec`. Upon workflow start, the file that the workflow is defined in is\nimported into a new sandbox created for that workflow run. In order to keep the sandbox performant a known set of\n"passthrough modules" are passed through from outside of the sandbox when they are imported. These are expected to be\nside-effect free on import and have their non-deterministic aspects restricted. By default the entire Python standard\nlibrary, `temporalio`, and a couple of other modules are passed through from outside of the sandbox. To update this\nlist, see "Customizing the Sandbox".\n\nRestrictions preventing known non-deterministic library calls are achieved using proxy objects on modules wrapped around\nthe custom importer set in the sandbox. Many restrictions apply at workflow import time and workflow run time, while\nsome restrictions only apply at workflow run time. A default set of restrictions is included that prevents most\ndangerous standard library calls. However it is known in Python that some otherwise-non-deterministic invocations, like\nreading a file from disk via `open` or using `os.environ`, are done as part of importing modules. To customize what is\nand isn\'t restricted, see "Customizing the Sandbox".\n\n##### Avoiding the Sandbox\n\nThere are three increasingly-scoped ways to avoid the sandbox. Users are discouraged from avoiding the sandbox if\npossible.\n\nTo remove restrictions around a particular block of code, use `with temporalio.workflow.unsafe.sandbox_unrestricted():`.\nThe workflow will still be running in the sandbox, but no restrictions for invalid library calls will be applied.\n\nTo run an entire workflow outside of a sandbox, set `sandboxed=False` on the `@workflow.defn` decorator when defining\nit. This will run the entire workflow outside of the workflow which means it can share global state and other bad\nthings.\n\nTo disable the sandbox entirely for a worker, set the `Worker` init\'s `workflow_runner` keyword argument to \n`temporalio.worker.UnsandboxedWorkflowRunner()`. This value is defaulted to\n`temporalio.worker.workflow_sandbox.SandboxedWorkflowRunner()` so by changing it to the unsandboxed runner, the sandbox\nwill not be used at all.\n\n##### Customizing the Sandbox\n\n⚠️ WARNING: APIs in the `temporalio.worker.workflow_sandbox` module are not yet considered stable and may change in\nfuture releases.\n\nWhen creating the `Worker`, the `workflow_runner` is defaulted to\n`temporalio.worker.workflow_sandbox.SandboxedWorkflowRunner()`. The `SandboxedWorkflowRunner`\'s init accepts a\n`restrictions` keyword argument that is defaulted to `SandboxRestrictions.default`. The `SandboxRestrictions` dataclass\nis immutable and contains three fields that can be customized, but only two have notable value. See below.\n\n###### Passthrough Modules\n\nBy default the sandbox completely reloads non-standard-library and non-Temporal modules for every workflow run. To make\nthe sandbox quicker and use less memory when importing known-side-effect-free third party modules, they can be marked\nas passthrough modules.\n\n**For performance and behavior reasons, users are encouraged to pass through all third party modules whose calls will be\ndeterministic.**\n\nOne way to pass through a module is at import time in the workflow file using the `imports_passed_through` context\nmanager like so:\n\n```python\n# my_workflow_file.py\n\nfrom temporalio import workflow\n\nwith workflow.unsafe.imports_passed_through():\n    import pydantic\n\n@workflow.defn\nclass MyWorkflow:\n    ...\n```\n\nAlternatively, this can be done at worker creation time by customizing the runner\'s restrictions. For example:\n\n```python\nmy_worker = Worker(\n  ...,\n  workflow_runner=SandboxedWorkflowRunner(\n    restrictions=SandboxRestrictions.default.with_passthrough_modules("pydantic")\n  )\n)\n```\n\nIn both of these cases, now the `pydantic` module will be passed through from outside of the sandbox instead of\nbeing reloaded for every workflow run.\n\n###### Invalid Module Members\n\n`SandboxRestrictions.invalid_module_members` contains a root matcher that applies to all module members. This already\nhas a default set which includes things like `datetime.date.today()` which should never be called from a workflow. To\nremove this restriction:\n\n```python\nmy_restrictions = dataclasses.replace(\n    SandboxRestrictions.default,\n    invalid_module_members=SandboxRestrictions.invalid_module_members_default.with_child_unrestricted(\n      "datetime", "date", "today",\n    ),\n)\nmy_worker = Worker(..., workflow_runner=SandboxedWorkflowRunner(restrictions=my_restrictions))\n```\n\nRestrictions can also be added by `|`\'ing together matchers, for example to restrict the `datetime.date` class from\nbeing used altogether:\n\n```python\nmy_restrictions = dataclasses.replace(\n    SandboxRestrictions.default,\n    invalid_module_members=SandboxRestrictions.invalid_module_members_default | SandboxMatcher(\n      children={"datetime": SandboxMatcher(use={"date"})},\n    ),\n)\nmy_worker = Worker(..., workflow_runner=SandboxedWorkflowRunner(restrictions=my_restrictions))\n```\n\nSee the API for more details on exact fields and their meaning.\n\n##### Known Sandbox Issues\n\nBelow are known sandbox issues. As the sandbox is developed and matures, some may be resolved.\n\n###### Global Import/Builtins\n\nCurrently the sandbox references/alters the global `sys.modules` and `builtins` fields while running workflow code. In\norder to prevent affecting other sandboxed code, thread locals are leveraged to only intercept these values during the\nworkflow thread running. Therefore, technically if top-level import code starts a thread, it may lose sandbox\nprotection.\n\n###### Sandbox is not Secure\n\nThe sandbox is built to catch many non-deterministic and state sharing issues, but it is not secure. Some known bad\ncalls are intercepted, but for performance reasons, every single attribute get/set cannot be checked. Therefore a simple\ncall like `setattr(temporalio.common, "__my_key", "my value")` will leak across sandbox runs.\n\nThe sandbox is only a helper, it does not provide full protection.\n\n###### Sandbox Performance\n\nThe sandbox does not add significant CPU or memory overhead for workflows that are in files which only import standard\nlibrary modules. This is because they are passed through from outside of the sandbox. However, every\nnon-standard-library import that is performed at the top of the same file the workflow is in will add CPU overhead (the\nmodule is re-imported every workflow run) and memory overhead (each module independently cached as part of the workflow\nrun for isolation reasons). This becomes more apparent for large numbers of workflow runs.\n\nTo mitigate this, users should:\n\n* Define workflows in files that have as few non-standard-library imports as possible\n* Alter the max workflow cache and/or max concurrent workflows settings if memory grows too large\n* Set third-party libraries as passthrough modules if they are known to be side-effect free\n\n###### Extending Restricted Classes\n\nExtending a restricted class causes Python to instantiate the restricted metaclass which is unsupported. Therefore if\nyou attempt to use a class in the sandbox that extends a restricted class, it will fail. For example, if you have a\n`class MyZipFile(zipfile.ZipFile)` and try to use that class inside a workflow, it will fail.\n\nClasses used inside the workflow should not extend restricted classes. For situations where third-party modules need to\nat import time, they should be marked as pass through modules.\n\n###### Certain Standard Library Calls on Restricted Objects\n\nIf an object is restricted, internal C Python validation may fail in some cases. For example, running\n`dict.items(os.__dict__)` will fail with:\n\n> descriptor \'items\' for \'dict\' objects doesn\'t apply to a \'_RestrictedProxy\' object\n\nThis is a low-level check that cannot be subverted. The solution is to not use restricted objects inside the sandbox.\nFor situations where third-party modules need to at import time, they should be marked as pass through modules.\n\n###### is_subclass of ABC-based Restricted Classes\n\nDue to [https://bugs.python.org/issue44847](https://bugs.python.org/issue44847), classes that are wrapped and then\nchecked to see if they are subclasses of another via `is_subclass` may fail (see also\n[this wrapt issue](https://github.com/GrahamDumpleton/wrapt/issues/130)).\n\n###### Compiled Pydantic Sometimes Using Wrong Types\n\nIf the Pydantic dependency is in compiled form (the default) and you are using a Pydantic model inside a workflow\nsandbox that uses a `datetime` type, it will grab the wrong validator and use `date` instead. This is because our\npatched form of `issubclass` is bypassed by compiled Pydantic.\n\nTo work around, either don\'t use `datetime`-based Pydantic model fields in workflows, or mark `datetime` library as\npassthrough (means you lose protection against calling the non-deterministic `now()`), or use non-compiled Pydantic\ndependency.\n\n### Activities\n\n#### Definition\n\nActivities are decorated with `@activity.defn` like so:\n\n```python\nfrom temporalio import activity\n\n@activity.defn\ndef say_hello_activity(name: str) -> str:\n    return f"Hello, {name}!"\n```\n\nSome things to note about activity definitions:\n\n* The `say_hello_activity` is synchronous which is the recommended activity type (see "Types of Activities" below), but\n  it can be `async`\n* A custom name for the activity can be set with a decorator argument, e.g. `@activity.defn(name="my activity")`\n* Long running activities should regularly heartbeat and handle cancellation\n* Activities can only have positional arguments. Best practice is to only take a single argument that is an\n  object/dataclass of fields that can be added to as needed.\n* Activities can be defined on methods instead of top-level functions. This allows the instance to carry state that an\n  activity may need (e.g. a DB connection). The instance method should be what is registered with the worker.\n* Activities can also be defined on callable classes (i.e. classes with `__call__`). An instance of the class should be\n  what is registered with the worker.\n* The `@activity.defn` can have `dynamic=True` set which means all otherwise unhandled activities fall through to this.\n  If present, cannot have `name` argument, and the activity function must accept a single parameter of\n  `Sequence[temporalio.common.RawValue]`. The payload of the raw value can be converted via\n  `activity.payload_converter().from_payload`.\n\n#### Types of Activities\n\nThere are 3 types of activity callables accepted and described below: synchronous multithreaded, synchronous\nmultiprocess/other, and asynchronous. Only positional parameters are allowed in activity callables.\n\n##### Synchronous Activities\n\nSynchronous activities, i.e. functions that do not have `async def`, can be used with workers, but the\n`activity_executor` worker parameter must be set with a `concurrent.futures.Executor` instance to use for executing the\nactivities.\n\nAll long running, non-local activities should heartbeat so they can be cancelled. Cancellation in threaded activities\nthrows but multiprocess/other activities does not. The sections below on each synchronous type explain further. There\nare also calls on the context that can check for cancellation. For more information, see "Activity Context" and\n"Heartbeating and Cancellation" sections later.\n\nNote, all calls from an activity to functions in the `temporalio.activity` package are powered by\n[contextvars](https://docs.python.org/3/library/contextvars.html). Therefore, new threads starting _inside_ of\nactivities must `copy_context()` and then `.run()` manually to ensure `temporalio.activity` calls like `heartbeat` still\nfunction in the new threads.\n\nIf any activity ever throws a `concurrent.futures.BrokenExecutor`, the failure is consisted unrecoverable and the worker\nwill fail and shutdown.\n\n###### Synchronous Multithreaded Activities\n\nIf `activity_executor` is set to an instance of `concurrent.futures.ThreadPoolExecutor` then the synchronous activities\nare considered multithreaded activities. If `max_workers` is not set to at least the worker\'s\n`max_concurrent_activities` setting a warning will be issued. Besides `activity_executor`, no other worker parameters\nare required for synchronous multithreaded activities.\n\nBy default, cancellation of a synchronous multithreaded activity is done via a `temporalio.exceptions.CancelledError`\nthrown into the activity thread. Activities that do not wish to have cancellation thrown can set\n`no_thread_cancel_exception=True` in the `@activity.defn` decorator.\n\nCode that wishes to be temporarily shielded from the cancellation exception can run inside\n`with activity.shield_thread_cancel_exception():`. But once the last nested form of that block is finished, even if\nthere is a return statement within, it will throw the cancellation if there was one. A `try` +\n`except temporalio.exceptions.CancelledError` would have to surround the `with` to handle the cancellation explicitly.\n\n###### Synchronous Multiprocess/Other Activities\n\nIf `activity_executor` is set to an instance of `concurrent.futures.Executor` that is _not_\n`concurrent.futures.ThreadPoolExecutor`, then the synchronous activities are considered multiprocess/other activities.\nUsers should prefer threaded activities over multiprocess ones since, among other reasons, threaded activities can raise\non cancellation.\n\nThese require special primitives for heartbeating and cancellation. The `shared_state_manager` worker parameter must be\nset to an instance of `temporalio.worker.SharedStateManager`. The most common implementation can be created by passing a\n`multiprocessing.managers.SyncManager` (i.e. result of `multiprocessing.managers.Manager()`) to\n`temporalio.worker.SharedStateManager.create_from_multiprocessing()`.\n\nAlso, all of these activity functions must be\n["picklable"](https://docs.python.org/3/library/pickle.html#what-can-be-pickled-and-unpickled).\n\n##### Asynchronous Activities\n\nAsynchronous activities are functions defined with `async def`. Asynchronous activities are often much more performant\nthan synchronous ones. When using asynchronous activities no special worker parameters are needed.\n\n**⚠️ WARNING: Do not block the thread in `async def` Python functions. This can stop the processing of the rest of the\nTemporal.**\n\nCancellation for asynchronous activities is done via\n[`asyncio.Task.cancel`](https://docs.python.org/3/library/asyncio-task.html#asyncio.Task.cancel). This means that\n`asyncio.CancelledError` will be raised (and can be caught, but it is not recommended). A non-local activity must\nheartbeat to receive cancellation and there are other ways to be notified about cancellation (see "Activity Context" and\n"Heartbeating and Cancellation" later).\n\n#### Activity Context\n\nDuring activity execution, an implicit activity context is set as a\n[context variable](https://docs.python.org/3/library/contextvars.html). The context variable itself is not visible, but\ncalls in the `temporalio.activity` package make use of it. Specifically:\n\n* `in_activity()` - Whether an activity context is present\n* `info()` - Returns the immutable info of the currently running activity\n* `heartbeat(*details)` - Record a heartbeat\n* `is_cancelled()` - Whether a cancellation has been requested on this activity\n* `wait_for_cancelled()` - `async` call to wait for cancellation request\n* `wait_for_cancelled_sync(timeout)` - Synchronous blocking call to wait for cancellation request\n* `shield_thread_cancel_exception()` - Context manager for use in `with` clauses by synchronous multithreaded activities\n  to prevent cancel exception from being thrown during the block of code\n* `is_worker_shutdown()` - Whether the worker has started graceful shutdown\n* `wait_for_worker_shutdown()` - `async` call to wait for start of graceful worker shutdown\n* `wait_for_worker_shutdown_sync(timeout)` - Synchronous blocking call to wait for start of graceful worker shutdown\n* `raise_complete_async()` - Raise an error that this activity will be completed asynchronously (i.e. after return of\n  the activity function in a separate client call)\n\nWith the exception of `in_activity()`, if any of the functions are called outside of an activity context, an error\noccurs. Synchronous activities cannot call any of the `async` functions.\n\n##### Heartbeating and Cancellation\n\nIn order for a non-local activity to be notified of cancellation requests, it must be given a `heartbeat_timeout` at\ninvocation time and invoke `temporalio.activity.heartbeat()` inside the activity. It is strongly recommended that all\nbut the fastest executing activities call this function regularly. "Types of Activities" has specifics on cancellation\nfor synchronous and asynchronous activities.\n\nIn addition to obtaining cancellation information, heartbeats also support detail data that is persisted on the server\nfor retrieval during activity retry. If an activity calls `temporalio.activity.heartbeat(123, 456)` and then fails and\nis retried, `temporalio.activity.info().heartbeat_details` will return an iterable containing `123` and `456` on the\nnext run.\n\nHeartbeating has no effect on local activities.\n\n##### Worker Shutdown\n\nAn activity can react to a worker shutdown. Using `is_worker_shutdown` or one of the `wait_for_worker_shutdown`\nfunctions an activity can react to a shutdown.\n\nWhen the `graceful_shutdown_timeout` worker parameter is given a `datetime.timedelta`, on shutdown the worker will\nnotify activities of the graceful shutdown. Once that timeout has passed (or if wasn\'t set), the worker will perform\ncancellation of all outstanding activities.\n\nThe `shutdown()` invocation will wait on all activities to complete, so if a long-running activity does not at least\nrespect cancellation, the shutdown may never complete.\n\n#### Testing\n\nUnit testing an activity or any code that could run in an activity is done via the\n`temporalio.testing.ActivityEnvironment` class. Simply instantiate this and any callable + params passed to `run` will\nbe invoked inside the activity context. The following are attributes/methods on the environment that can be used to\naffect calls activity code might make to functions on the `temporalio.activity` package.\n\n* `info` property can be set to customize what is returned from `activity.info()`\n* `on_heartbeat` property can be set to handle `activity.heartbeat()` calls\n* `cancel()` can be invoked to simulate a cancellation of the activity\n* `worker_shutdown()` can be invoked to simulate a worker shutdown during execution of the activity\n\n### Workflow Replay\n\nGiven a workflow\'s history, it can be replayed locally to check for things like non-determinism errors. For example,\nassuming `history_str` is populated with a JSON string history either exported from the web UI or from `tctl`, the\nfollowing function will replay it:\n\n```python\nfrom temporalio.client import WorkflowHistory\nfrom temporalio.worker import Replayer\n\nasync def run_replayer(history_str: str):\n  replayer = Replayer(workflows=[SayHello])\n  await replayer.replay_workflow(WorkflowHistory.from_json(history_str))\n```\n\nThis will throw an error if any non-determinism is detected.\n\nReplaying from workflow history is a powerful concept that many use to test that workflow alterations won\'t cause\nnon-determinisms with past-complete workflows. The following code will make sure that all workflow histories for a\ncertain workflow type (i.e. workflow class) are safe with the current code.\n\n```python\nfrom temporalio.client import Client, WorkflowHistory\nfrom temporalio.worker import Replayer\n\nasync def check_past_histories(my_client: Client):\n  replayer = Replayer(workflows=[SayHello])\n  await replayer.replay_workflows(\n    await my_client.list_workflows("WorkflowType = \'SayHello\'").map_histories(),\n  )\n```\n\n### OpenTelemetry Support\n\nOpenTelemetry support requires the optional `opentelemetry` dependencies which are part of the `opentelemetry` extra.\nWhen using `pip`, running\n\n    pip install temporalio[opentelemetry]\n\nwill install needed dependencies. Then the `temporalio.contrib.opentelemetry.TracingInterceptor` can be created and set\nas an interceptor on the `interceptors` argument of `Client.connect`. When set, spans will be created for all client\ncalls and for all activity and workflow invocations on the worker, spans will be created and properly serialized through\nthe server to give one proper trace for a workflow execution.\n\n### Protobuf 3.x vs 4.x\n\nPython currently has two somewhat-incompatible protobuf library versions - the 3.x series and the 4.x series. Python\ncurrently recommends 4.x and that is the primary supported version. Some libraries like\n[Pulumi](https://github.com/pulumi/pulumi) require 4.x. Other libraries such as [ONNX](https://github.com/onnx/onnx) and\n[Streamlit](https://github.com/streamlit/streamlit), for one reason or another, have/will not leave 3.x.\n\nTo support these, Temporal Python SDK allows any protobuf library >= 3.19. However, the C extension in older Python\nversions can cause issues with the sandbox due to global state sharing. Temporal strongly recommends using the latest\nprotobuf 4.x library unless you absolutely cannot at which point some proto libraries may have to be marked as\n[Passthrough Modules](#passthrough-modules).\n\n### Known Compatibility Issues\n\nBelow are known compatibility issues with the Python SDK.\n\n#### gevent Patching\n\nWhen using `gevent.monkey.patch_all()`, asyncio event loops can get messed up, especially those using custom event loops\nlike Temporal. See [this gevent issue](https://github.com/gevent/gevent/issues/982). This is a known incompatibility and\nusers are encouraged to not use gevent in asyncio applications (including Temporal). But if you must, there is\n[a sample](https://github.com/temporalio/samples-python/tree/main/gevent_async) showing how it is possible.\n\n# Development\n\nThe Python SDK is built to work with Python 3.8 and newer. It is built using\n[SDK Core](https://github.com/temporalio/sdk-core/) which is written in Rust.\n\n### Building\n\n#### Prepare\n\nTo build the SDK from source for use as a dependency, the following prerequisites are required:\n\n* [Python](https://www.python.org/) >= 3.8\n  * Make sure the latest version of `pip` is in use\n* [Rust](https://www.rust-lang.org/)\n* [poetry](https://github.com/python-poetry/poetry) (e.g. `python -m pip install poetry`)\n* [poe](https://github.com/nat-n/poethepoet) (e.g. `python -m pip install poethepoet`)\n\nmacOS note: If errors are encountered, it may be better to install Python and Rust as recommended from their websites\ninstead of via `brew`.\n\nWith the prerequisites installed, first clone the SDK repository recursively:\n\n```bash\ngit clone --recursive https://github.com/temporalio/sdk-python.git\ncd sdk-python\n```\n\nUse `poetry` to install the dependencies with `--no-root` to not install this package (because we still need to build\nit):\n\n```bash\npoetry install --no-root --all-extras\n```\n\n#### Build\n\nNow perform the release build:\n\n> This will take a while because Rust will compile the core project in release mode (see [Local SDK development\nenvironment](#local-sdk-development-environment) for the quicker approach to local development).\n\n```bash\npoetry build\n```\n\nThe compiled wheel doesn\'t have the exact right tags yet for use, so run this script to fix it:\n\n```bash\npoe fix-wheel\n```\n\nThe `whl` wheel file in `dist/` is now ready to use.\n\n#### Use\n\nThe wheel can now be installed into any virtual environment.\n\nFor example,\n[create a virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments)\nsomewhere and then run the following inside the virtual environment:\n\n```bash\npip install wheel\n```\n\n```bash\npip install /path/to/cloned/sdk-python/dist/*.whl\n```\n\nCreate this Python file at `example.py`:\n\n```python\nimport asyncio\nfrom temporalio import workflow, activity\nfrom temporalio.client import Client\nfrom temporalio.worker import Worker\n\n@workflow.defn\nclass SayHello:\n    @workflow.run\n    async def run(self, name: str) -> str:\n        return f"Hello, {name}!"\n\nasync def main():\n    client = await Client.connect("localhost:7233")\n    async with Worker(client, task_queue="my-task-queue", workflows=[SayHello]):\n        result = await client.execute_workflow(SayHello.run, "Temporal",\n            id="my-workflow-id", task_queue="my-task-queue")\n        print(f"Result: {result}")\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nAssuming there is a [local Temporal server](https://docs.temporal.io/docs/server/quick-install/) running, execute the\nfile with `python` (or `python3` if necessary):\n\n```bash\npython example.py\n```\n\nIt should output:\n\n    Result: Hello, Temporal!\n\n### Local SDK development environment\n\nFor local development, it is often quicker to use debug builds and a local virtual environment.\n\nWhile not required, it often helps IDEs if we put the virtual environment `.venv` directory in the project itself. This\ncan be configured system-wide via:\n\n```bash\npoetry config virtualenvs.in-project true\n```\n\nNow perform the same steps as the "Prepare" section above by installing the prerequisites, cloning the project,\ninstalling dependencies, and generating the protobuf code:\n\n```bash\ngit clone --recursive https://github.com/temporalio/sdk-python.git\ncd sdk-python\npoetry install --no-root --all-extras\n```\n\nNow compile the Rust extension in develop mode which is quicker than release mode:\n\n```bash\npoe build-develop\n```\n\nThat step can be repeated for any Rust changes made.\n\nThe environment is now ready to develop in.\n\n#### Testing\n\nTo execute tests:\n\n```bash\npoe test\n```\n\nThis runs against [Temporalite](https://github.com/temporalio/temporalite). To run against the time-skipping test\nserver, pass `--workflow-environment time-skipping`. To run against the `default` namespace of an already-running\nserver, pass the `host:port` to `--workflow-environment`. Can also use regular pytest arguments. For example, here\'s how\nto run a single test with debug logs on the console:\n\n```bash\npoe test -s --log-cli-level=DEBUG -k test_sync_activity_thread_cancel_caught\n```\n\n#### Proto Generation and Testing\n\nTo allow for backwards compatibility, protobuf code is generated on the 3.x series of the protobuf library. To generate\nprotobuf code, you must be on Python <= 3.10, and then run `poetry add "protobuf<4"`. Then the protobuf files can be\ngenerated via `poe gen-protos`. Tests can be run for protobuf version 3 by setting the `TEMPORAL_TEST_PROTO3` env var\nto `1` prior to running tests.\n\nDo not commit `poetry.lock` or `pyproject.toml` changes. To go back from this downgrade, restore `pyproject.toml` and\nrun `poetry update protobuf grpcio-tools`.\n\nFor a less system-intrusive approach, you can:\n```shell\ndocker build -f scripts/_proto/Dockerfile .\ndocker run -v "${PWD}/temporalio/api:/api_new" -v "${PWD}/temporalio/bridge/proto:/bridge_new" <just built image sha>\npoe format\n```\n\n### Style\n\n* Mostly [Google Style Guide](https://google.github.io/styleguide/pyguide.html). Notable exceptions:\n  * We use [Black](https://github.com/psf/black) for formatting, so that takes precedence\n  * In tests and example code, can import individual classes/functions to make it more readable. Can also do this for\n    rarely in library code for some Python common items (e.g. `dataclass` or `partial`), but not allowed to do this for\n    any `temporalio` packages (except `temporalio.types`) or any classes/functions that aren\'t clear when unqualified.\n  * We allow relative imports for private packages\n  * We allow `@staticmethod`\n',
+    'long_description': '![Temporal Python SDK](https://assets.temporal.io/w/py-banner.svg)\n\n[![Python 3.8+](https://img.shields.io/pypi/pyversions/temporalio.svg?style=for-the-badge)](https://pypi.org/project/temporalio)\n[![PyPI](https://img.shields.io/pypi/v/temporalio.svg?style=for-the-badge)](https://pypi.org/project/temporalio)\n[![MIT](https://img.shields.io/pypi/l/temporalio.svg?style=for-the-badge)](LICENSE)\n\n[Temporal](https://temporal.io/) is a distributed, scalable, durable, and highly available orchestration engine used to\nexecute asynchronous, long-running business logic in a scalable and resilient way.\n\n"Temporal Python SDK" is the framework for authoring workflows and activities using the Python programming language.\n\nAlso see:\n* [Application Development Guide](https://docs.temporal.io/application-development?lang=python) - Once you\'ve tried our\n  [Quick Start](#quick-start), check out our guide on how to use Temporal in your Python applications, including\n  information around Temporal core concepts.\n* [Python Code Samples](https://github.com/temporalio/samples-python)\n* [API Documentation](https://python.temporal.io) - Complete Temporal Python SDK Package reference.\n\nIn addition to features common across all Temporal SDKs, the Python SDK also has the following interesting features:\n\n**Type Safe**\n\nThis library uses the latest typing and MyPy support with generics to ensure all calls can be typed. For example,\nstarting a workflow with an `int` parameter when it accepts a `str` parameter would cause MyPy to fail.\n\n**Different Activity Types**\n\nThe activity worker has been developed to work with `async def`, threaded, and multiprocess activities. While\n`async def` activities are the easiest and recommended, care has been taken to make heartbeating and cancellation also\nwork across threads/processes.\n\n**Custom `asyncio` Event Loop**\n\nThe workflow implementation basically turns `async def` functions into workflows backed by a distributed, fault-tolerant\nevent loop. This means task management, sleep, cancellation, etc have all been developed to seamlessly integrate with\n`asyncio` concepts.\n\nSee the [blog post](https://temporal.io/blog/durable-distributed-asyncio-event-loop) introducing the Python SDK for an\ninformal introduction to the features and their implementation.\n\n---\n\n<!-- START doctoc generated TOC please keep comment here to allow auto update -->\n<!-- DON\'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->\n**Contents**\n\n- [Quick Start](#quick-start)\n  - [Installation](#installation)\n  - [Implementing a Workflow](#implementing-a-workflow)\n  - [Running a Workflow](#running-a-workflow)\n  - [Next Steps](#next-steps)\n- [Usage](#usage)\n    - [Client](#client)\n      - [Data Conversion](#data-conversion)\n        - [Custom Type Data Conversion](#custom-type-data-conversion)\n    - [Workers](#workers)\n    - [Workflows](#workflows)\n      - [Definition](#definition)\n      - [Running](#running)\n      - [Invoking Activities](#invoking-activities)\n      - [Invoking Child Workflows](#invoking-child-workflows)\n      - [Timers](#timers)\n      - [Conditions](#conditions)\n      - [Asyncio and Cancellation](#asyncio-and-cancellation)\n      - [Workflow Utilities](#workflow-utilities)\n      - [Exceptions](#exceptions)\n      - [External Workflows](#external-workflows)\n      - [Testing](#testing)\n        - [Automatic Time Skipping](#automatic-time-skipping)\n        - [Manual Time Skipping](#manual-time-skipping)\n        - [Mocking Activities](#mocking-activities)\n      - [Workflow Sandbox](#workflow-sandbox)\n        - [How the Sandbox Works](#how-the-sandbox-works)\n        - [Avoiding the Sandbox](#avoiding-the-sandbox)\n        - [Customizing the Sandbox](#customizing-the-sandbox)\n          - [Passthrough Modules](#passthrough-modules)\n          - [Invalid Module Members](#invalid-module-members)\n        - [Known Sandbox Issues](#known-sandbox-issues)\n          - [Global Import/Builtins](#global-importbuiltins)\n          - [Sandbox is not Secure](#sandbox-is-not-secure)\n          - [Sandbox Performance](#sandbox-performance)\n          - [Extending Restricted Classes](#extending-restricted-classes)\n          - [Certain Standard Library Calls on Restricted Objects](#certain-standard-library-calls-on-restricted-objects)\n          - [is_subclass of ABC-based Restricted Classes](#is_subclass-of-abc-based-restricted-classes)\n          - [Compiled Pydantic Sometimes Using Wrong Types](#compiled-pydantic-sometimes-using-wrong-types)\n    - [Activities](#activities)\n      - [Definition](#definition-1)\n      - [Types of Activities](#types-of-activities)\n        - [Synchronous Activities](#synchronous-activities)\n          - [Synchronous Multithreaded Activities](#synchronous-multithreaded-activities)\n          - [Synchronous Multiprocess/Other Activities](#synchronous-multiprocessother-activities)\n        - [Asynchronous Activities](#asynchronous-activities)\n      - [Activity Context](#activity-context)\n        - [Heartbeating and Cancellation](#heartbeating-and-cancellation)\n        - [Worker Shutdown](#worker-shutdown)\n      - [Testing](#testing-1)\n    - [Workflow Replay](#workflow-replay)\n    - [OpenTelemetry Support](#opentelemetry-support)\n    - [Protobuf 3.x vs 4.x](#protobuf-3x-vs-4x)\n    - [Known Compatibility Issues](#known-compatibility-issues)\n      - [gevent Patching](#gevent-patching)\n- [Development](#development)\n    - [Building](#building)\n      - [Prepare](#prepare)\n      - [Build](#build)\n      - [Use](#use)\n    - [Local SDK development environment](#local-sdk-development-environment)\n      - [Testing](#testing-2)\n      - [Proto Generation and Testing](#proto-generation-and-testing)\n    - [Style](#style)\n\n<!-- END doctoc generated TOC please keep comment here to allow auto update -->\n\n# Quick Start\n\nWe will guide you through the Temporal basics to create a "hello, world!" script on your machine. It is not intended as\none of the ways to use Temporal, but in reality it is very simplified and decidedly not "the only way" to use Temporal.\nFor more information, check out the docs references in "Next Steps" below the quick start.\n\n## Installation\n\nInstall the `temporalio` package from [PyPI](https://pypi.org/project/temporalio).\n\nThese steps can be followed to use with a virtual environment and `pip`:\n\n* [Create a virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments)\n* Update `pip` - `python -m pip install -U pip`\n  * Needed because older versions of `pip` may not pick the right wheel\n* Install Temporal SDK - `python -m pip install temporalio`\n\nThe SDK is now ready for use. To build from source, see "Building" near the end of this documentation.\n\n**NOTE: This README is for the current branch and not necessarily what\'s released on `PyPI`.**\n\n## Implementing a Workflow\n\nCreate the following in `activities.py`:\n\n```python\nfrom temporalio import activity\n\n@activity.defn\ndef say_hello(name: str) -> str:\n    return f"Hello, {name}!"\n```\n\nCreate the following in `workflows.py`:\n\n```python\nfrom datetime import timedelta\nfrom temporalio import workflow\n\n# Import our activity, passing it through the sandbox\nwith workflow.unsafe.imports_passed_through():\n    from .activities import say_hello\n\n@workflow.defn\nclass SayHello:\n    @workflow.run\n    async def run(self, name: str) -> str:\n        return await workflow.execute_activity(\n            say_hello, name, schedule_to_close_timeout=timedelta(seconds=5)\n        )\n```\n\nCreate the following in `run_worker.py`:\n\n```python\nimport asyncio\nimport concurrent.futures\nfrom temporalio.client import Client\nfrom temporalio.worker import Worker\n\n# Import the activity and workflow from our other files\nfrom .activities import say_hello\nfrom .workflows import SayHello\n\nasync def main():\n    # Create client connected to server at the given address\n    client = await Client.connect("localhost:7233")\n\n    # Run the worker\n    with concurrent.futures.ThreadPoolExecutor(max_workers=100) as activity_executor:\n        worker = Worker(\n          client,\n          task_queue="my-task-queue",\n          workflows=[SayHello],\n          activities=[say_hello],\n          activity_executor=activity_executor,\n        )\n        await worker.run()\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nAssuming you have a [Temporal server running on localhost](https://docs.temporal.io/docs/server/quick-install/), this\nwill run the worker:\n\n    python run_worker.py\n\n## Running a Workflow\n\nCreate the following script at `run_workflow.py`:\n\n```python\nimport asyncio\nfrom temporalio.client import Client\n\n# Import the workflow from the previous code\nfrom .workflows import SayHello\n\nasync def main():\n    # Create client connected to server at the given address\n    client = await Client.connect("localhost:7233")\n\n    # Execute a workflow\n    result = await client.execute_workflow(SayHello.run, "my name", id="my-workflow-id", task_queue="my-task-queue")\n\n    print(f"Result: {result}")\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nAssuming you have `run_worker.py` running from before, this will run the workflow:\n\n    python run_workflow.py\n\nThe output will be:\n\n    Result: Hello, my-name!\n\n## Next Steps\n\nTemporal can be implemented in your code in many different ways, to suit your application\'s needs. The links below will\ngive you much more information about how Temporal works with Python:\n\n* [Code Samples](https://github.com/temporalio/samples-python) - If you want to start with some code, we have provided\n  some pre-built samples.\n* [Application Development Guide](https://docs.temporal.io/application-development?lang=python) Our Python specific\n  Developer\'s Guide will give you much more information on how to build with Temporal in your Python applications than\n  our SDK README ever could (or should).\n* [API Documentation](https://python.temporal.io) - Full Temporal Python SDK package documentation.\n\n---\n\n# Usage\n\nFrom here, you will find reference documentation about specific pieces of the Temporal Python SDK that were built around\nTemporal concepts. *This section is not intended as a how-to guide* -- For more how-to oriented information, check out\nthe links in the [Next Steps](#next-steps) section above.\n\n### Client\n\nA client can be created and used to start a workflow like so:\n\n```python\nfrom temporalio.client import Client\n\nasync def main():\n    # Create client connected to server at the given address and namespace\n    client = await Client.connect("localhost:7233", namespace="my-namespace")\n\n    # Start a workflow\n    handle = await client.start_workflow(MyWorkflow.run, "some arg", id="my-workflow-id", task_queue="my-task-queue")\n\n    # Wait for result\n    result = await handle.result()\n    print(f"Result: {result}")\n```\n\nSome things to note about the above code:\n\n* A `Client` does not have an explicit "close"\n* To enable TLS, the `tls` argument to `connect` can be set to `True` or a `TLSConfig` object\n* A single positional argument can be passed to `start_workflow`. If there are multiple arguments, only the\n  non-type-safe form of `start_workflow` can be used (i.e. the one accepting a string workflow name) and it must be in\n  the `args` keyword argument.\n* The `handle` represents the workflow that was started and can be used for more than just getting the result\n* Since we are just getting the handle and waiting on the result, we could have called `client.execute_workflow` which\n  does the same thing\n* Clients can have many more options not shown here (e.g. data converters and interceptors)\n* A string can be used instead of the method reference to call a workflow by name (e.g. if defined in another language)\n* Clients do not work across forks\n\nClients also provide a shallow copy of their config for use in making slightly different clients backed by the same\nconnection. For instance, given the `client` above, this is how to have a client in another namespace:\n\n```python\nconfig = client.config()\nconfig["namespace"] = "my-other-namespace"\nother_ns_client = Client(**config)\n```\n\n#### Data Conversion\n\nData converters are used to convert raw Temporal payloads to/from actual Python types. A custom data converter of type\n`temporalio.converter.DataConverter` can be set via the `data_converter` client parameter. Data converters are a\ncombination of payload converters, payload codecs, and failure converters. Payload converters convert Python values\nto/from serialized bytes. Payload codecs convert bytes to bytes (e.g. for compression or encryption). Failure converters\nconvert exceptions to/from serialized failures.\n\nThe default data converter supports converting multiple types including:\n\n* `None`\n* `bytes`\n* `google.protobuf.message.Message` - As JSON when encoding, but has ability to decode binary proto from other languages\n* Anything that can be converted to JSON including:\n  * Anything that [`json.dump`](https://docs.python.org/3/library/json.html#json.dump) supports natively\n  * [dataclasses](https://docs.python.org/3/library/dataclasses.html)\n  * Iterables including ones JSON dump may not support by default, e.g. `set`\n  * Any class with a `dict()` method and a static `parse_obj()` method, e.g.\n    [Pydantic models](https://pydantic-docs.helpmanual.io/usage/models)\n    * The default data converter is deprecated for Pydantic models and will warn if used since not all fields work.\n      See [this sample](https://github.com/temporalio/samples-python/tree/main/pydantic_converter) for the recommended\n      approach.\n  * [IntEnum, StrEnum](https://docs.python.org/3/library/enum.html) based enumerates\n  * [UUID](https://docs.python.org/3/library/uuid.html)\n\nThis notably doesn\'t include any `date`, `time`, or `datetime` objects as they may not work across SDKs.\n\nUsers are strongly encouraged to use a single `dataclass` for parameter and return types so fields with defaults can be\neasily added without breaking compatibility.\n\nClasses with generics may not have the generics properly resolved. The current implementation does not have generic\ntype resolution. Users should use concrete types.\n\n##### Custom Type Data Conversion\n\nFor converting from JSON, the workflow/activity type hint is taken into account to convert to the proper type. Care has\nbeen taken to support all common typings including `Optional`, `Union`, all forms of iterables and mappings, `NewType`,\netc in addition to the regular JSON values mentioned before.\n\nData converters contain a reference to a payload converter class that is used to convert to/from payloads/values. This\nis a class and not an instance because it is instantiated on every workflow run inside the sandbox. The payload\nconverter is usually a `CompositePayloadConverter` which contains a multiple `EncodingPayloadConverter`s it uses to try\nto serialize/deserialize payloads. Upon serialization, each `EncodingPayloadConverter` is tried until one succeeds. The\n`EncodingPayloadConverter` provides an "encoding" string serialized onto the payload so that, upon deserialization, the\nspecific `EncodingPayloadConverter` for the given "encoding" is used.\n\nThe default data converter uses the `DefaultPayloadConverter` which is simply a `CompositePayloadConverter` with a known\nset of default `EncodingPayloadConverter`s. To implement a custom encoding for a custom type, a new\n`EncodingPayloadConverter` can be created for the new type. For example, to support `IPv4Address` types:\n\n```python\nclass IPv4AddressEncodingPayloadConverter(EncodingPayloadConverter):\n    @property\n    def encoding(self) -> str:\n        return "text/ipv4-address"\n\n    def to_payload(self, value: Any) -> Optional[Payload]:\n        if isinstance(value, ipaddress.IPv4Address):\n            return Payload(\n                metadata={"encoding": self.encoding.encode()},\n                data=str(value).encode(),\n            )\n        else:\n            return None\n\n    def from_payload(self, payload: Payload, type_hint: Optional[Type] = None) -> Any:\n        assert not type_hint or type_hint is ipaddress.IPv4Address\n        return ipaddress.IPv4Address(payload.data.decode())\n\nclass IPv4AddressPayloadConverter(CompositePayloadConverter):\n    def __init__(self) -> None:\n        # Just add ours as first before the defaults\n        super().__init__(\n            IPv4AddressEncodingPayloadConverter(),\n            *DefaultPayloadConverter.default_encoding_payload_converters,\n        )\n\nmy_data_converter = dataclasses.replace(\n    DataConverter.default,\n    payload_converter_class=IPv4AddressPayloadConverter,\n)\n```\n\nImports are left off for brevity.\n\nThis is good for many custom types. However, sometimes you want to override the behavior of the just the existing JSON\nencoding payload converter to support a new type. It is already the last encoding data converter in the list, so it\'s\nthe fall-through behavior for any otherwise unknown type. Customizing the existing JSON converter has the benefit of\nmaking the type work in lists, unions, etc.\n\nThe `JSONPlainPayloadConverter` uses the Python [json](https://docs.python.org/3/library/json.html) library with an\nadvanced JSON encoder by default and a custom value conversion method to turn `json.load`ed values to their type hints.\nThe conversion can be customized for serialization with a custom `json.JSONEncoder` and deserialization with a custom\n`JSONTypeConverter`. For example, to support `IPv4Address` types in existing JSON conversion:\n\n```python\nclass IPv4AddressJSONEncoder(AdvancedJSONEncoder):\n    def default(self, o: Any) -> Any:\n        if isinstance(o, ipaddress.IPv4Address):\n            return str(o)\n        return super().default(o)\nclass IPv4AddressJSONTypeConverter(JSONTypeConverter):\n    def to_typed_value(\n        self, hint: Type, value: Any\n    ) -> Union[Optional[Any], _JSONTypeConverterUnhandled]:\n        if issubclass(hint, ipaddress.IPv4Address):\n            return ipaddress.IPv4Address(value)\n        return JSONTypeConverter.Unhandled\n\nclass IPv4AddressPayloadConverter(CompositePayloadConverter):\n    def __init__(self) -> None:\n        # Replace default JSON plain with our own that has our encoder and type\n        # converter\n        json_converter = JSONPlainPayloadConverter(\n            encoder=IPv4AddressJSONEncoder,\n            custom_type_converters=[IPv4AddressJSONTypeConverter()],\n        )\n        super().__init__(\n            *[\n                c if not isinstance(c, JSONPlainPayloadConverter) else json_converter\n                for c in DefaultPayloadConverter.default_encoding_payload_converters\n            ]\n        )\n\nmy_data_converter = dataclasses.replace(\n    DataConverter.default,\n    payload_converter_class=IPv4AddressPayloadConverter,\n)\n```\n\nNow `IPv4Address` can be used in type hints including collections, optionals, etc.\n\n### Workers\n\nWorkers host workflows and/or activities. Here\'s how to run a worker:\n\n```python\nimport asyncio\nimport logging\nfrom temporalio.client import Client\nfrom temporalio.worker import Worker\n# Import your own workflows and activities\nfrom my_workflow_package import MyWorkflow, my_activity\n\nasync def run_worker(stop_event: asyncio.Event):\n    # Create client connected to server at the given address\n    client = await Client.connect("localhost:7233", namespace="my-namespace")\n\n    # Run the worker until the event is set\n    worker = Worker(client, task_queue="my-task-queue", workflows=[MyWorkflow], activities=[my_activity])\n    async with worker:\n        await stop_event.wait()\n```\n\nSome things to note about the above code:\n\n* This creates/uses the same client that is used for starting workflows\n* While this example accepts a stop event and uses `async with`, `run()` and `shutdown()` may be used instead\n* Workers can have many more options not shown here (e.g. data converters and interceptors)\n\n### Workflows\n\n#### Definition\n\nWorkflows are defined as classes decorated with `@workflow.defn`. The method invoked for the workflow is decorated with\n`@workflow.run`. Methods for signals, queries, and updates are decorated with `@workflow.signal`, `@workflow.query`\nand `@workflow.update` respectively. Here\'s an example of a workflow:\n\n```python\nimport asyncio\nfrom datetime import timedelta\nfrom temporalio import workflow\n\n# Pass the activities through the sandbox\nwith workflow.unsafe.imports_passed_through():\n    from .my_activities import GreetingInfo, create_greeting_activity\n\n@workflow.defn\nclass GreetingWorkflow:\n    def __init__(self) -> None:\n        self._current_greeting = "<unset>"\n        self._greeting_info = GreetingInfo()\n        self._greeting_info_update = asyncio.Event()\n        self._complete = asyncio.Event()\n\n    @workflow.run\n    async def run(self, name: str) -> str:\n        self._greeting_info.name = name\n        while True:\n            # Store greeting\n            self._current_greeting = await workflow.execute_activity(\n                create_greeting_activity,\n                self._greeting_info,\n                start_to_close_timeout=timedelta(seconds=5),\n            )\n            workflow.logger.debug("Greeting set to %s", self._current_greeting)\n            \n            # Wait for salutation update or complete signal (this can be\n            # cancelled)\n            await asyncio.wait(\n                [\n                    asyncio.create_task(self._greeting_info_update.wait()),\n                    asyncio.create_task(self._complete.wait()),\n                ],\n                return_when=asyncio.FIRST_COMPLETED,\n            )\n            if self._complete.is_set():\n                return self._current_greeting\n            self._greeting_info_update.clear()\n\n    @workflow.signal\n    async def update_salutation(self, salutation: str) -> None:\n        self._greeting_info.salutation = salutation\n        self._greeting_info_update.set()\n\n    @workflow.signal\n    async def complete_with_greeting(self) -> None:\n        self._complete.set()\n\n    @workflow.query\n    def current_greeting(self) -> str:\n        return self._current_greeting\n    \n    @workflow.update\n    def set_and_get_greeting(self, greeting: str) -> str:\n      old = self._current_greeting\n      self._current_greeting = greeting\n      return old\n\n```\n\nThis assumes there\'s an activity in `my_activities.py` like:\n\n```python\nfrom dataclasses import dataclass\nfrom temporalio import workflow\n\n@dataclass\nclass GreetingInfo:\n    salutation: str = "Hello"\n    name: str = "<unknown>"\n\n@activity.defn\ndef create_greeting_activity(info: GreetingInfo) -> str:\n    return f"{info.salutation}, {info.name}!"\n```\n\nSome things to note about the above workflow code:\n\n* Workflows run in a sandbox by default.\n  * Users are encouraged to define workflows in files with no side effects or other complicated code or unnecessary\n    imports to other third party libraries.\n  * Non-standard-library, non-`temporalio` imports should usually be "passed through" the sandbox. See the\n    [Workflow Sandbox](#workflow-sandbox) section for more details.\n* This workflow continually updates the queryable current greeting when signalled and can complete with the greeting on\n  a different signal\n* Workflows are always classes and must have a single `@workflow.run` which is an `async def` function\n* Workflow code must be deterministic. This means no threading, no randomness, no external calls to processes, no\n  network IO, and no global state mutation. All code must run in the implicit `asyncio` event loop and be deterministic.\n* `@activity.defn` is explained in a later section. For normal simple string concatenation, this would just be done in\n  the workflow. The activity is for demonstration purposes only.\n* `workflow.execute_activity(create_greeting_activity, ...` is actually a typed signature, and MyPy will fail if the\n  `self._greeting_info` parameter is not a `GreetingInfo`\n\nHere are the decorators that can be applied:\n\n* `@workflow.defn` - Defines a workflow class\n  * Must be defined on the class given to the worker (ignored if present on a base class)\n  * Can have a `name` param to customize the workflow name, otherwise it defaults to the unqualified class name\n  * Can have `dynamic=True` which means all otherwise unhandled workflows fall through to this. If present, cannot have\n    `name` argument, and run method must accept a single parameter of `Sequence[temporalio.common.RawValue]` type. The\n    payload of the raw value can be converted via `workflow.payload_converter().from_payload`.\n* `@workflow.run` - Defines the primary workflow run method\n  * Must be defined on the same class as `@workflow.defn`, not a base class (but can _also_ be defined on the same\n    method of a base class)\n  * Exactly one method name must have this decorator, no more or less\n  * Must be defined on an `async def` method\n  * The method\'s arguments are the workflow\'s arguments\n  * The first parameter must be `self`, followed by positional arguments. Best practice is to only take a single\n    argument that is an object/dataclass of fields that can be added to as needed.\n* `@workflow.signal` - Defines a method as a signal\n  * Can be defined on an `async` or non-`async` function at any hierarchy depth, but if decorated method is overridden,\n    the override must also be decorated\n  * The method\'s arguments are the signal\'s arguments\n  * Can have a `name` param to customize the signal name, otherwise it defaults to the unqualified method name\n  * Can have `dynamic=True` which means all otherwise unhandled signals fall through to this. If present, cannot have\n    `name` argument, and method parameters must be `self`, a string signal name, and a\n    `Sequence[temporalio.common.RawValue]`.\n  * Non-dynamic method can only have positional arguments. Best practice is to only take a single argument that is an\n    object/dataclass of fields that can be added to as needed.\n  * Return value is ignored\n* `@workflow.query` - Defines a method as a query\n  * All the same constraints as `@workflow.signal` but should return a value\n  * Should not be `async`\n  * Temporal queries should never mutate anything in the workflow or call any calls that would mutate the workflow\n* `@workflow.update` - Defines a method as an update\n  * May both accept as input and return a value\n  * May be `async` or non-`async`\n  * May mutate workflow state, and make calls to other workflow APIs like starting activities, etc.\n  * Also accepts the `name` and `dynamic` parameters like signals and queries, with the same semantics.\n  * Update handlers may optionally define a validator method by decorating it with `@update_handler_method.validator`.\n    To reject an update before any events are written to history, throw an exception in a validator. Validators cannot \n    be `async`, cannot mutate workflow state, and return nothing.\n\n#### Running\n\nTo start a locally-defined workflow from a client, you can simply reference its method like so:\n\n```python\nfrom temporalio.client import Client\nfrom my_workflow_package import GreetingWorkflow\n\nasync def create_greeting(client: Client) -> str:\n    # Start the workflow\n    handle = await client.start_workflow(GreetingWorkflow.run, "my name", id="my-workflow-id", task_queue="my-task-queue")\n    # Change the salutation\n    await handle.signal(GreetingWorkflow.update_salutation, "Aloha")\n    # Tell it to complete\n    await handle.signal(GreetingWorkflow.complete_with_greeting)\n    # Wait and return result\n    return await handle.result()\n```\n\nSome things to note about the above code:\n\n* This uses the `GreetingWorkflow` from the previous section\n* The result of calling this function is `"Aloha, my name!"`\n* `id` and `task_queue` are required for running a workflow\n* `client.start_workflow` is typed, so MyPy would fail if `"my name"` were something besides a string\n* `handle.signal` is typed, so MyPy would fail if `"Aloha"` were something besides a string or if we provided a\n  parameter to the parameterless `complete_with_greeting`\n* `handle.result` is typed to the workflow itself, so MyPy would fail if we said this `create_greeting` returned\n  something besides a string\n\n#### Invoking Activities\n\n* Activities are started with non-async `workflow.start_activity()` which accepts either an activity function reference\n  or a string name.\n* A single argument to the activity is positional. Multiple arguments are not supported in the type-safe form of\n  start/execute activity and must be supplied via the `args` keyword argument.\n* Activity options are set as keyword arguments after the activity arguments. At least one of `start_to_close_timeout`\n  or `schedule_to_close_timeout` must be provided.\n* The result is an activity handle which is an `asyncio.Task` and supports basic task features\n* An async `workflow.execute_activity()` helper is provided which takes the same arguments as\n  `workflow.start_activity()` and `await`s on the result. This should be used in most cases unless advanced task\n  capabilities are needed.\n* Local activities work very similarly except the functions are `workflow.start_local_activity()` and\n  `workflow.execute_local_activity()`\n  * ⚠️Local activities are currently experimental\n* Activities can be methods of a class. Invokers should use `workflow.start_activity_method()`,\n  `workflow.execute_activity_method()`, `workflow.start_local_activity_method()`, and\n  `workflow.execute_local_activity_method()` instead.\n* Activities can callable classes (i.e. that define `__call__`). Invokers should use `workflow.start_activity_class()`,\n  `workflow.execute_activity_class()`, `workflow.start_local_activity_class()`, and\n  `workflow.execute_local_activity_class()` instead.\n\n#### Invoking Child Workflows\n\n* Child workflows are started with async `workflow.start_child_workflow()` which accepts either a workflow run method\n  reference or a string name. The arguments to the workflow are positional.\n* A single argument to the child workflow is positional. Multiple arguments are not supported in the type-safe form of\n  start/execute child workflow and must be supplied via the `args` keyword argument.\n* Child workflow options are set as keyword arguments after the arguments. At least `id` must be provided.\n* The `await` of the start does not complete until the start has been accepted by the server\n* The result is a child workflow handle which is an `asyncio.Task` and supports basic task features. The handle also has\n  some child info and supports signalling the child workflow\n* An async `workflow.execute_child_workflow()` helper is provided which takes the same arguments as\n  `workflow.start_child_workflow()` and `await`s on the result. This should be used in most cases unless advanced task\n  capabilities are needed.\n\n#### Timers\n\n* A timer is represented by normal `asyncio.sleep()`\n* Timers are also implicitly started on any `asyncio` calls with timeouts (e.g. `asyncio.wait_for`)\n* Timers are Temporal server timers, not local ones, so sub-second resolution rarely has value\n* Calls that use a specific point in time, e.g. `call_at` or `timeout_at`, should be based on the current loop time\n  (i.e. `workflow.time()`) and not an actual point in time. This is because fixed times are translated to relative ones\n  by subtracting the current loop time which may not be the actual current time.\n\n#### Conditions\n\n* `workflow.wait_condition` is an async function that doesn\'t return until a provided callback returns true\n* A `timeout` can optionally be provided which will throw a `asyncio.TimeoutError` if reached (internally backed by\n  `asyncio.wait_for` which uses a timer)\n\n#### Asyncio and Cancellation\n\nWorkflows are backed by a custom [asyncio](https://docs.python.org/3/library/asyncio.html) event loop. This means many\nof the common `asyncio` calls work as normal. Some asyncio features are disabled such as:\n\n* Thread related calls such as `to_thread()`, `run_coroutine_threadsafe()`, `loop.run_in_executor()`, etc\n* Calls that alter the event loop such as `loop.close()`, `loop.stop()`, `loop.run_forever()`,\n  `loop.set_task_factory()`, etc\n* Calls that use anything external such as networking, subprocesses, disk IO, etc\n\nCancellation is done the same way as `asyncio`. Specifically, a task can be requested to be cancelled but does not\nnecessarily have to respect that cancellation immediately. This also means that `asyncio.shield()` can be used to\nprotect against cancellation. The following tasks, when cancelled, perform a Temporal cancellation:\n\n* Activities - when the task executing an activity is cancelled, a cancellation request is sent to the activity\n* Child workflows - when the task starting or executing a child workflow is cancelled, a cancellation request is sent to\n  cancel the child workflow\n* Timers - when the task executing a timer is cancelled (whether started via sleep or timeout), the timer is cancelled\n\nWhen the workflow itself is requested to cancel, `Task.cancel` is called on the main workflow task. Therefore,\n`asyncio.CancelledError` can be caught in order to handle the cancel gracefully.\n\nWorkflows follow `asyncio` cancellation rules exactly which can cause confusion among Python developers. Cancelling a\ntask doesn\'t always cancel the thing it created. For example, given\n`task = asyncio.create_task(workflow.start_child_workflow(...`, calling `task.cancel` does not cancel the child\nworkflow, it only cancels the starting of it, which has no effect if it has already started. However, cancelling the\nresult of `handle = await workflow.start_child_workflow(...` or\n`task = asyncio.create_task(workflow.execute_child_workflow(...` _does_ cancel the child workflow.\n\nAlso, due to Temporal rules, a cancellation request is a state not an event. Therefore, repeated cancellation requests\nare not delivered, only the first. If the workflow chooses swallow a cancellation, it cannot be requested again.\n\n#### Workflow Utilities\n\nWhile running in a workflow, in addition to features documented elsewhere, the following items are available from the\n`temporalio.workflow` package:\n\n* `continue_as_new()` - Async function to stop the workflow immediately and continue as new\n* `info()` - Returns information about the current workflow\n* `logger` - A logger for use in a workflow (properly skips logging on replay)\n* `now()` - Returns the "current time" from the workflow\'s perspective\n\n#### Exceptions\n\n* Workflows/updates can raise exceptions to fail the workflow or the "workflow task" (i.e. suspend the workflow\n  in a retrying state).\n* Exceptions that are instances of `temporalio.exceptions.FailureError` will fail the workflow with that exception\n  * For failing the workflow explicitly with a user exception, use `temporalio.exceptions.ApplicationError`. This can\n    be marked non-retryable or include details as needed.\n  * Other exceptions that come from activity execution, child execution, cancellation, etc are already instances of\n    `FailureError` and will fail the workflow when uncaught.\n* All other exceptions fail the "workflow task" which means the workflow will continually retry until the workflow is\n  fixed. This is helpful for bad code or other non-predictable exceptions. To actually fail the workflow, use an\n  `ApplicationError` as mentioned above.\n\nThis default can be changed by providing a list of exception types to `workflow_failure_exception_types` when creating a\n`Worker` or `failure_exception_types` on the `@workflow.defn` decorator. If a workflow-thrown exception is an instance\nof any type in either list, it will fail the workflow instead of the task. This means a value of `[Exception]` will\ncause every exception to fail the workflow instead of the task. Also, as a special case, if\n`temporalio.workflow.NondeterminismError` (or any superclass of it) is set, non-deterministic exceptions will fail the\nworkflow. WARNING: These settings are experimental.\n\n#### External Workflows\n\n* `workflow.get_external_workflow_handle()` inside a workflow returns a handle to interact with another workflow\n* `workflow.get_external_workflow_handle_for()` can be used instead for a type safe handle\n* `await handle.signal()` can be called on the handle to signal the external workflow\n* `await handle.cancel()` can be called on the handle to send a cancel to the external workflow\n\n#### Testing\n\nWorkflow testing can be done in an integration-test fashion against a real server, however it is hard to simulate\ntimeouts and other long time-based code. Using the time-skipping workflow test environment can help there.\n\nThe time-skipping `temporalio.testing.WorkflowEnvironment` can be created via the static async `start_time_skipping()`.\nThis internally downloads the Temporal time-skipping test server to a temporary directory if it doesn\'t already exist,\nthen starts the test server which has special APIs for skipping time.\n\n**NOTE:** The time-skipping test environment does not work on ARM. The SDK will try to download the x64 binary on macOS\nfor use with the Intel emulator, but for Linux or Windows ARM there is no proper time-skipping test server at this time.\n\n##### Automatic Time Skipping\n\nAnytime a workflow result is waited on, the time-skipping server automatically advances to the next event it can. To\nmanually advance time before waiting on the result of a workflow, the `WorkflowEnvironment.sleep` method can be used.\n\nHere\'s a simple example of a workflow that sleeps for 24 hours:\n\n```python\nimport asyncio\nfrom temporalio import workflow\n\n@workflow.defn\nclass WaitADayWorkflow:\n    @workflow.run\n    async def run(self) -> str:\n        await asyncio.sleep(24 * 60 * 60)\n        return "all done"\n```\n\nAn integration test of this workflow would be way too slow. However the time-skipping server automatically skips to the\nnext event when we wait on the result. Here\'s a test for that workflow:\n\n```python\nfrom temporalio.testing import WorkflowEnvironment\nfrom temporalio.worker import Worker\n\nasync def test_wait_a_day_workflow():\n    async with await WorkflowEnvironment.start_time_skipping() as env:\n        async with Worker(env.client, task_queue="tq1", workflows=[WaitADayWorkflow]):\n            assert "all done" == await env.client.execute_workflow(WaitADayWorkflow.run, id="wf1", task_queue="tq1")\n```\n\nThat test will run almost instantly. This is because by calling `execute_workflow` on our client, we have asked the\nenvironment to automatically skip time as much as it can (basically until the end of the workflow or until an activity\nis run).\n\nTo disable automatic time-skipping while waiting for a workflow result, run code inside a\n`with env.auto_time_skipping_disabled():` block.\n\n##### Manual Time Skipping\n\nUntil a workflow is waited on, all time skipping in the time-skipping environment is done manually via\n`WorkflowEnvironment.sleep`.\n\nHere\'s workflow that waits for a signal or times out:\n\n```python\nimport asyncio\nfrom temporalio import workflow\n\n@workflow.defn\nclass SignalWorkflow:\n    def __init__(self) -> None:\n        self.signal_received = False\n\n    @workflow.run\n    async def run(self) -> str:\n        # Wait for signal or timeout in 45 seconds\n        try:\n            await workflow.wait_condition(lambda: self.signal_received, timeout=45)\n            return "got signal"\n        except asyncio.TimeoutError:\n            return "got timeout"\n\n    @workflow.signal\n    def some_signal(self) -> None:\n        self.signal_received = True\n```\n\nTo test a normal signal, you might:\n\n```python\nfrom temporalio.testing import WorkflowEnvironment\nfrom temporalio.worker import Worker\n\nasync def test_signal_workflow():\n    async with await WorkflowEnvironment.start_time_skipping() as env:\n        async with Worker(env.client, task_queue="tq1", workflows=[SignalWorkflow]):\n            # Start workflow, send signal, check result\n            handle = await env.client.start_workflow(SignalWorkflow.run, id="wf1", task_queue="tq1")\n            await handle.signal(SignalWorkflow.some_signal)\n            assert "got signal" == await handle.result()\n```\n\nBut how would you test the timeout part? Like so:\n\n```python\nfrom temporalio.testing import WorkflowEnvironment\nfrom temporalio.worker import Worker\n\nasync def test_signal_workflow_timeout():\n    async with await WorkflowEnvironment.start_time_skipping() as env:\n        async with Worker(env.client, task_queue="tq1", workflows=[SignalWorkflow]):\n            # Start workflow, advance time past timeout, check result\n            handle = await env.client.start_workflow(SignalWorkflow.run, id="wf1", task_queue="tq1")\n            await env.sleep(50)\n            assert "got timeout" == await handle.result()\n```\n\nAlso, the current time of the workflow environment can be obtained via the async `WorkflowEnvironment.get_current_time`\nmethod.\n\n##### Mocking Activities\n\nActivities are just functions decorated with `@activity.defn`. Simply write different ones and pass those to the worker\nto have different activities called during the test.\n\n#### Workflow Sandbox\n\nBy default workflows are run in a sandbox to help avoid non-deterministic code. If a call that is known to be\nnon-deterministic is performed, an exception will be thrown in the workflow which will "fail the task" which means the\nworkflow will not progress until fixed.\n\nThe sandbox is not foolproof and non-determinism can still occur. It is simply a best-effort way to catch bad code\nearly. Users are encouraged to define their workflows in files with no other side effects.\n\nThe sandbox offers a mechanism to pass through modules from outside the sandbox. By default this already includes all\nstandard library modules and Temporal modules. **For performance and behavior reasons, users are encouraged to pass\nthrough all third party modules whose calls will be deterministic.** This includes modules containing the activities to\nbe referenced in workflows. See "Passthrough Modules" below on how to do this.\n\nIf you are getting an error like:\n\n> temporalio.worker.workflow_sandbox._restrictions.RestrictedWorkflowAccessError: Cannot access\n> http.client.IncompleteRead.\\_\\_mro_entries\\_\\_ from inside a workflow. If this is code from a module not used in a\n> workflow or known to only be used deterministically from a workflow, mark the import as pass through.\n\nThen you are either using an invalid construct from the workflow, this is a known limitation of the sandbox, or most\ncommonly this is from a module that is safe to pass through (see "Passthrough Modules" section below).\n\n##### How the Sandbox Works\n\nThe sandbox is made up of two components that work closely together:\n\n* Global state isolation\n* Restrictions preventing known non-deterministic library calls\n\nGlobal state isolation is performed by using `exec`. Upon workflow start, the file that the workflow is defined in is\nimported into a new sandbox created for that workflow run. In order to keep the sandbox performant a known set of\n"passthrough modules" are passed through from outside of the sandbox when they are imported. These are expected to be\nside-effect free on import and have their non-deterministic aspects restricted. By default the entire Python standard\nlibrary, `temporalio`, and a couple of other modules are passed through from outside of the sandbox. To update this\nlist, see "Customizing the Sandbox".\n\nRestrictions preventing known non-deterministic library calls are achieved using proxy objects on modules wrapped around\nthe custom importer set in the sandbox. Many restrictions apply at workflow import time and workflow run time, while\nsome restrictions only apply at workflow run time. A default set of restrictions is included that prevents most\ndangerous standard library calls. However it is known in Python that some otherwise-non-deterministic invocations, like\nreading a file from disk via `open` or using `os.environ`, are done as part of importing modules. To customize what is\nand isn\'t restricted, see "Customizing the Sandbox".\n\n##### Avoiding the Sandbox\n\nThere are three increasingly-scoped ways to avoid the sandbox. Users are discouraged from avoiding the sandbox if\npossible.\n\nTo remove restrictions around a particular block of code, use `with temporalio.workflow.unsafe.sandbox_unrestricted():`.\nThe workflow will still be running in the sandbox, but no restrictions for invalid library calls will be applied.\n\nTo run an entire workflow outside of a sandbox, set `sandboxed=False` on the `@workflow.defn` decorator when defining\nit. This will run the entire workflow outside of the workflow which means it can share global state and other bad\nthings.\n\nTo disable the sandbox entirely for a worker, set the `Worker` init\'s `workflow_runner` keyword argument to \n`temporalio.worker.UnsandboxedWorkflowRunner()`. This value is defaulted to\n`temporalio.worker.workflow_sandbox.SandboxedWorkflowRunner()` so by changing it to the unsandboxed runner, the sandbox\nwill not be used at all.\n\n##### Customizing the Sandbox\n\n⚠️ WARNING: APIs in the `temporalio.worker.workflow_sandbox` module are not yet considered stable and may change in\nfuture releases.\n\nWhen creating the `Worker`, the `workflow_runner` is defaulted to\n`temporalio.worker.workflow_sandbox.SandboxedWorkflowRunner()`. The `SandboxedWorkflowRunner`\'s init accepts a\n`restrictions` keyword argument that is defaulted to `SandboxRestrictions.default`. The `SandboxRestrictions` dataclass\nis immutable and contains three fields that can be customized, but only two have notable value. See below.\n\n###### Passthrough Modules\n\nBy default the sandbox completely reloads non-standard-library and non-Temporal modules for every workflow run. To make\nthe sandbox quicker and use less memory when importing known-side-effect-free third party modules, they can be marked\nas passthrough modules.\n\n**For performance and behavior reasons, users are encouraged to pass through all third party modules whose calls will be\ndeterministic.**\n\nOne way to pass through a module is at import time in the workflow file using the `imports_passed_through` context\nmanager like so:\n\n```python\n# my_workflow_file.py\n\nfrom temporalio import workflow\n\nwith workflow.unsafe.imports_passed_through():\n    import pydantic\n\n@workflow.defn\nclass MyWorkflow:\n    ...\n```\n\nAlternatively, this can be done at worker creation time by customizing the runner\'s restrictions. For example:\n\n```python\nmy_worker = Worker(\n  ...,\n  workflow_runner=SandboxedWorkflowRunner(\n    restrictions=SandboxRestrictions.default.with_passthrough_modules("pydantic")\n  )\n)\n```\n\nIn both of these cases, now the `pydantic` module will be passed through from outside of the sandbox instead of\nbeing reloaded for every workflow run.\n\n###### Invalid Module Members\n\n`SandboxRestrictions.invalid_module_members` contains a root matcher that applies to all module members. This already\nhas a default set which includes things like `datetime.date.today()` which should never be called from a workflow. To\nremove this restriction:\n\n```python\nmy_restrictions = dataclasses.replace(\n    SandboxRestrictions.default,\n    invalid_module_members=SandboxRestrictions.invalid_module_members_default.with_child_unrestricted(\n      "datetime", "date", "today",\n    ),\n)\nmy_worker = Worker(..., workflow_runner=SandboxedWorkflowRunner(restrictions=my_restrictions))\n```\n\nRestrictions can also be added by `|`\'ing together matchers, for example to restrict the `datetime.date` class from\nbeing used altogether:\n\n```python\nmy_restrictions = dataclasses.replace(\n    SandboxRestrictions.default,\n    invalid_module_members=SandboxRestrictions.invalid_module_members_default | SandboxMatcher(\n      children={"datetime": SandboxMatcher(use={"date"})},\n    ),\n)\nmy_worker = Worker(..., workflow_runner=SandboxedWorkflowRunner(restrictions=my_restrictions))\n```\n\nSee the API for more details on exact fields and their meaning.\n\n##### Known Sandbox Issues\n\nBelow are known sandbox issues. As the sandbox is developed and matures, some may be resolved.\n\n###### Global Import/Builtins\n\nCurrently the sandbox references/alters the global `sys.modules` and `builtins` fields while running workflow code. In\norder to prevent affecting other sandboxed code, thread locals are leveraged to only intercept these values during the\nworkflow thread running. Therefore, technically if top-level import code starts a thread, it may lose sandbox\nprotection.\n\n###### Sandbox is not Secure\n\nThe sandbox is built to catch many non-deterministic and state sharing issues, but it is not secure. Some known bad\ncalls are intercepted, but for performance reasons, every single attribute get/set cannot be checked. Therefore a simple\ncall like `setattr(temporalio.common, "__my_key", "my value")` will leak across sandbox runs.\n\nThe sandbox is only a helper, it does not provide full protection.\n\n###### Sandbox Performance\n\nThe sandbox does not add significant CPU or memory overhead for workflows that are in files which only import standard\nlibrary modules. This is because they are passed through from outside of the sandbox. However, every\nnon-standard-library import that is performed at the top of the same file the workflow is in will add CPU overhead (the\nmodule is re-imported every workflow run) and memory overhead (each module independently cached as part of the workflow\nrun for isolation reasons). This becomes more apparent for large numbers of workflow runs.\n\nTo mitigate this, users should:\n\n* Define workflows in files that have as few non-standard-library imports as possible\n* Alter the max workflow cache and/or max concurrent workflows settings if memory grows too large\n* Set third-party libraries as passthrough modules if they are known to be side-effect free\n\n###### Extending Restricted Classes\n\nExtending a restricted class causes Python to instantiate the restricted metaclass which is unsupported. Therefore if\nyou attempt to use a class in the sandbox that extends a restricted class, it will fail. For example, if you have a\n`class MyZipFile(zipfile.ZipFile)` and try to use that class inside a workflow, it will fail.\n\nClasses used inside the workflow should not extend restricted classes. For situations where third-party modules need to\nat import time, they should be marked as pass through modules.\n\n###### Certain Standard Library Calls on Restricted Objects\n\nIf an object is restricted, internal C Python validation may fail in some cases. For example, running\n`dict.items(os.__dict__)` will fail with:\n\n> descriptor \'items\' for \'dict\' objects doesn\'t apply to a \'_RestrictedProxy\' object\n\nThis is a low-level check that cannot be subverted. The solution is to not use restricted objects inside the sandbox.\nFor situations where third-party modules need to at import time, they should be marked as pass through modules.\n\n###### is_subclass of ABC-based Restricted Classes\n\nDue to [https://bugs.python.org/issue44847](https://bugs.python.org/issue44847), classes that are wrapped and then\nchecked to see if they are subclasses of another via `is_subclass` may fail (see also\n[this wrapt issue](https://github.com/GrahamDumpleton/wrapt/issues/130)).\n\n###### Compiled Pydantic Sometimes Using Wrong Types\n\nIf the Pydantic dependency is in compiled form (the default) and you are using a Pydantic model inside a workflow\nsandbox that uses a `datetime` type, it will grab the wrong validator and use `date` instead. This is because our\npatched form of `issubclass` is bypassed by compiled Pydantic.\n\nTo work around, either don\'t use `datetime`-based Pydantic model fields in workflows, or mark `datetime` library as\npassthrough (means you lose protection against calling the non-deterministic `now()`), or use non-compiled Pydantic\ndependency.\n\n### Activities\n\n#### Definition\n\nActivities are decorated with `@activity.defn` like so:\n\n```python\nfrom temporalio import activity\n\n@activity.defn\ndef say_hello_activity(name: str) -> str:\n    return f"Hello, {name}!"\n```\n\nSome things to note about activity definitions:\n\n* The `say_hello_activity` is synchronous which is the recommended activity type (see "Types of Activities" below), but\n  it can be `async`\n* A custom name for the activity can be set with a decorator argument, e.g. `@activity.defn(name="my activity")`\n* Long running activities should regularly heartbeat and handle cancellation\n* Activities can only have positional arguments. Best practice is to only take a single argument that is an\n  object/dataclass of fields that can be added to as needed.\n* Activities can be defined on methods instead of top-level functions. This allows the instance to carry state that an\n  activity may need (e.g. a DB connection). The instance method should be what is registered with the worker.\n* Activities can also be defined on callable classes (i.e. classes with `__call__`). An instance of the class should be\n  what is registered with the worker.\n* The `@activity.defn` can have `dynamic=True` set which means all otherwise unhandled activities fall through to this.\n  If present, cannot have `name` argument, and the activity function must accept a single parameter of\n  `Sequence[temporalio.common.RawValue]`. The payload of the raw value can be converted via\n  `activity.payload_converter().from_payload`.\n\n#### Types of Activities\n\nThere are 3 types of activity callables accepted and described below: synchronous multithreaded, synchronous\nmultiprocess/other, and asynchronous. Only positional parameters are allowed in activity callables.\n\n##### Synchronous Activities\n\nSynchronous activities, i.e. functions that do not have `async def`, can be used with workers, but the\n`activity_executor` worker parameter must be set with a `concurrent.futures.Executor` instance to use for executing the\nactivities.\n\nAll long running, non-local activities should heartbeat so they can be cancelled. Cancellation in threaded activities\nthrows but multiprocess/other activities does not. The sections below on each synchronous type explain further. There\nare also calls on the context that can check for cancellation. For more information, see "Activity Context" and\n"Heartbeating and Cancellation" sections later.\n\nNote, all calls from an activity to functions in the `temporalio.activity` package are powered by\n[contextvars](https://docs.python.org/3/library/contextvars.html). Therefore, new threads starting _inside_ of\nactivities must `copy_context()` and then `.run()` manually to ensure `temporalio.activity` calls like `heartbeat` still\nfunction in the new threads.\n\nIf any activity ever throws a `concurrent.futures.BrokenExecutor`, the failure is consisted unrecoverable and the worker\nwill fail and shutdown.\n\n###### Synchronous Multithreaded Activities\n\nIf `activity_executor` is set to an instance of `concurrent.futures.ThreadPoolExecutor` then the synchronous activities\nare considered multithreaded activities. If `max_workers` is not set to at least the worker\'s\n`max_concurrent_activities` setting a warning will be issued. Besides `activity_executor`, no other worker parameters\nare required for synchronous multithreaded activities.\n\nBy default, cancellation of a synchronous multithreaded activity is done via a `temporalio.exceptions.CancelledError`\nthrown into the activity thread. Activities that do not wish to have cancellation thrown can set\n`no_thread_cancel_exception=True` in the `@activity.defn` decorator.\n\nCode that wishes to be temporarily shielded from the cancellation exception can run inside\n`with activity.shield_thread_cancel_exception():`. But once the last nested form of that block is finished, even if\nthere is a return statement within, it will throw the cancellation if there was one. A `try` +\n`except temporalio.exceptions.CancelledError` would have to surround the `with` to handle the cancellation explicitly.\n\n###### Synchronous Multiprocess/Other Activities\n\nIf `activity_executor` is set to an instance of `concurrent.futures.Executor` that is _not_\n`concurrent.futures.ThreadPoolExecutor`, then the synchronous activities are considered multiprocess/other activities.\nUsers should prefer threaded activities over multiprocess ones since, among other reasons, threaded activities can raise\non cancellation.\n\nThese require special primitives for heartbeating and cancellation. The `shared_state_manager` worker parameter must be\nset to an instance of `temporalio.worker.SharedStateManager`. The most common implementation can be created by passing a\n`multiprocessing.managers.SyncManager` (i.e. result of `multiprocessing.managers.Manager()`) to\n`temporalio.worker.SharedStateManager.create_from_multiprocessing()`.\n\nAlso, all of these activity functions must be\n["picklable"](https://docs.python.org/3/library/pickle.html#what-can-be-pickled-and-unpickled).\n\n##### Asynchronous Activities\n\nAsynchronous activities are functions defined with `async def`. Asynchronous activities are often much more performant\nthan synchronous ones. When using asynchronous activities no special worker parameters are needed.\n\n**⚠️ WARNING: Do not block the thread in `async def` Python functions. This can stop the processing of the rest of the\nTemporal.**\n\nCancellation for asynchronous activities is done via\n[`asyncio.Task.cancel`](https://docs.python.org/3/library/asyncio-task.html#asyncio.Task.cancel). This means that\n`asyncio.CancelledError` will be raised (and can be caught, but it is not recommended). A non-local activity must\nheartbeat to receive cancellation and there are other ways to be notified about cancellation (see "Activity Context" and\n"Heartbeating and Cancellation" later).\n\n#### Activity Context\n\nDuring activity execution, an implicit activity context is set as a\n[context variable](https://docs.python.org/3/library/contextvars.html). The context variable itself is not visible, but\ncalls in the `temporalio.activity` package make use of it. Specifically:\n\n* `in_activity()` - Whether an activity context is present\n* `info()` - Returns the immutable info of the currently running activity\n* `heartbeat(*details)` - Record a heartbeat\n* `is_cancelled()` - Whether a cancellation has been requested on this activity\n* `wait_for_cancelled()` - `async` call to wait for cancellation request\n* `wait_for_cancelled_sync(timeout)` - Synchronous blocking call to wait for cancellation request\n* `shield_thread_cancel_exception()` - Context manager for use in `with` clauses by synchronous multithreaded activities\n  to prevent cancel exception from being thrown during the block of code\n* `is_worker_shutdown()` - Whether the worker has started graceful shutdown\n* `wait_for_worker_shutdown()` - `async` call to wait for start of graceful worker shutdown\n* `wait_for_worker_shutdown_sync(timeout)` - Synchronous blocking call to wait for start of graceful worker shutdown\n* `raise_complete_async()` - Raise an error that this activity will be completed asynchronously (i.e. after return of\n  the activity function in a separate client call)\n\nWith the exception of `in_activity()`, if any of the functions are called outside of an activity context, an error\noccurs. Synchronous activities cannot call any of the `async` functions.\n\n##### Heartbeating and Cancellation\n\nIn order for a non-local activity to be notified of cancellation requests, it must be given a `heartbeat_timeout` at\ninvocation time and invoke `temporalio.activity.heartbeat()` inside the activity. It is strongly recommended that all\nbut the fastest executing activities call this function regularly. "Types of Activities" has specifics on cancellation\nfor synchronous and asynchronous activities.\n\nIn addition to obtaining cancellation information, heartbeats also support detail data that is persisted on the server\nfor retrieval during activity retry. If an activity calls `temporalio.activity.heartbeat(123, 456)` and then fails and\nis retried, `temporalio.activity.info().heartbeat_details` will return an iterable containing `123` and `456` on the\nnext run.\n\nHeartbeating has no effect on local activities.\n\n##### Worker Shutdown\n\nAn activity can react to a worker shutdown. Using `is_worker_shutdown` or one of the `wait_for_worker_shutdown`\nfunctions an activity can react to a shutdown.\n\nWhen the `graceful_shutdown_timeout` worker parameter is given a `datetime.timedelta`, on shutdown the worker will\nnotify activities of the graceful shutdown. Once that timeout has passed (or if wasn\'t set), the worker will perform\ncancellation of all outstanding activities.\n\nThe `shutdown()` invocation will wait on all activities to complete, so if a long-running activity does not at least\nrespect cancellation, the shutdown may never complete.\n\n#### Testing\n\nUnit testing an activity or any code that could run in an activity is done via the\n`temporalio.testing.ActivityEnvironment` class. Simply instantiate this and any callable + params passed to `run` will\nbe invoked inside the activity context. The following are attributes/methods on the environment that can be used to\naffect calls activity code might make to functions on the `temporalio.activity` package.\n\n* `info` property can be set to customize what is returned from `activity.info()`\n* `on_heartbeat` property can be set to handle `activity.heartbeat()` calls\n* `cancel()` can be invoked to simulate a cancellation of the activity\n* `worker_shutdown()` can be invoked to simulate a worker shutdown during execution of the activity\n\n### Workflow Replay\n\nGiven a workflow\'s history, it can be replayed locally to check for things like non-determinism errors. For example,\nassuming `history_str` is populated with a JSON string history either exported from the web UI or from `tctl`, the\nfollowing function will replay it:\n\n```python\nfrom temporalio.client import WorkflowHistory\nfrom temporalio.worker import Replayer\n\nasync def run_replayer(history_str: str):\n  replayer = Replayer(workflows=[SayHello])\n  await replayer.replay_workflow(WorkflowHistory.from_json(history_str))\n```\n\nThis will throw an error if any non-determinism is detected.\n\nReplaying from workflow history is a powerful concept that many use to test that workflow alterations won\'t cause\nnon-determinisms with past-complete workflows. The following code will make sure that all workflow histories for a\ncertain workflow type (i.e. workflow class) are safe with the current code.\n\n```python\nfrom temporalio.client import Client, WorkflowHistory\nfrom temporalio.worker import Replayer\n\nasync def check_past_histories(my_client: Client):\n  replayer = Replayer(workflows=[SayHello])\n  await replayer.replay_workflows(\n    await my_client.list_workflows("WorkflowType = \'SayHello\'").map_histories(),\n  )\n```\n\n### OpenTelemetry Support\n\nOpenTelemetry support requires the optional `opentelemetry` dependencies which are part of the `opentelemetry` extra.\nWhen using `pip`, running\n\n    pip install temporalio[opentelemetry]\n\nwill install needed dependencies. Then the `temporalio.contrib.opentelemetry.TracingInterceptor` can be created and set\nas an interceptor on the `interceptors` argument of `Client.connect`. When set, spans will be created for all client\ncalls and for all activity and workflow invocations on the worker, spans will be created and properly serialized through\nthe server to give one proper trace for a workflow execution.\n\n### Protobuf 3.x vs 4.x\n\nPython currently has two somewhat-incompatible protobuf library versions - the 3.x series and the 4.x series. Python\ncurrently recommends 4.x and that is the primary supported version. Some libraries like\n[Pulumi](https://github.com/pulumi/pulumi) require 4.x. Other libraries such as [ONNX](https://github.com/onnx/onnx) and\n[Streamlit](https://github.com/streamlit/streamlit), for one reason or another, have/will not leave 3.x.\n\nTo support these, Temporal Python SDK allows any protobuf library >= 3.19. However, the C extension in older Python\nversions can cause issues with the sandbox due to global state sharing. Temporal strongly recommends using the latest\nprotobuf 4.x library unless you absolutely cannot at which point some proto libraries may have to be marked as\n[Passthrough Modules](#passthrough-modules).\n\n### Known Compatibility Issues\n\nBelow are known compatibility issues with the Python SDK.\n\n#### gevent Patching\n\nWhen using `gevent.monkey.patch_all()`, asyncio event loops can get messed up, especially those using custom event loops\nlike Temporal. See [this gevent issue](https://github.com/gevent/gevent/issues/982). This is a known incompatibility and\nusers are encouraged to not use gevent in asyncio applications (including Temporal). But if you must, there is\n[a sample](https://github.com/temporalio/samples-python/tree/main/gevent_async) showing how it is possible.\n\n# Development\n\nThe Python SDK is built to work with Python 3.8 and newer. It is built using\n[SDK Core](https://github.com/temporalio/sdk-core/) which is written in Rust.\n\n### Building\n\n#### Prepare\n\nTo build the SDK from source for use as a dependency, the following prerequisites are required:\n\n* [Python](https://www.python.org/) >= 3.8\n  * Make sure the latest version of `pip` is in use\n* [Rust](https://www.rust-lang.org/)\n* [poetry](https://github.com/python-poetry/poetry) (e.g. `python -m pip install poetry`)\n* [poe](https://github.com/nat-n/poethepoet) (e.g. `python -m pip install poethepoet`)\n\nmacOS note: If errors are encountered, it may be better to install Python and Rust as recommended from their websites\ninstead of via `brew`.\n\nWith the prerequisites installed, first clone the SDK repository recursively:\n\n```bash\ngit clone --recursive https://github.com/temporalio/sdk-python.git\ncd sdk-python\n```\n\nUse `poetry` to install the dependencies with `--no-root` to not install this package (because we still need to build\nit):\n\n```bash\npoetry install --no-root --all-extras\n```\n\n#### Build\n\nNow perform the release build:\n\n> This will take a while because Rust will compile the core project in release mode (see [Local SDK development\nenvironment](#local-sdk-development-environment) for the quicker approach to local development).\n\n```bash\npoetry build\n```\n\nThe compiled wheel doesn\'t have the exact right tags yet for use, so run this script to fix it:\n\n```bash\npoe fix-wheel\n```\n\nThe `whl` wheel file in `dist/` is now ready to use.\n\n#### Use\n\nThe wheel can now be installed into any virtual environment.\n\nFor example,\n[create a virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments)\nsomewhere and then run the following inside the virtual environment:\n\n```bash\npip install wheel\n```\n\n```bash\npip install /path/to/cloned/sdk-python/dist/*.whl\n```\n\nCreate this Python file at `example.py`:\n\n```python\nimport asyncio\nfrom temporalio import workflow, activity\nfrom temporalio.client import Client\nfrom temporalio.worker import Worker\n\n@workflow.defn\nclass SayHello:\n    @workflow.run\n    async def run(self, name: str) -> str:\n        return f"Hello, {name}!"\n\nasync def main():\n    client = await Client.connect("localhost:7233")\n    async with Worker(client, task_queue="my-task-queue", workflows=[SayHello]):\n        result = await client.execute_workflow(SayHello.run, "Temporal",\n            id="my-workflow-id", task_queue="my-task-queue")\n        print(f"Result: {result}")\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nAssuming there is a [local Temporal server](https://docs.temporal.io/docs/server/quick-install/) running, execute the\nfile with `python` (or `python3` if necessary):\n\n```bash\npython example.py\n```\n\nIt should output:\n\n    Result: Hello, Temporal!\n\n### Local SDK development environment\n\nFor local development, it is often quicker to use debug builds and a local virtual environment.\n\nWhile not required, it often helps IDEs if we put the virtual environment `.venv` directory in the project itself. This\ncan be configured system-wide via:\n\n```bash\npoetry config virtualenvs.in-project true\n```\n\nNow perform the same steps as the "Prepare" section above by installing the prerequisites, cloning the project,\ninstalling dependencies, and generating the protobuf code:\n\n```bash\ngit clone --recursive https://github.com/temporalio/sdk-python.git\ncd sdk-python\npoetry install --no-root --all-extras\n```\n\nNow compile the Rust extension in develop mode which is quicker than release mode:\n\n```bash\npoe build-develop\n```\n\nThat step can be repeated for any Rust changes made.\n\nThe environment is now ready to develop in.\n\n#### Testing\n\nTo execute tests:\n\n```bash\npoe test\n```\n\nThis runs against [Temporalite](https://github.com/temporalio/temporalite). To run against the time-skipping test\nserver, pass `--workflow-environment time-skipping`. To run against the `default` namespace of an already-running\nserver, pass the `host:port` to `--workflow-environment`. Can also use regular pytest arguments. For example, here\'s how\nto run a single test with debug logs on the console:\n\n```bash\npoe test -s --log-cli-level=DEBUG -k test_sync_activity_thread_cancel_caught\n```\n\n#### Proto Generation and Testing\n\nTo allow for backwards compatibility, protobuf code is generated on the 3.x series of the protobuf library. To generate\nprotobuf code, you must be on Python <= 3.10, and then run `poetry add "protobuf<4"`. Then the protobuf files can be\ngenerated via `poe gen-protos`. Tests can be run for protobuf version 3 by setting the `TEMPORAL_TEST_PROTO3` env var\nto `1` prior to running tests.\n\nDo not commit `poetry.lock` or `pyproject.toml` changes. To go back from this downgrade, restore `pyproject.toml` and\nrun `poetry update protobuf grpcio-tools`.\n\nFor a less system-intrusive approach, you can:\n```shell\ndocker build -f scripts/_proto/Dockerfile .\ndocker run -v "${PWD}/temporalio/api:/api_new" -v "${PWD}/temporalio/bridge/proto:/bridge_new" <just built image sha>\npoe format\n```\n\n### Style\n\n* Mostly [Google Style Guide](https://google.github.io/styleguide/pyguide.html). Notable exceptions:\n  * We use [Black](https://github.com/psf/black) for formatting, so that takes precedence\n  * In tests and example code, can import individual classes/functions to make it more readable. Can also do this for\n    rarely in library code for some Python common items (e.g. `dataclass` or `partial`), but not allowed to do this for\n    any `temporalio` packages (except `temporalio.types`) or any classes/functions that aren\'t clear when unqualified.\n  * We allow relative imports for private packages\n  * We allow `@staticmethod`\n',
     'author': 'Temporal Technologies Inc',
     'author_email': 'sdk@temporal.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/temporalio/sdk-python',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `temporalio-1.5.1/PKG-INFO` & `temporalio-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temporalio
-Version: 1.5.1
+Version: 1.6.0
 Summary: Temporal.io Python SDK
 Home-page: https://github.com/temporalio/sdk-python
 License: MIT
 Keywords: temporal,workflow
 Author: Temporal Technologies Inc
 Author-email: sdk@temporal.io
 Requires-Python: >=3.8,<4.0
@@ -748,24 +748,32 @@
 * `continue_as_new()` - Async function to stop the workflow immediately and continue as new
 * `info()` - Returns information about the current workflow
 * `logger` - A logger for use in a workflow (properly skips logging on replay)
 * `now()` - Returns the "current time" from the workflow's perspective
 
 #### Exceptions
 
-* Workflows can raise exceptions to fail the workflow or the "workflow task" (i.e. suspend the workflow retrying).
+* Workflows/updates can raise exceptions to fail the workflow or the "workflow task" (i.e. suspend the workflow
+  in a retrying state).
 * Exceptions that are instances of `temporalio.exceptions.FailureError` will fail the workflow with that exception
   * For failing the workflow explicitly with a user exception, use `temporalio.exceptions.ApplicationError`. This can
     be marked non-retryable or include details as needed.
   * Other exceptions that come from activity execution, child execution, cancellation, etc are already instances of
     `FailureError` and will fail the workflow when uncaught.
 * All other exceptions fail the "workflow task" which means the workflow will continually retry until the workflow is
   fixed. This is helpful for bad code or other non-predictable exceptions. To actually fail the workflow, use an
   `ApplicationError` as mentioned above.
 
+This default can be changed by providing a list of exception types to `workflow_failure_exception_types` when creating a
+`Worker` or `failure_exception_types` on the `@workflow.defn` decorator. If a workflow-thrown exception is an instance
+of any type in either list, it will fail the workflow instead of the task. This means a value of `[Exception]` will
+cause every exception to fail the workflow instead of the task. Also, as a special case, if
+`temporalio.workflow.NondeterminismError` (or any superclass of it) is set, non-deterministic exceptions will fail the
+workflow. WARNING: These settings are experimental.
+
 #### External Workflows
 
 * `workflow.get_external_workflow_handle()` inside a workflow returns a handle to interact with another workflow
 * `workflow.get_external_workflow_handle_for()` can be used instead for a type safe handle
 * `await handle.signal()` can be called on the handle to signal the external workflow
 * `await handle.cancel()` can be called on the handle to send a cancel to the external workflow
```

