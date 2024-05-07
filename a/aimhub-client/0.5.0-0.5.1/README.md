# Comparing `tmp/aimhub_client-0.5.0.tar.gz` & `tmp/aimhub_client-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimhub_client-0.5.0.tar", last modified: Tue May  7 05:54:14 2024, max compression
+gzip compressed data, was "aimhub_client-0.5.1.tar", last modified: Tue May  7 07:24:52 2024, max compression
```

## Comparing `aimhub_client-0.5.0.tar` & `aimhub_client-0.5.1.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.578050 aimhub_client-0.5.0/
--rw-r--r--   0 github     (503) staff       (20)      116 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/MANIFEST.in
--rw-r--r--   0 github     (503) staff       (20)     1245 2024-05-07 05:54:14.577805 aimhub_client-0.5.0/PKG-INFO
--rw-r--r--   0 github     (503) staff       (20)       56 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/README.md
--rw-r--r--   0 github     (503) staff       (20)      887 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/pyproject.toml
--rw-r--r--   0 github     (503) staff       (20)       38 2024-05-07 05:54:14.578093 aimhub_client-0.5.0/setup.cfg
--rw-r--r--   0 github     (503) staff       (20)     8118 2024-05-07 05:54:07.000000 aimhub_client-0.5.0/setup.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.536211 aimhub_client-0.5.0/src/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.539976 aimhub_client-0.5.0/src/aim/
--rw-r--r--   0 github     (503) staff       (20)        5 2024-05-07 05:54:07.000000 aimhub_client-0.5.0/src/aim/VERSION
--rw-r--r--   0 github     (503) staff       (20)     1077 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      183 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/__version__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.540192 aimhub_client-0.5.0/src/aim/_core/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.540940 aimhub_client-0.5.0/src/aim/_core/callbacks/
--rw-r--r--   0 github     (503) staff       (20)      130 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1601 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/callbacks/caller.py
--rw-r--r--   0 github     (503) staff       (20)      478 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/callbacks/events.py
--rw-r--r--   0 github     (503) staff       (20)     1416 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/callbacks/helpers.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.541069 aimhub_client-0.5.0/src/aim/_core/cleanup/
--rw-r--r--   0 github     (503) staff       (20)     3579 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/cleanup/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1254 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/error_handling.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.547773 aimhub_client-0.5.0/src/aim/_core/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   459207 2024-05-07 05:54:12.000000 aimhub_client-0.5.0/src/aim/_core/storage/arrayview.cpp
--rw-r--r--   0 github     (503) staff       (20)      278 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/arrayview.pxd
--rw-r--r--   0 github     (503) staff       (20)     3051 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/arrayview.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.549176 aimhub_client-0.5.0/src/aim/_core/storage/artifacts/
--rw-r--r--   0 github     (503) staff       (20)      113 2024-03-14 17:16:59.000000 aimhub_client-0.5.0/src/aim/_core/storage/artifacts/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      956 2024-03-14 17:16:59.000000 aimhub_client-0.5.0/src/aim/_core/storage/artifacts/artifact_registry.py
--rw-r--r--   0 github     (503) staff       (20)      479 2024-03-14 17:16:59.000000 aimhub_client-0.5.0/src/aim/_core/storage/artifacts/artifact_storage.py
--rw-r--r--   0 github     (503) staff       (20)     2644 2024-03-14 17:16:59.000000 aimhub_client-0.5.0/src/aim/_core/storage/artifacts/s3_storage.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.549801 aimhub_client-0.5.0/src/aim/_core/storage/embedded/
--rw-r--r--   0 github     (503) staff       (20)      977 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/embedded/container.pxd
--rw-r--r--   0 github     (503) staff       (20)      346 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/embedded/containertreeview.pxd
--rw-r--r--   0 github     (503) staff       (20)      897 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/embedded/prefixcontainer.pxd
--rw-r--r--   0 github     (503) staff       (20)    18700 2024-02-26 11:30:34.000000 aimhub_client-0.5.0/src/aim/_core/storage/embedded/rockscontainer.pyx
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.551736 aimhub_client-0.5.0/src/aim/_core/storage/encoding/
--rw-r--r--   0 github     (503) staff       (20)   149132 2024-05-07 05:54:12.000000 aimhub_client-0.5.0/src/aim/_core/storage/encoding/__init__.cpp
--rw-r--r--   0 github     (503) staff       (20)      167 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/encoding/__init__.pxd
--rw-r--r--   0 github     (503) staff       (20)      107 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/encoding/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   377857 2024-05-07 05:54:12.000000 aimhub_client-0.5.0/src/aim/_core/storage/encoding/encoding.cpp
--rw-r--r--   0 github     (503) staff       (20)      507 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/encoding/encoding.pxd
--rw-r--r--   0 github     (503) staff       (20)     7372 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/encoding/encoding.pyx
--rw-r--r--   0 github     (503) staff       (20)   356424 2024-05-07 05:54:12.000000 aimhub_client-0.5.0/src/aim/_core/storage/encoding/encoding_native.cpp
--rw-r--r--   0 github     (503) staff       (20)      930 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/encoding/encoding_native.pxd
--rw-r--r--   0 github     (503) staff       (20)     5980 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/encoding/encoding_native.pyx
--rw-r--r--   0 github     (503) staff       (20)      337 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/env.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.553415 aimhub_client-0.5.0/src/aim/_core/storage/hashing/
--rw-r--r--   0 github     (503) staff       (20)   142007 2024-05-07 05:54:13.000000 aimhub_client-0.5.0/src/aim/_core/storage/hashing/__init__.cpp
--rw-r--r--   0 github     (503) staff       (20)       97 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/hashing/__init__.pxd
--rw-r--r--   0 github     (503) staff       (20)       56 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/hashing/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   206084 2024-05-07 05:54:13.000000 aimhub_client-0.5.0/src/aim/_core/storage/hashing/c_hash.cpp
--rw-r--r--   0 github     (503) staff       (20)      151 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/hashing/c_hash.pxd
--rw-r--r--   0 github     (503) staff       (20)      913 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/hashing/c_hash.pyi
--rw-r--r--   0 github     (503) staff       (20)     1083 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/hashing/c_hash.pyx
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.553537 aimhub_client-0.5.0/src/aim/_core/storage/hashing/hash/
--rw-r--r--   0 github     (503) staff       (20)     1412 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/hashing/hash/hash.h
--rw-r--r--   0 github     (503) staff       (20)   394363 2024-05-07 05:54:13.000000 aimhub_client-0.5.0/src/aim/_core/storage/hashing/hashing.cpp
--rw-r--r--   0 github     (503) staff       (20)     1021 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/hashing/hashing.pxd
--rw-r--r--   0 github     (503) staff       (20)     5580 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/hashing/hashing.py
--rw-r--r--   0 github     (503) staff       (20)   682318 2024-05-07 05:54:13.000000 aimhub_client-0.5.0/src/aim/_core/storage/inmemorytreeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      202 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/inmemorytreeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     4448 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/inmemorytreeview.py
--rw-r--r--   0 github     (503) staff       (20)     5533 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/locking.py
--rw-r--r--   0 github     (503) staff       (20)     2125 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/object.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.553696 aimhub_client-0.5.0/src/aim/_core/storage/reporter/
--rw-r--r--   0 github     (503) staff       (20)    31357 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/reporter/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   706227 2024-05-07 05:54:13.000000 aimhub_client-0.5.0/src/aim/_core/storage/treearrayview.cpp
--rw-r--r--   0 github     (503) staff       (20)      263 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/treearrayview.pxd
--rw-r--r--   0 github     (503) staff       (20)     3044 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/treearrayview.py
--rw-r--r--   0 github     (503) staff       (20)   728335 2024-05-07 05:54:13.000000 aimhub_client-0.5.0/src/aim/_core/storage/treeutils.cpp
--rw-r--r--   0 github     (503) staff       (20)     8419 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/treeutils.pyx
--rw-r--r--   0 github     (503) staff       (20)      713 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/treeutils_non_native.py
--rw-r--r--   0 github     (503) staff       (20)   541998 2024-05-07 05:54:13.000000 aimhub_client-0.5.0/src/aim/_core/storage/treeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      311 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/treeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     3133 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/treeview.py
--rw-r--r--   0 github     (503) staff       (20)      522 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/types.py
--rw-r--r--   0 github     (503) staff       (20)   817793 2024-05-07 05:54:13.000000 aimhub_client-0.5.0/src/aim/_core/storage/utils.cpp
--rw-r--r--   0 github     (503) staff       (20)      469 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/utils.pxd
--rw-r--r--   0 github     (503) staff       (20)     2102 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/storage/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.554460 aimhub_client-0.5.0/src/aim/_core/transport/
--rw-r--r--   0 github     (503) staff       (20)       27 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/transport/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    11501 2024-05-07 05:54:07.000000 aimhub_client-0.5.0/src/aim/_core/transport/client.py
--rw-r--r--   0 github     (503) staff       (20)     3718 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/transport/heartbeat_sender.py
--rw-r--r--   0 github     (503) staff       (20)     3038 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/transport/message_utils.py
--rw-r--r--   0 github     (503) staff       (20)     3684 2024-04-25 13:38:27.000000 aimhub_client-0.5.0/src/aim/_core/transport/request_queue.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.554770 aimhub_client-0.5.0/src/aim/_core/utils/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/utils/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      722 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_core/utils/deprecation.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.554920 aimhub_client-0.5.0/src/aim/_ext/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.555014 aimhub_client-0.5.0/src/aim/_ext/analytics/
--rw-r--r--   0 github     (503) staff       (20)     4755 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/analytics/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.555644 aimhub_client-0.5.0/src/aim/_ext/cli/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2355 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/cli.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.556162 aimhub_client-0.5.0/src/aim/_ext/cli/conatiners/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/conatiners/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     6940 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/conatiners/commands.py
--rw-r--r--   0 github     (503) staff       (20)      796 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/conatiners/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.556387 aimhub_client-0.5.0/src/aim/_ext/cli/convert/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/convert/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3010 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/convert/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.557553 aimhub_client-0.5.0/src/aim/_ext/cli/convert/processors/
--rw-r--r--   0 github     (503) staff       (20)      113 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/convert/processors/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5916 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/convert/processors/mlflow.py
--rw-r--r--   0 github     (503) staff       (20)    10374 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/convert/processors/tensorboard.py
--rw-r--r--   0 github     (503) staff       (20)     6820 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/convert/processors/wandb.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.557835 aimhub_client-0.5.0/src/aim/_ext/cli/login/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/login/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      865 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/login/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.558307 aimhub_client-0.5.0/src/aim/_ext/cli/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     4088 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/storage/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.558591 aimhub_client-0.5.0/src/aim/_ext/cli/telemetry/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/telemetry/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      305 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/telemetry/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.559142 aimhub_client-0.5.0/src/aim/_ext/cli/upload/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/upload/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1831 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/upload/commands.py
--rw-r--r--   0 github     (503) staff       (20)      405 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/upload/utils.py
--rw-r--r--   0 github     (503) staff       (20)     3699 2024-05-07 05:54:07.000000 aimhub_client-0.5.0/src/aim/_ext/cli/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.559610 aimhub_client-0.5.0/src/aim/_ext/cli/version/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/version/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      223 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/version/commands.py
--rw-r--r--   0 github     (503) staff       (20)     9969 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/cli/watcher_cli.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.560112 aimhub_client-0.5.0/src/aim/_ext/notebook/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notebook/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2615 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notebook/manager.py
--rw-r--r--   0 github     (503) staff       (20)     7169 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notebook/notebook.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.562170 aimhub_client-0.5.0/src/aim/_ext/notifier/
--rw-r--r--   0 github     (503) staff       (20)      593 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notifier/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      305 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notifier/base_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1859 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notifier/config.py
--rw-r--r--   0 github     (503) staff       (20)      361 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notifier/config_default.json
--rw-r--r--   0 github     (503) staff       (20)       70 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notifier/config_empty.json
--rw-r--r--   0 github     (503) staff       (20)      523 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notifier/logging_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1429 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notifier/notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1162 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notifier/notifier_builder.py
--rw-r--r--   0 github     (503) staff       (20)      525 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notifier/slack_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1035 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notifier/utils.py
--rw-r--r--   0 github     (503) staff       (20)      863 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/notifier/workplace_notifier.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.563920 aimhub_client-0.5.0/src/aim/_ext/system_info/
--rw-r--r--   0 github     (503) staff       (20)      152 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/system_info/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      100 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/system_info/configs.py
--rw-r--r--   0 github     (503) staff       (20)   148706 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/system_info/pynvml.py
--rw-r--r--   0 github     (503) staff       (20)     7800 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/system_info/resource_tracker.py
--rw-r--r--   0 github     (503) staff       (20)     6670 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/system_info/stat.py
--rw-r--r--   0 github     (503) staff       (20)     2246 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_ext/system_info/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.565581 aimhub_client-0.5.0/src/aim/_sdk/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.567290 aimhub_client-0.5.0/src/aim/_sdk/base/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/base/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    14815 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/base/collections.py
--rw-r--r--   0 github     (503) staff       (20)    21089 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/base/container.py
--rw-r--r--   0 github     (503) staff       (20)     1837 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/base/context.py
--rw-r--r--   0 github     (503) staff       (20)    12464 2024-04-25 13:38:27.000000 aimhub_client-0.5.0/src/aim/_sdk/base/property.py
--rw-r--r--   0 github     (503) staff       (20)     2261 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/base/record.py
--rw-r--r--   0 github     (503) staff       (20)    25484 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/base/repo.py
--rw-r--r--   0 github     (503) staff       (20)    20689 2024-02-15 13:42:09.000000 aimhub_client-0.5.0/src/aim/_sdk/base/sequence.py
--rw-r--r--   0 github     (503) staff       (20)      965 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/configs.py
--rw-r--r--   0 github     (503) staff       (20)      561 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/exceptions.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.571960 aimhub_client-0.5.0/src/aim/_sdk/integrations/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1936 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/acme.py
--rw-r--r--   0 github     (503) staff       (20)     2759 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/catboost.py
--rw-r--r--   0 github     (503) staff       (20)     4818 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/fastai.py
--rw-r--r--   0 github     (503) staff       (20)     5048 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/hugging_face.py
--rw-r--r--   0 github     (503) staff       (20)     1819 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/keras.py
--rw-r--r--   0 github     (503) staff       (20)     1128 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/keras_mixins.py
--rw-r--r--   0 github     (503) staff       (20)     2162 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/keras_tuner.py
--rw-r--r--   0 github     (503) staff       (20)     2672 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/lightgbm.py
--rw-r--r--   0 github     (503) staff       (20)     7570 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/mxnet.py
--rw-r--r--   0 github     (503) staff       (20)     6539 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/optuna.py
--rw-r--r--   0 github     (503) staff       (20)     2822 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/paddle.py
--rw-r--r--   0 github     (503) staff       (20)     2289 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/prophet.py
--rw-r--r--   0 github     (503) staff       (20)     2458 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/pytorch.py
--rw-r--r--   0 github     (503) staff       (20)     8295 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/pytorch_ignite.py
--rw-r--r--   0 github     (503) staff       (20)     5235 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/pytorch_lightning.py
--rw-r--r--   0 github     (503) staff       (20)     3860 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/sb3.py
--rw-r--r--   0 github     (503) staff       (20)     1840 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/tensorflow.py
--rw-r--r--   0 github     (503) staff       (20)     2324 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/_sdk/integrations/xgboost.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.572689 aimhub_client-0.5.0/src/aim/_sdk/interfaces/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/interfaces/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1808 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/interfaces/container.py
--rw-r--r--   0 github     (503) staff       (20)     2411 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/interfaces/sequence.py
--rw-r--r--   0 github     (503) staff       (20)      706 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/interfaces/storage_engine.py
--rw-r--r--   0 github     (503) staff       (20)     3397 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/num_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.573558 aimhub_client-0.5.0/src/aim/_sdk/query/
--rw-r--r--   0 github     (503) staff       (20)      154 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/query/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     4823 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/query/analyzer.py
--rw-r--r--   0 github     (503) staff       (20)    11648 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/query/proxy.py
--rw-r--r--   0 github     (503) staff       (20)     4157 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/query/query.py
--rw-r--r--   0 github     (503) staff       (20)     4718 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/query/query_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.573749 aimhub_client-0.5.0/src/aim/_sdk/remote_storage/
--rw-r--r--   0 github     (503) staff       (20)    16343 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/remote_storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     4277 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/type_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.575930 aimhub_client-0.5.0/src/aim/_sdk/types/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/types/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1354 2024-03-14 17:16:59.000000 aimhub_client-0.5.0/src/aim/_sdk/types/artifact.py
--rw-r--r--   0 github     (503) staff       (20)     3341 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/types/audio.py
--rw-r--r--   0 github     (503) staff       (20)     4290 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/types/distribution.py
--rw-r--r--   0 github     (503) staff       (20)     3097 2024-04-25 13:38:27.000000 aimhub_client-0.5.0/src/aim/_sdk/types/experiment.py
--rw-r--r--   0 github     (503) staff       (20)     5307 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/types/figures.py
--rw-r--r--   0 github     (503) staff       (20)    10142 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/types/image.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.576234 aimhub_client-0.5.0/src/aim/_sdk/types/io/
--rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/types/io/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    21094 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/types/io/wavfile.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.576560 aimhub_client-0.5.0/src/aim/_sdk/types/logging/
--rw-r--r--   0 github     (503) staff       (20)     1658 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/types/logging/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2708 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/types/metric.py
--rw-r--r--   0 github     (503) staff       (20)    10895 2024-04-25 13:38:27.000000 aimhub_client-0.5.0/src/aim/_sdk/types/run.py
--rw-r--r--   0 github     (503) staff       (20)     3131 2024-04-25 13:38:27.000000 aimhub_client-0.5.0/src/aim/_sdk/types/tag.py
--rw-r--r--   0 github     (503) staff       (20)      779 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/types/text.py
--rw-r--r--   0 github     (503) staff       (20)     1489 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/uri_service.py
--rw-r--r--   0 github     (503) staff       (20)     3320 2024-02-13 12:24:52.000000 aimhub_client-0.5.0/src/aim/_sdk/utils.py
--rw-r--r--   0 github     (503) staff       (20)      105 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/acme.py
--rw-r--r--   0 github     (503) staff       (20)      101 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/catboost.py
--rw-r--r--   0 github     (503) staff       (20)       97 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/fastai.py
--rw-r--r--   0 github     (503) staff       (20)      110 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/hugging_face.py
--rw-r--r--   0 github     (503) staff       (20)      108 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/keras.py
--rw-r--r--   0 github     (503) staff       (20)      108 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/keras_tuner.py
--rw-r--r--   0 github     (503) staff       (20)      103 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/lightgbm.py
--rw-r--r--   0 github     (503) staff       (20)      102 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/mxnet.py
--rw-r--r--   0 github     (503) staff       (20)      103 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/optuna.py
--rw-r--r--   0 github     (503) staff       (20)      104 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/paddle.py
--rw-r--r--   0 github     (503) staff       (20)       98 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/prophet.py
--rw-r--r--   0 github     (503) staff       (20)      120 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/pytorch.py
--rw-r--r--   0 github     (503) staff       (20)      112 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/pytorch_ignite.py
--rw-r--r--   0 github     (503) staff       (20)      118 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/pytorch_lightning.py
--rw-r--r--   0 github     (503) staff       (20)       92 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/sb3.py
--rw-r--r--   0 github     (503) staff       (20)      124 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/tensorflow.py
--rw-r--r--   0 github     (503) staff       (20)      101 2024-02-19 07:16:26.000000 aimhub_client-0.5.0/src/aim/xgboost.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 05:54:14.577492 aimhub_client-0.5.0/src/aimhub_client.egg-info/
--rw-r--r--   0 github     (503) staff       (20)     1245 2024-05-07 05:54:14.000000 aimhub_client-0.5.0/src/aimhub_client.egg-info/PKG-INFO
--rw-r--r--   0 github     (503) staff       (20)     6937 2024-05-07 05:54:14.000000 aimhub_client-0.5.0/src/aimhub_client.egg-info/SOURCES.txt
--rw-r--r--   0 github     (503) staff       (20)        1 2024-05-07 05:54:14.000000 aimhub_client-0.5.0/src/aimhub_client.egg-info/dependency_links.txt
--rw-r--r--   0 github     (503) staff       (20)       57 2024-05-07 05:54:14.000000 aimhub_client-0.5.0/src/aimhub_client.egg-info/entry_points.txt
--rw-r--r--   0 github     (503) staff       (20)      264 2024-05-07 05:54:14.000000 aimhub_client-0.5.0/src/aimhub_client.egg-info/requires.txt
--rw-r--r--   0 github     (503) staff       (20)        4 2024-05-07 05:54:14.000000 aimhub_client-0.5.0/src/aimhub_client.egg-info/top_level.txt
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.903679 aimhub_client-0.5.1/
+-rw-r--r--   0 github     (503) staff       (20)      116 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/MANIFEST.in
+-rw-r--r--   0 github     (503) staff       (20)     1245 2024-05-07 07:24:52.903417 aimhub_client-0.5.1/PKG-INFO
+-rw-r--r--   0 github     (503) staff       (20)       56 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/README.md
+-rw-r--r--   0 github     (503) staff       (20)      887 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/pyproject.toml
+-rw-r--r--   0 github     (503) staff       (20)       38 2024-05-07 07:24:52.903717 aimhub_client-0.5.1/setup.cfg
+-rw-r--r--   0 github     (503) staff       (20)     8118 2024-05-07 05:54:07.000000 aimhub_client-0.5.1/setup.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.867178 aimhub_client-0.5.1/src/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.871068 aimhub_client-0.5.1/src/aim/
+-rw-r--r--   0 github     (503) staff       (20)        5 2024-05-07 07:24:45.000000 aimhub_client-0.5.1/src/aim/VERSION
+-rw-r--r--   0 github     (503) staff       (20)     1077 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      183 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/__version__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.871297 aimhub_client-0.5.1/src/aim/_core/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.872039 aimhub_client-0.5.1/src/aim/_core/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)      130 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1601 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/callbacks/caller.py
+-rw-r--r--   0 github     (503) staff       (20)      478 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/callbacks/events.py
+-rw-r--r--   0 github     (503) staff       (20)     1416 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/callbacks/helpers.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.872167 aimhub_client-0.5.1/src/aim/_core/cleanup/
+-rw-r--r--   0 github     (503) staff       (20)     3579 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/cleanup/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1254 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/error_handling.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.878535 aimhub_client-0.5.1/src/aim/_core/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   459207 2024-05-07 07:24:51.000000 aimhub_client-0.5.1/src/aim/_core/storage/arrayview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      278 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/arrayview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     3051 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/arrayview.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.879939 aimhub_client-0.5.1/src/aim/_core/storage/artifacts/
+-rw-r--r--   0 github     (503) staff       (20)      113 2024-03-14 17:16:59.000000 aimhub_client-0.5.1/src/aim/_core/storage/artifacts/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      956 2024-03-14 17:16:59.000000 aimhub_client-0.5.1/src/aim/_core/storage/artifacts/artifact_registry.py
+-rw-r--r--   0 github     (503) staff       (20)      479 2024-03-14 17:16:59.000000 aimhub_client-0.5.1/src/aim/_core/storage/artifacts/artifact_storage.py
+-rw-r--r--   0 github     (503) staff       (20)     2644 2024-03-14 17:16:59.000000 aimhub_client-0.5.1/src/aim/_core/storage/artifacts/s3_storage.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.880511 aimhub_client-0.5.1/src/aim/_core/storage/embedded/
+-rw-r--r--   0 github     (503) staff       (20)      977 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/embedded/container.pxd
+-rw-r--r--   0 github     (503) staff       (20)      346 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/embedded/containertreeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)      897 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/embedded/prefixcontainer.pxd
+-rw-r--r--   0 github     (503) staff       (20)    18700 2024-02-26 11:30:34.000000 aimhub_client-0.5.1/src/aim/_core/storage/embedded/rockscontainer.pyx
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.882494 aimhub_client-0.5.1/src/aim/_core/storage/encoding/
+-rw-r--r--   0 github     (503) staff       (20)   149132 2024-05-07 07:24:51.000000 aimhub_client-0.5.1/src/aim/_core/storage/encoding/__init__.cpp
+-rw-r--r--   0 github     (503) staff       (20)      167 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/encoding/__init__.pxd
+-rw-r--r--   0 github     (503) staff       (20)      107 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/encoding/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   377857 2024-05-07 07:24:51.000000 aimhub_client-0.5.1/src/aim/_core/storage/encoding/encoding.cpp
+-rw-r--r--   0 github     (503) staff       (20)      507 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/encoding/encoding.pxd
+-rw-r--r--   0 github     (503) staff       (20)     7372 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/encoding/encoding.pyx
+-rw-r--r--   0 github     (503) staff       (20)   356424 2024-05-07 07:24:51.000000 aimhub_client-0.5.1/src/aim/_core/storage/encoding/encoding_native.cpp
+-rw-r--r--   0 github     (503) staff       (20)      930 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/encoding/encoding_native.pxd
+-rw-r--r--   0 github     (503) staff       (20)     5980 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/encoding/encoding_native.pyx
+-rw-r--r--   0 github     (503) staff       (20)      337 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/env.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.884086 aimhub_client-0.5.1/src/aim/_core/storage/hashing/
+-rw-r--r--   0 github     (503) staff       (20)   142007 2024-05-07 07:24:51.000000 aimhub_client-0.5.1/src/aim/_core/storage/hashing/__init__.cpp
+-rw-r--r--   0 github     (503) staff       (20)       97 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/hashing/__init__.pxd
+-rw-r--r--   0 github     (503) staff       (20)       56 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/hashing/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   206084 2024-05-07 07:24:51.000000 aimhub_client-0.5.1/src/aim/_core/storage/hashing/c_hash.cpp
+-rw-r--r--   0 github     (503) staff       (20)      151 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/hashing/c_hash.pxd
+-rw-r--r--   0 github     (503) staff       (20)      913 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/hashing/c_hash.pyi
+-rw-r--r--   0 github     (503) staff       (20)     1083 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/hashing/c_hash.pyx
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.884208 aimhub_client-0.5.1/src/aim/_core/storage/hashing/hash/
+-rw-r--r--   0 github     (503) staff       (20)     1412 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/hashing/hash/hash.h
+-rw-r--r--   0 github     (503) staff       (20)   394363 2024-05-07 07:24:51.000000 aimhub_client-0.5.1/src/aim/_core/storage/hashing/hashing.cpp
+-rw-r--r--   0 github     (503) staff       (20)     1021 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/hashing/hashing.pxd
+-rw-r--r--   0 github     (503) staff       (20)     5580 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/hashing/hashing.py
+-rw-r--r--   0 github     (503) staff       (20)   682318 2024-05-07 07:24:51.000000 aimhub_client-0.5.1/src/aim/_core/storage/inmemorytreeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      202 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/inmemorytreeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     4448 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/inmemorytreeview.py
+-rw-r--r--   0 github     (503) staff       (20)     5533 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/locking.py
+-rw-r--r--   0 github     (503) staff       (20)     2125 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/object.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.884350 aimhub_client-0.5.1/src/aim/_core/storage/reporter/
+-rw-r--r--   0 github     (503) staff       (20)    31357 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/reporter/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   706227 2024-05-07 07:24:51.000000 aimhub_client-0.5.1/src/aim/_core/storage/treearrayview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      263 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/treearrayview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     3044 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/treearrayview.py
+-rw-r--r--   0 github     (503) staff       (20)   728335 2024-05-07 07:24:51.000000 aimhub_client-0.5.1/src/aim/_core/storage/treeutils.cpp
+-rw-r--r--   0 github     (503) staff       (20)     8419 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/treeutils.pyx
+-rw-r--r--   0 github     (503) staff       (20)      713 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/treeutils_non_native.py
+-rw-r--r--   0 github     (503) staff       (20)   541998 2024-05-07 07:24:51.000000 aimhub_client-0.5.1/src/aim/_core/storage/treeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      311 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/treeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     3133 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/treeview.py
+-rw-r--r--   0 github     (503) staff       (20)      522 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/types.py
+-rw-r--r--   0 github     (503) staff       (20)   817793 2024-05-07 07:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/utils.cpp
+-rw-r--r--   0 github     (503) staff       (20)      469 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/utils.pxd
+-rw-r--r--   0 github     (503) staff       (20)     2102 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/storage/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.885263 aimhub_client-0.5.1/src/aim/_core/transport/
+-rw-r--r--   0 github     (503) staff       (20)       27 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/transport/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    11501 2024-05-07 05:54:07.000000 aimhub_client-0.5.1/src/aim/_core/transport/client.py
+-rw-r--r--   0 github     (503) staff       (20)     3718 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/transport/heartbeat_sender.py
+-rw-r--r--   0 github     (503) staff       (20)     3038 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/transport/message_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     3684 2024-04-25 13:38:27.000000 aimhub_client-0.5.1/src/aim/_core/transport/request_queue.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.885693 aimhub_client-0.5.1/src/aim/_core/utils/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/utils/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      722 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_core/utils/deprecation.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.885848 aimhub_client-0.5.1/src/aim/_ext/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.885947 aimhub_client-0.5.1/src/aim/_ext/analytics/
+-rw-r--r--   0 github     (503) staff       (20)     4755 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/analytics/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.886492 aimhub_client-0.5.1/src/aim/_ext/cli/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2355 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/cli.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.886952 aimhub_client-0.5.1/src/aim/_ext/cli/conatiners/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/conatiners/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     6940 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/conatiners/commands.py
+-rw-r--r--   0 github     (503) staff       (20)      796 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/conatiners/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.887178 aimhub_client-0.5.1/src/aim/_ext/cli/convert/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/convert/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3010 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/convert/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.887836 aimhub_client-0.5.1/src/aim/_ext/cli/convert/processors/
+-rw-r--r--   0 github     (503) staff       (20)      113 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/convert/processors/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5916 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/convert/processors/mlflow.py
+-rw-r--r--   0 github     (503) staff       (20)    10374 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/convert/processors/tensorboard.py
+-rw-r--r--   0 github     (503) staff       (20)     6820 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/convert/processors/wandb.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.888064 aimhub_client-0.5.1/src/aim/_ext/cli/login/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/login/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      865 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/login/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.888289 aimhub_client-0.5.1/src/aim/_ext/cli/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     4088 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/storage/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.888511 aimhub_client-0.5.1/src/aim/_ext/cli/telemetry/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/telemetry/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      305 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/telemetry/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.888940 aimhub_client-0.5.1/src/aim/_ext/cli/upload/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/upload/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1831 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/upload/commands.py
+-rw-r--r--   0 github     (503) staff       (20)      405 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/upload/utils.py
+-rw-r--r--   0 github     (503) staff       (20)     3699 2024-05-07 05:54:07.000000 aimhub_client-0.5.1/src/aim/_ext/cli/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.889172 aimhub_client-0.5.1/src/aim/_ext/cli/version/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/version/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      223 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/version/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     9969 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/cli/watcher_cli.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.889581 aimhub_client-0.5.1/src/aim/_ext/notebook/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notebook/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2615 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notebook/manager.py
+-rw-r--r--   0 github     (503) staff       (20)     7169 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notebook/notebook.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.891356 aimhub_client-0.5.1/src/aim/_ext/notifier/
+-rw-r--r--   0 github     (503) staff       (20)      593 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notifier/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      305 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notifier/base_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1859 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notifier/config.py
+-rw-r--r--   0 github     (503) staff       (20)      361 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notifier/config_default.json
+-rw-r--r--   0 github     (503) staff       (20)       70 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notifier/config_empty.json
+-rw-r--r--   0 github     (503) staff       (20)      523 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notifier/logging_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1429 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notifier/notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1162 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notifier/notifier_builder.py
+-rw-r--r--   0 github     (503) staff       (20)      525 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notifier/slack_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1035 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notifier/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      863 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/notifier/workplace_notifier.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.892740 aimhub_client-0.5.1/src/aim/_ext/system_info/
+-rw-r--r--   0 github     (503) staff       (20)      152 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/system_info/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      100 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/system_info/configs.py
+-rw-r--r--   0 github     (503) staff       (20)   148706 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/system_info/pynvml.py
+-rw-r--r--   0 github     (503) staff       (20)     7800 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/system_info/resource_tracker.py
+-rw-r--r--   0 github     (503) staff       (20)     6670 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/system_info/stat.py
+-rw-r--r--   0 github     (503) staff       (20)     2246 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_ext/system_info/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.893968 aimhub_client-0.5.1/src/aim/_sdk/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.895539 aimhub_client-0.5.1/src/aim/_sdk/base/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/base/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    14815 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/base/collections.py
+-rw-r--r--   0 github     (503) staff       (20)    21089 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/base/container.py
+-rw-r--r--   0 github     (503) staff       (20)     1837 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/base/context.py
+-rw-r--r--   0 github     (503) staff       (20)    12464 2024-04-25 13:38:27.000000 aimhub_client-0.5.1/src/aim/_sdk/base/property.py
+-rw-r--r--   0 github     (503) staff       (20)     2261 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/base/record.py
+-rw-r--r--   0 github     (503) staff       (20)    25484 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/base/repo.py
+-rw-r--r--   0 github     (503) staff       (20)    20689 2024-02-15 13:42:09.000000 aimhub_client-0.5.1/src/aim/_sdk/base/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      965 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/configs.py
+-rw-r--r--   0 github     (503) staff       (20)      561 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/exceptions.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.898444 aimhub_client-0.5.1/src/aim/_sdk/integrations/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1936 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/acme.py
+-rw-r--r--   0 github     (503) staff       (20)     2759 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/catboost.py
+-rw-r--r--   0 github     (503) staff       (20)     4818 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/fastai.py
+-rw-r--r--   0 github     (503) staff       (20)     5048 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/hugging_face.py
+-rw-r--r--   0 github     (503) staff       (20)     1819 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/keras.py
+-rw-r--r--   0 github     (503) staff       (20)     1128 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/keras_mixins.py
+-rw-r--r--   0 github     (503) staff       (20)     2162 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/keras_tuner.py
+-rw-r--r--   0 github     (503) staff       (20)     2672 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/lightgbm.py
+-rw-r--r--   0 github     (503) staff       (20)     7570 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/mxnet.py
+-rw-r--r--   0 github     (503) staff       (20)     6539 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/optuna.py
+-rw-r--r--   0 github     (503) staff       (20)     2822 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/paddle.py
+-rw-r--r--   0 github     (503) staff       (20)     2289 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/prophet.py
+-rw-r--r--   0 github     (503) staff       (20)     2458 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/pytorch.py
+-rw-r--r--   0 github     (503) staff       (20)     8295 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/pytorch_ignite.py
+-rw-r--r--   0 github     (503) staff       (20)     5235 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/pytorch_lightning.py
+-rw-r--r--   0 github     (503) staff       (20)     3860 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/sb3.py
+-rw-r--r--   0 github     (503) staff       (20)     1840 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/tensorflow.py
+-rw-r--r--   0 github     (503) staff       (20)     2324 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/_sdk/integrations/xgboost.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.899005 aimhub_client-0.5.1/src/aim/_sdk/interfaces/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/interfaces/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1808 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/interfaces/container.py
+-rw-r--r--   0 github     (503) staff       (20)     2411 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/interfaces/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      706 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/interfaces/storage_engine.py
+-rw-r--r--   0 github     (503) staff       (20)     3397 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/num_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.899670 aimhub_client-0.5.1/src/aim/_sdk/query/
+-rw-r--r--   0 github     (503) staff       (20)      154 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/query/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     4823 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/query/analyzer.py
+-rw-r--r--   0 github     (503) staff       (20)    11648 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/query/proxy.py
+-rw-r--r--   0 github     (503) staff       (20)     4157 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/query/query.py
+-rw-r--r--   0 github     (503) staff       (20)     4718 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/query/query_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.899806 aimhub_client-0.5.1/src/aim/_sdk/remote_storage/
+-rw-r--r--   0 github     (503) staff       (20)    16343 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/remote_storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     4277 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/type_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.901730 aimhub_client-0.5.1/src/aim/_sdk/types/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/types/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1354 2024-03-14 17:16:59.000000 aimhub_client-0.5.1/src/aim/_sdk/types/artifact.py
+-rw-r--r--   0 github     (503) staff       (20)     3341 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/types/audio.py
+-rw-r--r--   0 github     (503) staff       (20)     4290 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/types/distribution.py
+-rw-r--r--   0 github     (503) staff       (20)     3097 2024-04-25 13:38:27.000000 aimhub_client-0.5.1/src/aim/_sdk/types/experiment.py
+-rw-r--r--   0 github     (503) staff       (20)     5307 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/types/figures.py
+-rw-r--r--   0 github     (503) staff       (20)    10142 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/types/image.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.901969 aimhub_client-0.5.1/src/aim/_sdk/types/io/
+-rw-r--r--   0 github     (503) staff       (20)        0 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/types/io/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    21094 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/types/io/wavfile.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.902183 aimhub_client-0.5.1/src/aim/_sdk/types/logging/
+-rw-r--r--   0 github     (503) staff       (20)     1658 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/types/logging/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2708 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/types/metric.py
+-rw-r--r--   0 github     (503) staff       (20)    10895 2024-04-25 13:38:27.000000 aimhub_client-0.5.1/src/aim/_sdk/types/run.py
+-rw-r--r--   0 github     (503) staff       (20)     3131 2024-04-25 13:38:27.000000 aimhub_client-0.5.1/src/aim/_sdk/types/tag.py
+-rw-r--r--   0 github     (503) staff       (20)      779 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/types/text.py
+-rw-r--r--   0 github     (503) staff       (20)     1489 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/uri_service.py
+-rw-r--r--   0 github     (503) staff       (20)     3320 2024-02-13 12:24:52.000000 aimhub_client-0.5.1/src/aim/_sdk/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      105 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/acme.py
+-rw-r--r--   0 github     (503) staff       (20)      101 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/catboost.py
+-rw-r--r--   0 github     (503) staff       (20)       97 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/fastai.py
+-rw-r--r--   0 github     (503) staff       (20)      110 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/hugging_face.py
+-rw-r--r--   0 github     (503) staff       (20)      108 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/keras.py
+-rw-r--r--   0 github     (503) staff       (20)      108 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/keras_tuner.py
+-rw-r--r--   0 github     (503) staff       (20)      103 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/lightgbm.py
+-rw-r--r--   0 github     (503) staff       (20)      102 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/mxnet.py
+-rw-r--r--   0 github     (503) staff       (20)      103 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/optuna.py
+-rw-r--r--   0 github     (503) staff       (20)      104 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/paddle.py
+-rw-r--r--   0 github     (503) staff       (20)       98 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/prophet.py
+-rw-r--r--   0 github     (503) staff       (20)      120 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/pytorch.py
+-rw-r--r--   0 github     (503) staff       (20)      112 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/pytorch_ignite.py
+-rw-r--r--   0 github     (503) staff       (20)      118 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/pytorch_lightning.py
+-rw-r--r--   0 github     (503) staff       (20)       92 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/sb3.py
+-rw-r--r--   0 github     (503) staff       (20)      124 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/tensorflow.py
+-rw-r--r--   0 github     (503) staff       (20)      101 2024-02-19 07:16:26.000000 aimhub_client-0.5.1/src/aim/xgboost.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2024-05-07 07:24:52.903111 aimhub_client-0.5.1/src/aimhub_client.egg-info/
+-rw-r--r--   0 github     (503) staff       (20)     1245 2024-05-07 07:24:52.000000 aimhub_client-0.5.1/src/aimhub_client.egg-info/PKG-INFO
+-rw-r--r--   0 github     (503) staff       (20)     6937 2024-05-07 07:24:52.000000 aimhub_client-0.5.1/src/aimhub_client.egg-info/SOURCES.txt
+-rw-r--r--   0 github     (503) staff       (20)        1 2024-05-07 07:24:52.000000 aimhub_client-0.5.1/src/aimhub_client.egg-info/dependency_links.txt
+-rw-r--r--   0 github     (503) staff       (20)       57 2024-05-07 07:24:52.000000 aimhub_client-0.5.1/src/aimhub_client.egg-info/entry_points.txt
+-rw-r--r--   0 github     (503) staff       (20)      264 2024-05-07 07:24:52.000000 aimhub_client-0.5.1/src/aimhub_client.egg-info/requires.txt
+-rw-r--r--   0 github     (503) staff       (20)        4 2024-05-07 07:24:52.000000 aimhub_client-0.5.1/src/aimhub_client.egg-info/top_level.txt
```

### Comparing `aimhub_client-0.5.0/PKG-INFO` & `aimhub_client-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimhub-client
-Version: 0.5.0
+Version: 0.5.1
 Summary: A super-easy way to record, search and compare AI experiments.
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `aimhub_client-0.5.0/pyproject.toml` & `aimhub_client-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/setup.py` & `aimhub_client-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/__init__.py` & `aimhub_client-0.5.1/src/aim/__init__.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/callbacks/caller.py` & `aimhub_client-0.5.1/src/aim/_core/callbacks/caller.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/callbacks/helpers.py` & `aimhub_client-0.5.1/src/aim/_core/callbacks/helpers.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/cleanup/__init__.py` & `aimhub_client-0.5.1/src/aim/_core/cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/error_handling.py` & `aimhub_client-0.5.1/src/aim/_core/error_handling.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/arrayview.cpp` & `aimhub_client-0.5.1/src/aim/_core/storage/arrayview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.arrayview",
         "sources": [
             "src/aim/_core/storage/arrayview.py"
         ]
     },
     "module_name": "aim._core.storage.arrayview"
```

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/arrayview.py` & `aimhub_client-0.5.1/src/aim/_core/storage/arrayview.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/artifacts/artifact_registry.py` & `aimhub_client-0.5.1/src/aim/_core/storage/artifacts/artifact_registry.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/artifacts/s3_storage.py` & `aimhub_client-0.5.1/src/aim/_core/storage/artifacts/s3_storage.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/embedded/container.pxd` & `aimhub_client-0.5.1/src/aim/_core/storage/embedded/container.pxd`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/embedded/prefixcontainer.pxd` & `aimhub_client-0.5.1/src/aim/_core/storage/embedded/prefixcontainer.pxd`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/embedded/rockscontainer.pyx` & `aimhub_client-0.5.1/src/aim/_core/storage/embedded/rockscontainer.pyx`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/encoding/__init__.cpp` & `aimhub_client-0.5.1/src/aim/_core/storage/encoding/__init__.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.encoding",
         "sources": [
             "src/aim/_core/storage/encoding/__init__.py"
         ]
     },
     "module_name": "aim._core.storage.encoding"
```

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/encoding/encoding.cpp` & `aimhub_client-0.5.1/src/aim/_core/storage/encoding/encoding.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.encoding.encoding",
         "sources": [
             "src/aim/_core/storage/encoding/encoding.pyx"
         ]
     },
     "module_name": "aim._core.storage.encoding.encoding"
```

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/encoding/encoding.pyx` & `aimhub_client-0.5.1/src/aim/_core/storage/encoding/encoding.pyx`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/encoding/encoding_native.cpp` & `aimhub_client-0.5.1/src/aim/_core/storage/encoding/encoding_native.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.encoding.encoding_native",
         "sources": [
             "src/aim/_core/storage/encoding/encoding_native.pyx"
         ]
     },
     "module_name": "aim._core.storage.encoding.encoding_native"
```

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/encoding/encoding_native.pxd` & `aimhub_client-0.5.1/src/aim/_core/storage/encoding/encoding_native.pxd`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/encoding/encoding_native.pyx` & `aimhub_client-0.5.1/src/aim/_core/storage/encoding/encoding_native.pyx`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/hashing/__init__.cpp` & `aimhub_client-0.5.1/src/aim/_core/storage/hashing/__init__.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "src/aim/_core/storage/hashing",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.hashing",
         "sources": [
             "src/aim/_core/storage/hashing/__init__.py"
         ]
     },
     "module_name": "aim._core.storage.hashing"
```

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/hashing/c_hash.cpp` & `aimhub_client-0.5.1/src/aim/_core/storage/hashing/c_hash.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,23 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "src/aim/_core/storage/hashing",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "language_level": "3",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.hashing.c_hash",
         "sources": [
             "src/aim/_core/storage/hashing/c_hash.pyx"
         ]
     },
     "module_name": "aim._core.storage.hashing.c_hash"
```

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/hashing/c_hash.pyi` & `aimhub_client-0.5.1/src/aim/_core/storage/hashing/c_hash.pyi`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/hashing/c_hash.pyx` & `aimhub_client-0.5.1/src/aim/_core/storage/hashing/c_hash.pyx`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/hashing/hash/hash.h` & `aimhub_client-0.5.1/src/aim/_core/storage/hashing/hash/hash.h`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/hashing/hashing.cpp` & `aimhub_client-0.5.1/src/aim/_core/storage/hashing/hashing.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "src/aim/_core/storage/hashing",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.hashing.hashing",
         "sources": [
             "src/aim/_core/storage/hashing/hashing.py"
         ]
     },
     "module_name": "aim._core.storage.hashing.hashing"
```

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/hashing/hashing.pxd` & `aimhub_client-0.5.1/src/aim/_core/storage/hashing/hashing.pxd`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/hashing/hashing.py` & `aimhub_client-0.5.1/src/aim/_core/storage/hashing/hashing.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/inmemorytreeview.cpp` & `aimhub_client-0.5.1/src/aim/_core/storage/inmemorytreeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.inmemorytreeview",
         "sources": [
             "src/aim/_core/storage/inmemorytreeview.py"
         ]
     },
     "module_name": "aim._core.storage.inmemorytreeview"
```

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/inmemorytreeview.py` & `aimhub_client-0.5.1/src/aim/_core/storage/inmemorytreeview.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/locking.py` & `aimhub_client-0.5.1/src/aim/_core/storage/locking.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/object.py` & `aimhub_client-0.5.1/src/aim/_core/storage/object.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/reporter/__init__.py` & `aimhub_client-0.5.1/src/aim/_core/storage/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/treearrayview.cpp` & `aimhub_client-0.5.1/src/aim/_core/storage/treearrayview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.treearrayview",
         "sources": [
             "src/aim/_core/storage/treearrayview.py"
         ]
     },
     "module_name": "aim._core.storage.treearrayview"
```

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/treearrayview.py` & `aimhub_client-0.5.1/src/aim/_core/storage/treearrayview.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/treeutils.cpp` & `aimhub_client-0.5.1/src/aim/_core/storage/treeutils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.treeutils",
         "sources": [
             "src/aim/_core/storage/treeutils.pyx"
         ]
     },
     "module_name": "aim._core.storage.treeutils"
```

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/treeutils.pyx` & `aimhub_client-0.5.1/src/aim/_core/storage/treeutils.pyx`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/treeutils_non_native.py` & `aimhub_client-0.5.1/src/aim/_core/storage/treeutils_non_native.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/treeview.cpp` & `aimhub_client-0.5.1/src/aim/_core/storage/treeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.treeview",
         "sources": [
             "src/aim/_core/storage/treeview.py"
         ]
     },
     "module_name": "aim._core.storage.treeview"
```

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/treeview.py` & `aimhub_client-0.5.1/src/aim/_core/storage/treeview.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/types.py` & `aimhub_client-0.5.1/src/aim/_core/storage/types.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/utils.cpp` & `aimhub_client-0.5.1/src/aim/_core/storage/utils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-z0ad0z_3/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-vd_96ct4/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.utils",
         "sources": [
             "src/aim/_core/storage/utils.py"
         ]
     },
     "module_name": "aim._core.storage.utils"
```

### Comparing `aimhub_client-0.5.0/src/aim/_core/storage/utils.py` & `aimhub_client-0.5.1/src/aim/_core/storage/utils.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/transport/client.py` & `aimhub_client-0.5.1/src/aim/_core/transport/client.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/transport/heartbeat_sender.py` & `aimhub_client-0.5.1/src/aim/_core/transport/heartbeat_sender.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/transport/message_utils.py` & `aimhub_client-0.5.1/src/aim/_core/transport/message_utils.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/transport/request_queue.py` & `aimhub_client-0.5.1/src/aim/_core/transport/request_queue.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_core/utils/deprecation.py` & `aimhub_client-0.5.1/src/aim/_core/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/analytics/__init__.py` & `aimhub_client-0.5.1/src/aim/_ext/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/cli/cli.py` & `aimhub_client-0.5.1/src/aim/_ext/cli/cli.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/cli/conatiners/commands.py` & `aimhub_client-0.5.1/src/aim/_ext/cli/conatiners/commands.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/cli/conatiners/utils.py` & `aimhub_client-0.5.1/src/aim/_ext/cli/conatiners/utils.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/cli/convert/commands.py` & `aimhub_client-0.5.1/src/aim/_ext/cli/convert/commands.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/cli/convert/processors/mlflow.py` & `aimhub_client-0.5.1/src/aim/_ext/cli/convert/processors/mlflow.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/cli/convert/processors/tensorboard.py` & `aimhub_client-0.5.1/src/aim/_ext/cli/convert/processors/tensorboard.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/cli/convert/processors/wandb.py` & `aimhub_client-0.5.1/src/aim/_ext/cli/convert/processors/wandb.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/cli/login/commands.py` & `aimhub_client-0.5.1/src/aim/_ext/cli/login/commands.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/cli/storage/commands.py` & `aimhub_client-0.5.1/src/aim/_ext/cli/storage/commands.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/cli/upload/commands.py` & `aimhub_client-0.5.1/src/aim/_ext/cli/upload/commands.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/cli/utils.py` & `aimhub_client-0.5.1/src/aim/_ext/cli/utils.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/cli/watcher_cli.py` & `aimhub_client-0.5.1/src/aim/_ext/cli/watcher_cli.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/notebook/manager.py` & `aimhub_client-0.5.1/src/aim/_ext/notebook/manager.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/notebook/notebook.py` & `aimhub_client-0.5.1/src/aim/_ext/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/notifier/__init__.py` & `aimhub_client-0.5.1/src/aim/_ext/notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/notifier/config.py` & `aimhub_client-0.5.1/src/aim/_ext/notifier/config.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/notifier/logging_notifier.py` & `aimhub_client-0.5.1/src/aim/_ext/notifier/logging_notifier.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/notifier/notifier.py` & `aimhub_client-0.5.1/src/aim/_ext/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/notifier/notifier_builder.py` & `aimhub_client-0.5.1/src/aim/_ext/notifier/notifier_builder.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/notifier/slack_notifier.py` & `aimhub_client-0.5.1/src/aim/_ext/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/notifier/utils.py` & `aimhub_client-0.5.1/src/aim/_ext/notifier/utils.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/notifier/workplace_notifier.py` & `aimhub_client-0.5.1/src/aim/_ext/notifier/workplace_notifier.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/system_info/pynvml.py` & `aimhub_client-0.5.1/src/aim/_ext/system_info/pynvml.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/system_info/resource_tracker.py` & `aimhub_client-0.5.1/src/aim/_ext/system_info/resource_tracker.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/system_info/stat.py` & `aimhub_client-0.5.1/src/aim/_ext/system_info/stat.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_ext/system_info/utils.py` & `aimhub_client-0.5.1/src/aim/_ext/system_info/utils.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/base/collections.py` & `aimhub_client-0.5.1/src/aim/_sdk/base/collections.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/base/container.py` & `aimhub_client-0.5.1/src/aim/_sdk/base/container.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/base/context.py` & `aimhub_client-0.5.1/src/aim/_sdk/base/context.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/base/property.py` & `aimhub_client-0.5.1/src/aim/_sdk/base/property.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/base/record.py` & `aimhub_client-0.5.1/src/aim/_sdk/base/record.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/base/repo.py` & `aimhub_client-0.5.1/src/aim/_sdk/base/repo.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/base/sequence.py` & `aimhub_client-0.5.1/src/aim/_sdk/base/sequence.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/configs.py` & `aimhub_client-0.5.1/src/aim/_sdk/configs.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/exceptions.py` & `aimhub_client-0.5.1/src/aim/_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/acme.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/acme.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/catboost.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/catboost.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/fastai.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/fastai.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/hugging_face.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/hugging_face.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/keras.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/keras.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/keras_mixins.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/keras_mixins.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/keras_tuner.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/keras_tuner.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/lightgbm.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/lightgbm.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/mxnet.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/mxnet.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/optuna.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/optuna.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/paddle.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/paddle.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/prophet.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/prophet.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/pytorch.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/pytorch.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/pytorch_ignite.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/pytorch_ignite.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/pytorch_lightning.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/sb3.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/sb3.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/tensorflow.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/tensorflow.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/integrations/xgboost.py` & `aimhub_client-0.5.1/src/aim/_sdk/integrations/xgboost.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/interfaces/container.py` & `aimhub_client-0.5.1/src/aim/_sdk/interfaces/container.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/interfaces/sequence.py` & `aimhub_client-0.5.1/src/aim/_sdk/interfaces/sequence.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/interfaces/storage_engine.py` & `aimhub_client-0.5.1/src/aim/_sdk/interfaces/storage_engine.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/num_utils.py` & `aimhub_client-0.5.1/src/aim/_sdk/num_utils.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/query/analyzer.py` & `aimhub_client-0.5.1/src/aim/_sdk/query/analyzer.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/query/proxy.py` & `aimhub_client-0.5.1/src/aim/_sdk/query/proxy.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/query/query.py` & `aimhub_client-0.5.1/src/aim/_sdk/query/query.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/query/query_utils.py` & `aimhub_client-0.5.1/src/aim/_sdk/query/query_utils.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/remote_storage/__init__.py` & `aimhub_client-0.5.1/src/aim/_sdk/remote_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/type_utils.py` & `aimhub_client-0.5.1/src/aim/_sdk/type_utils.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/types/artifact.py` & `aimhub_client-0.5.1/src/aim/_sdk/types/artifact.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/types/audio.py` & `aimhub_client-0.5.1/src/aim/_sdk/types/audio.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/types/distribution.py` & `aimhub_client-0.5.1/src/aim/_sdk/types/distribution.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/types/experiment.py` & `aimhub_client-0.5.1/src/aim/_sdk/types/experiment.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/types/figures.py` & `aimhub_client-0.5.1/src/aim/_sdk/types/figures.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/types/image.py` & `aimhub_client-0.5.1/src/aim/_sdk/types/image.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/types/io/wavfile.py` & `aimhub_client-0.5.1/src/aim/_sdk/types/io/wavfile.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/types/logging/__init__.py` & `aimhub_client-0.5.1/src/aim/_sdk/types/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/types/metric.py` & `aimhub_client-0.5.1/src/aim/_sdk/types/metric.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/types/run.py` & `aimhub_client-0.5.1/src/aim/_sdk/types/run.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/types/tag.py` & `aimhub_client-0.5.1/src/aim/_sdk/types/tag.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/types/text.py` & `aimhub_client-0.5.1/src/aim/_sdk/types/text.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/uri_service.py` & `aimhub_client-0.5.1/src/aim/_sdk/uri_service.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aim/_sdk/utils.py` & `aimhub_client-0.5.1/src/aim/_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `aimhub_client-0.5.0/src/aimhub_client.egg-info/PKG-INFO` & `aimhub_client-0.5.1/src/aimhub_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimhub-client
-Version: 0.5.0
+Version: 0.5.1
 Summary: A super-easy way to record, search and compare AI experiments.
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `aimhub_client-0.5.0/src/aimhub_client.egg-info/SOURCES.txt` & `aimhub_client-0.5.1/src/aimhub_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

