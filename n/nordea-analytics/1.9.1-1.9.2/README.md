# Comparing `tmp/nordea-analytics-1.9.1.tar.gz` & `tmp/nordea-analytics-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nordea-analytics-1.9.1.tar", last modified: Fri Aug 18 09:58:27 2023, max compression
+gzip compressed data, was "nordea-analytics-1.9.2.tar", last modified: Fri Aug 18 11:53:06 2023, max compression
```

## Comparing `nordea-analytics-1.9.1.tar` & `nordea-analytics-1.9.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:58:27.398617 nordea-analytics-1.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:58:27.374617 nordea-analytics-1.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:58:27.378617 nordea-analytics-1.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35801 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-18 09:58:27.398617 nordea-analytics-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-18 09:58:27.402618 nordea-analytics-1.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:58:27.374617 nordea-analytics-1.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:58:27.382617 nordea-analytics-1.9.1/src/nordea_analytics/
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/convention_variable_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/curve_variable_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/forecast_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/instrument_variable_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/key_figure_names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:58:27.386617 nordea-analytics-1.9.1/src/nordea_analytics/nalib/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/config_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/data_retrieval_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:58:27.386617 nordea-analytics-1.9.1/src/nordea_analytics/nalib/http/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/http/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/http/open_banking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:58:27.386617 nordea-analytics-1.9.1/src/nordea_analytics/nalib/live_keyfigures/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/live_keyfigures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/live_keyfigures/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/live_keyfigures/open_banking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/live_keyfigures/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/proxy_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:58:27.398617 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BenchmarkDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BondFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureHorizonCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BondKeyFigures.py
--rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BondRepoCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BondStaticData.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/Curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/CurveDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/CurveTimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/DateSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/FXForecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/FXQuotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/IndexComposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/LiveBondKeyFigures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/LiveBondUniverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/Quotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/ShiftDate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/ShiftDays.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/TimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/YearFraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/YieldForecast.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:58:27.398617 nordea-analytics-1.9.1/src/nordea_analytics/nordea_analytics_service/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nordea_analytics_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32666 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nordea_analytics_service/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nordea_analytics_service/open_banking.py
--rw-r--r--   0 runner    (1001) docker     (123)    27146 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/nordea_analytics_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/search_bond_names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:58:27.398617 nordea-analytics-1.9.1/src/nordea_analytics/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/shortcuts/open_banking.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/shortcuts/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/src/nordea_analytics/shortcuts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:58:27.382617 nordea-analytics-1.9.1/src/nordea_analytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-18 09:58:27.000000 nordea-analytics-1.9.1/src/nordea_analytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-18 09:58:27.000000 nordea-analytics-1.9.1/src/nordea_analytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-18 09:58:27.000000 nordea-analytics-1.9.1/src/nordea_analytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-18 09:58:27.000000 nordea-analytics-1.9.1/src/nordea_analytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-18 09:58:27.000000 nordea-analytics-1.9.1/src/nordea_analytics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:58:27.398617 nordea-analytics-1.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/tests/test_proxy_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-08-18 09:58:15.000000 nordea-analytics-1.9.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:53:06.519056 nordea-analytics-1.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:53:06.495055 nordea-analytics-1.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:53:06.499055 nordea-analytics-1.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35801 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-18 11:53:06.519056 nordea-analytics-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-18 11:53:06.519056 nordea-analytics-1.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:53:06.495055 nordea-analytics-1.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:53:06.503055 nordea-analytics-1.9.2/src/nordea_analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/convention_variable_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/curve_variable_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/forecast_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/instrument_variable_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/key_figure_names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:53:06.507056 nordea-analytics-1.9.2/src/nordea_analytics/nalib/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/config_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/data_retrieval_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:53:06.507056 nordea-analytics-1.9.2/src/nordea_analytics/nalib/http/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/http/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/http/open_banking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:53:06.507056 nordea-analytics-1.9.2/src/nordea_analytics/nalib/live_keyfigures/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/live_keyfigures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/live_keyfigures/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/live_keyfigures/open_banking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/live_keyfigures/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/proxy_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:53:06.515056 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BenchmarkDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BondFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureHorizonCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BondKeyFigures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BondRepoCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BondStaticData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/Curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/CurveDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/CurveTimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/DateSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/FXForecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/FXQuotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/IndexComposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/LiveBondKeyFigures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/LiveBondUniverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/Quotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/ShiftDate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/ShiftDays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/YearFraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/YieldForecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:53:06.515056 nordea-analytics-1.9.2/src/nordea_analytics/nordea_analytics_service/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nordea_analytics_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32666 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nordea_analytics_service/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nordea_analytics_service/open_banking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27146 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/nordea_analytics_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/search_bond_names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:53:06.519056 nordea-analytics-1.9.2/src/nordea_analytics/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/shortcuts/open_banking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/shortcuts/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/src/nordea_analytics/shortcuts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:53:06.503055 nordea-analytics-1.9.2/src/nordea_analytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-18 11:53:06.000000 nordea-analytics-1.9.2/src/nordea_analytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-18 11:53:06.000000 nordea-analytics-1.9.2/src/nordea_analytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-18 11:53:06.000000 nordea-analytics-1.9.2/src/nordea_analytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-18 11:53:06.000000 nordea-analytics-1.9.2/src/nordea_analytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-18 11:53:06.000000 nordea-analytics-1.9.2/src/nordea_analytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:53:06.519056 nordea-analytics-1.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/tests/test_proxy_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-08-18 11:52:52.000000 nordea-analytics-1.9.2/tests/test_util.py
```

### Comparing `nordea-analytics-1.9.1/.github/workflows/python-publish.yml` & `nordea-analytics-1.9.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/LICENCE.md` & `nordea-analytics-1.9.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/PKG-INFO` & `nordea-analytics-1.9.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nordea-analytics
-Version: 1.9.1
+Version: 1.9.2
 Summary: Nordea Analytics Python library
 Home-page: https://github.com/NordeaOSS/nordea-analytics
 Author: Nordea Desk Quants and Markets Advisory Tools
 Author-email: E-advisorySupport@nordea.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nordea-analytics-1.9.1/setup.cfg` & `nordea-analytics-1.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/__init__.py` & `nordea-analytics-1.9.2/src/nordea_analytics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 try:
     from .shortcuts.nordea import get_nordea_analytics_client  # type: ignore
     from .shortcuts.nordea import get_nordea_analytics_test_client  # type: ignore # noqa: E401
 except (NameError, ModuleNotFoundError):
     from .shortcuts.open_banking import get_nordea_analytics_client  # type: ignore
     from .shortcuts.open_banking import get_nordea_analytics_test_client  # type: ignore # noqa: F401
 
-__version__ = "1.9.1"
+__version__ = "1.9.2"
 __all__ = [
     "get_nordea_analytics_client",
     "get_nordea_analytics_test_client",
     "disable_analytics_warnings",
     "AmortisationType",
     "AssetType",
     "BenchmarkName",
```

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/convention_variable_names.py` & `nordea-analytics-1.9.2/src/nordea_analytics/convention_variable_names.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/curve_variable_names.py` & `nordea-analytics-1.9.2/src/nordea_analytics/curve_variable_names.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/forecast_names.py` & `nordea-analytics-1.9.2/src/nordea_analytics/forecast_names.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/instrument_variable_names.py` & `nordea-analytics-1.9.2/src/nordea_analytics/instrument_variable_names.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/key_figure_names.py` & `nordea-analytics-1.9.2/src/nordea_analytics/key_figure_names.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/auth.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/auth.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/config.yml` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/config.yml`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/config_test.yml` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/config_test.yml`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/data_retrieval_client.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/data_retrieval_client.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/exceptions.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/exceptions.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/http/core.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/http/core.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/http/open_banking.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/http/open_banking.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/live_keyfigures/open_banking.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/live_keyfigures/open_banking.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/live_keyfigures/parsing.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/live_keyfigures/parsing.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/proxy_finder.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/proxy_finder.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/util.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/util.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retriever.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retriever.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BenchmarkDefinition.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BenchmarkDefinition.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BondFinder.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BondFinder.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureCalculator.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureCalculator.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureHorizonCalculator.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BondKeyFigureHorizonCalculator.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BondKeyFigures.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BondKeyFigures.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BondRepoCalculator.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BondRepoCalculator.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/BondStaticData.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/BondStaticData.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/Curve.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/Curve.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/CurveDefinition.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/CurveDefinition.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/CurveTimeSeries.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/CurveTimeSeries.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/DateSequence.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/DateSequence.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/FXForecast.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/FXForecast.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/FXQuotes.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/FXQuotes.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/IndexComposition.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/IndexComposition.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/LiveBondKeyFigures.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/LiveBondKeyFigures.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/LiveBondUniverse.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/LiveBondUniverse.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/Quotes.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/Quotes.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/ShiftDate.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/ShiftDate.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/ShiftDays.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/ShiftDays.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/TimeSeries.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/YearFraction.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/YearFraction.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nalib/value_retrievers/YieldForecast.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nalib/value_retrievers/YieldForecast.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nordea_analytics_service/core.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nordea_analytics_service/core.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/nordea_analytics_service.py` & `nordea-analytics-1.9.2/src/nordea_analytics/nordea_analytics_service.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/search_bond_names.py` & `nordea-analytics-1.9.2/src/nordea_analytics/search_bond_names.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics/shortcuts/open_banking.py` & `nordea-analytics-1.9.2/src/nordea_analytics/shortcuts/open_banking.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics.egg-info/PKG-INFO` & `nordea-analytics-1.9.2/src/nordea_analytics.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nordea-analytics
-Version: 1.9.1
+Version: 1.9.2
 Summary: Nordea Analytics Python library
 Home-page: https://github.com/NordeaOSS/nordea-analytics
 Author: Nordea Desk Quants and Markets Advisory Tools
 Author-email: E-advisorySupport@nordea.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nordea-analytics-1.9.1/src/nordea_analytics.egg-info/SOURCES.txt` & `nordea-analytics-1.9.2/src/nordea_analytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/tests/test_proxy_finder.py` & `nordea-analytics-1.9.2/tests/test_proxy_finder.py`

 * *Files identical despite different names*

### Comparing `nordea-analytics-1.9.1/tests/test_util.py` & `nordea-analytics-1.9.2/tests/test_util.py`

 * *Files identical despite different names*

