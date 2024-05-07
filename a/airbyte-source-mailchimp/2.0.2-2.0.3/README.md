# Comparing `tmp/airbyte_source_mailchimp-2.0.2.tar.gz` & `tmp/airbyte_source_mailchimp-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_mailchimp-2.0.2.tar", max compression
+gzip compressed data, was "airbyte_source_mailchimp-2.0.3.tar", max compression
```

## Comparing `airbyte_source_mailchimp-2.0.2.tar` & `airbyte_source_mailchimp-2.0.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     4550 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/README.md
--rw-r--r--   0        0        0      781 2024-04-25 13:07:21.351862 airbyte_source_mailchimp-2.0.2/pyproject.toml
--rw-r--r--   0        0        0       67 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/__init__.py
--rw-r--r--   0        0        0     2528 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/components.py
--rw-r--r--   0        0        0     3724 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/config_migrations.py
--rw-r--r--   0        0        0    11728 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/manifest.yaml
--rw-r--r--   0        0        0      356 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/run.py
--rw-r--r--   0        0        0     4542 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/automations.json
--rw-r--r--   0        0        0    29465 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/campaigns.json
--rw-r--r--   0        0        0     1987 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/email_activity.json
--rw-r--r--   0        0        0      383 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/interest_categories.json
--rw-r--r--   0        0        0      455 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/interests.json
--rw-r--r--   0        0        0     4162 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/list_members.json
--rw-r--r--   0        0        0    12237 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/lists.json
--rw-r--r--   0        0        0    19375 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/reports.json
--rw-r--r--   0        0        0     2720 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/segment_members.json
--rw-r--r--   0        0        0     1333 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/segments.json
--rw-r--r--   0        0        0      930 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/addressMergeSegment.json
--rw-r--r--   0        0        0     1085 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/addressZipWithinSegment.json
--rw-r--r--   0        0        0     1054 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/aimSegment.json
--rw-r--r--   0        0        0     1113 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/automationSegment.json
--rw-r--r--   0        0        0      883 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/birthdayMergeSegment.json
--rw-r--r--   0        0        0      852 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/campaignPollSegment.json
--rw-r--r--   0        0        0      263 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/campaignStatus.json
--rw-r--r--   0        0        0      396 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/campaignType.json
--rw-r--r--   0        0        0     1070 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/conversationSegment.json
--rw-r--r--   0        0        0     1021 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/countryStateSegment.json
--rw-r--r--   0        0        0      897 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/dateMergeSegment.json
--rw-r--r--   0        0        0     1510 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/dateSegment.json
--rw-r--r--   0        0        0      908 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/dropdownRadioMergeSegment.json
--rw-r--r--   0        0        0     1103 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/ecommCategorySegment.json
--rw-r--r--   0        0        0     1283 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/ecommNumberSegment.json
--rw-r--r--   0        0        0      741 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/ecommPurchasedSegment.json
--rw-r--r--   0        0        0      923 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/ecommSpentSegment.json
--rw-r--r--   0        0        0      856 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/ecommStoreSegment.json
--rw-r--r--   0        0        0      958 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/emailClientSegment.json
--rw-r--r--   0        0        0     1039 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/emailSegment.json
--rw-r--r--   0        0        0      924 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/fuzzySegment.json
--rw-r--r--   0        0        0     1455 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/geoInSegment.json
--rw-r--r--   0        0        0      964 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/goalActivitySegment.json
--rw-r--r--   0        0        0      971 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/goalTimestampSegment.json
--rw-r--r--   0        0        0     1096 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/interestSegment.json
--rw-r--r--   0        0        0     1039 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/ipGeoInZipSegment.json
--rw-r--r--   0        0        0      856 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/languageSegment.json
--rw-r--r--   0        0        0      939 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/memberRatingSegment.json
--rw-r--r--   0        0        0      823 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/newSubscribers.json
--rw-r--r--   0        0        0      874 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/predictedAgeSegment.json
--rw-r--r--   0        0        0      862 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/predictedGenderSegment.json
--rw-r--r--   0        0        0     2773 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/segmentCondition.json
--rw-r--r--   0        0        0      917 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/segmentationOptions.json
--rw-r--r--   0        0        0      840 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/signupSourceSegment.json
--rw-r--r--   0        0        0      922 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/socialAgeSegment.json
--rw-r--r--   0        0        0      941 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/socialGenderSegment.json
--rw-r--r--   0        0        0      988 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/socialInfluenceSegment.json
--rw-r--r--   0        0        0     1023 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/socialNetworkFollowSegment.json
--rw-r--r--   0        0        0     1177 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/socialNetworkSegment.json
--rw-r--r--   0        0        0      894 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/staticSegment.json
--rw-r--r--   0        0        0     1083 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/surveyMonkeySegment.json
--rw-r--r--   0        0        0     1127 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/textOrNumberMergeSegment.json
--rw-r--r--   0        0        0      751 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/unknownSegment.json
--rw-r--r--   0        0        0      639 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/vipSegment.json
--rw-r--r--   0        0        0      896 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/zipSegment.json
--rw-r--r--   0        0        0      265 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/tags.json
--rw-r--r--   0        0        0      782 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/unsubscribes.json
--rw-r--r--   0        0        0      287 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/source.py
--rw-r--r--   0        0        0     4138 2024-04-25 12:01:10.000000 airbyte_source_mailchimp-2.0.2/source_mailchimp/spec.json
--rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 airbyte_source_mailchimp-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4550 2024-05-07 10:35:31.000000 airbyte_source_mailchimp-2.0.3/README.md
+-rw-r--r--   0        0        0      785 2024-05-07 12:30:29.612578 airbyte_source_mailchimp-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0       67 2024-05-07 10:35:31.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/__init__.py
+-rw-r--r--   0        0        0     2528 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/components.py
+-rw-r--r--   0        0        0     3724 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/config_migrations.py
+-rw-r--r--   0        0        0    11728 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/manifest.yaml
+-rw-r--r--   0        0        0      356 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/run.py
+-rw-r--r--   0        0        0     7700 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/automations.json
+-rw-r--r--   0        0        0    29651 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/campaigns.json
+-rw-r--r--   0        0        0     1987 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/email_activity.json
+-rw-r--r--   0        0        0      802 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/interest_categories.json
+-rw-r--r--   0        0        0      943 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/interests.json
+-rw-r--r--   0        0        0     7545 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/list_members.json
+-rw-r--r--   0        0        0    11499 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/lists.json
+-rw-r--r--   0        0        0    19388 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/reports.json
+-rw-r--r--   0        0        0     5118 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/segment_members.json
+-rw-r--r--   0        0        0     2252 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/segments.json
+-rw-r--r--   0        0        0      930 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/addressMergeSegment.json
+-rw-r--r--   0        0        0     1085 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/addressZipWithinSegment.json
+-rw-r--r--   0        0        0     1054 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/aimSegment.json
+-rw-r--r--   0        0        0     1113 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/automationSegment.json
+-rw-r--r--   0        0        0      883 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/birthdayMergeSegment.json
+-rw-r--r--   0        0        0      852 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/campaignPollSegment.json
+-rw-r--r--   0        0        0      263 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/campaignStatus.json
+-rw-r--r--   0        0        0      396 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/campaignType.json
+-rw-r--r--   0        0        0     1070 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/conversationSegment.json
+-rw-r--r--   0        0        0     1021 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/countryStateSegment.json
+-rw-r--r--   0        0        0      897 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/dateMergeSegment.json
+-rw-r--r--   0        0        0     1510 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/dateSegment.json
+-rw-r--r--   0        0        0      908 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/dropdownRadioMergeSegment.json
+-rw-r--r--   0        0        0     1103 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/ecommCategorySegment.json
+-rw-r--r--   0        0        0     1283 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/ecommNumberSegment.json
+-rw-r--r--   0        0        0      741 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/ecommPurchasedSegment.json
+-rw-r--r--   0        0        0      923 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/ecommSpentSegment.json
+-rw-r--r--   0        0        0      856 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/ecommStoreSegment.json
+-rw-r--r--   0        0        0      958 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/emailClientSegment.json
+-rw-r--r--   0        0        0     1039 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/emailSegment.json
+-rw-r--r--   0        0        0      924 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/fuzzySegment.json
+-rw-r--r--   0        0        0     1455 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/geoInSegment.json
+-rw-r--r--   0        0        0      964 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/goalActivitySegment.json
+-rw-r--r--   0        0        0      971 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/goalTimestampSegment.json
+-rw-r--r--   0        0        0     1096 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/interestSegment.json
+-rw-r--r--   0        0        0     1039 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/ipGeoInZipSegment.json
+-rw-r--r--   0        0        0      856 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/languageSegment.json
+-rw-r--r--   0        0        0      939 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/memberRatingSegment.json
+-rw-r--r--   0        0        0      823 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/newSubscribers.json
+-rw-r--r--   0        0        0      874 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/predictedAgeSegment.json
+-rw-r--r--   0        0        0      862 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/predictedGenderSegment.json
+-rw-r--r--   0        0        0     2773 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/segmentCondition.json
+-rw-r--r--   0        0        0      917 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/segmentationOptions.json
+-rw-r--r--   0        0        0      840 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/signupSourceSegment.json
+-rw-r--r--   0        0        0      922 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/socialAgeSegment.json
+-rw-r--r--   0        0        0      941 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/socialGenderSegment.json
+-rw-r--r--   0        0        0      988 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/socialInfluenceSegment.json
+-rw-r--r--   0        0        0     1023 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/socialNetworkFollowSegment.json
+-rw-r--r--   0        0        0     1177 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/socialNetworkSegment.json
+-rw-r--r--   0        0        0      894 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/staticSegment.json
+-rw-r--r--   0        0        0     1083 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/surveyMonkeySegment.json
+-rw-r--r--   0        0        0     1127 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/textOrNumberMergeSegment.json
+-rw-r--r--   0        0        0      751 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/unknownSegment.json
+-rw-r--r--   0        0        0      639 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/vipSegment.json
+-rw-r--r--   0        0        0      896 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/zipSegment.json
+-rw-r--r--   0        0        0      433 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/tags.json
+-rw-r--r--   0        0        0     1456 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/unsubscribes.json
+-rw-r--r--   0        0        0      287 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/source.py
+-rw-r--r--   0        0        0     4138 2024-05-07 10:35:32.000000 airbyte_source_mailchimp-2.0.3/source_mailchimp/spec.json
+-rw-r--r--   0        0        0     5295 1970-01-01 00:00:00.000000 airbyte_source_mailchimp-2.0.3/PKG-INFO
```

### Comparing `airbyte_source_mailchimp-2.0.2/README.md` & `airbyte_source_mailchimp-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/pyproject.toml` & `airbyte_source_mailchimp-2.0.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.0.2"
+version = "2.0.3"
 name = "airbyte-source-mailchimp"
 description = "Source implementation for Mailchimp."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_mailchimp" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.85.0"
 pytest = "==6.2.5"
 
 [tool.poetry.scripts]
 source-mailchimp = "source_mailchimp.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest-mock = "^3.6.1"
```

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/components.py` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/config_migrations.py` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/manifest.yaml` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/automations.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/segment_members.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7051724137931035%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier of the segment member.'}, "*

 * *                 "'status': {'description': 'The subscription status of the segment member.'}, "*

 * *                 "'email_address': OrderedDict([('description', 'The email address of the segment "*

 * *                 "member.'), ('type', ['null', 'string'])]), 'unique_email_id': "*

 * *                 "OrderedDict([('description', 'The unique identifier related to the email "*

 * *                 "address.'), ('type', ['null',  […]*

```diff
@@ -1,351 +1,254 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": true,
     "properties": {
-        "create_time": {
-            "airbyte-type": "timestamp_with_timezone",
-            "format": "date-time",
+        "email_address": {
+            "description": "The email address of the segment member.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "emails_sent": {
+        "email_client": {
+            "description": "The client used by the segment member to access their email.",
             "type": [
                 "null",
-                "number"
+                "string"
+            ]
+        },
+        "email_type": {
+            "description": "The type of email the segment member receives.",
+            "type": [
+                "null",
+                "string"
             ]
         },
         "id": {
+            "description": "The unique identifier of the segment member.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "interests": {
+            "additionalProperties": true,
+            "description": "Interests or preferences of the segment member.",
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "ip_opt": {
+            "description": "The IP address where the segment member opted in.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "ip_signup": {
+            "description": "The IP address where the segment member signed up.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "language": {
+            "description": "The preferred language of the segment member.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "recipients": {
+        "last_changed": {
+            "airbyte_type": "timestamp_with_timezone",
+            "description": "The date and time when the segment member record was last updated.",
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "last_note": {
+            "description": "The last note added for the segment member.",
             "properties": {
-                "list_id": {
+                "created_at": {
+                    "airbyte_type": "timestamp_with_timezone",
+                    "description": "The date and time when the note was created.",
+                    "format": "date-time",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "list_is_active": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                },
-                "list_name": {
+                "created_by": {
+                    "description": "The user who created the note.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "segment_opts": {
-                    "properties": {
-                        "conditions": {
-                            "items": {
-                                "additionalProperties": true,
-                                "type": [
-                                    "null",
-                                    "object"
-                                ]
-                            },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "match": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "saved_segment_id": {
-                            "type": [
-                                "null",
-                                "number"
-                            ]
-                        }
-                    },
+                "note": {
+                    "description": "The content of the note.",
                     "type": [
                         "null",
-                        "object"
+                        "string"
                     ]
                 },
-                "store_id": {
+                "note_id": {
+                    "description": "The unique identifier of the note.",
                     "type": [
                         "null",
-                        "string"
+                        "integer"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "report_summary": {
+        "list_id": {
+            "description": "The identifier of the list to which the segment member belongs.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "location": {
+            "description": "Geographical location information of the segment member.",
             "properties": {
-                "click_rate": {
+                "country_code": {
+                    "description": "The country code of the location.",
                     "type": [
                         "null",
-                        "number"
+                        "string"
                     ]
                 },
-                "clicks": {
+                "dstoff": {
+                    "description": "The Daylight Saving Time offset of the location.",
                     "type": [
                         "null",
-                        "number"
+                        "integer"
                     ]
                 },
-                "open_rate": {
+                "gmtoff": {
+                    "description": "The GMT offset of the location.",
                     "type": [
                         "null",
-                        "number"
+                        "integer"
                     ]
                 },
-                "opens": {
+                "latitude": {
+                    "description": "The latitude coordinate of the location.",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
-                "subscriber_clicks": {
+                "longitude": {
+                    "description": "The longitude coordinate of the location.",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
-                "unique_opens": {
+                "timezone": {
+                    "description": "The timezone of the location.",
                     "type": [
                         "null",
-                        "number"
+                        "string"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "settings": {
+        "member_rating": {
+            "description": "The rating assigned to the segment member.",
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "merge_fields": {
+            "additionalProperties": true,
+            "description": "Additional information merged with the segment member data.",
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "segment_id": {
+            "description": "The identifier of the segment the member belongs to.",
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "stats": {
+            "description": "Statistics related to the email engagement of the segment member.",
             "properties": {
-                "authenticate": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                },
-                "auto_footer": {
+                "avg_click_rate": {
+                    "description": "The average click-through rate of the segment member.",
                     "type": [
                         "null",
-                        "boolean"
-                    ]
-                },
-                "from_name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "inline_css": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                },
-                "reply_to": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "title": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "to_name": {
-                    "type": [
-                        "null",
-                        "string"
+                        "number"
                     ]
                 },
-                "use_conversation": {
+                "avg_open_rate": {
+                    "description": "The average open rate of the segment member.",
                     "type": [
                         "null",
-                        "boolean"
+                        "number"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "start_time": {
+        "status": {
+            "description": "The subscription status of the segment member.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "timestamp_opt": {
             "airbyte_type": "timestamp_with_timezone",
+            "description": "The date and time when the segment member opted in.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "status": {
+        "timestamp_signup": {
+            "airbyte_type": "timestamp_with_timezone",
+            "description": "The date and time when the segment member signed up.",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tracking": {
-            "properties": {
-                "capsule": {
-                    "properties": {
-                        "notes": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "clicktale": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "ecomm360": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                },
-                "goal_tracking": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                },
-                "google_analytics": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "html_clicks": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                },
-                "opens": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                },
-                "salesforce": {
-                    "properties": {
-                        "campaign": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        },
-                        "notes": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "text_clicks": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                }
-            },
+        "unique_email_id": {
+            "description": "The unique identifier related to the email address.",
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "trigger_settings": {
-            "properties": {
-                "runtime": {
-                    "properties": {
-                        "days": {
-                            "items": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "hours": {
-                            "properties": {
-                                "type": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "workflow_emails_count": {
-                    "type": [
-                        "null",
-                        "number"
-                    ]
-                },
-                "workflow_title": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "workflow_type": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "vip": {
+            "description": "Flag indicating if the segment member is a VIP.",
             "type": [
                 "null",
-                "object"
+                "boolean"
             ]
         }
     },
-    "title": "Automations",
     "type": "object"
 }
```

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/campaigns.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/campaigns.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971590909090909%*

 * *Differences: {"'properties'": '{\'type\': {\'description\': "The type of campaign (e.g., \'regular\', '*

 * *                 '\'automated\', \'plain-text\')"}, \'status\': {\'description\': "The current '*

 * *                 'status of the campaign (e.g., \'sent\', \'draft\', \'scheduled\')"}}'}*

```diff
@@ -656,15 +656,16 @@
                     ]
                 }
             },
             "title": "Campaign Social Card",
             "type": "object"
         },
         "status": {
-            "$ref": "campaignStatus.json"
+            "$ref": "campaignStatus.json",
+            "description": "The current status of the campaign (e.g., 'sent', 'draft', 'scheduled')"
         },
         "tracking": {
             "description": "The tracking options for a campaign.",
             "properties": {
                 "capsule": {
                     "description": "Capsule tracking options for a campaign. Must be using Mailchimp's built-in Capsule integration.",
                     "properties": {
@@ -736,15 +737,16 @@
                     "type": "boolean"
                 }
             },
             "title": "Campaign Tracking Options",
             "type": "object"
         },
         "type": {
-            "$ref": "campaignType.json"
+            "$ref": "campaignType.json",
+            "description": "The type of campaign (e.g., 'regular', 'automated', 'plain-text')"
         },
         "variate_settings": {
             "description": "The settings specific to A/B test campaigns.",
             "properties": {
                 "combinations": {
                     "description": "Combinations of possible variables used to build emails.",
                     "items": {
```

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/email_activity.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/email_activity.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,83 +1,83 @@
 {
     "type": "object",
     "title": "Email Activity",
     "description": "A list of member's subscriber activity in a specific campaign.",
     "properties": {
         "campaign_id": {
+            "description": "The unique id for the campaign.",
             "type": "string",
-            "title": "The unique id for the campaign.",
-            "description": "The unique id for the campaign."
+            "title": "The unique id for the campaign."
         },
         "list_id": {
+            "description": "The unique id for the list.",
             "type": "string",
-            "title": "The unique id for the list.",
-            "description": "The unique id for the list."
+            "title": "The unique id for the list."
         },
         "list_is_active": {
+            "description": "The status of the list used, namely if it's deleted or disabled.",
             "type": "boolean",
-            "title": "The status of the list used.",
-            "description": "The status of the list used, namely if it's deleted or disabled."
+            "title": "The status of the list used."
         },
         "email_id": {
+            "description": "The MD5 hash of the lowercase version of the list member's email address.",
             "type": "string",
-            "title": "email MD5 hash.",
-            "description": "The MD5 hash of the lowercase version of the list member's email address."
+            "title": "email MD5 hash."
         },
         "email_address": {
+            "description": "Email address for a subscriber.",
             "type": "string",
-            "title": "Email address for a subscriber.",
-            "description": "Email address for a subscriber."
+            "title": "Email address for a subscriber."
         },
         "action": {
+            "description": "One of the following actions: 'open', 'click', or 'bounce'",
             "type": [
                 "string",
                 "null"
             ],
             "title": "action",
             "enum": [
                 "open",
                 "click",
                 "bounce"
-            ],
-            "description": "One of the following actions: 'open', 'click', or 'bounce'"
+            ]
         },
         "type": {
+            "description": "If the action is a 'bounce', the type of bounce received: 'hard', 'soft'.",
             "type": [
                 "string",
                 "null"
             ],
             "title": "Type",
             "enum": [
                 "hard",
                 "soft"
-            ],
-            "description": "If the action is a 'bounce', the type of bounce received: 'hard', 'soft'."
+            ]
         },
         "timestamp": {
+            "description": "The date and time recorded for the action in ISO 8601 format.",
             "type": [
                 "string",
                 "null"
             ],
             "title": "Action date and time",
-            "description": "The date and time recorded for the action in ISO 8601 format.",
             "format": "date-time",
             "airbyte_type": "timestamp_with_timezone"
         },
         "url": {
+            "description": "If the action is a 'click', the URL on which the member clicked.",
             "type": [
                 "string",
                 "null"
             ],
-            "title": "Click url",
-            "description": "If the action is a 'click', the URL on which the member clicked."
+            "title": "Click url"
         },
         "ip": {
+            "description": "The IP address recorded for the action.",
             "type": [
                 "string",
                 "null"
             ],
-            "title": "Action ip address",
-            "description": "The IP address recorded for the action."
+            "title": "Action ip address"
         }
     }
 }
```

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/lists.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/lists.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9957225012400794%*

 * *Differences: {"'properties'": "{'contact': {'description': 'Contact information displayed in campaign footers "*

 * *                 "to comply with international spam laws.', 'properties': {'address2': "*

 * *                 "{'description': 'The street address line 2 for the list contact.'}}}, "*

 * *                 "'permission_reminder': {'description': 'The permission reminder for the list.'}, "*

 * *                 "'use_archive_bar': {'description': 'Whether campaigns for this list use the "*

 * *                 "Archive Bar in arch […]*

```diff
@@ -1,21 +1,21 @@
 {
     "description": "Information about a specific list.",
     "properties": {
         "beamer_address": {
-            "description": "The list's [Email Beamer](https://mailchimp.com/help/use-email-beamer-to-create-a-campaign/) address.",
+            "description": "The list's Email Beamer address.",
             "readOnly": true,
             "title": "Beamer Address",
             "type": [
                 "null",
                 "string"
             ]
         },
         "campaign_defaults": {
-            "description": "[Default values for campaigns](https://mailchimp.com/help/edit-your-emails-subject-preview-text-from-name-or-from-email-address/) created for this list.",
+            "description": "Default values for campaigns created for this list.",
             "properties": {
                 "from_email": {
                     "description": "The default from email for campaigns sent to this list.",
                     "title": "Sender's Email Address",
                     "type": [
                         "null",
                         "string"
@@ -26,15 +26,15 @@
                     "title": "Sender's Name",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "language": {
-                    "description": "The default language for this lists's forms.",
+                    "description": "The default language for this list's forms.",
                     "title": "Language",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "subject": {
@@ -46,26 +46,26 @@
                     ]
                 }
             },
             "title": "Campaign Defaults",
             "type": "object"
         },
         "contact": {
-            "description": "[Contact information displayed in campaign footers](https://mailchimp.com/help/about-campaign-footers/) to comply with international spam laws.",
+            "description": "Contact information displayed in campaign footers to comply with international spam laws.",
             "properties": {
                 "address1": {
                     "description": "The street address for the list contact.",
                     "title": "Address",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "address2": {
-                    "description": "The street address for the list contact.",
+                    "description": "The street address line 2 for the list contact.",
                     "title": "Address",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "city": {
@@ -131,21 +131,21 @@
         "double_optin": {
             "default": false,
             "description": "Whether or not to require the subscriber to confirm subscription via email.",
             "title": "Double Opt In",
             "type": "boolean"
         },
         "email_type_option": {
-            "description": "Whether the list supports [multiple formats for emails](https://mailchimp.com/help/change-list-name-and-defaults/). When set to `true`, subscribers can choose whether they want to receive HTML or plain-text emails. When set to `false`, subscribers will receive HTML emails, with a plain-text alternative backup.",
+            "description": "Whether the list supports multiple formats for emails. When set to `true`, subscribers can choose whether they want to receive HTML or plain-text emails. When set to `false`, subscribers will receive HTML emails, with a plain-text alternative backup.",
             "title": "Email Type Option",
             "type": "boolean"
         },
         "has_welcome": {
             "default": false,
-            "description": "Whether or not this list has a welcome automation connected. Welcome Automations: welcomeSeries, singleWelcome, emailFollowup.",
+            "description": "Whether or not this list has a welcome automation connected.",
             "example": false,
             "title": "Has Welcome",
             "type": "boolean"
         },
         "id": {
             "description": "A string that uniquely identifies this list.",
             "readOnly": true,
@@ -182,32 +182,32 @@
             "type": [
                 "null",
                 "string"
             ]
         },
         "notify_on_subscribe": {
             "default": false,
-            "description": "The email address to send [subscribe notifications](https://mailchimp.com/help/change-subscribe-and-unsubscribe-notifications/) to.",
+            "description": "The email address to send subscribe notifications to.",
             "title": "Notify on Subscribe",
             "type": [
                 "null",
                 "string"
             ]
         },
         "notify_on_unsubscribe": {
             "default": false,
-            "description": "The email address to send [unsubscribe notifications](https://mailchimp.com/help/change-subscribe-and-unsubscribe-notifications/) to.",
+            "description": "The email address to send unsubscribe notifications to.",
             "title": "Notify on Unsubscribe",
             "type": [
                 "null",
                 "string"
             ]
         },
         "permission_reminder": {
-            "description": "The [permission reminder](https://mailchimp.com/help/edit-the-permission-reminder/) for the list.",
+            "description": "The permission reminder for the list.",
             "title": "Permission Reminder",
             "type": [
                 "null",
                 "string"
             ]
         },
         "stats": {
@@ -341,30 +341,30 @@
             "title": "Subscribe URL Long",
             "type": [
                 "null",
                 "string"
             ]
         },
         "subscribe_url_short": {
-            "description": "Our [EepURL shortened](https://mailchimp.com/help/share-your-signup-form/) version of this list's subscribe form.",
+            "description": "Our EepURL shortened version of this list's subscribe form.",
             "readOnly": true,
             "title": "Subscribe URL Short",
             "type": [
                 "null",
                 "string"
             ]
         },
         "use_archive_bar": {
             "default": false,
-            "description": "Whether campaigns for this list use the [Archive Bar](https://mailchimp.com/help/about-email-campaign-archives-and-pages/) in archives by default.",
+            "description": "Whether campaigns for this list use the Archive Bar in archives by default.",
             "title": "Use Archive Bar",
             "type": "boolean"
         },
         "visibility": {
-            "description": "Whether this list is [public or private](https://mailchimp.com/help/about-list-publicity/).",
+            "description": "Whether this list is public or private.",
             "enum": [
                 "pub",
                 "prv"
             ],
             "title": "Visibility",
             "type": [
                 "null",
```

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/reports.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/reports.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996912247095353%*

 * *Differences: {"'properties'": "{'timewarp': {'items': {'properties': {'gmt_offset': {'description': 'For "*

 * *                 "campaigns sent with timewarp, the time zone group the member is part of.'}}}}, "*

 * *                 "'share_report': {'description': 'The url and password for the VIP report.'}, "*

 * *                 "'ecommerce': {'properties': {'currency_code': {'description': 'The currency code "*

 * *                 "used for the campaign.'}}}}"}*

```diff
@@ -241,14 +241,15 @@
             "title": "Campaign Delivery Status",
             "type": "object"
         },
         "ecommerce": {
             "description": "E-Commerce stats for a campaign.",
             "properties": {
                 "currency_code": {
+                    "description": "The currency code used for the campaign.",
                     "example": "USD",
                     "readOnly": true,
                     "title": "Three letter currency code for this user",
                     "type": [
                         "null",
                         "string"
                     ]
@@ -480,15 +481,15 @@
             "title": "Send Time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "share_report": {
-            "description": "The url and password for the [VIP report](https://mailchimp.com/help/share-a-campaign-report/).",
+            "description": "The url and password for the VIP report.",
             "properties": {
                 "share_password": {
                     "description": "If password protected, the password for the VIP report.",
                     "readOnly": true,
                     "title": "Report Password",
                     "type": [
                         "null",
@@ -563,15 +564,15 @@
                     },
                     "clicks": {
                         "description": "The number of clicks.",
                         "title": "Clicks",
                         "type": "integer"
                     },
                     "gmt_offset": {
-                        "description": "For campaigns sent with timewarp, the time zone group the member is apart of.",
+                        "description": "For campaigns sent with timewarp, the time zone group the member is part of.",
                         "title": "GMT Offset",
                         "type": "integer"
                     },
                     "last_click": {
                         "airbyte_type": "timestamp_with_timezone",
                         "description": "The date and time of the last click in ISO 8601 format.",
                         "format": "date-time",
```

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/segment_members.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/segments.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8815586419753086%*

 * *Differences: {"'properties'": "{'id': {'type': {insert: [(1, 'integer')], delete: [1]}, 'description': 'Unique "*

 * *                 "identifier for the segment'}, 'list_id': {'description': 'ID of the list to "*

 * *                 "which the segment belongs'}, 'name': OrderedDict([('description', 'Name of the "*

 * *                 "segment'), ('type', ['null', 'string'])]), 'member_count': "*

 * *                 "OrderedDict([('description', 'Total number of members in the segment'), ('type', "*

 * *                 "['null', 'integer'] […]*

```diff
@@ -1,221 +1,114 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": true,
     "properties": {
-        "email_address": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "email_client": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "email_type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "interests": {
-            "additionalProperties": true,
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "ip_opt": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "ip_signup": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "language": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "last_changed": {
+        "created_at": {
             "airbyte_type": "timestamp_with_timezone",
+            "description": "The date and time when the segment was created",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "last_note": {
-            "properties": {
-                "created_at": {
-                    "airbyte_type": "timestamp_with_timezone",
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "created_by": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "note": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "note_id": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                }
-            },
+        "id": {
+            "description": "Unique identifier for the segment",
             "type": [
                 "null",
-                "object"
+                "integer"
             ]
         },
         "list_id": {
+            "description": "ID of the list to which the segment belongs",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "location": {
-            "properties": {
-                "country_code": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "dstoff": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "gmtoff": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "latitude": {
-                    "type": [
-                        "null",
-                        "number"
-                    ]
-                },
-                "longitude": {
-                    "type": [
-                        "null",
-                        "number"
-                    ]
-                },
-                "timezone": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "member_rating": {
+        "member_count": {
+            "description": "Total number of members in the segment",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "merge_fields": {
-            "additionalProperties": true,
+        "name": {
+            "description": "Name of the segment",
             "type": [
                 "null",
-                "object"
-            ]
-        },
-        "segment_id": {
-            "type": [
-                "null",
-                "integer"
+                "string"
             ]
         },
-        "stats": {
+        "options": {
+            "description": "The available options for segment data",
             "properties": {
-                "avg_click_rate": {
+                "conditions": {
+                    "description": "Conditions set for segment filtering",
+                    "items": {
+                        "additionalProperties": true,
+                        "description": "Specific conditions to filter segments",
+                        "properties": {
+                            "condition_type": {
+                                "description": "Type of condition applied",
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "field": {
+                                "description": "Field to which the condition is applied",
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "op": {
+                                "description": "Operator used in the condition",
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
                     "type": [
                         "null",
-                        "number"
+                        "array"
                     ]
                 },
-                "avg_open_rate": {
+                "match": {
+                    "description": "Type of match applied for multiple conditions (all, any)",
                     "type": [
                         "null",
-                        "number"
+                        "string"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "status": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "timestamp_opt": {
-            "airbyte_type": "timestamp_with_timezone",
-            "format": "date-time",
+        "type": {
+            "description": "Type of segment (static, dynamic)",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "timestamp_signup": {
+        "updated_at": {
             "airbyte_type": "timestamp_with_timezone",
+            "description": "The date and time when the segment was last updated",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "unique_email_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "vip": {
-            "type": [
-                "null",
-                "boolean"
-            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/addressMergeSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/addressMergeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/addressZipWithinSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/addressZipWithinSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/aimSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/aimSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/automationSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/automationSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/birthdayMergeSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/birthdayMergeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/campaignPollSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/campaignPollSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/conversationSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/conversationSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/countryStateSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/countryStateSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/dateMergeSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/dateMergeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/dateSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/dateSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/dropdownRadioMergeSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/dropdownRadioMergeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/ecommCategorySegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/ecommCategorySegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/ecommNumberSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/ecommNumberSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/ecommPurchasedSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/ecommPurchasedSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/ecommSpentSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/ecommSpentSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/ecommStoreSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/ecommStoreSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/emailClientSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/emailClientSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/emailSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/emailSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/fuzzySegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/fuzzySegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/geoInSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/geoInSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/goalActivitySegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/goalActivitySegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/goalTimestampSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/goalTimestampSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/interestSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/interestSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/ipGeoInZipSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/ipGeoInZipSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/languageSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/languageSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/memberRatingSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/memberRatingSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/newSubscribers.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/newSubscribers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/predictedAgeSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/predictedAgeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/predictedGenderSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/predictedGenderSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/segmentCondition.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/segmentCondition.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/segmentationOptions.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/segmentationOptions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/signupSourceSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/signupSourceSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/socialAgeSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/socialAgeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/socialGenderSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/socialGenderSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/socialInfluenceSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/socialInfluenceSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/socialNetworkFollowSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/socialNetworkFollowSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/socialNetworkSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/socialNetworkSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/staticSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/staticSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/surveyMonkeySegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/surveyMonkeySegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/textOrNumberMergeSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/textOrNumberMergeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/unknownSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/unknownSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/vipSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/vipSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/shared/zipSegment.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/shared/zipSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/schemas/unsubscribes.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/schemas/interest_categories.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6322115384615384%*

 * *Differences: {"'properties'": "{'list_id': {'description': 'The ID of the list to which this interest category "*

 * *                 "belongs.'}, 'id': OrderedDict([('description', 'The unique identifier for the "*

 * *                 "interest category.'), ('type', ['null', 'string'])]), 'title': "*

 * *                 "OrderedDict([('description', 'The title or name of the interest category.'), "*

 * *                 "('type', ['null', 'string'])]), 'display_order': OrderedDict([('description', "*

 * *                 "'The order in whic […]*

```diff
@@ -1,64 +1,41 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "additionalProperties": true,
     "properties": {
-        "campaign_id": {
+        "display_order": {
+            "description": "The order in which this interest category should be displayed in the UI.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "email_address": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "email_id": {
+        "id": {
+            "description": "The unique identifier for the interest category.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "list_id": {
+            "description": "The ID of the list to which this interest category belongs.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "list_is_active": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "merge_fields": {
-            "additionalProperties": true,
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "reason": {
+        "title": {
+            "description": "The title or name of the interest category.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "timestamp": {
-            "airbyte_type": "timestamp_with_timezone",
-            "format": "date-time",
+        "type": {
+            "description": "The type of interest category, e.g., 'checkboxes', 'hidden', 'dropdown'.",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "vip": {
-            "type": [
-                "null",
-                "boolean"
-            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_mailchimp-2.0.2/source_mailchimp/spec.json` & `airbyte_source_mailchimp-2.0.3/source_mailchimp/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-2.0.2/PKG-INFO` & `airbyte_source_mailchimp-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-mailchimp
-Version: 2.0.2
+Version: 2.0.3
 Summary: Source implementation for Mailchimp.
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
+Requires-Dist: airbyte-cdk (==0.85.0)
 Requires-Dist: pytest (==6.2.5)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/mailchimp
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Mailchimp source connector
```

