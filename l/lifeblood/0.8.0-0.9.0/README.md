# Comparing `tmp/lifeblood-0.8.0.tar.gz` & `tmp/lifeblood-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeblood-0.8.0.tar", last modified: Wed Feb 28 20:25:58 2024, max compression
+gzip compressed data, was "lifeblood-0.9.0.tar", last modified: Sun Mar 10 23:19:47 2024, max compression
```

## Comparing `lifeblood-0.8.0.tar` & `lifeblood-0.9.0.tar`

### file list

```diff
@@ -1,221 +1,222 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.088398 lifeblood-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-28 20:25:42.000000 lifeblood-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-02-28 20:25:58.088398 lifeblood-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-02-28 20:25:42.000000 lifeblood-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-28 20:25:42.000000 lifeblood-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-28 20:25:58.088398 lifeblood-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.052397 lifeblood-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.068398 lifeblood-0.8.0/src/lifeblood/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/aiosqlite_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/basenode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/basenode_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/basenode_serializer_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/basenode_serializer_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/broadcasting.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/buffer_serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/buffered_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/component_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.072398 lifeblood-0.8.0/src/lifeblood/core_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/attribute_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/del_attrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/environment_resolver_setter.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/kill.py
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/mod_attrib.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/null.py
--rw-r--r--   0 runner    (1001) docker     (127)    11495 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/parent_children_waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/rename_attrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/set_attrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/spawn_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/split_waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/wait_for_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/core_nodes/wedge.py
--rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/db_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    18201 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/environment_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/filelock.py
--rw-r--r--   0 runner    (1001) docker     (127)    18955 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/invocationjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/local_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/main_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/main_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/main_workerpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/matrix_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/names.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.072398 lifeblood-0.8.0/src/lifeblood/net_messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.076398 lifeblood-0.8.0/src/lifeblood/net_messages/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/impl/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/impl/message_haldlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/impl/message_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/impl/tcp_message_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/impl/tcp_message_receiver.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/impl/tcp_message_receiver_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/impl/tcp_message_stream_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/impl/tcp_simple_command_message_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12098 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/message_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/message_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    13395 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/net_messages/stream_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/nethelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/node_dataprovider_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/node_type_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/node_visualization_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/nodegraph_holder_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/nodethings.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/os_based_cheats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/plugin_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    15571 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/pluginloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/process_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/processingcontext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/pulse_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/rwlock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.076398 lifeblood-0.8.0/src/lifeblood/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15844 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/scheduler/data_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/scheduler/pinger.py
--rw-r--r--   0 runner    (1001) docker     (127)    94892 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/scheduler/scheduler_component_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/scheduler/state_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    63210 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/scheduler/task_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    40555 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/scheduler/ui_state_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/scheduler_event_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    19092 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/scheduler_message_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/scheduler_task_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    61387 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/scheduler_ui_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/shared_lazy_sqlite_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    22011 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/simple_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/snippets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.076398 lifeblood-0.8.0/src/lifeblood/stock_nodes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.052397 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.080398 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/camera_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/depth_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/depth_map_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/feature_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/image_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/mesh_filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/meshing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/prepare_dense_scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/sfmtransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/structure_from_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/texturing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.052397 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.052397 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/python/3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.080398 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/python/3/lifeblood_alicevision_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/python/3/lifeblood_alicevision_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/python/3/lifeblood_alicevision_modules/base_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.052397 lifeblood-0.8.0/src/lifeblood/stock_nodes/blender/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.080398 lifeblood-0.8.0/src/lifeblood/stock_nodes/blender/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/blender/nodes/blender_batch_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/blender/nodes/blender_script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.080398 lifeblood-0.8.0/src/lifeblood/stock_nodes/blender/presets/
--rw-r--r--   0 runner    (1001) docker     (127)    13410 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/blender/presets/blender_render.lbp
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/fileop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/filepattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/framerange_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.052397 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.080398 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/copy_temp_hip.py
--rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/hip_driver_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/hip_ifd_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/hip_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/hip_usd_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/husk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/karma.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/mantra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.084398 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/presets/
--rw-r--r--   0 runner    (1001) docker     (127)    25180 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/presets/karma.lbp
--rw-r--r--   0 runner    (1001) docker     (127)    25557 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/presets/mantra.lbp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.052397 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.052397 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/python/3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.084398 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/python/3/lifeblood_stock_houdini_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/python/3/lifeblood_stock_houdini_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/python/3/lifeblood_stock_houdini_helpers/rop_base_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.052397 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini_distributed_sim/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.084398 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini_distributed_sim/data/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini_distributed_sim/data/killer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini_distributed_sim/data/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.084398 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini_distributed_sim/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini_distributed_sim/nodes/houdini_distributed_tracker_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini_distributed_sim/nodes/houdini_distributed_tracker_stopper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.084398 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini_distributed_sim/presets/
--rw-r--r--   0 runner    (1001) docker     (127)    18813 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini_distributed_sim/presets/distributed_slices.lbp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.052397 lifeblood-0.8.0/src/lifeblood/stock_nodes/htoa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.084398 lifeblood-0.8.0/src/lifeblood/stock_nodes/htoa/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/htoa/nodes/arnold.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/htoa/nodes/hip_ass_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.084398 lifeblood-0.8.0/src/lifeblood/stock_nodes/htoa/presets/
--rw-r--r--   0 runner    (1001) docker     (127)    25196 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/htoa/presets/htoa.lbp
--rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/imagemagik.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.056397 lifeblood-0.8.0/src/lifeblood/stock_nodes/matrixclient/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.084398 lifeblood-0.8.0/src/lifeblood/stock_nodes/matrixclient/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/matrixclient/data/install_matrix_commander.py
--rw-r--r--   0 runner    (1001) docker     (127)   464243 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/matrixclient/data/matrixclient.pyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.084398 lifeblood-0.8.0/src/lifeblood/stock_nodes/matrixclient/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/matrixclient/nodes/matrixnotifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.056397 lifeblood-0.8.0/src/lifeblood/stock_nodes/redshift/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.084398 lifeblood-0.8.0/src/lifeblood/stock_nodes/redshift/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/redshift/nodes/redshift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.056397 lifeblood-0.8.0/src/lifeblood/stock_nodes/stock_presets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.088398 lifeblood-0.8.0/src/lifeblood/stock_nodes/stock_presets/presets/
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/stock_presets/presets/cache.lbp
--rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/stock_presets/presets/wedge.lbp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.056397 lifeblood-0.8.0/src/lifeblood/stock_nodes/webserver/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.088398 lifeblood-0.8.0/src/lifeblood/stock_nodes/webserver/data/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/webserver/data/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/webserver/data/result_not_ready.html
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/webserver/data/result_ready.html
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/webserver/data/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/webserver/data/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.088398 lifeblood-0.8.0/src/lifeblood/stock_nodes/webserver/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/stock_nodes/webserver/nodes/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/taskspawn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/toml_coders.py
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/ui_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    30011 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/ui_protocol_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    58177 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/uidata.py
--rw-r--r--   0 runner    (1001) docker     (127)    42188 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/worker_invocation_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/worker_messsage_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/worker_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/worker_pool_message_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/worker_pool_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.088398 lifeblood-0.8.0/src/lifeblood/worker_runtime_pythonpath/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/worker_runtime_pythonpath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13189 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/worker_runtime_pythonpath/lifeblood_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12206 2024-02-28 20:25:42.000000 lifeblood-0.8.0/src/lifeblood/worker_task_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:25:58.088398 lifeblood-0.8.0/src/lifeblood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-02-28 20:25:58.000000 lifeblood-0.8.0/src/lifeblood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-02-28 20:25:58.000000 lifeblood-0.8.0/src/lifeblood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 20:25:58.000000 lifeblood-0.8.0/src/lifeblood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-28 20:25:58.000000 lifeblood-0.8.0/src/lifeblood.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-28 20:25:58.000000 lifeblood-0.8.0/src/lifeblood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-28 20:25:58.000000 lifeblood-0.8.0/src/lifeblood.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.999384 lifeblood-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-10 23:19:42.000000 lifeblood-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-03-10 23:19:46.999384 lifeblood-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-10 23:19:42.000000 lifeblood-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-10 23:19:42.000000 lifeblood-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-10 23:19:46.999384 lifeblood-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.963383 lifeblood-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.979383 lifeblood-0.9.0/src/lifeblood/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/aiosqlite_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/basenode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/basenode_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/basenode_serializer_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/basenode_serializer_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/broadcasting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/buffer_serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/buffered_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/component_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.983383 lifeblood-0.9.0/src/lifeblood/core_nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/attribute_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/del_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/environment_resolver_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/kill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/mod_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/null.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11495 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/parent_children_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/rename_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/set_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/spawn_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/split_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/wait_for_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/core_nodes/wedge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/db_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21445 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/environment_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/expiring_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18955 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/invocationjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/local_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/main_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/main_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/main_workerpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/matrix_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.987383 lifeblood-0.9.0/src/lifeblood/net_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.987383 lifeblood-0.9.0/src/lifeblood/net_messages/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/impl/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/impl/message_haldlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/impl/message_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/impl/tcp_message_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/impl/tcp_message_receiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/impl/tcp_message_receiver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/impl/tcp_message_stream_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/impl/tcp_simple_command_message_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12098 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/message_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/message_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13395 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/net_messages/stream_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/nethelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/node_dataprovider_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/node_type_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/node_visualization_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/nodegraph_holder_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/nodethings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/os_based_cheats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/plugin_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15571 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/pluginloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/process_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/processingcontext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/pulse_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/rwlock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.987383 lifeblood-0.9.0/src/lifeblood/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16716 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/scheduler/data_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/scheduler/pinger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94892 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/scheduler/scheduler_component_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/scheduler/state_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64957 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/scheduler/task_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40555 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/scheduler/ui_state_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/scheduler_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19092 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/scheduler_message_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/scheduler_task_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61387 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/scheduler_ui_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/shared_lazy_sqlite_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22011 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/simple_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.991383 lifeblood-0.9.0/src/lifeblood/stock_nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.967383 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.991383 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/camera_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/depth_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/depth_map_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/feature_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/image_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/mesh_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/prepare_dense_scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/sfmtransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/structure_from_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/texturing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.967383 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.967383 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/python/3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.991383 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/python/3/lifeblood_alicevision_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/python/3/lifeblood_alicevision_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/python/3/lifeblood_alicevision_modules/base_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.967383 lifeblood-0.9.0/src/lifeblood/stock_nodes/blender/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.991383 lifeblood-0.9.0/src/lifeblood/stock_nodes/blender/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/blender/nodes/blender_batch_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/blender/nodes/blender_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.991383 lifeblood-0.9.0/src/lifeblood/stock_nodes/blender/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)    13410 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/blender/presets/blender_render.lbp
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/fileop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/filepattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/framerange_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.967383 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.995384 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/copy_temp_hip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/hip_driver_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/hip_ifd_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/hip_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/hip_usd_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/husk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/karma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/mantra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.995384 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)    25180 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/presets/karma.lbp
+-rw-r--r--   0 runner    (1001) docker     (127)    25557 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/presets/mantra.lbp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.967383 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.967383 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/python/3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.995384 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/python/3/lifeblood_stock_houdini_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/python/3/lifeblood_stock_houdini_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/python/3/lifeblood_stock_houdini_helpers/rop_base_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.967383 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini_distributed_sim/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.995384 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini_distributed_sim/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini_distributed_sim/data/killer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini_distributed_sim/data/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.995384 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini_distributed_sim/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini_distributed_sim/nodes/houdini_distributed_tracker_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini_distributed_sim/nodes/houdini_distributed_tracker_stopper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.995384 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini_distributed_sim/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)    18813 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini_distributed_sim/presets/distributed_slices.lbp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.967383 lifeblood-0.9.0/src/lifeblood/stock_nodes/htoa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.995384 lifeblood-0.9.0/src/lifeblood/stock_nodes/htoa/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/htoa/nodes/arnold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/htoa/nodes/hip_ass_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.995384 lifeblood-0.9.0/src/lifeblood/stock_nodes/htoa/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)    25196 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/htoa/presets/htoa.lbp
+-rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/imagemagik.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.967383 lifeblood-0.9.0/src/lifeblood/stock_nodes/matrixclient/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.995384 lifeblood-0.9.0/src/lifeblood/stock_nodes/matrixclient/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/matrixclient/data/install_matrix_commander.py
+-rw-r--r--   0 runner    (1001) docker     (127)   464243 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/matrixclient/data/matrixclient.pyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.995384 lifeblood-0.9.0/src/lifeblood/stock_nodes/matrixclient/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/matrixclient/nodes/matrixnotifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.967383 lifeblood-0.9.0/src/lifeblood/stock_nodes/redshift/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.995384 lifeblood-0.9.0/src/lifeblood/stock_nodes/redshift/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/redshift/nodes/redshift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.967383 lifeblood-0.9.0/src/lifeblood/stock_nodes/stock_presets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.999384 lifeblood-0.9.0/src/lifeblood/stock_nodes/stock_presets/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/stock_presets/presets/cache.lbp
+-rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/stock_presets/presets/wedge.lbp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.967383 lifeblood-0.9.0/src/lifeblood/stock_nodes/webserver/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.999384 lifeblood-0.9.0/src/lifeblood/stock_nodes/webserver/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/webserver/data/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/webserver/data/result_not_ready.html
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/webserver/data/result_ready.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/webserver/data/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/webserver/data/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.999384 lifeblood-0.9.0/src/lifeblood/stock_nodes/webserver/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/stock_nodes/webserver/nodes/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/taskspawn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/toml_coders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/ui_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30011 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/ui_protocol_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58177 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/uidata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42067 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/worker_invocation_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/worker_messsage_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/worker_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/worker_pool_message_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/worker_pool_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.999384 lifeblood-0.9.0/src/lifeblood/worker_runtime_pythonpath/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/worker_runtime_pythonpath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13189 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/worker_runtime_pythonpath/lifeblood_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12206 2024-03-10 23:19:42.000000 lifeblood-0.9.0/src/lifeblood/worker_task_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 23:19:46.999384 lifeblood-0.9.0/src/lifeblood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-03-10 23:19:46.000000 lifeblood-0.9.0/src/lifeblood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-03-10 23:19:46.000000 lifeblood-0.9.0/src/lifeblood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 23:19:46.000000 lifeblood-0.9.0/src/lifeblood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-10 23:19:46.000000 lifeblood-0.9.0/src/lifeblood.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-10 23:19:46.000000 lifeblood-0.9.0/src/lifeblood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-10 23:19:46.000000 lifeblood-0.9.0/src/lifeblood.egg-info/top_level.txt
```

### Comparing `lifeblood-0.8.0/PKG-INFO` & `lifeblood-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: lifeblood
-Version: 0.8.0
+Version: 0.9.0
 Summary: LIFEBLOOD !!
 Home-page: https://github.com/pedohorse/lifeblood
 Author: XAPKOHHEH
 Project-URL: Bug Tracker, https://github.com/pedohorse/lifeblood/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles~=0.8
 Requires-Dist: aiosqlite~=0.17
 Requires-Dist: aiorwlock~=1.3
 Requires-Dist: lz4~=4.0
 Requires-Dist: psutil~=5.8
-Requires-Dist: pywin32==304; platform_system == "Windows"
+Requires-Dist: pywin32==306; platform_system == "Windows"
 Requires-Dist: semantic-version~=2.10
 Requires-Dist: toml~=0.10
 Requires-Dist: watchdog~=2.1
 
 [Documentation](https://pedohorse.github.io/lifeblood)
 
-|master|dev|
-|---|---|
-|[![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml/badge.svg?branch=master)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)<br>[![Tests windows](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml/badge.svg?branch=master)](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml)|[![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)<br>[![Tests windows](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml)|
+| dev                                                                                                                                                                         |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| [![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/tests.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)|
 
 ![](icon/lifeblood.svg)
 
 ## Lifeblood
 Lifeblood is a task/job management software package  
 currently it aims for smaller teams, farms or even individual setups, but with scaling  always in mind.
 
@@ -43,14 +43,16 @@
 processing graph.
 
 This system overview should be very familiar to anyone who saw at least one renderfarm.
 
 check [documentation here](https://pedohorse.github.io/lifeblood)  
 and also [video tutorials](https://pedohorse.github.io/lifeblood/tutorials.html)
 
+## UNDER DEVELOPMENT
+
 ### Features:
 - instantly and easily deployable
 - easy scaling in mind
 - dynamic slots, worker resources management
 - support for environment wrappers (allow you to integrate with existing packaging systems like rez)
 
 ### Features To Be Done:
@@ -66,9 +68,12 @@
 
 ## Installation
 
 There are multiple ways to get Lifeblood to try it out, refer to [installation section in the docs](https://pedohorse.github.io/lifeblood/installation.html#simplest-lifeblood-manager)
 
 In short - easiest way is to use [Lifeblood-Manager](https://github.com/pedohorse/lifeblood-manager/releases), as described in the docs
 
-## UNDER DEVELOPMENT
+## Links
 
+- [blog + support](https://www.patreon.com/xapkohheh)
+- [telegram support/discussion group](https://t.me/+v9klFGZcKVY2MjYy)
+- [documentation](https://pedohorse.github.io/lifeblood)
```

### Comparing `lifeblood-0.8.0/README.md` & `lifeblood-0.9.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [Documentation](https://pedohorse.github.io/lifeblood)
 
-|master|dev|
-|---|---|
-|[![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml/badge.svg?branch=master)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)<br>[![Tests windows](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml/badge.svg?branch=master)](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml)|[![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)<br>[![Tests windows](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml)|
+| dev                                                                                                                                                                         |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| [![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/tests.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)|
 
 ![](icon/lifeblood.svg)
 
 ## Lifeblood
 Lifeblood is a task/job management software package  
 currently it aims for smaller teams, farms or even individual setups, but with scaling  always in mind.
 
@@ -21,14 +21,16 @@
 processing graph.
 
 This system overview should be very familiar to anyone who saw at least one renderfarm.
 
 check [documentation here](https://pedohorse.github.io/lifeblood)  
 and also [video tutorials](https://pedohorse.github.io/lifeblood/tutorials.html)
 
+## UNDER DEVELOPMENT
+
 ### Features:
 - instantly and easily deployable
 - easy scaling in mind
 - dynamic slots, worker resources management
 - support for environment wrappers (allow you to integrate with existing packaging systems like rez)
 
 ### Features To Be Done:
@@ -44,9 +46,12 @@
 
 ## Installation
 
 There are multiple ways to get Lifeblood to try it out, refer to [installation section in the docs](https://pedohorse.github.io/lifeblood/installation.html#simplest-lifeblood-manager)
 
 In short - easiest way is to use [Lifeblood-Manager](https://github.com/pedohorse/lifeblood-manager/releases), as described in the docs
 
-## UNDER DEVELOPMENT
+## Links
 
+- [blog + support](https://www.patreon.com/xapkohheh)
+- [telegram support/discussion group](https://t.me/+v9klFGZcKVY2MjYy)
+- [documentation](https://pedohorse.github.io/lifeblood)
```

### Comparing `lifeblood-0.8.0/setup.cfg` & `lifeblood-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lifeblood
-version = 0.8.0
+version = 0.9.0
 author = XAPKOHHEH
 description = LIFEBLOOD !!
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pedohorse/lifeblood
 project_urls = 
 	Bug Tracker = https://github.com/pedohorse/lifeblood/issues
@@ -20,15 +20,15 @@
 python_requires = >=3.8, <3.11
 install_requires = 
 	aiofiles~=0.8
 	aiosqlite~=0.17
 	aiorwlock~=1.3
 	lz4~=4.0
 	psutil~=5.8
-	pywin32==304; platform_system=="Windows"
+	pywin32==306; platform_system=="Windows"
 	semantic-version~=2.10
 	toml~=0.10
 	watchdog~=2.1
 
 [options.packages.find]
 where = src
 include =
```

### Comparing `lifeblood-0.8.0/src/lifeblood/aiosqlite_overlay.py` & `lifeblood-0.9.0/src/lifeblood/aiosqlite_overlay.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/basenode.py` & `lifeblood-0.9.0/src/lifeblood/basenode.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/basenode_serialization.py` & `lifeblood-0.9.0/src/lifeblood/basenode_serialization.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/basenode_serializer_v1.py` & `lifeblood-0.9.0/src/lifeblood/basenode_serializer_v1.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/basenode_serializer_v2.py` & `lifeblood-0.9.0/src/lifeblood/basenode_serializer_v2.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/broadcasting.py` & `lifeblood-0.9.0/src/lifeblood/broadcasting.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/buffer_serializable.py` & `lifeblood-0.9.0/src/lifeblood/buffer_serializable.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/buffered_connection.py` & `lifeblood-0.9.0/src/lifeblood/buffered_connection.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/component_base.py` & `lifeblood-0.9.0/src/lifeblood/component_base.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/config.py` & `lifeblood-0.9.0/src/lifeblood/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.__write_file_lock = Lock()
 
         self.__sources: List["Path"] = []
         self.__broken_sources: Set["Path"] = set()
 
         self.__config_paths_to_check = [config_path]
         if configd_path.exists() and configd_path.is_dir():
-            self.__config_paths_to_check.extend(configd_path.iterdir())
+            self.__config_paths_to_check.extend(sorted(filepath for filepath in configd_path.iterdir() if filepath.suffix == '.toml'))
 
         self.__stuff = {}
 
         self.__encoder_generator = None
         self.__overrides = {}
         self.set_overrides(overrides)
```

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/attribute_splitter.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/attribute_splitter.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/del_attrib.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/del_attrib.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/environment_resolver_setter.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/environment_resolver_setter.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/kill.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/kill.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/mod_attrib.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/mod_attrib.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/null.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/null.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/parent_children_waiter.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/parent_children_waiter.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/python.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/python.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/rename_attrib.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/rename_attrib.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/set_attrib.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/set_attrib.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/spawn_children.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/spawn_children.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/split_waiter.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/split_waiter.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/switch.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/switch.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/test.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/test.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/wait_for_task.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/wait_for_task.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/core_nodes/wedge.py` & `lifeblood-0.9.0/src/lifeblood/core_nodes/wedge.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/db_misc.py` & `lifeblood-0.9.0/src/lifeblood/db_misc.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/enums.py` & `lifeblood-0.9.0/src/lifeblood/enums.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/environment_resolver.py` & `lifeblood-0.9.0/src/lifeblood/environment_resolver.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,29 +14,33 @@
 import asyncio
 import os
 import sys
 import json
 import inspect
 import pathlib
 import re
+import shutil
 from copy import deepcopy
 from semantic_version import Version, SimpleSpec
 from types import MappingProxyType
 from . import invocationjob, paths, logging
 from .config import get_config
 from .toml_coders import TomlFlatConfigEncoder
-from .process_utils import oh_no_its_windows
+from .process_utils import create_process, oh_no_its_windows
+from .exceptions import ProcessInitializationError
 
-from typing import Dict, Mapping, Optional, Type, Iterable
+from typing import Dict,  Iterable, List, Mapping, Optional, Type
 
 
 _resolvers: Dict[str, Type["BaseEnvironmentResolver"]] = {}  # this should be loaded from plugins
 
 
 def _populate_resolvers():
+    # TODO: This horrible logic needs refactoring. All plugins must be loaded with pluginloader
+    #  everything is tightly coupled here, interdependent... no planing
     for k, v in dict(globals()).items():
         if not inspect.isclass(v) \
                 or not issubclass(v, BaseEnvironmentResolver) \
                 or v == BaseEnvironmentResolver \
                 or v.__module__ != __name__:
             continue
         _resolvers[k] = v
@@ -49,15 +53,15 @@
 
 class ResolutionImpossibleError(RuntimeError):
     pass
 
 
 class EnvironmentResolverArguments:
     """
-    this class objects specity requirements a task/invocation have for int's worker environment wrapper.
+    this class objects specify requirements a task/invocation have for it's worker environment wrapper.
     """
     def __init__(self, resolver_name=None, arguments: Optional[Mapping] = None):
         """
 
         :param resolver_name: if None - treat as no arguments at all
         :param arguments:
         """
@@ -82,57 +86,110 @@
 
     def remove_argument(self, name: str):
         del self.__args[name]
 
     def get_resolver(self):
         return get_resolver(self.__resolver_name)
 
-    def get_environment(self) -> "invocationjob.Environment":
-        return get_resolver(self.name()).get_environment(self.arguments())
+    async def get_environment(self) -> "invocationjob.Environment":
+        return await get_resolver(self.name()).get_environment(self.arguments())
 
     def serialize(self) -> bytes:
-        return json.dumps(self.__dict__).encode('utf-8')
+        return json.dumps({
+            '_EnvironmentResolverArguments__resolver_name': self.__resolver_name,
+            '_EnvironmentResolverArguments__args': self.__args,
+        }).encode('utf-8')
 
     async def serialize_async(self):
         return await asyncio.get_running_loop().run_in_executor(None, self.serialize)
 
     @classmethod
     def deserialize(cls, data: bytes):
         wrp = EnvironmentResolverArguments(None)
-        wrp.__dict__.update(json.loads(data.decode('utf-8')))
+        data_dict = json.loads(data.decode('utf-8'))
+        wrp.__resolver_name = data_dict['_EnvironmentResolverArguments__resolver_name']
+        wrp.__args = data_dict['_EnvironmentResolverArguments__args']
         return wrp
 
     @classmethod
     async def deserialize_async(cls, data: bytes):
         return await asyncio.get_running_loop().run_in_executor(None, cls.deserialize, data)
 
 
 class BaseEnvironmentResolver:
-    def get_environment(self, arguments: Mapping) -> "invocationjob.Environment":
+    async def get_environment(self, arguments: Mapping) -> "invocationjob.Environment":
         """
         this is the main reason for environment wrapper's existance.
         give it your specific arguments
 
         :param additional_env:
         :param arguments:
         :return:
         """
         raise NotImplementedError()
 
+    async def create_process(self, arguments: Mapping, call_args: List[str], *, env: Optional[invocationjob.Environment] = None, cwd: Optional[str] = None) -> asyncio.subprocess.Process:
+        """
+        this should create process, maybe in a special way
+
+        :param arguments: EnvironmentResolverArguments for the resolver
+        :param call_args: what to call: process and arguments
+        :param env: optional environment to launch process in. If None - get_environment should be called
+        :param cwd: current working directory for the process
+        """
+        raise NotImplementedError()
 
-class TrivialEnvironmentResolver(BaseEnvironmentResolver):
+
+class BaseSimpleProcessSpawnEnvironmentResolver(BaseEnvironmentResolver):
+    async def create_process(self, arguments: Mapping, call_args: List[str], *, env: Optional[invocationjob.Environment] = None, cwd: Optional[str] = None) -> asyncio.subprocess.Process:
+        if env is None:
+            env = await self.get_environment(arguments)
+
+        if os.path.isabs(call_args[0]):
+            bin_path = call_args[0]
+        else:
+            bin_path = shutil.which(call_args[0], path=env.get('PATH', ''))
+        if bin_path is None:
+            raise ProcessInitializationError(f'"{call_args[0]}" was not found. Check environment resolver arguments and system setup')
+
+        if cwd is None:
+            cwd = os.path.dirname(bin_path)
+
+        return await create_process(call_args, env, cwd)
+
+
+class BaseSimpleProcessSpawnEnvironmentResolverWithPythonCheat(BaseSimpleProcessSpawnEnvironmentResolver):
+    # even though lifeblood worker runs with python interpreter - it does NOT expect
+    #  python to be available in run environment. User might want to have multiple versions of packaged python.
+    #  However, simple one user artist might not care, and would just want python code to work without any packages setup.
+    #  So to simplify the life of smaller setup users, this hack was introduced.
+    async def create_process(self, arguments: Mapping, call_args: List[str], *, env: Optional[invocationjob.Environment] = None, cwd: Optional[str] = None) -> asyncio.subprocess.Process:
+        """
+        This introduces path to sys.executable if no python is found in PATH, yet `python` is first arg in call_args
+        """
+        if env is None:
+            env = await self.get_environment(arguments)
+        if call_args[0] in ('python', 'python.exe') and shutil.which(call_args[0], path=env.get('PATH', '')) is None:
+            env.append('PATH', os.path.dirname(sys.executable))
+
+        return await super().create_process(arguments, call_args, env=env, cwd=cwd)
+
+
+class TrivialEnvironmentResolver(BaseSimpleProcessSpawnEnvironmentResolverWithPythonCheat):
     """
     trivial environment wrapper does nothing
     """
-    def get_environment(self, arguments: dict) -> "invocationjob.Environment":
+    async def get_environment(self, arguments: Mapping) -> "invocationjob.Environment":
         env = invocationjob.Environment(os.environ)
+        for key, value in arguments.items():
+            env[key] = value
         return env
 
 
-class StandardEnvironmentResolver(BaseEnvironmentResolver):
+class StandardEnvironmentResolver(BaseSimpleProcessSpawnEnvironmentResolverWithPythonCheat):
     """
     will initialize environment based on requested software versions and it's own config
     will raise ResolutionImpossibleError if he doesn't know how to resolve given configuration
 
     example configuration:
     [packages.houdini."18.5.666"]
     env.PATH.prepend=[
@@ -158,15 +215,15 @@
                     self.logger.info(f'found {pkgname} : {verstr}')
             config.set_option_noasync('packages', packages)
             self.logger.info(f'autogenerated config saved to {config.writeable_file()}')
         elif len(config.loaded_files()) == 0:  # so all sources are broken
             self.logger.error('environment resolver configs found, but all have errors! Aborting!')
             raise RuntimeError('all resolver configs are broken')
 
-    def get_environment(self, arguments: Mapping) -> "invocationjob.Environment":
+    async def get_environment(self, arguments: Mapping) -> "invocationjob.Environment":
         """
 
         :param arguments: are expected to be in format of package_name: version_specification
                           like houdini
         :return:
         """
         config = get_config('standard_environment_resolver')
@@ -373,29 +430,29 @@
                                               'entries intact', action='store_true')
 
     schparser = subparser.add_parser('scan', description='scan for software but do NOT generate config files')
     schparser.add_argument('--basepath', '-p', help='optional comma (,) separated base path list to search software in')
 
     opts = parser.parse_args(args)
 
+    logger = logging.get_logger('environment resolver')
+    logger.info('auto detecting packages...')
     packages = StandardEnvironmentResolver.autodetect_software()
     if opts.basepath:
         for basepath in opts.basepath.split(','):
             packages.update(StandardEnvironmentResolver.autodetect_software(basepath))
+    for pkgname, v in packages.items():
+        for verstr in v.keys():
+            logger.info(f'found {pkgname} : {verstr}')
 
     if opts.command == 'generate':
         config = get_config('standard_environment_resolver')
         if opts.output:
             config.override_config_save_location(opts.output)
         config.set_toml_encoder_generator(TomlFlatConfigEncoder)
-        logger = logging.get_logger('environment resolver')
-        logger.info('standard environment resolver is used, but no configuration found. auto generating configuration...')
-        for pkgname, v in packages.items():
-            for verstr in v.keys():
-                logger.info(f'found {pkgname} : {verstr}')
 
         if opts.override:  # do full config override
             config.set_option_noasync('packages', packages)
             logger.info(f'autogenerated config saved to {config.writeable_file()}')
         else:  # if not full override - only add new entries, no touch existing ones
             conf_packages = deepcopy(config.get_option_noasync('packages', {}))
             needs_resaving = False
@@ -409,14 +466,15 @@
                         continue
                     conf_packages[package_name][ver] = meta
                     needs_resaving = True
             if needs_resaving:
                 config.set_option_noasync('packages', conf_packages)
 
     elif opts.command == 'scan':
+        print('\n')
         for pkgname, stuff in packages.items():
             print(f'{pkgname}:')
             for ver, meta in stuff.items():
                 print(f'\t{ver}' + (f' ({meta.get("label", "")})' if 'label' in meta else ''))
                 print('\n'.join(f'\t\t{k}: {v}' for k, v in meta.items() if k != 'label'))
```

### Comparing `lifeblood-0.8.0/src/lifeblood/exceptions.py` & `lifeblood-0.9.0/src/lifeblood/exceptions.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/filelock.py` & `lifeblood-0.9.0/src/lifeblood/filelock.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/invocationjob.py` & `lifeblood-0.9.0/src/lifeblood/invocationjob.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/launch.py` & `lifeblood-0.9.0/src/lifeblood/launch.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/local_notifier.py` & `lifeblood-0.9.0/src/lifeblood/local_notifier.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/logging.py` & `lifeblood-0.9.0/src/lifeblood/logging.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/main_scheduler.py` & `lifeblood-0.9.0/src/lifeblood/main_scheduler.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/main_worker.py` & `lifeblood-0.9.0/src/lifeblood/main_worker.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/main_workerpool.py` & `lifeblood-0.9.0/src/lifeblood/main_workerpool.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/maintenance.py` & `lifeblood-0.9.0/src/lifeblood/maintenance.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/misc.py` & `lifeblood-0.9.0/src/lifeblood/misc.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/names.py` & `lifeblood-0.9.0/src/lifeblood/names.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_classes.py` & `lifeblood-0.9.0/src/lifeblood/net_classes.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/address.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/address.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/client.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/client.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/connections.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/connections.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/exceptions.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/exceptions.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/impl/clients.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/impl/clients.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/impl/message_haldlers.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/impl/message_haldlers.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/impl/message_protocol.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/impl/message_protocol.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/impl/tcp_message_processor.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/impl/tcp_message_processor.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/impl/tcp_message_receiver.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/impl/tcp_message_receiver.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/impl/tcp_message_receiver_factory.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/impl/tcp_message_receiver_factory.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/impl/tcp_message_stream_factory.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/impl/tcp_message_stream_factory.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/impl/tcp_simple_command_message_processor.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/impl/tcp_simple_command_message_processor.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/interfaces.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/interfaces.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/message_processor.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/message_processor.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/message_stream.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/message_stream.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/messages.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/messages.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/queue.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/queue.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/net_messages/stream_wrappers.py` & `lifeblood-0.9.0/src/lifeblood/net_messages/stream_wrappers.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/nethelpers.py` & `lifeblood-0.9.0/src/lifeblood/nethelpers.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/node_dataprovider_base.py` & `lifeblood-0.9.0/src/lifeblood/node_dataprovider_base.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/node_type_metadata.py` & `lifeblood-0.9.0/src/lifeblood/node_type_metadata.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/nodegraph_holder_base.py` & `lifeblood-0.9.0/src/lifeblood/nodegraph_holder_base.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/nodethings.py` & `lifeblood-0.9.0/src/lifeblood/nodethings.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/paths.py` & `lifeblood-0.9.0/src/lifeblood/paths.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/plugin_info.py` & `lifeblood-0.9.0/src/lifeblood/plugin_info.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/pluginloader.py` & `lifeblood-0.9.0/src/lifeblood/pluginloader.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/process_utils.py` & `lifeblood-0.9.0/src/lifeblood/process_utils.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/processingcontext.py` & `lifeblood-0.9.0/src/lifeblood/processingcontext.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/pulse_checker.py` & `lifeblood-0.9.0/src/lifeblood/pulse_checker.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/rwlock.py` & `lifeblood-0.9.0/src/lifeblood/rwlock.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/scheduler/data_access.py` & `lifeblood-0.9.0/src/lifeblood/scheduler/data_access.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import aiosqlite
 import sqlite3
 import random
 import struct
 import json
 from dataclasses import dataclass
 from ..db_misc import sql_init_script
+from ..expiring_collections import ExpiringValuesSetMap
+from ..config import get_config
 from ..enums import TaskState, InvocationState
 from ..worker_metadata import WorkerMetadata
 from ..logging import get_logger
 from ..shared_lazy_sqlite_connection import SharedLazyAiosqliteConnection
 from .. import aiosqlite_overlay
 from ..environment_resolver import EnvironmentResolverArguments
 
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Dict, Iterable, Optional, Tuple
 
 SCHEDULER_DB_FORMAT_VERSION = 2
 
 
 @dataclass
 class InvocationStatistics:
     invoking: int
@@ -46,14 +48,18 @@
         # "public" members
         self.mem_cache_workers_resources: dict = {}
         self.mem_cache_workers_state: dict = {}
         self.mem_cache_invocations: dict = {}
         #
 
         self.__task_blocking_values: Dict[int, int] = {}
+        # on certain submission errors we might want to ban hwid for some time, as it can be assumed
+        # that consecutive submission attempts will result in the same error (like package resolution error)
+        self.__banned_hwids_per_task: ExpiringValuesSetMap = ExpiringValuesSetMap()
+        self.__ban_time = get_config('scheduler').get_option_noasync('data_access.hwid_ban_timeout', 10)
 
         self.__workers_metadata: Dict[int, WorkerMetadata] = {}
         #
         # ensure database is initialized
         with sqlite3.connect(db_path) as con:
             con.executescript(sql_init_script)
         with sqlite3.connect(db_path) as con:
@@ -190,16 +196,27 @@
         if not con.in_transaction:
             await con.execute('BEGIN IMMEDIATE')
         await self.hint_task_needs_unblocking(task_id, dec_amount=self.__task_blocking_values[task_id], con=con)
         # we just remove task_id from dict, as default value is 0
         # And we ensure it is done within a transaction
         self.__task_blocking_values.pop(task_id)
 
+    #
+
+    def suspend_hwid(self, task_id: int, hwid: int):
+        self.__banned_hwids_per_task.add_expiring_value(task_id, hwid, self.__ban_time)
+
     # task query
 
+    def get_suspended_hwids(self, task_id: int) -> Iterable[int]:
+        return self.__banned_hwids_per_task.get_values(task_id, prune=True)
+
+    def prune_suspended_hwids(self):
+        self.__banned_hwids_per_task.prune()
+
     async def is_task_blocked(self, task_id: int, *, con: Optional[aiosqlite.Connection] = None) -> bool:
         """
         is task blocked
         TODO: use get_task_state when it's moved here from scheduler
         """
         if con is None:
             async with self.data_connection() as con:
```

### Comparing `lifeblood-0.8.0/src/lifeblood/scheduler/pinger.py` & `lifeblood-0.9.0/src/lifeblood/scheduler/pinger.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/scheduler/scheduler.py` & `lifeblood-0.9.0/src/lifeblood/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/scheduler/scheduler_component_base.py` & `lifeblood-0.9.0/src/lifeblood/scheduler/scheduler_component_base.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/scheduler/task_processor.py` & `lifeblood-0.9.0/src/lifeblood/scheduler/task_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -370,21 +370,23 @@
             # actually communicating submission to the worker
             self.__logger.debug(f'submitting task to {addr}')
             try:
                 # this is potentially a long operation - db must NOT be locked during it
                 with WorkerControlClient.get_worker_control_client(addr, self.scheduler.message_processor()) as client:  # type: WorkerControlClient
                     # import random
                     # await asyncio.sleep(random.uniform(0, 8))  # DEBUG! IMITATE HIGH LOAD
-                    reply = await client.give_task(job, self.scheduler.server_message_address())
+                    reply, fail_class, reply_message = await client.give_task(job, self.scheduler.server_message_address())
                     # TODO: introduce optional "worker cookie" - uid that one passes with some commands
                     #  like give_task to ensure that we are submitting here to the same worker task processing loop selected
-                self.__logger.debug(f'got reply {reply}')
+                self.__logger.debug(f'got reply {reply} ({fail_class}), ({reply_message})')
             except Exception as e:
                 self.__logger.error('some unexpected error %s %s' % (str(type(e)), str(e)))
                 reply = TaskScheduleStatus.FAILED
+                fail_class = 'submission'
+                reply_message = None
 
             # Second main transaction of the submission
             async with self.awaiter_lock:
                 await submit_transaction.execute('BEGIN IMMEDIATE')
                 async with submit_transaction.execute('SELECT "state" FROM workers WHERE "id" == ?', (worker_row['id'],)) as incur:
                     worker_state = WorkerState((await incur.fetchone())[0])
                 async with submit_transaction.execute('SELECT "state" FROM invocations WHERE "id" == ?', (invocation_id,)) as incur:
@@ -427,14 +429,27 @@
                     self.__logger.warning(f'submitter failed, rolling back for wid {worker_row["id"]}')
                     ui_task_delta.state = TaskState.READY  # for ui event
                     # for now invoking invocation are invalidated by deletion (here and in scheduler start)
                     await submit_transaction.execute('DELETE FROM invocations WHERE "id" = ?',
                                                      (invocation_id,))
                     await self.__submitter_finalize_cancel_transaction(submit_transaction, worker_row, worker_state, task_id)
 
+                    if reply == TaskScheduleStatus.FAILED:
+                        if reply_message:
+                            state_details = json.dumps({'message': f'worker {worker_row["id"]} failed to take task: {reply_message}',
+                                                        'happened_at': task_row['state'],
+                                                        'type': fail_class,
+                                                        })
+                            await submit_transaction.execute('UPDATE tasks SET state_details = ? WHERE "id" == ?',
+                                                             (state_details, task_id))
+                        # for some fail reasons we put workers into a temporary suspend list,
+                        #  not to spam and get same error hundreds of times per second
+                        if fail_class in ('environment_resolver', 'spawn'):
+                            self.scheduler.data_access.suspend_hwid(task_id, worker_row['hwid'])
+
                     # we poke scheduler after transaction commit to process task again straight away
                     submit_transaction.add_after_commit_callback(self.poke)
                 submit_transaction.add_after_commit_callback(self.scheduler.ui_state_access.scheduler_reports_task_updated, ui_task_delta)  # ui event
                 await submit_transaction.commit()
 
     async def __submitter_finalize_cancel_transaction(self, submit_transaction, worker_row, worker_state: WorkerState, task_id: int):
         """
@@ -450,22 +465,32 @@
         #
         await submit_transaction.execute('UPDATE workers SET state = ? WHERE "id" = ?',
                                          (WorkerState.IDLE.value if worker_state != WorkerState.OFF else WorkerState.OFF.value,
                                           worker_row['id']))
         # update resource usage to none
         await self.scheduler._update_worker_resouce_usage(worker_row['id'], hwid=worker_row['hwid'], connection=submit_transaction)
 
+    @atimeit(0)
+    async def __task_processor_housekeeping(self):
+        """
+        some cleanup operations that can be done every once in a rare while
+        """
+        self.__logger.debug('performing housekeeping')
+        self.scheduler.data_access.prune_suspended_hwids()
+
     #
 
     async def task_processor(self):
         # this will hold references to tasks created with asyncio.create_task
         tasks_to_wait = set()
         stop_task = asyncio.create_task(self._stop_event.wait())
         kick_wait_task = asyncio.create_task(self._poke_event.wait())
         gc_counter = 0
+        housekeeping_timestamp = time.monotonic()
+        housekeeping_interval = await get_config('scheduler').get_option('task_processor.housekeeping_interval', 60)
         # tm_counter = 0
         self._main_task_is_ready_now()
         while not self._stop_event.is_set():
             data_access = self.scheduler.data_access
             gc_counter += 1
             # tm_counter += 1
             if gc_counter >= 120:  # TODO: to config this timing
@@ -527,14 +552,20 @@
                     to_remove.add(task_to_wait)
                     try:
                         await task_to_wait
                     except Exception as e:
                         self.__logger.exception('awaited task raised some problems')
             tasks_to_wait -= to_remove
 
+            # housekeeping
+            housekeeping_now = time.monotonic()
+            if housekeeping_now - housekeeping_timestamp > housekeeping_interval:
+                await self.__task_processor_housekeeping()
+                housekeeping_timestamp = housekeeping_now
+
             # now proceed with processing
             _debug_con = time.perf_counter()
             total_processed = 0
             total_state_changes = 0  # note that total_state_changes may be greater than total_processed, as total_processed refers to existing tasks only, but total_state_changes counts new splits as well
             async with data_access.data_connection() as con:
                 con.row_factory = aiosqlite.Row
 
@@ -648,104 +679,15 @@
                             await con.executemany('UPDATE tasks SET "state" = ? WHERE "id" = ?', set_to_stuff)
                             await con.commit()
                         for coro in awaiters:
                             tasks_to_wait.add(asyncio.create_task(coro))  # note - dont change to run in executors in threads - there are things here like asyncio locks that RELY ON BEING IN SAME THREAD
                     #
                     # real scheduling should happen here
                     elif task_state == TaskState.READY:
-                        submitters = []
-                        # there may be a lot of similar queries, and if there's nothing available at some point - we may just leave it for next submission iteration
-                        # and anyway - if transaction has already started - there wont be any new idle worker, since sqlite block everything
-                        where_empty_cache = set()
-                        ui_task_deltas = []  # for ui event
-                        task_rows_to_retry = []
-                        for task_row in itertools.chain(all_task_rows, task_rows_to_retry):
-                            # check max attempts first
-                            if task_row['work_data_invocation_attempt'] >= self.__invocation_attempts:
-                                state_details = json.dumps({'message': 'maximum invocation attempts reached',
-                                                               'happened_at': task_row['state'],
-                                                               'type': 'limit',
-                                                               'limit_threshold': self.__invocation_attempts,
-                                                               'limit_value': task_row['work_data_invocation_attempt']})
-                                await con.execute('UPDATE tasks SET "state" = ?, "state_details" = ? WHERE "id" = ?',
-                                                  (TaskState.ERROR.value,
-                                                   state_details,
-                                                   task_row['id']))
-                                total_state_changes += 1
-                                ui_task_deltas.append(TaskDelta(task_row['id'], state=TaskState.ERROR, state_details=state_details))  # for ui event
-                                self.__logger.warning(f'{task_row["id"]} reached maximum invocation attempts, setting it to error state')
-                                continue
-                            #
-                            requirements_clause_sql: str = task_row["_invoc_requirement_clause"]
-                            requirements_clause_dict = None
-                            if (splitpos := requirements_clause_sql.rfind(':::')) > -1:
-                                requirements_clause_dict = json.loads(requirements_clause_sql[splitpos+3:])
-                                requirements_clause_sql = requirements_clause_sql[:splitpos]
-                            if requirements_clause_sql in where_empty_cache:
-                                continue
-                            try:
-                                self.__logger.debug('submitter selecting worker')
-                                async with con.execute(f'SELECT workers.id, workers.hwid, last_address from workers '
-                                                       f'INNER JOIN resources ON workers.hwid=resources.hwid '
-                                                       f'WHERE state == ? AND ( {requirements_clause_sql} ) ORDER BY RANDOM() LIMIT 1', (WorkerState.IDLE.value,)) as worcur:
-                                    worker = await worcur.fetchone()
-                            except aiosqlite.Error as e:
-                                state_details = json.dumps({'message': traceback.format_exc(),
-                                                               'happened_at': task_row['state'],
-                                                               'type': 'exception',
-                                                               'exception_str': str(e),
-                                                               'exception_type': str(type(e))})
-                                await con.execute('UPDATE tasks SET "state" = ?, "state_details" = ? WHERE "id" = ?',
-                                                  (TaskState.ERROR.value,
-                                                   state_details,
-                                                   task_row['id']))
-                                total_state_changes += 1
-                                ui_task_deltas.append(TaskDelta(task_row['id'], state=TaskState.ERROR, state_details=state_details))  # for ui event
-                                self.__logger.exception(f'error matching workers for the task {task_row["id"]}')
-                                continue
-                            if worker is None:  # nothing available
-                                where_empty_cache.add(requirements_clause_sql)
-                                continue
-                            # note that there might be no implicit transaction here yet, so previously selected
-                            # worker might have changed states between that select and this update
-                            # so we doublecheck in a transaction
-                            if not con.in_transaction:
-                                await con.execute('BEGIN IMMEDIATE')
-                                async with con.execute('SELECT "state" FROM workers WHERE "id" == ?', (worker['id'],)) as worcur:
-                                    actual_state = (await worcur.fetchone())['state']
-                                    if actual_state != WorkerState.IDLE.value:
-                                        self.__logger.debug(f'submitter: worker changed state (to {actual_state}) while trying to submit, skipping')
-                                        # we add to retry list, and we don't care to limit it,
-                                        # cuz this code is only reachable if we were NOT in a transaction, and now we are
-                                        task_rows_to_retry.append(task_row)
-                                        continue
-                            await con.execute('UPDATE tasks SET state = ? WHERE "id" = ?',
-                                              (TaskState.INVOKING.value, task_row['id']))
-                            total_state_changes += 1
-                            ui_task_deltas.append(TaskDelta(task_row['id'], state=TaskState.INVOKING))  # for ui event
-                            await con.execute('UPDATE workers SET state = ? WHERE "id" = ?',
-                                              (WorkerState.INVOKING.value, worker['id']))
-                            # set resource usage straight away
-                            try:
-                                await self.scheduler._update_worker_resouce_usage(worker['id'], resources=requirements_clause_dict, hwid=worker['hwid'], connection=con)
-                            except NotEnoughResources:
-                                self.__logger.warning(f'inconsistence in worker resource tracking! could not submit to worker {worker["id"]}')
-                                continue
-
-                            submitters.append(self._submitter(dict(task_row), dict(worker)))
-                            self.__logger.debug('submitter scheduled')
-                        # ui event
-                        if ui_task_deltas:
-                            con.add_after_commit_callback(
-                                self.scheduler.ui_state_access.scheduler_reports_tasks_updated, ui_task_deltas
-                            )
-                        #
-                        await con.commit()
-                        for coro in submitters:
-                            tasks_to_wait.add(asyncio.create_task(coro))
+                        total_state_changes += await self.__process_ready(all_task_rows, tasks_to_wait, con=con)
                     #
                     # means task is done being processed by current node,
                     # now it should be passed to the next node
                     elif task_state == TaskState.DONE or task_state == TaskState.SPAWNED:
                         ui_task_deltas = []  # for ui event
                         for task_row in all_task_rows:
                             if task_row['state'] == TaskState.DONE.value:
@@ -838,14 +780,127 @@
         for task in (stop_task, kick_wait_task):
             if not task.done():
                 task.cancel()
         if len(tasks_to_wait) > 0:
             await asyncio.wait(tasks_to_wait, return_when=asyncio.ALL_COMPLETED)
         self.__logger.info('task processor finished')
 
+    async def __process_ready(self, all_task_rows, tasks_to_wait, *, con: aiosqlite_overlay.ConnectionWithCallbacks) -> int:
+        """
+        does all the processing for tasks in READY state
+        helper for task_processor routine
+
+        returns number of tasks that had changes
+        """
+        total_state_changes = 0
+        submitters = []
+        # there may be a lot of similar queries, and if there's nothing available at some point - we may just leave it for next submission iteration
+        # and anyway - if transaction has already started - there wont be any new idle worker, since sqlite block everything
+        where_empty_cache = set()
+        ui_task_deltas = []  # for ui event
+        task_rows_to_retry = []
+        for task_row in itertools.chain(all_task_rows, task_rows_to_retry):
+            # check max attempts first
+            if task_row['work_data_invocation_attempt'] >= self.__invocation_attempts:
+                state_details = json.dumps({'message': 'maximum invocation attempts reached',
+                                            'happened_at': task_row['state'],
+                                            'type': 'limit',
+                                            'limit_threshold': self.__invocation_attempts,
+                                            'limit_value': task_row['work_data_invocation_attempt']})
+                await con.execute('UPDATE tasks SET "state" = ?, "state_details" = ? WHERE "id" = ?',
+                                  (TaskState.ERROR.value,
+                                   state_details,
+                                   task_row['id']))
+                total_state_changes += 1
+                ui_task_deltas.append(TaskDelta(task_row['id'], state=TaskState.ERROR, state_details=state_details))  # for ui event
+                self.__logger.warning(f'{task_row["id"]} reached maximum invocation attempts, setting it to error state')
+                continue
+            #
+            requirements_clause_sql: str = task_row["_invoc_requirement_clause"]
+            requirements_clause_dict = None
+            if (splitpos := requirements_clause_sql.rfind(':::')) > -1:
+                requirements_clause_dict = json.loads(requirements_clause_sql[splitpos + 3:])
+                requirements_clause_sql = requirements_clause_sql[:splitpos]
+            if requirements_clause_sql in where_empty_cache:
+                continue
+            try:
+                self.__logger.debug('submitter selecting worker')
+                # we get total for further optimizations
+                async with con.execute(f'SELECT COUNT(workers.id) as "total" from workers '
+                                       f'INNER JOIN resources ON workers.hwid=resources.hwid '
+                                       f'WHERE state == ? AND ( {requirements_clause_sql} )', (WorkerState.IDLE.value,)) as worcur:
+                    potential_count = (await worcur.fetchone())['total']
+                # actual selecting workers
+                async with con.execute(f'SELECT workers.id, workers.hwid, last_address from workers '
+                                       f'INNER JOIN resources ON workers.hwid=resources.hwid '
+                                       f'WHERE state == ? AND ( {requirements_clause_sql} ) '
+                                       f'AND workers.hwid NOT IN ({",".join(str(x) for x in self.scheduler.data_access.get_suspended_hwids(task_row["id"]))}) '
+                                       f'ORDER BY RANDOM() LIMIT 1', (WorkerState.IDLE.value,)) as worcur:
+                    worker = await worcur.fetchone()
+            except aiosqlite.Error as e:  # wait, how can this happen?
+                state_details = json.dumps({'message': traceback.format_exc(),
+                                            'happened_at': task_row['state'],
+                                            'type': 'exception',
+                                            'exception_str': str(e),
+                                            'exception_type': str(type(e))})
+                await con.execute('UPDATE tasks SET "state" = ?, "state_details" = ? WHERE "id" = ?',
+                                  (TaskState.ERROR.value,
+                                   state_details,
+                                   task_row['id']))
+                total_state_changes += 1
+                ui_task_deltas.append(TaskDelta(task_row['id'], state=TaskState.ERROR, state_details=state_details))  # for ui event
+                self.__logger.exception(f'error matching workers for the task {task_row["id"]}')
+                continue
+            if potential_count == 0:  # nothing available
+                where_empty_cache.add(requirements_clause_sql)
+            if worker is None:
+                self.__logger.debug('submitter: no worker available')
+                continue
+            # note that there might be no implicit transaction here yet, so previously selected
+            # worker might have changed states between that select and this update
+            # so we doublecheck in a transaction
+            if not con.in_transaction:
+                await con.execute('BEGIN IMMEDIATE')
+                async with con.execute('SELECT "state" FROM workers WHERE "id" == ?', (worker['id'],)) as worcur:
+                    actual_state = (await worcur.fetchone())['state']
+                    if actual_state != WorkerState.IDLE.value:
+                        self.__logger.debug(f'submitter: worker changed state (to {actual_state}) while trying to submit, skipping')
+                        # we add to retry list, and we don't care to limit it,
+                        # cuz this code is only reachable if we were NOT in a transaction, and now we are
+                        task_rows_to_retry.append(task_row)
+                        continue
+
+            # set resource usage straight away
+            try:
+                await self.scheduler._update_worker_resouce_usage(worker['id'], resources=requirements_clause_dict, hwid=worker['hwid'], connection=con)
+            except NotEnoughResources:
+                self.__logger.error(f'inconsistency in worker resource tracking! could not submit to worker {worker["id"]}')
+                continue
+
+            await con.execute('UPDATE tasks SET state = ? WHERE "id" = ?',
+                              (TaskState.INVOKING.value, task_row['id']))
+            total_state_changes += 1
+            ui_task_deltas.append(TaskDelta(task_row['id'], state=TaskState.INVOKING))  # for ui event
+            await con.execute('UPDATE workers SET state = ? WHERE "id" = ?',
+                              (WorkerState.INVOKING.value, worker['id']))
+
+            submitters.append(self._submitter(dict(task_row), dict(worker)))
+            self.__logger.debug('submitter scheduled')
+        # ui event
+        if ui_task_deltas:
+            con.add_after_commit_callback(
+                self.scheduler.ui_state_access.scheduler_reports_tasks_updated, ui_task_deltas
+            )
+        #
+        await con.commit()
+        for coro in submitters:
+            tasks_to_wait.add(asyncio.create_task(coro))
+
+        return total_state_changes
+
     # helpers
 
     async def split_task(self, task_id: int, into: int, con: aiosqlite_overlay.ConnectionWithCallbacks) -> List[int]:
         """
         con is expected to be a opened db connection with dict factory
         :param task_id
         :param into:
```

### Comparing `lifeblood-0.8.0/src/lifeblood/scheduler/ui_state_accessor.py` & `lifeblood-0.9.0/src/lifeblood/scheduler/ui_state_accessor.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/scheduler_event_log.py` & `lifeblood-0.9.0/src/lifeblood/scheduler_event_log.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/scheduler_message_processor.py` & `lifeblood-0.9.0/src/lifeblood/scheduler_message_processor.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/scheduler_task_protocol.py` & `lifeblood-0.9.0/src/lifeblood/scheduler_task_protocol.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/scheduler_ui_protocol.py` & `lifeblood-0.9.0/src/lifeblood/scheduler_ui_protocol.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/shared_lazy_sqlite_connection.py` & `lifeblood-0.9.0/src/lifeblood/shared_lazy_sqlite_connection.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/simple_worker_pool.py` & `lifeblood-0.9.0/src/lifeblood/simple_worker_pool.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/snippets.py` & `lifeblood-0.9.0/src/lifeblood/snippets.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/camera_init.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/camera_init.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/depth_map.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/depth_map.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/depth_map_filter.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/depth_map_filter.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/feature_extraction.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/feature_matching.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/feature_matching.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/image_matching.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/image_matching.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/mesh_filtering.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/mesh_filtering.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/meshing.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/meshing.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/prepare_dense_scene.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/prepare_dense_scene.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/sfmtransform.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/sfmtransform.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/structure_from_motion.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/structure_from_motion.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/alicevision/nodes/texturing.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/alicevision/nodes/texturing.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/blender/nodes/blender_batch_render.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/blender/nodes/blender_batch_render.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/blender/nodes/blender_script.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/blender/nodes/blender_script.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/blender/presets/blender_render.lbp` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/blender/presets/blender_render.lbp`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/ffmpeg.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/file_watcher.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/file_watcher.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/fileop.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/fileop.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/filepattern.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/filepattern.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/framerange_splitter.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/framerange_splitter.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/copy_temp_hip.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/copy_temp_hip.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/hip_driver_renderer.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/hip_driver_renderer.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/hip_ifd_generator.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/hip_ifd_generator.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/hip_script.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/hip_script.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/hip_usd_generator.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/hip_usd_generator.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/husk.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/husk.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/karma.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/karma.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/nodes/mantra.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/nodes/mantra.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/presets/karma.lbp` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/presets/karma.lbp`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/presets/mantra.lbp` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/presets/mantra.lbp`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini/python/3/lifeblood_stock_houdini_helpers/rop_base_node.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini/python/3/lifeblood_stock_houdini_helpers/rop_base_node.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini_distributed_sim/data/server.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini_distributed_sim/data/server.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini_distributed_sim/nodes/houdini_distributed_tracker_runner.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini_distributed_sim/nodes/houdini_distributed_tracker_runner.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini_distributed_sim/nodes/houdini_distributed_tracker_stopper.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini_distributed_sim/nodes/houdini_distributed_tracker_stopper.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/houdini_distributed_sim/presets/distributed_slices.lbp` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/houdini_distributed_sim/presets/distributed_slices.lbp`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/htoa/nodes/arnold.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/htoa/nodes/arnold.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/htoa/nodes/hip_ass_generator.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/htoa/nodes/hip_ass_generator.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/htoa/presets/htoa.lbp` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/htoa/presets/htoa.lbp`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/imagemagik.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/imagemagik.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/matrixclient/data/install_matrix_commander.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/matrixclient/data/install_matrix_commander.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/matrixclient/data/matrixclient.pyz` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/matrixclient/data/matrixclient.pyz`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/matrixclient/nodes/matrixnotifier.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/matrixclient/nodes/matrixnotifier.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/redshift/nodes/redshift.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/redshift/nodes/redshift.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/stock_presets/presets/cache.lbp` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/stock_presets/presets/cache.lbp`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/stock_presets/presets/wedge.lbp` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/stock_presets/presets/wedge.lbp`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/webserver/data/index.html` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/webserver/data/index.html`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/webserver/data/server.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/webserver/data/server.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/webserver/data/styles.css` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/webserver/data/styles.css`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/stock_nodes/webserver/nodes/webserver.py` & `lifeblood-0.9.0/src/lifeblood/stock_nodes/webserver/nodes/webserver.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/taskspawn.py` & `lifeblood-0.9.0/src/lifeblood/taskspawn.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/text.py` & `lifeblood-0.9.0/src/lifeblood/text.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/toml_coders.py` & `lifeblood-0.9.0/src/lifeblood/toml_coders.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/ui_events.py` & `lifeblood-0.9.0/src/lifeblood/ui_events.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/ui_protocol_data.py` & `lifeblood-0.9.0/src/lifeblood/ui_protocol_data.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/uidata.py` & `lifeblood-0.9.0/src/lifeblood/uidata.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/worker.py` & `lifeblood-0.9.0/src/lifeblood/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 import datetime
 import time
 import tempfile
 from . import logging
 from .nethelpers import get_addr_to, get_localhost, get_hostname
 from .net_classes import WorkerResources
 from .worker_metadata import WorkerMetadata
-from .exceptions import ProcessInitializationError, WorkerNotAvailable, AlreadyRunning,\
+from .exceptions import WorkerNotAvailable, AlreadyRunning, \
     InvocationMessageWrongInvocationId, InvocationMessageAddresseeTimeout, InvocationCancelled
 from .worker_messsage_processor import WorkerMessageProcessor
 from .scheduler_message_processor import SchedulerWorkerControlClient
 from .worker_invocation_protocol import WorkerInvocationProtocolHandlerV10, WorkerInvocationServerProtocol
 from .worker_pool_message_processor import WorkerPoolControlClient
 from .invocationjob import InvocationJob
 from .config import get_config
 from . import environment_resolver
 from .enums import WorkerType, WorkerState, ProcessPriorityAdjustment
 from .paths import config_path
-from .process_utils import create_process, kill_process_tree
+from .process_utils import kill_process_tree
 from .misc import event_set_context
 from .net_messages.address import AddressChain, DirectAddress
 from .net_messages.exceptions import MessageTransferError
 from .defaults import worker_start_port as default_worker_start_port
 
 from .worker_runtime_pythonpath import lifeblood_connection
 import inspect
@@ -340,18 +340,22 @@
                         args.append(arg)
             else:
                 args = task.args()
 
             try:
                 if task.environment_resolver_arguments() is None:
                     config = get_config('worker')
-                    env = environment_resolver.get_resolver(config.get_option_noasync('default_env_wrapper.name', 'TrivialEnvironmentResolver'))\
-                        .get_environment(config.get_option_noasync('default_env_wrapper.arguments', {}))
+                    resolver = environment_resolver.get_resolver(config.get_option_noasync('default_env_wrapper.name', 'TrivialEnvironmentResolver'))
+                    resolver_arguments = config.get_option_noasync('default_env_wrapper.arguments', {})
                 else:
-                    env = task.environment_resolver_arguments().get_environment()
+                    env_res_args = task.environment_resolver_arguments()
+                    resolver = env_res_args.get_resolver()
+                    resolver_arguments = env_res_args.arguments()
+
+                env = await resolver.get_environment(resolver_arguments)
             except environment_resolver.ResolutionImpossibleError as e:
                 self.__logger.error(f'cannot run the task: Unable to resolve environment: {str(e)}')
                 raise
 
             # TODO: resolver args get_environment() acually does resolution so should be renamed to like resolve_environment()
             #  Environment's resolve() actually just expands and merges everything, so naming it "resolve" is misleading next to EnvironmentResolver
 
@@ -373,22 +377,19 @@
                 env['LB_EF_ROOT'] = self.__extra_files_base_dir
             try:
                 #with open(self.get_log_filepath('output', task.invocation_id()), 'a') as stdout:
                 #    with open(self.get_log_filepath('error', task.invocation_id()), 'a') as stderr:
                 # TODO: proper child process priority adjustment should be done, for now it's implemented in constructor.
                 self.__running_process_start_time = time.time()
 
-                if os.path.isabs(args[0]):
-                    bin_path = args[0]
-                else:
-                    bin_path = shutil.which(args[0], path=env.get('PATH'))
-                if bin_path is None:
-                    raise ProcessInitializationError(f'"{args[0]}" was not found. Check environment resolver arguments and system setup')
-
-                self.__running_process: asyncio.subprocess.Process = await create_process(args, env, os.path.dirname(bin_path))
+                self.__running_process: asyncio.subprocess.Process = await resolver.create_process(
+                    resolver_arguments,
+                    args,
+                    env=env
+                )
             except Exception as e:
                 self.__logger.exception('task creation failed with error: %s' % (repr(e),))
                 raise
 
             self.__running_task = task
             self.__running_awaiter = asyncio.create_task(self._awaiter())
             self.__running_task_progress = 0
```

### Comparing `lifeblood-0.8.0/src/lifeblood/worker_invocation_protocol.py` & `lifeblood-0.9.0/src/lifeblood/worker_invocation_protocol.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/worker_messsage_processor.py` & `lifeblood-0.9.0/src/lifeblood/worker_messsage_processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -82,29 +82,40 @@
         try:
             self.__logger.debug('taking the task')
             await self.__worker.run_task(task, addr)
             reply['status'] = TaskScheduleStatus.SUCCESS.value
         except AlreadyRunning:
             self.__logger.debug('BUSY. rejecting task')
             reply['status'] = TaskScheduleStatus.BUSY.value
+            reply['message'] = 'worker already working on a task'
         except ResolutionImpossibleError:
             self.__logger.info('Worker failed to resolve required environment. rejecting task')
             reply['status'] = TaskScheduleStatus.FAILED.value
+            reply['message'] = 'failed to resolve requested environment'
+            reply['error_class'] = 'environment_resolver'
         except ProcessInitializationError:
             self.__logger.info('Failed to initialize payload process. rejecting task')
             reply['status'] = TaskScheduleStatus.FAILED.value
-        except NotEnoughResources:
+            reply['message'] = 'failed to start the process'
+            reply['error_class'] = 'spawn'
+        except NotEnoughResources:  # currently not raised by worker
             self.__logger.warning('Not enough resources (this is unusual error - scheduler should know our resources). rejecting task')
             reply['status'] = TaskScheduleStatus.FAILED.value
+            reply['message'] = 'not enough resources'
+            reply['error_class'] = 'resources'
         except WorkerNotAvailable:
             self.__logger.warning('Got a task, but Worker is not available. Most probably is stopping right now')
             reply['status'] = TaskScheduleStatus.FAILED.value
+            reply['message'] = 'worker is stopping'
+            reply['error_class'] = 'stopping'
         except Exception as e:
             self.__logger.exception('no, cuz %s', e)
             reply['status'] = TaskScheduleStatus.FAILED.value
+            reply['message'] = f'error happened: {e}'
+            reply['error_class'] = 'exception'
 
         await client.send_message_as_json(reply)
 
     #
     # quit worker
     async def _command_quit(self, args: dict, client: CommandJsonMessageClient, original_message: Message):
         """
@@ -218,25 +229,25 @@
     async def ping(self) -> Tuple[WorkerPingReply, float]:
         await self.__client.send_command('ping', {})
 
         reply_message = await self.__client.receive_message()
         data_json = await reply_message.message_body_as_json()
         return WorkerPingReply(data_json['ps']), float(data_json['pv'])
 
-    async def give_task(self, task: invocationjob.InvocationJob, reply_address: Optional[AddressChain] = None) -> TaskScheduleStatus:
+    async def give_task(self, task: invocationjob.InvocationJob, reply_address: Optional[AddressChain] = None) -> Tuple[TaskScheduleStatus, str, str]:
         """
         if reply_address is not given - message source address will be used
         """
         await self.__client.send_command('task', {
             'task': (await task.serialize_async()).decode('latin1'),
             'reply_to': str(reply_address) if reply_address else None
         })
 
         reply = await (await self.__client.receive_message()).message_body_as_json()
-        return TaskScheduleStatus(reply['status'])
+        return TaskScheduleStatus(reply['status']), reply.get('error_class', ''), reply.get('message', '')
 
     async def quit_worker(self):
         await self.__client.send_command('quit', {})
 
         await self.__client.receive_message()
 
     async def cancel_task(self) -> None:
```

### Comparing `lifeblood-0.8.0/src/lifeblood/worker_pool_message_processor.py` & `lifeblood-0.9.0/src/lifeblood/worker_pool_message_processor.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/worker_pool_protocol.py` & `lifeblood-0.9.0/src/lifeblood/worker_pool_protocol.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/worker_runtime_pythonpath/lifeblood_connection.py` & `lifeblood-0.9.0/src/lifeblood/worker_runtime_pythonpath/lifeblood_connection.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood/worker_task_protocol.py` & `lifeblood-0.9.0/src/lifeblood/worker_task_protocol.py`

 * *Files identical despite different names*

### Comparing `lifeblood-0.8.0/src/lifeblood.egg-info/PKG-INFO` & `lifeblood-0.9.0/src/lifeblood.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: lifeblood
-Version: 0.8.0
+Version: 0.9.0
 Summary: LIFEBLOOD !!
 Home-page: https://github.com/pedohorse/lifeblood
 Author: XAPKOHHEH
 Project-URL: Bug Tracker, https://github.com/pedohorse/lifeblood/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles~=0.8
 Requires-Dist: aiosqlite~=0.17
 Requires-Dist: aiorwlock~=1.3
 Requires-Dist: lz4~=4.0
 Requires-Dist: psutil~=5.8
-Requires-Dist: pywin32==304; platform_system == "Windows"
+Requires-Dist: pywin32==306; platform_system == "Windows"
 Requires-Dist: semantic-version~=2.10
 Requires-Dist: toml~=0.10
 Requires-Dist: watchdog~=2.1
 
 [Documentation](https://pedohorse.github.io/lifeblood)
 
-|master|dev|
-|---|---|
-|[![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml/badge.svg?branch=master)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)<br>[![Tests windows](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml/badge.svg?branch=master)](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml)|[![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)<br>[![Tests windows](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/tests-win.yml)|
+| dev                                                                                                                                                                         |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| [![Tests](https://github.com/pedohorse/lifeblood/actions/workflows/tests.yml/badge.svg?branch=dev)](https://github.com/pedohorse/lifeblood/actions/workflows/python-app.yml)|
 
 ![](icon/lifeblood.svg)
 
 ## Lifeblood
 Lifeblood is a task/job management software package  
 currently it aims for smaller teams, farms or even individual setups, but with scaling  always in mind.
 
@@ -43,14 +43,16 @@
 processing graph.
 
 This system overview should be very familiar to anyone who saw at least one renderfarm.
 
 check [documentation here](https://pedohorse.github.io/lifeblood)  
 and also [video tutorials](https://pedohorse.github.io/lifeblood/tutorials.html)
 
+## UNDER DEVELOPMENT
+
 ### Features:
 - instantly and easily deployable
 - easy scaling in mind
 - dynamic slots, worker resources management
 - support for environment wrappers (allow you to integrate with existing packaging systems like rez)
 
 ### Features To Be Done:
@@ -66,9 +68,12 @@
 
 ## Installation
 
 There are multiple ways to get Lifeblood to try it out, refer to [installation section in the docs](https://pedohorse.github.io/lifeblood/installation.html#simplest-lifeblood-manager)
 
 In short - easiest way is to use [Lifeblood-Manager](https://github.com/pedohorse/lifeblood-manager/releases), as described in the docs
 
-## UNDER DEVELOPMENT
+## Links
 
+- [blog + support](https://www.patreon.com/xapkohheh)
+- [telegram support/discussion group](https://t.me/+v9klFGZcKVY2MjYy)
+- [documentation](https://pedohorse.github.io/lifeblood)
```

### Comparing `lifeblood-0.8.0/src/lifeblood.egg-info/SOURCES.txt` & `lifeblood-0.9.0/src/lifeblood.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/lifeblood/component_base.py
 src/lifeblood/config.py
 src/lifeblood/db_misc.py
 src/lifeblood/defaults.py
 src/lifeblood/enums.py
 src/lifeblood/environment_resolver.py
 src/lifeblood/exceptions.py
+src/lifeblood/expiring_collections.py
 src/lifeblood/filelock.py
 src/lifeblood/invocationjob.py
 src/lifeblood/launch.py
 src/lifeblood/local_notifier.py
 src/lifeblood/logging.py
 src/lifeblood/main_scheduler.py
 src/lifeblood/main_worker.py
```

