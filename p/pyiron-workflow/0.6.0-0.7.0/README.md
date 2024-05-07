# Comparing `tmp/pyiron_workflow-0.6.0.tar.gz` & `tmp/pyiron_workflow-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_workflow-0.6.0.tar", last modified: Mon Apr 29 18:41:49 2024, max compression
+gzip compressed data, was "pyiron_workflow-0.7.0.tar", last modified: Tue May  7 00:18:16 2024, max compression
```

## Comparing `pyiron_workflow-0.6.0.tar` & `pyiron_workflow-0.7.0.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.295286 pyiron_workflow-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-29 18:41:49.295286 pyiron_workflow-0.6.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.287286 pyiron_workflow-0.6.0/pyiron_workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-29 18:41:49.295286 pyiron_workflow-0.6.0/pyiron_workflow/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25563 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)    21826 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/draw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.291286 pyiron_workflow-0.6.0/pyiron_workflow/executors/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/executors/cloudpickleprocesspool.py
--rw-r--r--   0 runner    (1001) docker     (127)    16969 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/has_interface_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/has_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/injection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21838 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/io_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)    10004 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/loops.py
--rw-r--r--   0 runner    (1001) docker     (127)    23019 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    39289 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.291286 pyiron_workflow-0.6.0/pyiron_workflow/node_library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.291286 pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/pyiron_atomistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_library/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/node_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    14282 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/semantics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/single_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.291286 pyiron_workflow-0.6.0/pyiron_workflow/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/dotdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/has_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/snippets/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)    13002 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/type_hinting.py
--rw-r--r--   0 runner    (1001) docker     (127)    23787 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/pyiron_workflow/working.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:41:49.291286 pyiron_workflow-0.6.0/pyiron_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-29 18:41:49.000000 pyiron_workflow-0.6.0/pyiron_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-29 18:41:49.000000 pyiron_workflow-0.6.0/pyiron_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:41:49.000000 pyiron_workflow-0.6.0/pyiron_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-29 18:41:49.000000 pyiron_workflow-0.6.0/pyiron_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 18:41:49.000000 pyiron_workflow-0.6.0/pyiron_workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 18:41:49.295286 pyiron_workflow-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-29 18:41:48.000000 pyiron_workflow-0.6.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-29 18:41:46.000000 pyiron_workflow-0.6.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.393709 pyiron_workflow-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-07 00:18:16.393709 pyiron_workflow-0.7.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.385709 pyiron_workflow-0.7.0/pyiron_workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-07 00:18:16.393709 pyiron_workflow-0.7.0/pyiron_workflow/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25333 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21754 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/draw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.389709 pyiron_workflow-0.7.0/pyiron_workflow/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/executors/cloudpickleprocesspool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17674 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/for_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/has_interface_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/has_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21838 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/io_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24685 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39869 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.389709 pyiron_workflow-0.7.0/pyiron_workflow/node_library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.389709 pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/pyiron_atomistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_library/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/node_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13029 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/semantics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/single_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.389709 pyiron_workflow-0.7.0/pyiron_workflow/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/dotdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/has_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/snippets/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/type_hinting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23787 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/pyiron_workflow/working.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:18:16.389709 pyiron_workflow-0.7.0/pyiron_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-07 00:18:16.000000 pyiron_workflow-0.7.0/pyiron_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-07 00:18:16.000000 pyiron_workflow-0.7.0/pyiron_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 00:18:16.000000 pyiron_workflow-0.7.0/pyiron_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-07 00:18:16.000000 pyiron_workflow-0.7.0/pyiron_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 00:18:16.000000 pyiron_workflow-0.7.0/pyiron_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-07 00:18:16.393709 pyiron_workflow-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-07 00:18:15.000000 pyiron_workflow-0.7.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-05-07 00:18:10.000000 pyiron_workflow-0.7.0/versioneer.py
```

### Comparing `pyiron_workflow-0.6.0/LICENSE` & `pyiron_workflow-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/PKG-INFO` & `pyiron_workflow-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_workflow
-Version: 0.6.0
+Version: 0.7.0
 Summary: Graph-and-node based workflow tools.
 Home-page: https://github.com/pyiron/pyiron_workflow
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: liamhuber@greyhavensolutions.com
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 3 - Alpha
@@ -17,20 +17,20 @@
 License-File: LICENSE
 Requires-Dist: bidict>=0.23.1
 Requires-Dist: cloudpickle>=3.0.0
 Requires-Dist: graphviz>=0.20.3
 Requires-Dist: h5io>=0.2.2
 Requires-Dist: h5io_browser>=0.0.12
 Requires-Dist: matplotlib>=3.8.4
-Requires-Dist: pyiron_base>=0.8.2
+Requires-Dist: pyiron_base>=0.8.3
 Requires-Dist: pyiron_contrib>=0.1.16
-Requires-Dist: pympipool>=0.7.17
+Requires-Dist: pympipool>=0.8.0
 Requires-Dist: toposort>=1.10
 Requires-Dist: typeguard>=4.2.1
 Provides-Extra: node-library
 Requires-Dist: ase>=3.22.1; extra == "node-library"
 Requires-Dist: atomistics>=0.1.27; extra == "node-library"
 Requires-Dist: numpy>=1.26.4; extra == "node-library"
 Requires-Dist: phonopy>=2.22.1; extra == "node-library"
-Requires-Dist: pyiron_atomistics>=0.5.3; extra == "node-library"
+Requires-Dist: pyiron_atomistics>=0.5.4; extra == "node-library"
 
 http://pyiron.org
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/__init__.py` & `pyiron_workflow-0.7.0/pyiron_workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/channels.py` & `pyiron_workflow-0.7.0/pyiron_workflow/channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 """
 
 from __future__ import annotations
 
 import typing
 from abc import ABC, abstractmethod
 import inspect
-from warnings import warn
 
 from pyiron_workflow.has_interface_mixins import HasChannel, HasLabel, UsesState
 from pyiron_workflow.has_to_dict import HasToDict
 from pyiron_workflow.snippets.singleton import Singleton
 from pyiron_workflow.type_hinting import (
     valid_value,
     type_hint_is_as_or_more_specific_than,
@@ -168,19 +167,14 @@
         """
         destroyed_connections = []
         for other in others:
             if other in self.connections:
                 self.connections.remove(other)
                 other.disconnect(self)
                 destroyed_connections.append((self, other))
-            else:
-                warn(
-                    f"The channel {self.label} was not connected to {other.label}, and"
-                    f"thus could not disconnect from it."
-                )
         return destroyed_connections
 
     def disconnect_all(self) -> list[tuple[Channel, Channel]]:
         """
         Disconnect from all other channels currently in the connections list.
         """
         return self.disconnect(*self.connections)
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/composite.py` & `pyiron_workflow-0.7.0/pyiron_workflow/composite.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 A base class for nodal objects that have internal structure -- i.e. they hold a
 sub-graph
 """
 
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
+from abc import ABC
 from time import sleep
 from typing import Literal, Optional, TYPE_CHECKING
 
 from pyiron_workflow.create import HasCreator
 from pyiron_workflow.node import Node
 from pyiron_workflow.semantics import SemanticParent
 from pyiron_workflow.topology import set_run_connections_according_to_dag
@@ -142,38 +142,32 @@
 
     def to_dict(self):
         return {
             "label": self.label,
             "nodes": {n.label: n.to_dict() for n in self.children.values()},
         }
 
-    @property
     def on_run(self):
-        return self.run_graph
-
-    @staticmethod
-    def run_graph(_composite: Composite):
         # Reset provenance and run status trackers
-        _composite.provenance_by_execution = []
-        _composite.provenance_by_completion = []
-        _composite.running_children = []
-        _composite.signal_queue = []
+        self.provenance_by_execution = []
+        self.provenance_by_completion = []
+        self.running_children = []
+        self.signal_queue = []
 
-        for node in _composite.starting_nodes:
+        for node in self.starting_nodes:
             node.run()
 
-        while len(_composite.running_children) > 0 or len(_composite.signal_queue) > 0:
+        while len(self.running_children) > 0 or len(self.signal_queue) > 0:
             try:
-                ran_signal, receiver = _composite.signal_queue.pop(0)
+                ran_signal, receiver = self.signal_queue.pop(0)
                 receiver(ran_signal)
             except IndexError:
                 # The signal queue is empty, but there is still someone running...
-                sleep(_composite._child_sleep_interval)
-
-        return _composite
+                sleep(self._child_sleep_interval)
+        return self
 
     def register_child_starting(self, child: Node) -> None:
         """
         To be called by children when they start their run cycle.
 
         Args:
             child [Node]: The child that is finished and would like to fire its `ran`
@@ -210,28 +204,30 @@
                 signal. Should always be a child of `self`, but this is not explicitly
                 verified at runtime.
         """
         for conn in child.signals.output.ran.connections:
             self.signal_queue.append((child.signals.output.ran, conn))
 
     @property
-    def run_args(self) -> dict:
-        return {"_composite": self}
+    def run_args(self) -> tuple[tuple, dict]:
+        return (), {}
 
     def process_run_result(self, run_output):
         if run_output is not self:
             self._parse_remotely_executed_self(run_output)
         return DotDict(self.outputs.to_value_dict())
 
     def _parse_remotely_executed_self(self, other_self):
         # Un-parent existing nodes before ditching them
         for node in self:
             node._parent = None
         other_self.running = False  # It's done now
-        self.__setstate__(other_self.__getstate__())
+        state = other_self.__getstate__()
+        state.pop("executor")  # Got overridden to None for __getstate__, so keep local
+        self.__setstate__(state)
 
     def disconnect_run(self) -> list[tuple[Channel, Channel]]:
         """
         Disconnect all `signals.input.run` connections on all child nodes.
 
         Returns:
             list[tuple[Channel, Channel]]: Any disconnected pairs.
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/create.py` & `pyiron_workflow-0.7.0/pyiron_workflow/create.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,36 @@
 """
 Container classes for giving access to various workflow objects and tools
 """
 
 from __future__ import annotations
 
 from abc import ABC
-from functools import wraps
+from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
+from functools import wraps, lru_cache
 from importlib import import_module
 import pkgutil
 from sys import version_info
 from types import ModuleType
 from typing import Optional, TYPE_CHECKING
 
 from bidict import bidict
-from pyiron_workflow.snippets.singleton import Singleton
-
-# Import all the supported executors
-from pympipool import Executor as PyMpiPoolExecutor, PyMPIExecutor
-
-try:
-    from pympipool import PySlurmExecutor
-except ImportError:
-    PySlurmExecutor = None
-try:
-    from pympipool import PyFluxExecutor
-except ImportError:
-    PyFluxExecutor = None
+from pympipool import Executor as PyMpiPoolExecutor
 
 from pyiron_workflow.executors import CloudpickleProcessPoolExecutor
-
-# Then choose one executor to be "standard"
-Executor = PyMpiPoolExecutor
-
 from pyiron_workflow.function import function_node, as_function_node
 from pyiron_workflow.snippets.dotdict import DotDict
+from pyiron_workflow.snippets.singleton import Singleton
 
 if TYPE_CHECKING:
     from pyiron_workflow.node_package import NodePackage
 
+# Specify the standard executor
+Executor = PyMpiPoolExecutor
+
 
 class Creator(metaclass=Singleton):
     """
     A container class for providing access to various workflow objects.
     Handles the registration of new node packages and, by virtue of being a singleton,
     makes them available to all composite nodes holding a creator.
 
@@ -54,80 +43,90 @@
     """
 
     def __init__(self):
         self._package_access = DotDict()
         self._package_registry = bidict()
 
         self.Executor = Executor
+        # Standard lib
+        self.ProcessPoolExecutor = ProcessPoolExecutor
+        self.ThreadPoolExecutor = ThreadPoolExecutor
+        # Local cloudpickler
         self.CloudpickleProcessPoolExecutor = CloudpickleProcessPoolExecutor
-        self.PyMPIExecutor = PyMPIExecutor
+        # pympipool
         self.PyMpiPoolExecutor = PyMpiPoolExecutor
 
         self.function_node = function_node
 
-        # Avoid circular imports by delaying import for children of Composite
-        self._macro_node = None
-        self._workflow = None
-        self._meta = None
-
         if version_info[0] == 3 and version_info[1] >= 10:
             # These modules use syntactic sugar for type hinting that is only supported
             # in python >=3.10
             # If the CI skips testing on 3.9 gets dropped, we can think about removing
             # this if-clause and just letting users of python <3.10 hit an error.
             self.register("pyiron_workflow.node_library.standard", "standard")
 
     @property
-    def PyFluxExecutor(self):
-        if PyFluxExecutor is None:
-            raise ImportError(f"{PyFluxExecutor.__name__} is not available")
-        return PyFluxExecutor
+    @lru_cache(maxsize=1)
+    def for_node(self):
+        from pyiron_workflow.for_loop import for_node
 
-    @property
-    def PySlurmExecutor(self):
-        if PySlurmExecutor is None:
-            raise ImportError(f"{PySlurmExecutor.__name__} is not available")
-        return PySlurmExecutor
+        return for_node
 
     @property
+    @lru_cache(maxsize=1)
     def macro_node(self):
-        if self._macro_node is None:
-            from pyiron_workflow.macro import macro_node
+        from pyiron_workflow.macro import macro_node
 
-            self._macro_node = macro_node
-        return self._macro_node
+        return macro_node
 
     @property
+    @lru_cache(maxsize=1)
     def Workflow(self):
-        if self._workflow is None:
-            from pyiron_workflow.workflow import Workflow
+        from pyiron_workflow.workflow import Workflow
 
-            self._workflow = Workflow
-        return self._workflow
+        return Workflow
 
     @property
+    @lru_cache(maxsize=1)
     def meta(self):
-        if self._meta is None:
-            from pyiron_workflow.meta import (
-                input_to_list,
-                list_to_output,
-            )
-            from pyiron_workflow.loops import while_loop
-            from pyiron_workflow.loops import for_loop
-            from pyiron_workflow.snippets.dotdict import DotDict
-
-            self._meta = DotDict(
-                {
-                    for_loop.__name__: for_loop,
-                    input_to_list.__name__: input_to_list,
-                    list_to_output.__name__: list_to_output,
-                    while_loop.__name__: while_loop,
-                }
-            )
-        return self._meta
+        from pyiron_workflow.transform import inputs_to_list, list_to_outputs
+        from pyiron_workflow.loops import while_loop
+        from pyiron_workflow.snippets.dotdict import DotDict
+
+        return DotDict(
+            {
+                inputs_to_list.__name__: inputs_to_list,
+                list_to_outputs.__name__: list_to_outputs,
+                while_loop.__name__: while_loop,
+            }
+        )
+
+    @property
+    @lru_cache(maxsize=1)
+    def transformer(self):
+        from pyiron_workflow.transform import (
+            dataclass_node,
+            inputs_to_dataframe,
+            inputs_to_dict,
+            inputs_to_list,
+            list_to_outputs,
+        )
+
+        return DotDict(
+            {
+                f.__name__: f
+                for f in [
+                    dataclass_node,
+                    inputs_to_dataframe,
+                    inputs_to_dict,
+                    inputs_to_list,
+                    list_to_outputs,
+                ]
+            }
+        )
 
     def __getattr__(self, item):
         try:
             return self._package_access[item]
         except KeyError as e:
             raise AttributeError(
                 f"{self.__class__.__name__} could not find attribute {item} -- did you "
@@ -313,27 +312,29 @@
 
 
 class Wrappers(metaclass=Singleton):
     """
     A container class giving access to the decorators that transform functions to nodes.
     """
 
-    def __init__(self):
-        self.as_function_node = as_function_node
-
-        # Avoid circular imports by delaying import when wrapping children of Composite
-        self._as_macro_node = None
+    as_function_node = staticmethod(as_function_node)
 
     @property
+    @lru_cache(maxsize=1)
     def as_macro_node(self):
-        if self._as_macro_node is None:
-            from pyiron_workflow.macro import as_macro_node
+        from pyiron_workflow.macro import as_macro_node
+
+        return as_macro_node
+
+    @property
+    @lru_cache(maxsize=1)
+    def as_dataclass_node(self):
+        from pyiron_workflow.transform import as_dataclass_node
 
-            self._as_macro_node = as_macro_node
-        return self._as_macro_node
+        return as_dataclass_node
 
 
 class HasCreator(ABC):
     """
     A mixin class for creator (including both class-like and decorator) and
     registration methods.
     """
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/draw.py` & `pyiron_workflow-0.7.0/pyiron_workflow/draw.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/executors/cloudpickleprocesspool.py` & `pyiron_workflow-0.7.0/pyiron_workflow/executors/cloudpickleprocesspool.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/function.py` & `pyiron_workflow-0.7.0/pyiron_workflow/function.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Any, Literal, Optional, TYPE_CHECKING
+from typing import Any
 
-from pyiron_workflow.io_preview import DecoratedNode, decorated_node_decorator_factory
+from pyiron_workflow.io_preview import StaticNode, ScrapesIO
 from pyiron_workflow.snippets.colors import SeabornColors
+from pyiron_workflow.snippets.factory import classfactory
 
-if TYPE_CHECKING:
-    from pyiron_workflow.composite import Composite
 
-
-class Function(DecoratedNode, ABC):
+class Function(StaticNode, ScrapesIO, ABC):
     """
     Function nodes wrap an arbitrary python function.
 
     Actual function node instances can either be instances of the base node class, in
     which case the callable node function *must* be provided OR they can be instances
     of children of this class which provide the node function as a class-level method.
     Those children may define some or all of the node behaviour at the class level, and
@@ -293,35 +291,34 @@
         Using the `self` argument for function nodes is not fully supported; it will
         raise an error when combined with an executor, and otherwise behaviour is not
         guaranteed.
     """
 
     @staticmethod
     @abstractmethod
-    def node_function(*args, **kwargs) -> callable:
+    def node_function(**kwargs) -> callable:
         """What the node _does_."""
 
     @classmethod
     def _io_defining_function(cls) -> callable:
         return cls.node_function
 
     @classmethod
     def _build_outputs_preview(cls) -> dict[str, Any]:
         preview = super(Function, cls)._build_outputs_preview()
         return preview if len(preview) > 0 else {"None": type(None)}
         # If clause facilitates functions with no return value
 
-    @property
-    def on_run(self):
-        return self.node_function
+    def on_run(self, **kwargs):
+        return self.node_function(**kwargs)
 
     @property
-    def run_args(self) -> dict:
+    def run_args(self) -> tuple[tuple, dict]:
         kwargs = self.inputs.to_value_dict()
-        return kwargs
+        return (), kwargs
 
     def process_run_result(self, function_output: Any | tuple) -> Any | tuple:
         """
         Take the results of the node function, and use them to update the node output.
         """
         for out, value in zip(
             self.outputs,
@@ -343,68 +340,55 @@
 
     @property
     def color(self) -> str:
         """For drawing the graph"""
         return SeabornColors.green
 
 
-as_function_node = decorated_node_decorator_factory(Function, Function.node_function)
-
-
-def function_node(
-    node_function: callable,
-    *args,
-    label: Optional[str] = None,
-    parent: Optional[Composite] = None,
-    overwrite_save: bool = False,
-    run_after_init: bool = False,
-    storage_backend: Optional[Literal["h5io", "tinybase"]] = None,
-    save_after_run: bool = False,
-    output_labels: Optional[str | tuple[str]] = None,
-    validate_output_labels: bool = True,
-    **kwargs,
+@classfactory
+def function_node_factory(
+    node_function: callable, validate_output_labels: bool, /, *output_labels
 ):
-    """
-    Dynamically creates a new child of :class:`Function` using the
-    provided :func:`node_function` and returns an instance of that.
-
-    Beyond the standard :class:`Function`, initialization allows the args...
+    return (
+        node_function.__name__,
+        (Function,),  # Define parentage
+        {
+            "node_function": staticmethod(node_function),
+            "__module__": node_function.__module__,
+            "__qualname__": node_function.__qualname__,
+            "_output_labels": None if len(output_labels) == 0 else output_labels,
+            "_validate_output_labels": validate_output_labels,
+        },
+        {},
+    )
 
-    Args:
-        node_function (callable): The function determining the behaviour of the node.
-        output_labels (Optional[str | list[str] | tuple[str]]): A name for each return
-            value of the node function OR a single label. (Default is None, which
-            scrapes output labels automatically from the source code of the wrapped
-            function.) This can be useful when returned values are not well named, e.g.
-            to make the output channel dot-accessible if it would otherwise have a label
-            that requires item-string-based access. Additionally, specifying a _single_
-            label for a wrapped function that returns a tuple of values ensures that a
-            _single_ output channel (holding the tuple) is created, instead of one
-            channel for each return value. The default approach of extracting labels
-            from the function source code also requires that the function body contain
-            _at most_ one `return` expression, so providing explicit labels can be used
-            to circumvent this (at your own risk), or to circumvent un-inspectable
-            source code (e.g. a function that exists only in memory).
-    """
 
-    if not callable(node_function):
-        raise AttributeError(
-            f"Expected `node_function` to be callable but got {node_function}"
+def as_function_node(*output_labels, validate_output_labels=True):
+    def decorator(node_function):
+        function_node_factory.clear(node_function.__name__)  # Force a fresh class
+        factory_made = function_node_factory(
+            node_function, validate_output_labels, *output_labels
         )
+        factory_made._class_returns_from_decorated_function = node_function
+        factory_made.preview_io()
+        return factory_made
+
+    return decorator
+
 
+def function_node(
+    node_function,
+    *node_args,
+    output_labels=None,
+    validate_output_labels=True,
+    **node_kwargs,
+):
     if output_labels is None:
         output_labels = ()
     elif isinstance(output_labels, str):
         output_labels = (output_labels,)
-
-    return as_function_node(
-        *output_labels, validate_output_labels=validate_output_labels
-    )(node_function)(
-        *args,
-        label=label,
-        parent=parent,
-        overwrite_save=overwrite_save,
-        run_after_init=run_after_init,
-        storage_backend=storage_backend,
-        save_after_run=save_after_run,
-        **kwargs,
+    function_node_factory.clear(node_function.__name__)  # Force a fresh class
+    factory_made = function_node_factory(
+        node_function, validate_output_labels, *output_labels
     )
+    factory_made.preview_io()
+    return factory_made(*node_args, **node_kwargs)
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/has_interface_mixins.py` & `pyiron_workflow-0.7.0/pyiron_workflow/has_interface_mixins.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/injection.py` & `pyiron_workflow-0.7.0/pyiron_workflow/injection.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/io.py` & `pyiron_workflow-0.7.0/pyiron_workflow/io.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/io_preview.py` & `pyiron_workflow-0.7.0/pyiron_workflow/io_preview.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,18 +11,26 @@
 """
 
 from __future__ import annotations
 
 import inspect
 import warnings
 from abc import ABC, abstractmethod
-from functools import lru_cache
+from functools import lru_cache, wraps
 from textwrap import dedent
 from types import FunctionType
-from typing import Any, get_args, get_type_hints, Literal, Optional, TYPE_CHECKING
+from typing import (
+    Any,
+    ClassVar,
+    get_args,
+    get_type_hints,
+    Literal,
+    Optional,
+    TYPE_CHECKING,
+)
 
 from pyiron_workflow.channels import InputData, NOT_DATA
 from pyiron_workflow.injection import OutputDataWithInjection, OutputsWithInjection
 from pyiron_workflow.io import Inputs
 from pyiron_workflow.node import Node
 from pyiron_workflow.output_parser import ParseOutput
 from pyiron_workflow.snippets.dotdict import DotDict
@@ -75,14 +83,30 @@
     @classmethod
     def preview_io(cls) -> DotDict[str:dict]:
         return DotDict(
             {"inputs": cls.preview_inputs(), "outputs": cls.preview_outputs()}
         )
 
 
+def builds_class_io(subclass_factory: callable[..., type[HasIOPreview]]):
+    """
+    A decorator for factories producing subclasses of `HasIOPreview` to invoke
+    :meth:`preview_io` after the class is created, thus ensuring the IO has been
+    constructed at the class level.
+    """
+
+    @wraps(subclass_factory)
+    def wrapped(*args, **kwargs):
+        node_class = subclass_factory(*args, **kwargs)
+        node_class.preview_io()
+        return node_class
+
+    return wrapped
+
+
 class ScrapesIO(HasIOPreview, ABC):
     """
     A mixin class for scraping IO channel information from a specific class method's
     signature and returns.
 
     Requires that the (static and class) method :meth:`_io_defining_function` be
     specified in child classes, as well as :meth:`_io_defining_function_uses_self`.
@@ -108,19 +132,21 @@
         depend on the :meth:`_io_defining_function` and its signature, which should
         thus be left static from the time of class definition onwards.
     """
 
     @classmethod
     @abstractmethod
     def _io_defining_function(cls) -> callable:
-        """Must return a static class method."""
+        """Must return a static method."""
 
-    _output_labels: tuple[str] | None = None  # None: scrape them
-    _validate_output_labels: bool = True  # True: validate against source code
-    _io_defining_function_uses_self: bool = False  # False: use entire signature
+    _output_labels: ClassVar[tuple[str] | None] = None  # None: scrape them
+    _validate_output_labels: ClassVar[bool] = True  # True: validate against source code
+    _io_defining_function_uses_self: ClassVar[bool] = (
+        False  # False: use entire signature
+    )
 
     @classmethod
     def _build_inputs_preview(cls):
         type_hints = cls._get_type_hints()
         scraped: dict[str, tuple[Any, Any]] = {}
         for i, (label, value) in enumerate(cls._get_input_args().items()):
             if cls._io_defining_function_uses_self and i == 0:
@@ -334,119 +360,7 @@
     @property
     def inputs(self) -> Inputs:
         return self._inputs
 
     @property
     def outputs(self) -> OutputsWithInjection:
         return self._outputs
-
-
-class DecoratedNode(StaticNode, ScrapesIO, ABC):
-    """
-    A static node whose IO is defined by a function's information (and maybe output
-    labels).
-    """
-
-
-def decorated_node_decorator_factory(
-    parent_class: type[DecoratedNode],
-    io_static_method: callable,
-    decorator_docstring_additions: str = "",
-    **parent_class_attr_overrides,
-):
-    """
-    A decorator factory for building decorators to dynamically create new subclasses
-    of some subclass of :class:`DecoratedNode` using the function they decorate.
-
-    New classes get their class name and module set using the decorated function's
-    name and module.
-
-    Args:
-        parent_class (type[DecoratedNode]): The base class for the new node class.
-        io_static_method: The static method on the :param:`parent_class` which will
-            store the io-defining function the resulting decorator will decorate.
-            :param:`parent_class` must override :meth:`_io_defining_function` inherited
-            from :class:`DecoratedNode` to return this method. This allows
-            :param:`parent_class` classes to have unique names for their io-defining
-            functions.
-        decorator_docstring_additions (str): Any extra text to add between the main
-            body of the docstring and the arguments.
-        **parent_class_attr_overrides: Any additional attributes to pass to the new,
-            dynamically created class created by the resulting decorator.
-
-    Returns:
-        (callable): A decorator that takes creates a new subclass of
-            :param:`parent_class` that uses the wrapped function as the return value of
-            :meth:`_io_defining_function` for the :class:`DecoratedNode` mixin.
-    """
-    if getattr(parent_class, io_static_method.__name__) is not io_static_method:
-        raise ValueError(
-            f"{io_static_method.__name__} is not a method on {parent_class}"
-        )
-    if not isinstance(io_static_method, FunctionType):
-        raise TypeError(f"{io_static_method.__name__} should be a static method")
-
-    def as_decorated_node_decorator(
-        *output_labels: str,
-        validate_output_labels: bool = True,
-    ):
-        output_labels = None if len(output_labels) == 0 else output_labels
-
-        def as_decorated_node(io_defining_function: callable):
-            if not callable(io_defining_function):
-                raise AttributeError(
-                    f"Tried to create a new child class of {parent_class.__name__}, "
-                    f"but got {io_defining_function} instead of a callable."
-                )
-
-            decorated_node_class = type(
-                io_defining_function.__name__,
-                (parent_class,),  # Define parentage
-                {
-                    io_static_method.__name__: staticmethod(io_defining_function),
-                    "__module__": io_defining_function.__module__,
-                    "_output_labels": output_labels,
-                    "_validate_output_labels": validate_output_labels,
-                    **parent_class_attr_overrides,
-                },
-            )
-            decorated_node_class.preview_io()  # Construct everything
-            return decorated_node_class
-
-        return as_decorated_node
-
-    as_decorated_node_decorator.__doc__ = dedent(
-        f"""
-        A decorator for dynamically creating `{parent_class.__name__}` sub-classes by 
-        wrapping a function as the `{io_static_method.__name__}`.
-        
-        The returned subclass uses the wrapped function (and optionally any provided 
-        :param:`output_labels`) to specify its IO.
-        
-        {decorator_docstring_additions}
-        
-        Args:
-            *output_labels (str): A name for each return value of the graph creating
-                function. When empty, scrapes output labels automatically from the
-                source code of the wrapped function. This can be useful when returned
-                values are not well named, e.g. to make the output channel 
-                dot-accessible if it would otherwise have a label that requires 
-                item-string-based access. Additionally, specifying a _single_ label for 
-                a wrapped function that returns a tuple of values ensures that a 
-                _single_ output channel (holding the tuple) is created, instead of one 
-                channel for each return value. The default approach of extracting 
-                labels from the function source code also requires that the function 
-                body contain _at most_ one `return` expression, so providing explicit 
-                labels can be used to circumvent this (at your own risk). (Default is 
-                empty, try to scrape labels from the source code of the wrapped 
-                function.)
-            validate_output_labels (bool): Whether to compare the provided output labels
-                (if any) against the source code (if available). (Default is True.)
-                
-        Returns:
-            (callable[[callable], type[{parent_class.__name__}]]): A decorator that 
-                transforms a function into a child class of `{parent_class.__name__}` 
-                using the decorated function as 
-                `{parent_class.__name__}.{io_static_method.__name__}`.
-        """
-    )
-    return as_decorated_node_decorator
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/job.py` & `pyiron_workflow-0.7.0/pyiron_workflow/job.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,21 @@
 take values _other_ than an actual executor instance (which don't serialize). The
 infrastructure is in place for this in :meth:`Node._parse_executor`, but it is not yet
 leveraged.
 """
 
 from __future__ import annotations
 
+import base64
 import inspect
 import os
 import sys
 
+import cloudpickle
+
 from pyiron_base import TemplateJob, JOB_CLASS_DICT
 from pyiron_base.jobs.flex.pythonfunctioncontainer import (
     PythonFunctionContainerJob,
     get_function_parameter_dict,
 )
 from pyiron_workflow.node import Node
 from h5io._h5io import _import_class
@@ -99,33 +102,59 @@
             raise TypeError(f"'node' input must be of type {Node.__name__}")
         elif not self.input["node"].ready:
             nl = "\n"
             raise ValueError(
                 f"Node not ready:{nl}{self.input['node'].readiness_report}"
             )
 
+    def save(self):
+        # DataContainer can't handle custom reconstructors, so convert the node to
+        # bytestream
+        self.input["node"] = base64.b64encode(
+            cloudpickle.dumps(self.input["node"])
+        ).decode("utf-8")
+        super().save()
+
     def run_static(self):
         # Overrides the parent method
         # Copy and paste except for the output update, which makes sure the output is
         # flat and not tested beneath "result"
+
+        # Unpack the node
+        input_dict = self.input.to_builtin()
+        input_dict["node"] = cloudpickle.loads(base64.b64decode(self.input["node"]))
+
         if (
             self._executor_type is not None
             and "executor" in inspect.signature(self._function).parameters.keys()
         ):
-            input_dict = self.input.to_builtin()
             del input_dict["executor"]
             output = self._function(
                 **input_dict, executor=self._get_executor(max_workers=self.server.cores)
             )
         else:
-            output = self._function(**self.input.to_builtin())
+            output = self._function(**input_dict)
         self.output.update(output)  # DIFFERS FROM PARENT METHOD
         self.to_hdf()
         self.status.finished = True
 
+    def get_input_node(self):
+        """
+        On saving, we turn the input node into a bytestream so that the DataContainer
+        can store it. You might want to look at it again though, so you can use this
+        to unpack it
+
+        Returns:
+            (Node): The input node as a node again
+        """
+        if isinstance(self.input["node"], Node):
+            return self.input["node"]
+        else:
+            return cloudpickle.loads(base64.b64decode(self.input["node"]))
+
 
 JOB_CLASS_DICT[NodeOutputJob.__name__] = NodeOutputJob.__module__
 
 
 class NodeJob(NodeOutputJob):
     # Just to expose it under the simpler name per @JNmpi's request
     # This is a temporary change ahead of the 2024 DPG conference,
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/macro.py` & `pyiron_workflow-0.7.0/pyiron_workflow/macro.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 from abc import ABC, abstractmethod
 import re
 from typing import Literal, Optional, TYPE_CHECKING
 
 from pyiron_workflow.composite import Composite
 from pyiron_workflow.has_interface_mixins import HasChannel
 from pyiron_workflow.io import Outputs, Inputs
-from pyiron_workflow.io_preview import DecoratedNode, decorated_node_decorator_factory
+from pyiron_workflow.io_preview import StaticNode, ScrapesIO
+from pyiron_workflow.snippets.factory import classfactory
 
 if TYPE_CHECKING:
     from pyiron_workflow.channels import Channel
 
 
-class Macro(Composite, DecoratedNode, ABC):
+class Macro(Composite, StaticNode, ScrapesIO, ABC):
     """
     A macro is a composite node that holds a graph with a fixed interface, like a
     pre-populated workflow that is the same every time you instantiate it.
 
     At instantiation, the macro uses a provided callable to build and wire the graph,
     then builds a static IO interface for this graph.
     This callable must use the macro object itself as the first argument (e.g. adding
@@ -466,78 +467,127 @@
         for inp, (child, child_inp) in input_links:
             self.inputs[inp].value_receiver = self.children[child].inputs[child_inp]
 
         for (child, child_out), out in output_links:
             self.children[child].outputs[child_out].value_receiver = self.outputs[out]
 
 
-as_macro_node = decorated_node_decorator_factory(
-    Macro,
-    Macro.graph_creator,
-    decorator_docstring_additions="The first argument in the wrapped function is "
-    "`self`-like and will receive the macro instance "
-    "itself, and thus is ignored in the IO.",
-)
-
-
-def macro_node(
-    graph_creator,
-    label: Optional[str] = None,
-    parent: Optional[Composite] = None,
-    overwrite_save: bool = False,
-    run_after_init: bool = False,
-    storage_backend: Optional[Literal["h5io", "tinybase"]] = None,
-    save_after_run: bool = False,
-    strict_naming: bool = True,
-    output_labels: Optional[str | list[str] | tuple[str]] = None,
-    validate_output_labels: bool = True,
-    **kwargs,
+@classfactory
+def macro_node_factory(
+    graph_creator: callable, validate_output_labels: bool, /, *output_labels
 ):
-    """
-    Creates a new child of :class:`Macro` using the provided
-    :func:`graph_creator` and returns an instance of that.
-
-    Quacks like a :class:`Composite` for the sake of creating and registering nodes.
+    return (
+        graph_creator.__name__,
+        (Macro,),  # Define parentage
+        {
+            "graph_creator": staticmethod(graph_creator),
+            "__module__": graph_creator.__module__,
+            "_output_labels": None if len(output_labels) == 0 else output_labels,
+            "_validate_output_labels": validate_output_labels,
+        },
+        {},
+    )
 
-    Beyond the standard :class:`Macro`, initialization allows the args...
 
-    Args:
-        graph_creator (callable): The function defining macro's graph.
-        output_labels (Optional[str | list[str] | tuple[str]]): A name for each return
-            value of the node function OR a single label. (Default is None, which
-            scrapes output labels automatically from the source code of the wrapped
-            function.) This can be useful when returned values are not well named, e.g.
-            to make the output channel dot-accessible if it would otherwise have a label
-            that requires item-string-based access. Additionally, specifying a _single_
-            label for a wrapped function that returns a tuple of values ensures that a
-            _single_ output channel (holding the tuple) is created, instead of one
-            channel for each return value. The default approach of extracting labels
-            from the function source code also requires that the function body contain
-            _at most_ one `return` expression, so providing explicit labels can be used
-            to circumvent this (at your own risk), or to circumvent un-inspectable
-            source code (e.g. a function that exists only in memory).
-    """
-    if not callable(graph_creator):
-        # `function_node` quacks like a class, even though it's a function and
-        # dynamically creates children of `Macro` by providing the necessary
-        # callable to the decorator
-        raise AttributeError(
-            f"Expected `graph_creator` to be callable but got {graph_creator}"
+def as_macro_node(*output_labels, validate_output_labels=True):
+    def decorator(node_function):
+        macro_node_factory.clear(node_function.__name__)  # Force a fresh class
+        factory_made = macro_node_factory(
+            node_function, validate_output_labels, *output_labels
         )
+        factory_made._class_returns_from_decorated_function = node_function
+        factory_made.preview_io()
+        return factory_made
 
+    return decorator
+
+
+def macro_node(
+    node_function,
+    *node_args,
+    output_labels=None,
+    validate_output_labels=True,
+    **node_kwargs,
+):
     if output_labels is None:
         output_labels = ()
     elif isinstance(output_labels, str):
         output_labels = (output_labels,)
-
-    return as_macro_node(*output_labels, validate_output_labels=validate_output_labels)(
-        graph_creator
-    )(
-        label=label,
-        parent=parent,
-        overwrite_save=overwrite_save,
-        run_after_init=run_after_init,
-        storage_backend=storage_backend,
-        save_after_run=save_after_run,
-        strict_naming=strict_naming,
-        **kwargs,
+    macro_node_factory.clear(node_function.__name__)  # Force a fresh class
+    factory_made = macro_node_factory(
+        node_function, validate_output_labels, *output_labels
     )
+    factory_made.preview_io()
+    return factory_made(*node_args, **node_kwargs)
+
+
+# as_macro_node = decorated_node_decorator_factory(
+#     Macro,
+#     Macro.graph_creator,
+#     decorator_docstring_additions="The first argument in the wrapped function is "
+#     "`self`-like and will receive the macro instance "
+#     "itself, and thus is ignored in the IO.",
+# )
+#
+#
+# def macro_node(
+#     graph_creator,
+#     label: Optional[str] = None,
+#     parent: Optional[Composite] = None,
+#     overwrite_save: bool = False,
+#     run_after_init: bool = False,
+#     storage_backend: Optional[Literal["h5io", "tinybase"]] = None,
+#     save_after_run: bool = False,
+#     strict_naming: bool = True,
+#     output_labels: Optional[str | list[str] | tuple[str]] = None,
+#     validate_output_labels: bool = True,
+#     **kwargs,
+# ):
+#     """
+#     Creates a new child of :class:`Macro` using the provided
+#     :func:`graph_creator` and returns an instance of that.
+#
+#     Quacks like a :class:`Composite` for the sake of creating and registering nodes.
+#
+#     Beyond the standard :class:`Macro`, initialization allows the args...
+#
+#     Args:
+#         graph_creator (callable): The function defining macro's graph.
+#         output_labels (Optional[str | list[str] | tuple[str]]): A name for each return
+#             value of the node function OR a single label. (Default is None, which
+#             scrapes output labels automatically from the source code of the wrapped
+#             function.) This can be useful when returned values are not well named, e.g.
+#             to make the output channel dot-accessible if it would otherwise have a label
+#             that requires item-string-based access. Additionally, specifying a _single_
+#             label for a wrapped function that returns a tuple of values ensures that a
+#             _single_ output channel (holding the tuple) is created, instead of one
+#             channel for each return value. The default approach of extracting labels
+#             from the function source code also requires that the function body contain
+#             _at most_ one `return` expression, so providing explicit labels can be used
+#             to circumvent this (at your own risk), or to circumvent un-inspectable
+#             source code (e.g. a function that exists only in memory).
+#     """
+#     if not callable(graph_creator):
+#         # `function_node` quacks like a class, even though it's a function and
+#         # dynamically creates children of `Macro` by providing the necessary
+#         # callable to the decorator
+#         raise AttributeError(
+#             f"Expected `graph_creator` to be callable but got {graph_creator}"
+#         )
+#
+#     if output_labels is None:
+#         output_labels = ()
+#     elif isinstance(output_labels, str):
+#         output_labels = (output_labels,)
+#
+#     return as_macro_node(*output_labels, validate_output_labels=validate_output_labels)(
+#         graph_creator
+#     )(
+#         label=label,
+#         parent=parent,
+#         overwrite_save=overwrite_save,
+#         run_after_init=run_after_init,
+#         storage_backend=storage_backend,
+#         save_after_run=save_after_run,
+#         strict_naming=strict_naming,
+#         **kwargs,
+#     )
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/node.py` & `pyiron_workflow-0.7.0/pyiron_workflow/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,61 +104,70 @@
     - Nodes can be instructed to run at the end of their initialization, but will exit
         cleanly if they get to checking their readiness and find they are not ready
     - Nodes have a label by which they are identified
     - Nodes may open a working directory related to their label, their parent(age) and
         the python process working directory
     - Nodes can run their computation using remote resources by setting an executor
         - Any executor must have a :meth:`submit` method with the same interface as
-            :class:`concurrent.futures.Executor`, must return a :class:`concurrent.futures.Future`
-            (or child thereof) object, and must be able to serialize dynamically
-            defined objects
+            :class:`concurrent.futures.Executor`, must return a
+            :class:`concurrent.futures.Future` (or child thereof) object.
+        - Standard available nodes are pickleable and work with
+            `concurrent.futures.ProcessPoolExecutor`, but if you define your node
+            somewhere that it can't be imported (e.g. `__main__` in a jupyter
+            notebook), or it is otherwise not pickleable (e.g. it holds un-pickleable
+            io data), you will need a more powerful executor, e.g. `pympipool.Executor`.
         - On executing this way, a futures object will be returned instead of the usual
             result, this future will also be stored as an attribute, and a callback will
             be registered with the executor
         - Post-execution processing -- e.g. updating output and firing signals -- will
             not occur until the futures object is finished and the callback fires.
-        - WARNING: Executors are currently only working when the node executable
-            function does not use `self`
         - NOTE: Executors are only allowed in a "push" paradigm, and you will get an
             exception if you try to :meth:`pull` and one of the upstream nodes uses an
             executor
-        - NOTE: Don't forget to :meth:`shutdown` any created executors outside of a `with`
-            context when you're done with them; we give a convenience method for this.
+        - NOTE: Don't forget to :meth:`shutdown` any created executors outside of a
+            `with` context when you're done with them; we give a convenience method for
+            this.
     - Nodes created from a registered package store their package identifier as a class
         attribute.
     - [ALPHA FEATURE] Nodes can be saved to and loaded from file if python >= 3.11.
+        - As long as you haven't put anything unpickleable on them, or defined them in
+            an unpicklable place (e.g. in the `<locals>` of another function), you can
+            simple (un)pickle nodes. There is no save/load interface for this right
+            now, just import pickle and do it.
         - Saving is triggered manually, or by setting a flag to save after the nodes
             runs.
-        - On instantiation, nodes will load automatically if they find saved content.
+        - At the end of instantiation, nodes will load automatically if they find saved
+            content.
           - Discovered content can instead be deleted with a kwarg.
           - You can't load saved content _and_ run after instantiation at once.
-        - The nodes must be somewhere importable, and the imported object must match
-            the type of the node being saved. This basically just rules out one edge
-            case where a node class is defined like
-            `SomeFunctionNode = Workflow.wrap.as_function_node()(some_function)`, since
-            then the new class gets the name `some_function`, which when imported is
-            the _function_ "some_function" and not the desired class "SomeFunctionNode".
-            This is checked for at save-time and will cause a nice early failure.
+        - The nodes must be defined somewhere importable, i.e. in a module, `__main__`,
+            and as a class property are all fine, but, e.g., inside the `<locals>` of
+            another function is not.
         - [ALPHA ISSUE] If the source code (cells, `.py` files...) for a saved graph is
             altered between saving and loading the graph, there are no guarantees about
             the loaded state; depending on the nature of the changes everything may
             work fine with the new node definition, the graph may load but silently
             behave unexpectedly (e.g. if node functionality has changed but the
             interface is the same), or may crash on loading (e.g. if IO channel labels
             have changed).
         - [ALPHA ISSUE] There is no filtering available, saving a node stores all of
             its IO and does the same thing recursively for its children; depending on
             your graph this could be expensive in terms of storage space and/or time.
         - [ALPHA ISSUE] Similarly, there is no way to save only part of a graph; only
             the entire graph may be saved at once.
         - [ALPHA ISSUE] There are two possible back-ends for saving: one leaning on
             `tinybase.storage.GenericStorage` (in practice,
-            `H5ioStorage(GenericStorage)`), and the other, default back-end that uses
-            the `h5io` module directly. The backend used is always the one on the graph
-            root.
+            `H5ioStorage(GenericStorage)`), that is the default, and the other that
+            uses the `h5io` module directly. The backend used is always the one on the
+            graph root.
+        - [ALPHA ISSUE] The `h5io` backend is deprecated -- it can't handle custom
+            reconstructors (i.e. when `__reduce__` returns a tuple with some
+            non-standard callable as its first entry), and basically all our nodes do
+            that now! `tinybase` gets around this by falling back on `cloudpickle` when
+            its own interactions with `h5io` fail.
         - [ALPHA ISSUE] Restrictions on data:
             - For the `h5io` backend: Most data that can be pickled will be fine, but
                 some classes will hit an edge case and throw an exception from `h5io`
                 (at a minimum, those classes which define a custom reconstructor hit,
                 this, but there also seems to be issues with dynamic methods, e.g. the
                 `Calculator` class and its children from `ase`).
             - For the `tinybase` backend: Any data that can be pickled will be fine,
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/calculator.py` & `pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/calculator.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/macro.py` & `pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/macro.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/node_library/atomistics/task.py` & `pyiron_workflow-0.7.0/pyiron_workflow/node_library/atomistics/task.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/node_library/pyiron_atomistics.py` & `pyiron_workflow-0.7.0/pyiron_workflow/node_library/pyiron_atomistics.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/node_library/standard.py` & `pyiron_workflow-0.7.0/pyiron_workflow/node_library/standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Common-use nodes relying only on the standard library
 """
 
 from __future__ import annotations
 
 import random
+from time import sleep
 
 from pyiron_workflow.channels import NOT_DATA, OutputSignal
 from pyiron_workflow.function import Function, as_function_node
 
 
 @as_function_node()
 def UserInput(user_input):
@@ -48,14 +49,20 @@
 
 
 @as_function_node("random")
 def RandomFloat():
     return random.random()
 
 
+@as_function_node("time")
+def Sleep(t):
+    sleep(t)
+    return t
+
+
 @as_function_node("slice")
 def Slice(start=None, stop=NOT_DATA, step=None):
     if start is None:
         if stop is None:
             raise ValueError(
                 "Slice must define at least start or stop, but both are None"
             )
@@ -287,13 +294,14 @@
     NotEquals,
     Or,
     Positive,
     Power,
     RandomFloat,
     RightMultiply,
     Round,
+    Sleep,
     Slice,
     String,
     Subtract,
     UserInput,
     XOr,
 ]
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/node_package.py` & `pyiron_workflow-0.7.0/pyiron_workflow/node_package.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/output_parser.py` & `pyiron_workflow-0.7.0/pyiron_workflow/output_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Inspects code to automatically parse return values as strings
 """
 
 import ast
+from functools import lru_cache
 import inspect
 import re
 from textwrap import dedent
 
 
 def _remove_spaces_until_character(string):
     pattern = r"\s+(?=\s)"
@@ -22,15 +23,14 @@
     This parsed value is evaluated at instantiation and stored in the `output`
     attribute.
     In case more than one `return` expression is found, a `ValueError` is raised.
     """
 
     def __init__(self, function):
         self._func = function
-        self._source = None
         self._output = self.get_parsed_output()
 
     @property
     def func(self):
         return self._func
 
     @property
@@ -53,18 +53,17 @@
 
         try:
             return returns[0]
         except IndexError:
             return None
 
     @property
+    @lru_cache(maxsize=1)
     def source(self):
-        if self._source is None:
-            self._source = self.dedented_source_string.split("\n")[:-1]
-        return self._source
+        return self.dedented_source_string.split("\n")[:-1]
 
     def get_string(self, node):
         string = ""
         for ll in range(node.lineno - 1, node.end_lineno):
             if ll == node.lineno - 1 == node.end_lineno - 1:
                 string += _remove_spaces_until_character(
                     self.source[ll][node.col_offset : node.end_col_offset]
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/run.py` & `pyiron_workflow-0.7.0/pyiron_workflow/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 A module to extract encapsulate for complex run mechanics, such as status, executor
 interaction, etc.
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from concurrent.futures import Executor as StdLibExecutor, Future
+from concurrent.futures import Executor as StdLibExecutor, Future, ThreadPoolExecutor
+from time import sleep
 from typing import Any, Optional
 
 from pyiron_workflow.has_interface_mixins import HasLabel, HasRun, UsesState
 
 
 def manage_status(status_managed_method):
     """
@@ -46,17 +47,17 @@
 
 
 class Runnable(UsesState, HasLabel, HasRun, ABC):
     """
     An abstract class for interfacing with executors, etc.
 
     Child classes must define :meth:`on_run` and :attr:`.Runnable.run_args`, then the
-    :meth:`run` will invoke `on_run(**run_args)`. The :class:`Runnable` class then
-    handles the status of the run, passing the call off for remote execution, handling
-    any returned futures object, etc.
+    :meth:`run` will invoke `self.on_run(*run_args[0], **run_args[1])`. The
+    :class:`Runnable` class then handles the status of the run, passing the call off
+    for remote execution, handling any returned futures object, etc.
 
     Child classes can optionally override :meth:`process_run_result` to do something
     with the returned value of :meth:`on_run`, but by default the returned value just
     passes cleanly through the function.
     """
 
     def __init__(self, *args, **kwargs):
@@ -64,28 +65,27 @@
         self.running = False
         self.failed = False
         self.executor = None
         # We call it an executor, but it's just whether to use one.
         # This is a simply stop-gap as we work out more sophisticated ways to reference
         # (or create) an executor process without ever trying to pickle a `_thread.lock`
         self.future: None | Future = None
+        self._thread_pool_sleep_time = 1e-6
 
-    @property
     @abstractmethod
-    def on_run(self) -> callable[..., Any | tuple]:
+    def on_run(self, *args, **kwargs) -> Any:  # callable[..., Any | tuple]:
         """
         What the :meth:`run` method actually does!
         """
-        pass
 
     @property
     @abstractmethod
-    def run_args(self) -> dict:
+    def run_args(self) -> tuple[tuple, dict]:
         """
-        Any data needed for :meth:`on_run`, will be passed as **kwargs.
+        Any data needed for :meth:`on_run`, will be passed as (*args, **kwargs).
         """
 
     def process_run_result(self, run_output):
         """
         What to _do_ with the results of :meth:`on_run` once you have them.
 
         By extracting this as a separate method, we allow the runnable to pass the
@@ -164,32 +164,41 @@
 
     @manage_status
     def _run(
         self,
         finished_callback: callable,
         force_local_execution: bool,
     ) -> Any | tuple | Future:
+        args, kwargs = self.run_args
+        if "self" in kwargs.keys():
+            raise ValueError(
+                f"{self.label} got 'self' as a run kwarg, but self is already the "
+                f"first positional argument passed to :meth:`on_run`."
+            )
         if force_local_execution or self.executor is None:
             # Run locally
-            run_output = self.on_run(**self.run_args)
+            run_output = self.on_run(*args, **kwargs)
             return finished_callback(run_output)
         else:
             # Just blindly try to execute -- as we nail down the executor interaction
             # we'll want to fail more cleanly here.
             executor = self._parse_executor(self.executor)
-            kwargs = self.run_args
-            if "self" in kwargs.keys():
-                raise ValueError(
-                    f"{self.label} got 'self' as a run argument, but self cannot "
-                    f"currently be combined with running on executors."
-                )
-            self.future = executor.submit(self.on_run, **kwargs)
+            if isinstance(self.executor, ThreadPoolExecutor):
+                self.future = executor.submit(self.thread_pool_run, *args, **kwargs)
+            else:
+                self.future = executor.submit(self.on_run, *args, **kwargs)
             self.future.add_done_callback(finished_callback)
             return self.future
 
+    def thread_pool_run(self, *args, **kwargs):
+        #
+        result = self.on_run(*args, **kwargs)
+        sleep(self._thread_pool_sleep_time)
+        return result
+
     @staticmethod
     def _parse_executor(executor) -> StdLibExecutor:
         """
         We may want to allow users to specify how to build an executor rather than
         actually providing an executor instance -- so here we can interpret these.
 
         NOTE:
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/semantics.py` & `pyiron_workflow-0.7.0/pyiron_workflow/semantics.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,40 +89,20 @@
     def semantic_root(self) -> Semantic:
         """The parent-most object in this semantic path; may be self."""
         return self.parent.semantic_root if isinstance(self.parent, Semantic) else self
 
     def __getstate__(self):
         state = super().__getstate__()
         state["_parent"] = None
-        # Comment on moving this to semantics)
+        # Regarding removing parent from state:
         # Basically we want to avoid recursion during (de)serialization; when the
         # parent object is deserializing itself, _it_ should know who its children are
         # and inform them of this.
-        #
-        # Original comment when this behaviour belonged to node)
-        # I am not at all confident that removing the parent here is the _right_
-        # solution.
-        # In order to run composites on a parallel process, we ship off just the nodes
-        # and starting nodes.
-        # When the parallel process returns these, they're obviously different
-        # instances, so we re-parent them back to the receiving composite.
-        # At the same time, we want to make sure that the _old_ children get orphaned.
-        # Of course, we could do that directly in the composite method, but it also
-        # works to do it here.
-        # Something I like about this, is it also means that when we ship groups of
-        # nodes off to another process with cloudpickle, they're definitely not lugging
-        # along their parent, its connections, etc. with them!
-        # This is all working nicely as demonstrated over in the macro test suite.
-        # However, I have a bit of concern that when we start thinking about
-        # serialization for storage instead of serialization to another process, this
-        # might introduce a hard-to-track-down bug.
-        # For now, it works and I'm going to be super pragmatic and go for it, but
-        # for the record I am admitting that the current shallowness of my understanding
-        # may cause me/us headaches in the future.
-        # -Liam
+        # In the case the object gets passed to another process using __getstate__,
+        # this also avoids dragging our whole semantic parent graph along with us.
         return state
 
 
 class CyclicPathError(ValueError):
     """
     To be raised when adding a child would result in a cyclic semantic path.
     """
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/single_output.py` & `pyiron_workflow-0.7.0/pyiron_workflow/single_output.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/snippets/colors.py` & `pyiron_workflow-0.7.0/pyiron_workflow/snippets/colors.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/snippets/dotdict.py` & `pyiron_workflow-0.7.0/pyiron_workflow/snippets/dotdict.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/snippets/files.py` & `pyiron_workflow-0.7.0/pyiron_workflow/snippets/files.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/snippets/has_post.py` & `pyiron_workflow-0.7.0/pyiron_workflow/snippets/has_post.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/snippets/logger.py` & `pyiron_workflow-0.7.0/pyiron_workflow/snippets/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/snippets/singleton.py` & `pyiron_workflow-0.7.0/pyiron_workflow/snippets/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/snippets/testcase.py` & `pyiron_workflow-0.7.0/pyiron_workflow/snippets/testcase.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/storage.py` & `pyiron_workflow-0.7.0/pyiron_workflow/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,18 +368,14 @@
 class HasH5ioStorage(HasStorage, ABC):
     @classmethod
     def _storage_interfaces(cls):
         interfaces = super(HasH5ioStorage, cls)._storage_interfaces()
         interfaces["h5io"] = H5ioStorage
         return interfaces
 
-    @classmethod
-    def default_backend(cls):
-        return "h5io"
-
 
 class HasTinybaseStorage(HasStorage, ABC):
     @classmethod
     def _storage_interfaces(cls):
         interfaces = super(HasTinybaseStorage, cls)._storage_interfaces()
         interfaces["tinybase"] = TinybaseStorage
         return interfaces
@@ -387,7 +383,11 @@
     @abstractmethod
     def to_storage(self, storage: TinybaseStorage):
         pass
 
     @abstractmethod
     def from_storage(self, storage: TinybaseStorage):
         pass
+
+    @classmethod
+    def default_backend(cls):
+        return "tinybase"
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/topology.py` & `pyiron_workflow-0.7.0/pyiron_workflow/topology.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/type_hinting.py` & `pyiron_workflow-0.7.0/pyiron_workflow/type_hinting.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/workflow.py` & `pyiron_workflow-0.7.0/pyiron_workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow/working.py` & `pyiron_workflow-0.7.0/pyiron_workflow/working.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow.egg-info/PKG-INFO` & `pyiron_workflow-0.7.0/pyiron_workflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_workflow
-Version: 0.6.0
+Version: 0.7.0
 Summary: Graph-and-node based workflow tools.
 Home-page: https://github.com/pyiron/pyiron_workflow
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: liamhuber@greyhavensolutions.com
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 3 - Alpha
@@ -17,20 +17,20 @@
 License-File: LICENSE
 Requires-Dist: bidict>=0.23.1
 Requires-Dist: cloudpickle>=3.0.0
 Requires-Dist: graphviz>=0.20.3
 Requires-Dist: h5io>=0.2.2
 Requires-Dist: h5io_browser>=0.0.12
 Requires-Dist: matplotlib>=3.8.4
-Requires-Dist: pyiron_base>=0.8.2
+Requires-Dist: pyiron_base>=0.8.3
 Requires-Dist: pyiron_contrib>=0.1.16
-Requires-Dist: pympipool>=0.7.17
+Requires-Dist: pympipool>=0.8.0
 Requires-Dist: toposort>=1.10
 Requires-Dist: typeguard>=4.2.1
 Provides-Extra: node-library
 Requires-Dist: ase>=3.22.1; extra == "node-library"
 Requires-Dist: atomistics>=0.1.27; extra == "node-library"
 Requires-Dist: numpy>=1.26.4; extra == "node-library"
 Requires-Dist: phonopy>=2.22.1; extra == "node-library"
-Requires-Dist: pyiron_atomistics>=0.5.3; extra == "node-library"
+Requires-Dist: pyiron_atomistics>=0.5.4; extra == "node-library"
 
 http://pyiron.org
```

### Comparing `pyiron_workflow-0.6.0/pyiron_workflow.egg-info/SOURCES.txt` & `pyiron_workflow-0.7.0/pyiron_workflow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,32 +6,33 @@
 pyiron_workflow/__init__.py
 pyiron_workflow/_tests.py
 pyiron_workflow/_version.py
 pyiron_workflow/channels.py
 pyiron_workflow/composite.py
 pyiron_workflow/create.py
 pyiron_workflow/draw.py
+pyiron_workflow/for_loop.py
 pyiron_workflow/function.py
 pyiron_workflow/has_interface_mixins.py
 pyiron_workflow/has_to_dict.py
 pyiron_workflow/injection.py
 pyiron_workflow/io.py
 pyiron_workflow/io_preview.py
 pyiron_workflow/job.py
 pyiron_workflow/loops.py
 pyiron_workflow/macro.py
-pyiron_workflow/meta.py
 pyiron_workflow/node.py
 pyiron_workflow/node_package.py
 pyiron_workflow/output_parser.py
 pyiron_workflow/run.py
 pyiron_workflow/semantics.py
 pyiron_workflow/single_output.py
 pyiron_workflow/storage.py
 pyiron_workflow/topology.py
+pyiron_workflow/transform.py
 pyiron_workflow/type_hinting.py
 pyiron_workflow/workflow.py
 pyiron_workflow/working.py
 pyiron_workflow.egg-info/PKG-INFO
 pyiron_workflow.egg-info/SOURCES.txt
 pyiron_workflow.egg-info/dependency_links.txt
 pyiron_workflow.egg-info/requires.txt
@@ -45,12 +46,13 @@
 pyiron_workflow/node_library/atomistics/__init__.py
 pyiron_workflow/node_library/atomistics/calculator.py
 pyiron_workflow/node_library/atomistics/macro.py
 pyiron_workflow/node_library/atomistics/task.py
 pyiron_workflow/snippets/__init__.py
 pyiron_workflow/snippets/colors.py
 pyiron_workflow/snippets/dotdict.py
+pyiron_workflow/snippets/factory.py
 pyiron_workflow/snippets/files.py
 pyiron_workflow/snippets/has_post.py
 pyiron_workflow/snippets/logger.py
 pyiron_workflow/snippets/singleton.py
 pyiron_workflow/snippets/testcase.py
```

### Comparing `pyiron_workflow-0.6.0/setup.py` & `pyiron_workflow-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,25 @@
     install_requires=[
         'bidict>=0.23.1',
         'cloudpickle>=3.0.0',
         'graphviz>=0.20.3',
         'h5io>=0.2.2',
         'h5io_browser>=0.0.12',
         'matplotlib>=3.8.4',
-        'pyiron_base>=0.8.2',
+        'pyiron_base>=0.8.3',
         'pyiron_contrib>=0.1.16',
-        'pympipool>=0.7.17',
+        'pympipool>=0.8.0',
         'toposort>=1.10',
         'typeguard>=4.2.1',
     ],
     extras_require={
         "node_library": [
             'ase>=3.22.1',
             'atomistics>=0.1.27',
             'numpy>=1.26.4',
             'phonopy>=2.22.1',
-            'pyiron_atomistics>=0.5.3',
+            'pyiron_atomistics>=0.5.4',
         ],
     },
     cmdclass=versioneer.get_cmdclass(),
 
     )
```

### Comparing `pyiron_workflow-0.6.0/versioneer.py` & `pyiron_workflow-0.7.0/versioneer.py`

 * *Files identical despite different names*

