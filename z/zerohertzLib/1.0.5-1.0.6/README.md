# Comparing `tmp/zerohertzLib-1.0.5.tar.gz` & `tmp/zerohertzLib-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerohertzLib-1.0.5.tar", last modified: Mon Apr  8 09:33:56 2024, max compression
+gzip compressed data, was "zerohertzLib-1.0.6.tar", last modified: Tue May  7 14:02:15 2024, max compression
```

## Comparing `zerohertzLib-1.0.5.tar` & `zerohertzLib-1.0.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-04-08 09:33:51.000000 zerohertzLib-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-08 09:33:51.000000 zerohertzLib-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3338 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2316 2024-04-08 09:33:51.000000 zerohertzLib-1.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2704 2024-04-08 09:33:51.000000 zerohertzLib-1.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.680283 zerohertzLib-1.0.5/test/
--rw-r--r--   0 root         (0) root         (0)     4501 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_api.py
--rw-r--r--   0 root         (0) root         (0)     1230 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_logging.py
--rw-r--r--   0 root         (0) root         (0)      220 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)     8641 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_plot.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_quant.py
--rw-r--r--   0 root         (0) root         (0)     1961 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_util.py
--rw-r--r--   0 root         (0) root         (0)    14679 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/test/test_vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.680283 zerohertzLib-1.0.5/zerohertzLib/
--rw-r--r--   0 root         (0) root         (0)     1794 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.680283 zerohertzLib-1.0.5/zerohertzLib/algorithm/
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2626 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/bisect.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/collections.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/fft.py
--rw-r--r--   0 root         (0) root         (0)     7065 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/graph.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/prime.py
--rw-r--r--   0 root         (0) root         (0)     8048 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/algorithm/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.684284 zerohertzLib-1.0.5/zerohertzLib/api/
--rw-r--r--   0 root         (0) root         (0)      446 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3865 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/api/discord.py
--rw-r--r--   0 root         (0) root         (0)    11096 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/api/github.py
--rw-r--r--   0 root         (0) root         (0)    30846 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/api/koreainvestment.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/api/open_ai.py
--rw-r--r--   0 root         (0) root         (0)     8841 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/api/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.684284 zerohertzLib-1.0.5/zerohertzLib/logging/
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4738 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/logging/handler.py
--rw-r--r--   0 root         (0) root         (0)     5264 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/logging/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.684284 zerohertzLib-1.0.5/zerohertzLib/mlops/
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/mlops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18002 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/mlops/triton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.684284 zerohertzLib-1.0.5/zerohertzLib/monitoring/
--rw-r--r--   0 root         (0) root         (0)      333 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2829 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/monitoring/cpu.py
--rw-r--r--   0 root         (0) root         (0)     5184 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/monitoring/gpu.py
--rw-r--r--   0 root         (0) root         (0)     2678 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/monitoring/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.684284 zerohertzLib-1.0.5/zerohertzLib/plot/
--rw-r--r--   0 root         (0) root         (0)     1552 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15381 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/bar_chart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/zerohertzLib/plot/fonts/
--rw-r--r--   0 root         (0) root         (0)  7549348 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
--rw-r--r--   0 root         (0) root         (0)   347988 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/fonts/times.ttf
--rw-r--r--   0 root         (0) root         (0)     3435 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/pie.py
--rw-r--r--   0 root         (0) root         (0)    11476 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/plot.py
--rw-r--r--   0 root         (0) root         (0)     4046 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/scatter.py
--rw-r--r--   0 root         (0) root         (0)     3292 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/table.py
--rw-r--r--   0 root         (0) root         (0)     4838 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/zerohertzLib/quant/
--rw-r--r--   0 root         (0) root         (0)      885 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/quant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14935 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/quant/backtest.py
--rw-r--r--   0 root         (0) root         (0)    13182 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/quant/methods.py
--rw-r--r--   0 root         (0) root         (0)    45350 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/quant/quant.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/quant/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/zerohertzLib/util/
--rw-r--r--   0 root         (0) root         (0)      458 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4527 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/util/csv.py
--rw-r--r--   0 root         (0) root         (0)    11173 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/util/data.py
--rw-r--r--   0 root         (0) root         (0)    11650 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/util/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.688284 zerohertzLib-1.0.5/zerohertzLib/vision/
--rw-r--r--   0 root         (0) root         (0)     1623 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6967 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/compare.py
--rw-r--r--   0 root         (0) root         (0)    12885 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/convert.py
--rw-r--r--   0 root         (0) root         (0)    22648 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/data.py
--rw-r--r--   0 root         (0) root         (0)    14878 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/eval.py
--rw-r--r--   0 root         (0) root         (0)     4188 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/gif.py
--rw-r--r--   0 root         (0) root         (0)    22281 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/loader.py
--rw-r--r--   0 root         (0) root         (0)     7826 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/transform.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/util.py
--rw-r--r--   0 root         (0) root         (0)    17516 2024-04-08 09:33:52.000000 zerohertzLib-1.0.5/zerohertzLib/vision/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 09:33:56.680283 zerohertzLib-1.0.5/zerohertzLib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3338 2024-04-08 09:33:56.000000 zerohertzLib-1.0.5/zerohertzLib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1923 2024-04-08 09:33:56.000000 zerohertzLib-1.0.5/zerohertzLib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 09:33:56.000000 zerohertzLib-1.0.5/zerohertzLib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      430 2024-04-08 09:33:56.000000 zerohertzLib-1.0.5/zerohertzLib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-08 09:33:56.000000 zerohertzLib-1.0.5/zerohertzLib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.071348 zerohertzLib-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 14:02:09.000000 zerohertzLib-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-07 14:02:09.000000 zerohertzLib-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-05-07 14:02:15.071348 zerohertzLib-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-05-07 14:02:09.000000 zerohertzLib-1.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 14:02:15.071348 zerohertzLib-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2704 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.059347 zerohertzLib-1.0.6/test/
+-rw-r--r--   0 root         (0) root         (0)     4501 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/test/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/test/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/test/test_logging.py
+-rw-r--r--   0 root         (0) root         (0)      220 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/test/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/test/test_plot.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/test/test_quant.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/test/test_util.py
+-rw-r--r--   0 root         (0) root         (0)    14679 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/test/test_vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.059347 zerohertzLib-1.0.6/zerohertzLib/
+-rw-r--r--   0 root         (0) root         (0)     1794 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.063347 zerohertzLib-1.0.6/zerohertzLib/algorithm/
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/algorithm/bisect.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/algorithm/collections.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/algorithm/fft.py
+-rw-r--r--   0 root         (0) root         (0)     7065 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/algorithm/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/algorithm/prime.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/algorithm/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.063347 zerohertzLib-1.0.6/zerohertzLib/api/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/api/discord.py
+-rw-r--r--   0 root         (0) root         (0)    11096 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/api/github.py
+-rw-r--r--   0 root         (0) root         (0)    30846 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/api/koreainvestment.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/api/open_ai.py
+-rw-r--r--   0 root         (0) root         (0)     7698 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/api/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.063347 zerohertzLib-1.0.6/zerohertzLib/logging/
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/logging/handler.py
+-rw-r--r--   0 root         (0) root         (0)     5264 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/logging/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.063347 zerohertzLib-1.0.6/zerohertzLib/mlops/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/mlops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18002 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/mlops/triton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.063347 zerohertzLib-1.0.6/zerohertzLib/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      333 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2829 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/monitoring/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/monitoring/gpu.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/monitoring/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.063347 zerohertzLib-1.0.6/zerohertzLib/plot/
+-rw-r--r--   0 root         (0) root         (0)     1552 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15381 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/plot/bar_chart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.071348 zerohertzLib-1.0.6/zerohertzLib/plot/fonts/
+-rw-r--r--   0 root         (0) root         (0)  7549348 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
+-rw-r--r--   0 root         (0) root         (0)   347988 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/plot/fonts/times.ttf
+-rw-r--r--   0 root         (0) root         (0)     3435 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/plot/pie.py
+-rw-r--r--   0 root         (0) root         (0)    11476 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/plot/plot.py
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/plot/scatter.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/plot/table.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.071348 zerohertzLib-1.0.6/zerohertzLib/quant/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/quant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/quant/backtest.py
+-rw-r--r--   0 root         (0) root         (0)    13182 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/quant/methods.py
+-rw-r--r--   0 root         (0) root         (0)    44750 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/quant/quant.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/quant/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.071348 zerohertzLib-1.0.6/zerohertzLib/util/
+-rw-r--r--   0 root         (0) root         (0)      458 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4527 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/util/csv.py
+-rw-r--r--   0 root         (0) root         (0)    11173 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/util/data.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/util/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.071348 zerohertzLib-1.0.6/zerohertzLib/vision/
+-rw-r--r--   0 root         (0) root         (0)     1623 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6967 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/vision/compare.py
+-rw-r--r--   0 root         (0) root         (0)    12885 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/vision/convert.py
+-rw-r--r--   0 root         (0) root         (0)    22648 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/vision/data.py
+-rw-r--r--   0 root         (0) root         (0)    14878 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/vision/eval.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/vision/gif.py
+-rw-r--r--   0 root         (0) root         (0)    22281 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/vision/loader.py
+-rw-r--r--   0 root         (0) root         (0)     7826 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/vision/transform.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/vision/util.py
+-rw-r--r--   0 root         (0) root         (0)    17516 2024-05-07 14:02:10.000000 zerohertzLib-1.0.6/zerohertzLib/vision/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:02:15.063347 zerohertzLib-1.0.6/zerohertzLib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-05-07 14:02:15.000000 zerohertzLib-1.0.6/zerohertzLib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-05-07 14:02:15.000000 zerohertzLib-1.0.6/zerohertzLib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 14:02:15.000000 zerohertzLib-1.0.6/zerohertzLib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      470 2024-05-07 14:02:15.000000 zerohertzLib-1.0.6/zerohertzLib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 14:02:15.000000 zerohertzLib-1.0.6/zerohertzLib.egg-info/top_level.txt
```

### Comparing `zerohertzLib-1.0.5/LICENSE` & `zerohertzLib-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/PKG-INFO` & `zerohertzLib-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.5
+Version: 1.0.6
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.5 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.6 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.5/README.md` & `zerohertzLib-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/setup.py` & `zerohertzLib-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/test/test_algorithm.py` & `zerohertzLib-1.0.6/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/test/test_api.py` & `zerohertzLib-1.0.6/test/test_api.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/test/test_logging.py` & `zerohertzLib-1.0.6/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/test/test_plot.py` & `zerohertzLib-1.0.6/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/test/test_quant.py` & `zerohertzLib-1.0.6/test/test_quant.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/test/test_util.py` & `zerohertzLib-1.0.6/test/test_util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/test/test_vision.py` & `zerohertzLib-1.0.6/test/test_vision.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/__init__.py` & `zerohertzLib-1.0.6/zerohertzLib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     print("=" * 100)
     print(f"[Warning] {error}")
     print("Please Install OpenCV Dependency")
     print("--->\t$ sudo apt install python3-opencv -y\t<---")
     print("(but you can use other submodules except zerohertzLib.vision)")
     print("=" * 100)
 
-__version__ = "v1.0.5"
+__version__ = "v1.0.6"
```

### Comparing `zerohertzLib-1.0.5/zerohertzLib/algorithm/__init__.py` & `zerohertzLib-1.0.6/zerohertzLib/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/algorithm/bisect.py` & `zerohertzLib-1.0.6/zerohertzLib/algorithm/bisect.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/algorithm/collections.py` & `zerohertzLib-1.0.6/zerohertzLib/algorithm/collections.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/algorithm/fft.py` & `zerohertzLib-1.0.6/zerohertzLib/algorithm/fft.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/algorithm/graph.py` & `zerohertzLib-1.0.6/zerohertzLib/algorithm/graph.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/algorithm/prime.py` & `zerohertzLib-1.0.6/zerohertzLib/algorithm/prime.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/algorithm/sort.py` & `zerohertzLib-1.0.6/zerohertzLib/algorithm/sort.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/api/discord.py` & `zerohertzLib-1.0.6/zerohertzLib/api/discord.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/api/github.py` & `zerohertzLib-1.0.6/zerohertzLib/api/github.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/api/koreainvestment.py` & `zerohertzLib-1.0.6/zerohertzLib/api/koreainvestment.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/api/open_ai.py` & `zerohertzLib-1.0.6/zerohertzLib/api/open_ai.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/api/slack.py` & `zerohertzLib-1.0.6/zerohertzLib/api/slack.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 SOFTWARE.
 """
 
 import json
 from typing import Optional
 
 import requests
+from slack_sdk import WebClient
+from slack_sdk.web import SlackResponse
 
 
 class SlackWebhook:
     """Slack Webhook의 data 전송을 위한 class
 
     Args:
         webhook_url (``str``): Slack Webhook의 URL
@@ -130,119 +132,84 @@
     def __init__(
         self,
         token: str,
         channel: str,
         name: Optional[str] = None,
         icon_emoji: Optional[str] = None,
         icon_url: Optional[str] = None,
-        timeout: Optional[int] = 10,
+        timeout: Optional[int] = 30,
     ) -> None:
-        self.token = token
-        self.headers = {
-            "Authorization": "Bearer " + token,
-        }
-        self.channel = channel
-        self.data = {
-            "channel": channel,
-        }
-        if name is not None:
-            self.data["username"] = name
-        if icon_emoji is not None:
-            self.data["icon_emoji"] = f":{icon_emoji}:"
-        if icon_url is not None:
-            self.data["icon_url"] = icon_url
-        self.timeout = timeout
+        self.webclient = WebClient(token, timeout=timeout)
+        self.channel2id = {}
+        for channel_info in self.webclient.conversations_list(
+            types="public_channel,private_channel"
+        ).data["channels"]:
+            channel_id, channel_name, is_channel = (
+                channel_info.get("id"),
+                channel_info.get("name"),
+                channel_info.get("is_channel"),
+            )
+            if is_channel:
+                self.channel2id[channel_name] = channel_id
+        self.channel_name = channel
+        self.channel_id = self.channel2id[channel]
+        self.username = name
+        self.icon_emoji = icon_emoji
+        self.icon_url = icon_url
 
     def message(
         self,
         message: str,
         codeblock: Optional[bool] = False,
         thread_ts: Optional[str] = None,
-    ) -> requests.models.Response:
+    ) -> SlackResponse:
         """Slack Bot을 통해 message 전송
 
         Args:
             message (``str``): 전송할 message
             codeblock (``Optional[bool]``): 전송되는 message의 스타일
             thread_ts (``Optional[str]``): 댓글을 전송할 thread의 timestamp
 
         Returns:
-            ``requests.models.Response``: Slack Bot의 응답
+            ``slack_sdk.web.slack_response.SlackResponse``: Slack Bot의 응답
 
         Examples:
             >>> response = slack.message("test")
             >>> response
-            <Response [200]>
-            >>> slack.message("test", True, response.json()["ts"])
-            <Response [200]>
-            >>> response = slack.file("test.jpg")
-            >>> slack.message("test", thread_ts=list(response.json()["file"]["shares"]["private"].values())[0][0]["ts"])
-            <Response [200]>
+            <slack_sdk.web.slack_response.SlackResponse object at 0x7fb0c4346340>
+            >>> slack.message("test", True, response.get("ts"))
+            <slack_sdk.web.slack_response.SlackResponse object at 0x7fb0761b1100>
         """
         if message == "":
             return None
         if codeblock:
             message = f"```{message}```"
-        data = self.data.copy()
-        data["text"] = message
-        if thread_ts is not None:
-            data["thread_ts"] = thread_ts
-        response = requests.post(
-            "https://slack.com/api/chat.postMessage",
-            headers=self.headers,
-            json=data,
-            timeout=self.timeout,
+        return self.webclient.chat_postMessage(
+            channel=self.channel_id,
+            text=message,
+            thread_ts=thread_ts,
+            icon_emoji=self.icon_emoji,
+            icon_url=self.icon_url,
+            username=self.username,
         )
-        if not response.json()["ok"]:
-            error = response.json()["error"]
-            print(
-                "[zerohertzLib.api.SlackBot] Failed: " + error.replace("_", " ").upper()
-            )
-            if error in ["not_authed", "invalid_auth", "channel_not_found"]:
-                return response
-            response_metadata = "\n".join(
-                response.json()["response_metadata"]["messages"]
-            )
-            self.message(
-                f"[`zerohertzLib.api.SlackBot`] Failed: `{error}`\n```>>> message({message}, {codeblock}, {thread_ts})\n{response_metadata}```"
-            )
-        return response
 
-    def file(
-        self, path: str, thread_ts: Optional[str] = None
-    ) -> requests.models.Response:
+    def file(self, path: str, thread_ts: Optional[str] = None) -> SlackResponse:
         """Slack Bot을 통해 file 전송
 
         Note:
             ``name`` 과 ``icon_*`` 의 적용 불가
 
         Args:
             path (``str``): 전송할 file 경로
             thread_ts (``Optional[str]``): 댓글을 전송할 thread의 timestamp
 
         Returns:
-            ``requests.models.Response``: Slack Bot의 응답
+            ``slack_sdk.web.slack_response.SlackResponse``: Slack Bot의 응답
 
         Examples:
             >>> response = slack.file("test.jpg")
             >>> response
-            <Response [200]>
+            <slack_sdk.web.slack_response.SlackResponse object at 0x7fb0675e0c10>
         """
-        with open(path, "rb") as file:
-            response = requests.post(
-                "https://slack.com/api/files.upload",
-                headers=self.headers,
-                files={"file": file},
-                data={"channels": self.channel, "thread_ts": thread_ts},
-                timeout=self.timeout,
-            )
-        if not response.json()["ok"]:
-            error = response.json()["error"]
-            print(
-                "[zerohertzLib.api.SlackBot] Failed: " + error.replace("_", " ").upper()
-            )
-            if error in ["not_authed", "invalid_auth", "channel_not_found"]:
-                return response
-            self.message(
-                f"[`zerohertzLib.api.SlackBot`] Failed: `{error}`\n```>>> file({path}, {thread_ts})```"
-            )
-        return response
+        return self.webclient.files_upload_v2(
+            file=path, channel=self.channel_id, thread_ts=thread_ts
+        )
```

### Comparing `zerohertzLib-1.0.5/zerohertzLib/logging/handler.py` & `zerohertzLib-1.0.6/zerohertzLib/logging/handler.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/logging/logger.py` & `zerohertzLib-1.0.6/zerohertzLib/logging/logger.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/mlops/triton.py` & `zerohertzLib-1.0.6/zerohertzLib/mlops/triton.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/monitoring/cpu.py` & `zerohertzLib-1.0.6/zerohertzLib/monitoring/cpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/monitoring/gpu.py` & `zerohertzLib-1.0.6/zerohertzLib/monitoring/gpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/monitoring/storage.py` & `zerohertzLib-1.0.6/zerohertzLib/monitoring/storage.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/plot/__init__.py` & `zerohertzLib-1.0.6/zerohertzLib/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/plot/bar_chart.py` & `zerohertzLib-1.0.6/zerohertzLib/plot/bar_chart.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf` & `zerohertzLib-1.0.6/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/plot/fonts/times.ttf` & `zerohertzLib-1.0.6/zerohertzLib/plot/fonts/times.ttf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/plot/pie.py` & `zerohertzLib-1.0.6/zerohertzLib/plot/pie.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/plot/plot.py` & `zerohertzLib-1.0.6/zerohertzLib/plot/plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/plot/scatter.py` & `zerohertzLib-1.0.6/zerohertzLib/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/plot/table.py` & `zerohertzLib-1.0.6/zerohertzLib/plot/table.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/plot/util.py` & `zerohertzLib-1.0.6/zerohertzLib/plot/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/quant/__init__.py` & `zerohertzLib-1.0.6/zerohertzLib/quant/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/quant/backtest.py` & `zerohertzLib-1.0.6/zerohertzLib/quant/backtest.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/quant/methods.py` & `zerohertzLib-1.0.6/zerohertzLib/quant/methods.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/quant/quant.py` & `zerohertzLib-1.0.6/zerohertzLib/quant/quant.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,29 +18,28 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-import json
 import multiprocessing as mp
 import time
 import traceback
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from datetime import datetime, timedelta
 from itertools import combinations
 from typing import Any, Dict, ItemsView, List, Optional, Tuple, TypeVar, Union
 
 import FinanceDataReader as fdr
 import pandas as pd
-import requests
 from matplotlib import pyplot as plt
 from matplotlib import ticker
+from slack_sdk.web import SlackResponse
 
 from zerohertzLib.api import KoreaInvestment, SlackBot
 from zerohertzLib.plot import barh, barv, candle, figure, hist, pie, savefig, table
 
 from .backtest import Experiments, backtest
 from .util import _cash2str, _method2str, _seconds_to_hms
 
@@ -336,28 +335,20 @@
                         stock["pdno"],  # 종목번호
                         float(stock["avg_unpr3"]),  # 평균단가
                         float(stock["ovrs_now_pric1"]),  # 해외현재가격
                         int(float(stock["ccld_qty_smtl1"])),  # 해외잔고수량
                         float(stock["evlu_pfls_rt1"]),  # 평가손익율
                         float(stock["evlu_pfls_amt2"]),  # 평가손익금액
                     ]
-            # self.balance["cash"] = (
-            #     int(response["output3"]["tot_asst_amt"])  # 총자산금액
-            #     - int(response["output3"]["ustl_sll_amt_smtl"])  # 미결제매도금액합계
-            #     - int(response["output3"]["ustl_buy_amt_smtl"])  # 미결제매수금액합계
-            # ) / self._exchange()
             self.balance["cash"] = (
-                float(response["output3"]["evlu_amt_smtl_amt"])  # 평가금액합계금액
-                + float(response["output3"]["frcr_use_psbl_amt"])  # 외화사용가능금액
+                int(response["output3"]["evlu_amt_smtl_amt"])  # 평가금액합계금액
+                + int(response["output3"]["frcr_use_psbl_amt"])  # 외화사용가능금액
+                + int(response["output3"]["ustl_sll_amt_smtl"])  # 미결제매도금액합계
+                - int(response["output3"]["ustl_buy_amt_smtl"])  # 미결제매수금액합계
             ) / self._exchange()
-            # self.balance["cash"] = (
-            #     float(response["output3"]["evlu_amt_smtl"])  # 평가금액합계
-            #     + float(response["output3"]["frcr_use_psbl_amt"])  # 외화사용가능금액
-            #     / self._exchange()
-            # )
         self.balance["stock"] = dict(
             sorted(
                 self.balance["stock"].items(),
                 key=lambda item: item[1][1] * item[1][3],
                 reverse=True,
             )
         )
@@ -688,48 +679,42 @@
         self.report = report
 
     def message(
         self,
         message: str,
         codeblock: Optional[bool] = False,
         thread_ts: Optional[str] = None,
-    ) -> requests.models.Response:
+    ) -> SlackResponse:
         """``token`` 혹은 ``channel`` 이 입력되지 않을 시 전송 불가
 
         Args:
             message (``str``): 전송할 message
             codeblock (``Optional[bool]``): 전송되는 message의 스타일
             thread_ts (``Optional[str]``): 댓글을 전송할 thread의 timestamp
 
         Returns:
-            ``requests.models.Response``: Slack Bot의 응답
+            ``slack_sdk.web.slack_response.SlackResponse``: Slack Bot의 응답
         """
         if self.slack:
             return super().message(message, codeblock, thread_ts)
-        response = requests.Response()
-        response._content = json.dumps({"ts": None}).encode("utf-8")
-        return response
-
-    def file(
-        self, path: str, thread_ts: Optional[str] = None
-    ) -> requests.models.Response:
+        return None
+
+    def file(self, path: str, thread_ts: Optional[str] = None) -> SlackResponse:
         """``token`` 혹은 ``channel`` 이 입력되지 않을 시 전송 불가
 
         Args:
             path (``str``): 전송할 file 경로
             thread_ts (``Optional[str]``): 댓글을 전송할 thread의 timestamp
 
         Returns:
-            ``requests.models.Response``: Slack Bot의 응답
+            ``slack_sdk.web.slack_response.SlackResponse``: Slack Bot의 응답
         """
         if self.slack:
             return super().file(path, thread_ts)
-        response = requests.Response()
-        response._content = json.dumps({"ts": None}).encode("utf-8")
-        return response
+        return None
 
     def _plot(self, quant: Quant) -> Tuple[str]:
         candle_path = candle(
             quant.data[-500:],
             quant.title,
             signals=quant.signals.iloc[-500:, :].loc[
                 :, [*quant.methods, "signals", "logic"]
@@ -816,16 +801,17 @@
         symbol, mode = args
         try:
             title, data = self._get_data(symbol)
             if len(data) < 20:
                 return None, None
         except KeyError as error:
             response = self.message(f":x: `{symbol}` was not found")
-            self.message(str(error), True, response.json()["ts"])
-            self.message(traceback.format_exc(), True, response.json()["ts"])
+            thread_ts = response.get("ts")
+            self.message(str(error), True, thread_ts)
+            self.message(traceback.format_exc(), True, thread_ts)
             return None, None
         try:
             quant = Quant(
                 title,
                 data,
                 ohlc=self.ohlc,
                 top=self.top,
@@ -833,16 +819,17 @@
                 report=self.report,
             )
             today = quant()
         except IndexError as error:
             response = self.message(
                 f":x: `{symbol}` ({title}): {data.index[0]} ({len(data)})"
             )
-            self.message(str(error), True, response.json()["ts"])
-            self.message(traceback.format_exc(), True, response.json()["ts"])
+            thread_ts = response.get("ts")
+            self.message(str(error), True, thread_ts)
+            self.message(traceback.format_exc(), True, thread_ts)
             return None, None
         if today["position"] == "NULL":
             return None, None
         if not self.slack:
             return None, quant
         if mode == "Buy":
             positions = ["Buy"]
@@ -852,15 +839,15 @@
             return self._report(symbol, quant, today), quant
         return None, quant
 
     def _send(self, report: Dict[str, str]) -> None:
         if report is None:
             return
         response = self.message(report["main"])
-        thread_ts = response.json()["ts"]
+        thread_ts = response.get("ts")
         self.file(report["candle"], thread_ts)
         response = self.message(report["backtest"], thread_ts=thread_ts)
         self.file(report["hist"], thread_ts)
         response = self.message(report["param"], thread_ts=thread_ts)
 
     def _analysis_update(
         self,
@@ -884,15 +871,15 @@
                 self.exps_cnt[method] = [defaultdict(int) for _ in range(len(cnt))]
             for idx, cnt_ in enumerate(cnt):
                 for param, cnt__ in cnt_.items():
                     self.exps_cnt[method][idx][param] += cnt__
 
     def _analysis_send(self) -> None:
         response = self.message("> :memo: Parameter Analysis")
-        thread_ts = response.json()["ts"]
+        thread_ts = response.get("ts")
         figure((30, 20))
         plt.subplot(2, 2, 1)
         barv(
             dict(sorted(self.miu_cnt.items())),
             title=f"Methods in Use (Avg: {sum(self.miu_cnt.values()) / self.quant_cnt:.2f})",
             dim="%",
             save=False,
@@ -953,15 +940,15 @@
             # [Methods in Use: O] 사용된 전략의 수 (같은 전략 포함)
             self.total_cnt = []
             # [Methods in Use: X] 전략에 따른 이익이 존재하는 수
             self.methods_cnt = defaultdict(list)
             # [Methods in Use: X] 전략과 parameter에 따른 이익이 존재하는 수
             self.exps_cnt = defaultdict(list)
         response = self.message(f"> :moneybag: Check {mode} Signals")
-        self.message(", ".join(symbols), True, response.json()["ts"])
+        self.message(", ".join(symbols), True, response.get("ts"))
         if self.mp_num == 0 or self.mp_num >= len(symbols):
             for symbol in symbols:
                 report, quant = self._run([symbol, mode])
                 self._send(report)
                 if self.analysis and quant is not None:
                     self._analysis_update(quant)
         else:
@@ -1063,16 +1050,17 @@
         한국투자증권의 잔고와 주식 보유 상황을 image로 변환하여 slack으로 전송 및 보유 중인 주식에 대해 매도 signals 탐색
         """
         path_balance, path_portfolio = self.table(), self.pie()
         if path_balance is None:
             self.message("Balance: NULL", True)
             return None
         response = self.message("> :bank: Balance")
-        self.file(path_balance, response.json()["ts"])
-        self.file(path_portfolio, response.json()["ts"])
+        thread_ts = response.get("ts")
+        self.file(path_balance, thread_ts)
+        self.file(path_portfolio, thread_ts)
         self._inference(self.symbols_bought, "Sell")
         return None
 
 
 class QuantSlackBotFDR(QuantSlackBot):
     """`FinanceDataReader <https://github.com/FinanceData/FinanceDataReader>`_ module 기반으로 입력된 여러 종목에 대해 매수, 매도 signal을 판단하고 Slack으로 message와 graph를 전송하는 class
```

### Comparing `zerohertzLib-1.0.5/zerohertzLib/quant/util.py` & `zerohertzLib-1.0.6/zerohertzLib/quant/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/util/csv.py` & `zerohertzLib-1.0.6/zerohertzLib/util/csv.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/util/data.py` & `zerohertzLib-1.0.6/zerohertzLib/util/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/util/json.py` & `zerohertzLib-1.0.6/zerohertzLib/util/json.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/vision/__init__.py` & `zerohertzLib-1.0.6/zerohertzLib/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/vision/compare.py` & `zerohertzLib-1.0.6/zerohertzLib/vision/compare.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/vision/convert.py` & `zerohertzLib-1.0.6/zerohertzLib/vision/convert.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/vision/data.py` & `zerohertzLib-1.0.6/zerohertzLib/vision/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/vision/eval.py` & `zerohertzLib-1.0.6/zerohertzLib/vision/eval.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/vision/gif.py` & `zerohertzLib-1.0.6/zerohertzLib/vision/gif.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/vision/loader.py` & `zerohertzLib-1.0.6/zerohertzLib/vision/loader.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/vision/transform.py` & `zerohertzLib-1.0.6/zerohertzLib/vision/transform.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/vision/util.py` & `zerohertzLib-1.0.6/zerohertzLib/vision/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib/vision/visual.py` & `zerohertzLib-1.0.6/zerohertzLib/vision/visual.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.5/zerohertzLib.egg-info/PKG-INFO` & `zerohertzLib-1.0.6/zerohertzLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.5
+Version: 1.0.6
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.5 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.6 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.5/zerohertzLib.egg-info/SOURCES.txt` & `zerohertzLib-1.0.6/zerohertzLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

