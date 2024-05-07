# Comparing `tmp/pawnlib-1.1.6.tar.gz` & `tmp/pawnlib-1.1.8.tar.gz`

## Comparing `pawnlib-1.1.6.tar` & `pawnlib-1.1.8.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    10481 2020-02-02 00:00:00.000000 pawnlib-1.1.6/README.md
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/.DS_Store
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/__main__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/__version__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/asyncio/__init__.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/asyncio/run.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/builder/__init__.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/builder/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/builder/templates/__init__.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/builder/templates/app_with_logging.tmpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/__init__.py
--rwxr-xr-x   0        0        0     3290 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/aws.py
--rwxr-xr-x   0        0        0     1170 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/banner.py
--rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/docker.py
--rwxr-xr-x   0        0        0     3303 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/gs.py
--rwxr-xr-x   0        0        0    21479 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/http.py
--rwxr-xr-x   0        0        0     2805 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/icon.py
--rwxr-xr-x   0        0        0     6105 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/info.py
--rwxr-xr-x   0        0        0     1493 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/init.py
--rwxr-xr-x   0        0        0     6923 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/main_cli.py
--rwxr-xr-x   0        0        0     2965 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/main_cli_with_required.py__
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/net.py
--rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/pawns_cli.py__
--rwxr-xr-x   0        0        0    16005 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/proxy.py
--rw-r--r--   0        0        0    16006 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/rpc.py
--rwxr-xr-x   0        0        0    11497 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/top.py
--rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/wallet.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/websocket.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/templates/__init__.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/templates/docker_echo.tmpl
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/cli/templates/docker_planet.tmpl
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/config/__fix_import.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/config/__init__.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/config/configure.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/config/console.py
--rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/config/first_run_checker.py
--rw-r--r--   0        0        0    30148 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/config/globalconfig.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/docker/__init__.py
--rw-r--r--   0        0        0    15894 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/docker/async_docker.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/input/__init__.py
--rw-r--r--   0        0        0    43248 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/input/prompt.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/output/__init__.py
--rw-r--r--   0        0        0    55490 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/output/color_print.py
--rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/output/file.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/resource/__init__.py
--rw-r--r--   0        0        0    19961 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/resource/net.py
--rw-r--r--   0        0        0    34175 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/resource/server.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/typing/__init__.py
--rw-r--r--   0        0        0    18737 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/typing/check.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/typing/constants.py
--rw-r--r--   0        0        0    83951 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/typing/converter.py
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/typing/date_utils.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/typing/defines.py
--rw-r--r--   0        0        0    14793 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/typing/generator.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/utils/__init__.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/utils/genesis.py
--rw-r--r--   0        0        0    80276 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/utils/http.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/utils/icx_raw_singer.py
--rw-r--r--   0        0        0    27296 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/utils/icx_signer.py
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/utils/in_memory_zip.py
--rw-r--r--   0        0        0    12702 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/utils/log.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/utils/notify.py
--rw-r--r--   0        0        0    25836 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pawnlib/utils/operate_handler.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pawnlib-1.1.6/.gitignore
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 pawnlib-1.1.6/pyproject.toml
--rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 pawnlib-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    10481 2020-02-02 00:00:00.000000 pawnlib-1.1.8/README.md
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/.DS_Store
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/__main__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/__version__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/asyncio/__init__.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/asyncio/run.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/builder/__init__.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/builder/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/builder/templates/__init__.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/builder/templates/app_with_logging.tmpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/__init__.py
+-rwxr-xr-x   0        0        0     3290 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/aws.py
+-rwxr-xr-x   0        0        0     1170 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/banner.py
+-rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/docker.py
+-rwxr-xr-x   0        0        0     3303 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/gs.py
+-rwxr-xr-x   0        0        0    21479 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/http.py
+-rwxr-xr-x   0        0        0     2805 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/icon.py
+-rwxr-xr-x   0        0        0     6105 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/info.py
+-rwxr-xr-x   0        0        0     1493 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/init.py
+-rwxr-xr-x   0        0        0     6923 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/main_cli.py
+-rwxr-xr-x   0        0        0     2965 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/main_cli_with_required.py__
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/net.py
+-rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/pawns_cli.py__
+-rwxr-xr-x   0        0        0    16005 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/proxy.py
+-rw-r--r--   0        0        0    16006 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/rpc.py
+-rwxr-xr-x   0        0        0    11482 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/top.py
+-rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/wallet.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/websocket.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/templates/__init__.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/templates/docker_echo.tmpl
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/cli/templates/docker_planet.tmpl
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/config/__fix_import.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/config/__init__.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/config/configure.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/config/console.py
+-rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/config/first_run_checker.py
+-rw-r--r--   0        0        0    30148 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/config/globalconfig.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/docker/__init__.py
+-rw-r--r--   0        0        0    15894 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/docker/async_docker.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/input/__init__.py
+-rw-r--r--   0        0        0    43248 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/input/prompt.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/output/__init__.py
+-rw-r--r--   0        0        0    55490 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/output/color_print.py
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/output/file.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/resource/__init__.py
+-rw-r--r--   0        0        0    19961 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/resource/net.py
+-rw-r--r--   0        0        0    34175 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/resource/server.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/__init__.py
+-rw-r--r--   0        0        0    18737 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/check.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/constants.py
+-rw-r--r--   0        0        0    83698 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/converter.py
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/date_utils.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/defines.py
+-rw-r--r--   0        0        0    14793 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/typing/generator.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/__init__.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/genesis.py
+-rw-r--r--   0        0        0    80276 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/http.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/icx_raw_singer.py
+-rw-r--r--   0        0        0    27296 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/icx_signer.py
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/in_memory_zip.py
+-rw-r--r--   0        0        0    12702 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/log.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/notify.py
+-rw-r--r--   0        0        0    25836 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pawnlib/utils/operate_handler.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pawnlib-1.1.8/.gitignore
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 pawnlib-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 pawnlib-1.1.8/PKG-INFO
```

### Comparing `pawnlib-1.1.6/README.md` & `pawnlib-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/.DS_Store` & `pawnlib-1.1.8/pawnlib/.DS_Store`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/__init__.py` & `pawnlib-1.1.8/pawnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/__main__.py` & `pawnlib-1.1.8/pawnlib/__main__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/asyncio/run.py` & `pawnlib-1.1.8/pawnlib/asyncio/run.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/builder/generator.py` & `pawnlib-1.1.8/pawnlib/builder/generator.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/builder/templates/app_with_logging.tmpl` & `pawnlib-1.1.8/pawnlib/builder/templates/app_with_logging.tmpl`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/aws.py` & `pawnlib-1.1.8/pawnlib/cli/aws.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/banner.py` & `pawnlib-1.1.8/pawnlib/cli/banner.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/docker.py` & `pawnlib-1.1.8/pawnlib/cli/docker.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/gs.py` & `pawnlib-1.1.8/pawnlib/cli/gs.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/http.py` & `pawnlib-1.1.8/pawnlib/cli/http.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/icon.py` & `pawnlib-1.1.8/pawnlib/cli/icon.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/info.py` & `pawnlib-1.1.8/pawnlib/cli/info.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/init.py` & `pawnlib-1.1.8/pawnlib/cli/init.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/main_cli.py` & `pawnlib-1.1.8/pawnlib/cli/main_cli.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/main_cli_with_required.py__` & `pawnlib-1.1.8/pawnlib/cli/main_cli_with_required.py__`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/net.py` & `pawnlib-1.1.8/pawnlib/cli/net.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/pawns_cli.py__` & `pawnlib-1.1.8/pawnlib/cli/pawns_cli.py__`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/proxy.py` & `pawnlib-1.1.8/pawnlib/cli/proxy.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/rpc.py` & `pawnlib-1.1.8/pawnlib/cli/rpc.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/top.py` & `pawnlib-1.1.8/pawnlib/cli/top.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             "net_out": 100,
             "usr": 80,
             "sys": 80,
             "mem_used": 99.5,
             "disk_read":  100,
             "disk_write":  100,
             "load":  int(cores),
-            "io_wait":  int(cores) * 2,
+            "io":  int(cores) * 2,
             "cached":  10,
         }
         self.warning_percent = warning_percent
         self.medium_percent = medium_percent
         self.low_percent = low_percent
 
     @staticmethod
@@ -281,21 +281,21 @@
             "net_in": f"{network['Total'].get('recv'):.2f}M",
             "net_out": f"{network['Total'].get('sent'):.2f}M",
             "pk_in": f"{network['Total'].get('packets_recv')}",
             "pk_out": f"{network['Total'].get('packets_sent')}",
             "load": f"{get_cpu_load()['1min']}",
             "usr": f"{cpu.get('usr')}%",
             "sys": f"{cpu.get('sys')}%",
-            "io_wait": f"{cpu.get('io_wait')}",
-            "disk_read":  f"{disk['total'].get('read_mb')} M",
-            "disk_write":  f"{disk['total'].get('write_mb')} M",
-            "mem_total": f"{memory.get('total')} {memory_unit}",
+            "io": f"{cpu.get('io_wait')}",
+            "disk_read":  f"{disk['total'].get('read_mb')}M",
+            "disk_write":  f"{disk['total'].get('write_mb')}M",
+            "mem_total": f"{memory.get('total')}{memory_unit}",
             # "mem_used": f"{memory.get('percent')}%",
-            "mem_free": f"{memory.get('free')} {memory_unit}",
-            "cached": f"{memory.get('cached')} {memory_unit}",
+            "mem_free": f"{memory.get('free')}{memory_unit}",
+            "cached": f"{memory.get('cached')}{memory_unit}",
         }
     return data
 
 
 if __name__ == '__main__':
     try:
         main()
```

### Comparing `pawnlib-1.1.6/pawnlib/cli/wallet.py` & `pawnlib-1.1.8/pawnlib/cli/wallet.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/websocket.py` & `pawnlib-1.1.8/pawnlib/cli/websocket.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/templates/docker_echo.tmpl` & `pawnlib-1.1.8/pawnlib/cli/templates/docker_echo.tmpl`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/cli/templates/docker_planet.tmpl` & `pawnlib-1.1.8/pawnlib/cli/templates/docker_planet.tmpl`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/config/__fix_import.py` & `pawnlib-1.1.8/pawnlib/config/__fix_import.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/config/configure.py` & `pawnlib-1.1.8/pawnlib/config/configure.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/config/console.py` & `pawnlib-1.1.8/pawnlib/config/console.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/config/first_run_checker.py` & `pawnlib-1.1.8/pawnlib/config/first_run_checker.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/config/globalconfig.py` & `pawnlib-1.1.8/pawnlib/config/globalconfig.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/docker/async_docker.py` & `pawnlib-1.1.8/pawnlib/docker/async_docker.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/input/__init__.py` & `pawnlib-1.1.8/pawnlib/input/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/input/prompt.py` & `pawnlib-1.1.8/pawnlib/input/prompt.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/output/__init__.py` & `pawnlib-1.1.8/pawnlib/output/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/output/color_print.py` & `pawnlib-1.1.8/pawnlib/output/color_print.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/output/file.py` & `pawnlib-1.1.8/pawnlib/output/file.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/resource/__init__.py` & `pawnlib-1.1.8/pawnlib/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/resource/net.py` & `pawnlib-1.1.8/pawnlib/resource/net.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/resource/server.py` & `pawnlib-1.1.8/pawnlib/resource/server.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/typing/__init__.py` & `pawnlib-1.1.8/pawnlib/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/typing/check.py` & `pawnlib-1.1.8/pawnlib/typing/check.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/typing/constants.py` & `pawnlib-1.1.8/pawnlib/typing/constants.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/typing/converter.py` & `pawnlib-1.1.8/pawnlib/typing/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1354,58 +1354,47 @@
                 else:
                     ret[f"{key}{separator}{i}"] = value
         else:
             ret[key] = val
     return ret
 
 
-def dict_to_line(dict_param: dict, quotes: bool = False, separator: str = "=", end_separator: str = ",",
+def dict_to_line(dict_param: dict, quotes: Literal[None, 'all', 'strings_only'] = None, separator: str = "=", end_separator: str = ",",
                  pad_width: int = 0, key_pad_width: int = 0, alignment: str = 'left', key_alignment: str = 'right',
                  callback: callable = None) -> str:
     """
-       Converts a dictionary into a string with various formatting options.
+    Converts a dictionary into a string with various formatting options. Optionally wraps values or string values in quotes.
 
-       :param dict_param: The dictionary to convert.
-       :param quotes: If True, wraps values in quotes.
-       :param separator: The separator between keys and values.
-       :param end_separator: The separator between key-value pairs.
-       :param pad_width: The minimum width for value alignment.
-       :param key_pad_width: The minimum width for key alignment.
-       :param alignment: The alignment of the values ('left', 'right', 'center').
-       :param key_alignment: The alignment of the keys ('left', 'right', 'center').
-       :param callback: An optional callback function to apply to each value.
-       :return: The formatted string.
-
-       Example:
-
-           .. code-block:: python
-
-               dict_param = {'a': 1, 'bb': 22, 'ccc': 333}
-               print(dict_to_line(dict_param, quotes=True, separator=": ", end_separator="; ", pad_width=5, key_pad_width=4, alignment='right', key_alignment='left'))
-               # "a   : "    1"; bb  : "   22"; ccc : "  333"
-       """
+    :param dict_param: The dictionary to convert.
+    :param quotes: 'all' to wrap all values in quotes, 'strings_only' to wrap only string values in quotes, or None.
+    :param separator: The separator between keys and values.
+    :param end_separator: The separator between key-value pairs.
+    :param pad_width: The minimum width for value alignment.
+    :param key_pad_width: The minimum width for key alignment.
+    :param alignment: The alignment of the values ('left', 'right', 'center').
+    :param key_alignment: The alignment of the keys ('left', 'right', 'center').
+    :param callback: An optional callback function to apply to each value.
+    :return: The formatted string.
+    """
     def _format_with_alignment(text, width, alignment):
-        """
-        Formats text according to the given alignment and width.
-        """
         formats = {'left': f"<{width}", 'right': f">{width}", 'center': f"^{width}"}
         format_spec = formats.get(alignment, "<")
         return f"{text:{format_spec}}"
 
     formatted_pairs = []
     for k, v in sorted(dict_param.items()):
         if callback and callable(callback):
             v = callback(v)  # Apply the callback function to the value, if provided
 
         # Apply alignment and padding to keys and values
         formatted_key = _format_with_alignment(k, key_pad_width, key_alignment)
         formatted_value = _format_with_alignment(v, pad_width, alignment)
 
         # Handle quotes option for values
-        if quotes:
+        if (quotes == 'all') or (quotes == 'strings_only' and isinstance(v, str)):
             formatted_value = f"\"{formatted_value}\""
 
         formatted_pairs.append(f"{formatted_key}{separator}{formatted_value}")
 
     return end_separator.join(formatted_pairs)
 
 
@@ -2507,14 +2496,15 @@
         if shorten_middle:
             half_width = width // 2
             return f"{_origin_text[:half_width]}{placeholder}{_origin_text[-half_width:]}"
         else:
             return f"{_origin_text[:width]} {placeholder}"
     return text
 
+
 def remove_ascii_and_tags(text: str = "", case_sensitive: Literal["lower", "upper", "both"] = "lower"):
     text = remove_ascii_color_codes(text)
     text = remove_tags(text, case_sensitive=case_sensitive)
     return text
 
 # def shorten_text(text="", width=None, placeholder='[...]', shorten_middle=False):
 #     """
```

### Comparing `pawnlib-1.1.6/pawnlib/typing/date_utils.py` & `pawnlib-1.1.8/pawnlib/typing/date_utils.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/typing/defines.py` & `pawnlib-1.1.8/pawnlib/typing/defines.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/typing/generator.py` & `pawnlib-1.1.8/pawnlib/typing/generator.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/utils/__init__.py` & `pawnlib-1.1.8/pawnlib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/utils/genesis.py` & `pawnlib-1.1.8/pawnlib/utils/genesis.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/utils/http.py` & `pawnlib-1.1.8/pawnlib/utils/http.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/utils/icx_raw_singer.py` & `pawnlib-1.1.8/pawnlib/utils/icx_raw_singer.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/utils/icx_signer.py` & `pawnlib-1.1.8/pawnlib/utils/icx_signer.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/utils/in_memory_zip.py` & `pawnlib-1.1.8/pawnlib/utils/in_memory_zip.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/utils/log.py` & `pawnlib-1.1.8/pawnlib/utils/log.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/utils/notify.py` & `pawnlib-1.1.8/pawnlib/utils/notify.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pawnlib/utils/operate_handler.py` & `pawnlib-1.1.8/pawnlib/utils/operate_handler.py`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/.gitignore` & `pawnlib-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/pyproject.toml` & `pawnlib-1.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pawnlib-1.1.6/PKG-INFO` & `pawnlib-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawnlib
-Version: 1.1.6
+Version: 1.1.8
 Summary: pawnlib is a collection of libraries for IaC.
 Project-URL: Changelog, https://github.com/jinwoo-j/pawnlib
 Project-URL: Documentation, https://pawnlib.readthedocs.io
 Project-URL: Homepage, https://pawnlib.readthedocs.io
 Project-URL: Source, https://github.com/jinwoo-j/pawnlib
 Author-email: Jinwoo <jinwoo@parametacorp.com>
 License-Expression: MIT
```

