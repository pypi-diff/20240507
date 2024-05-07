# Comparing `tmp/hahomematic-2024.5.0.tar.gz` & `tmp/hahomematic-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.5.0.tar", last modified: Sun May  5 06:54:23 2024, max compression
+gzip compressed data, was "hahomematic-2024.5.1.tar", last modified: Tue May  7 11:23:49 2024, max compression
```

## Comparing `hahomematic-2024.5.0.tar` & `hahomematic-2024.5.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.146227 hahomematic-2024.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-05 06:54:23.146227 hahomematic-2024.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.134227 hahomematic-2024.5.0/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/async_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.134227 hahomematic-2024.5.0/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18130 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/caches/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.134227 hahomematic-2024.5.0/hahomematic/central/
--rw-r--r--   0 runner    (1001) docker     (127)    54833 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/central/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/central/command_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/central/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/central/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.138227 hahomematic-2024.5.0/hahomematic/client/
--rw-r--r--   0 runner    (1001) docker     (127)    46091 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/client/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/client/xml_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.138227 hahomematic-2024.5.0/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.138227 hahomematic-2024.5.0/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26229 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24631 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30099 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    44054 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33380 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    30606 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.142227 hahomematic-2024.5.0/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.142227 hahomematic-2024.5.0/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.142227 hahomematic-2024.5.0/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.146227 hahomematic-2024.5.0/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-05 06:54:23.000000 hahomematic-2024.5.0/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-05 06:54:23.000000 hahomematic-2024.5.0/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 06:54:23.000000 hahomematic-2024.5.0/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 06:54:22.000000 hahomematic-2024.5.0/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-05 06:54:23.000000 hahomematic-2024.5.0/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 06:54:23.000000 hahomematic-2024.5.0/hahomematic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.142227 hahomematic-2024.5.0/hahomematic_support/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/hahomematic_support/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-05 06:54:23.146227 hahomematic-2024.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:54:23.146227 hahomematic-2024.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    32324 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_central_pydevccu.py
--rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    39142 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    17156 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-05 06:53:58.000000 hahomematic-2024.5.0/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.723751 hahomematic-2024.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-07 11:23:49.723751 hahomematic-2024.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.707751 hahomematic-2024.5.1/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/async_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.711751 hahomematic-2024.5.1/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18130 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/caches/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.711751 hahomematic-2024.5.1/hahomematic/central/
+-rw-r--r--   0 runner    (1001) docker     (127)    55184 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/central/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/central/command_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/central/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/central/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.711751 hahomematic-2024.5.1/hahomematic/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    46155 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/client/json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/client/xml_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.711751 hahomematic-2024.5.1/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.715752 hahomematic-2024.5.1/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26229 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24631 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30099 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44054 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33428 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30413 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.715752 hahomematic-2024.5.1/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.719751 hahomematic-2024.5.1/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.719751 hahomematic-2024.5.1/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.723751 hahomematic-2024.5.1/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-07 11:23:49.000000 hahomematic-2024.5.1/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-07 11:23:49.000000 hahomematic-2024.5.1/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:23:49.000000 hahomematic-2024.5.1/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:23:49.000000 hahomematic-2024.5.1/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 11:23:49.000000 hahomematic-2024.5.1/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 11:23:49.000000 hahomematic-2024.5.1/hahomematic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.719751 hahomematic-2024.5.1/hahomematic_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/hahomematic_support/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 11:23:49.723751 hahomematic-2024.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:23:49.723751 hahomematic-2024.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_central_pydevccu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39142 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17156 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-07 11:23:27.000000 hahomematic-2024.5.1/tests/test_text.py
```

### Comparing `hahomematic-2024.5.0/LICENSE` & `hahomematic-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/PKG-INFO` & `hahomematic-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.5.0/README.md` & `hahomematic-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/__init__.py` & `hahomematic-2024.5.1/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/async_support.py` & `hahomematic-2024.5.1/hahomematic/async_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/caches/dynamic.py` & `hahomematic-2024.5.1/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/caches/persistent.py` & `hahomematic-2024.5.1/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/caches/visibility.py` & `hahomematic-2024.5.1/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/central/__init__.py` & `hahomematic-2024.5.1/hahomematic/central/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,22 +100,22 @@
         # Keep the config for the central
         self.config: Final = central_config
         self._name: Final = central_config.name
         self._model: str | None = None
         self._connection_state: Final = central_config.connection_state
         self._looper = Looper()
         self._xml_rpc_server: Final = (
-            xmlrpc.register_xml_rpc_server(
+            xmlrpc.create_xml_rpc_server(
                 local_port=central_config.callback_port or central_config.default_callback_port
             )
             if central_config.enable_server
             else None
         )
         if self._xml_rpc_server:
-            self._xml_rpc_server.register_central(self)
+            self._xml_rpc_server.add_central(self)
         self.local_port: Final[int] = (
             self._xml_rpc_server.local_port if self._xml_rpc_server else 0
         )
 
         # Caches for CCU data
         self.data_cache: Final[CentralDataCache] = CentralDataCache(central=self)
         self.device_details: Final[DeviceDetailsCache] = DeviceDetailsCache(central=self)
@@ -185,15 +185,15 @@
     @property
     def _has_active_threads(self) -> bool:
         """Return if active sub threads are alive."""
         if self._connection_checker.is_alive():
             return True
         if (
             self._xml_rpc_server
-            and self._xml_rpc_server.no_central_registered
+            and self._xml_rpc_server.no_central_assigned
             and self._xml_rpc_server.is_alive()
         ):
             return True
         return False
 
     @property
     def interface_ids(self) -> tuple[str, ...]:
@@ -324,17 +324,17 @@
         self._stop_connection_checker()
         await self._stop_clients()
         if self.json_rpc_client.is_activated:
             await self.json_rpc_client.logout()
 
         if self._xml_rpc_server:
             # un-register this instance from XmlRPC-Server
-            self._xml_rpc_server.unregister_central(central=self)
+            self._xml_rpc_server.remove_central(central=self)
             # un-register and stop XmlRPC-Server, if possible
-            if self._xml_rpc_server.no_central_registered:
+            if self._xml_rpc_server.no_central_assigned:
                 self._xml_rpc_server.stop()
             _LOGGER.debug("STOP: XmlRPC-Server stopped")
         else:
             _LOGGER.debug(
                 "STOP: shared XmlRPC-Server NOT stopped. "
                 "There is still another central instance registered"
             )
@@ -867,16 +867,17 @@
         entity_key = get_entity_key(
             channel_address=channel_address,
             parameter=parameter,
         )
 
         if entity_key in self._entity_event_subscriptions:
             try:
-                for callback in self._entity_event_subscriptions[entity_key]:
-                    await callback(value)
+                for callback_handler in self._entity_event_subscriptions[entity_key]:
+                    if callable(callback_handler):
+                        await callback_handler(value)
             except RuntimeError as rte:  # pragma: no cover
                 _LOGGER.debug(
                     "EVENT: RuntimeError [%s]. Failed to call callback for: %s, %s, %s",
                     reduce_args(args=rte.args),
                     interface_id,
                     channel_address,
                     parameter,
@@ -1030,16 +1031,18 @@
         await self.device_descriptions.clear()
         await self.paramset_descriptions.clear()
         self.device_details.clear()
         self.data_cache.clear()
 
     def register_homematic_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register ha_event callback in central."""
-        self._homematic_callbacks.add(cb)
-        return partial(self._unregister_homematic_callback, cb)
+        if callable(cb) and cb not in self._homematic_callbacks:
+            self._homematic_callbacks.add(cb)
+            return partial(self._unregister_homematic_callback, cb)
+        return None
 
     def _unregister_homematic_callback(self, cb: Callable) -> None:
         """RUn register ha_event callback in central."""
         if cb in self._homematic_callbacks:
             self._homematic_callbacks.remove(cb)
 
     @loop_check
@@ -1058,16 +1061,18 @@
                 _LOGGER.error(
                     "FIRE_HOMEMATIC_CALLBACK: Unable to call handler: %s",
                     reduce_args(args=ex.args),
                 )
 
     def register_backend_parameter_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register backend_parameter callback in central."""
-        self._backend_parameter_callbacks.add(cb)
-        return partial(self._unregister_backend_parameter_callback, cb)
+        if callable(cb) and cb not in self._backend_parameter_callbacks:
+            self._backend_parameter_callbacks.add(cb)
+            return partial(self._unregister_backend_parameter_callback, cb)
+        return None
 
     def _unregister_backend_parameter_callback(self, cb: Callable) -> None:
         """Un register backend_parameter callback in central."""
         if cb in self._backend_parameter_callbacks:
             self._backend_parameter_callbacks.remove(cb)
 
     @loop_check
@@ -1087,16 +1092,18 @@
                 _LOGGER.error(
                     "FIRE_BACKEND_PARAMETER_CALLBACK: Unable to call handler: %s",
                     reduce_args(args=ex.args),
                 )
 
     def register_backend_system_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register system_event callback in central."""
-        self._backend_system_callbacks.add(cb)
-        return partial(self._unregister_backend_system_callback, cb)
+        if callable(cb) and cb not in self._backend_parameter_callbacks:
+            self._backend_system_callbacks.add(cb)
+            return partial(self._unregister_backend_system_callback, cb)
+        return None
 
     def _unregister_backend_system_callback(self, cb: Callable) -> None:
         """Un register system_event callback in central."""
         if cb in self._backend_system_callbacks:
             self._backend_system_callbacks.remove(cb)
 
     @loop_check
```

### Comparing `hahomematic-2024.5.0/hahomematic/central/command_queue.py` & `hahomematic-2024.5.1/hahomematic/central/command_queue.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/central/decorators.py` & `hahomematic-2024.5.1/hahomematic/central/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/central/xml_rpc_server.py` & `hahomematic-2024.5.1/hahomematic/central/xml_rpc_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,37 +209,37 @@
             del self._instances[self.local_port]
 
     @property
     def started(self) -> bool:
         """Return if thread is active."""
         return self._started.is_set() is True  # type: ignore[attr-defined]
 
-    def register_central(self, central: hmcu.CentralUnit) -> None:
+    def add_central(self, central: hmcu.CentralUnit) -> None:
         """Register a central in the XmlRPC-Server."""
         if not self._centrals.get(central.name):
             self._centrals[central.name] = central
 
-    def unregister_central(self, central: hmcu.CentralUnit) -> None:
+    def remove_central(self, central: hmcu.CentralUnit) -> None:
         """Unregister a central from XmlRPC-Server."""
         if self._centrals.get(central.name):
             del self._centrals[central.name]
 
     def get_central(self, interface_id: str) -> hmcu.CentralUnit | None:
         """Return a central by interface_id."""
         for central in self._centrals.values():
             if central.has_client(interface_id=interface_id):
                 return central
         return None
 
     @property
-    def no_central_registered(self) -> bool:
-        """Return if no central is registered."""
+    def no_central_assigned(self) -> bool:
+        """Return if no central is assigned."""
         return len(self._centrals) == 0
 
 
-def register_xml_rpc_server(local_port: int = PORT_ANY) -> XmlRpcServer:
+def create_xml_rpc_server(local_port: int = PORT_ANY) -> XmlRpcServer:
     """Register the xml rpc server."""
     xml_rpc = XmlRpcServer(local_port=local_port)
     if not xml_rpc.started:
         xml_rpc.start()
-        _LOGGER.debug("REGISTER_XML_RPC_SERVER: Starting XmlRPC-Server")
+        _LOGGER.debug("CREATE_XML_RPC_SERVER: Starting XmlRPC-Server")
     return xml_rpc
```

### Comparing `hahomematic-2024.5.0/hahomematic/client/__init__.py` & `hahomematic-2024.5.1/hahomematic/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1175,17 +1175,20 @@
     if entity := device.get_generic_entity(channel_address=channel_address, parameter=parameter):
         if not entity.supports_events:
             _LOGGER.debug(
                 "TRACK_SINGLE_ENTITY_STATE_CHANGE_OR_TIMEOUT: Entity supports no events %s",
                 entity_key,
             )
             return
-        unsub = entity.register_entity_updated_callback(
-            cb=_async_event_changed, custom_id=DEFAULT_CUSTOM_ID
-        )
+        if (
+            unsub := entity.register_entity_updated_callback(
+                cb=_async_event_changed, custom_id=DEFAULT_CUSTOM_ID
+            )
+        ) is None:
+            return
 
         try:
             async with asyncio.timeout(wait_for_callback):
                 await ev.wait()
         except TimeoutError:
             _LOGGER.debug(
                 "TRACK_SINGLE_ENTITY_STATE_CHANGE_OR_TIMEOUT: Timeout waiting for event %s with value %s",
```

### Comparing `hahomematic-2024.5.0/hahomematic/client/json_rpc.py` & `hahomematic-2024.5.1/hahomematic/client/json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/client/xml_rpc.py` & `hahomematic-2024.5.1/hahomematic/client/xml_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/config.py` & `hahomematic-2024.5.1/hahomematic/config.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/const.py` & `hahomematic-2024.5.1/hahomematic/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 MAX_CACHE_AGE: Final = 60
 
 NO_CACHE_ENTRY: Final = "NO_CACHE_ENTRY"
 
 # channel_address, parameter
 ENTITY_KEY = tuple[str, str]
-CALLBACK_TYPE = Callable[[], None]
+CALLBACK_TYPE = Callable[[], None] | None
 
 
 class Backend(StrEnum):
     """Enum with supported hahomematic backends."""
 
     CCU = "CCU"
     HOMEGEAR = "Homegear"
```

### Comparing `hahomematic-2024.5.0/hahomematic/converter.py` & `hahomematic-2024.5.1/hahomematic/converter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/exceptions.py` & `hahomematic-2024.5.1/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/hmcli.py` & `hahomematic-2024.5.1/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/performance.py` & `hahomematic-2024.5.1/hahomematic/performance.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/__init__.py` & `hahomematic-2024.5.1/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/custom/__init__.py` & `hahomematic-2024.5.1/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/custom/climate.py` & `hahomematic-2024.5.1/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/custom/const.py` & `hahomematic-2024.5.1/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/custom/cover.py` & `hahomematic-2024.5.1/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/custom/definition.py` & `hahomematic-2024.5.1/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/custom/entity.py` & `hahomematic-2024.5.1/hahomematic/platforms/custom/entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from collections.abc import Callable, Mapping
 from datetime import datetime
 import logging
 from typing import Any, Final, TypeVar, cast
 
-from hahomematic.const import ENTITY_KEY, INIT_DATETIME, CallSource, EntityUsage
+from hahomematic.const import CALLBACK_TYPE, ENTITY_KEY, INIT_DATETIME, CallSource, EntityUsage
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.custom import definition as hmed
 from hahomematic.platforms.custom.const import DeviceProfile, Field
 from hahomematic.platforms.custom.support import ExtendedConfig
 from hahomematic.platforms.decorators import config_property
 from hahomematic.platforms.entity import BaseEntity, CallParameterCollector
 from hahomematic.platforms.generic import entity as hmge
@@ -37,14 +37,15 @@
         device_def: Mapping[str, Any],
         entity_def: Mapping[int | tuple[int, ...], tuple[str, ...]],
         channel_no: int,
         base_channel_no: int,
         extended: ExtendedConfig | None = None,
     ) -> None:
         """Initialize the entity."""
+        self._unregister_callbacks: list[CALLBACK_TYPE] = []
         self._device_profile: Final = device_profile
         # required for name in BaseEntity
         self._device_desc: Final = device_def
         self._entity_def: Final = entity_def
         self._base_channel_no: int = base_channel_no
         super().__init__(
             device=device,
@@ -235,21 +236,24 @@
             return
         self.device.add_sub_device_channel(
             channel_no=self._channel_no, base_channel_no=self._base_channel_no
         )
         if is_visible:
             entity.set_usage(EntityUsage.CE_VISIBLE)
 
-        entity.register_internal_entity_updated_callback(cb=self.fire_entity_updated_callback)
+        self._unregister_callbacks.append(
+            entity.register_internal_entity_updated_callback(cb=self.fire_entity_updated_callback)
+        )
         self._data_entities[field] = entity
 
     def _unregister_entity_updated_callback(self, cb: Callable, custom_id: str) -> None:
         """Unregister update callback."""
-        for entity in self._data_entities.values():
-            entity.unregister_internal_entity_updated_callback(cb=cb)
+        for unregister in self._unregister_callbacks:
+            if unregister is not None:
+                unregister()
 
         super()._unregister_entity_updated_callback(cb=cb, custom_id=custom_id)
 
     def _mark_entities(self, entity_def: Mapping[int | tuple[int, ...], tuple[str, ...]]) -> None:
         """Mark entities to be created in HA."""
         if not entity_def:
             return
```

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/custom/light.py` & `hahomematic-2024.5.1/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/custom/lock.py` & `hahomematic-2024.5.1/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/custom/siren.py` & `hahomematic-2024.5.1/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/custom/support.py` & `hahomematic-2024.5.1/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/custom/switch.py` & `hahomematic-2024.5.1/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/decorators.py` & `hahomematic-2024.5.1/hahomematic/platforms/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/device.py` & `hahomematic-2024.5.1/hahomematic/platforms/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,26 +393,28 @@
             self.remove_entity(custom_entity)
         self._custom_entities.clear()
 
     def _register_device_updated_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register update callback."""
         if callable(cb) and cb not in self._device_updated_callbacks:
             self._device_updated_callbacks.append(cb)
-        return partial(self._unregister_device_updated_callback, cb)
+            return partial(self._unregister_device_updated_callback, cb)
+        return None
 
     def _unregister_device_updated_callback(self, cb: Callable) -> None:
         """Remove update callback."""
         if cb in self._device_updated_callbacks:
             self._device_updated_callbacks.remove(cb)
 
     def register_firmware_update_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register firmware update callback."""
         if callable(cb) and cb not in self._firmware_update_callbacks:
             self._firmware_update_callbacks.append(cb)
-        return partial(self.unregister_firmware_update_callback, cb)
+            return partial(self.unregister_firmware_update_callback, cb)
+        return None
 
     def unregister_firmware_update_callback(self, cb: Callable) -> None:
         """Remove firmware update callback."""
         if cb in self._firmware_update_callbacks:
             self._firmware_update_callbacks.remove(cb)
 
     def _set_last_updated(self) -> None:
```

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/entity.py` & `hahomematic-2024.5.1/hahomematic/platforms/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,45 +183,43 @@
     @property
     def is_registered(self) -> bool:
         """Return if entity is registered externally."""
         return self._custom_id is not None
 
     def register_internal_entity_updated_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register internal entity updated callback."""
-        self.register_entity_updated_callback(cb=cb, custom_id=DEFAULT_CUSTOM_ID)
-        return partial(self.unregister_internal_entity_updated_callback, cb)
+        return self.register_entity_updated_callback(cb=cb, custom_id=DEFAULT_CUSTOM_ID)
 
     def register_entity_updated_callback(self, cb: Callable, custom_id: str) -> CALLBACK_TYPE:
         """Register entity updated callback."""
-        if callable(cb):
-            self._entity_updated_callbacks[cb] = custom_id
         if custom_id != DEFAULT_CUSTOM_ID:
             if self._custom_id is not None and self._custom_id != custom_id:
                 raise HaHomematicException(
                     f"REGISTER_entity_updated_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
                 )
             self._custom_id = custom_id
-        return partial(self._unregister_entity_updated_callback, cb, custom_id)
 
-    def unregister_internal_entity_updated_callback(self, cb: Callable) -> None:
-        """Unregister entity updated callback."""
-        self._unregister_entity_updated_callback(cb=cb, custom_id=DEFAULT_CUSTOM_ID)
+        if callable(cb) and cb not in self._entity_updated_callbacks:
+            self._entity_updated_callbacks[cb] = custom_id
+            return partial(self._unregister_entity_updated_callback, cb, custom_id)
+        return None
 
     def _unregister_entity_updated_callback(self, cb: Callable, custom_id: str) -> None:
         """Unregister entity updated callback."""
         if cb in self._entity_updated_callbacks:
             del self._entity_updated_callbacks[cb]
         if self.custom_id == custom_id:
             self._custom_id = None
 
     def register_device_removed_callback(self, cb: Callable) -> CALLBACK_TYPE:
         """Register the device removed callback."""
         if callable(cb) and cb not in self._device_removed_callbacks:
             self._device_removed_callbacks.append(cb)
-        return partial(self._unregister_device_removed_callback, cb)
+            return partial(self._unregister_device_removed_callback, cb)
+        return None
 
     def _unregister_device_removed_callback(self, cb: Callable) -> None:
         """Unregister the device removed callback."""
         if cb in self._device_removed_callbacks:
             self._device_removed_callbacks.remove(cb)
 
     @loop_check
```

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/event.py` & `hahomematic-2024.5.1/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/generic/__init__.py` & `hahomematic-2024.5.1/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/generic/action.py` & `hahomematic-2024.5.1/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2024.5.1/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/generic/button.py` & `hahomematic-2024.5.1/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/generic/entity.py` & `hahomematic-2024.5.1/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/generic/number.py` & `hahomematic-2024.5.1/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/generic/select.py` & `hahomematic-2024.5.1/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/generic/sensor.py` & `hahomematic-2024.5.1/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/generic/switch.py` & `hahomematic-2024.5.1/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/hub/__init__.py` & `hahomematic-2024.5.1/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2024.5.1/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/hub/button.py` & `hahomematic-2024.5.1/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/hub/entity.py` & `hahomematic-2024.5.1/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/hub/number.py` & `hahomematic-2024.5.1/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/hub/select.py` & `hahomematic-2024.5.1/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/hub/sensor.py` & `hahomematic-2024.5.1/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/hub/text.py` & `hahomematic-2024.5.1/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/support.py` & `hahomematic-2024.5.1/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/platforms/update.py` & `hahomematic-2024.5.1/hahomematic/platforms/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,28 +71,30 @@
     @value_property
     def firmware_update_state(self) -> str | None:
         """Latest version available for install."""
         return self._device.firmware_update_state
 
     def register_entity_updated_callback(self, cb: Callable, custom_id: str) -> CALLBACK_TYPE:
         """Register update callback."""
-        self._device.register_firmware_update_callback(cb)
         if custom_id != DEFAULT_CUSTOM_ID:
             if self._custom_id is not None:
                 raise HaHomematicException(
                     f"REGISTER_UPDATE_CALLBACK failed: hm_entity: {self.full_name} is already registered by {self._custom_id}"
                 )
             self._custom_id = custom_id
-        return partial(self._unregister_entity_updated_callback, cb, custom_id)
+
+        if self._device.register_firmware_update_callback(cb) is not None:
+            return partial(self._unregister_entity_updated_callback, cb, custom_id)
+        return None
 
     def _unregister_entity_updated_callback(self, cb: Callable, custom_id: str) -> None:
         """Unregister update callback."""
-        self._device.unregister_firmware_update_callback(cb)
         if custom_id is not None:
             self._custom_id = None
+        self._device.unregister_firmware_update_callback(cb)
 
     async def update_firmware(self, refresh_after_update_intervals: tuple[int, ...]) -> bool:
         """Turn the update on."""
         return await self._device.update_firmware(
             refresh_after_update_intervals=refresh_after_update_intervals
         )
```

### Comparing `hahomematic-2024.5.0/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2024.5.1/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2024.5.1/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2024.5.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic/support.py` & `hahomematic-2024.5.1/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic.egg-info/PKG-INFO` & `hahomematic-2024.5.1/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.5.0/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2024.5.1/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/hahomematic_support/client_local.py` & `hahomematic-2024.5.1/hahomematic_support/client_local.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/pyproject.toml` & `hahomematic-2024.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=69.2.0", "wheel~=0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2024.5.0"
+version     = "2024.5.1"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

### Comparing `hahomematic-2024.5.0/tests/test_action.py` & `hahomematic-2024.5.1/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_binary_sensor.py` & `hahomematic-2024.5.1/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_button.py` & `hahomematic-2024.5.1/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_central.py` & `hahomematic-2024.5.1/tests/test_central.py`

 * *Files 0% similar despite different names*

```diff
@@ -923,15 +923,15 @@
                 "instance_name": "CentralTest",
                 "pong_mismatch_count": 16,
             },
             "interface_id": "CentralTest-BidCos-RF",
             "type": InterfaceEventType.PENDING_PONG,
         },
     )
-    assert len(factory.ha_event_mock.mock_calls) == 9
+    assert len(factory.ha_event_mock.mock_calls) == 10
 
 
 @pytest.mark.asyncio()
 @pytest.mark.parametrize(
     (
         "address_device_translation",
         "do_mock_client",
```

### Comparing `hahomematic-2024.5.0/tests/test_central_pydevccu.py` & `hahomematic-2024.5.1/tests/test_central_pydevccu.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_climate.py` & `hahomematic-2024.5.1/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_cover.py` & `hahomematic-2024.5.1/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_decorator.py` & `hahomematic-2024.5.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_device.py` & `hahomematic-2024.5.1/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_entity.py` & `hahomematic-2024.5.1/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_event.py` & `hahomematic-2024.5.1/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_json_rpc.py` & `hahomematic-2024.5.1/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_light.py` & `hahomematic-2024.5.1/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_lock.py` & `hahomematic-2024.5.1/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_number.py` & `hahomematic-2024.5.1/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_select.py` & `hahomematic-2024.5.1/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_sensor.py` & `hahomematic-2024.5.1/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_siren.py` & `hahomematic-2024.5.1/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_support.py` & `hahomematic-2024.5.1/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_switch.py` & `hahomematic-2024.5.1/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.0/tests/test_text.py` & `hahomematic-2024.5.1/tests/test_text.py`

 * *Files identical despite different names*

