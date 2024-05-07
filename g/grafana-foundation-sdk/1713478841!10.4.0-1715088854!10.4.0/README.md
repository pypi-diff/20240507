# Comparing `tmp/grafana_foundation_sdk-1713478841!10.4.0.tar.gz` & `tmp/grafana_foundation_sdk-1715088854!10.4.0.tar.gz`

## Comparing `grafana_foundation_sdk-1713478841!10.4.0.tar` & `grafana_foundation_sdk-1715088854!10.4.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/__init__.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/accesspolicy.py
--rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/alertgroups.py
--rw-r--r--   0        0        0    19607 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/annotationslist.py
--rw-r--r--   0        0        0    27683 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/azuremonitor.py
--rw-r--r--   0        0        0    38594 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/barchart.py
--rw-r--r--   0        0        0    20412 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/bargauge.py
--rw-r--r--   0        0        0    48859 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/candlestick.py
--rw-r--r--   0        0        0    18470 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/canvas.py
--rw-r--r--   0        0        0    29609 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/cloudwatch.py
--rw-r--r--   0        0        0    49337 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/common.py
--rw-r--r--   0        0        0    68373 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/dashboard.py
--rw-r--r--   0        0        0    19940 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/dashboardlist.py
--rw-r--r--   0        0        0    16778 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/datagrid.py
--rw-r--r--   0        0        0    16973 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/debug.py
--rw-r--r--   0        0        0    62126 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/elasticsearch.py
--rw-r--r--   0        0        0    19322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/gauge.py
--rw-r--r--   0        0        0    18193 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/geomap.py
--rw-r--r--   0        0        0    19996 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/grafanapyroscope.py
--rw-r--r--   0        0        0    24316 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/heatmap.py
--rw-r--r--   0        0        0    32428 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/histogram.py
--rw-r--r--   0        0        0    12777 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/librarypanel.py
--rw-r--r--   0        0        0    19537 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/logs.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/loki.py
--rw-r--r--   0        0        0    17049 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/news.py
--rw-r--r--   0        0        0    16998 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/nodegraph.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/parca.py
--rw-r--r--   0        0        0    20039 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/piechart.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/preferences.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/prometheus.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/publicdashboard.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/role.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/rolebinding.py
--rw-r--r--   0        0        0    19639 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/stat.py
--rw-r--r--   0        0        0    22365 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/statetimeline.py
--rw-r--r--   0        0        0    22064 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/statushistory.py
--rw-r--r--   0        0        0    27310 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/table.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/team.py
--rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/tempo.py
--rw-r--r--   0        0        0    11410 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/testdata.py
--rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/text.py
--rw-r--r--   0        0        0    46439 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/timeseries.py
--rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/trend.py
--rw-r--r--   0        0        0    36156 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/xychart.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/cog/__init__.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/cog/builder.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/cog/encoder.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/cog/plugins.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/cog/runtime.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/cog/variants.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/__init__.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/accesspolicy.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/alertgroups.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/annotationslist.py
--rw-r--r--   0        0        0    40749 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/azuremonitor.py
--rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/barchart.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/bargauge.py
--rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/candlestick.py
--rw-r--r--   0        0        0    14128 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/canvas.py
--rw-r--r--   0        0        0    39904 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/cloudwatch.py
--rw-r--r--   0        0        0    87408 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/common.py
--rw-r--r--   0        0        0    86939 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/dashboard.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/dashboardlist.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/datagrid.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/debug.py
--rw-r--r--   0        0        0    90714 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/elasticsearch.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/gauge.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/geomap.py
--rw-r--r--   0        0        0    27783 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/grafanapyroscope.py
--rw-r--r--   0        0        0    21480 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/heatmap.py
--rw-r--r--   0        0        0     8134 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/histogram.py
--rw-r--r--   0        0        0    16344 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/librarypanel.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/logs.py
--rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/loki.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/news.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/nodegraph.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/parca.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/piechart.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/preferences.py
--rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/prometheus.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/publicdashboard.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/role.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/rolebinding.py
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/stat.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/statetimeline.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/statushistory.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/table.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/team.py
--rw-r--r--   0        0        0    10814 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/tempo.py
--rw-r--r--   0        0        0    20662 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/testdata.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/text.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/timeseries.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/trend.py
--rw-r--r--   0        0        0    18310 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/xychart.py
--rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/LICENSE.md
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/README.md
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/pyproject.toml
--rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1713478841!10.4.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/__init__.py
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/accesspolicy.py
+-rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/alertgroups.py
+-rw-r--r--   0        0        0    19607 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/annotationslist.py
+-rw-r--r--   0        0        0    27683 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/azuremonitor.py
+-rw-r--r--   0        0        0    38594 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/barchart.py
+-rw-r--r--   0        0        0    20412 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/bargauge.py
+-rw-r--r--   0        0        0    48859 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/candlestick.py
+-rw-r--r--   0        0        0    18470 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/canvas.py
+-rw-r--r--   0        0        0    29609 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/cloudwatch.py
+-rw-r--r--   0        0        0    49337 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/common.py
+-rw-r--r--   0        0        0    68373 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/dashboard.py
+-rw-r--r--   0        0        0    19940 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/dashboardlist.py
+-rw-r--r--   0        0        0    16778 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/datagrid.py
+-rw-r--r--   0        0        0    16973 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/debug.py
+-rw-r--r--   0        0        0    62126 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/elasticsearch.py
+-rw-r--r--   0        0        0    19322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/gauge.py
+-rw-r--r--   0        0        0    18193 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/geomap.py
+-rw-r--r--   0        0        0    19996 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/grafanapyroscope.py
+-rw-r--r--   0        0        0    24316 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/heatmap.py
+-rw-r--r--   0        0        0    32428 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/histogram.py
+-rw-r--r--   0        0        0    12777 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/librarypanel.py
+-rw-r--r--   0        0        0    19537 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/logs.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/loki.py
+-rw-r--r--   0        0        0    17049 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/news.py
+-rw-r--r--   0        0        0    16998 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/nodegraph.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/parca.py
+-rw-r--r--   0        0        0    20039 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/piechart.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/preferences.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/prometheus.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/publicdashboard.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/role.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/rolebinding.py
+-rw-r--r--   0        0        0    19639 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/stat.py
+-rw-r--r--   0        0        0    22365 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/statetimeline.py
+-rw-r--r--   0        0        0    22064 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/statushistory.py
+-rw-r--r--   0        0        0    27310 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/table.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/team.py
+-rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/tempo.py
+-rw-r--r--   0        0        0    11410 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/testdata.py
+-rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/text.py
+-rw-r--r--   0        0        0    46439 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/timeseries.py
+-rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/trend.py
+-rw-r--r--   0        0        0    36156 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/xychart.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/cog/__init__.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/cog/builder.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/cog/encoder.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/cog/plugins.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/cog/runtime.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/cog/variants.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/__init__.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/accesspolicy.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/alertgroups.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/annotationslist.py
+-rw-r--r--   0        0        0    40767 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/azuremonitor.py
+-rw-r--r--   0        0        0    11975 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/barchart.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/bargauge.py
+-rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/candlestick.py
+-rw-r--r--   0        0        0    14128 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/canvas.py
+-rw-r--r--   0        0        0    39994 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/cloudwatch.py
+-rw-r--r--   0        0        0    87462 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/common.py
+-rw-r--r--   0        0        0    86957 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/dashboard.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/dashboardlist.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/datagrid.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/debug.py
+-rw-r--r--   0        0        0    90822 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/elasticsearch.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/gauge.py
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/geomap.py
+-rw-r--r--   0        0        0    27783 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/googlecloudmonitoring.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/grafanapyroscope.py
+-rw-r--r--   0        0        0    21480 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/heatmap.py
+-rw-r--r--   0        0        0     8134 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/histogram.py
+-rw-r--r--   0        0        0    16344 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/librarypanel.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/logs.py
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/loki.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/news.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/nodegraph.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/parca.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/piechart.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/preferences.py
+-rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/prometheus.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/publicdashboard.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/role.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/rolebinding.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/stat.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/statetimeline.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/statushistory.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/table.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/team.py
+-rw-r--r--   0        0        0    10814 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/tempo.py
+-rw-r--r--   0        0        0    20662 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/testdata.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/text.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/timeseries.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/trend.py
+-rw-r--r--   0        0        0    18310 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/xychart.py
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/LICENSE.md
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/README.md
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 grafana_foundation_sdk-1715088854!10.4.0/PKG-INFO
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/accesspolicy.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/accesspolicy.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/alertgroups.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/alertgroups.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/annotationslist.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/annotationslist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/azuremonitor.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/azuremonitor.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/barchart.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/barchart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/bargauge.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/bargauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/candlestick.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/candlestick.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/canvas.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/canvas.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/cloudwatch.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/common.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/common.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/dashboard.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1413,16 +1413,16 @@
     Row panel
     """
     
     _internal: dashboard.RowPanel
 
     def __init__(self, title: typing.Optional[str]):
         self._internal = dashboard.RowPanel()        
-        self._internal.title = title        
-        self._internal.type_val = "row"
+        self._internal.type_val = "row"        
+        self._internal.title = title
 
     def build(self) -> dashboard.RowPanel:
         return self._internal    
     
     def collapsed(self, collapsed: bool) -> typing.Self:    
         """
         Whether this row should be collapsed or not.
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/dashboardlist.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/dashboardlist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/datagrid.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/datagrid.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/debug.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/debug.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/elasticsearch.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/gauge.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/gauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/geomap.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/geomap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/googlecloudmonitoring.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/grafanapyroscope.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/grafanapyroscope.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/heatmap.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/heatmap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/histogram.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/histogram.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/librarypanel.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/librarypanel.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/logs.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/logs.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/loki.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/loki.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/news.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/news.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/nodegraph.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/nodegraph.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/parca.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/parca.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/piechart.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/piechart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/preferences.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/preferences.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/prometheus.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/prometheus.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/publicdashboard.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/role.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/role.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/rolebinding.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/stat.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/stat.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/statetimeline.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/statetimeline.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/statushistory.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/statushistory.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/table.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/table.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/team.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/tempo.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/tempo.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/testdata.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/testdata.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/text.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/text.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/timeseries.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/timeseries.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/trend.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/trend.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/builders/xychart.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/builders/xychart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/cog/plugins.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/cog/plugins.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # Code generated - EDITING IS FUTILE. DO NOT EDIT.
 
-from ..models import logs
-from ..models import azuremonitor
-from ..models import barchart
-from ..models import heatmap
-from ..models import histogram
-from ..models import statushistory
-from ..models import table
-from ..models import timeseries
+from ..models import nodegraph
 from ..models import bargauge
-from ..models import dashboardlist
-from ..models import debug
 from ..models import gauge
-from ..models import geomap
-from ..models import stat
+from ..models import histogram
+from ..models import timeseries
 from ..models import alertgroups
-from ..models import annotationslist
-from ..models import candlestick
-from ..models import canvas
-from ..models import googlecloudmonitoring
+from ..models import stat
 from ..models import xychart
+from ..models import statushistory
+from ..models import table
+from ..models import text
+from ..models import dashboardlist
 from ..models import datagrid
-from ..models import news
-from ..models import nodegraph
-from ..models import piechart
-from ..models import testdata
-from ..models import trend
 from ..models import grafanapyroscope
-from ..models import loki
-from ..models import parca
 from ..models import prometheus
-from ..models import text
+from ..models import trend
+from ..models import logs
+from ..models import news
+from ..models import annotationslist
+from ..models import barchart
+from ..models import debug
+from ..models import geomap
 from ..models import cloudwatch
-from ..models import elasticsearch
 from ..models import statetimeline
+from ..models import googlecloudmonitoring
+from ..models import heatmap
+from ..models import parca
+from ..models import piechart
 from ..models import tempo
+from ..models import testdata
+from ..models import azuremonitor
+from ..models import candlestick
+from ..models import canvas
+from ..models import elasticsearch
+from ..models import loki
 from . import runtime as cogruntime
 
 
 def register_default_plugins():
     # Panelcfg variants
     cogruntime.register_panelcfg_variant(alertgroups.variant_config())
     cogruntime.register_panelcfg_variant(annotationslist.variant_config())
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/cog/runtime.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/cog/runtime.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/accesspolicy.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/accesspolicy.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/alertgroups.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/alertgroups.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/annotationslist.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/annotationslist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/azuremonitor.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/azuremonitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -999,11 +999,11 @@
             args["raw_query"] = data["rawQuery"]
         if "subscription" in data:
             args["subscription"] = data["subscription"]        
 
         return cls(**args)
 
 
-GrafanaTemplateVariableQuery = typing.Union['AppInsightsMetricNameQuery', 'AppInsightsGroupByQuery', 'SubscriptionsQuery', 'ResourceGroupsQuery', 'ResourceNamesQuery', 'MetricNamespaceQuery', 'MetricDefinitionsQuery', 'MetricNamesQuery', 'WorkspacesQuery', 'UnknownQuery']
+GrafanaTemplateVariableQuery: typing.TypeAlias = typing.Union['AppInsightsMetricNameQuery', 'AppInsightsGroupByQuery', 'SubscriptionsQuery', 'ResourceGroupsQuery', 'ResourceNamesQuery', 'MetricNamespaceQuery', 'MetricDefinitionsQuery', 'MetricNamesQuery', 'WorkspacesQuery', 'UnknownQuery']
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/barchart.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/barchart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/bargauge.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/bargauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/candlestick.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/candlestick.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             args["tooltip"] = common.VizTooltipOptions.from_json(data["tooltip"])
         if "includeAllFields" in data:
             args["include_all_fields"] = data["includeAllFields"]        
 
         return cls(**args)
 
 
-FieldConfig = common.GraphFieldConfig
+FieldConfig: typing.TypeAlias = common.GraphFieldConfig
 
 
 
 
 
 def variant_config():
     return cogruntime.PanelCfgConfig(
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/canvas.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/canvas.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/cloudwatch.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/cloudwatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         if "statistics" in data:
             args["statistics"] = data["statistics"]        
 
         return cls(**args)
 
 
 # A name/value pair that is part of the identity of a metric. For example, you can get statistics for a specific EC2 instance by specifying the InstanceId dimension when you search for metrics.
-Dimensions = dict[str, typing.Union[str, list[str]]]
+Dimensions: typing.TypeAlias = dict[str, typing.Union[str, list[str]]]
 
 
 class CloudWatchMetricsQuery(cogvariants.Dataquery):
     """
     Shape of a CloudWatch Metrics query
     """
 
@@ -528,18 +528,18 @@
             args["name"] = data["name"]
         if "value" in data:
             args["value"] = data["value"]        
 
         return cls(**args)
 
 
-QueryEditorOperatorValueType = typing.Union[str, bool, int, list['QueryEditorOperatorType']]
+QueryEditorOperatorValueType: typing.TypeAlias = typing.Union[str, bool, int, list['QueryEditorOperatorType']]
 
 
-QueryEditorOperatorType = typing.Union[str, bool, int]
+QueryEditorOperatorType: typing.TypeAlias = typing.Union[str, bool, int]
 
 
 class QueryEditorProperty:
     type_val: 'QueryEditorPropertyType'
     name: typing.Optional[str]
 
     def __init__(self, type_val: typing.Optional['QueryEditorPropertyType'] = None, name: typing.Optional[str] = None):
@@ -593,15 +593,15 @@
             args["type_val"] = data["type"]
         if "expressions" in data:
             args["expressions"] = data["expressions"]        
 
         return cls(**args)
 
 
-QueryEditorExpression = typing.Union['QueryEditorArrayExpression', 'QueryEditorPropertyExpression', 'QueryEditorGroupByExpression', 'QueryEditorFunctionExpression', 'QueryEditorFunctionParameterExpression', 'QueryEditorOperatorExpression']
+QueryEditorExpression: typing.TypeAlias = typing.Union['QueryEditorArrayExpression', 'QueryEditorPropertyExpression', 'QueryEditorGroupByExpression', 'QueryEditorFunctionExpression', 'QueryEditorFunctionParameterExpression', 'QueryEditorOperatorExpression']
 
 
 class CloudWatchLogsQuery(cogvariants.Dataquery):
     """
     Shape of a CloudWatch Logs query
     """
 
@@ -892,15 +892,15 @@
             args["datasource"] = data["datasource"]
         if "statistics" in data:
             args["statistics"] = data["statistics"]        
 
         return cls(**args)
 
 
-CloudWatchQuery = typing.Union['CloudWatchMetricsQuery', 'CloudWatchLogsQuery', 'CloudWatchAnnotationQuery']
+CloudWatchQuery: typing.TypeAlias = typing.Union['CloudWatchMetricsQuery', 'CloudWatchLogsQuery', 'CloudWatchAnnotationQuery']
 
 
 def variant_config() -> cogruntime.DataqueryConfig:
     decoding_map: dict[str, typing.Union[typing.Type[CloudWatchMetricsQuery], typing.Type[CloudWatchLogsQuery], typing.Type[CloudWatchAnnotationQuery]]] = {"Metrics": CloudWatchMetricsQuery, "Logs": CloudWatchLogsQuery, "Annotations": CloudWatchAnnotationQuery}
     return cogruntime.DataqueryConfig(
         identifier="cloudwatch",
         from_json_hook=lambda data: decoding_map[data["queryMode"]].from_json(data),
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/common.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1781,15 +1781,15 @@
             args["max_width"] = data["maxWidth"]
         if "maxHeight" in data:
             args["max_height"] = data["maxHeight"]        
 
         return cls(**args)
 
 
-Labels = dict[str, str]
+Labels: typing.TypeAlias = dict[str, str]
 
 
 class TableCellDisplayMode(enum.StrEnum):
     """
     Internally, this is the "type" of cell that's being displayed
     in the table such as colored text, JSON, gauge, etc.
     The color-background-solid, gradient-gauge, and lcd-gauge
@@ -2309,15 +2309,15 @@
     SM = "sm"
     MD = "md"
     LG = "lg"
 
 
 # Table cell options. Each cell has a display mode
 # and other potential options for that display.
-TableCellOptions = typing.Union['TableAutoCellOptions', 'TableSparklineCellOptions', 'TableBarGaugeCellOptions', 'TableColoredBackgroundCellOptions', 'TableColorTextCellOptions', 'TableImageCellOptions', 'TableDataLinksCellOptions', 'TableJsonViewCellOptions']
+TableCellOptions: typing.TypeAlias = typing.Union['TableAutoCellOptions', 'TableSparklineCellOptions', 'TableBarGaugeCellOptions', 'TableColoredBackgroundCellOptions', 'TableColorTextCellOptions', 'TableImageCellOptions', 'TableDataLinksCellOptions', 'TableJsonViewCellOptions']
 
 
 # Use UTC/GMT timezone
 TimeZoneUtc: typing.Literal["utc"] = "utc"
 
 
 # Use the timezone defined by end user web browser
@@ -2604,11 +2604,11 @@
         if "hideHeader" in data:
             args["hide_header"] = data["hideHeader"]        
 
         return cls(**args)
 
 
 # A specific timezone from https://en.wikipedia.org/wiki/Tz_database
-TimeZone = typing.Union[typing.Literal["utc"], typing.Literal["browser"], str]
+TimeZone: typing.TypeAlias = typing.Union[typing.Literal["utc"], typing.Literal["browser"], str]
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/dashboard.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -973,15 +973,15 @@
         if "steps" in data:
             args["steps"] = data["steps"]        
 
         return cls(**args)
 
 
 # Allow to transform the visual representation of specific data values in a visualization, irrespective of their original units
-ValueMapping = typing.Union['ValueMap', 'RangeMap', 'RegexMap', 'SpecialValueMap']
+ValueMapping: typing.TypeAlias = typing.Union['ValueMap', 'RangeMap', 'RegexMap', 'SpecialValueMap']
 
 
 class MappingType(enum.StrEnum):
     """
     Supported value mapping types
     `value`: Maps text values to a color or different display text and color. For example, you can configure a value mapping so that all instances of the value 10 appear as Perfection! rather than the number.
     `range`: Maps numerical ranges to a display text and color. For example, if a value is within a certain range, you can configure a range value mapping to display Low or High rather than the number.
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/dashboardlist.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/dashboardlist.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/datagrid.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/datagrid.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/debug.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/debug.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/elasticsearch.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/elasticsearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import typing
 import enum
 from ..cog import variants as cogvariants
 from ..cog import runtime as cogruntime
 
 
-BucketAggregation = typing.Union['DateHistogram', 'Histogram', 'Terms', 'Filters', 'GeoHashGrid', 'Nested']
+BucketAggregation: typing.TypeAlias = typing.Union['DateHistogram', 'Histogram', 'Terms', 'Filters', 'GeoHashGrid', 'Nested']
 
 
-MetricAggregation = typing.Union['Count', 'MovingAverage', 'Derivative', 'CumulativeSum', 'BucketScript', 'SerialDiff', 'RawData', 'RawDocument', 'UniqueCount', 'Percentiles', 'ExtendedStats', 'Min', 'Max', 'Sum', 'Average', 'MovingFunction', 'Logs', 'Rate', 'TopMetrics']
+MetricAggregation: typing.TypeAlias = typing.Union['Count', 'MovingAverage', 'Derivative', 'CumulativeSum', 'BucketScript', 'SerialDiff', 'RawData', 'RawDocument', 'UniqueCount', 'Percentiles', 'ExtendedStats', 'Min', 'Max', 'Sum', 'Average', 'MovingFunction', 'Logs', 'Rate', 'TopMetrics']
 
 
 class BucketAggregationType(enum.StrEnum):
     TERMS = "terms"
     FILTERS = "filters"
     GEOHASH_GRID = "geohash_grid"
     DATE_HISTOGRAM = "date_histogram"
@@ -515,15 +515,15 @@
     MOVING_FN = "moving_fn"
     DERIVATIVE = "derivative"
     SERIAL_DIFF = "serial_diff"
     CUMULATIVE_SUM = "cumulative_sum"
     BUCKET_SCRIPT = "bucket_script"
 
 
-MetricAggregationType = typing.Union[typing.Literal["count"], 'PipelineMetricAggregationType']
+MetricAggregationType: typing.TypeAlias = typing.Union[typing.Literal["count"], 'PipelineMetricAggregationType']
 
 
 class BaseMetricAggregation:
     type_val: 'MetricAggregationType'
     id_val: str
     hide: typing.Optional[bool]
 
@@ -656,15 +656,15 @@
             args["id_val"] = data["id"]
         if "hide" in data:
             args["hide"] = data["hide"]        
 
         return cls(**args)
 
 
-InlineScript = typing.Union[str, 'ElasticsearchInlineScript']
+InlineScript: typing.TypeAlias = typing.Union[str, 'ElasticsearchInlineScript']
 
 
 class MetricAggregationWithInlineScript:
     settings: typing.Optional['ElasticsearchMetricAggregationWithInlineScriptSettings']
     type_val: 'MetricAggregationType'
     id_val: str
     hide: typing.Optional[bool]
@@ -1889,18 +1889,18 @@
             args["settings"] = ElasticsearchTopMetricsSettings.from_json(data["settings"])
         if "hide" in data:
             args["hide"] = data["hide"]        
 
         return cls(**args)
 
 
-PipelineMetricAggregation = typing.Union['MovingAverage', 'Derivative', 'CumulativeSum', 'BucketScript']
+PipelineMetricAggregation: typing.TypeAlias = typing.Union['MovingAverage', 'Derivative', 'CumulativeSum', 'BucketScript']
 
 
-MetricAggregationWithSettings = typing.Union['BucketScript', 'CumulativeSum', 'Derivative', 'SerialDiff', 'RawData', 'RawDocument', 'UniqueCount', 'Percentiles', 'ExtendedStats', 'Min', 'Max', 'Sum', 'Average', 'MovingAverage', 'MovingFunction', 'Logs', 'Rate', 'TopMetrics']
+MetricAggregationWithSettings: typing.TypeAlias = typing.Union['BucketScript', 'CumulativeSum', 'Derivative', 'SerialDiff', 'RawData', 'RawDocument', 'UniqueCount', 'Percentiles', 'ExtendedStats', 'Min', 'Max', 'Sum', 'Average', 'MovingAverage', 'MovingFunction', 'Logs', 'Rate', 'TopMetrics']
 
 
 class Dataquery(cogvariants.Dataquery):
     alias: typing.Optional[str]
     query: typing.Optional[str]
     time_field: typing.Optional[str]
     bucket_aggs: typing.Optional[list['BucketAggregation']]
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/gauge.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/gauge.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/geomap.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/geomap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/googlecloudmonitoring.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/googlecloudmonitoring.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/grafanapyroscope.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/grafanapyroscope.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/heatmap.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/heatmap.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/histogram.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/histogram.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/librarypanel.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/librarypanel.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/logs.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/logs.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/loki.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/loki.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/news.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/news.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/nodegraph.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/nodegraph.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/parca.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/parca.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/piechart.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/piechart.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             args["legend"] = PieChartLegendOptions.from_json(data["legend"])
         if "orientation" in data:
             args["orientation"] = data["orientation"]        
 
         return cls(**args)
 
 
-FieldConfig = common.HideableFieldConfig
+FieldConfig: typing.TypeAlias = common.HideableFieldConfig
 
 
 
 
 
 def variant_config():
     return cogruntime.PanelCfgConfig(
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/preferences.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/preferences.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/prometheus.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/prometheus.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/publicdashboard.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/publicdashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/role.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/role.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/rolebinding.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/rolebinding.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/stat.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/stat.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/statetimeline.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/statetimeline.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/statushistory.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/statushistory.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/table.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/table.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             args["footer"] = common.TableFooterOptions.from_json(data["footer"])
         if "cellHeight" in data:
             args["cell_height"] = data["cellHeight"]        
 
         return cls(**args)
 
 
-FieldConfig = common.TableFieldOptions
+FieldConfig: typing.TypeAlias = common.TableFieldOptions
 
 
 
 
 
 def variant_config():
     return cogruntime.PanelCfgConfig(
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/team.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/tempo.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/tempo.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/testdata.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/testdata.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/text.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/text.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/timeseries.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/timeseries.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             args["legend"] = common.VizLegendOptions.from_json(data["legend"])
         if "tooltip" in data:
             args["tooltip"] = common.VizTooltipOptions.from_json(data["tooltip"])        
 
         return cls(**args)
 
 
-FieldConfig = common.GraphFieldConfig
+FieldConfig: typing.TypeAlias = common.GraphFieldConfig
 
 
 
 
 
 def variant_config():
     return cogruntime.PanelCfgConfig(
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/trend.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/trend.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             args["tooltip"] = common.VizTooltipOptions.from_json(data["tooltip"])
         if "xField" in data:
             args["x_field"] = data["xField"]        
 
         return cls(**args)
 
 
-FieldConfig = common.GraphFieldConfig
+FieldConfig: typing.TypeAlias = common.GraphFieldConfig
 
 
 
 
 
 def variant_config():
     return cogruntime.PanelCfgConfig(
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/grafana_foundation_sdk/models/xychart.py` & `grafana_foundation_sdk-1715088854!10.4.0/grafana_foundation_sdk/models/xychart.py`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/LICENSE.md` & `grafana_foundation_sdk-1715088854!10.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/README.md` & `grafana_foundation_sdk-1715088854!10.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 > [!NOTE]
 > This branch contains **types and builders generated for Grafana v10.4.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1713478841!10.4.0'
+python3 -m pip install 'grafana_foundation_sdk==1715088854!10.4.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/pyproject.toml` & `grafana_foundation_sdk-1715088854!10.4.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "observability",
     "sdk",
     "grafana",
     "logs",
     "traces",
     "metrics"
 ]
-version = "1713478841!10.4.0"
+version = "1715088854!10.4.0"
 dependencies = []
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `grafana_foundation_sdk-1713478841!10.4.0/PKG-INFO` & `grafana_foundation_sdk-1715088854!10.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grafana_foundation_sdk
-Version: 1713478841!10.4.0
+Version: 1715088854!10.4.0
 Summary: A set of tools, types and libraries for building and manipulating Grafana objects.
 Project-URL: Homepage, https://github.com/grafana/grafana-foundation-sdk
 Project-URL: Repository, https://github.com/grafana/grafana-foundation-sdk.git
 Project-URL: Issues, https://github.com/grafana/grafana-foundation-sdk/issues
 Author: Grafana Labs
 License-File: LICENSE.md
 Keywords: grafana,logs,metrics,observability,sdk,traces
@@ -27,15 +27,15 @@
 > [!NOTE]
 > This branch contains **types and builders generated for Grafana v10.4.x.**
 > Other supported versions of Grafana can be found at [this repository's root](https://github.com/grafana/grafana-foundation-sdk/).
 
 ## Installing
 
 ```shell
-python3 -m pip install 'grafana_foundation_sdk==1713478841!10.4.0'
+python3 -m pip install 'grafana_foundation_sdk==1715088854!10.4.0'
 ```
 
 ## Example usage
 
 ### Building a dashboard
 
 ```python
```

