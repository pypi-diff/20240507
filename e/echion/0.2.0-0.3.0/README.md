# Comparing `tmp/echion-0.2.0.tar.gz` & `tmp/echion-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echion-0.2.0.tar", last modified: Sat Oct 14 16:15:15 2023, max compression
+gzip compressed data, was "echion-0.3.0.tar", last modified: Tue May  7 11:00:47 2024, max compression
```

## Comparing `echion-0.2.0.tar` & `echion-0.3.0.tar`

### file list

```diff
@@ -1,73 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 16:15:15.281535 echion-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-10-14 16:15:07.000000 echion-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 16:15:15.273535 echion-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-14 16:15:07.000000 echion-0.2.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 16:15:15.273535 echion-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-10-14 16:15:07.000000 echion-0.2.0/.github/workflows/build_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-10-14 16:15:07.000000 echion-0.2.0/.github/workflows/checks.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      238 2023-10-14 16:15:07.000000 echion-0.2.0/.github/workflows/cibw_before_all.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2023-10-14 16:15:07.000000 echion-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2023-10-14 16:15:07.000000 echion-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-14 16:15:07.000000 echion-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2023-10-14 16:15:15.281535 echion-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2023-10-14 16:15:07.000000 echion-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 16:15:15.273535 echion-0.2.0/art/
--rw-r--r--   0 runner    (1001) docker     (127)   666720 2023-10-14 16:15:07.000000 echion-0.2.0/art/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 16:15:15.277535 echion-0.2.0/echion/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-10-14 16:15:07.000000 echion-0.2.0/echion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2023-10-14 16:15:07.000000 echion-0.2.0/echion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-14 16:15:15.000000 echion-0.2.0/echion/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 16:15:15.277535 echion-0.2.0/echion/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2023-10-14 16:15:07.000000 echion-0.2.0/echion/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2023-10-14 16:15:07.000000 echion-0.2.0/echion/bootstrap/attach.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-10-14 16:15:07.000000 echion-0.2.0/echion/bootstrap/preload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2023-10-14 16:15:07.000000 echion-0.2.0/echion/bootstrap/sitecustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2023-10-14 16:15:07.000000 echion-0.2.0/echion/cache.h
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-10-14 16:15:07.000000 echion-0.2.0/echion/config.h
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-10-14 16:15:07.000000 echion-0.2.0/echion/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11470 2023-10-14 16:15:07.000000 echion-0.2.0/echion/coremodule.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 16:15:15.277535 echion-0.2.0/echion/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2023-10-14 16:15:07.000000 echion-0.2.0/echion/cpython/tasks.h
--rw-r--r--   0 runner    (1001) docker     (127)    10942 2023-10-14 16:15:07.000000 echion-0.2.0/echion/frame.h
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2023-10-14 16:15:07.000000 echion-0.2.0/echion/mirrors.h
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2023-10-14 16:15:07.000000 echion-0.2.0/echion/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 16:15:15.277535 echion-0.2.0/echion/monkey/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-14 16:15:07.000000 echion-0.2.0/echion/monkey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2023-10-14 16:15:07.000000 echion-0.2.0/echion/monkey/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2023-10-14 16:15:07.000000 echion-0.2.0/echion/monkey/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-10-14 16:15:07.000000 echion-0.2.0/echion/signals.h
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2023-10-14 16:15:07.000000 echion-0.2.0/echion/stacks.h
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-10-14 16:15:07.000000 echion-0.2.0/echion/state.h
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2023-10-14 16:15:07.000000 echion-0.2.0/echion/strings.h
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2023-10-14 16:15:07.000000 echion-0.2.0/echion/tasks.h
--rw-r--r--   0 runner    (1001) docker     (127)    13394 2023-10-14 16:15:07.000000 echion-0.2.0/echion/threads.h
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-10-14 16:15:07.000000 echion-0.2.0/echion/timing.h
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2023-10-14 16:15:07.000000 echion-0.2.0/echion/vm.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 16:15:15.277535 echion-0.2.0/echion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2023-10-14 16:15:15.000000 echion-0.2.0/echion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2023-10-14 16:15:15.000000 echion-0.2.0/echion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-14 16:15:15.000000 echion-0.2.0/echion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-14 16:15:15.000000 echion-0.2.0/echion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-14 16:15:15.000000 echion-0.2.0/echion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-14 16:15:15.000000 echion-0.2.0/echion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2023-10-14 16:15:07.000000 echion-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 16:15:15.277535 echion-0.2.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      197 2023-10-14 16:15:07.000000 echion-0.2.0/scripts/build_libunwind.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-14 16:15:15.281535 echion-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2023-10-14 16:15:07.000000 echion-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 16:15:15.281535 echion-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-14 16:15:07.000000 echion-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2023-10-14 16:15:07.000000 echion-0.2.0/tests/target.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-10-14 16:15:07.000000 echion-0.2.0/tests/target_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-10-14 16:15:07.000000 echion-0.2.0/tests/target_async_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-10-14 16:15:07.000000 echion-0.2.0/tests/target_attach.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-10-14 16:15:07.000000 echion-0.2.0/tests/target_bytecode.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1395 2023-10-14 16:15:07.000000 echion-0.2.0/tests/target_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2023-10-14 16:15:07.000000 echion-0.2.0/tests/target_gather.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-10-14 16:15:07.000000 echion-0.2.0/tests/target_where.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-10-14 16:15:07.000000 echion-0.2.0/tests/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2023-10-14 16:15:07.000000 echion-0.2.0/tests/test_cpu_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-10-14 16:15:07.000000 echion-0.2.0/tests/test_echion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2023-10-14 16:15:07.000000 echion-0.2.0/tests/test_wall_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-10-14 16:15:07.000000 echion-0.2.0/tests/test_where.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2023-10-14 16:15:07.000000 echion-0.2.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:47.711127 echion-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-07 11:00:42.000000 echion-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:47.699127 echion-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 11:00:42.000000 echion-0.3.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:47.699127 echion-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-07 11:00:42.000000 echion-0.3.0/.github/workflows/build_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-07 11:00:42.000000 echion-0.3.0/.github/workflows/checks.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      238 2024-05-07 11:00:42.000000 echion-0.3.0/.github/workflows/cibw_before_all.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-07 11:00:42.000000 echion-0.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-07 11:00:42.000000 echion-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-07 11:00:42.000000 echion-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-05-07 11:00:47.711127 echion-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-07 11:00:42.000000 echion-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:47.699127 echion-0.3.0/art/
+-rw-r--r--   0 runner    (1001) docker     (127)   666720 2024-05-07 11:00:42.000000 echion-0.3.0/art/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:47.703127 echion-0.3.0/echion/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-07 11:00:42.000000 echion-0.3.0/echion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-07 11:00:42.000000 echion-0.3.0/echion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 11:00:47.000000 echion-0.3.0/echion/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:47.707127 echion-0.3.0/echion/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-07 11:00:42.000000 echion-0.3.0/echion/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-07 11:00:42.000000 echion-0.3.0/echion/bootstrap/attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 11:00:42.000000 echion-0.3.0/echion/bootstrap/preload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-07 11:00:42.000000 echion-0.3.0/echion/bootstrap/sitecustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-07 11:00:42.000000 echion-0.3.0/echion/cache.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-07 11:00:42.000000 echion-0.3.0/echion/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-07 11:00:42.000000 echion-0.3.0/echion/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-05-07 11:00:42.000000 echion-0.3.0/echion/coremodule.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:47.707127 echion-0.3.0/echion/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-05-07 11:00:42.000000 echion-0.3.0/echion/cpython/tasks.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15814 2024-05-07 11:00:42.000000 echion-0.3.0/echion/frame.h
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-07 11:00:42.000000 echion-0.3.0/echion/interp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-05-07 11:00:42.000000 echion-0.3.0/echion/memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-07 11:00:42.000000 echion-0.3.0/echion/mirrors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-07 11:00:42.000000 echion-0.3.0/echion/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-07 11:00:42.000000 echion-0.3.0/echion/mojo.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:47.707127 echion-0.3.0/echion/monkey/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:42.000000 echion-0.3.0/echion/monkey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-07 11:00:42.000000 echion-0.3.0/echion/monkey/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-07 11:00:42.000000 echion-0.3.0/echion/monkey/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-07 11:00:42.000000 echion-0.3.0/echion/signals.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-05-07 11:00:42.000000 echion-0.3.0/echion/stacks.h
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-07 11:00:42.000000 echion-0.3.0/echion/state.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-07 11:00:42.000000 echion-0.3.0/echion/strings.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-05-07 11:00:42.000000 echion-0.3.0/echion/tasks.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-05-07 11:00:42.000000 echion-0.3.0/echion/threads.h
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-07 11:00:42.000000 echion-0.3.0/echion/timing.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-07 11:00:42.000000 echion-0.3.0/echion/vm.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:47.711127 echion-0.3.0/echion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-05-07 11:00:47.000000 echion-0.3.0/echion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-07 11:00:47.000000 echion-0.3.0/echion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:00:47.000000 echion-0.3.0/echion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 11:00:47.000000 echion-0.3.0/echion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 11:00:47.000000 echion-0.3.0/echion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 11:00:47.000000 echion-0.3.0/echion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-07 11:00:42.000000 echion-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:47.707127 echion-0.3.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-05-07 11:00:42.000000 echion-0.3.0/scripts/build_libunwind.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:00:47.711127 echion-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-07 11:00:42.000000 echion-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:47.707127 echion-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:42.000000 echion-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 11:00:42.000000 echion-0.3.0/tests/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-07 11:00:42.000000 echion-0.3.0/tests/target_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-07 11:00:42.000000 echion-0.3.0/tests/target_async_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-07 11:00:42.000000 echion-0.3.0/tests/target_attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-07 11:00:42.000000 echion-0.3.0/tests/target_bytecode.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1395 2024-05-07 11:00:42.000000 echion-0.3.0/tests/target_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-07 11:00:42.000000 echion-0.3.0/tests/target_gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-07 11:00:42.000000 echion-0.3.0/tests/target_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-07 11:00:42.000000 echion-0.3.0/tests/target_where.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-07 11:00:42.000000 echion-0.3.0/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-07 11:00:42.000000 echion-0.3.0/tests/test_cpu_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-07 11:00:42.000000 echion-0.3.0/tests/test_echion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-07 11:00:42.000000 echion-0.3.0/tests/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-07 11:00:42.000000 echion-0.3.0/tests/test_wall_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-07 11:00:42.000000 echion-0.3.0/tests/test_where.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-07 11:00:42.000000 echion-0.3.0/tests/utils.py
```

### Comparing `echion-0.2.0/.github/workflows/build_release.yml` & `echion-0.3.0/.github/workflows/build_release.yml`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/.github/workflows/checks.yml` & `echion-0.3.0/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/.github/workflows/tests.yml` & `echion-0.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/.gitignore` & `echion-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/LICENSE` & `echion-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/PKG-INFO` & `echion-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: echion
-Version: 0.2.0
-Summary: In-process CPython frame stack sampler
-Author: Gabriele N. Tornetta
-Author-email: "Gabriele N. Tornetta" <phoenix1987@gmail.com>
-Project-URL: homepage, https://github.com/P403n1x87/echion
-Project-URL: repository, https://github.com/P403n1x87/echion
-Project-URL: issues, https://github.com/P403n1x87/echion/issues
-Keywords: performance,profiling,testing,development
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: hypno~=1.0
-
 <p align="center">
   <img align="center" src="art/logo.png" height="320px" />
 </p>
 
 <h1 align="center">Echion</h1>
 
 <p align="center">
@@ -76,14 +54,15 @@
 options:
   -h, --help            show this help message and exit
   -i INTERVAL, --interval INTERVAL
                         sampling interval in microseconds
   -c, --cpu             sample on-CPU stacks only
   -x EXPOSURE, --exposure EXPOSURE
                         exposure time, in seconds
+  -m, --memory          Collect memory allocation events
   -n, --native          sample native stacks
   -o OUTPUT, --output OUTPUT
                         output location (can use %(pid) to insert the process ID)
   -p PID, --pid PID     Attach to the process with the given PID
   -s, --stealth         stealth mode (sampler thread is not accounted for)
   -w WHERE, --where WHERE
                         where mode: display thread stacks of the given process
@@ -119,14 +98,33 @@
 
 When running or attaching to a process, you can also send a `SIGQUIT` signal to
 dump the stacks of all running threads. The result is similar to the where mode.
 You can normally send a `SIGQUIT` signal with the <kbd>CTRL</kbd>+<kbd>\\</kbd>
 key combination.
 
 
+## Memory mode
+
+Besides wall time and CPU time, Echion can be used to profile memory
+allocations. In this mode, Echion tracks the Python memory domain allocators and
+accounts for each single event. Because of the tracing nature, this mode
+introduces considerable overhead, but gives pretty accurate results that can be
+used to investigate potential memory leaks. To fully understand that data that
+is collected in this mode, one should be aware of how Echion tracks allocations
+and deallocations. When an allocation is made, Echion records the frame stack
+that was involved and maps it to the returned memory address. When a
+deallocation for a tracked memory address is made, the freed memory is accounted
+for the same stack. Therefore, objects that are allocated and deallocated during
+the tracking period account for a total of 0 allocated bytes. This means that
+all the non-negative values reported by Echion represent memory that was still
+allocated by the time the tracking ended.
+
+*Since Echion 0.3.0*.
+
+
 ## Why Echion?
 
 Sampling in-process comes with some benefits. One has easier access to more
 information, like thread names, and potentially the task abstraction of async
 frameworks, like `asyncio`, `gevent`, ... . Also available is more accurate
 per-thread CPU timing information.
```

### Comparing `echion-0.2.0/README.md` & `echion-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: echion
+Version: 0.3.0
+Summary: In-process CPython frame stack sampler
+Author: Gabriele N. Tornetta
+Author-email: "Gabriele N. Tornetta" <phoenix1987@gmail.com>
+Project-URL: homepage, https://github.com/P403n1x87/echion
+Project-URL: repository, https://github.com/P403n1x87/echion
+Project-URL: issues, https://github.com/P403n1x87/echion/issues
+Keywords: performance,profiling,testing,development
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: hypno~=1.0
+
 <p align="center">
   <img align="center" src="art/logo.png" height="320px" />
 </p>
 
 <h1 align="center">Echion</h1>
 
 <p align="center">
@@ -54,14 +76,15 @@
 options:
   -h, --help            show this help message and exit
   -i INTERVAL, --interval INTERVAL
                         sampling interval in microseconds
   -c, --cpu             sample on-CPU stacks only
   -x EXPOSURE, --exposure EXPOSURE
                         exposure time, in seconds
+  -m, --memory          Collect memory allocation events
   -n, --native          sample native stacks
   -o OUTPUT, --output OUTPUT
                         output location (can use %(pid) to insert the process ID)
   -p PID, --pid PID     Attach to the process with the given PID
   -s, --stealth         stealth mode (sampler thread is not accounted for)
   -w WHERE, --where WHERE
                         where mode: display thread stacks of the given process
@@ -97,14 +120,33 @@
 
 When running or attaching to a process, you can also send a `SIGQUIT` signal to
 dump the stacks of all running threads. The result is similar to the where mode.
 You can normally send a `SIGQUIT` signal with the <kbd>CTRL</kbd>+<kbd>\\</kbd>
 key combination.
 
 
+## Memory mode
+
+Besides wall time and CPU time, Echion can be used to profile memory
+allocations. In this mode, Echion tracks the Python memory domain allocators and
+accounts for each single event. Because of the tracing nature, this mode
+introduces considerable overhead, but gives pretty accurate results that can be
+used to investigate potential memory leaks. To fully understand that data that
+is collected in this mode, one should be aware of how Echion tracks allocations
+and deallocations. When an allocation is made, Echion records the frame stack
+that was involved and maps it to the returned memory address. When a
+deallocation for a tracked memory address is made, the freed memory is accounted
+for the same stack. Therefore, objects that are allocated and deallocated during
+the tracking period account for a total of 0 allocated bytes. This means that
+all the non-negative values reported by Echion represent memory that was still
+allocated by the time the tracking ended.
+
+*Since Echion 0.3.0*.
+
+
 ## Why Echion?
 
 Sampling in-process comes with some benefits. One has easier access to more
 information, like thread names, and potentially the task abstraction of async
 frameworks, like `asyncio`, `gevent`, ... . Also available is more accurate
 per-thread CPU timing information.
```

### Comparing `echion-0.2.0/art/logo.png` & `echion-0.3.0/art/logo.png`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/echion/__main__.py` & `echion-0.3.0/echion/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,42 +83,59 @@
         detach(pid)
 
     finally:
         if args.where and pipe_name is not None and pipe_name.exists():
             pipe_name.unlink()
 
 
+def microseconds(v: str) -> int:
+    try:
+        if v.endswith("ms"):
+            return int(v[:-2]) * 1000
+        if v.endswith("s"):
+            return int(v[:-1]) * 1000000
+        return int(v)
+    except Exception as e:
+        raise ValueError("Invalid interval: %s" % v) from e
+
+
 def main() -> None:
     parser = argparse.ArgumentParser(
         description="In-process CPython frame stack sampler",
         prog="echion",
     )
     parser.add_argument(
         "command", nargs=argparse.REMAINDER, type=str, help="Command string to execute."
     )
     parser.add_argument(
         "-i",
         "--interval",
         help="sampling interval in microseconds",
         default=1000,
-        type=int,
+        type=microseconds,
     )
     parser.add_argument(
         "-c",
         "--cpu",
         help="sample on-CPU stacks only",
         action="store_true",
     )
     parser.add_argument(
         "-x",
         "--exposure",
         help="exposure time, in seconds",
         type=int,
     )
     parser.add_argument(
+        "-m",
+        "--memory",
+        help="Collect memory allocation events",
+        action="store_true",
+    )
+    parser.add_argument(
         "-n",
         "--native",
         help="sample native stacks",
         action="store_true",
     )
     parser.add_argument(
         "-o",
@@ -153,22 +170,29 @@
     )
     parser.add_argument(
         "-V",
         "--version",
         action="version",
         version="%(prog)s " + __version__,
     )
-    args = parser.parse_args()
+
+    try:
+        args = parser.parse_args()
+    except Exception as e:
+        print("echion: %s" % e)
+        parser.print_usage()
+        sys.exit(1)
 
     # TODO: Validate arguments
 
     env = os.environ.copy()
 
     env["ECHION_INTERVAL"] = str(args.interval)
     env["ECHION_CPU"] = str(int(bool(args.cpu)))
+    env["ECHION_MEMORY"] = str(int(bool(args.memory)))
     env["ECHION_NATIVE"] = str(int(bool(args.native)))
     env["ECHION_OUTPUT"] = args.output.replace("%%(pid)", str(os.getpid()))
     env["ECHION_STEALTH"] = str(int(bool(args.stealth)))
     env["ECHION_WHERE"] = str(args.where or "")
 
     if args.pid or args.where:
         try:
```

### Comparing `echion-0.2.0/echion/bootstrap/__init__.py` & `echion-0.3.0/echion/bootstrap/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 def start():
     global do_on_fork
 
     # Set the configuration
     ec.set_interval(int(os.getenv("ECHION_INTERVAL", 1000)))
     ec.set_cpu(bool(int(os.getenv("ECHION_CPU", 0))))
+    ec.set_memory(bool(int(os.getenv("ECHION_MEMORY", 0))))
     ec.set_native(bool(int(os.getenv("ECHION_NATIVE", 0))))
     ec.set_where(bool(int(os.getenv("ECHION_WHERE", 0) or 0)))
 
     # Monkey-patch the standard library on import
     try:
         ModuleWatchdog.install()
         atexit.register(ModuleWatchdog.uninstall)
```

### Comparing `echion-0.2.0/echion/bootstrap/attach.py` & `echion-0.3.0/echion/bootstrap/attach.py`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/echion/bootstrap/sitecustomize.py` & `echion-0.3.0/echion/bootstrap/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/echion/cache.h` & `echion-0.3.0/echion/cache.h`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/echion/config.h` & `echion-0.3.0/echion/config.h`

 * *Files 14% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 // Sampling interval
 static unsigned int interval = 1000;
 
 // CPU Time mode
 static int cpu = 0;
 
-// Output stream
-static std::ofstream output;
+// Memory events
+static int memory = 0;
 
 // Native stack sampling
 static int native = 0;
 
 // Where mode
 static int where = 0;
 
@@ -53,14 +53,27 @@
     cpu = new_cpu;
 
     Py_RETURN_NONE;
 }
 
 // ----------------------------------------------------------------------------
 static PyObject *
+set_memory(PyObject *Py_UNUSED(m), PyObject *args)
+{
+    int new_memory;
+    if (!PyArg_ParseTuple(args, "p", &new_memory))
+        return NULL;
+
+    memory = new_memory;
+
+    Py_RETURN_NONE;
+}
+
+// ----------------------------------------------------------------------------
+static PyObject *
 set_native(PyObject *Py_UNUSED(m), PyObject *args)
 {
     int new_native;
     if (!PyArg_ParseTuple(args, "p", &new_native))
         return NULL;
 
     native = new_native;
```

### Comparing `echion-0.2.0/echion/core.pyi` & `echion-0.3.0/echion/core.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -17,10 +17,11 @@
 def init_asyncio(
     threads: list, scheduled_tasks: set, eager_tasks: set | None
 ) -> None: ...
 
 # Configuration interface
 def set_interval(interval: int) -> None: ...
 def set_cpu(cpu: bool) -> None: ...
+def set_memory(memory: bool) -> None: ...
 def set_native(native: bool) -> None: ...
 def set_where(where: bool) -> None: ...
 def set_pipe_name(name: str) -> None: ...
```

### Comparing `echion-0.2.0/echion/coremodule.cc` & `echion-0.3.0/echion/coremodule.cc`

 * *Files 5% similar despite different names*

```diff
@@ -23,40 +23,47 @@
 #include <sys/stat.h>
 #include <unistd.h>
 #if defined PL_DARWIN
 #include <pthread.h>
 #endif
 
 #include <echion/config.h>
+#include <echion/interp.h>
+#include <echion/memory.h>
+#include <echion/mojo.h>
 #include <echion/signals.h>
 #include <echion/stacks.h>
 #include <echion/state.h>
 #include <echion/threads.h>
 #include <echion/timing.h>
 
 // ----------------------------------------------------------------------------
 static void do_where(std::ostream &stream)
 {
     stream << "\r"
            << "🐴 Echion reporting for duty" << std::endl
            << std::endl;
 
-    // TODO: Add support for tasks
-    for_each_thread(
-        [&stream](PyThreadState *tstate, ThreadInfo &thread) -> void
+    for_each_interp(
+        [&stream](PyInterpreterState *interp) -> void
         {
-            thread.unwind(tstate);
-            if (native)
-            {
-                interleave_stacks();
-                thread.render_where(interleaved_stack, stream);
-            }
-            else
-                thread.render_where(python_stack, stream);
-            stream << std::endl;
+            for_each_thread(
+                interp,
+                [&stream](PyThreadState *tstate, ThreadInfo &thread) -> void
+                {
+                    thread.unwind(tstate);
+                    if (native)
+                    {
+                        interleave_stacks();
+                        thread.render_where(interleaved_stack, stream);
+                    }
+                    else
+                        thread.render_where(python_stack, stream);
+                    stream << std::endl;
+                });
         });
 }
 
 // ----------------------------------------------------------------------------
 static void where_listener()
 {
     for (;;)
@@ -95,122 +102,154 @@
 
 // ----------------------------------------------------------------------------
 static inline void
 _start()
 {
     init_frame_cache(MAX_FRAMES * (1 + native));
 
+    try
+    {
+        mojo.open();
+    }
+    catch (MojoWriter::Error &)
+    {
+        return;
+    }
+
     install_signals();
 
 #if defined PL_DARWIN
     // Get the wall time clock resource.
     host_get_clock_service(mach_host_self(), CALENDAR_CLOCK, &cclock);
 #endif
+
+    if (where)
+    {
+        std::ofstream pipe(pipe_name, std::ios::out);
+
+        if (pipe)
+            do_where(pipe);
+
+        else
+            std::cerr << "Failed to open pipe " << pipe_name << std::endl;
+
+        running = 0;
+
+        return;
+    }
+
+    setup_where();
+
+    mojo.header();
+
+    if (memory)
+    {
+        mojo.metadata("mode", "memory");
+    }
+    else
+    {
+        mojo.metadata("mode", (cpu ? "cpu" : "wall"));
+    }
+    mojo.metadata("interval", std::to_string(interval));
+    mojo.metadata("sampler", "echion");
+
+    // DEV: Workaround for the austin-python library: we send an empty sample
+    // to set the PID. We also map the key value 0 to the empty string, to
+    // support task name frames.
+    mojo.stack(pid, 0, "MainThread");
+    mojo.string(0, "");
+    mojo.string(1, "<invalid>");
+    mojo.string(2, "<unknown>");
+    mojo.metric_time(0);
+
+    if (memory)
+        setup_memory();
 }
 
 // ----------------------------------------------------------------------------
 static inline void
 _stop()
 {
+    if (memory)
+        teardown_memory();
+
     // Clean up the thread info map. When not running async, we need to guard
     // the map lock because we are not in control of the sampling thread.
     {
         const std::lock_guard<std::mutex> guard(thread_info_map_lock);
 
         thread_info_map.clear();
+        string_table.clear();
     }
 
+    teardown_where();
+
 #if defined PL_DARWIN
     mach_port_deallocate(mach_task_self(), cclock);
 #endif
 
     restore_signals();
 
+    mojo.close();
+
     reset_frame_cache();
 }
 
 // ----------------------------------------------------------------------------
 static inline void
 _sampler()
 {
     // This function can run without the GIL on the basis that these assumptions
     // hold:
     // 1. The interpreter state object lives as long as the process itself.
 
-    if (where)
-    {
-        std::ofstream pipe(pipe_name, std::ios::out);
-
-        if (pipe)
-            do_where(pipe);
-
-        else
-            std::cerr << "Failed to open pipe " << pipe_name << std::endl;
-
-        running = 0;
-
-        return;
-    }
-
-    setup_where();
-
     last_time = gettime();
 
-    output.open(std::getenv("ECHION_OUTPUT"));
-    if (!output.is_open())
-    {
-        std::cerr << "Failed to open output file " << std::getenv("ECHION_OUTPUT") << std::endl;
-        return;
-    }
-
-    output << "# mode: " << (cpu ? "cpu" : "wall") << std::endl;
-    output << "# interval: " << interval << std::endl;
-
-    // Install the signal handler if we are sampling the native stacks.
-    if (native)
-        // We use SIGPROF to sample the stacks within each thread.
-        signal(SIGPROF, sigprof_handler);
-
     while (running)
     {
         microsecond_t now = gettime();
         microsecond_t end_time = now + interval;
-        microsecond_t wall_time = now - last_time;
 
-        for_each_thread(
-            [=](PyThreadState *tstate, ThreadInfo &thread)
-            { thread.sample(tstate, wall_time); });
+        if (memory)
+        {
+            if (rss_tracker.check())
+                stack_stats.flush();
+        }
+        else
+        {
+            microsecond_t wall_time = now - last_time;
+
+            for_each_interp(
+                [=](PyInterpreterState *interp) -> void
+                {
+                    for_each_thread(
+                        interp,
+                        [=](PyThreadState *tstate, ThreadInfo &thread)
+                        { thread.sample(interp->id, tstate, wall_time); });
+                });
+        }
 
         while (gettime() < end_time && running)
             sched_yield();
 
         last_time = now;
     }
-
-    output.close();
-
-    teardown_where();
 }
 
 static void
 sampler()
 {
     _start();
     _sampler();
     _stop();
 }
 
 // ----------------------------------------------------------------------------
 static void _init()
 {
-#if PY_VERSION_HEX >= 0x03090000
-    interp = PyInterpreterState_Get();
-#else
-    interp = _PyInterpreterState_Get();
-#endif
     pid = getpid();
 }
 
 // ----------------------------------------------------------------------------
 static PyObject *
 start_async(PyObject *Py_UNUSED(m), PyObject *Py_UNUSED(args))
 {
@@ -273,30 +312,23 @@
 
     if (!PyArg_ParseTuple(args, "lsi", &thread_id, &thread_name, &native_id))
         return NULL;
 
     {
         const std::lock_guard<std::mutex> guard(thread_info_map_lock);
 
-        if (thread_info_map.find(thread_id) != thread_info_map.end())
-        {
+        auto entry = thread_info_map.find(thread_id);
+        if (entry != thread_info_map.end())
             // Thread is already tracked so we update its info
-            auto &thread = *thread_info_map.find(thread_id)->second;
-
-            thread.name = thread_name;
-            thread.native_id = native_id;
-            thread.update_cpu_time();
-        }
+            entry->second = std::make_unique<ThreadInfo>(thread_id, native_id, thread_name);
         else
-        {
-            // Untracked thread. Create a new info entry.
+            // Thread is already tracked so we update its info
             thread_info_map.emplace(
                 thread_id,
                 std::make_unique<ThreadInfo>(thread_id, native_id, thread_name));
-        }
     }
 
     Py_RETURN_NONE;
 }
 
 // ----------------------------------------------------------------------------
 static PyObject *
@@ -390,14 +422,15 @@
     // Task support
     {"track_asyncio_loop", track_asyncio_loop, METH_VARARGS, "Map the name of a task with its identifier"},
     {"init_asyncio", init_asyncio, METH_VARARGS, "Initialise asyncio tracking"},
     {"link_tasks", link_tasks, METH_VARARGS, "Link two tasks"},
     // Configuration interface
     {"set_interval", set_interval, METH_VARARGS, "Set the sampling interval"},
     {"set_cpu", set_cpu, METH_VARARGS, "Set whether to use CPU time instead of wall time"},
+    {"set_memory", set_memory, METH_VARARGS, "Set whether to sample memory usage"},
     {"set_native", set_native, METH_VARARGS, "Set whether to sample the native stacks"},
     {"set_where", set_where, METH_VARARGS, "Set whether to use where mode"},
     {"set_pipe_name", set_pipe_name, METH_VARARGS, "Set the pipe name"},
     {NULL, NULL, 0, NULL} /* Sentinel */
 };
 
 // ----------------------------------------------------------------------------
```

### Comparing `echion-0.2.0/echion/cpython/tasks.h` & `echion-0.3.0/echion/cpython/tasks.h`

 * *Files 5% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         }
 
         return yf;
     }
 
 #elif PY_VERSION_HEX >= 0x030a0000
     PyObject *
-    PyGen_yf(PyGenObject *gen, PyObject *frame_addr)
+    PyGen_yf(PyGenObject *Py_UNUSED(gen), PyObject *frame_addr)
     {
         PyObject *yf = NULL;
         PyFrameObject *f = (PyFrameObject *)frame_addr;
 
         if (f)
         {
             PyFrameObject frame;
@@ -216,15 +216,15 @@
         }
 
         return yf;
     }
 
 #else
     PyObject *
-    PyGen_yf(PyGenObject *gen, PyObject *frame_addr)
+    PyGen_yf(PyGenObject *Py_UNUSED(gen), PyObject *frame_addr)
     {
         PyObject *yf = NULL;
         PyFrameObject *f = (PyFrameObject *)frame_addr;
 
         if (frame_addr == NULL)
             return NULL;
```

### Comparing `echion-0.2.0/echion/frame.h` & `echion-0.3.0/echion/frame.h`

 * *Files 24% similar despite different names*

```diff
@@ -19,409 +19,519 @@
 #include <iostream>
 
 #include <cxxabi.h>
 #define UNW_LOCAL_ONLY
 #include <libunwind.h>
 
 #include <echion/cache.h>
+#include <echion/mojo.h>
 #include <echion/strings.h>
 #include <echion/vm.h>
 
-#define MOJO_INT32 ((uintptr_t)(1 << (6 + 7 * 3)) - 1)
+// ----------------------------------------------------------------------------
+#if PY_VERSION_HEX >= 0x030b0000
+static inline int
+_read_varint(unsigned char *table, ssize_t size, ssize_t *i)
+{
+    ssize_t guard = size - 1;
+    if (*i >= guard)
+        return 0;
+
+    int val = table[++*i] & 63;
+    int shift = 0;
+    while (table[*i] & 64 && *i < guard)
+    {
+        shift += 6;
+        val |= (table[++*i] & 63) << shift;
+    }
+    return val;
+}
+
+// ----------------------------------------------------------------------------
+static inline int
+_read_signed_varint(unsigned char *table, ssize_t size, ssize_t *i)
+{
+    int val = _read_varint(table, size, i);
+    return (val & 1) ? -(val >> 1) : (val >> 1);
+}
+#endif
 
+// ----------------------------------------------------------------------------
 class Frame
 {
 public:
-    typedef std::reference_wrapper<Frame> Ref;
-    typedef std::unique_ptr<Frame> Ptr;
+    using Ref = std::reference_wrapper<Frame>;
+    using Ptr = std::unique_ptr<Frame>;
+    using Key = uintptr_t;
 
+    // ------------------------------------------------------------------------
     class Error : public std::exception
     {
     public:
         const char *what() const noexcept override
         {
             return "Cannot read frame";
         }
     };
 
+    // ------------------------------------------------------------------------
     class LocationError : public Error
     {
     public:
         const char *what() const noexcept override
         {
             return "Cannot determine frame location information";
         }
     };
 
-    std::string filename = "";
-    std::string name = "";
+    // ------------------------------------------------------------------------
+
+    Key cache_key = 0;
+    StringTable::Key filename = 0;
+    StringTable::Key name = 0;
 
     struct _location
     {
         int line = 0;
         int line_end = 0;
         int column = 0;
         int column_end = 0;
     } location;
+
 #if PY_VERSION_HEX >= 0x030b0000
     bool is_entry = false;
 #endif
 
-    void render(std::ostream &stream)
+    // ------------------------------------------------------------------------
+
+    Frame(StringTable::Key name) : name(name){};
+
+    static Frame &read(PyObject *frame_addr, PyObject **prev_addr);
+
+    static Frame &get(PyCodeObject *code_addr, int lasti);
+    static Frame &get(PyObject *frame);
+    static Frame &get(unw_cursor_t &cursor);
+    static Frame &get(StringTable::Key name);
+
+    // ------------------------------------------------------------------------
+    Frame(PyObject *frame)
     {
-        stream << ";" << filename << ":" << name << ":" << location.line;
+#if PY_VERSION_HEX >= 0x030b0000
+        const _PyInterpreterFrame *iframe = (_PyInterpreterFrame *)frame;
+        const int lasti = _PyInterpreterFrame_LASTI(iframe);
+        PyCodeObject *code = iframe->f_code;
+
+        PyCode_Addr2Location(code, lasti << 1, &location.line, &location.column, &location.line_end, &location.column_end);
+        location.column++;
+        location.column_end++;
+        name = string_table.key_unsafe(code->co_qualname);
+#if PY_VERSION_HEX >= 0x030c0000
+        is_entry = (iframe->owner == FRAME_OWNED_BY_CSTACK); // Shim frame
+#else
+        is_entry = iframe->is_entry;
+#endif
+
+#else
+        PyFrameObject *py_frame = (PyFrameObject *)frame;
+        const int lasti = py_frame->f_lasti;
+        PyCodeObject *code = py_frame->f_code;
+
+        location.line = PyFrame_GetLineNumber(py_frame);
+        name = string_table.key_unsafe(code->co_name);
+#endif
+        filename = string_table.key_unsafe(code->co_filename);
     }
 
+    // ------------------------------------------------------------------------
+    Frame(PyCodeObject *code, int lasti)
+    {
+        try
+        {
+            filename = string_table.key(code->co_filename);
+#if PY_VERSION_HEX >= 0x030b0000
+            name = string_table.key(code->co_qualname);
+#else
+            name = string_table.key(code->co_name);
+#endif
+        }
+        catch (StringTable::Error &)
+        {
+            throw Error();
+        }
+
+        infer_location(code, lasti);
+    }
+
+    // ------------------------------------------------------------------------
+    Frame(unw_cursor_t &cursor, unw_word_t pc)
+    {
+        try
+        {
+            filename = string_table.key(pc);
+            name = string_table.key(cursor);
+        }
+        catch (StringTable::Error &)
+        {
+            throw Error();
+        }
+    }
+
+    // ------------------------------------------------------------------------
+    void inline render(std::ostream &stream)
+    {
+        stream
+            << ";" << string_table.lookup(filename)
+            << ":" << string_table.lookup(name)
+            << ":" << location.line;
+    }
+
+    // ------------------------------------------------------------------------
     void render_where(std::ostream &stream)
     {
-        if ((filename).rfind("native@", 0) == 0)
-            stream << "          \033[38;5;248;1m" << name
-                   << "\033[0m \033[38;5;246m(" << filename
+        if ((string_table.lookup(filename)).rfind("native@", 0) == 0)
+            stream << "          \033[38;5;248;1m" << string_table.lookup(name)
+                   << "\033[0m \033[38;5;246m(" << string_table.lookup(filename)
                    << "\033[0m:\033[38;5;246m" << location.line
                    << ")\033[0m" << std::endl;
         else
-            stream << "          \033[33;1m" << name
-                   << "\033[0m (\033[36m" << filename
+            stream << "          \033[33;1m" << string_table.lookup(name)
+                   << "\033[0m (\033[36m" << string_table.lookup(filename)
                    << "\033[0m:\033[32m" << location.line
                    << "\033[0m)" << std::endl;
     }
 
-    Frame(const char *name) : name({std::string(name)}){};
-    Frame(std::string &name) : name(name){};
-
-    static Frame &read(PyObject *, PyObject **);
+    // ------------------------------------------------------------------------
     static Frame &read(PyObject *frame_addr)
     {
         PyObject *unused;
-        return Frame::read(frame_addr, &unused);
+        return read(frame_addr, &unused);
     }
 
-    static Frame &get(PyCodeObject *code, int lasti);
-    static Frame &get(unw_word_t pc, const char *name, unw_word_t offset);
-    static Frame &get(PyObject *, std::string &);
-
-    Frame(PyCodeObject *, int);
-    Frame(unw_word_t, const char *, unw_word_t);
-
 private:
-    void infer_location(PyCodeObject *, int);
-
-    static inline uintptr_t key(PyCodeObject *code, int lasti)
+    // ------------------------------------------------------------------------
+    void inline infer_location(PyCodeObject *code, int lasti)
     {
-        return (((uintptr_t)(((uintptr_t)code) & MOJO_INT32) << 16) | lasti);
-    }
-};
-
-#if PY_VERSION_HEX >= 0x030b0000
-// ----------------------------------------------------------------------------
-static inline int
-_read_varint(unsigned char *table, ssize_t size, ssize_t *i)
-{
-    ssize_t guard = size - 1;
-    if (*i >= guard)
-        return 0;
-
-    int val = table[++*i] & 63;
-    int shift = 0;
-    while (table[*i] & 64 && *i < guard)
-    {
-        shift += 6;
-        val |= (table[++*i] & 63) << shift;
-    }
-    return val;
-}
-
-// ----------------------------------------------------------------------------
-static inline int
-_read_signed_varint(unsigned char *table, ssize_t size, ssize_t *i)
-{
-    int val = _read_varint(table, size, i);
-    return (val & 1) ? -(val >> 1) : (val >> 1);
-}
-#endif
-
-// ----------------------------------------------------------------------------
-void Frame::infer_location(PyCodeObject *code, int lasti)
-{
-    unsigned int lineno = code->co_firstlineno;
-    Py_ssize_t len = 0;
+        unsigned int lineno = code->co_firstlineno;
+        Py_ssize_t len = 0;
 
 #if PY_VERSION_HEX >= 0x030b0000
-    auto table = pybytes_to_bytes_and_size(code->co_linetable, &len);
-    if (table == nullptr)
-        throw LocationError();
+        auto table = pybytes_to_bytes_and_size(code->co_linetable, &len);
+        if (table == nullptr)
+            throw LocationError();
 
-    auto table_data = table.get();
+        auto table_data = table.get();
 
-    for (Py_ssize_t i = 0, bc = 0; i < len; i++)
-    {
-        bc += (table[i] & 7) + 1;
-        int code = (table[i] >> 3) & 15;
-        unsigned char next_byte = 0;
-        switch (code)
+        for (Py_ssize_t i = 0, bc = 0; i < len; i++)
         {
-        case 15:
-            break;
-
-        case 14: // Long form
-            lineno += _read_signed_varint(table_data, len, &i);
-
-            this->location.line = lineno;
-            this->location.line_end = lineno + _read_varint(table_data, len, &i);
-            this->location.column = _read_varint(table_data, len, &i);
-            this->location.column_end = _read_varint(table_data, len, &i);
-
-            break;
-
-        case 13: // No column data
-            lineno += _read_signed_varint(table_data, len, &i);
-
-            this->location.line = lineno;
-            this->location.line_end = lineno;
-            this->location.column = this->location.column_end = 0;
-
-            break;
+            bc += (table[i] & 7) + 1;
+            int code = (table[i] >> 3) & 15;
+            unsigned char next_byte = 0;
+            switch (code)
+            {
+            case 15:
+                break;
+
+            case 14: // Long form
+                lineno += _read_signed_varint(table_data, len, &i);
+
+                this->location.line = lineno;
+                this->location.line_end = lineno + _read_varint(table_data, len, &i);
+                this->location.column = _read_varint(table_data, len, &i);
+                this->location.column_end = _read_varint(table_data, len, &i);
+
+                break;
+
+            case 13: // No column data
+                lineno += _read_signed_varint(table_data, len, &i);
+
+                this->location.line = lineno;
+                this->location.line_end = lineno;
+                this->location.column = this->location.column_end = 0;
+
+                break;
+
+            case 12: // New lineno
+            case 11:
+            case 10:
+                if (i >= len - 2)
+                    throw LocationError();
+
+                lineno += code - 10;
+
+                this->location.line = lineno;
+                this->location.line_end = lineno;
+                this->location.column = 1 + table[++i];
+                this->location.column_end = 1 + table[++i];
+
+                break;
+
+            default:
+                if (i >= len - 1)
+                    throw LocationError();
+
+                next_byte = table[++i];
+
+                this->location.line = lineno;
+                this->location.line_end = lineno;
+                this->location.column = 1 + (code << 3) + ((next_byte >> 4) & 7);
+                this->location.column_end = this->location.column + (next_byte & 15);
+            }
 
-        case 12: // New lineno
-        case 11:
-        case 10:
-            if (i >= len - 2)
-                throw LocationError();
+            if (bc > lasti)
+                break;
+        }
 
-            lineno += code - 10;
+#elif PY_VERSION_HEX >= 0x030a0000
+        auto table = pybytes_to_bytes_and_size(code->co_linetable, &len);
+        if (table == nullptr)
+            throw LocationError();
 
-            this->location.line = lineno;
-            this->location.line_end = lineno;
-            this->location.column = 1 + table[++i];
-            this->location.column_end = 1 + table[++i];
+        lasti <<= 1;
+        for (int i = 0, bc = 0; i < len; i++)
+        {
+            int sdelta = table[i++];
+            if (sdelta == 0xff)
+                break;
+
+            bc += sdelta;
+
+            int ldelta = table[i];
+            if (ldelta == 0x80)
+                ldelta = 0;
+            else if (ldelta > 0x80)
+                lineno -= 0x100;
+
+            lineno += ldelta;
+            if (bc > lasti)
+                break;
+        }
 
-            break;
+#else
+        auto table = pybytes_to_bytes_and_size(code->co_lnotab, &len);
+        if (table == nullptr)
+            throw LocationError();
 
-        default:
-            if (i >= len - 1)
-                throw LocationError();
+        for (int i = 0, bc = 0; i < len; i++)
+        {
+            bc += table[i++];
+            if (bc > lasti)
+                break;
 
-            next_byte = table[++i];
+            if (table[i] >= 0x80)
+                lineno -= 0x100;
 
-            this->location.line = lineno;
-            this->location.line_end = lineno;
-            this->location.column = 1 + (code << 3) + ((next_byte >> 4) & 7);
-            this->location.column_end = this->location.column + (next_byte & 15);
+            lineno += table[i];
         }
 
-        if (bc > lasti)
-            break;
-    }
+#endif
 
-#elif PY_VERSION_HEX >= 0x030a0000
-    auto table = pybytes_to_bytes_and_size(code->co_linetable, &len);
-    if (table == nullptr)
-        throw LocationError();
-
-    lasti <<= 1;
-    for (int i = 0, bc = 0; i < len; i++)
-    {
-        int sdelta = table[i++];
-        if (sdelta == 0xff)
-            break;
-
-        bc += sdelta;
-
-        int ldelta = table[i];
-        if (ldelta == 0x80)
-            ldelta = 0;
-        else if (ldelta > 0x80)
-            lineno -= 0x100;
-
-        lineno += ldelta;
-        if (bc > lasti)
-            break;
+        this->location.line = lineno;
+        this->location.line_end = lineno;
+        this->location.column = 0;
+        this->location.column_end = 0;
     }
 
-#else
-    auto table = pybytes_to_bytes_and_size(code->co_lnotab, &len);
-    if (table == nullptr)
-        throw LocationError();
-
-    for (int i = 0, bc = 0; i < len; i++)
+    // ------------------------------------------------------------------------
+    static inline Key key(PyCodeObject *code, int lasti)
     {
-        bc += table[i++];
-        if (bc > lasti)
-            break;
-
-        if (table[i] >= 0x80)
-            lineno -= 0x100;
-
-        lineno += table[i];
+        return (((uintptr_t)(((uintptr_t)code) & MOJO_INT32) << 16) | lasti);
     }
 
-#endif
-
-    this->location.line = lineno;
-    this->location.line_end = lineno;
-    this->location.column = 0;
-    this->location.column_end = 0;
-}
-
-// ----------------------------------------------------------------------------
-Frame::Frame(PyCodeObject *code, int lasti)
-{
-    try
+    // ------------------------------------------------------------------------
+    static inline Key key(PyObject *frame)
     {
-        filename = pyunicode_to_utf8(code->co_filename);
 #if PY_VERSION_HEX >= 0x030b0000
-        name = pyunicode_to_utf8(code->co_qualname);
+        const _PyInterpreterFrame *iframe = (_PyInterpreterFrame *)frame;
+        const int lasti = _PyInterpreterFrame_LASTI(iframe);
+        PyCodeObject *code = iframe->f_code;
 #else
-        name = pyunicode_to_utf8(code->co_name);
+        const PyFrameObject *py_frame = (PyFrameObject *)frame;
+        const int lasti = py_frame->f_lasti;
+        PyCodeObject *code = py_frame->f_code;
 #endif
+        return key(code, lasti);
     }
-    catch (StringError &)
-    {
-        throw Error();
-    }
-
-    infer_location(code, lasti);
-}
-
-Frame::Frame(unw_word_t pc, const char *name, unw_word_t offset)
-{
-    filename = std::string(32, '\0');
-    std::snprintf((char *)filename.c_str(), 32, "native@%p", (void *)pc);
-
-    // Try to demangle C++ names
-    char *demangled = NULL;
-    if (name[0] == '_' && name[1] == 'Z')
-    {
-        int status;
-        demangled = abi::__cxa_demangle(name, NULL, NULL, &status);
-        if (status == 0)
-            name = demangled;
-    }
-
-    // Make a copy
-    this->name = std::string(name);
-
-    if (demangled != NULL)
-        std::free(demangled);
-
-    location.line = offset;
-}
+};
 
 // ----------------------------------------------------------------------------
 
-static Frame INVALID_FRAME("<invalid>");
-static Frame UNKNOWN_FRAME("<unknown>");
+static auto INVALID_FRAME = Frame(StringTable::INVALID);
+static auto UNKNOWN_FRAME = Frame(StringTable::UNKNOWN);
 
 // We make this a raw pointer to prevent its destruction on exit, since we
 // control the lifetime of the cache.
 static LRUCache<uintptr_t, Frame> *frame_cache = nullptr;
 
+// ----------------------------------------------------------------------------
 static void init_frame_cache(size_t capacity)
 {
     frame_cache = new LRUCache<uintptr_t, Frame>(capacity);
 }
 
+// ----------------------------------------------------------------------------
 static void reset_frame_cache()
 {
     delete frame_cache;
     frame_cache = nullptr;
 }
 
+// ------------------------------------------------------------------------
+Frame &Frame::read(PyObject *frame_addr, PyObject **prev_addr)
+{
+#if PY_VERSION_HEX >= 0x030b0000
+    _PyInterpreterFrame iframe;
+
+    if (copy_type(frame_addr, iframe))
+        throw Error();
+
+    // We cannot use _PyInterpreterFrame_LASTI because _PyCode_CODE reads
+    // from the code object.
+    const int lasti = ((int)(iframe.prev_instr - (_Py_CODEUNIT *)(iframe.f_code))) - offsetof(PyCodeObject, co_code_adaptive) / sizeof(_Py_CODEUNIT);
+    auto &frame = Frame::get(iframe.f_code, lasti);
+
+    if (&frame != &INVALID_FRAME)
+    {
+#if PY_VERSION_HEX >= 0x030c0000
+        frame.is_entry = (iframe.owner == FRAME_OWNED_BY_CSTACK); // Shim frame
+#else
+        frame.is_entry = iframe.is_entry;
+#endif
+    }
+
+    *prev_addr = &frame == &INVALID_FRAME ? NULL : (PyObject *)iframe.previous;
+
+#else // Python < 3.11
+      // Unwind the stack from leaf to root and store it in a stack. This way we
+      // can print it from root to leaf.
+    PyFrameObject py_frame;
+
+    if (copy_type(frame_addr, py_frame))
+        throw Error();
+
+    auto &frame = Frame::get(py_frame.f_code, py_frame.f_lasti);
+
+    *prev_addr = (&frame == &INVALID_FRAME) ? NULL : (PyObject *)py_frame.f_back;
+#endif
+
+    return frame;
+}
+
+// ----------------------------------------------------------------------------
 Frame &Frame::get(PyCodeObject *code_addr, int lasti)
 {
     PyCodeObject code;
     if (copy_type(code_addr, code))
         return INVALID_FRAME;
 
-    uintptr_t frame_key = Frame::key(code_addr, lasti);
+    auto frame_key = Frame::key(code_addr, lasti);
 
     try
     {
         return frame_cache->lookup(frame_key);
     }
     catch (LRUCache<uintptr_t, Frame>::LookupError &)
     {
         try
         {
             auto new_frame = std::make_unique<Frame>(&code, lasti);
+            new_frame->cache_key = frame_key;
             auto &f = *new_frame;
+            mojo.frame(
+                frame_key,
+                new_frame->filename,
+                new_frame->name,
+                new_frame->location.line, new_frame->location.line_end,
+                new_frame->location.column, new_frame->location.column_end);
             frame_cache->store(frame_key, std::move(new_frame));
             return f;
         }
         catch (Frame::Error &)
         {
             return INVALID_FRAME;
         }
     }
 }
 
-Frame &Frame::get(unw_word_t pc, const char *name, unw_word_t offset)
+// ----------------------------------------------------------------------------
+Frame &Frame::get(PyObject *frame)
 {
-    uintptr_t frame_key = (uintptr_t)pc;
+    auto frame_key = Frame::key(frame);
+
     try
     {
         return frame_cache->lookup(frame_key);
     }
     catch (LRUCache<uintptr_t, Frame>::LookupError &)
     {
-        auto frame = std::make_unique<Frame>(pc, name, offset);
-        auto &f = *frame;
-        frame_cache->store(frame_key, std::move(frame));
+        auto new_frame = std::make_unique<Frame>(frame);
+        new_frame->cache_key = frame_key;
+        auto &f = *new_frame;
+        mojo.frame(
+            frame_key,
+            new_frame->filename,
+            new_frame->name,
+            new_frame->location.line, new_frame->location.line_end,
+            new_frame->location.column, new_frame->location.column_end);
+        frame_cache->store(frame_key, std::move(new_frame));
         return f;
     }
 }
 
-Frame &Frame::get(PyObject *origin, std::string &name)
+// ----------------------------------------------------------------------------
+Frame &Frame::get(unw_cursor_t &cursor)
 {
-    uintptr_t frame_key = (uintptr_t)origin;
+    unw_word_t pc;
+    unw_get_reg(&cursor, UNW_REG_IP, &pc);
+    if (pc == 0)
+        throw Error();
+
+    uintptr_t frame_key = (uintptr_t)pc;
     try
     {
         return frame_cache->lookup(frame_key);
     }
     catch (LRUCache<uintptr_t, Frame>::LookupError &)
     {
-        auto frame = std::make_unique<Frame>(name);
-        auto &f = *frame;
-        frame_cache->store(frame_key, std::move(frame));
-        return f;
+        try
+        {
+            auto frame = std::make_unique<Frame>(cursor, pc);
+            frame->cache_key = frame_key;
+            auto &f = *frame;
+            mojo.frame(
+                frame_key,
+                frame->filename,
+                frame->name,
+                frame->location.line, frame->location.line_end,
+                frame->location.column, frame->location.column_end);
+            frame_cache->store(frame_key, std::move(frame));
+            return f;
+        }
+        catch (Frame::Error &)
+        {
+            return UNKNOWN_FRAME;
+        }
     }
 }
 
-Frame &Frame::read(PyObject *frame_addr, PyObject **prev_addr)
+// ----------------------------------------------------------------------------
+Frame &Frame::get(StringTable::Key name)
 {
-#if PY_VERSION_HEX >= 0x030b0000
-    _PyInterpreterFrame iframe;
-
-    if (copy_type(frame_addr, iframe))
-        throw Error();
-
-    // We cannot use _PyInterpreterFrame_LASTI because _PyCode_CODE reads
-    // from the code object.
-    const int lasti = ((int)(iframe.prev_instr - (_Py_CODEUNIT *)(iframe.f_code))) - offsetof(PyCodeObject, co_code_adaptive) / sizeof(_Py_CODEUNIT);
-    auto &frame = Frame::get(iframe.f_code, lasti);
-
-    if (&frame != &INVALID_FRAME)
+    uintptr_t frame_key = (uintptr_t)name;
+    try
     {
-#if PY_VERSION_HEX >= 0x030c0000
-        frame.is_entry = (iframe.owner == FRAME_OWNED_BY_CSTACK); // Shim frame
-#else
-        frame.is_entry = iframe.is_entry;
-#endif
+        return frame_cache->lookup(frame_key);
+    }
+    catch (LRUCache<uintptr_t, Frame>::LookupError &)
+    {
+        auto frame = std::make_unique<Frame>(name);
+        frame->cache_key = frame_key;
+        auto &f = *frame;
+        mojo.frame(
+            frame_key,
+            frame->filename,
+            frame->name,
+            frame->location.line, frame->location.line_end,
+            frame->location.column, frame->location.column_end);
+        frame_cache->store(frame_key, std::move(frame));
+        return f;
     }
-
-    *prev_addr = &frame == &INVALID_FRAME ? NULL : (PyObject *)iframe.previous;
-
-#else // Python < 3.11
-    // Unwind the stack from leaf to root and store it in a stack. This way we
-    // can print it from root to leaf.
-    PyFrameObject py_frame;
-
-    if (copy_type(frame_addr, py_frame))
-        throw Error();
-
-    auto &frame = Frame::get(py_frame.f_code, py_frame.f_lasti);
-
-    *prev_addr = (&frame == &INVALID_FRAME) ? NULL : (PyObject *)py_frame.f_back;
-#endif
-
-    return frame;
 }
```

### Comparing `echion-0.2.0/echion/mirrors.h` & `echion-0.3.0/echion/mirrors.h`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/echion/module.py` & `echion-0.3.0/echion/module.py`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/echion/monkey/asyncio.py` & `echion-0.3.0/echion/monkey/asyncio.py`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/echion/monkey/threading.py` & `echion-0.3.0/echion/monkey/threading.py`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/echion/signals.h` & `echion-0.3.0/echion/signals.h`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/echion/stacks.h` & `echion-0.3.0/echion/stacks.h`

 * *Files 23% similar despite different names*

```diff
@@ -4,40 +4,67 @@
 
 #pragma once
 
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 
 #include <deque>
+#include <mutex>
+#include <unordered_map>
 #include <unordered_set>
 
 #define UNW_LOCAL_ONLY
 #include <libunwind.h>
 
 #include <echion/frame.h>
+#include <echion/mojo.h>
 
 #define MAX_FRAMES 2048
 
 class FrameStack : public std::deque<Frame::Ref>
 {
 public:
-    void render(std::ostream &output)
+    using Ptr = std::unique_ptr<FrameStack>;
+    using Key = Frame::Key;
+
+    // ------------------------------------------------------------------------
+    Key key()
+    {
+        Key h = 0;
+
+        for (auto it = this->begin(); it != this->end(); ++it)
+            h = rotl(h) ^ (*it).get().cache_key;
+
+        return h;
+    }
+
+    // ------------------------------------------------------------------------
+    void render()
     {
         for (auto it = this->rbegin(); it != this->rend(); ++it)
         {
 #if PY_VERSION_HEX >= 0x030c0000
             if ((*it).get().is_entry)
                 // This is a shim frame so we skip it.
                 continue;
 #endif
-            (*it).get().render(output);
+            mojo.frame_ref((*it).get().cache_key);
         }
     }
+
+private:
+    // ------------------------------------------------------------------------
+    static inline Frame::Key rotl(Key key)
+    {
+        return (key << 1) | (key >> (CHAR_BIT * sizeof(key) - 1));
+    }
 };
 
+// ----------------------------------------------------------------------------
+
 static FrameStack python_stack;
 static FrameStack native_stack;
 static FrameStack interleaved_stack;
 
 // ----------------------------------------------------------------------------
 void unwind_native_stack()
 {
@@ -47,27 +74,22 @@
     unw_getcontext(&context);
     unw_init_local(&cursor, &context);
 
     native_stack.clear();
 
     while (unw_step(&cursor) > 0 && native_stack.size() < MAX_FRAMES)
     {
-        unw_word_t offset, pc;
-        unw_get_reg(&cursor, UNW_REG_IP, &pc);
-        if (pc == 0)
+        try
+        {
+            native_stack.push_back(Frame::get(cursor));
+        }
+        catch (Frame::Error &)
         {
-            // TODO: Invalid stack
             break;
         }
-
-        char sym[256];
-        native_stack.push_back(
-            unw_get_proc_name(&cursor, sym, sizeof(sym), &offset)
-                ? UNKNOWN_FRAME
-                : Frame::get(pc, sym, offset));
     }
 }
 
 // ----------------------------------------------------------------------------
 static size_t
 unwind_frame(PyObject *frame_addr, FrameStack &stack)
 {
@@ -97,19 +119,47 @@
         }
     }
 
     return count;
 }
 
 // ----------------------------------------------------------------------------
+static size_t
+unwind_frame_unsafe(PyObject *frame, FrameStack &stack)
+{
+    std::unordered_set<PyObject *> seen_frames; // Used to detect cycles in the stack
+    int count = 0;
+
+    PyObject *current_frame = frame;
+    while (current_frame != NULL && stack.size() < MAX_FRAMES)
+    {
+
+        if (seen_frames.find(current_frame) != seen_frames.end())
+            break;
+
+        count++;
+
+        seen_frames.insert(current_frame);
+
+        stack.push_back(Frame::get(current_frame));
+
+#if PY_VERSION_HEX >= 0x030b0000
+        current_frame = (PyObject *)((_PyInterpreterFrame *)current_frame)->previous;
+#else
+        current_frame = (PyObject *)((PyFrameObject *)current_frame)->f_back;
+#endif
+    }
+
+    return count;
+}
+
+// ----------------------------------------------------------------------------
 static void
 unwind_python_stack(PyThreadState *tstate, FrameStack &stack)
 {
-    std::unordered_set<void *> seen_frames; // Used to detect cycles in the stack
-
     stack.clear();
 
 #if PY_VERSION_HEX >= 0x030b0000
     _PyCFrame cframe;
     _PyCFrame *cframe_addr = tstate->cframe;
     if (copy_type(cframe_addr, cframe))
         // TODO: Invalid frame
@@ -120,14 +170,28 @@
     PyObject *frame_addr = (PyObject *)tstate->frame;
 #endif
     unwind_frame(frame_addr, stack);
 }
 
 // ----------------------------------------------------------------------------
 static void
+unwind_python_stack_unsafe(PyThreadState *tstate, FrameStack &stack)
+{
+    stack.clear();
+
+#if PY_VERSION_HEX >= 0x030b0000
+    PyObject *frame_addr = (PyObject *)tstate->cframe->current_frame;
+#else // Python < 3.11
+    PyObject *frame_addr = (PyObject *)tstate->frame;
+#endif
+    unwind_frame_unsafe(frame_addr, stack);
+}
+
+// ----------------------------------------------------------------------------
+static void
 unwind_python_stack(PyThreadState *tstate)
 {
     unwind_python_stack(tstate, python_stack);
 }
 
 // ----------------------------------------------------------------------------
 static void
@@ -138,15 +202,15 @@
     auto p = python_stack.rbegin();
     // The last two frames are usually the signal trampoline and the signal
     // handler. We skip them.
     for (auto n = native_stack.rbegin(); n != native_stack.rend() - 2; ++n)
     {
         auto native_frame = *n;
 
-        if (native_frame.get().name.find("PyEval_EvalFrameDefault") != std::string::npos)
+        if (string_table.lookup(native_frame.get().name).find("PyEval_EvalFrameDefault") != std::string::npos)
         {
             if (p == python_stack.rend())
             {
                 // We expected a Python frame but we found none, so we report
                 // the native frame instead.
                 std::cerr << "Expected Python frame(s), found none!" << std::endl;
                 interleaved_stack.push_front(native_frame);
@@ -187,7 +251,60 @@
 
 // ----------------------------------------------------------------------------
 static void
 interleave_stacks()
 {
     interleave_stacks(python_stack);
 }
+
+// ----------------------------------------------------------------------------
+// This table is used to store entire stacks and index them by key. This is
+// used when profiling memory events to account for deallocations.
+class StackTable
+{
+public:
+    // ------------------------------------------------------------------------
+    FrameStack::Key inline store(FrameStack::Ptr stack)
+    {
+        std::lock_guard<std::mutex> lock(this->lock);
+
+        auto stack_key = stack->key();
+
+        auto stack_entry = table.find(stack_key);
+        if (stack_entry == table.end())
+        {
+            table.emplace(stack_key, std::move(stack));
+        }
+        else
+        {
+            // TODO: Check for collisions.
+        }
+
+        return stack_key;
+    }
+
+    // ------------------------------------------------------------------------
+    FrameStack &retrieve(FrameStack::Key stack_key)
+    {
+        std::lock_guard<std::mutex> lock(this->lock);
+
+        return *table.find(stack_key)->second;
+    }
+
+    // ------------------------------------------------------------------------
+    void clear()
+    {
+        std::lock_guard<std::mutex> lock(this->lock);
+
+        table.clear();
+    }
+
+private:
+    std::unordered_map<FrameStack::Key, std::unique_ptr<FrameStack>> table;
+    std::mutex lock;
+};
+
+// ----------------------------------------------------------------------------
+// We make this a reference to a heap-allocated object so that we can avoid
+// the destruction on exit. We are in charge of cleaning up the object. Note
+// that the object will leak, but this is not a problem.
+static auto &stack_table = *(new StackTable());
```

### Comparing `echion-0.2.0/echion/tasks.h` & `echion-0.3.0/echion/tasks.h`

 * *Files 4% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     };
 
     PyObject *origin = NULL;
     PyObject *loop = NULL;
 
     GenInfo::Ptr coro = nullptr;
 
-    std::string name;
+    StringTable::Key name;
 
     // Information to reconstruct the async stack as best as we can
     TaskInfo::Ptr waiter = nullptr;
 
     TaskInfo(TaskObj *);
 
     static TaskInfo current(PyObject *);
@@ -163,25 +163,17 @@
         throw GeneratorError();
     }
 
     origin = (PyObject *)task_addr;
 
     try
     {
-#if PY_VERSION_HEX >= 0x030c0000
-        // The task name might hold a PyLong for deferred task name formatting.
-        PyLongObject name_obj;
-        name = (!copy_type(task.task_name, name_obj) && PyLong_CheckExact(&name_obj))
-                   ? "Task-" + std::to_string(PyLong_AsLong((PyObject *)&name_obj))
-                   : pyunicode_to_utf8(task.task_name);
-#else
-        name = pyunicode_to_utf8(task.task_name);
-#endif
+        name = string_table.key(task.task_name);
     }
-    catch (StringError &)
+    catch (StringTable::Error &)
     {
         throw Error();
     }
 
     loop = task.task_loop;
 
     if (task.task_fut_waiter)
```

### Comparing `echion-0.2.0/echion/threads.h` & `echion-0.3.0/echion/threads.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 // This file is part of "echion" which is released under MIT.
 //
 // Copyright (c) 2023 Gabriele N. Tornetta <phoenix1987@gmail.com>.
 
 #pragma once
 
+#include <Python.h>
+#define Py_BUILD_CORE
+
 #include <cstdint>
 #include <exception>
 #include <functional>
 #include <mutex>
 #include <sstream>
 #include <unordered_map>
 
@@ -50,25 +53,26 @@
     microsecond_t cpu_time;
 
     uintptr_t asyncio_loop = 0;
 
     void update_cpu_time();
     bool is_running();
 
-    void sample(PyThreadState *, microsecond_t);
+    void sample(int64_t, PyThreadState *, microsecond_t);
     void unwind(PyThreadState *);
 
     void render_where(FrameStack &stack, std::ostream &output)
     {
         output << "    🧵 " << name << ":" << std::endl;
 
         for (auto it = stack.rbegin(); it != stack.rend(); ++it)
             (*it).get().render_where(output);
     }
 
+    // ------------------------------------------------------------------------
     ThreadInfo(uintptr_t thread_id, unsigned long native_id, const char *name)
         : thread_id(thread_id), native_id(native_id), name(name)
     {
 #if defined PL_LINUX
         // Try to check that the thread_id is a valid pointer to a pthread
         // structure. Calling pthread_getcpuclockid on an invalid memory address
         // will cause a segmentation fault.
@@ -184,22 +188,24 @@
         // for the next thread.
         sigprof_handler_lock.lock();
     }
     else
     {
         unwind_python_stack(tstate);
         if (asyncio_loop)
+        {
             try
             {
                 unwind_tasks();
             }
             catch (TaskInfo::Error &)
             {
                 // We failed to unwind tasks
             }
+        }
     }
 }
 
 // ----------------------------------------------------------------------------
 void ThreadInfo::unwind_tasks()
 {
     std::vector<TaskInfo::Ref> leaf_tasks;
@@ -275,15 +281,15 @@
                 {
                     stack->push_front(temp_stack.front());
                     temp_stack.pop_front();
                 }
             }
 
             // Add the task name frame
-            stack->push_back(Frame::get(task.origin, task.name));
+            stack->push_back(Frame::get(task.name));
 
             // Get the next task in the chain
             PyObject *task_origin = task.origin;
             if (waitee_map.find(task_origin) != waitee_map.end())
             {
                 current_task = waitee_map.find(task_origin)->second;
                 continue;
@@ -310,15 +316,15 @@
             stack->push_back(*p);
 
         current_tasks.push_back(std::move(stack));
     }
 }
 
 // ----------------------------------------------------------------------------
-void ThreadInfo::sample(PyThreadState *tstate, microsecond_t delta)
+void ThreadInfo::sample(int64_t iid, PyThreadState *tstate, microsecond_t delta)
 {
     if (cpu)
     {
         microsecond_t previous_cpu_time = cpu_time;
         update_cpu_time();
 
         if (!is_running())
@@ -330,53 +336,53 @@
 
     unwind(tstate);
 
     // Asyncio tasks
     if (current_tasks.empty())
     {
         // Print the PID and thread name
-        output << "P" << pid << ";T" << name;
+        mojo.stack(pid, iid, name);
 
         // Print the stack
         if (native)
         {
             interleave_stacks();
-            interleaved_stack.render(output);
+            interleaved_stack.render();
         }
         else
-            python_stack.render(output);
+            python_stack.render();
 
         // Print the metric
-        output << " " << delta << std::endl;
+        mojo.metric_time(delta);
     }
     else
     {
         for (auto &task_stack : current_tasks)
         {
-            output << "P" << pid << ";T" << name;
+            mojo.stack(pid, iid, name);
 
             if (native)
             {
                 // NOTE: These stacks might be non-sensical, especially with
                 // Python < 3.11.
                 interleave_stacks(*task_stack);
-                interleaved_stack.render(output);
+                interleaved_stack.render();
             }
             else
-                task_stack->render(output);
+                task_stack->render();
 
-            output << " " << delta << std::endl;
+            mojo.metric_time(delta);
         }
 
         current_tasks.clear();
     }
 }
 
 // ----------------------------------------------------------------------------
-static void for_each_thread(std::function<void(PyThreadState *, ThreadInfo &)> callback)
+static void for_each_thread(PyInterpreterState *interp, std::function<void(PyThreadState *, ThreadInfo &)> callback)
 {
     std::unordered_set<PyThreadState *> threads;
     std::unordered_set<PyThreadState *> seen_threads;
 
     threads.clear();
     seen_threads.clear();
```

### Comparing `echion-0.2.0/echion/timing.h` & `echion-0.3.0/echion/timing.h`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/echion/vm.h` & `echion-0.3.0/echion/vm.h`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/echion.egg-info/PKG-INFO` & `echion-0.3.0/echion.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echion
-Version: 0.2.0
+Version: 0.3.0
 Summary: In-process CPython frame stack sampler
 Author: Gabriele N. Tornetta
 Author-email: "Gabriele N. Tornetta" <phoenix1987@gmail.com>
 Project-URL: homepage, https://github.com/P403n1x87/echion
 Project-URL: repository, https://github.com/P403n1x87/echion
 Project-URL: issues, https://github.com/P403n1x87/echion/issues
 Keywords: performance,profiling,testing,development
@@ -76,14 +76,15 @@
 options:
   -h, --help            show this help message and exit
   -i INTERVAL, --interval INTERVAL
                         sampling interval in microseconds
   -c, --cpu             sample on-CPU stacks only
   -x EXPOSURE, --exposure EXPOSURE
                         exposure time, in seconds
+  -m, --memory          Collect memory allocation events
   -n, --native          sample native stacks
   -o OUTPUT, --output OUTPUT
                         output location (can use %(pid) to insert the process ID)
   -p PID, --pid PID     Attach to the process with the given PID
   -s, --stealth         stealth mode (sampler thread is not accounted for)
   -w WHERE, --where WHERE
                         where mode: display thread stacks of the given process
@@ -119,14 +120,33 @@
 
 When running or attaching to a process, you can also send a `SIGQUIT` signal to
 dump the stacks of all running threads. The result is similar to the where mode.
 You can normally send a `SIGQUIT` signal with the <kbd>CTRL</kbd>+<kbd>\\</kbd>
 key combination.
 
 
+## Memory mode
+
+Besides wall time and CPU time, Echion can be used to profile memory
+allocations. In this mode, Echion tracks the Python memory domain allocators and
+accounts for each single event. Because of the tracing nature, this mode
+introduces considerable overhead, but gives pretty accurate results that can be
+used to investigate potential memory leaks. To fully understand that data that
+is collected in this mode, one should be aware of how Echion tracks allocations
+and deallocations. When an allocation is made, Echion records the frame stack
+that was involved and maps it to the returned memory address. When a
+deallocation for a tracked memory address is made, the freed memory is accounted
+for the same stack. Therefore, objects that are allocated and deallocated during
+the tracking period account for a total of 0 allocated bytes. This means that
+all the non-negative values reported by Echion represent memory that was still
+allocated by the time the tracking ended.
+
+*Since Echion 0.3.0*.
+
+
 ## Why Echion?
 
 Sampling in-process comes with some benefits. One has easier access to more
 information, like thread names, and potentially the task abstraction of async
 frameworks, like `asyncio`, `gevent`, ... . Also available is more accurate
 per-thread CPU timing information.
```

### Comparing `echion-0.2.0/echion.egg-info/SOURCES.txt` & `echion-0.3.0/echion.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 echion/__main__.py
 echion/_version.py
 echion/cache.h
 echion/config.h
 echion/core.pyi
 echion/coremodule.cc
 echion/frame.h
+echion/interp.h
+echion/memory.h
 echion/mirrors.h
 echion/module.py
+echion/mojo.h
 echion/signals.h
 echion/stacks.h
 echion/state.h
 echion/strings.h
 echion/tasks.h
 echion/threads.h
 echion/timing.h
@@ -47,14 +50,16 @@
 tests/target.py
 tests/target_async.py
 tests/target_async_tasks.py
 tests/target_attach.py
 tests/target_bytecode.py
 tests/target_cpu.py
 tests/target_gather.py
+tests/target_mem.py
 tests/target_where.py
 tests/test_asyncio.py
 tests/test_cpu_data.py
 tests/test_echion.py
+tests/test_memory.py
 tests/test_wall_data.py
 tests/test_where.py
 tests/utils.py
```

### Comparing `echion-0.2.0/pyproject.toml` & `echion-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 echion = "echion.__main__:main"
 
 [tool.hatch.envs.tests]
 template = "tests"
 dependencies = [
   "pytest>=5.4.2",
   "pytest-cov>=2.8.1",
-  "austin-python",
+  "austin-python~=1.7",
   "bytecode",
 ]
 
 [tool.hatch.envs.tests.scripts]
 tests = "pytest --cov=echion --cov-report=term-missing --cov-report=xml {args}"
 
 [[tool.hatch.envs.tests.matrix]]
```

### Comparing `echion-0.2.0/setup.py` & `echion-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/tests/target_bytecode.py` & `echion-0.3.0/tests/target_bytecode.py`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/tests/target_cpu.py` & `echion-0.3.0/tests/target_cpu.py`

 * *Files identical despite different names*

### Comparing `echion-0.2.0/tests/test_asyncio.py` & `echion-0.3.0/tests/test_asyncio.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
     expected_nthreads = 2
     assert summary.nthreads == expected_nthreads, summary.threads
     assert summary.total_metric >= 1.4 * 1e6
 
     # Test line numbers
     assert (
-        summary.query("MainThread", (("F4_0", 0), ("f4", 22), ("f5", 26))) is not None
+        summary.query("0:MainThread", (("F4_0", 0), ("f4", 22), ("f5", 26))) is not None
     )
     assert (
-        summary.query("MainThread", (("F4_1", 0), ("f4", 22), ("f5", 26))) is not None
+        summary.query("0:MainThread", (("F4_1", 0), ("f4", 22), ("f5", 26))) is not None
     )
 
     # Test stacks and expected values
     if PY >= (3, 11):
         for t in ("F4_0", "F4_1"):
             summary.assert_substack(
-                "MainThread",
+                "0:MainThread",
                 (
                     "_run_module_as_main",
                     "_run_code",
                     "<module>",
                     "run",
                     "Runner.run",
                     "BaseEventLoop.run_until_complete",
@@ -57,15 +57,15 @@
                     "sleep",
                 ),
                 lambda v: v >= 0.45e6,
             )
     else:
         for t in ("F4_0", "F4_1"):
             summary.assert_substack(
-                "MainThread",
+                "0:MainThread",
                 (
                     "_run_module_as_main",
                     "_run_code",
                     "<module>",
                     "run",
                     "run_until_complete",
                     "run_forever",
```

### Comparing `echion-0.2.0/tests/test_cpu_data.py` & `echion-0.3.0/tests/test_cpu_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,73 +19,73 @@
 
     expected_nthreads = 3 - bool(stealth)
     assert summary.nthreads == expected_nthreads
     assert summary.total_metric >= 0.5 * 1e6 * (2 - bool(stealth))
     assert summary.nsamples
 
     # Test line numbers
-    assert summary.query("MainThread", (("main", 22), ("bar", 17))) is None
+    assert summary.query("0:MainThread", (("main", 22), ("bar", 17))) is None
     assert (
         summary.query(
-            "SecondaryThread",
+            "0:SecondaryThread",
             ("Thread.run" if PY >= (3, 11) else "run", "keep_cpu_busy"),
         )
         is not None
     )
 
     # Test stacks and expected values
     summary.assert_stack(
-        "MainThread",
+        "0:MainThread",
         (
             "_run_module_as_main",
             "_run_code",
             "<module>",
             "keep_cpu_busy",
         ),
         lambda v: v >= 3e5,
     )
 
     if PY >= (3, 11):
         summary.assert_stack(
-            "SecondaryThread",
+            "0:SecondaryThread",
             (
                 "Thread._bootstrap",
                 "thread_bootstrap_inner",
                 "Thread._bootstrap_inner",
                 "Thread.run",
                 "keep_cpu_busy",
             ),
             lambda v: v >= 3e5,
         )
         if not bool(stealth):
             summary.assert_stack(
-                "echion.core.sampler",
+                "0:echion.core.sampler",
                 (
                     "Thread._bootstrap",
                     "thread_bootstrap_inner",
                     "Thread._bootstrap_inner",
                     "Thread.run",
                 ),
                 lambda v: v >= 0.5e6,
             )
     else:
         summary.assert_stack(
-            "SecondaryThread",
+            "0:SecondaryThread",
             (
                 "_bootstrap",
                 "thread_bootstrap_inner",
                 "_bootstrap_inner",
                 "run",
                 "keep_cpu_busy",
             ),
             lambda v: v >= 3e5,
         )
         if not bool(stealth):
             summary.assert_stack(
-                "echion.core.sampler",
+                "0:echion.core.sampler",
                 (
                     "_bootstrap",
                     "thread_bootstrap_inner",
                     "_bootstrap_inner",
                     "run",
                 ),
                 lambda v: v >= 0.5e6,
@@ -108,19 +108,19 @@
     assert summary.nthreads == expected_nthreads
     assert summary.total_metric
 
     # Test line numbers. This only works with CFrame
     if PY >= (3, 11):
         assert (
             summary.query(
-                "MainThread",
+                "0:MainThread",
                 (
                     ("<module>", 48),
                     ("keep_cpu_busy", 39),
                 ),
             )
             is not None
-        ), summary.threads["MainThread"]
-        assert summary.query("SecondaryThread", (("keep_cpu_busy", 39),)) is not None
+        ), summary.threads["0:MainThread"]
+        assert summary.query("0:SecondaryThread", (("keep_cpu_busy", 39),)) is not None
     else:
-        assert summary.query("MainThread", (("keep_cpu_busy", 39),)) is not None
-        assert summary.query("SecondaryThread", (("keep_cpu_busy", 39),)) is not None
+        assert summary.query("0:MainThread", (("keep_cpu_busy", 39),)) is not None
+        assert summary.query("0:SecondaryThread", (("keep_cpu_busy", 39),)) is not None
```

### Comparing `echion-0.2.0/tests/test_wall_data.py` & `echion-0.3.0/tests/test_wall_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,58 +18,58 @@
     summary = DataSummary(data)
 
     expected_nthreads = 3 - bool(stealth)
     assert summary.nthreads == expected_nthreads
     assert summary.total_metric >= 1e6 * expected_nthreads
 
     # Test line numbers
-    assert summary.query("MainThread", (("main", 22), ("bar", 17))) is not None
-    assert summary.query("SecondaryThread", (("bar", 18), ("foo", 13))) is not None
+    assert summary.query("0:MainThread", (("main", 22), ("bar", 17))) is not None
+    assert summary.query("0:SecondaryThread", (("bar", 18), ("foo", 13))) is not None
 
     # Test stacks and expected values
     summary.assert_stack(
-        "MainThread",
+        "0:MainThread",
         (
             "_run_module_as_main",
             "_run_code",
             "<module>",
             "main",
             "bar",
         ),
         lambda v: v >= 0.95e6,
     )
     summary.assert_stack(
-        "MainThread",
+        "0:MainThread",
         (
             "_run_module_as_main",
             "_run_code",
             "<module>",
             "main",
             "bar",
             "foo",
             "cpu_sleep",
         ),
         lambda v: v >= 4.5e5,
     )
 
     if PY >= (3, 11):
         summary.assert_stack(
-            "SecondaryThread",
+            "0:SecondaryThread",
             (
                 "Thread._bootstrap",
                 "thread_bootstrap_inner",
                 "Thread._bootstrap_inner",
                 "Thread.run",
                 "main",
                 "bar",
             ),
             lambda v: v >= 0.95e6,
         )
         summary.assert_stack(
-            "SecondaryThread",
+            "0:SecondaryThread",
             (
                 "Thread._bootstrap",
                 "thread_bootstrap_inner",
                 "Thread._bootstrap_inner",
                 "Thread.run",
                 "main",
                 "bar",
@@ -77,38 +77,38 @@
                 "cpu_sleep",
             ),
             lambda v: v >= 4.5e5,
         )
 
         if not bool(stealth):
             summary.assert_stack(
-                "echion.core.sampler",
+                "0:echion.core.sampler",
                 (
                     "Thread._bootstrap",
                     "thread_bootstrap_inner",
                     "Thread._bootstrap_inner",
                     "Thread.run",
                 ),
                 lambda v: v >= 1.45e6,
             )
     else:
         summary.assert_stack(
-            "SecondaryThread",
+            "0:SecondaryThread",
             (
                 "_bootstrap",
                 "thread_bootstrap_inner",
                 "_bootstrap_inner",
                 "run",
                 "main",
                 "bar",
             ),
             lambda v: v >= 0.95e6,
         )
         summary.assert_stack(
-            "SecondaryThread",
+            "0:SecondaryThread",
             (
                 "_bootstrap",
                 "thread_bootstrap_inner",
                 "_bootstrap_inner",
                 "run",
                 "main",
                 "bar",
@@ -116,15 +116,15 @@
                 "cpu_sleep",
             ),
             lambda v: v >= 4.5e5,
         )
 
         if not bool(stealth):
             summary.assert_stack(
-                "echion.core.sampler",
+                "0:echion.core.sampler",
                 (
                     "_bootstrap",
                     "thread_bootstrap_inner",
                     "_bootstrap_inner",
                     "run",
                 ),
                 lambda v: v >= 1.45e6,
@@ -145,12 +145,14 @@
 
     expected_nthreads = 3 - bool(stealth)
     assert summary.nthreads == expected_nthreads
     assert summary.total_metric
 
     # Test line numbers. This only works with CFrames
     if PY >= (3, 11):
-        assert summary.query("MainThread", (("main", 22), ("bar", 17))) is not None
-        assert summary.query("SecondaryThread", (("bar", 18), ("foo", 13))) is not None
+        assert summary.query("0:MainThread", (("main", 22), ("bar", 17))) is not None
+        assert (
+            summary.query("0:SecondaryThread", (("bar", 18), ("foo", 13))) is not None
+        )
     else:
-        assert summary.query("MainThread", (("bar", 17),)) is not None
-        assert summary.query("SecondaryThread", (("foo", 13),)) is not None
+        assert summary.query("0:MainThread", (("bar", 17),)) is not None
+        assert summary.query("0:SecondaryThread", (("foo", 13),)) is not None
```

### Comparing `echion-0.2.0/tests/test_where.py` & `echion-0.3.0/tests/test_where.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # This test requires sudo on unix to work
 @requires_sudo
 def test_where():
     with Popen(
         [sys.executable, "-m", "tests.target_attach"], stdout=PIPE, stderr=PIPE
     ) as target:
-        sleep(0.5)
+        sleep(1)
         try:
             # attach multiple times
             for _ in range(10):
                 result = run_echion("-w", str(target.pid))
                 assert result.returncode == 0
 
                 err = result.stdout.decode()
```

### Comparing `echion-0.2.0/tests/utils.py` & `echion-0.3.0/tests/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,63 +8,58 @@
 from subprocess import CompletedProcess
 from subprocess import Popen
 from subprocess import run
 from tempfile import TemporaryDirectory
 from time import sleep
 
 import pytest
-from austin.stats import AustinFileReader
-from austin.stats import MetricType
-from austin.stats import Sample
+from austin.format.mojo import MojoFile
 
 
 PY = sys.version_info[:2]
 
 
-class Data:
-    def __init__(self, file: Path) -> None:
-        self.source = file
-        self.samples = []
-
-        with AustinFileReader(str(file)) as afr:
-            for s in afr:
-                self.samples.append(Sample.parse(s, MetricType.TIME)[0])
-
-            self.metadata = afr.metadata
-
-
 class DataSummary:
-    def __init__(self, data: Data) -> None:
+    def __init__(self, data: MojoFile) -> None:
         self.data = data
         self.metadata = data.metadata
 
         self.threads: t.Dict[str, dict] = {}
         self.total_metric = 0
         self.nsamples = 0
 
         for sample in data.samples:
             self.nsamples += 1
             frames = sample.frames
-            v = sample.metric.value
+            v = sample.metrics[0].value
+
+            if not sample.thread or not v:
+                continue
 
             self.total_metric += v
-            stacks = self.threads.setdefault(sample.thread, {})
 
-            stack = tuple((f.function, f.line) for f in frames)
+            stacks = self.threads.setdefault(f"{sample.iid}:{sample.thread}", {})
+
+            stack = tuple((f.scope.string.value, f.line) for f in frames)
             stacks[stack] = stacks.get(stack, 0) + v
 
-            fstack = tuple(f.function for f in frames)
+            fstack = tuple(f.scope.string.value for f in frames)
             stacks[fstack] = stacks.get(fstack, 0) + v
 
     @property
     def nthreads(self):
         return len(self.threads)
 
     def query(self, thread_name, frames):
-        stacks = self.threads[thread_name]
+        try:
+            stacks = self.threads[thread_name]
+        except KeyError as e:
+            raise AssertionError(
+                f"Expected thread {thread_name}, found {list(self.threads.keys())}"
+            ) from e
         for stack in stacks:
             for i in range(0, len(stack) - len(frames) + 1):
                 if stack[i : i + len(frames)] == frames:
                     return stacks[stack]
         return None
 
     def assert_stack(self, thread, frames, predicate):
@@ -115,28 +110,35 @@
         )
     except CalledProcessError as e:
         print(e.stdout.decode())
         print(e.stderr.decode())
         raise
 
 
-def run_target(target: Path, *args: str) -> t.Tuple[CompletedProcess, t.Optional[Data]]:
+def run_target(
+    target: Path, *args: str
+) -> t.Tuple[CompletedProcess, t.Optional[MojoFile]]:
     with TemporaryDirectory(prefix="echion") as td:
         output_file = Path(td) / "output.echion"
 
         result = run_echion(
             "-o",
             str(output_file),
             *args,
             sys.executable,
             "-m",
             f"tests.{target}",
         )
 
-        return result, (Data(output_file) if output_file.is_file() else None)
+        if not output_file.is_file():
+            return result, None
+
+        m = MojoFile(output_file.open(mode="rb"))
+        m.unwind()
+        return result, m
 
 
 def run_with_signal(target: Path, signal: int, delay: float, *args: str) -> Popen:
     p = Popen(
         [
             t.cast(str, which("echion")),
             *args,
```

