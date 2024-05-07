# Comparing `tmp/folioflex-1.1.0.tar.gz` & `tmp/folioflex-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folioflex-1.1.0.tar", last modified: Sat Mar 16 05:50:02 2024, max compression
+gzip compressed data, was "folioflex-1.2.0.tar", last modified: Tue May  7 20:18:22 2024, max compression
```

## Comparing `folioflex-1.1.0.tar` & `folioflex-1.2.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.988414 folioflex-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-16 05:49:53.000000 folioflex-1.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-16 05:49:53.000000 folioflex-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11812 2024-03-16 05:50:02.988414 folioflex-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-03-16 05:49:53.000000 folioflex-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.976414 folioflex-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.976414 folioflex-1.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-16 05:49:53.000000 folioflex-1.1.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.976414 folioflex-1.1.0/folioflex/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.980414 folioflex-1.1.0/folioflex/budget/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/budget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19802 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/budget/budget.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/budget/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.980414 folioflex-1.1.0/folioflex/chatbot/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/chatbot/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/chatbot/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.980414 folioflex-1.1.0/folioflex/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/configs/budget_personal.ini
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/configs/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/configs/portfolio_dash.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/configs/portfolio_demo.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/configs/portfolio_personal.ini
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/configs/transactions_dash.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/configs/transactions_demo.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.980414 folioflex-1.1.0/folioflex/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/dashboard/dashboard_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/dashboard/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.984414 folioflex-1.1.0/folioflex/dashboard/pages/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/dashboard/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/dashboard/pages/budget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/dashboard/pages/ideas.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/dashboard/pages/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/dashboard/pages/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/dashboard/pages/personal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/dashboard/pages/sectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/dashboard/pages/stocks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.984414 folioflex-1.1.0/folioflex/market/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/market/screener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.984414 folioflex-1.1.0/folioflex/portfolio/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32371 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/portfolio/broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/portfolio/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/portfolio/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    68299 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/portfolio/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)    20733 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/portfolio/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.984414 folioflex-1.1.0/folioflex/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/utils/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/utils/cq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/utils/custom_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/utils/mailer.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-16 05:49:53.000000 folioflex-1.1.0/folioflex/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.988414 folioflex-1.1.0/folioflex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11812 2024-03-16 05:50:02.000000 folioflex-1.1.0/folioflex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-16 05:50:02.000000 folioflex-1.1.0/folioflex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 05:50:02.000000 folioflex-1.1.0/folioflex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-16 05:50:02.000000 folioflex-1.1.0/folioflex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-16 05:50:02.000000 folioflex-1.1.0/folioflex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-16 05:50:02.000000 folioflex-1.1.0/folioflex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-03-16 05:49:53.000000 folioflex-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 05:50:02.988414 folioflex-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-16 05:49:53.000000 folioflex-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 05:50:02.984414 folioflex-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-03-16 05:49:53.000000 folioflex-1.1.0/tests/test_budget.py
--rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-03-16 05:49:53.000000 folioflex-1.1.0/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-16 05:49:53.000000 folioflex-1.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-16 05:49:53.000000 folioflex-1.1.0/tests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.867471 folioflex-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 20:18:11.000000 folioflex-1.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-07 20:18:11.000000 folioflex-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-05-07 20:18:22.867471 folioflex-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-07 20:18:11.000000 folioflex-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.855471 folioflex-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.855471 folioflex-1.2.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-07 20:18:11.000000 folioflex-1.2.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.855471 folioflex-1.2.0/folioflex/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.859470 folioflex-1.2.0/folioflex/budget/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/budget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19802 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/budget/budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/budget/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.859470 folioflex-1.2.0/folioflex/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10679 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/chatbot/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/chatbot/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.859470 folioflex-1.2.0/folioflex/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/budget_personal.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/portfolio_dash.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/portfolio_demo.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/portfolio_personal.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/transactions_dash.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/configs/transactions_demo.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.859470 folioflex-1.2.0/folioflex/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/dashboard_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.863471 folioflex-1.2.0/folioflex/dashboard/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/ideas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/personal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/sectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/dashboard/pages/stocks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.863471 folioflex-1.2.0/folioflex/market/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/market/screener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.863471 folioflex-1.2.0/folioflex/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33000 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/portfolio/broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/portfolio/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/portfolio/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68299 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/portfolio/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20733 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/portfolio/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.863471 folioflex-1.2.0/folioflex/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/utils/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/utils/cq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/utils/custom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/utils/mailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 20:18:11.000000 folioflex-1.2.0/folioflex/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.867471 folioflex-1.2.0/folioflex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-05-07 20:18:22.000000 folioflex-1.2.0/folioflex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-07 20:18:22.000000 folioflex-1.2.0/folioflex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:18:22.000000 folioflex-1.2.0/folioflex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 20:18:22.000000 folioflex-1.2.0/folioflex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-07 20:18:22.000000 folioflex-1.2.0/folioflex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 20:18:22.000000 folioflex-1.2.0/folioflex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-07 20:18:11.000000 folioflex-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:18:22.867471 folioflex-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 20:18:11.000000 folioflex-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:18:22.867471 folioflex-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-07 20:18:11.000000 folioflex-1.2.0/tests/test_budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-07 20:18:11.000000 folioflex-1.2.0/tests/test_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-05-07 20:18:11.000000 folioflex-1.2.0/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-07 20:18:11.000000 folioflex-1.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-07 20:18:11.000000 folioflex-1.2.0/tests/test_wrappers.py
```

### Comparing `folioflex-1.1.0/LICENSE.md` & `folioflex-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/PKG-INFO` & `folioflex-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folioflex
-Version: 1.1.0
+Version: 1.2.0
 Summary: A collection of portfolio tracking capabilities
 Author-email: John Koestner <johnkoestner@outlook.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 John Koestner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,23 +50,23 @@
 Requires-Dist: dash-table>=4.0.2
 Requires-Dist: Flask>=1.1.1
 Requires-Dist: Flask-Compress>=1.4.0
 Requires-Dist: gunicorn>=19.9.0
 Requires-Dist: celery>=5.3.1
 Requires-Dist: flower>=2.0.0
 Requires-Dist: redis>=3.3.8
-Requires-Dist: g4f==0.1.9.3
+Requires-Dist: g4f==0.2.4.1
 Requires-Dist: hugchat>=0.3.8
 Requires-Dist: openai>=1.3.7
 Requires-Dist: seleniumbase>=4.22.0
 Provides-Extra: budget
 Requires-Dist: emoji>=2.9.0; extra == "budget"
 Requires-Dist: gensim>=4.3.2; extra == "budget"
 Requires-Dist: scikit-learn>=1.3.2; extra == "budget"
-Requires-Dist: scipy>=1.10.1; extra == "budget"
+Requires-Dist: scipy==1.10.1; extra == "budget"
 Requires-Dist: psycopg2-binary; extra == "budget"
 Provides-Extra: dev
 Requires-Dist: black>=23.7.0; extra == "dev"
 Requires-Dist: isort>=5.13.2; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: ruff>=0.1.5; extra == "dev"
@@ -343,15 +343,15 @@
 ```python
 from folioflex.utils import config_helper
 config_helper.set_log_level("DEBUG")
 ```
 
 ### Coverage
 
-To see the test coverage the following command is run in the root directory. This is also documented in the `.coveragerc` file.
+To see the test coverage the following command is run in the root directory.
 ```
 pytest --cov=folioflex --cov-report=html
 ```
 
 <hr>
 
 [Go to Top](#table-of-contents)
```

### Comparing `folioflex-1.1.0/README.md` & `folioflex-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
 ```python
 from folioflex.utils import config_helper
 config_helper.set_log_level("DEBUG")
 ```
 
 ### Coverage
 
-To see the test coverage the following command is run in the root directory. This is also documented in the `.coveragerc` file.
+To see the test coverage the following command is run in the root directory.
 ```
 pytest --cov=folioflex --cov-report=html
 ```
 
 <hr>
 
 [Go to Top](#table-of-contents)
```

### Comparing `folioflex-1.1.0/docs/source/conf.py` & `folioflex-1.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/budget/budget.py` & `folioflex-1.2.0/folioflex/budget/budget.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/budget/models.py` & `folioflex-1.2.0/folioflex/budget/models.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/chatbot/providers.py` & `folioflex-1.2.0/folioflex/chatbot/providers.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Creates chatbots from different providers.
 
 This section will be a work in progress as integrations will be refined
 over time depending on the openness and reliability of the data sources are.
 """
 
 import g4f
+import nest_asyncio
 from hugchat import hugchat
 from hugchat.login import Login
 from openai import OpenAI
 
 from folioflex.chatbot import scraper
 from folioflex.utils import config_helper, custom_logger
 
@@ -157,38 +158,44 @@
 
         Returns
         -------
         formatted_response : str
             the response from the chatbot
 
         """
+        nest_asyncio.apply()
         scrape_text = None
+        url = None
+        formatted_response = ""
         if not self.chatbot:
             raise ValueError("Please initialize the chatbot first.")
         if scrape_url:
             scrape_results = scraper.scrape_html(scrape_url, **kwargs)
             scrape_text = scrape_results["text"]
             url = scrape_results["url"]
+            formatted_response = f"{url}\n\n"
             if scrape_text is None:
                 return f"Did not find any text to scrape at {url}."
 
-        logger.info(f"querying the chatbot - G4F with {self.chatbot['provider']}")
+        logger.info(
+            f"querying the chatbot - G4F with {self.chatbot['provider'].__module__}"
+        )
         response = g4f.ChatCompletion.create(
             model=self.chatbot["model"],
             messages=[
                 {
                     "role": "user",
                     "content": f"{query} {scrape_text}",
                 }
             ],
             provider=self.chatbot["provider"],
             auth=self.chatbot["auth"],
             access_token=self.chatbot["access_token"],
         )
-        formatted_response = f"{url}\n\n"
+
         formatted_response += response
 
         return formatted_response
 
 
 class HugChatProvider(ChatBotProvider):
     """
@@ -226,15 +233,15 @@
         self.hugchat_password = hugchat_password or config_helper.HUGCHAT_PASSWORD
         if not self.hugchat_login or not self.hugchat_password:
             raise ValueError(
                 "Please provide a HugChat login and password "
                 "or set them in the config file."
             )
 
-        logger.info("logging in to HugChat with {}")
+        logger.info("logging in to HugChat")
         sign = Login(self.hugchat_login, self.hugchat_password)
         cookies = sign.login()
 
         # Create a ChatBot
         self.chatbot = hugchat.ChatBot(cookies=cookies.get_dict())
 
         return self.chatbot
@@ -255,37 +262,37 @@
         Returns
         -------
         formatted_response : str
             the response from the chatbot
 
         """
         scrape_text = None
+        url = None
+        web_search = kwargs.get("web_search", False)
+        formatted_response = ""
         if not self.chatbot:
             raise ValueError("Please initialize the chatbot first.")
         if scrape_url:
             scrape_results = scraper.scrape_html(scrape_url, **kwargs)
             scrape_text = scrape_results["text"]
             url = scrape_results["url"]
+            formatted_response = f"{url}\n\n"
             if scrape_text is None:
                 return f"Did not find any text to scrape at {url}."
 
-        logger.info("querying the chatbot - HugChat")
+        logger.info(f"querying the chatbot - HugChat - web_search: {web_search}")
         response = self.chatbot.query(
             f"{query} {scrape_text}",
-            web_search=True,
+            web_search=web_search,
         )
         formatted_response = [response["text"]]
-        for source in response.web_search_sources:
-            formatted_response.append(source.link)
-            formatted_response.append(source.title)
-            formatted_response.append(source.hostname)
-
-        # join as new lines
-        formatted_response = f"{url}\n\n"
-        formatted_response += "\n".join(formatted_response)
+        for source in response["web_search_sources"]:
+            formatted_response.append(source["link"])
+            formatted_response.append(source["title"])
+            formatted_response.append(source["hostname"])
 
         return formatted_response
 
 
 class OpenaiProvider(ChatBotProvider):
     """
     Wrapper for OpenAI.
@@ -339,20 +346,22 @@
         -------
         formatted_response : str
             the response from the chatbot
 
         """
         scrape_text = None
         url = None
+        formatted_response = ""
         if not self.chatbot:
             raise ValueError("Please initialize the chatbot first.")
         if scrape_url:
             scrape_results = scraper.scrape_html(scrape_url, **kwargs)
             scrape_text = scrape_results["text"]
             url = scrape_results["url"]
+            formatted_response = f"{url}\n\n"
             if scrape_text is None:
                 return f"Did not find any text to scrape at {url}."
 
         logger.info("querying the chatbot - OpenAI")
         response = self.chatbot.chat.completions.create(
             model=model,
             messages=[
@@ -361,11 +370,10 @@
                     "content": f"{query} {scrape_text}",
                 }
             ],
         )
 
         # TODO add in handler for rate limits
 
-        formatted_response = f"{url}\n\n"
         formatted_response += response.choices[0].message.content
 
         return formatted_response
```

### Comparing `folioflex-1.1.0/folioflex/chatbot/scraper.py` & `folioflex-1.2.0/folioflex/chatbot/scraper.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/configs/budget_personal.ini` & `folioflex-1.2.0/folioflex/configs/budget_personal.ini`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/configs/config.ini` & `folioflex-1.2.0/folioflex/configs/config.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # initialization file config
 # ----------------
 # there are some symbols that are special characters
 # `static`: used to separate sections from keys
 # `$`: used to reference an environment variable
 
 [credentials]
-ffx_username = admin
-ffx_password = folioflex
+ffx_username = folioflex
+ffx_password = strongpassword
 
 [api]
 fred_api = None
 yodlee_client_id = None
 yodlee_secret = None
 yodlee_endpoint = None
```

### Comparing `folioflex-1.1.0/folioflex/configs/portfolio_dash.ini` & `folioflex-1.2.0/folioflex/configs/portfolio_dash.ini`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/configs/portfolio_demo.ini` & `folioflex-1.2.0/folioflex/configs/portfolio_demo.ini`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/configs/portfolio_personal.ini` & `folioflex-1.2.0/folioflex/configs/portfolio_personal.ini`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/configs/transactions_dash.csv` & `folioflex-1.2.0/folioflex/configs/transactions_dash.csv`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/configs/transactions_demo.csv` & `folioflex-1.2.0/folioflex/configs/transactions_demo.csv`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/dashboard/dashboard_helper.py` & `folioflex-1.2.0/folioflex/dashboard/dashboard_helper.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/dashboard/layouts.py` & `folioflex-1.2.0/folioflex/dashboard/layouts.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/dashboard/pages/budget.py` & `folioflex-1.2.0/folioflex/dashboard/pages/budget.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/dashboard/pages/ideas.py` & `folioflex-1.2.0/folioflex/dashboard/pages/ideas.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/dashboard/pages/login.py` & `folioflex-1.2.0/folioflex/dashboard/pages/login.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/dashboard/pages/macro.py` & `folioflex-1.2.0/folioflex/dashboard/pages/macro.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/dashboard/pages/personal.py` & `folioflex-1.2.0/folioflex/dashboard/pages/personal.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/dashboard/pages/sectors.py` & `folioflex-1.2.0/folioflex/dashboard/pages/sectors.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/dashboard/pages/stocks.py` & `folioflex-1.2.0/folioflex/dashboard/pages/stocks.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/portfolio/broker.py` & `folioflex-1.2.0/folioflex/portfolio/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     ------------------------------------------
     - go to www.fidelity.com/
     - go to Activity & Orders
     - download data to .csv
 
     Notes
     -----
-    - The headers have started on line 6, if this changes need to update
+    - The headers seem to change, and if greater than 10 code should be updated
     - the date has had a space at beggining of string, so need to strip
 
     Parameters
     ----------
     broker_file : str
         path to transactions file that was downloaded from Ally
     output_file : str (optional)
@@ -142,24 +142,39 @@
         "DIVIDEND": "DIVIDEND",
         "CASH DISTRIBUTN": "Cash",
         "YOU BOUGHT": "BUY",
         "REINVESTMENT": "BUY",
         "YOU SOLD": "SELL",
     }
 
+    def find_header_row(broker_file):
+        with open(broker_file, "r") as file:
+            for i, line in enumerate(file):
+                if i >= 10:
+                    break
+                columns = [col.strip() for col in line.split(",")]
+                if "Run Date" in columns:
+                    logger.info(f"using header row at line {i}")
+                    return i
+        raise ValueError(
+            "Could not find column 'Run Date' in the first 10 lines of the file"
+        )
+
     # read in the transactions file
     try:
-        df = pd.read_csv(broker_file, skiprows=5)
+        skiprows = find_header_row(broker_file) - 1
+        df = pd.read_csv(broker_file, skiprows=skiprows)
     except FileNotFoundError:
         logger.error("Transactions file not found")
         return
 
     # cleaning dataframe by formatting columns and removing whitespace from strings
     df.columns = df.columns.str.strip().str.lower().str.replace(" ", "_")
-    df = df.applymap(lambda x: x.strip() if isinstance(x, str) else x)
+    for column in df.columns:
+        df[column] = df[column].map(lambda x: x.strip() if isinstance(x, str) else x)
 
     # remove footer of dataframe
     df_end = df[df["action"].isna()].index.min()
     if pd.notna(df_end):
         df = df.loc[: df_end - 1]
     else:
         pass
@@ -288,15 +303,15 @@
     df = df.apply(lambda x: x.strip() if isinstance(x, str) else x)
     df = df[df["symbol"] != "Symbol"]  # remove header rows not first row
     df["quantity"] = df["quantity"].astype(float)
     df["proceeds"] = df["proceeds"].astype(float)
     df["tradeprice"] = df["tradeprice"].astype(float)
 
     # update date column type
-    df["date"] = pd.to_datetime(df["datetime"]).dt.date
+    df["date"] = pd.to_datetime(df["datetime"], format="mixed").dt.date
 
     # Loop through each type_lkup and update type
     for string, tag in type_lkup.items():
         df.loc[
             df["description"].str.contains(r"\b" + string + r"\b", case=False), "type"
         ] = tag
```

### Comparing `folioflex-1.1.0/folioflex/portfolio/heatmap.py` & `folioflex-1.2.0/folioflex/portfolio/heatmap.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/portfolio/helper.py` & `folioflex-1.2.0/folioflex/portfolio/helper.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/portfolio/portfolio.py` & `folioflex-1.2.0/folioflex/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/portfolio/wrappers.py` & `folioflex-1.2.0/folioflex/portfolio/wrappers.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/utils/cli.py` & `folioflex-1.2.0/folioflex/utils/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,16 @@
         "-p",
         "--proxy",
         type=str,
         default=None,
         help=("The proxy to use for the chatbot - user:password@ip:port"),
     )
 
+    return _parser
+
 
 parser = _create_argparser()
 
 
 def cli():
     """Command line interface."""
     args = parser.parse_args()
```

### Comparing `folioflex-1.1.0/folioflex/utils/config_helper.py` & `folioflex-1.2.0/folioflex/utils/config_helper.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/utils/cq.py` & `folioflex-1.2.0/folioflex/utils/cq.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/utils/custom_logger.py` & `folioflex-1.2.0/folioflex/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex/utils/mailer.py` & `folioflex-1.2.0/folioflex/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/folioflex.egg-info/PKG-INFO` & `folioflex-1.2.0/folioflex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folioflex
-Version: 1.1.0
+Version: 1.2.0
 Summary: A collection of portfolio tracking capabilities
 Author-email: John Koestner <johnkoestner@outlook.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 John Koestner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,23 +50,23 @@
 Requires-Dist: dash-table>=4.0.2
 Requires-Dist: Flask>=1.1.1
 Requires-Dist: Flask-Compress>=1.4.0
 Requires-Dist: gunicorn>=19.9.0
 Requires-Dist: celery>=5.3.1
 Requires-Dist: flower>=2.0.0
 Requires-Dist: redis>=3.3.8
-Requires-Dist: g4f==0.1.9.3
+Requires-Dist: g4f==0.2.4.1
 Requires-Dist: hugchat>=0.3.8
 Requires-Dist: openai>=1.3.7
 Requires-Dist: seleniumbase>=4.22.0
 Provides-Extra: budget
 Requires-Dist: emoji>=2.9.0; extra == "budget"
 Requires-Dist: gensim>=4.3.2; extra == "budget"
 Requires-Dist: scikit-learn>=1.3.2; extra == "budget"
-Requires-Dist: scipy>=1.10.1; extra == "budget"
+Requires-Dist: scipy==1.10.1; extra == "budget"
 Requires-Dist: psycopg2-binary; extra == "budget"
 Provides-Extra: dev
 Requires-Dist: black>=23.7.0; extra == "dev"
 Requires-Dist: isort>=5.13.2; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: ruff>=0.1.5; extra == "dev"
@@ -343,15 +343,15 @@
 ```python
 from folioflex.utils import config_helper
 config_helper.set_log_level("DEBUG")
 ```
 
 ### Coverage
 
-To see the test coverage the following command is run in the root directory. This is also documented in the `.coveragerc` file.
+To see the test coverage the following command is run in the root directory.
 ```
 pytest --cov=folioflex --cov-report=html
 ```
 
 <hr>
 
 [Go to Top](#table-of-contents)
```

### Comparing `folioflex-1.1.0/folioflex.egg-info/SOURCES.txt` & `folioflex-1.2.0/folioflex.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -48,10 +48,11 @@
 folioflex/utils/__init__.py
 folioflex/utils/cli.py
 folioflex/utils/config_helper.py
 folioflex/utils/cq.py
 folioflex/utils/custom_logger.py
 folioflex/utils/mailer.py
 tests/test_budget.py
+tests/test_chatbot.py
 tests/test_portfolio.py
 tests/test_utils.py
 tests/test_wrappers.py
```

### Comparing `folioflex-1.1.0/folioflex.egg-info/requires.txt` & `folioflex-1.2.0/folioflex.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 dash-table>=4.0.2
 Flask>=1.1.1
 Flask-Compress>=1.4.0
 gunicorn>=19.9.0
 celery>=5.3.1
 flower>=2.0.0
 redis>=3.3.8
-g4f==0.1.9.3
+g4f==0.2.4.1
 hugchat>=0.3.8
 openai>=1.3.7
 seleniumbase>=4.22.0
 
 [budget]
 emoji>=2.9.0
 gensim>=4.3.2
 scikit-learn>=1.3.2
-scipy>=1.10.1
+scipy==1.10.1
 psycopg2-binary
 
 [dev]
 black>=23.7.0
 isort>=5.13.2
 pytest>=7.4.0
 pytest-cov>=4.1.0
```

### Comparing `folioflex-1.1.0/pyproject.toml` & `folioflex-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,26 +38,26 @@
 
     # worker
     "celery>=5.3.1",
     "flower>=2.0.0",
     "redis>=3.3.8",
 
     # gpt
-    "g4f==0.1.9.3",         # this package has loose testing support
+    "g4f==0.2.4.1",         # this package has loose testing support
     "hugchat>=0.3.8",
     "openai>=1.3.7",
     "seleniumbase>=4.22.0",
 ]
 
 [project.optional-dependencies]
 budget = [
     "emoji>=2.9.0",
     "gensim>=4.3.2",
     "scikit-learn>=1.3.2",
-    "scipy>=1.10.1",
+    "scipy==1.10.1",       # gensim needs to update to newest scipy 
     "psycopg2-binary",
 ]
 
 dev = [
     "black>=23.7.0",
     "isort>=5.13.2",
     "pytest>=7.4.0",
```

### Comparing `folioflex-1.1.0/tests/test_budget.py` & `folioflex-1.2.0/tests/test_budget.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/tests/test_portfolio.py` & `folioflex-1.2.0/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/tests/test_utils.py` & `folioflex-1.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `folioflex-1.1.0/tests/test_wrappers.py` & `folioflex-1.2.0/tests/test_wrappers.py`

 * *Files identical despite different names*

