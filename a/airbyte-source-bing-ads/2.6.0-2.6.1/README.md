# Comparing `tmp/airbyte_source_bing_ads-2.6.0.tar.gz` & `tmp/airbyte_source_bing_ads-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_bing_ads-2.6.0.tar", max compression
+gzip compressed data, was "airbyte_source_bing_ads-2.6.1.tar", max compression
```

## Comparing `airbyte_source_bing_ads-2.6.0.tar` & `airbyte_source_bing_ads-2.6.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     4532 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/README.md
--rw-r--r--   0        0        0      865 2024-04-29 15:48:11.141847 airbyte_source_bing_ads-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/__init__.py
--rw-r--r--   0        0        0    14454 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/base_streams.py
--rw-r--r--   0        0        0     7851 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/bulk_streams.py
--rw-r--r--   0        0        0    11425 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/client.py
--rw-r--r--   0        0        0    32975 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/report_streams.py
--rw-r--r--   0        0        0      234 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/run.py
--rw-r--r--   0        0        0     5723 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_impression_performance_report.json
--rw-r--r--   0        0        0     4545 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_impression_performance_report_hourly.json
--rw-r--r--   0        0        0     2532 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_performance_report.json
--rw-r--r--   0        0        0     2586 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_performance_report_hourly.json
--rw-r--r--   0        0        0     3550 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/accounts.json
--rw-r--r--   0        0        0     6540 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_impression_performance_report.json
--rw-r--r--   0        0        0     5159 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_impression_performance_report_hourly.json
--rw-r--r--   0        0        0      648 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_labels.json
--rw-r--r--   0        0        0     3547 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_performance_report.json
--rw-r--r--   0        0        0     3306 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_performance_report_hourly.json
--rw-r--r--   0        0        0     3618 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_groups.json
--rw-r--r--   0        0        0     3300 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_performance_report.json
--rw-r--r--   0        0        0     3198 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_performance_report_hourly.json
--rw-r--r--   0        0        0     8896 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ads.json
--rw-r--r--   0        0        0     2274 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/age_gender_audience_report.json
--rw-r--r--   0        0        0     2328 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/age_gender_audience_report_hourly.json
--rw-r--r--   0        0        0      532 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/app_install_ad_labels.json
--rw-r--r--   0        0        0     1490 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/app_install_ads.json
--rw-r--r--   0        0        0     3244 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/audience_performance_report.json
--rw-r--r--   0        0        0     3298 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/audience_performance_report_hourly.json
--rw-r--r--   0        0        0      825 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/budget.json
--rw-r--r--   0        0        0      675 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/budget_summary_report.json
--rw-r--r--   0        0        0     6912 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_impression_performance_report.json
--rw-r--r--   0        0        0     5456 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_impression_performance_report_hourly.json
--rw-r--r--   0        0        0      590 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_labels.json
--rw-r--r--   0        0        0     4008 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_performance_report.json
--rw-r--r--   0        0        0     3767 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_performance_report_hourly.json
--rw-r--r--   0        0        0     3521 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaigns.json
--rw-r--r--   0        0        0     4445 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/geographic_performance_report.json
--rw-r--r--   0        0        0     4499 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/geographic_performance_report_hourly.json
--rw-r--r--   0        0        0     1779 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/goals_and_funnels_report.json
--rw-r--r--   0        0        0     1833 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/goals_and_funnels_report_hourly.json
--rw-r--r--   0        0        0      532 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keyword_labels.json
--rw-r--r--   0        0        0     4755 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keyword_performance_report.json
--rw-r--r--   0        0        0     5018 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keyword_performance_report_daily.json
--rw-r--r--   0        0        0     4809 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keyword_performance_report_hourly.json
--rw-r--r--   0        0        0     2210 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keywords.json
--rw-r--r--   0        0        0      643 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/labels.json
--rw-r--r--   0        0        0     5371 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/product_dimension_performance_report.json
--rw-r--r--   0        0        0     5425 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/product_dimension_performance_report_hourly.json
--rw-r--r--   0        0        0     3656 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/product_search_query_performance_report.json
--rw-r--r--   0        0        0     3710 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/product_search_query_performance_report_hourly.json
--rw-r--r--   0        0        0     3752 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/search_query_performance_report.json
--rw-r--r--   0        0        0     3806 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/search_query_performance_report_hourly.json
--rw-r--r--   0        0        0     4511 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/user_location_performance_report.json
--rw-r--r--   0        0        0     4565 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/user_location_performance_report_hourly.json
--rw-r--r--   0        0        0     7578 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/source.py
--rw-r--r--   0        0        0     9533 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/spec.json
--rw-r--r--   0        0        0     1207 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/utils.py
--rw-r--r--   0        0        0     5385 1970-01-01 00:00:00.000000 airbyte_source_bing_ads-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     4532 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/README.md
+-rw-r--r--   0        0        0      869 2024-05-07 12:20:44.551148 airbyte_source_bing_ads-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/__init__.py
+-rw-r--r--   0        0        0    14454 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/base_streams.py
+-rw-r--r--   0        0        0     7851 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/bulk_streams.py
+-rw-r--r--   0        0        0    11425 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/client.py
+-rw-r--r--   0        0        0    32975 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/report_streams.py
+-rw-r--r--   0        0        0      234 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/run.py
+-rw-r--r--   0        0        0    11795 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/account_impression_performance_report.json
+-rw-r--r--   0        0        0     8503 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/account_impression_performance_report_hourly.json
+-rw-r--r--   0        0        0     4628 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/account_performance_report.json
+-rw-r--r--   0        0        0     5329 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/account_performance_report_hourly.json
+-rw-r--r--   0        0        0     5770 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/accounts.json
+-rw-r--r--   0        0        0    13592 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/ad_group_impression_performance_report.json
+-rw-r--r--   0        0        0    10513 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/ad_group_impression_performance_report_hourly.json
+-rw-r--r--   0        0        0     1243 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/ad_group_labels.json
+-rw-r--r--   0        0        0     6989 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/ad_group_performance_report.json
+-rw-r--r--   0        0        0     6784 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/ad_group_performance_report_hourly.json
+-rw-r--r--   0        0        0     6680 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/ad_groups.json
+-rw-r--r--   0        0        0     6747 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/ad_performance_report.json
+-rw-r--r--   0        0        0     6618 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/ad_performance_report_hourly.json
+-rw-r--r--   0        0        0    15046 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/ads.json
+-rw-r--r--   0        0        0     4567 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/age_gender_audience_report.json
+-rw-r--r--   0        0        0     5228 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/age_gender_audience_report_hourly.json
+-rw-r--r--   0        0        0     1055 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/app_install_ad_labels.json
+-rw-r--r--   0        0        0     3221 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/app_install_ads.json
+-rw-r--r--   0        0        0     5957 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/audience_performance_report.json
+-rw-r--r--   0        0        0     6286 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/audience_performance_report_hourly.json
+-rw-r--r--   0        0        0     1742 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/budget.json
+-rw-r--r--   0        0        0     1237 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/budget_summary_report.json
+-rw-r--r--   0        0        0    13630 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/campaign_impression_performance_report.json
+-rw-r--r--   0        0        0    10974 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/campaign_impression_performance_report_hourly.json
+-rw-r--r--   0        0        0     1225 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/campaign_labels.json
+-rw-r--r--   0        0        0     8133 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/campaign_performance_report.json
+-rw-r--r--   0        0        0     7418 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/campaign_performance_report_hourly.json
+-rw-r--r--   0        0        0     6291 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/campaigns.json
+-rw-r--r--   0        0        0     8769 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/geographic_performance_report.json
+-rw-r--r--   0        0        0     9140 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/geographic_performance_report_hourly.json
+-rw-r--r--   0        0        0     3520 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/goals_and_funnels_report.json
+-rw-r--r--   0        0        0     3421 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/goals_and_funnels_report_hourly.json
+-rw-r--r--   0        0        0     1024 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/keyword_labels.json
+-rw-r--r--   0        0        0     9338 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/keyword_performance_report.json
+-rw-r--r--   0        0        0     8502 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/keyword_performance_report_daily.json
+-rw-r--r--   0        0        0     7980 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/keyword_performance_report_hourly.json
+-rw-r--r--   0        0        0     4491 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/keywords.json
+-rw-r--r--   0        0        0     1315 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/labels.json
+-rw-r--r--   0        0        0     9913 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/product_dimension_performance_report.json
+-rw-r--r--   0        0        0    10559 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/product_dimension_performance_report_hourly.json
+-rw-r--r--   0        0        0     6683 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/product_search_query_performance_report.json
+-rw-r--r--   0        0        0     7391 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/product_search_query_performance_report_hourly.json
+-rw-r--r--   0        0        0     7571 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/search_query_performance_report.json
+-rw-r--r--   0        0        0     7209 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/search_query_performance_report_hourly.json
+-rw-r--r--   0        0        0     8657 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/user_location_performance_report.json
+-rw-r--r--   0        0        0     9547 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/user_location_performance_report_hourly.json
+-rw-r--r--   0        0        0     7578 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/source.py
+-rw-r--r--   0        0        0     9533 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/spec.json
+-rw-r--r--   0        0        0     1207 2024-05-07 10:13:35.000000 airbyte_source_bing_ads-2.6.1/source_bing_ads/utils.py
+-rw-r--r--   0        0        0     5387 1970-01-01 00:00:00.000000 airbyte_source_bing_ads-2.6.1/PKG-INFO
```

### Comparing `airbyte_source_bing_ads-2.6.0/README.md` & `airbyte_source_bing_ads-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.6.0/pyproject.toml` & `airbyte_source_bing_ads-2.6.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.6.0"
+version = "2.6.1"
 name = "airbyte-source-bing-ads"
 description = "Source implementation for Bing Ads."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -21,15 +21,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 bingads = "==13.0.18.1"
 pandas = "==2.2.0"
 urllib3 = "==1.26.18"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.84.0"
 cached-property = "==1.5.2"
 
 [tool.poetry.scripts]
 source-bing-ads = "source_bing_ads.run:run"
 
 [tool.poetry.group.dev.dependencies]
 freezegun = "^1.4.0"
```

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/__init__.py` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/base_streams.py` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/base_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/bulk_streams.py` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/bulk_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/client.py` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/client.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/report_streams.py` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/report_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_impression_performance_report.json` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/account_performance_report.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7166666666666667%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'properties'": "{'AccountName': {'description': 'Name of the Bing Ads account'}, "*

 * *                 "'AccountNumber': {'description': 'Numeric account number'}, 'AccountId': "*

 * *                 "{'description': 'Unique identifier for the Bing Ads account'}, 'TimePeriod': "*

 * *                 "{'description': 'Time period for the report'}, 'CurrencyCode': {'description': "*

 * *                 "'Currency code used for reporting'}, 'AdDistribution': {'desc […]*

```diff
@@ -1,493 +1,273 @@
 {
-    "$schema": "https://json-schema.org/draft-07/schema#",
+    "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "AbsoluteTopImpressionRatePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AbsoluteTopImpressionShareLostToBudgetPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AbsoluteTopImpressionShareLostToRankPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AbsoluteTopImpressionSharePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "AccountId": {
+            "description": "Unique identifier for the Bing Ads account",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "AccountName": {
+            "description": "Name of the Bing Ads account",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AccountNumber": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "AccountStatus": {
+            "description": "Numeric account number",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdDistribution": {
+            "description": "Type of ad distribution (search, content, both)",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AllConversionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllConversions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "AllConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllCostPerConversion": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllReturnOnAdSpend": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllRevenue": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllRevenuePerConversion": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Assists": {
+            "description": "Number of assist conversions",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AudienceImpressionLostToBudgetPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AudienceImpressionLostToRankPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AudienceImpressionSharePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AverageCPV": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "AverageCpc": {
+            "description": "Average cost per click",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AverageCpm": {
+            "description": "Average cost per thousand impressions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AveragePosition": {
+            "description": "Average ad position",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "AverageWatchTimePerImpression": {
+        "BidMatchType": {
+            "description": "Type of bidding match (exact, phrase, broad)",
             "type": [
                 "null",
-                "number"
-            ]
-        },
-        "AverageWatchTimePerVideoView": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ClickSharePercent": {
-            "type": [
-                "null",
-                "number"
+                "string"
             ]
         },
         "Clicks": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "CompletedVideoViews": {
+            "description": "Total number of clicks",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ConversionRate": {
+            "description": "Percentage of conversions from clicks",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Conversions": {
+            "description": "Total number of conversions",
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
         "ConversionsQualified": {
+            "description": "Number of qualified conversions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CostPerAssist": {
+            "description": "Cost per assist conversion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CostPerConversion": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CostPerInstall": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CostPerSale": {
+            "description": "Cost per conversion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Ctr": {
+            "description": "Click-through rate",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CurrencyCode": {
+            "description": "Currency code used for reporting",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "DeviceType": {
+        "DeliveredMatchType": {
+            "description": "Type of match in ad delivery",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ExactMatchImpressionSharePercent": {
+        "DeviceOS": {
+            "description": "Operating system of the device",
             "type": [
                 "null",
-                "number"
-            ]
-        },
-        "ImpressionLostToBudgetPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ImpressionLostToRankAggPercent": {
-            "type": [
-                "null",
-                "number"
+                "string"
             ]
         },
-        "ImpressionSharePercent": {
+        "DeviceType": {
+            "description": "Type of device used",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
         "Impressions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "Installs": {
+            "description": "Total number of ad impressions",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "LowQualityClicks": {
+            "description": "Number of low-quality clicks",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "LowQualityClicksPercent": {
+            "description": "Percentage of low-quality clicks",
             "type": [
                 "null",
                 "number"
             ]
         },
         "LowQualityConversionRate": {
+            "description": "Conversion rate for low-quality clicks",
             "type": [
                 "null",
                 "number"
             ]
         },
         "LowQualityConversions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "LowQualityConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "LowQualityGeneralClicks": {
+            "description": "Total number of low-quality conversions",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "LowQualityImpressions": {
+            "description": "Number of low-quality impressions",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "LowQualityImpressionsPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "LowQualitySophisticatedClicks": {
+            "description": "Number of sophisticated low-quality clicks",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "Network": {
+            "description": "Type of network (search, audience)",
             "type": [
                 "null",
                 "string"
             ]
         },
         "PhoneCalls": {
+            "description": "Number of phone calls generated",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "PhoneImpressions": {
+            "description": "Number of ad impressions on phone devices",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "Ptr": {
+            "description": "Phone-through rate",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ReturnOnAdSpend": {
+            "description": "Return on ad spend",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Revenue": {
+            "description": "Total revenue generated",
             "type": [
                 "null",
                 "number"
             ]
         },
         "RevenuePerAssist": {
+            "description": "Revenue per assist conversion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "RevenuePerConversion": {
+            "description": "Revenue per conversion",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "RevenuePerInstall": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "RevenuePerSale": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "Sales": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "Spend": {
+            "description": "Total spend on ad campaigns",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TimePeriod": {
+            "description": "Time period for the report",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "TopImpressionRatePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "TopImpressionShareLostToBudgetPercent": {
+        "TopVsOther": {
+            "description": "Performance comparison between top and other ad positions",
             "type": [
                 "null",
-                "number"
-            ]
-        },
-        "TopImpressionShareLostToRankPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "TopImpressionSharePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "TotalWatchTimeInMS": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoCompletionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "VideoViews": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt25Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt50Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt75Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "ViewThroughConversions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "ViewThroughConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ViewThroughRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ViewThroughRevenue": {
-            "type": [
-                "null",
-                "number"
+                "string"
             ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_performance_report.json` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/goals_and_funnels_report_hourly.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6361933479532164%*

 * *Differences: {"'additionalProperties'": 'True',*

 * * "'properties'": "{'AccountId': {'type': {insert: [(1, 'string')], delete: [1]}, 'description': "*

 * *                 "'The unique identifier of the account associated with the data.'}, 'TimePeriod': "*

 * *                 "{'format': 'date-time', 'description': 'The time period the data corresponds "*

 * *                 "to.', 'airbyte_type': 'timestamp_with_timezone'}, 'DeviceType': {'description': "*

 * *                 "'The type of device used.'}, 'DeviceOS': {'description': 'The o […]*

```diff
@@ -1,235 +1,191 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
+    "additionalProperties": true,
     "properties": {
         "AccountId": {
+            "description": "The unique identifier of the account associated with the data.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "AccountName": {
+            "description": "The name of the account associated with the data.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AccountNumber": {
+            "description": "The account number assigned to the account.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AdDistribution": {
+        "AccountStatus": {
+            "description": "The status of the account.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "Assists": {
+        "AdGroupId": {
+            "description": "The unique identifier of the ad group.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AverageCpc": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AverageCpm": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AveragePosition": {
+        "AdGroupName": {
+            "description": "The name of the ad group.",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "BidMatchType": {
+        "AdGroupStatus": {
+            "description": "The status of the ad group.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "Clicks": {
+        "AllConversions": {
+            "description": "Total number of conversions recorded.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "ConversionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "Conversions": {
+        "AllConversionsQualified": {
+            "description": "Number of qualified conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "ConversionsQualified": {
+        "AllRevenue": {
+            "description": "Total revenue generated from all conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "CostPerAssist": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CostPerConversion": {
+        "Assists": {
+            "description": "Number of assists in the conversion process.",
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
-        "Ctr": {
+        "CampaignId": {
+            "description": "The unique identifier of the campaign.",
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
-        "CurrencyCode": {
+        "CampaignName": {
+            "description": "The name of the campaign.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "DeliveredMatchType": {
+        "CampaignStatus": {
+            "description": "The status of the campaign.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "DeviceOS": {
+            "description": "The operating system of the device.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "DeviceType": {
+            "description": "The type of device used.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "Impressions": {
+        "Goal": {
+            "description": "The goal achieved.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "LowQualityClicks": {
+        "GoalId": {
+            "description": "The unique identifier of the goal.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "LowQualityClicksPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "LowQualityConversionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "LowQualityConversions": {
+        "GoalType": {
+            "description": "The type of goal achieved.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "LowQualityImpressions": {
+        "Keyword": {
+            "description": "The keyword triggered in the process.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "LowQualitySophisticatedClicks": {
+        "KeywordId": {
+            "description": "The unique identifier of the keyword.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "Network": {
+        "KeywordStatus": {
+            "description": "The status of the keyword.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "PhoneCalls": {
+        "TimePeriod": {
+            "airbyte_type": "timestamp_with_timezone",
+            "description": "The time period the data corresponds to.",
+            "format": "date-time",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "PhoneImpressions": {
+        "ViewThroughConversions": {
+            "description": "Number of view-through conversions recorded.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "Ptr": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ReturnOnAdSpend": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "Revenue": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "RevenuePerAssist": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "RevenuePerConversion": {
+        "ViewThroughConversionsQualified": {
+            "description": "Number of qualified view-through conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "Spend": {
+        "ViewThroughRevenue": {
+            "description": "Total revenue generated from view-through conversions.",
             "type": [
                 "null",
                 "number"
             ]
-        },
-        "TimePeriod": {
-            "format": "date",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "TopVsOther": {
-            "type": [
-                "null",
-                "string"
-            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_impression_performance_report.json` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/ad_group_performance_report.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.728675645342312%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'properties'": "{'AccountName': {'description': 'The name of the Bing Ads account.'}, "*

 * *                 "'AccountId': {'description': 'The unique identifier for the Bing Ads account.'}, "*

 * *                 "'TimePeriod': {'description': 'The time period for the data.'}, 'CampaignName': "*

 * *                 "{'description': 'The name of the campaign.'}, 'CampaignId': {'description': 'The "*

 * *                 "unique identifier for the campaign.'}, 'AdG […]*

```diff
@@ -1,577 +1,385 @@
 {
-    "$schema": "https://json-schema.org/draft-07/schema#",
+    "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "AbsoluteTopImpressionRatePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AbsoluteTopImpressionShareLostToBudgetPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AbsoluteTopImpressionShareLostToRankPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AbsoluteTopImpressionSharePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "AccountId": {
+            "description": "The unique identifier for the Bing Ads account.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "AccountName": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "AccountNumber": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "AccountStatus": {
+            "description": "The name of the Bing Ads account.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdDistribution": {
+            "description": "The distribution network where the ad was shown.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdGroupId": {
+            "description": "The unique identifier for the ad group.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AdGroupLabels": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "AdGroupName": {
+            "description": "The name of the ad group.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdGroupType": {
+            "description": "The type of ad group, like product ads or audience ads.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdRelevance": {
+            "description": "The relevance of the ad to its targeted keywords.",
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
         "AllConversionRate": {
+            "description": "The conversion rate across all conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllConversions": {
+            "description": "The total number of all conversions.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AllConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "AllCostPerConversion": {
+            "description": "The cost per conversion across all conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllReturnOnAdSpend": {
+            "description": "The return on ad spend across all conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllRevenue": {
+            "description": "The total revenue across all conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllRevenuePerConversion": {
+            "description": "The revenue per conversion across all conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Assists": {
+            "description": "The number of assists for conversions.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AudienceImpressionLostToBudgetPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AudienceImpressionLostToRankPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AudienceImpressionSharePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AverageCPV": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "AverageCpc": {
+            "description": "The average cost per click.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AverageCpm": {
+            "description": "The average cost per thousand impressions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AveragePosition": {
+            "description": "The average position of the ad when shown.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "AverageWatchTimePerImpression": {
+        "BidMatchType": {
+            "description": "The match type of the bid.",
             "type": [
                 "null",
-                "number"
-            ]
-        },
-        "AverageWatchTimePerVideoView": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "BaseCampaignId": {
-            "type": [
-                "null",
-                "integer"
+                "string"
             ]
         },
         "CampaignId": {
+            "description": "The unique identifier for the campaign.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "CampaignName": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "CampaignStatus": {
+            "description": "The name of the campaign.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "CampaignType": {
+            "description": "The type of campaign, like search or shopping.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ClickSharePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Clicks": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "CompletedVideoViews": {
+            "description": "The total number of clicks.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ConversionRate": {
+            "description": "The conversion rate for a specific goal.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Conversions": {
+            "description": "The total number of specified goal conversions.",
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
         "ConversionsQualified": {
+            "description": "The number of qualified conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CostPerAssist": {
+            "description": "The cost per assist for conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CostPerConversion": {
+            "description": "The cost per specified goal conversion.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "CostPerInstall": {
+        "Ctr": {
+            "description": "The click-through rate.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "CostPerSale": {
+        "CurrencyCode": {
+            "description": "The currency code used for the data.",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "Ctr": {
+        "CustomParameters": {
+            "description": "Any custom parameters associated with the ad.",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "CurrencyCode": {
+        "DeliveredMatchType": {
+            "description": "The match type when ads are shown.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "CustomParameters": {
+        "DeviceOS": {
+            "description": "The operating system of the device.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "DeviceType": {
+            "description": "The type of device where the ad was shown.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ExactMatchImpressionSharePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "ExpectedCtr": {
+            "description": "The expected click-through rate based on historical data.",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
         "FinalUrlSuffix": {
+            "description": "The suffix added to the final URL.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "HistoricalAdRelevance": {
+            "description": "The historical relevance of the ad.",
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
         "HistoricalExpectedCtr": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "HistoricalLandingPageExperience": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "HistoricalQualityScore": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "ImpressionLostToBudgetPercent": {
+            "description": "The historically expected click-through rate.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "ImpressionLostToRankAggPercent": {
+        "HistoricalLandingPageExperience": {
+            "description": "The historical landing page experience.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "ImpressionSharePercent": {
+        "HistoricalQualityScore": {
+            "description": "The historical quality score of the ad.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Impressions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "Installs": {
+            "description": "The total number of impressions.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "LandingPageExperience": {
+            "description": "The landing page experience score.",
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
         "Language": {
+            "description": "The language used in the ad.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Network": {
+            "description": "The network where the ad was shown.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "PhoneCalls": {
+            "description": "The number of phone calls made as a result of the ad.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "PhoneImpressions": {
+            "description": "The number of times phone number was shown.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "Ptr": {
+            "description": "The phone-through rate.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "QualityScore": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "RelativeCtr": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ReturnOnAdSpend": {
+            "description": "The quality score of the ad.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Revenue": {
+            "description": "The total revenue generated.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "RevenuePerAssist": {
+            "description": "The revenue per assist for conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "RevenuePerConversion": {
+            "description": "The revenue per specified goal conversion.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "RevenuePerInstall": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "RevenuePerSale": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "Sales": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "Spend": {
+            "description": "The total spend for the specified period.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "Status": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "TimePeriod": {
+            "description": "The time period for the data.",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "TopImpressionRatePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "TopImpressionShareLostToBudgetPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "TopImpressionShareLostToRankPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "TopImpressionSharePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "TotalWatchTimeInMS": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "TrackingTemplate": {
+        "TopVsOther": {
+            "description": "The performance in top positions versus other positions.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "VideoCompletionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "VideoViews": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt25Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt50Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt75Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "ViewThroughConversions": {
+            "description": "The number of view-through conversions recorded.",
             "type": [
                 "null",
                 "integer"
             ]
-        },
-        "ViewThroughConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ViewThroughRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ViewThroughRevenue": {
-            "type": [
-                "null",
-                "number"
-            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_impression_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/audience_performance_report.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5393288352272727%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'additionalProperties'": 'True',*

 * * "'properties'": "{'AccountName': {'description': 'The name of the account'}, 'AccountNumber': "*

 * *                 "{'description': 'The account number'}, 'AccountId': {'description': 'The unique "*

 * *                 "identifier for the account'}, 'TimePeriod': {'format': 'date', 'description': "*

 * *                 "'The time period of the report', delete: ['airbyte_type']}, 'CampaignName': "*

 * *                 "{'descrip […]*

```diff
@@ -1,469 +1,343 @@
 {
-    "$schema": "https://json-schema.org/draft-07/schema#",
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "additionalProperties": true,
     "properties": {
         "AbsoluteTopImpressionRatePercent": {
+            "description": "The percentage of absolute top impressions compared to total impressions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AccountId": {
+            "description": "The unique identifier for the account",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "AccountName": {
+            "description": "The name of the account",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AccountNumber": {
+            "description": "The account number",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AccountStatus": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "AdDistribution": {
+            "description": "The status of the account",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdGroupId": {
+            "description": "The unique identifier for the ad group",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AdGroupLabels": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "AdGroupName": {
+            "description": "The name of the ad group",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AdGroupType": {
+        "AdGroupStatus": {
+            "description": "The status of the ad group",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AdRelevance": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "AllConversionRate": {
+            "description": "The rate of all conversions generated",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllConversions": {
+            "description": "The total number of all conversions",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "AllConversionsQualified": {
+            "description": "The number of all conversions qualified",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllCostPerConversion": {
+            "description": "The cost per all conversion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllReturnOnAdSpend": {
+            "description": "The return on ad spend for all conversions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllRevenue": {
+            "description": "The total revenue generated from all conversions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllRevenuePerConversion": {
+            "description": "The revenue per all conversion",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "Assists": {
+        "AssociationId": {
+            "description": "The unique identifier for the association",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AverageCPV": {
+        "AssociationLevel": {
+            "description": "The level of the association",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "AverageCpc": {
+        "AssociationStatus": {
+            "description": "The status of the association",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "AverageCpm": {
+        "AudienceId": {
+            "description": "The unique identifier for the audience",
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
-        "AveragePosition": {
+        "AudienceName": {
+            "description": "The name of the audience",
             "type": [
                 "null",
-                "number"
+                "string"
+            ]
+        },
+        "AudienceType": {
+            "description": "The type of the audience",
+            "type": [
+                "null",
+                "string"
             ]
         },
-        "AverageWatchTimePerImpression": {
+        "AverageCpc": {
+            "description": "The average cost per click",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "AverageWatchTimePerVideoView": {
+        "AverageCpm": {
+            "description": "The average cost per thousand impressions",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "BaseCampaignId": {
+        "AveragePosition": {
+            "description": "The average position of the ad",
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
-        "CampaignId": {
+        "BaseCampaignId": {
+            "description": "The base campaign's ID",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "CampaignName": {
+        "BidAdjustment": {
+            "description": "The bid adjustment value",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "CampaignStatus": {
+        "CampaignId": {
+            "description": "The unique identifier for the campaign",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "CampaignType": {
+        "CampaignName": {
+            "description": "The name of the campaign",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "Clicks": {
+        "CampaignStatus": {
+            "description": "The status of the campaign",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "CompletedVideoViews": {
+        "Clicks": {
+            "description": "The total number of clicks",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ConversionRate": {
+            "description": "The rate of conversions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Conversions": {
+            "description": "The total number of conversions",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CostPerAssist": {
+            "description": "The number of conversions qualified",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CostPerConversion": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CostPerInstall": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CostPerSale": {
+            "description": "The cost per conversion",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Ctr": {
+            "description": "The click-through rate",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "CurrencyCode": {
+        "Goal": {
+            "description": "The goal of the report",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "CustomParameters": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "DeviceType": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "ExpectedCtr": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "FinalUrlSuffix": {
+        "GoalType": {
+            "description": "The type of goal",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Impressions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "Installs": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "LandingPageExperience": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "Language": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Network": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "PhoneCalls": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "PhoneImpressions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "Ptr": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "QualityScore": {
+            "description": "The total number of impressions",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ReturnOnAdSpend": {
+            "description": "The return on ad spend",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Revenue": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "RevenuePerAssist": {
+            "description": "The total revenue",
             "type": [
                 "null",
                 "number"
             ]
         },
         "RevenuePerConversion": {
+            "description": "The revenue per conversion",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "RevenuePerInstall": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "RevenuePerSale": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "Sales": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "Spend": {
+            "description": "The total spend",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "Status": {
+        "TargetingSetting": {
+            "description": "The targeting settings used",
             "type": [
                 "null",
                 "string"
             ]
         },
         "TimePeriod": {
-            "airbyte_type": "timestamp_with_timezone",
-            "format": "date-time",
+            "description": "The time period of the report",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
         "TopImpressionRatePercent": {
+            "description": "The percentage of top impressions compared to total impressions",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "TopImpressionSharePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "TotalWatchTimeInMS": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "TrackingTemplate": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "VideoCompletionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "VideoViews": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt25Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt50Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt75Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "ViewThroughConversions": {
+            "description": "The total number of view-through conversions",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ViewThroughConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ViewThroughRate": {
+            "description": "The number of view-through conversions qualified",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ViewThroughRevenue": {
+            "description": "The total revenue generated from view-through conversions",
             "type": [
                 "null",
                 "number"
             ]
         }
     },
     "type": "object"
```

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/app_install_ads.json` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/keyword_labels.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8620580808080808%*

 * *Differences: {"'properties'": "{'Client Id': {'type': {insert: [(1, 'string')], delete: [1]}, 'description': "*

 * *                 "'Unique identifier for the client associated with the keyword label.'}, 'Id': "*

 * *                 "{'description': 'Unique identifier for the keyword label.'}, 'Modified Time': "*

 * *                 "{'description': 'Timestamp indicating when the keyword label was last "*

 * *                 "modified.'}, 'Parent Id': {'description': 'Unique identifier for the parent "*

 * *                 "entity related […]*

```diff
@@ -1,133 +1,49 @@
 {
     "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
-        "Ad Group": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "App Id": {
+        "Account Id": {
+            "description": "Unique identifier for the account associated with the keyword label.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "Campaign": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "Client Id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "Custom Parameter": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Device Preference": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Editorial Appeal Status": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Editorial Location": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Editorial Reason Code": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Editorial Status": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Editorial Term": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Final Url": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Final Url Suffix": {
+            "description": "Unique identifier for the client associated with the keyword label.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Id": {
+            "description": "Unique identifier for the keyword label.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "Modified Time": {
             "airbyte_type": "timestamp_with_timezone",
+            "description": "Timestamp indicating when the keyword label was last modified.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Parent Id": {
+            "description": "Unique identifier for the parent entity related to the keyword label.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "Publisher Countries": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "Status": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Text": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Title": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Tracking Template": {
+            "description": "Current status of the keyword label.",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": "object"
```

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_impression_performance_report.json` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/search_query_performance_report.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8719907407407407%*

 * *Differences: {"'properties'": "{'AccountName': {'description': 'The name of the Bing Ads account.'}, "*

 * *                 "'AccountNumber': {'description': 'The account number associated with the Bing "*

 * *                 "Ads account.'}, 'AccountId': {'description': 'The unique identifier of the Bing "*

 * *                 "Ads account.'}, 'TimePeriod': {'description': 'The time period of the data.'}, "*

 * *                 "'CampaignStatus': {'description': 'The status of the campaign.'}, "*

 * *                 "'CampaignName': {'des […]*

```diff
@@ -1,601 +1,413 @@
 {
     "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
         "AbsoluteTopImpressionRatePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AbsoluteTopImpressionShareLostToBudgetPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AbsoluteTopImpressionShareLostToRankPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AbsoluteTopImpressionSharePercent": {
+            "description": "The percentage of impressions shown at the absolute top of the search results page.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AccountId": {
+            "description": "The unique identifier of the Bing Ads account.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "AccountName": {
+            "description": "The name of the Bing Ads account.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AccountNumber": {
+            "description": "The account number associated with the Bing Ads account.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AccountStatus": {
+            "description": "The status of the Bing Ads account.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AdDistribution": {
+        "AdGroupCriterionId": {
+            "description": "The unique identifier of the ad group criterion.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AdRelevance": {
+        "AdGroupId": {
+            "description": "The unique identifier of the ad group.",
             "type": [
                 "null",
-                "number"
-            ]
-        },
-        "AllConversionRate": {
-            "type": [
-                "null",
-                "number"
+                "integer"
             ]
         },
-        "AllConversions": {
+        "AdGroupName": {
+            "description": "The name of the ad group.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "AllConversionsQualified": {
+        "AdGroupStatus": {
+            "description": "The status of the ad group.",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "AllCostPerConversion": {
+        "AdId": {
+            "description": "The unique identifier of the ad.",
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
-        "AllReturnOnAdSpend": {
+        "AdStatus": {
+            "description": "The status of the ad.",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "AllRevenue": {
+        "AdType": {
+            "description": "The type of ad (text ad, responsive ad, etc.).",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "AllRevenuePerConversion": {
+        "AllConversionRate": {
+            "description": "The percentage of all clicks that resulted in a conversion.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "Assists": {
+        "AllConversions": {
+            "description": "The total number of all conversions.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AudienceImpressionLostToBudgetPercent": {
+        "AllConversionsQualified": {
+            "description": "The total number of qualified conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "AudienceImpressionLostToRankPercent": {
+        "AllCostPerConversion": {
+            "description": "The cost per conversion for all conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "AudienceImpressionSharePercent": {
+        "AllReturnOnAdSpend": {
+            "description": "The return on ad spend for all conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "AverageCPV": {
+        "AllRevenue": {
+            "description": "The total revenue generated from all conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "AverageCpc": {
+        "AllRevenuePerConversion": {
+            "description": "The average revenue per conversion for all conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "AverageCpm": {
+        "Assists": {
+            "description": "The number of assists on conversions.",
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
-        "AveragePosition": {
+        "AverageCpc": {
+            "description": "The average cost per click.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "AverageWatchTimePerImpression": {
+        "AverageCpm": {
+            "description": "The average cost per thousand impressions.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "AverageWatchTimePerVideoView": {
+        "AveragePosition": {
+            "description": "The average position of the ad on search results pages.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "BaseCampaignId": {
+        "BidMatchType": {
+            "description": "The type of match (bidded, auto, etc.) for the keyword bid.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "CampaignId": {
+            "description": "The unique identifier of the campaign.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "CampaignLabels": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "CampaignName": {
+            "description": "The name of the campaign.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "CampaignStatus": {
+            "description": "The status of the campaign.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "CampaignType": {
+            "description": "The type of campaign (search, display, etc.).",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ClickSharePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Clicks": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "CompletedVideoViews": {
+            "description": "The total number of clicks.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ConversionRate": {
+            "description": "The percentage of clicks that resulted in a conversion.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Conversions": {
+            "description": "The total number of conversions.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ConversionsQualified": {
+            "description": "The total number of qualified conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CostPerAssist": {
+            "description": "The cost per assist on conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CostPerConversion": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CostPerInstall": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CostPerSale": {
+            "description": "The cost per conversion.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Ctr": {
+            "description": "The click-through rate.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "CurrencyCode": {
+        "CustomerId": {
+            "description": "The unique identifier of the customer.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "CustomParameters": {
+        "CustomerName": {
+            "description": "The name of the customer.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "DeviceType": {
+        "DeliveredMatchType": {
+            "description": "The type of match (exact, broad, etc.) for the keyword delivery.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ExactMatchImpressionSharePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ExpectedCtr": {
+        "DestinationUrl": {
+            "description": "The URL where the ad directs traffic.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "FinalUrlSuffix": {
+        "DeviceOS": {
+            "description": "The operating system of the device where the ad was displayed.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "HistoricalAdRelevance": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "HistoricalExpectedCtr": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "HistoricalLandingPageExperience": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "HistoricalQualityScore": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "ImpressionLostToBudgetPercent": {
+        "DeviceType": {
+            "description": "The type of device (desktop, mobile, tablet, etc.).",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "ImpressionLostToRankAggPercent": {
+        "Goal": {
+            "description": "The goal associated with the campaign.",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "ImpressionSharePercent": {
+        "GoalType": {
+            "description": "The type of goal (e.g., ROAS, CPA) for the campaign.",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
         "Impressions": {
+            "description": "The total number of times the ad was shown.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "Installs": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "LandingPageExperience": {
+        "Keyword": {
+            "description": "The keyword associated with the ad.",
             "type": [
                 "null",
-                "number"
-            ]
-        },
-        "LowQualityClicks": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "LowQualityClicksPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "LowQualityConversionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "LowQualityConversions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "LowQualityConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "LowQualityGeneralClicks": {
-            "type": [
-                "null",
-                "integer"
+                "string"
             ]
         },
-        "LowQualityImpressions": {
+        "KeywordId": {
+            "description": "The unique identifier of the keyword.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "LowQualityImpressionsPercent": {
+        "KeywordStatus": {
+            "description": "The status of the keyword.",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "LowQualitySophisticatedClicks": {
+        "Language": {
+            "description": "The language setting targeted by the ad.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "Network": {
+            "description": "The network where the ad was shown (Bing, partner sites, etc.).",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "PhoneCalls": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "PhoneImpressions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "Ptr": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "QualityScore": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "RelativeCtr": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "ReturnOnAdSpend": {
+            "description": "The return on ad spend.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Revenue": {
+            "description": "The total revenue generated.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "RevenuePerAssist": {
+            "description": "The average revenue per assist.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "RevenuePerConversion": {
+            "description": "The average revenue per conversion.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "RevenuePerInstall": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "RevenuePerSale": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "Sales": {
+        "SearchQuery": {
+            "description": "The search query that triggered the ad.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "Spend": {
+            "description": "The total spend on the ad.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TimePeriod": {
+            "description": "The time period of the data.",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
         "TopImpressionRatePercent": {
+            "description": "The percentage of impressions shown at the top of the search results page.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "TopImpressionShareLostToBudgetPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "TopImpressionShareLostToRankPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "TopImpressionSharePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "TotalWatchTimeInMS": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "TrackingTemplate": {
+        "TopVsOther": {
+            "description": "Indicates if the ad was shown in the top position or elsewhere.",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "VideoCompletionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "VideoViews": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt25Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt50Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt75Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "ViewThroughConversions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "ViewThroughConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ViewThroughRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ViewThroughRevenue": {
-            "type": [
-                "null",
-                "number"
-            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_impression_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/account_performance_report_hourly.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7173445767195767%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'properties'": "{'AccountName': {'description': 'The name of the Bing Ads account'}, "*

 * *                 "'AccountNumber': {'description': 'The account number associated with the Bing "*

 * *                 "Ads account'}, 'AccountId': {'description': 'The unique identifier for the Bing "*

 * *                 "Ads account'}, 'TimePeriod': {'description': 'The time period for the report "*

 * *                 "data'}, 'CurrencyCode': {'description': 'The curren […]*

```diff
@@ -1,488 +1,274 @@
 {
-    "$schema": "https://json-schema.org/draft-07/schema#",
+    "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "AbsoluteTopImpressionRatePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "AccountId": {
+            "description": "The unique identifier for the Bing Ads account",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "AccountName": {
+            "description": "The name of the Bing Ads account",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AccountNumber": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "AccountStatus": {
+            "description": "The account number associated with the Bing Ads account",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdDistribution": {
+            "description": "The distribution network for the ad (search partners, audience network, etc.)",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AdRelevance": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllConversionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllConversions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "AllConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllCostPerConversion": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllReturnOnAdSpend": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllRevenue": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllRevenuePerConversion": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Assists": {
+            "description": "The number of assists generated by the ad",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AverageCPV": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "AverageCpc": {
+            "description": "The average cost per click for the ad",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AverageCpm": {
+            "description": "The average cost per thousand impressions for the ad",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AveragePosition": {
+            "description": "The average position where the ad appeared on the search results page",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "AverageWatchTimePerImpression": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AverageWatchTimePerVideoView": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "BaseCampaignId": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "CampaignId": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "CampaignLabels": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "CampaignName": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "CampaignStatus": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "CampaignType": {
+        "BidMatchType": {
+            "description": "The match type for which the bid was set",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Clicks": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "CompletedVideoViews": {
+            "description": "The total number of clicks on the ad",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ConversionRate": {
+            "description": "The rate at which clicks on the ad led to conversions",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Conversions": {
+            "description": "The total number of conversions generated by the ad",
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
         "ConversionsQualified": {
+            "description": "The number of conversions that met certain criteria",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CostPerAssist": {
+            "description": "The cost per assist generated by the ad",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CostPerConversion": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CostPerInstall": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CostPerSale": {
+            "description": "The cost per conversion generated by the ad",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Ctr": {
+            "description": "The click-through rate for the ad",
             "type": [
                 "null",
                 "number"
             ]
         },
         "CurrencyCode": {
+            "description": "The currency code used for monetary values",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "CustomParameters": {
+        "DeliveredMatchType": {
+            "description": "The match type for the delivered ad",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "DeviceType": {
+        "DeviceOS": {
+            "description": "The operating system of the device on which the ad was displayed",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ExpectedCtr": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "FinalUrlSuffix": {
+        "DeviceType": {
+            "description": "The type of device on which the ad was displayed",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Impressions": {
+            "description": "The total number of impressions generated by the ad",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "Installs": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "LandingPageExperience": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "LowQualityClicks": {
+            "description": "The number of low-quality clicks on the ad",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "LowQualityClicksPercent": {
+            "description": "The percentage of low-quality clicks out of total clicks",
             "type": [
                 "null",
                 "number"
             ]
         },
         "LowQualityConversionRate": {
+            "description": "The conversion rate for low-quality clicks",
             "type": [
                 "null",
                 "number"
             ]
         },
         "LowQualityConversions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "LowQualityConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "LowQualityGeneralClicks": {
+            "description": "The number of conversions from low-quality clicks",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "LowQualityImpressions": {
+            "description": "The number of low-quality impressions generated by the ad",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "LowQualityImpressionsPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "LowQualitySophisticatedClicks": {
+            "description": "The number of sophisticated clicks recognized as low-quality",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "Network": {
+            "description": "The network on which the ad appeared (e.g., Bing, AOL)",
             "type": [
                 "null",
                 "string"
             ]
         },
         "PhoneCalls": {
+            "description": "The number of phone calls generated by the ad",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "PhoneImpressions": {
+            "description": "The number of impressions that included a phone number",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "Ptr": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "QualityScore": {
+            "description": "The phone-through rate for the ad",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ReturnOnAdSpend": {
+            "description": "The return on ad spend (ROAS) for the ad campaign",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Revenue": {
+            "description": "The total revenue generated by the ad",
             "type": [
                 "null",
                 "number"
             ]
         },
         "RevenuePerAssist": {
+            "description": "The revenue per assist generated by the ad",
             "type": [
                 "null",
                 "number"
             ]
         },
         "RevenuePerConversion": {
+            "description": "The revenue per conversion generated by the ad",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "RevenuePerInstall": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "RevenuePerSale": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "Sales": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "Spend": {
+            "description": "The total spend on the ad campaign",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TimePeriod": {
             "airbyte_type": "timestamp_with_timezone",
+            "description": "The time period for the report data",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "TopImpressionRatePercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "TotalWatchTimeInMS": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "TrackingTemplate": {
+        "TopVsOther": {
+            "description": "Indicates whether the ad appeared at the top or other positions",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "VideoCompletionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "VideoViews": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt25Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt50Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "VideoViewsAt75Percent": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "ViewThroughConversions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "ViewThroughConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ViewThroughRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ViewThroughRevenue": {
-            "type": [
-                "null",
-                "number"
-            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/app_install_ads.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft-07/schema#'",*

 * * "'properties'": "{replace: OrderedDict([('Ad Group', OrderedDict([('description', 'The name or ID "*

 * *                 "of the ad group to which the app install ad belongs.'), ('type', ['null', "*

 * *                 "'string'])])), ('App Id', OrderedDict([('description', 'The unique identifier of "*

 * *                 "the mobile app being promoted.'), ('type', ['null', 'integer'])])), ('Campaign', "*

 * *                 "OrderedDict([('description', 'The nam […]*

```diff
@@ -1,344 +1,155 @@
 {
-    "$schema": "http://json-schema.org/draft-07/schema#",
+    "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
-        "AccountId": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "AccountName": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "AdDistribution": {
+        "Ad Group": {
+            "description": "The name or ID of the ad group to which the app install ad belongs.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AdRelevance": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllConversionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllConversions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "AllCostPerConversion": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllReturnOnAdSpend": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllRevenue": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllRevenuePerConversion": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "Assists": {
+        "App Id": {
+            "description": "The unique identifier of the mobile app being promoted.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AverageCpc": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AverageCpm": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AveragePosition": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "BidMatchType": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "BudgetAssociationStatus": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "BudgetName": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "BudgetStatus": {
+        "Campaign": {
+            "description": "The name or ID of the advertising campaign associated with the app install ad.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "CampaignId": {
+        "Client Id": {
+            "description": "The unique identifier of the client or advertiser account.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "CampaignLabels": {
+        "Custom Parameter": {
+            "description": "Optional custom parameters configured for tracking purposes.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "CampaignName": {
+        "Device Preference": {
+            "description": "Device preference targeting for the app install ad.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "CampaignStatus": {
+        "Editorial Appeal Status": {
+            "description": "The editorial appeal status of the ad.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "CampaignType": {
+        "Editorial Location": {
+            "description": "The editorial location where the ad is being reviewed.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "Clicks": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "ConversionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "Conversions": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CostPerAssist": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CostPerConversion": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "Ctr": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CurrencyCode": {
+        "Editorial Reason Code": {
+            "description": "The editorial reason code indicating the reason for disapproval of the ad.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "CustomParameters": {
+        "Editorial Status": {
+            "description": "The editorial status of the ad (e.g., pending, approved, disapproved).",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "DeliveredMatchType": {
+        "Editorial Term": {
+            "description": "The editorial term triggered in the review process.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "DeviceOS": {
+        "Final Url": {
+            "description": "The final URL users are directed to after clicking the app install ad.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "DeviceType": {
+        "Final Url Suffix": {
+            "description": "Additional tracking information appended to the final URL.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "Impressions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "LandingPageExperience": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "LowQualityClicks": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "LowQualityClicksPercent": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "LowQualityConversionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "LowQualityConversions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "LowQualityImpressions": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "LowQualitySophisticatedClicks": {
+        "Id": {
+            "description": "The unique identifier of the app install ad.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "Network": {
+        "Modified Time": {
+            "airbyte_type": "timestamp_with_timezone",
+            "description": "The date and time when the app install ad was last modified.",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "PhoneCalls": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "PhoneImpressions": {
+        "Parent Id": {
+            "description": "The ID of the parent object to which the app install ad belongs.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "Ptr": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "QualityScore": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ReturnOnAdSpend": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "Revenue": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "RevenuePerAssist": {
+        "Publisher Countries": {
+            "description": "List of countries targeted for publishing the app install ad.",
             "type": [
                 "null",
-                "number"
-            ]
-        },
-        "RevenuePerConversion": {
-            "type": [
-                "null",
-                "number"
+                "string"
             ]
         },
-        "Spend": {
+        "Status": {
+            "description": "The status of the app install ad (e.g., enabled, paused, deleted).",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "TimePeriod": {
-            "airbyte_type": "timestamp_with_timezone",
-            "format": "date-time",
+        "Text": {
+            "description": "The text content of the app install ad.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "TopVsOther": {
+        "Title": {
+            "description": "The title of the app install ad.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ViewThroughConversions": {
+        "Tracking Template": {
+            "description": "The tracking template URL for monitoring ad performance.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keyword_performance_report_daily.json` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/schemas/age_gender_audience_report.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7108739837398375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft-07/schema#'",*

 * * "'properties'": "{'AccountId': {'description': 'The ID of the Bing Ads account.'}, 'CampaignId': "*

 * *                 "{'description': 'The ID of the campaign.'}, 'AdGroupId': {'description': 'The ID "*

 * *                 "of the ad group.'}, 'TimePeriod': {'description': 'The time period for which the "*

 * *                 "data is reported.'}, 'AdDistribution': {'description': 'The type of ad "*

 * *                 "distribution, such as search or content n […]*

```diff
@@ -1,468 +1,244 @@
 {
-    "$schema": "http://json-schema.org/draft-07/schema#",
+    "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
         "AbsoluteTopImpressionRatePercent": {
+            "description": "The percentage of times your ad was shown at the absolute top of the search results page.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AccountId": {
+            "description": "The ID of the Bing Ads account.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "AccountName": {
+            "description": "The name of the Bing Ads account.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AccountNumber": {
+            "description": "The account number associated with the Bing Ads account.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AccountStatus": {
+            "description": "The status of the Bing Ads account.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdDistribution": {
+            "description": "The type of ad distribution, such as search or content network.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdGroupId": {
+            "description": "The ID of the ad group.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "AdGroupName": {
+            "description": "The name of the ad group.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdGroupStatus": {
+            "description": "The status of the ad group.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AdId": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "AdRelevance": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AdType": {
+        "AgeGroup": {
+            "description": "The age group of the audience targeted by the ad campaign.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AllConversionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "AllConversions": {
+            "description": "The total number of conversions.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AllCostPerConversion": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllReturnOnAdSpend": {
+        "AllConversionsQualified": {
+            "description": "The total number of qualified conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllRevenue": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AllRevenuePerConversion": {
+            "description": "The total revenue generated from all conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Assists": {
+            "description": "The number of assists that contributed to conversions.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AverageCpc": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AverageCpm": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "AveragePosition": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "BaseCampaignId": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "BidMatchType": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "BidStrategyType": {
+            "description": "The ID of the base campaign.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "CampaignId": {
+            "description": "The ID of the campaign.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "CampaignName": {
+            "description": "The name of the campaign.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "CampaignStatus": {
+            "description": "The status of the campaign.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Clicks": {
+            "description": "The number of clicks on the ad.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "ConversionRate": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Conversions": {
+            "description": "The number of conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "ConversionsQualified": {
+            "description": "The number of qualified conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "CostPerAssist": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CostPerConversion": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "Ctr": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "CurrencyCode": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "CurrentMaxCpc": {
+        "ExtendedCost": {
+            "description": "The total cost extended due to possible monthly budget overspend.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "CustomParameters": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "DeliveredMatchType": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "DestinationUrl": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "DeviceOS": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "DeviceType": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "ExpectedCtr": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "FinalAppUrl": {
+        "Gender": {
+            "description": "The gender of the audience targeted by the ad campaign.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "FinalMobileUrl": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "FinalUrl": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "FinalUrlSuffix": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "FirstPageBid": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Goal": {
+            "description": "The goal set for the ad campaign.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "GoalType": {
+            "description": "The type of goal set for the ad campaign.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "HistoricalAdRelevance": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "HistoricalExpectedCtr": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "HistoricalLandingPageExperience": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "HistoricalQualityScore": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Impressions": {
+            "description": "The number of times the ad was displayed.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "Keyword": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "KeywordId": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "KeywordLabels": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "KeywordStatus": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "LandingPageExperience": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Language": {
+            "description": "The language used in targeting the audience.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "Mainline1Bid": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "MainlineBid": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "Network": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "QualityImpact": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "QualityScore": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "ReturnOnAdSpend": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Revenue": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "RevenuePerAssist": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "RevenuePerConversion": {
+            "description": "The total revenue generated from conversions.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "Spend": {
+            "description": "The total amount spent on the ad campaign.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "TimePeriod": {
+            "description": "The time period for which the data is reported.",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
         "TopImpressionRatePercent": {
+            "description": "The percentage of times your ad was shown above organic search results.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "TopVsOther": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "TrackingTemplate": {
+        "ViewThroughConversions": {
+            "description": "The number of view-through conversions.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "ViewThroughConversions": {
+        "ViewThroughConversionsQualified": {
+            "description": "The number of qualified view-through conversions.",
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
-        "ViewThroughConversionsQualified": {
+        "ViewThroughRevenue": {
+            "description": "The total revenue generated from view-through conversions.",
             "type": [
                 "null",
                 "number"
             ]
         }
     },
     "type": "object"
```

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/source.py` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/spec.json` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.6.0/source_bing_ads/utils.py` & `airbyte_source_bing_ads-2.6.1/source_bing_ads/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.6.0/PKG-INFO` & `airbyte_source_bing_ads-2.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-bing-ads
-Version: 2.6.0
+Version: 2.6.1
 Summary: Source implementation for Bing Ads.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.84.0)
 Requires-Dist: bingads (==13.0.18.1)
 Requires-Dist: cached-property (==1.5.2)
 Requires-Dist: pandas (==2.2.0)
 Requires-Dist: urllib3 (==1.26.18)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/bing-ads
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
```

