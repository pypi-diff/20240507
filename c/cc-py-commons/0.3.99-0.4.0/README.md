# Comparing `tmp/cc_py_commons-0.3.99.tar.gz` & `tmp/cc_py_commons-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cc_py_commons-0.3.99.tar", last modified: Sun May  5 20:37:57 2024, max compression
+gzip compressed data, was "dist/cc_py_commons-0.4.0.tar", last modified: Mon May  6 23:40:54 2024, max compression
```

## Comparing `cc_py_commons-0.3.99.tar` & `cc_py_commons-0.4.0.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/
--rw-r--r--   0 kirk       (501) staff       (20)      266 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/PKG-INFO
--rw-r--r--   0 kirk       (501) staff       (20)     1118 2021-04-14 01:41:32.000000 cc_py_commons-0.3.99/README.md
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2021-05-07 00:00:50.000000 cc_py_commons-0.3.99/cc_py_commons/__init__.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/bids/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/bids/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      802 2024-04-09 00:53:10.000000 cc_py_commons-0.3.99/cc_py_commons/bids/bid.py
--rw-r--r--   0 kirk       (501) staff       (20)      300 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/bids/bid_history.py
--rw-r--r--   0 kirk       (501) staff       (20)      471 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/bids/bid_history_schema.py
--rw-r--r--   0 kirk       (501) staff       (20)     1332 2024-04-09 00:53:10.000000 cc_py_commons-0.3.99/cc_py_commons/bids/bid_schema.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/carriers/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2021-04-14 01:41:32.000000 cc_py_commons-0.3.99/cc_py_commons/carriers/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      233 2023-07-27 21:32:34.000000 cc_py_commons-0.3.99/cc_py_commons/carriers/account_carrier_map.py
--rw-r--r--   0 kirk       (501) staff       (20)      687 2023-02-02 05:49:27.000000 cc_py_commons-0.3.99/cc_py_commons/carriers/account_carrier_map_schema.py
--rw-r--r--   0 kirk       (501) staff       (20)     3383 2024-05-05 05:28:58.000000 cc_py_commons-0.3.99/cc_py_commons/carriers/carrier.py
--rw-r--r--   0 kirk       (501) staff       (20)     3093 2024-05-05 05:28:58.000000 cc_py_commons-0.3.99/cc_py_commons/carriers/carrier_schema.py
--rw-r--r--   0 kirk       (501) staff       (20)      429 2024-04-09 00:53:10.000000 cc_py_commons-0.3.99/cc_py_commons/carriers/contact.py
--rw-r--r--   0 kirk       (501) staff       (20)      787 2024-04-09 00:53:10.000000 cc_py_commons-0.3.99/cc_py_commons/carriers/contact_schema.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/config/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2020-08-11 23:45:04.000000 cc_py_commons-0.3.99/cc_py_commons/config/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)     6364 2024-04-09 00:53:10.000000 cc_py_commons-0.3.99/cc_py_commons/config/env.py
--rw-r--r--   0 kirk       (501) staff       (20)     1364 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/config/mcleod_load_fields.py
--rw-r--r--   0 kirk       (501) staff       (20)     1455 2020-08-11 23:45:04.000000 cc_py_commons-0.3.99/cc_py_commons/config/pc_miler_config.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/db/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2023-01-07 20:27:47.000000 cc_py_commons-0.3.99/cc_py_commons/db/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      566 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/db/connection.py
--rw-r--r--   0 kirk       (501) staff       (20)    13659 2024-05-05 07:32:52.000000 cc_py_commons-0.3.99/cc_py_commons/geolocate.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/lanes/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/lanes/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      972 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/lanes/carrier_lane.py
--rw-r--r--   0 kirk       (501) staff       (20)     1251 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/lanes/carrier_lane_schema.py
--rw-r--r--   0 kirk       (501) staff       (20)      663 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/lanes/lane.py
--rw-r--r--   0 kirk       (501) staff       (20)      941 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/lanes/lane_schema.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/loads/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/loads/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      154 2022-09-25 19:11:30.000000 cc_py_commons-0.3.99/cc_py_commons/loads/equipment.py
--rw-r--r--   0 kirk       (501) staff       (20)      384 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/loads/equipment_schema.py
--rw-r--r--   0 kirk       (501) staff       (20)      965 2023-09-07 00:25:21.000000 cc_py_commons-0.3.99/cc_py_commons/loads/equipment_types.py
--rw-r--r--   0 kirk       (501) staff       (20)      338 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/loads/freighthub_contact.py
--rw-r--r--   0 kirk       (501) staff       (20)      442 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/loads/freighthub_contact_schema.py
--rw-r--r--   0 kirk       (501) staff       (20)     3350 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/loads/load.py
--rw-r--r--   0 kirk       (501) staff       (20)     4000 2023-09-07 00:25:21.000000 cc_py_commons-0.3.99/cc_py_commons/loads/load_schema.py
--rw-r--r--   0 kirk       (501) staff       (20)      501 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/loads/load_status.py
--rw-r--r--   0 kirk       (501) staff       (20)      286 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/loads/location.py
--rw-r--r--   0 kirk       (501) staff       (20)      463 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/loads/location_schema.py
--rw-r--r--   0 kirk       (501) staff       (20)      751 2023-01-07 20:27:47.000000 cc_py_commons-0.3.99/cc_py_commons/loads/map_load_response.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/quotes/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/quotes/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)     1967 2023-07-13 01:51:13.000000 cc_py_commons-0.3.99/cc_py_commons/quotes/quote.py
--rw-r--r--   0 kirk       (501) staff       (20)     2638 2023-07-13 01:51:13.000000 cc_py_commons-0.3.99/cc_py_commons/quotes/quote_schema.py
--rw-r--r--   0 kirk       (501) staff       (20)      501 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/quotes/quote_status.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/rfp/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2023-01-07 20:27:47.000000 cc_py_commons-0.3.99/cc_py_commons/rfp/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      145 2023-01-07 20:27:47.000000 cc_py_commons-0.3.99/cc_py_commons/rfp/rfp_status.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/schemas/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2021-04-14 01:41:32.000000 cc_py_commons-0.3.99/cc_py_commons/schemas/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      439 2021-04-14 01:41:32.000000 cc_py_commons-0.3.99/cc_py_commons/schemas/camel_case_schema.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/services/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2022-07-22 01:21:18.000000 cc_py_commons-0.3.99/cc_py_commons/services/__init__.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2023-07-13 01:51:13.000000 cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      653 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/accept_bid.py
--rw-r--r--   0 kirk       (501) staff       (20)      746 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/cancel_bid.py
--rw-r--r--   0 kirk       (501) staff       (20)      671 2023-07-13 01:51:13.000000 cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/constants.py
--rw-r--r--   0 kirk       (501) staff       (20)      704 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/counter_bid.py
--rw-r--r--   0 kirk       (501) staff       (20)      702 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/decline_bid.py
--rw-r--r--   0 kirk       (501) staff       (20)      648 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/get_bid_by_amazon_order_id.py
--rw-r--r--   0 kirk       (501) staff       (20)      943 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/get_quote.py
--rw-r--r--   0 kirk       (501) staff       (20)      674 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/update_bid.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/services/c4/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2022-07-22 01:21:18.000000 cc_py_commons-0.3.99/cc_py_commons/services/c4/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      491 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/c4/amazon_session_token.py
--rw-r--r--   0 kirk       (501) staff       (20)      147 2023-07-13 01:51:13.000000 cc_py_commons-0.3.99/cc_py_commons/services/c4/constants.py
--rw-r--r--   0 kirk       (501) staff       (20)      922 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/c4/get_integration.py
--rw-r--r--   0 kirk       (501) staff       (20)      681 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/c4/get_users_for_account.py
--rw-r--r--   0 kirk       (501) staff       (20)      660 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/c4/refresh_amazon_token.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/services/carrier_hub/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2023-08-22 21:56:55.000000 cc_py_commons-0.3.99/cc_py_commons/services/carrier_hub/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      673 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/carrier_hub/get_carrier.py
--rw-r--r--   0 kirk       (501) staff       (20)     1016 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/carrier_hub/list_carriers.py
--rw-r--r--   0 kirk       (501) staff       (20)     1413 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/carrier_hub/list_contacts.py
--rw-r--r--   0 kirk       (501) staff       (20)      724 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/carrier_hub/update_contact.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/services/freight_hub/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2022-07-22 01:21:18.000000 cc_py_commons-0.3.99/cc_py_commons/services/freight_hub/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      477 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/freight_hub/post_freight_hub_load.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/services/mercury/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2022-11-08 05:26:59.000000 cc_py_commons-0.3.99/cc_py_commons/services/mercury/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      571 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/mercury/get_green_screens_lane_price.py
--rw-r--r--   0 kirk       (501) staff       (20)      553 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/mercury/get_lane_price.py
--rw-r--r--   0 kirk       (501) staff       (20)      563 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/mercury/get_lane_price_for_bulk.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/services/slack/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2023-09-15 20:36:29.000000 cc_py_commons-0.3.99/cc_py_commons/services/slack/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)     1044 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/services/slack/send_slack_message.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/sns/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2021-04-14 01:41:32.000000 cc_py_commons-0.3.99/cc_py_commons/sns/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      932 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/sns/book_load_notification.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/sns/booking_agent/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2023-07-13 01:51:13.000000 cc_py_commons-0.3.99/cc_py_commons/sns/booking_agent/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      971 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/sns/booking_agent/bid_counter_failure_notification.py
--rw-r--r--   0 kirk       (501) staff       (20)       77 2023-07-13 01:51:13.000000 cc_py_commons-0.3.99/cc_py_commons/sns/booking_agent/constants.py
--rw-r--r--   0 kirk       (501) staff       (20)      747 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/sns/booking_agent/send_sns_notification.py
--rw-r--r--   0 kirk       (501) staff       (20)      987 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/sns/booking_assistant_flow_notification.py
--rw-r--r--   0 kirk       (501) staff       (20)      751 2021-06-09 01:06:31.000000 cc_py_commons-0.3.99/cc_py_commons/sns/import_movements_notification.py
--rw-r--r--   0 kirk       (501) staff       (20)      901 2024-04-30 23:06:40.000000 cc_py_commons-0.3.99/cc_py_commons/sns/parsed_carrier_notification.py
--rw-r--r--   0 kirk       (501) staff       (20)      269 2021-04-14 01:41:32.000000 cc_py_commons-0.3.99/cc_py_commons/sns/sns_service.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/sqs/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2022-09-16 05:49:21.000000 cc_py_commons-0.3.99/cc_py_commons/sqs/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)     1152 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/sqs/booking_assistant_flow_event.py
--rw-r--r--   0 kirk       (501) staff       (20)      440 2022-09-16 05:49:21.000000 cc_py_commons-0.3.99/cc_py_commons/sqs/sqs_service.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/tests/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2021-11-16 01:32:23.000000 cc_py_commons-0.3.99/cc_py_commons/tests/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      844 2021-12-22 05:36:02.000000 cc_py_commons-0.3.99/cc_py_commons/tests/test_case_conversion.py
--rw-r--r--   0 kirk       (501) staff       (20)      760 2023-03-29 19:12:55.000000 cc_py_commons-0.3.99/cc_py_commons/tests/test_lambda_utils.py
--rw-r--r--   0 kirk       (501) staff       (20)     2036 2023-09-07 00:25:21.000000 cc_py_commons-0.3.99/cc_py_commons/tests/test_map_transaction.py
--rw-r--r--   0 kirk       (501) staff       (20)      475 2022-05-25 05:49:37.000000 cc_py_commons-0.3.99/cc_py_commons/tests/test_temperature_utils.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/transactions/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2021-11-16 01:32:23.000000 cc_py_commons-0.3.99/cc_py_commons/transactions/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)      442 2021-11-16 01:32:23.000000 cc_py_commons-0.3.99/cc_py_commons/transactions/equipment_clas_schema.py
--rw-r--r--   0 kirk       (501) staff       (20)      213 2021-11-16 01:32:23.000000 cc_py_commons-0.3.99/cc_py_commons/transactions/equipment_class.py
--rw-r--r--   0 kirk       (501) staff       (20)      289 2021-11-16 01:32:23.000000 cc_py_commons-0.3.99/cc_py_commons/transactions/equipment_mapping.py
--rw-r--r--   0 kirk       (501) staff       (20)      540 2021-11-16 01:32:23.000000 cc_py_commons-0.3.99/cc_py_commons/transactions/equipment_mapping_schema.py
--rw-r--r--   0 kirk       (501) staff       (20)     3181 2024-04-09 00:53:10.000000 cc_py_commons-0.3.99/cc_py_commons/transactions/map_transaction.py
--rw-r--r--   0 kirk       (501) staff       (20)     4931 2023-09-07 00:25:21.000000 cc_py_commons-0.3.99/cc_py_commons/transactions/transaction.py
--rw-r--r--   0 kirk       (501) staff       (20)     5159 2023-10-26 00:50:00.000000 cc_py_commons-0.3.99/cc_py_commons/transactions/transaction_schema.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons/utils/
--rw-r--r--   0 kirk       (501) staff       (20)        0 2020-08-11 23:45:04.000000 cc_py_commons-0.3.99/cc_py_commons/utils/__init__.py
--rw-r--r--   0 kirk       (501) staff       (20)     1519 2022-07-22 01:21:18.000000 cc_py_commons-0.3.99/cc_py_commons/utils/case_conversion.py
--rw-r--r--   0 kirk       (501) staff       (20)     1168 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/utils/datadog_logger.py
--rw-r--r--   0 kirk       (501) staff       (20)      759 2023-01-07 20:27:47.000000 cc_py_commons-0.3.99/cc_py_commons/utils/datetimes.py
--rw-r--r--   0 kirk       (501) staff       (20)      723 2023-08-22 21:56:55.000000 cc_py_commons-0.3.99/cc_py_commons/utils/dimension_utils.py
--rw-r--r--   0 kirk       (501) staff       (20)      513 2024-04-09 00:53:10.000000 cc_py_commons-0.3.99/cc_py_commons/utils/get_delivery_date.py
--rw-r--r--   0 kirk       (501) staff       (20)      893 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/utils/json_logger.py
--rw-r--r--   0 kirk       (501) staff       (20)      219 2023-03-29 19:12:55.000000 cc_py_commons-0.3.99/cc_py_commons/utils/lambda_utils.py
--rw-r--r--   0 kirk       (501) staff       (20)     1051 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/utils/local_file.py
--rw-r--r--   0 kirk       (501) staff       (20)      998 2023-10-26 00:50:00.000000 cc_py_commons-0.3.99/cc_py_commons/utils/logger.py
--rw-r--r--   0 kirk       (501) staff       (20)     2026 2024-04-09 00:53:10.000000 cc_py_commons-0.3.99/cc_py_commons/utils/logger_v2.py
--rw-r--r--   0 kirk       (501) staff       (20)     2792 2020-08-11 23:45:04.000000 cc_py_commons-0.3.99/cc_py_commons/utils/pc_miler_utils.py
--rw-r--r--   0 kirk       (501) staff       (20)     1237 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/utils/price_utils.py
--rw-r--r--   0 kirk       (501) staff       (20)     1044 2020-08-11 23:45:04.000000 cc_py_commons-0.3.99/cc_py_commons/utils/redis.py
--rw-r--r--   0 kirk       (501) staff       (20)     2367 2024-02-08 21:28:28.000000 cc_py_commons-0.3.99/cc_py_commons/utils/s3_file.py
--rw-r--r--   0 kirk       (501) staff       (20)      353 2023-08-22 21:56:55.000000 cc_py_commons-0.3.99/cc_py_commons/utils/temperature_utils.py
-drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons.egg-info/
--rw-r--r--   0 kirk       (501) staff       (20)      266 2024-05-05 20:37:56.000000 cc_py_commons-0.3.99/cc_py_commons.egg-info/PKG-INFO
--rw-r--r--   0 kirk       (501) staff       (20)     4989 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/cc_py_commons.egg-info/SOURCES.txt
--rw-r--r--   0 kirk       (501) staff       (20)        1 2024-05-05 20:37:56.000000 cc_py_commons-0.3.99/cc_py_commons.egg-info/dependency_links.txt
--rw-r--r--   0 kirk       (501) staff       (20)       66 2024-05-05 20:37:56.000000 cc_py_commons-0.3.99/cc_py_commons.egg-info/requires.txt
--rw-r--r--   0 kirk       (501) staff       (20)       14 2024-05-05 20:37:56.000000 cc_py_commons-0.3.99/cc_py_commons.egg-info/top_level.txt
--rw-r--r--   0 kirk       (501) staff       (20)       38 2024-05-05 20:37:57.000000 cc_py_commons-0.3.99/setup.cfg
--rw-r--r--   0 kirk       (501) staff       (20)      436 2024-05-05 07:32:56.000000 cc_py_commons-0.3.99/setup.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/
+-rw-r--r--   0 kirk       (501) staff       (20)      265 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/PKG-INFO
+-rw-r--r--   0 kirk       (501) staff       (20)     1118 2021-04-14 01:41:32.000000 cc_py_commons-0.4.0/README.md
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2021-05-07 00:00:50.000000 cc_py_commons-0.4.0/cc_py_commons/__init__.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/bids/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/bids/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      802 2024-04-09 00:53:10.000000 cc_py_commons-0.4.0/cc_py_commons/bids/bid.py
+-rw-r--r--   0 kirk       (501) staff       (20)      300 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/bids/bid_history.py
+-rw-r--r--   0 kirk       (501) staff       (20)      471 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/bids/bid_history_schema.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1332 2024-04-09 00:53:10.000000 cc_py_commons-0.4.0/cc_py_commons/bids/bid_schema.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/carriers/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2021-04-14 01:41:32.000000 cc_py_commons-0.4.0/cc_py_commons/carriers/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      233 2023-07-27 21:32:34.000000 cc_py_commons-0.4.0/cc_py_commons/carriers/account_carrier_map.py
+-rw-r--r--   0 kirk       (501) staff       (20)      687 2023-02-02 05:49:27.000000 cc_py_commons-0.4.0/cc_py_commons/carriers/account_carrier_map_schema.py
+-rw-r--r--   0 kirk       (501) staff       (20)     3383 2024-05-05 05:28:58.000000 cc_py_commons-0.4.0/cc_py_commons/carriers/carrier.py
+-rw-r--r--   0 kirk       (501) staff       (20)     3093 2024-05-05 05:28:58.000000 cc_py_commons-0.4.0/cc_py_commons/carriers/carrier_schema.py
+-rw-r--r--   0 kirk       (501) staff       (20)      429 2024-04-09 00:53:10.000000 cc_py_commons-0.4.0/cc_py_commons/carriers/contact.py
+-rw-r--r--   0 kirk       (501) staff       (20)      787 2024-04-09 00:53:10.000000 cc_py_commons-0.4.0/cc_py_commons/carriers/contact_schema.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/config/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2020-08-11 23:45:04.000000 cc_py_commons-0.4.0/cc_py_commons/config/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)     6364 2024-04-09 00:53:10.000000 cc_py_commons-0.4.0/cc_py_commons/config/env.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1364 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/config/mcleod_load_fields.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1455 2020-08-11 23:45:04.000000 cc_py_commons-0.4.0/cc_py_commons/config/pc_miler_config.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/db/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2023-01-07 20:27:47.000000 cc_py_commons-0.4.0/cc_py_commons/db/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      566 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/db/connection.py
+-rw-r--r--   0 kirk       (501) staff       (20)    14097 2024-05-06 23:37:42.000000 cc_py_commons-0.4.0/cc_py_commons/geolocate.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/lanes/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/lanes/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      972 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/lanes/carrier_lane.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1251 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/lanes/carrier_lane_schema.py
+-rw-r--r--   0 kirk       (501) staff       (20)      663 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/lanes/lane.py
+-rw-r--r--   0 kirk       (501) staff       (20)      941 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/lanes/lane_schema.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/loads/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/loads/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      154 2022-09-25 19:11:30.000000 cc_py_commons-0.4.0/cc_py_commons/loads/equipment.py
+-rw-r--r--   0 kirk       (501) staff       (20)      384 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/loads/equipment_schema.py
+-rw-r--r--   0 kirk       (501) staff       (20)      965 2023-09-07 00:25:21.000000 cc_py_commons-0.4.0/cc_py_commons/loads/equipment_types.py
+-rw-r--r--   0 kirk       (501) staff       (20)      338 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/loads/freighthub_contact.py
+-rw-r--r--   0 kirk       (501) staff       (20)      442 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/loads/freighthub_contact_schema.py
+-rw-r--r--   0 kirk       (501) staff       (20)     3350 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/loads/load.py
+-rw-r--r--   0 kirk       (501) staff       (20)     4000 2023-09-07 00:25:21.000000 cc_py_commons-0.4.0/cc_py_commons/loads/load_schema.py
+-rw-r--r--   0 kirk       (501) staff       (20)      501 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/loads/load_status.py
+-rw-r--r--   0 kirk       (501) staff       (20)      286 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/loads/location.py
+-rw-r--r--   0 kirk       (501) staff       (20)      463 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/loads/location_schema.py
+-rw-r--r--   0 kirk       (501) staff       (20)      751 2023-01-07 20:27:47.000000 cc_py_commons-0.4.0/cc_py_commons/loads/map_load_response.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/quotes/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/quotes/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1967 2023-07-13 01:51:13.000000 cc_py_commons-0.4.0/cc_py_commons/quotes/quote.py
+-rw-r--r--   0 kirk       (501) staff       (20)     2638 2023-07-13 01:51:13.000000 cc_py_commons-0.4.0/cc_py_commons/quotes/quote_schema.py
+-rw-r--r--   0 kirk       (501) staff       (20)      501 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/quotes/quote_status.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/rfp/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2023-01-07 20:27:47.000000 cc_py_commons-0.4.0/cc_py_commons/rfp/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      145 2023-01-07 20:27:47.000000 cc_py_commons-0.4.0/cc_py_commons/rfp/rfp_status.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/schemas/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2021-04-14 01:41:32.000000 cc_py_commons-0.4.0/cc_py_commons/schemas/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      439 2021-04-14 01:41:32.000000 cc_py_commons-0.4.0/cc_py_commons/schemas/camel_case_schema.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/services/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2022-07-22 01:21:18.000000 cc_py_commons-0.4.0/cc_py_commons/services/__init__.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2023-07-13 01:51:13.000000 cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      653 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/accept_bid.py
+-rw-r--r--   0 kirk       (501) staff       (20)      746 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/cancel_bid.py
+-rw-r--r--   0 kirk       (501) staff       (20)      671 2023-07-13 01:51:13.000000 cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/constants.py
+-rw-r--r--   0 kirk       (501) staff       (20)      704 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/counter_bid.py
+-rw-r--r--   0 kirk       (501) staff       (20)      702 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/decline_bid.py
+-rw-r--r--   0 kirk       (501) staff       (20)      648 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/get_bid_by_amazon_order_id.py
+-rw-r--r--   0 kirk       (501) staff       (20)      943 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/get_quote.py
+-rw-r--r--   0 kirk       (501) staff       (20)      674 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/update_bid.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/services/c4/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2022-07-22 01:21:18.000000 cc_py_commons-0.4.0/cc_py_commons/services/c4/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      491 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/c4/amazon_session_token.py
+-rw-r--r--   0 kirk       (501) staff       (20)      147 2023-07-13 01:51:13.000000 cc_py_commons-0.4.0/cc_py_commons/services/c4/constants.py
+-rw-r--r--   0 kirk       (501) staff       (20)      922 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/c4/get_integration.py
+-rw-r--r--   0 kirk       (501) staff       (20)      681 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/c4/get_users_for_account.py
+-rw-r--r--   0 kirk       (501) staff       (20)      660 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/c4/refresh_amazon_token.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/services/carrier_hub/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2023-08-22 21:56:55.000000 cc_py_commons-0.4.0/cc_py_commons/services/carrier_hub/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      673 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/carrier_hub/get_carrier.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1016 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/carrier_hub/list_carriers.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1413 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/carrier_hub/list_contacts.py
+-rw-r--r--   0 kirk       (501) staff       (20)      724 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/carrier_hub/update_contact.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/services/freight_hub/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2022-07-22 01:21:18.000000 cc_py_commons-0.4.0/cc_py_commons/services/freight_hub/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      477 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/freight_hub/post_freight_hub_load.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/services/mercury/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2022-11-08 05:26:59.000000 cc_py_commons-0.4.0/cc_py_commons/services/mercury/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      571 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/mercury/get_green_screens_lane_price.py
+-rw-r--r--   0 kirk       (501) staff       (20)      553 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/mercury/get_lane_price.py
+-rw-r--r--   0 kirk       (501) staff       (20)      563 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/mercury/get_lane_price_for_bulk.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/services/slack/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2023-09-15 20:36:29.000000 cc_py_commons-0.4.0/cc_py_commons/services/slack/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1044 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/services/slack/send_slack_message.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/sns/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2021-04-14 01:41:32.000000 cc_py_commons-0.4.0/cc_py_commons/sns/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      932 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/sns/book_load_notification.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/sns/booking_agent/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2023-07-13 01:51:13.000000 cc_py_commons-0.4.0/cc_py_commons/sns/booking_agent/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      971 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/sns/booking_agent/bid_counter_failure_notification.py
+-rw-r--r--   0 kirk       (501) staff       (20)       77 2023-07-13 01:51:13.000000 cc_py_commons-0.4.0/cc_py_commons/sns/booking_agent/constants.py
+-rw-r--r--   0 kirk       (501) staff       (20)      747 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/sns/booking_agent/send_sns_notification.py
+-rw-r--r--   0 kirk       (501) staff       (20)      987 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/sns/booking_assistant_flow_notification.py
+-rw-r--r--   0 kirk       (501) staff       (20)      751 2021-06-09 01:06:31.000000 cc_py_commons-0.4.0/cc_py_commons/sns/import_movements_notification.py
+-rw-r--r--   0 kirk       (501) staff       (20)      901 2024-04-30 23:06:40.000000 cc_py_commons-0.4.0/cc_py_commons/sns/parsed_carrier_notification.py
+-rw-r--r--   0 kirk       (501) staff       (20)      269 2021-04-14 01:41:32.000000 cc_py_commons-0.4.0/cc_py_commons/sns/sns_service.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/sqs/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2022-09-16 05:49:21.000000 cc_py_commons-0.4.0/cc_py_commons/sqs/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1152 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/sqs/booking_assistant_flow_event.py
+-rw-r--r--   0 kirk       (501) staff       (20)      440 2022-09-16 05:49:21.000000 cc_py_commons-0.4.0/cc_py_commons/sqs/sqs_service.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/tests/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2021-11-16 01:32:23.000000 cc_py_commons-0.4.0/cc_py_commons/tests/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      844 2021-12-22 05:36:02.000000 cc_py_commons-0.4.0/cc_py_commons/tests/test_case_conversion.py
+-rw-r--r--   0 kirk       (501) staff       (20)      760 2023-03-29 19:12:55.000000 cc_py_commons-0.4.0/cc_py_commons/tests/test_lambda_utils.py
+-rw-r--r--   0 kirk       (501) staff       (20)     2036 2023-09-07 00:25:21.000000 cc_py_commons-0.4.0/cc_py_commons/tests/test_map_transaction.py
+-rw-r--r--   0 kirk       (501) staff       (20)      475 2022-05-25 05:49:37.000000 cc_py_commons-0.4.0/cc_py_commons/tests/test_temperature_utils.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/transactions/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2021-11-16 01:32:23.000000 cc_py_commons-0.4.0/cc_py_commons/transactions/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)      442 2021-11-16 01:32:23.000000 cc_py_commons-0.4.0/cc_py_commons/transactions/equipment_clas_schema.py
+-rw-r--r--   0 kirk       (501) staff       (20)      213 2021-11-16 01:32:23.000000 cc_py_commons-0.4.0/cc_py_commons/transactions/equipment_class.py
+-rw-r--r--   0 kirk       (501) staff       (20)      289 2021-11-16 01:32:23.000000 cc_py_commons-0.4.0/cc_py_commons/transactions/equipment_mapping.py
+-rw-r--r--   0 kirk       (501) staff       (20)      540 2021-11-16 01:32:23.000000 cc_py_commons-0.4.0/cc_py_commons/transactions/equipment_mapping_schema.py
+-rw-r--r--   0 kirk       (501) staff       (20)     3181 2024-04-09 00:53:10.000000 cc_py_commons-0.4.0/cc_py_commons/transactions/map_transaction.py
+-rw-r--r--   0 kirk       (501) staff       (20)     4931 2023-09-07 00:25:21.000000 cc_py_commons-0.4.0/cc_py_commons/transactions/transaction.py
+-rw-r--r--   0 kirk       (501) staff       (20)     5159 2023-10-26 00:50:00.000000 cc_py_commons-0.4.0/cc_py_commons/transactions/transaction_schema.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons/utils/
+-rw-r--r--   0 kirk       (501) staff       (20)        0 2020-08-11 23:45:04.000000 cc_py_commons-0.4.0/cc_py_commons/utils/__init__.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1519 2022-07-22 01:21:18.000000 cc_py_commons-0.4.0/cc_py_commons/utils/case_conversion.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1168 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/utils/datadog_logger.py
+-rw-r--r--   0 kirk       (501) staff       (20)      759 2023-01-07 20:27:47.000000 cc_py_commons-0.4.0/cc_py_commons/utils/datetimes.py
+-rw-r--r--   0 kirk       (501) staff       (20)      723 2023-08-22 21:56:55.000000 cc_py_commons-0.4.0/cc_py_commons/utils/dimension_utils.py
+-rw-r--r--   0 kirk       (501) staff       (20)      513 2024-04-09 00:53:10.000000 cc_py_commons-0.4.0/cc_py_commons/utils/get_delivery_date.py
+-rw-r--r--   0 kirk       (501) staff       (20)      893 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/utils/json_logger.py
+-rw-r--r--   0 kirk       (501) staff       (20)      219 2023-03-29 19:12:55.000000 cc_py_commons-0.4.0/cc_py_commons/utils/lambda_utils.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1051 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/utils/local_file.py
+-rw-r--r--   0 kirk       (501) staff       (20)      998 2023-10-26 00:50:00.000000 cc_py_commons-0.4.0/cc_py_commons/utils/logger.py
+-rw-r--r--   0 kirk       (501) staff       (20)     2026 2024-04-09 00:53:10.000000 cc_py_commons-0.4.0/cc_py_commons/utils/logger_v2.py
+-rw-r--r--   0 kirk       (501) staff       (20)     2792 2020-08-11 23:45:04.000000 cc_py_commons-0.4.0/cc_py_commons/utils/pc_miler_utils.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1237 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/utils/price_utils.py
+-rw-r--r--   0 kirk       (501) staff       (20)     1044 2020-08-11 23:45:04.000000 cc_py_commons-0.4.0/cc_py_commons/utils/redis.py
+-rw-r--r--   0 kirk       (501) staff       (20)     2367 2024-02-08 21:28:28.000000 cc_py_commons-0.4.0/cc_py_commons/utils/s3_file.py
+-rw-r--r--   0 kirk       (501) staff       (20)      353 2023-08-22 21:56:55.000000 cc_py_commons-0.4.0/cc_py_commons/utils/temperature_utils.py
+drwxr-xr-x   0 kirk       (501) staff       (20)        0 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons.egg-info/
+-rw-r--r--   0 kirk       (501) staff       (20)      265 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons.egg-info/PKG-INFO
+-rw-r--r--   0 kirk       (501) staff       (20)     4989 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 kirk       (501) staff       (20)        1 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 kirk       (501) staff       (20)       66 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons.egg-info/requires.txt
+-rw-r--r--   0 kirk       (501) staff       (20)       14 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/cc_py_commons.egg-info/top_level.txt
+-rw-r--r--   0 kirk       (501) staff       (20)       38 2024-05-06 23:40:54.000000 cc_py_commons-0.4.0/setup.cfg
+-rw-r--r--   0 kirk       (501) staff       (20)      435 2024-05-06 23:26:33.000000 cc_py_commons-0.4.0/setup.py
```

### Comparing `cc_py_commons-0.3.99/README.md` & `cc_py_commons-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/bids/bid.py` & `cc_py_commons-0.4.0/cc_py_commons/bids/bid.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/bids/bid_schema.py` & `cc_py_commons-0.4.0/cc_py_commons/bids/bid_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/carriers/account_carrier_map_schema.py` & `cc_py_commons-0.4.0/cc_py_commons/carriers/account_carrier_map_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/carriers/carrier.py` & `cc_py_commons-0.4.0/cc_py_commons/carriers/carrier.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/carriers/carrier_schema.py` & `cc_py_commons-0.4.0/cc_py_commons/carriers/carrier_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/carriers/contact_schema.py` & `cc_py_commons-0.4.0/cc_py_commons/carriers/contact_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/config/env.py` & `cc_py_commons-0.4.0/cc_py_commons/config/env.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/config/mcleod_load_fields.py` & `cc_py_commons-0.4.0/cc_py_commons/config/mcleod_load_fields.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/config/pc_miler_config.py` & `cc_py_commons-0.4.0/cc_py_commons/config/pc_miler_config.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/db/connection.py` & `cc_py_commons-0.4.0/cc_py_commons/db/connection.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/geolocate.py` & `cc_py_commons-0.4.0/cc_py_commons/geolocate.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,51 @@
 from ast import literal_eval
 
 def get_location(city, state, zipcode, logger):
   return get_location_with_country(city, state, zipcode, None, logger)
 
 def get_location_with_country(city, state, zipcode, country, logger):
   from_cache = False
-  data = __get_location_from_cache(city, state, zipcode, logger)
+  postcode = zipcode
+
+  if postcode:
+    parts = zipcode.split('-')
+    postcode = parts[0] if len(parts) > 0 else zipcode
+
+  data = __get_location_from_cache(city, state, postcode, logger)
 
   if data:
-    if data.get('country') and (not zipcode or zipcode == data.get('postcode')):
+    if data.get('country') and (not postcode or postcode == data.get('postcode')):
       from_cache = True
     else:
+      logger.debug(json.dumps({
+        'message': 'Found locatin in cache that was not a match',
+        'city': city,
+        'state': state,
+        'zipcode': zipcode,
+        'postcode': postcode,
+        'country': country,
+        'cache_key': __get_location_string(city, state, postcode) 
+      }))
       data = None
       
   if not data:
     logger.debug(json.dumps({
       'message': 'Could not find location in cache',
       'city': city,
       'state': state,
       'postcode': zipcode,
       'country': country,
-      'cache_key': __get_location_string(city, state, zipcode) 
+      'cache_key': __get_location_string(city, state, postcode) 
     }))
-    data = __get_google_location(city, state, zipcode, country, logger)
+    data = __get_google_location(city, state, postcode, country, logger)
 
-  if not data and zipcode:
+  if not data and postcode:
     from_cache = False
-    data = __get_google_location(city=None, state=None, zipcode=zipcode, country=None, logger=logger)
+    data = __get_google_location(city=None, state=None, zipcode=postcode, country=None, logger=logger)
 
   if data:
     if not from_cache:
       __cache_location(city, state, zipcode, data, logger)
   else:
     logger.debug(f"geolocate.get_location - Google returned no result for ({city}, {state}, {zipcode}, {country})")
```

### Comparing `cc_py_commons-0.3.99/cc_py_commons/lanes/carrier_lane.py` & `cc_py_commons-0.4.0/cc_py_commons/lanes/carrier_lane.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/lanes/carrier_lane_schema.py` & `cc_py_commons-0.4.0/cc_py_commons/lanes/carrier_lane_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/lanes/lane.py` & `cc_py_commons-0.4.0/cc_py_commons/lanes/lane.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/lanes/lane_schema.py` & `cc_py_commons-0.4.0/cc_py_commons/lanes/lane_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/loads/equipment_types.py` & `cc_py_commons-0.4.0/cc_py_commons/loads/equipment_types.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/loads/load.py` & `cc_py_commons-0.4.0/cc_py_commons/loads/load.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/loads/load_schema.py` & `cc_py_commons-0.4.0/cc_py_commons/loads/load_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/loads/map_load_response.py` & `cc_py_commons-0.4.0/cc_py_commons/loads/map_load_response.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/quotes/quote.py` & `cc_py_commons-0.4.0/cc_py_commons/quotes/quote.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/quotes/quote_schema.py` & `cc_py_commons-0.4.0/cc_py_commons/quotes/quote_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/accept_bid.py` & `cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/accept_bid.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/cancel_bid.py` & `cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/cancel_bid.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/constants.py` & `cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/constants.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/counter_bid.py` & `cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/counter_bid.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/decline_bid.py` & `cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/decline_bid.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/get_bid_by_amazon_order_id.py` & `cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/get_bid_by_amazon_order_id.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/get_quote.py` & `cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/get_quote.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/booking_agent/update_bid.py` & `cc_py_commons-0.4.0/cc_py_commons/services/booking_agent/update_bid.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/c4/get_integration.py` & `cc_py_commons-0.4.0/cc_py_commons/services/c4/get_integration.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/c4/get_users_for_account.py` & `cc_py_commons-0.4.0/cc_py_commons/services/c4/get_users_for_account.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/c4/refresh_amazon_token.py` & `cc_py_commons-0.4.0/cc_py_commons/services/c4/refresh_amazon_token.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/carrier_hub/get_carrier.py` & `cc_py_commons-0.4.0/cc_py_commons/services/carrier_hub/get_carrier.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/carrier_hub/list_carriers.py` & `cc_py_commons-0.4.0/cc_py_commons/services/carrier_hub/list_carriers.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/carrier_hub/list_contacts.py` & `cc_py_commons-0.4.0/cc_py_commons/services/carrier_hub/list_contacts.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/carrier_hub/update_contact.py` & `cc_py_commons-0.4.0/cc_py_commons/services/carrier_hub/update_contact.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/mercury/get_green_screens_lane_price.py` & `cc_py_commons-0.4.0/cc_py_commons/services/mercury/get_green_screens_lane_price.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/mercury/get_lane_price.py` & `cc_py_commons-0.4.0/cc_py_commons/services/mercury/get_lane_price.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/mercury/get_lane_price_for_bulk.py` & `cc_py_commons-0.4.0/cc_py_commons/services/mercury/get_lane_price_for_bulk.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/services/slack/send_slack_message.py` & `cc_py_commons-0.4.0/cc_py_commons/services/slack/send_slack_message.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/sns/book_load_notification.py` & `cc_py_commons-0.4.0/cc_py_commons/sns/book_load_notification.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/sns/booking_agent/bid_counter_failure_notification.py` & `cc_py_commons-0.4.0/cc_py_commons/sns/booking_agent/bid_counter_failure_notification.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/sns/booking_agent/send_sns_notification.py` & `cc_py_commons-0.4.0/cc_py_commons/sns/booking_agent/send_sns_notification.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/sns/booking_assistant_flow_notification.py` & `cc_py_commons-0.4.0/cc_py_commons/sns/booking_assistant_flow_notification.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/sns/import_movements_notification.py` & `cc_py_commons-0.4.0/cc_py_commons/sns/import_movements_notification.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/sns/parsed_carrier_notification.py` & `cc_py_commons-0.4.0/cc_py_commons/sns/parsed_carrier_notification.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/sqs/booking_assistant_flow_event.py` & `cc_py_commons-0.4.0/cc_py_commons/sqs/booking_assistant_flow_event.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/tests/test_case_conversion.py` & `cc_py_commons-0.4.0/cc_py_commons/tests/test_case_conversion.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/tests/test_lambda_utils.py` & `cc_py_commons-0.4.0/cc_py_commons/tests/test_lambda_utils.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/tests/test_map_transaction.py` & `cc_py_commons-0.4.0/cc_py_commons/tests/test_map_transaction.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/transactions/equipment_mapping_schema.py` & `cc_py_commons-0.4.0/cc_py_commons/transactions/equipment_mapping_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/transactions/map_transaction.py` & `cc_py_commons-0.4.0/cc_py_commons/transactions/map_transaction.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/transactions/transaction.py` & `cc_py_commons-0.4.0/cc_py_commons/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/transactions/transaction_schema.py` & `cc_py_commons-0.4.0/cc_py_commons/transactions/transaction_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/utils/case_conversion.py` & `cc_py_commons-0.4.0/cc_py_commons/utils/case_conversion.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/utils/datadog_logger.py` & `cc_py_commons-0.4.0/cc_py_commons/utils/datadog_logger.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/utils/datetimes.py` & `cc_py_commons-0.4.0/cc_py_commons/utils/datetimes.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/utils/dimension_utils.py` & `cc_py_commons-0.4.0/cc_py_commons/utils/dimension_utils.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/utils/get_delivery_date.py` & `cc_py_commons-0.4.0/cc_py_commons/utils/get_delivery_date.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/utils/json_logger.py` & `cc_py_commons-0.4.0/cc_py_commons/utils/json_logger.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/utils/local_file.py` & `cc_py_commons-0.4.0/cc_py_commons/utils/local_file.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/utils/logger.py` & `cc_py_commons-0.4.0/cc_py_commons/utils/logger.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/utils/logger_v2.py` & `cc_py_commons-0.4.0/cc_py_commons/utils/logger_v2.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/utils/pc_miler_utils.py` & `cc_py_commons-0.4.0/cc_py_commons/utils/pc_miler_utils.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/utils/price_utils.py` & `cc_py_commons-0.4.0/cc_py_commons/utils/price_utils.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/utils/redis.py` & `cc_py_commons-0.4.0/cc_py_commons/utils/redis.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons/utils/s3_file.py` & `cc_py_commons-0.4.0/cc_py_commons/utils/s3_file.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.99/cc_py_commons.egg-info/SOURCES.txt` & `cc_py_commons-0.4.0/cc_py_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*
