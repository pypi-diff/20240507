# Comparing `tmp/multimetric-2.2.0.tar.gz` & `tmp/multimetric-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimetric-2.2.0.tar", last modified: Sat Jan 27 07:38:32 2024, max compression
+gzip compressed data, was "multimetric-2.2.1.tar", last modified: Tue May  7 05:32:52 2024, max compression
```

## Comparing `multimetric-2.2.0.tar` & `multimetric-2.2.1.tar`

### file list

```diff
@@ -1,50 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:32.673551 multimetric-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-01-27 07:38:20.000000 multimetric-2.2.0/LICENSE.Zlib
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-27 07:38:20.000000 multimetric-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-01-27 07:38:32.673551 multimetric-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-01-27 07:38:20.000000 multimetric-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:32.665551 multimetric-2.2.0/multimetric/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:32.669551 multimetric-2.2.0/multimetric/cls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/base_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/base_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:32.669551 multimetric-2.2.0/multimetric/cls/calc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/calc/halstead.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/calc/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/calc/pylint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/calc/tiobe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:32.669551 multimetric-2.2.0/multimetric/cls/importer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/importer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/importer/filtered.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:32.669551 multimetric-2.2.0/multimetric/cls/importer/mods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/importer/mods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/importer/mods/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/importer/mods/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/importer/pick.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:32.673551 multimetric-2.2.0/multimetric/cls/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/metric/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/metric/cyclomatic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/metric/fanout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/metric/loc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/metric/operands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/metric/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:32.673551 multimetric-2.2.0/multimetric/cls/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/stats/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-01-27 07:38:20.000000 multimetric-2.2.0/multimetric/cls/tokentree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 07:38:32.665551 multimetric-2.2.0/multimetric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-01-27 07:38:32.000000 multimetric-2.2.0/multimetric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-01-27 07:38:32.000000 multimetric-2.2.0/multimetric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-27 07:38:32.000000 multimetric-2.2.0/multimetric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-27 07:38:32.000000 multimetric-2.2.0/multimetric.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-27 07:38:32.000000 multimetric-2.2.0/multimetric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-27 07:38:20.000000 multimetric-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-01-27 07:38:32.673551 multimetric-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-01-27 07:38:32.000000 multimetric-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:52.410842 multimetric-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-07 05:32:39.000000 multimetric-2.2.1/LICENSE.Zlib
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 05:32:39.000000 multimetric-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-05-07 05:32:52.410842 multimetric-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-07 05:32:39.000000 multimetric-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:52.398842 multimetric-2.2.1/multimetric/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:52.402842 multimetric-2.2.1/multimetric/cls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/base_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/base_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:52.402842 multimetric-2.2.1/multimetric/cls/calc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/calc/halstead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/calc/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/calc/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/calc/tiobe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:52.402842 multimetric-2.2.1/multimetric/cls/importer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/importer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/importer/filtered.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:52.402842 multimetric-2.2.1/multimetric/cls/importer/mods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/importer/mods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/importer/mods/csv_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/importer/mods/json_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/importer/pick.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:52.402842 multimetric-2.2.1/multimetric/cls/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/metric/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/metric/cyclomatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/metric/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/metric/loc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/metric/operands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/metric/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:52.402842 multimetric-2.2.1/multimetric/cls/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/stats/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-07 05:32:39.000000 multimetric-2.2.1/multimetric/cls/tokentree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:52.410842 multimetric-2.2.1/multimetric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-05-07 05:32:52.000000 multimetric-2.2.1/multimetric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-07 05:32:52.000000 multimetric-2.2.1/multimetric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 05:32:52.000000 multimetric-2.2.1/multimetric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 05:32:52.000000 multimetric-2.2.1/multimetric.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 05:32:52.000000 multimetric-2.2.1/multimetric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 05:32:39.000000 multimetric-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-07 05:32:52.410842 multimetric-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-07 05:32:50.000000 multimetric-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:32:52.410842 multimetric-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_calc_halstead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_calc_maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_coffeescript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_cornercases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_csharp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_dart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_groovy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_haskell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_import_cornercases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_import_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_import_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_java.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_julia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_kotlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_lisp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_lua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_objective_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_perl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_php.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_rust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_tcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_typescript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-07 05:32:39.000000 multimetric-2.2.1/tests/test_zig.py
```

### Comparing `multimetric-2.2.0/LICENSE.Zlib` & `multimetric-2.2.1/LICENSE.Zlib`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/PKG-INFO` & `multimetric-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: multimetric
-Version: 2.2.0
+Version: 2.2.1
 Summary: Calculate code metrics in various languages
 Home-page: https://github.com/priv-kweihmann/multimetric
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: zlib/libpng License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -242,9 +240,7 @@
     B --> C(Create fanout settings)
     C --> D[Code your changes]
     D -->|Flake8 successful| E[Open PR]
     D -->|pytest successful| E[Open PR]
     D -->|Contribution guideline accepted| E[Open PR]
     D -->|README updated| E[Open PR]
 ```
-
-
```

### Comparing `multimetric-2.2.0/README.md` & `multimetric-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/__main__.py` & `multimetric-2.2.1/multimetric/__main__.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/base.py` & `multimetric-2.2.1/multimetric/cls/base.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/calc/halstead.py` & `multimetric-2.2.1/multimetric/cls/calc/halstead.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/calc/maintenance.py` & `multimetric-2.2.1/multimetric/cls/calc/maintenance.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,16 +125,16 @@
         try:
             res = 171.0
             res -= 5.2 * math.log(metrics["halstead_volume"])
             res -= 0.23 * metrics["cyclomatic_complexity"]
             res -= 16.2 * math.log(metrics["loc"])
             res *= 100.0 / 171.0
             return max(0, res)
-        except ValueError:
-            return 0
+        except ValueError:  # pragma: no cover
+            return 0  # pragma: no cover
 
     @staticmethod
     def _mi_classic(metrics):
         """Calculate the maintenance index using the classic method.
 
         Parameters
         ----------
```

### Comparing `multimetric-2.2.0/multimetric/cls/calc/pylint.py` & `multimetric-2.2.1/multimetric/cls/calc/pylint.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/calc/tiobe.py` & `multimetric-2.2.1/multimetric/cls/calc/tiobe.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/importer/base.py` & `multimetric-2.2.1/multimetric/cls/importer/base.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/importer/mods/csv.py` & `multimetric-2.2.1/multimetric/cls/importer/mods/csv_importer.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/importer/mods/json.py` & `multimetric-2.2.1/multimetric/cls/importer/mods/json_importer.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/importer/pick.py` & `multimetric-2.2.1/multimetric/cls/importer/pick.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2023 Konrad Weihmann
 # SPDX-License-Identifier: Zlib
 import os
 import logging
 
 from multimetric.cls.importer.base import Importer
-from multimetric.cls.importer.mods.csv import ImporterCSV
-from multimetric.cls.importer.mods.json import ImporterJSON
+from multimetric.cls.importer.mods.csv_importer import ImporterCSV
+from multimetric.cls.importer.mods.json_importer import ImporterJSON
 
 
 def importer_pick(args, filearg):  # noqa: CFQ004
     if not filearg:
         return None
     _file, _ext = os.path.splitext(filearg)
     if _ext in [".csv"]:
```

### Comparing `multimetric-2.2.0/multimetric/cls/metric/comments.py` & `multimetric-2.2.1/multimetric/cls/metric/comments.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/metric/cyclomatic.py` & `multimetric-2.2.1/multimetric/cls/metric/cyclomatic.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/metric/fanout.py` & `multimetric-2.2.1/multimetric/cls/metric/fanout.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/metric/loc.py` & `multimetric-2.2.1/multimetric/cls/metric/loc.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/metric/operands.py` & `multimetric-2.2.1/multimetric/cls/metric/operands.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/metric/operators.py` & `multimetric-2.2.1/multimetric/cls/metric/operators.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/modules.py` & `multimetric-2.2.1/multimetric/cls/modules.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/stats/stats.py` & `multimetric-2.2.1/multimetric/cls/stats/stats.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric/cls/tokentree.py` & `multimetric-2.2.1/multimetric/cls/tokentree.py`

 * *Files identical despite different names*

### Comparing `multimetric-2.2.0/multimetric.egg-info/PKG-INFO` & `multimetric-2.2.1/multimetric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: multimetric
-Version: 2.2.0
+Version: 2.2.1
 Summary: Calculate code metrics in various languages
 Home-page: https://github.com/priv-kweihmann/multimetric
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: zlib/libpng License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -242,9 +240,7 @@
     B --> C(Create fanout settings)
     C --> D[Code your changes]
     D -->|Flake8 successful| E[Open PR]
     D -->|pytest successful| E[Open PR]
     D -->|Contribution guideline accepted| E[Open PR]
     D -->|README updated| E[Open PR]
 ```
-
-
```

### Comparing `multimetric-2.2.0/setup.py` & `multimetric-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="multimetric",
-    version="2.2.0",
+    version="2.2.1",
     author="Konrad Weihmann",
     author_email="kweihmann@outlook.com",
     description="Calculate code metrics in various languages",
     long_description=_long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/priv-kweihmann/multimetric",
     packages=setuptools.find_packages(exclude=('tests',)),
```

