# Comparing `tmp/airbyte_source_amazon_seller_partner-4.2.1.tar.gz` & `tmp/airbyte_source_amazon_seller_partner-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_amazon_seller_partner-4.2.1.tar", max compression
+gzip compressed data, was "airbyte_source_amazon_seller_partner-4.2.2.tar", max compression
```

## Comparing `airbyte_source_amazon_seller_partner-4.2.1.tar` & `airbyte_source_amazon_seller_partner-4.2.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     4765 2024-04-10 13:21:02.682068 airbyte_source_amazon_seller_partner-4.2.1/README.md
--rw-r--r--   0        0        0      895 2024-04-10 13:24:04.473507 airbyte_source_amazon_seller_partner-4.2.1/pyproject.toml
--rw-r--r--   0        0        0     1191 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/__init__.py
--rw-r--r--   0        0        0      638 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/auth.py
--rw-r--r--   0        0        0     6322 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/config_migrations.py
--rw-r--r--   0        0        0     3387 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/constants.py
--rw-r--r--   0        0        0      479 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/run.py
--rw-r--r--   0        0        0      576 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json
--rw-r--r--   0        0        0      568 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json
--rw-r--r--   0        0        0     2997 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json
--rw-r--r--   0        0        0      799 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json
--rw-r--r--   0        0        0     1112 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json
--rw-r--r--   0        0        0      823 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json
--rw-r--r--   0        0        0     2434 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json
--rw-r--r--   0        0        0      950 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json
--rw-r--r--   0        0        0      744 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json
--rw-r--r--   0        0        0     1816 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json
--rw-r--r--   0        0        0     1305 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json
--rw-r--r--   0        0        0      916 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json
--rw-r--r--   0        0        0     4986 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json
--rw-r--r--   0        0        0     1453 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json
--rw-r--r--   0        0        0     1497 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json
--rw-r--r--   0        0        0     1345 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json
--rw-r--r--   0        0        0     1637 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json
--rw-r--r--   0        0        0     2397 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json
--rw-r--r--   0        0        0     1999 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json
--rw-r--r--   0        0        0     2464 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json
--rw-r--r--   0        0        0     2471 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
--rw-r--r--   0        0        0     1945 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json
--rw-r--r--   0        0        0     1833 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json
--rw-r--r--   0        0        0     2113 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json
--rw-r--r--   0        0        0     1033 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json
--rw-r--r--   0        0        0     1353 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json
--rw-r--r--   0        0        0      645 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json
--rw-r--r--   0        0        0     2590 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json
--rw-r--r--   0        0        0     2157 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json
--rw-r--r--   0        0        0     2891 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json
--rw-r--r--   0        0        0     2830 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json
--rw-r--r--   0        0        0     1756 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json
--rw-r--r--   0        0        0     5258 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json
--rw-r--r--   0        0        0     2208 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json
--rw-r--r--   0        0        0     2235 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json
--rw-r--r--   0        0        0      647 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json
--rw-r--r--   0        0        0     1250 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json
--rw-r--r--   0        0        0     2408 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json
--rw-r--r--   0        0        0      387 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_FRESH_REPORT.json
--rw-r--r--   0        0        0      388 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_RETAIL_REPORT.json
--rw-r--r--   0        0        0     2154 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json
--rw-r--r--   0        0        0      979 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json
--rw-r--r--   0        0        0      812 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json
--rw-r--r--   0        0        0     1269 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json
--rw-r--r--   0        0        0      940 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json
--rw-r--r--   0        0        0     2255 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
--rw-r--r--   0        0        0     2266 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json
--rw-r--r--   0        0        0     1543 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json
--rw-r--r--   0        0        0    25722 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/ListFinancialEvents.json
--rw-r--r--   0        0        0     6713 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/OrderItems.json
--rw-r--r--   0        0        0     3950 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/Orders.json
--rw-r--r--   0        0        0     6865 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json
--rw-r--r--   0        0        0    10312 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/VendorOrders.json
--rw-r--r--   0        0        0      605 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json
--rw-r--r--   0        0        0    10019 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/source.py
--rw-r--r--   0        0        0     8913 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/spec.json
--rw-r--r--   0        0        0    56375 2024-04-10 13:21:02.690068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/streams.py
--rw-r--r--   0        0        0      403 2024-04-10 13:21:02.690068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/utils.py
--rw-r--r--   0        0        0     5587 1970-01-01 00:00:00.000000 airbyte_source_amazon_seller_partner-4.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4765 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/README.md
+-rw-r--r--   0        0        0      899 2024-05-07 12:17:53.700421 airbyte_source_amazon_seller_partner-4.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1191 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/__init__.py
+-rw-r--r--   0        0        0      638 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/auth.py
+-rw-r--r--   0        0        0     6322 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/config_migrations.py
+-rw-r--r--   0        0        0     3387 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/constants.py
+-rw-r--r--   0        0        0      479 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/run.py
+-rw-r--r--   0        0        0     1291 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json
+-rw-r--r--   0        0        0     1221 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json
+-rw-r--r--   0        0        0     6635 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json
+-rw-r--r--   0        0        0     1441 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json
+-rw-r--r--   0        0        0     2173 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json
+-rw-r--r--   0        0        0     1729 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json
+-rw-r--r--   0        0        0     5029 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json
+-rw-r--r--   0        0        0     2159 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json
+-rw-r--r--   0        0        0     1613 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json
+-rw-r--r--   0        0        0     2036 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json
+-rw-r--r--   0        0        0     2446 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json
+-rw-r--r--   0        0        0     1802 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json
+-rw-r--r--   0        0        0    11885 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json
+-rw-r--r--   0        0        0     3678 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json
+-rw-r--r--   0        0        0     2965 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json
+-rw-r--r--   0        0        0     3066 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json
+-rw-r--r--   0        0        0     3349 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json
+-rw-r--r--   0        0        0     4645 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json
+-rw-r--r--   0        0        0     3699 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json
+-rw-r--r--   0        0        0     4684 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json
+-rw-r--r--   0        0        0     4819 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
+-rw-r--r--   0        0        0     4125 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json
+-rw-r--r--   0        0        0     3434 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json
+-rw-r--r--   0        0        0     4629 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json
+-rw-r--r--   0        0        0     2193 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json
+-rw-r--r--   0        0        0     2823 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json
+-rw-r--r--   0        0        0     1381 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json
+-rw-r--r--   0        0        0     6146 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json
+-rw-r--r--   0        0        0     3884 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json
+-rw-r--r--   0        0        0     6479 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json
+-rw-r--r--   0        0        0     6472 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json
+-rw-r--r--   0        0        0     3988 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json
+-rw-r--r--   0        0        0     8105 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json
+-rw-r--r--   0        0        0     4129 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json
+-rw-r--r--   0        0        0     4223 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json
+-rw-r--r--   0        0        0     1185 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json
+-rw-r--r--   0        0        0     2709 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json
+-rw-r--r--   0        0        0     5477 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json
+-rw-r--r--   0        0        0      387 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_FRESH_REPORT.json
+-rw-r--r--   0        0        0      388 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_RETAIL_REPORT.json
+-rw-r--r--   0        0        0     4217 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json
+-rw-r--r--   0        0        0     1550 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json
+-rw-r--r--   0        0        0     1313 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json
+-rw-r--r--   0        0        0     2411 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json
+-rw-r--r--   0        0        0     1384 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json
+-rw-r--r--   0        0        0     4860 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
+-rw-r--r--   0        0        0     3786 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json
+-rw-r--r--   0        0        0     2970 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json
+-rw-r--r--   0        0        0    44785 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/ListFinancialEvents.json
+-rw-r--r--   0        0        0    11058 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/OrderItems.json
+-rw-r--r--   0        0        0     7150 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/Orders.json
+-rw-r--r--   0        0        0     9967 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json
+-rw-r--r--   0        0        0    16089 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/VendorOrders.json
+-rw-r--r--   0        0        0      605 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json
+-rw-r--r--   0        0        0    10019 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/source.py
+-rw-r--r--   0        0        0     8913 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/spec.json
+-rw-r--r--   0        0        0    56375 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/streams.py
+-rw-r--r--   0        0        0      403 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/utils.py
+-rw-r--r--   0        0        0     5589 1970-01-01 00:00:00.000000 airbyte_source_amazon_seller_partner-4.2.2/PKG-INFO
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/README.md` & `airbyte_source_amazon_seller_partner-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/pyproject.toml` & `airbyte_source_amazon_seller_partner-4.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "4.2.1"
+version = "4.2.2"
 name = "airbyte-source-amazon-seller-partner"
 description = "Source implementation for Amazon Seller Partner."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_amazon_seller_partner" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.80.0"
 xmltodict = "~=0.12"
 dateparser = "==1.2.0"
 
 [tool.poetry.scripts]
 source-amazon-seller-partner = "source_amazon_seller_partner.run:run"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/__init__.py` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/auth.py` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/config_migrations.py` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/constants.py` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/constants.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7185897435897436%*

 * *Differences: {"'description'": "'This report shares inventory data at an ASIN level, aggregated to an hourly "*

 * *                  'granularity. Requests can span multiple date range periods, including the '*

 * *                  "current day.'",*

 * * "'properties'": "{'asin': {'description': 'Unique identifier for the product on Amazon.'}, "*

 * *                 "'dataEndTime': {'description': 'The timestamp when the inventory data is current "*

 * *                 "until.'}, 'queryEndDate': {'description': 'The end date of the query pe […]*

```diff
@@ -1,83 +1,54 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "Brand Analytics Repeat Purchase Reports",
+    "description": "This report shares inventory data at an ASIN level, aggregated to an hourly granularity. Requests can span multiple date range periods, including the current day.",
     "properties": {
         "asin": {
+            "description": "Unique identifier for the product on Amazon.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "dataEndTime": {
+            "description": "The timestamp when the inventory data is current until.",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "endDate": {
-            "format": "date",
+        "endTime": {
+            "description": "The timestamp when the real-time inventory report query ends.",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "orders": {
+        "highlyAvailableInventory": {
+            "description": "Indicator for products with high availability in inventory.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "queryEndDate": {
+            "description": "The end date of the query period for real-time inventory report data.",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "repeatCustomersPctTotal": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "repeatPurchaseRevenue": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "null",
-                        "number"
-                    ]
-                },
-                "currencyCode": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": "object"
-        },
-        "repeatPurchaseRevenuePctTotal": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "startDate": {
-            "format": "date",
+        "startTime": {
+            "description": "The timestamp when the real-time inventory report query starts.",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "uniqueCustomers": {
-            "type": [
-                "null",
-                "integer"
-            ]
         }
     },
-    "title": "Brand Analytics Repeat Purchase Reports",
+    "title": "Rapid Retail Analytics Inventory Report",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8014880952380953%*

 * *Differences: {"'properties'": "{'dataEndTime': {'description': 'End time of the data'}, 'Date': "*

 * *                 "OrderedDict([('description', 'Date of the event'), ('type', ['null', 'string']), "*

 * *                 "('format', 'date')]), 'FNSKU': OrderedDict([('description', 'Fulfillment Network "*

 * *                 "Stock Keeping Unit'), ('type', ['null', 'string'])]), 'ASIN': "*

 * *                 "OrderedDict([('description', 'Amazon Standard Identification Number for the "*

 * *                 "product'), ('type', ['null',  […]*

```diff
@@ -1,220 +1,164 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "description": "",
     "properties": {
-        "asin": {
+        "ASIN": {
+            "description": "Amazon Standard Identification Number for the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "brand": {
+        "Customer Returns": {
+            "description": "Products returned by customers",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "currency": {
+        "Customer Shipments": {
+            "description": "Products shipped to customers",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "current-fee-category": {
+        "Damaged": {
+            "description": "Products that are damaged",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "dataEndTime": {
+        "Date": {
+            "description": "Date of the event",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "estimated-fee-total": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "estimated-future-fee (Current Selling on Amazon + Future Fulfillment fees)": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "estimated-future-order-handling-fee-per-order": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "estimated-future-pick-pack-fee-per-unit": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "estimated-future-referral-fee-per-unit": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "estimated-future-weight-handling-fee-per-unit": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "estimated-order-handling-fee-per-order": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "estimated-pick-pack-fee-per-unit": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "estimated-referral-fee-per-unit": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "estimated-variable-closing-fee": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "estimated-weight-handling-fee-per-unit": {
+        "Disposed": {
+            "description": "Products that have been disposed of",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "expected-fulfillment-fee-per-unit": {
+        "Disposition": {
+            "description": "Action taken with the products",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "expected-future-fulfillment-fee-per-unit": {
+        "Ending Warehouse Balance": {
+            "description": "The balance of products at the end of the period",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "fnsku": {
+        "FNSKU": {
+            "description": "Fulfillment Network Stock Keeping Unit",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "fulfilled-by": {
+        "Found": {
+            "description": "Products that were found",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "future-fee-category": {
+        "In Transit Between Warehouses": {
+            "description": "Products moving between warehouses",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "future-fee-category-effective-date": {
-            "format": "date-time",
+        "Location": {
+            "description": "Location of the warehouse",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "item-package-weight": {
+        "Lost": {
+            "description": "Products that are lost",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "length-and-girth": {
+        "MSKU": {
+            "description": "Merchant Stock Keeping Unit",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "longest-side": {
+        "Other Events": {
+            "description": "Any other events related to the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "median-side": {
+        "Receipts": {
+            "description": "Products received",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "product-group": {
+        "Starting Warehouse Balance": {
+            "description": "The balance of products at the start of the period",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "product-name": {
+        "Title": {
+            "description": "Title of the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "product-size-tier": {
+        "Unknown Events": {
+            "description": "Any events with unknown causes",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "sales-price": {
+        "Vendor Returns": {
+            "description": "Products returned by vendors",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "shortest-side": {
+        "Warehouse Transfer In/Out": {
+            "description": "Products transferred in or out of the warehouse",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "sku": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "unit-of-dimension": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "unit-of-weight": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "your-price": {
+        "dataEndTime": {
+            "description": "End time of the data",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "title": "FBA Fee Preview Report",
+    "title": "Inventory Ledger Report - Summary View",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.991875%*

 * *Differences: {"'properties'": "{'shipment-date': {'description': 'Date and time of the free replacement "*

 * *                 "shipment in DD-MON-YYYY format'}, 'sku': {'description': 'Unique identifier of "*

 * *                 "the item used by the seller'}, 'fulfillment-center-id': {'description': 'ID of "*

 * *                 "the fulfillment center shipping this unit'}, 'original-fulfillment-center-id': "*

 * *                 "{'description': 'ID of the original fulfillment center shipping the free "*

 * *                 "replaced it […]*

```diff
@@ -7,79 +7,80 @@
             "title": "ASIN",
             "type": [
                 "null",
                 "string"
             ]
         },
         "dataEndTime": {
+            "description": "End time of the data collection period",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
         "fulfillment-center-id": {
-            "description": "Fulfillment center shipping this unit.",
+            "description": "ID of the fulfillment center shipping this unit",
             "title": "Warehouse ID",
             "type": [
                 "null",
                 "string"
             ]
         },
         "original-amazon-order-id": {
-            "description": "Order ID of original shipment",
+            "description": "Order ID of the original shipment for the replacement item",
             "title": "Original Customer Order ID",
             "type": [
                 "null",
                 "string"
             ]
         },
         "original-fulfillment-center-id": {
-            "description": "Original fulfillment center shipping free replaced item.",
+            "description": "ID of the original fulfillment center shipping the free replaced item",
             "title": "Original Warehouse ID",
             "type": [
                 "null",
                 "string"
             ]
         },
         "quantity": {
-            "description": "Units shipped in replacement shipment",
+            "description": "Number of units shipped in the replacement shipment",
             "title": "Quantity",
             "type": [
                 "null",
                 "string"
             ]
         },
         "replacement-customer-order-id": {
-            "description": "Order ID of the replacement order",
+            "description": "Order ID of the replacement order for the original item",
             "title": "Replacement Customer Order Id",
             "type": [
                 "null",
                 "string"
             ]
         },
         "replacement-reason-code": {
-            "description": "Reason for replacement",
+            "description": "Code indicating the reason for the replacement",
             "title": "Replacement Reason Code",
             "type": [
                 "null",
                 "string"
             ]
         },
         "shipment-date": {
-            "description": "DD-MON-YYYY. Date of free replacement shipment",
+            "description": "Date and time of the free replacement shipment in DD-MON-YYYY format",
             "format": "date-time",
             "title": "Date",
             "type": [
                 "null",
                 "string"
             ]
         },
         "sku": {
-            "description": "Seller's item identifier",
+            "description": "Unique identifier of the item used by the seller",
             "title": "Merchant SKU",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7037878787878789%*

 * *Differences: {"'description'": "''",*

 * * "'properties'": "{'dataEndTime': {'description': 'Timestamp indicating when the data was last "*

 * *                 "updated'}, 'seller-sku': OrderedDict([('description', 'Unique SKU assigned by "*

 * *                 "the seller for the product'), ('type', ['null', 'string'])]), "*

 * *                 "'fulfillment-channel-sku': OrderedDict([('description', 'Unique SKU assigned by "*

 * *                 "the seller for fulfillment'), ('type', ['null', 'string'])]), 'asin': "*

 * *                 "Ord […]*

```diff
@@ -1,107 +1,58 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "FBA Fulfillment Removal Order Detail Data Reports",
+    "description": "",
     "properties": {
-        "cancelled-quantity": {
+        "asin": {
+            "description": "Unique Amazon Standard Identification Number assigned to the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "currency": {
+        "condition-type": {
+            "description": "Type of condition (new, used, refurbished, etc.) of the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "dataEndTime": {
-            "format": "date",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "disposed-quantity": {
+        "country": {
+            "description": "Country code identifying the country the inventory data pertains to",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "disposition": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "fnsku": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "in-process-quantity": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "last-updated-date": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "order-id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "order-status": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "order-type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "removal-fee": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "request-date": {
-            "format": "date-time",
+        "dataEndTime": {
+            "description": "Timestamp indicating when the data was last updated",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "requested-quantity": {
+        "fulfillment-channel-sku": {
+            "description": "Unique SKU assigned by the seller for fulfillment",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "shipped-quantity": {
+        "quantity-for-local-fulfillment": {
+            "description": "Quantity of the product available for local fulfillment",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "sku": {
+        "seller-sku": {
+            "description": "Unique SKU assigned by the seller for the product",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "title": "FBA Fulfillment Removal Order Detail Data",
+    "title": "FBA Multi-Country Inventory Report",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7049019607843137%*

 * *Differences: {"'description'": "'Brand Analytics Market Basket Reports'",*

 * * "'properties'": "{'dataEndTime': {'description': 'The date and time when the data collection "*

 * *                 "ended.'}, 'startDate': OrderedDict([('description', 'The start date of the data "*

 * *                 "collection period.'), ('type', ['null', 'string']), ('format', 'date')]), "*

 * *                 "'endDate': OrderedDict([('description', 'The end date of the data collection "*

 * *                 "period.'), ('type', ['null', 'string']), ('for […]*

```diff
@@ -1,71 +1,68 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "FBA Fulfillment Removal Shipment Detail Data Reports",
+    "description": "Brand Analytics Market Basket Reports",
     "properties": {
-        "carrier": {
+        "asin": {
+            "description": "The ASIN (Amazon Standard Identification Number) of the product.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "dataEndTime": {
-            "format": "date",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "disposition": {
+        "combinationPct": {
+            "description": "The percentage of times this ASIN was purchased with another ASIN.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "fnsku": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "order-id": {
+        "dataEndTime": {
+            "description": "The date and time when the data collection ended.",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "quantity shipped": {
+        "endDate": {
+            "description": "The end date of the data collection period.",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "removal-date": {
-            "format": "date-time",
+        "purchasedWithAsin": {
+            "description": "The ASINs of the products that were frequently purchased with this ASIN.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "shipment-date": {
-            "format": "date-time",
+        "purchasedWithRank": {
+            "description": "The ranking of products that were frequently purchased with this ASIN.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "sku": {
+        "queryEndDate": {
+            "description": "The end date of the query period.",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tracking-number": {
+        "startDate": {
+            "description": "The start date of the data collection period.",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "title": "FBA Fulfillment Removal Shipment Detail Data",
+    "title": "Brand Analytics Market Basket Reports",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7055555555555555%*

 * *Differences: {"'description'": "''",*

 * * "'properties'": "{'product-name': {'description': 'Name of the product'}, 'sku': {'description': "*

 * *                 "'Stock Keeping Unit (SKU) of the product'}, 'dataEndTime': {'description': 'End "*

 * *                 "time of the data'}, 'primary-action': OrderedDict([('description', 'Primary "*

 * *                 "action to be taken for the inventory'), ('type', ['null', 'string'])]), "*

 * *                 "'date-stranded': OrderedDict([('description', 'Date when the inventory was "*

 * *      […]*

```diff
@@ -1,154 +1,144 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "Flat File All Orders Data by Last Update Date General Reports",
+    "description": "",
     "properties": {
-        "buyer-email": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "buyer-phone-number": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "dataEndTime": {
-            "format": "date",
+        "Date-to-take-auto-removal": {
+            "description": "Date when the stranded inventory will be automatically removed",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "days-past-promise": {
+        "asin": {
+            "description": "Amazon Standard Identification Number (ASIN) of the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "is-business-order": {
+        "condition": {
+            "description": "Condition of the product in the inventory",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "order-id": {
-            "type": "string"
-        },
-        "order-item-id": {
+        "dataEndTime": {
+            "description": "End time of the data",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "payments-date": {
+        "date-stranded": {
+            "description": "Date when the inventory was stranded",
             "format": "date-time",
-            "type": "string"
-        },
-        "product-name": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "promise-date": {
-            "format": "date-time",
-            "type": "string"
-        },
-        "purchase-date": {
-            "format": "date-time",
-            "type": "string"
-        },
-        "purchase-order-number": {
+        "error-message": {
+            "description": "Any error message related to the inventory status",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "quantity-purchased": {
+        "fnsku": {
+            "description": "Fulfillment Network Stock Keeping Unit (FNSKU) of the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "quantity-shipped": {
+        "fulfillable-qty": {
+            "description": "Quantity of the product that is fulfillable",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "quantity-to-ship": {
+        "fulfilled-by": {
+            "description": "Who fulfills the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "recipient-name": {
+        "inbound-shipped-qty": {
+            "description": "Quantity of the product that has been shipped to the fulfillment center",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "reporting-date": {
-            "format": "date-time",
-            "type": "string"
-        },
-        "ship-city": {
+        "primary-action": {
+            "description": "Primary action to be taken for the inventory",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ship-country": {
+        "product-name": {
+            "description": "Name of the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ship-postal-code": {
+        "reserved-quantity": {
+            "description": "Quantity of the product that is reserved",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ship-promotion-discount": {
+        "sku": {
+            "description": "Stock Keeping Unit (SKU) of the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ship-service-level": {
+        "status-primary": {
+            "description": "Primary status of the inventory",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ship-state": {
+        "status-secondary": {
+            "description": "Secondary status of the inventory",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "shipping-price": {
+        "stranded-reason": {
+            "description": "Reason why the inventory is stranded",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "shipping-tax": {
+        "unfulfillable-qty": {
+            "description": "Quantity of the product that is unfulfillable",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "sku": {
+        "your-price": {
+            "description": "Price set for the product by the seller",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "title": "Flat File All Orders Data Reports (by last update)",
+    "title": "FBA Stranded Inventory Report",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9753472222222221%*

 * *Differences: {"'properties'": "{'sku': {'description': 'Stock Keeping Unit code for the product'}, 'asin': "*

 * *                 "{'description': 'Amazon Standard Identification Number for the product'}, "*

 * *                 "'price': {'description': 'Current price of the product'}, 'quantity': "*

 * *                 "{'description': 'Available quantity of the product'}, 'Business Price': "*

 * *                 "{'description': 'The price set by the business for the listing'}, 'Quantity "*

 * *                 "Price Type': {'description […]*

```diff
@@ -1,151 +1,175 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "description": "Flat File Open Listings Data Reports",
     "properties": {
         "Business Price": {
+            "description": "The price set by the business for the listing",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Progressive Lower Bound 1": {
+            "description": "Minimum threshold for progressive pricing tier 1",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Progressive Lower Bound 2": {
+            "description": "Minimum threshold for progressive pricing tier 2",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Progressive Lower Bound 3": {
+            "description": "Minimum threshold for progressive pricing tier 3",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Progressive Price 1": {
+            "description": "Price for products in progressive tier 1",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Progressive Price 2": {
+            "description": "Price for products in progressive tier 2",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Progressive Price 3": {
+            "description": "Price for products in progressive tier 3",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Progressive Price Type": {
+            "description": "Type of pricing strategy used for progressive pricing",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Quantity Lower Bound 1": {
+            "description": "Minimum quantity threshold for pricing tier 1",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Quantity Lower Bound 2": {
+            "description": "Minimum quantity threshold for pricing tier 2",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Quantity Lower Bound 3": {
+            "description": "Minimum quantity threshold for pricing tier 3",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Quantity Lower Bound 4": {
+            "description": "Minimum quantity threshold for pricing tier 4",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Quantity Lower Bound 5": {
+            "description": "Minimum quantity threshold for pricing tier 5",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Quantity Price 1": {
+            "description": "Price for products in quantity tier 1",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Quantity Price 2": {
+            "description": "Price for products in quantity tier 2",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Quantity Price 3": {
+            "description": "Price for products in quantity tier 3",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Quantity Price 4": {
+            "description": "Price for products in quantity tier 4",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Quantity Price 5": {
+            "description": "Price for products in quantity tier 5",
             "type": [
                 "null",
                 "string"
             ]
         },
         "Quantity Price Type": {
+            "description": "Type of pricing strategy used for quantity pricing",
             "type": [
                 "null",
                 "string"
             ]
         },
         "asin": {
+            "description": "Amazon Standard Identification Number for the product",
             "type": [
                 "null",
                 "string"
             ]
         },
         "dataEndTime": {
+            "description": "End time of the data entry",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
         "price": {
+            "description": "Current price of the product",
             "type": [
                 "null",
                 "string"
             ]
         },
         "quantity": {
+            "description": "Available quantity of the product",
             "type": [
                 "null",
                 "string"
             ]
         },
         "sku": {
+            "description": "Stock Keeping Unit code for the product",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "title": "Flat File Open Listings Data",
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7056910569105691%*

 * *Differences: {"'description'": "'FBA customer returns report Data Reports'",*

 * * "'properties'": "{'quantity': {'description': 'The quantity of the item returned'}, 'status': "*

 * *                 "{'description': 'The status of the return process'}, 'dataEndTime': "*

 * *                 "{'description': 'The end date and time of the data record'}, 'return-date': "*

 * *                 "OrderedDict([('description', 'The date and time when the return was initiated'), "*

 * *                 "('type', ['null', 'string']), ('format', 'date-t […]*

```diff
@@ -1,190 +1,108 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "Get Merchant Listings All Data Reports",
+    "description": "FBA customer returns report Data Reports",
     "properties": {
-        "add-delete": {
+        "asin": {
+            "description": "The Amazon Standard Identification Number of the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "asin1": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "asin2": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "asin3": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "bid-for-featured-placement": {
+        "customer-comments": {
+            "description": "Comments provided by the customer regarding the return",
             "type": [
                 "null",
                 "string"
             ]
         },
         "dataEndTime": {
+            "description": "The end date and time of the data record",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "expedited-shipping": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "fulfillment-channel": {
+        "detailed-disposition": {
+            "description": "Detailed description of the disposition of the returned item",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "image-url": {
+        "fnsku": {
+            "description": "Fulfillment Network Stock Keeping Unit of the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "item-condition": {
+        "fulfillment-center-id": {
+            "description": "Identification of the fulfillment center where the return was processed",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "item-description": {
+        "license-plate-number": {
+            "description": "The unique identifier of the license plate associated with the return",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "item-is-marketplace": {
+        "order-id": {
+            "description": "The unique identifier of the order associated with the return",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "item-name": {
+        "product-name": {
+            "description": "The name of the product returned by the customer",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "item-note": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "listing-id": {
+        "quantity": {
+            "description": "The quantity of the item returned",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "merchant-shipping-group": {
+        "reason": {
+            "description": "The reason provided for the return by the customer",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "open-date": {
+        "return-date": {
+            "description": "The date and time when the return was initiated",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "pending-quantity": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "price": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "product-id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "product-id-type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "quantity": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "seller-sku": {
+        "sku": {
+            "description": "Stock Keeping Unit of the product",
             "type": [
                 "null",
                 "string"
             ]
         },
         "status": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "will-ship-internationally": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "zshop-boldface": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "zshop-browse-path": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "zshop-category1": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "zshop-shipping-fee": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "zshop-storefront-feature": {
+            "description": "The status of the return process",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "title": "Get Merchant Listings Reports",
+    "title": "FBA customer returns",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7019841269841269%*

 * *Differences: {"'description'": "'Flat File All Orders Data by Order Date General Reports'",*

 * * "'properties'": "{'dataEndTime': {'description': 'End timestamp of the data'}, 'amazon-order-id': "*

 * *                 "OrderedDict([('description', 'Unique identifier for the order on Amazon "*

 * *                 "platform'), ('type', ['null', 'string'])]), 'merchant-order-id': "*

 * *                 "OrderedDict([('description', 'Identifier for the order set by the merchant'), "*

 * *                 "('type', ['null', 'string'])]), 'purcha […]*

```diff
@@ -1,342 +1,249 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "GET_ORDER_REPORT_DATA_SHIPPING",
+    "description": "Flat File All Orders Data by Order Date General Reports",
     "properties": {
-        "AmazonOrderID": {
+        "amazon-order-id": {
+            "description": "Unique identifier for the order on Amazon platform",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AmazonSessionID": {
+        "asin": {
+            "description": "Amazon Standard Identification Number for the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "BillingData": {
-            "additionalProperties": true,
-            "properties": {
-                "BuyerEmailAddress": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "BuyerName": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "BuyerPhoneNumber": {
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
-        "FulfillmentData": {
-            "additionalProperties": true,
-            "properties": {
-                "Address": {
-                    "additionalProperties": true,
-                    "properties": {
-                        "AddressFieldOne": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "City": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "CountryCode": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "Name": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "PhoneNumber": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "PostalCode": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "StateOrRegion": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "FulfillmentMethod": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "FulfillmentServiceLevel": {
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
-        "IsBusinessOrder": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Item": {
-            "additionalProperties": true,
-            "properties": {
-                "AmazonOrderItemCode": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "ItemFees": {
-                    "additionalProperties": true,
-                    "properties": {
-                        "Fee": {
-                            "additionalProperties": true,
-                            "properties": {
-                                "Amount": {
-                                    "additionalProperties": true,
-                                    "properties": {
-                                        "currency": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        },
-                                        "value": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                },
-                                "Type": {
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
-                "ItemPrice": {
-                    "additionalProperties": true,
-                    "properties": {
-                        "Component": {
-                            "items": {
-                                "type": [
-                                    "null",
-                                    "object"
-                                ]
-                            },
-                            "properties": {
-                                "Amount": {
-                                    "additionalProperties": true,
-                                    "properties": {
-                                        "currency": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        },
-                                        "value": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                },
-                                "Type": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "array"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "ProductTaxCode": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "Promotion": {
-                    "additionalProperties": true,
-                    "properties": {
-                        "Component": {
-                            "additionalProperties": true,
-                            "properties": {
-                                "Amount": {
-                                    "additionalProperties": true,
-                                    "properties": {
-                                        "currency": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        },
-                                        "value": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                },
-                                "Type": {
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
-                        },
-                        "MerchantPromotionID": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "PromotionClaimCode": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "Quantity": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "SKU": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "SignatureConfirmationRecommended": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "Title": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "cpf": {
+            "description": "Cadastro de Pessoas F\u00edsicas - Brazilian individual taxpayer registry identification number",
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "OrderDate": {
-            "format": "date",
+        "currency": {
+            "description": "Currency used for the order",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "OrderPostedDate": {
+        "dataEndTime": {
+            "description": "End timestamp of the data",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "dataEndTime": {
-            "format": "date",
+        "fulfillment-channel": {
+            "description": "Channel through which the order is fulfilled (e.g., FBA, Seller Fulfilled)",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "gift-wrap-price": {
+            "description": "Price of gift wrapping for the order",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "gift-wrap-tax": {
+            "description": "Tax applied on the gift wrapping price",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "is-business-order": {
+            "description": "Indicator if the order is a business order",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "item-price": {
+            "description": "Price of each item in the order",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "item-promotion-discount": {
+            "description": "Discount applied on the item price due to promotion",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "item-status": {
+            "description": "Status of the item in the order",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "item-tax": {
+            "description": "Tax charged on the item price",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "last-updated-date": {
+            "description": "Timestamp of the last update for the order",
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "merchant-order-id": {
+            "description": "Identifier for the order set by the merchant",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "order-channel": {
+            "description": "Channel through which the order was placed",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "order-status": {
+            "description": "Status of the order (e.g., Pending, Shipped)",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "price-designation": {
+            "description": "Price designation for the order (e.g., Regular price, Discounted price)",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "product-name": {
+            "description": "Name of the product in the order",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "promotion-ids": {
+            "description": "Identifiers for promotions applied to the order",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "purchase-date": {
+            "description": "Timestamp of the order purchase date",
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "purchase-order-number": {
+            "description": "Number associated with the order for purchase tracking",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "quantity": {
+            "description": "Number of units ordered",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "sales-channel": {
+            "description": "Channel through which the sale was made",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "ship-city": {
+            "description": "City to which the order is being shipped",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "ship-country": {
+            "description": "Country to which the order is being shipped",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "ship-postal-code": {
+            "description": "Postal code of the shipping address",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "ship-promotion-discount": {
+            "description": "Discount applied to the shipping cost due to promotions",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "ship-service-level": {
+            "description": "Service level of shipping (e.g., Standard, Expedited)",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "ship-state": {
+            "description": "State to which the order is being shipped",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "shipping-price": {
+            "description": "Price of shipping for the order",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "shipping-tax": {
+            "description": "Tax applied on the shipping price",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "signature-confirmation-recommended": {
+            "description": "Indicator if signature confirmation is recommended for the order",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "sku": {
+            "description": "Stock Keeping Unit for the product in the order",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "title": "GET_ORDER_REPORT_DATA_SHIPPING",
+    "title": "Flat File All Orders Data Reports",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7020833333333333%*

 * *Differences: {"'description'": "'Brand Analytics Repeat Purchase Reports'",*

 * * "'properties'": "{'dataEndTime': {'description': 'The end time of the data collection period in "*

 * *                 "date format.'}, 'startDate': OrderedDict([('description', 'The start date of the "*

 * *                 "data collection period in date format.'), ('type', ['null', 'string']), "*

 * *                 "('format', 'date')]), 'endDate': OrderedDict([('description', 'The end date of "*

 * *                 "the data collection period in date forma […]*

```diff
@@ -1,195 +1,95 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "Restock Inventory Report",
+    "description": "Brand Analytics Repeat Purchase Reports",
     "properties": {
-        "ASIN": {
+        "asin": {
+            "description": "The unique identifier for the ASIN (Amazon Standard Identification Number).",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "Alert": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Available": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Condition": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Country": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Currency code": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Customer Order": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Days of Supply at Amazon Fulfillment Network": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "FC Processing": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "FC transfer": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "FNSKU": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Fulfilled by": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Inbound": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Merchant SKU": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Price": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Product Name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Receiving": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Recommended action": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Recommended replenishment qty": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Recommended ship date": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Sales last 30 days": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Shipped": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Supplier": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "Supplier part no.": {
+        "dataEndTime": {
+            "description": "The end time of the data collection period in date format.",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "Total Days of Supply (including units from open shipments)": {
+        "endDate": {
+            "description": "The end date of the data collection period in date format.",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "Total Units": {
+        "orders": {
+            "description": "The total number of orders placed during the specified time period.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "Unfulfillable": {
+        "queryEndDate": {
+            "description": "The end date of the query period for data analysis in date format.",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "Unit storage size": {
+        "repeatCustomersPctTotal": {
+            "description": "The percentage of repeat customers out of the total customers.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "Units Sold Last 30 Days": {
+        "repeatPurchaseRevenue": {
+            "description": "The revenue generated from repeat purchases.",
+            "properties": {
+                "amount": {
+                    "description": "The amount of repeat purchase revenue.",
+                    "type": [
+                        "null",
+                        "number"
+                    ]
+                },
+                "currencyCode": {
+                    "description": "The currency code (e.g., USD) for the repeat purchase revenue amount.",
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": "object"
+        },
+        "repeatPurchaseRevenuePctTotal": {
+            "description": "The percentage of repeat purchase revenue out of the total revenue.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "Working": {
+        "startDate": {
+            "description": "The start date of the data collection period in date format.",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "dataEndTime": {
-            "format": "date",
+        "uniqueCustomers": {
+            "description": "The total number of unique customers who made purchases during the specified time period.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         }
     },
-    "title": "Restock Inventory Report",
+    "title": "Brand Analytics Repeat Purchase Reports",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7055555555555555%*

 * *Differences: {"'description'": "''",*

 * * "'properties'": "{'dataEndTime': {'description': 'End time of the report data'}, 'Status': "*

 * *                 "OrderedDict([('description', 'Current status of the listing (Active, Inactive, "*

 * *                 "Under Review, etc.)'), ('type', ['null', 'string'])]), 'Reason': "*

 * *                 "OrderedDict([('description', 'Reason for the listing status change or issue'), "*

 * *                 "('type', ['null', 'string'])]), 'SKU': OrderedDict([('description', 'Stock "*

 * *                 […]*

```diff
@@ -1,52 +1,73 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "Seller Feedback Data Reports",
+    "description": "",
     "properties": {
-        "comments": {
+        "ASIN": {
+            "description": "Unique Amazon Standard Identification Number for the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "dataEndTime": {
-            "format": "date",
+        "Condition": {
+            "description": "Condition of the product (New, Used, Refurbished, etc.)",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "date": {
-            "format": "date",
+        "Issue Description": {
+            "description": "Description of any issues with the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "order_id": {
+        "Product name": {
+            "description": "Name of the product listed",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "rater_email": {
+        "Reason": {
+            "description": "Reason for the listing status change or issue",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "rating": {
+        "SKU": {
+            "description": "Stock Keeping Unit for the product",
             "type": [
                 "null",
-                "number"
+                "string"
+            ]
+        },
+        "Status": {
+            "description": "Current status of the listing (Active, Inactive, Under Review, etc.)",
+            "type": [
+                "null",
+                "string"
             ]
         },
-        "response": {
+        "Status Change Date": {
+            "description": "Date when the status of the listing was last changed",
+            "format": "date",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "dataEndTime": {
+            "description": "End time of the report data",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "title": "Seller Feedback Data Reports",
+    "title": "Suppressed Listings Report",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.71875%*

 * *Differences: {"'description'": '"This report shares data on the customer traffic to the detail pages of the '*

 * *                  "vendor's items both at an aggregated level (across the vendor's entire catalog "*

 * *                  'of items) and at a per-ASIN level. Data is available for different date range '*

 * *                  'aggregation levels: DAY, WEEK, MONTH, QUARTER, YEAR. Requests can span multiple '*

 * *                  'date range periods."',*

 * * "'properties'": "{'startDate': {'format': 'date', 'description': 'The da […]*

```diff
@@ -1,97 +1,54 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "Vendor Sales Reports",
+    "description": "This report shares data on the customer traffic to the detail pages of the vendor's items both at an aggregated level (across the vendor's entire catalog of items) and at a per-ASIN level. Data is available for different date range aggregation levels: DAY, WEEK, MONTH, QUARTER, YEAR. Requests can span multiple date range periods.",
     "properties": {
         "asin": {
+            "description": "Unique identifier for the Amazon Standard Identification Number",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "customerReturns": {
+        "dataEndTime": {
+            "description": "The timestamp indicating the end time of the data collection",
+            "format": "date",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
         "endDate": {
-            "format": "date-time",
+            "description": "The date when the data collection ended",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "orderedRevenue": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "null",
-                        "number"
-                    ]
-                },
-                "currencyCode": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": "object"
-        },
-        "orderedUnits": {
+        "glanceViews": {
+            "description": "Total number of quick views on the product",
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
-        "shippedCogs": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "null",
-                        "number"
-                    ]
-                },
-                "currencyCode": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": "object"
-        },
-        "shippedRevenue": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "null",
-                        "number"
-                    ]
-                },
-                "currencyCode": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
-            "type": "object"
-        },
-        "shippedUnits": {
+        "queryEndDate": {
+            "description": "The date when the query for data collection ended",
+            "format": "date",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
         "startDate": {
-            "format": "date-time",
+            "description": "The date when the data collection started",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "title": "Vendor Sales Reports",
+    "title": "Vendor Traffic Report",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6043859649122807%*

 * *Differences: {"'description'": "'Brand Analytics Search Terms Reports'",*

 * * "'properties'": "{'dataEndTime': {'description': 'The end time of the data collection period for "*

 * *                 "this report.'}, 'departmentName': OrderedDict([('description', 'The name of the "*

 * *                 "department or category associated with the search term.'), ('type', ['null', "*

 * *                 "'string'])]), 'searchTerm': OrderedDict([('description', 'The specific term or "*

 * *                 "keyword entered by users in search que […]*

```diff
@@ -1,172 +1,73 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
+    "description": "Brand Analytics Search Terms Reports",
     "properties": {
-        "browseNodeAttributes": {
-            "properties": {
-                "attribute": {
-                    "items": {
-                        "type": [
-                            "null",
-                            "object"
-                        ]
-                    },
-                    "properties": {
-                        "name": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "text": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "array"
-                    ]
-                },
-                "count": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "clickShare": {
+            "description": "The share of total clicks that this search term received out of all the clicks in the report period.",
             "type": [
                 "null",
-                "object"
+                "number"
             ]
         },
-        "browseNodeId": {
-            "type": [
-                "string"
-            ]
-        },
-        "browseNodeName": {
+        "clickShareRank": {
+            "description": "The ranking of this search term based on the click share it received.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "browseNodeStoreContextName": {
+        "clickedAsin": {
+            "description": "The ASIN (Amazon Standard Identification Number) that was clicked for this search term.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "browsePathById": {
+        "conversionShare": {
+            "description": "The share of total conversions attributed to this search term out of all conversions in the report period.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "browsePathByName": {
+        "dataEndTime": {
+            "description": "The end time of the data collection period for this report.",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "childNodes": {
-            "properties": {
-                "count": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "id": {
-                    "items": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "type": [
-                        "array"
-                    ]
-                }
-            },
+        "departmentName": {
+            "description": "The name of the department or category associated with the search term.",
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "dataEndTime": {
+        "queryEndDate": {
+            "description": "The end date of the search term query.",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "hasChildren": {
-            "type": [
-                "string"
-            ]
-        },
-        "productTypeDefinitions": {
+        "searchFrequencyRank": {
+            "description": "The ranking of this search term based on its frequency of occurrence in search queries.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "refinementsInformation": {
-            "properties": {
-                "count": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "refinementName": {
-                    "properties": {
-                        "refinementField": {
-                            "properties": {
-                                "acceptedValues": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "hasModifier": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "modifiers": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "refinementAttribute": {
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
-                }
-            },
+        "searchTerm": {
+            "description": "The specific term or keyword entered by users in search queries.",
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         }
     },
-    "title": "XML Browse Tree Data",
+    "title": "Brand Analytics Search Terms Reports",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7%*

 * *Differences: {"'description'": "'Vendor Sales Reports'",*

 * * "'properties'": "{replace: OrderedDict([('startDate', OrderedDict([('description', 'The start "*

 * *                 "date and time for the sales report data.'), ('type', ['null', 'string']), "*

 * *                 "('format', 'date-time')])), ('endDate', OrderedDict([('description', 'The end "*

 * *                 "date and time for the sales report data.'), ('type', ['null', 'string']), "*

 * *                 "('format', 'date-time')])), ('asin', OrderedDict([('description', ' […]*

```diff
@@ -1,119 +1,112 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "List Financial Event Groups",
+    "description": "Vendor Sales Reports",
     "properties": {
-        "AccountTail": {
+        "asin": {
+            "description": "The unique Amazon Standard Identification Number for the product.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "BeginningBalance": {
+        "customerReturns": {
+            "description": "The number of units of the product that customers returned.",
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "endDate": {
+            "description": "The end date and time for the sales report data.",
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "orderedRevenue": {
+            "description": "The total revenue generated from customer orders.",
             "properties": {
-                "CurrencyAmount": {
+                "amount": {
+                    "description": "The revenue amount in the specified currency.",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
-                "CurrencyCode": {
+                "currencyCode": {
+                    "description": "The currency code for the revenue amount.",
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
+            "type": "object"
+        },
+        "orderedUnits": {
+            "description": "The total number of units of the product ordered by customers.",
             "type": [
                 "null",
-                "object"
+                "number"
             ]
         },
-        "ConvertedTotal": {
+        "shippedCogs": {
+            "description": "The cost of goods sold for the shipped units.",
             "properties": {
-                "CurrencyAmount": {
+                "amount": {
+                    "description": "The cost amount in the specified currency.",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
-                "CurrencyCode": {
+                "currencyCode": {
+                    "description": "The currency code for the cost amount.",
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "FinancialEventGroupEnd": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
+            "type": "object"
         },
-        "FinancialEventGroupId": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "FinancialEventGroupStart": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "FundTransferDate": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "FundTransferStatus": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "OriginalTotal": {
+        "shippedRevenue": {
+            "description": "The total revenue generated from the shipped units.",
             "properties": {
-                "CurrencyAmount": {
+                "amount": {
+                    "description": "The revenue amount in the specified currency.",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
-                "CurrencyCode": {
+                "currencyCode": {
+                    "description": "The currency code for the revenue amount.",
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
-            "type": [
-                "null",
-                "object"
-            ]
+            "type": "object"
         },
-        "ProcessingStatus": {
+        "shippedUnits": {
+            "description": "The total number of units of the product shipped to customers.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "TraceId": {
+        "startDate": {
+            "description": "The start date and time for the sales report data.",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "title": "ListFinancialEventGroups",
+    "title": "Vendor Sales Reports",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/OrderItems.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5833333333333334%*

 * *Differences: {"'description'": "'GET_ORDER_REPORT_DATA_SHIPPING'",*

 * * "'properties'": "{replace: OrderedDict([('AmazonOrderID', OrderedDict([('description', 'Unique "*

 * *                 "identifier for the Amazon order'), ('type', ['null', 'string'])])), "*

 * *                 "('AmazonSessionID', OrderedDict([('description', 'Unique identifier for the "*

 * *                 "Amazon session'), ('type', ['null', 'string'])])), ('OrderDate', "*

 * *                 "OrderedDict([('description', 'Date when the order was placed'), ('type',  […]*

```diff
@@ -1,516 +1,390 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "additionalProperties": true,
-    "description": "All order items that were updated after a specified date",
+    "description": "GET_ORDER_REPORT_DATA_SHIPPING",
     "properties": {
-        "ASIN": {
+        "AmazonOrderID": {
+            "description": "Unique identifier for the Amazon order",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AmazonOrderId": {
+        "AmazonSessionID": {
+            "description": "Unique identifier for the Amazon session",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "BuyerInfo": {
+        "BillingData": {
             "additionalProperties": true,
+            "description": "Data related to billing information",
             "properties": {
-                "BuyerCustomizedInfo": {
-                    "additionalProperties": true,
-                    "properties": {
-                        "CustomizedURL": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
+                "BuyerEmailAddress": {
+                    "description": "Email address of the buyer",
                     "type": [
                         "null",
-                        "object"
+                        "string"
                     ]
                 },
-                "GiftMessageText": {
+                "BuyerName": {
+                    "description": "Name of the buyer",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "GiftWrapLevel": {
+                "BuyerPhoneNumber": {
+                    "description": "Phone number of the buyer",
                     "type": [
                         "null",
                         "string"
                     ]
-                },
-                "GiftWrapPrice": {
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "FulfillmentData": {
+            "additionalProperties": true,
+            "description": "Data related to order fulfillment",
+            "properties": {
+                "Address": {
                     "additionalProperties": true,
+                    "description": "Shipping address details",
                     "properties": {
-                        "Amount": {
+                        "AddressFieldOne": {
+                            "description": "Address line 1",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "City": {
+                            "description": "City of the shipping address",
                             "type": [
                                 "null",
                                 "string"
                             ]
                         },
-                        "CurrencyCode": {
+                        "CountryCode": {
+                            "description": "Country code of the shipping address",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "Name": {
+                            "description": "Name associated with the address",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "PhoneNumber": {
+                            "description": "Phone number associated with the address",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "PostalCode": {
+                            "description": "Postal code of the shipping address",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "StateOrRegion": {
+                            "description": "State or region of the shipping address",
                             "type": [
                                 "null",
                                 "string"
                             ]
                         }
                     },
                     "type": [
                         "null",
                         "object"
                     ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "BuyerRequestedCancel": {
-            "additionalProperties": true,
-            "properties": {
-                "BuyerCancelReason": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
                 },
-                "IsBuyerRequestedCancel": {
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
-        "CODFee": {
-            "additionalProperties": true,
-            "properties": {
-                "Amount": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "CurrencyCode": {
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
-        "CODFeeDiscount": {
-            "additionalProperties": true,
-            "properties": {
-                "Amount": {
+                "FulfillmentMethod": {
+                    "description": "Method used for order fulfillment",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "CurrencyCode": {
+                "FulfillmentServiceLevel": {
+                    "description": "Service level for fulfillment",
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "ConditionId": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "ConditionNote": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "ConditionSubtypeId": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "DeemedResellerCategory": {
+        "IsBusinessOrder": {
+            "description": "Indicates if the order is a business order",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "IossNumber": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "IsGift": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "IsTransparency": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "ItemPrice": {
+        "Item": {
             "additionalProperties": true,
+            "description": "Details of the item ordered",
             "properties": {
-                "Amount": {
+                "AmazonOrderItemCode": {
+                    "description": "Unique identifier for the ordered item",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "CurrencyCode": {
+                "ItemFees": {
+                    "additionalProperties": true,
+                    "description": "Fees associated with the item",
+                    "properties": {
+                        "Fee": {
+                            "additionalProperties": true,
+                            "description": "Specific fee data",
+                            "properties": {
+                                "Amount": {
+                                    "additionalProperties": true,
+                                    "description": "Amount of the fee",
+                                    "properties": {
+                                        "currency": {
+                                            "description": "Currency type",
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "value": {
+                                            "description": "Value of the fee",
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        }
+                                    },
+                                    "type": [
+                                        "null",
+                                        "object"
+                                    ]
+                                },
+                                "Type": {
+                                    "description": "Type of fee",
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                }
+                            },
+                            "type": [
+                                "null",
+                                "object"
+                            ]
+                        }
+                    },
                     "type": [
                         "null",
-                        "string"
+                        "object"
                     ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "ItemTax": {
-            "additionalProperties": true,
-            "properties": {
-                "Amount": {
+                },
+                "ItemPrice": {
+                    "additionalProperties": true,
+                    "description": "Price details for the item",
+                    "properties": {
+                        "Component": {
+                            "description": "Price components for the item",
+                            "items": {
+                                "type": [
+                                    "null",
+                                    "object"
+                                ]
+                            },
+                            "properties": {
+                                "Amount": {
+                                    "additionalProperties": true,
+                                    "description": "Amount of the price component",
+                                    "properties": {
+                                        "currency": {
+                                            "description": "Currency type for the component",
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "value": {
+                                            "description": "Value of the price component",
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        }
+                                    },
+                                    "type": [
+                                        "null",
+                                        "object"
+                                    ]
+                                },
+                                "Type": {
+                                    "description": "Type of price component",
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                }
+                            },
+                            "type": [
+                                "array"
+                            ]
+                        }
+                    },
                     "type": [
                         "null",
-                        "string"
+                        "object"
                     ]
                 },
-                "CurrencyCode": {
+                "ProductTaxCode": {
+                    "description": "Tax code for the product",
                     "type": [
                         "null",
                         "string"
                     ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "LastUpdateDate": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "OrderItemId": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "PointsGranted": {
-            "additionalProperties": true,
-            "properties": {
-                "PointsMonetaryValue": {
+                },
+                "Promotion": {
                     "additionalProperties": true,
+                    "description": "Promotion details for the item",
                     "properties": {
-                        "Amount": {
+                        "Component": {
+                            "additionalProperties": true,
+                            "description": "Promotion amount and type",
+                            "properties": {
+                                "Amount": {
+                                    "additionalProperties": true,
+                                    "description": "Amount of the promotion",
+                                    "properties": {
+                                        "currency": {
+                                            "description": "Currency type",
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        },
+                                        "value": {
+                                            "description": "Value of the promotion",
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        }
+                                    },
+                                    "type": [
+                                        "null",
+                                        "object"
+                                    ]
+                                },
+                                "Type": {
+                                    "description": "Type of promotion",
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                }
+                            },
+                            "type": [
+                                "null",
+                                "object"
+                            ]
+                        },
+                        "MerchantPromotionID": {
+                            "description": "ID of the merchant promotion",
                             "type": [
                                 "null",
                                 "string"
                             ]
                         },
-                        "CurrencyCode": {
+                        "PromotionClaimCode": {
+                            "description": "Claim code for the promotion",
                             "type": [
                                 "null",
                                 "string"
                             ]
                         }
                     },
                     "type": [
                         "null",
                         "object"
                     ]
                 },
-                "PointsNumber": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "PriceDesignation": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "ProductInfo": {
-            "additionalProperties": true,
-            "properties": {
-                "NumberOfItems": {
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
-        "PromotionDiscount": {
-            "additionalProperties": true,
-            "properties": {
-                "Amount": {
+                "Quantity": {
+                    "description": "Quantity of the item ordered",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "CurrencyCode": {
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
-        "PromotionDiscountTax": {
-            "additionalProperties": true,
-            "properties": {
-                "Amount": {
+                "SKU": {
+                    "description": "Stock Keeping Unit (SKU) for the item",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "CurrencyCode": {
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
-        "PromotionIds": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "QuantityOrdered": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "QuantityShipped": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "ScheduledDeliveryEndDate": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "ScheduledDeliveryStartDate": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "SellerSKU": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "SerialNumberRequired": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "SerialNumbers": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "ShippingDiscount": {
-            "additionalProperties": true,
-            "properties": {
-                "Amount": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "CurrencyCode": {
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
-        "ShippingDiscountTax": {
-            "additionalProperties": true,
-            "properties": {
-                "Amount": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "CurrencyCode": {
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
-        "ShippingPrice": {
-            "additionalProperties": true,
-            "properties": {
-                "Amount": {
+                "SignatureConfirmationRecommended": {
+                    "description": "Indicates if signature confirmation is recommended",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "CurrencyCode": {
+                "Title": {
+                    "description": "Title of the item",
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "ShippingTax": {
-            "additionalProperties": true,
-            "properties": {
-                "Amount": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "CurrencyCode": {
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
-        "StoreChainStoreId": {
+        "OrderDate": {
+            "description": "Date when the order was placed",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "TaxCollection": {
-            "additionalProperties": true,
-            "properties": {
-                "Model": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "ResponsibleParty": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "OrderPostedDate": {
+            "description": "Date when the order was posted",
+            "format": "date",
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "Title": {
+        "dataEndTime": {
+            "description": "End time for the data",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "title": "Order Items",
+    "title": "GET_ORDER_REPORT_DATA_SHIPPING",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/Orders.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5833333333333334%*

 * *Differences: {"'description'": "''",*

 * * "'properties'": "{replace: OrderedDict([('amazon-order-id', OrderedDict([('description', 'The "*

 * *                 "unique identifier for the Amazon order'), ('type', ['null', 'string'])])), "*

 * *                 '(\'merchant-order-id\', OrderedDict([(\'description\', "The merchant\'s unique '*

 * *                 'identifier for the order"), (\'type\', [\'null\', \'string\'])])), '*

 * *                 "('purchase-date', OrderedDict([('description', 'The date and time when the order "*

 * *          […]*

```diff
@@ -1,313 +1,235 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "additionalProperties": true,
-    "description": "All orders that were updated after a specified date",
+    "description": "",
     "properties": {
-        "AmazonOrderId": {
+        "amazon-order-id": {
+            "description": "The unique identifier for the Amazon order",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AutomatedShippingSettings": {
-            "additionalProperties": true,
-            "properties": {
-                "HasAutomatedShippingSettings": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "BuyerInfo": {
-            "additionalProperties": true,
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "DefaultShipFromLocationAddress": {
-            "properties": {
-                "AddressLine1": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "City": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "CountryCode": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "Name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "PostalCode": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "StateOrRegion": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "asin": {
+            "description": "The Amazon Standard Identification Number for the product",
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "EarliestDeliveryDate": {
-            "airbyte_type": "timestamp_with_timezone",
-            "format": "date-time",
+        "currency": {
+            "description": "The currency used for the transaction",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "EarliestShipDate": {
-            "format": "date-time",
+        "dataEndTime": {
+            "description": "The end time of the data",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "FulfillmentChannel": {
+        "fulfillment-channel": {
+            "description": "The type of fulfillment channel",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "HasRegulatedItems": {
+        "gift-wrap-price": {
+            "description": "The price of gift wrapping",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "IsAccessPointOrder": {
+        "gift-wrap-tax": {
+            "description": "The tax applied to gift wrapping",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "IsBusinessOrder": {
+        "is-business-order": {
+            "description": "Indicates if the order is a business order",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "IsGlobalExpressEnabled": {
+        "is-replacement-order": {
+            "description": "Indicates if the order is a replacement order",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "IsISPU": {
+        "item-price": {
+            "description": "The price of the item",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "IsPremiumOrder": {
+        "item-promotion-discount": {
+            "description": "Discount applied to the item",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "IsPrime": {
+        "item-status": {
+            "description": "The status of the item",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "IsReplacementOrder": {
+        "item-tax": {
+            "description": "Tax applied to the item",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "IsSoldByAB": {
+        "last-updated-date": {
+            "description": "The date and time when the order was last updated",
+            "format": "date-time",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "LastUpdateDate": {
-            "format": "date-time",
+        "merchant-order-id": {
+            "description": "The merchant's unique identifier for the order",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "LatestDeliveryDate": {
-            "airbyte_type": "timestamp_with_timezone",
-            "format": "date-time",
+        "order-channel": {
+            "description": "The channel through which the order was placed",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "LatestShipDate": {
-            "format": "date-time",
+        "order-status": {
+            "description": "The status of the order",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "MarketplaceId": {
+        "price-designation": {
+            "description": "The designation of the price",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "NumberOfItemsShipped": {
+        "product-name": {
+            "description": "The name of the product",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "NumberOfItemsUnshipped": {
+        "promotion-ids": {
+            "description": "IDs of promotions applied",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "OrderStatus": {
+        "purchase-date": {
+            "description": "The date and time when the order was purchased",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "OrderTotal": {
-            "properties": {
-                "Amount": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "CurrencyCode": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "purchase-order-number": {
+            "description": "The purchase order number",
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "OrderType": {
+        "quantity": {
+            "description": "The quantity of the product",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "PaymentMethod": {
+        "sales-channel": {
+            "description": "The sales channel where the order was made",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "PaymentMethodDetails": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
+        "ship-country": {
+            "description": "The country where the item is to be shipped",
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "PurchaseDate": {
-            "format": "date-time",
+        "ship-promotion-discount": {
+            "description": "Discount applied to shipping",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "SalesChannel": {
+        "ship-promotion-id": {
+            "description": "ID of the shipping promotion",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "SellerOrderId": {
+        "ship-service-level": {
+            "description": "The service level for shipping",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ShipServiceLevel": {
+        "shipping-price": {
+            "description": "The price of shipping",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ShipmentServiceLevelCategory": {
+        "shipping-tax": {
+            "description": "Tax applied to shipping",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ShippingAddress": {
-            "properties": {
-                "City": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "CountryCode": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "PostalCode": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "StateOrRegion": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "sku": {
+            "description": "The stock keeping unit of the product",
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "seller_id": {
-            "title": "seller_id",
-            "type": "string"
+        "url": {
+            "description": "The URL of the product",
+            "type": [
+                "null",
+                "string"
+            ]
         }
     },
-    "title": "Orders",
+    "title": "Flat File Archived Orders Report",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7%*

 * *Differences: {"'description'": "''",*

 * * "'properties'": "{replace: OrderedDict([('item-name', OrderedDict([('description', 'The name of "*

 * *                 "the item'), ('type', ['null', 'string'])])), ('item-description', "*

 * *                 "OrderedDict([('description', 'Description of the item'), ('type', ['null', "*

 * *                 "'string'])])), ('listing-id', OrderedDict([('description', 'Unique identifier "*

 * *                 "for the listing'), ('type', ['null', 'string'])])), ('seller-sku', "*

 * *                 "Order […]*

```diff
@@ -1,459 +1,339 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "description": "Vendor Direct Fulfillment Shipping",
+    "description": "",
     "properties": {
-        "createdBefore": {
+        "Business Price": {
+            "description": "The price of the item for business customers",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Progressive Lower Bound 1": {
+            "description": "The lower boundary for a progressive pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Progressive Lower Bound 2": {
+            "description": "The second lower boundary for a progressive pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Progressive Lower Bound 3": {
+            "description": "The third lower boundary for a progressive pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Progressive Price 1": {
+            "description": "The price associated with the first progressive pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Progressive Price 2": {
+            "description": "The price associated with the second progressive pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Progressive Price 3": {
+            "description": "The price associated with the third progressive pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Progressive Price Type": {
+            "description": "The type of pricing for progressive pricing tiers",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Quantity Lower Bound 1": {
+            "description": "The lower boundary for the first quantity pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Quantity Lower Bound 2": {
+            "description": "The lower boundary for the second quantity pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Quantity Lower Bound 3": {
+            "description": "The lower boundary for the third quantity pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Quantity Lower Bound 4": {
+            "description": "The lower boundary for the fourth quantity pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Quantity Lower Bound 5": {
+            "description": "The lower boundary for the fifth quantity pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Quantity Price 1": {
+            "description": "The price associated with the first quantity pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Quantity Price 2": {
+            "description": "The price associated with the second quantity pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Quantity Price 3": {
+            "description": "The price associated with the third quantity pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Quantity Price 4": {
+            "description": "The price associated with the fourth quantity pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Quantity Price 5": {
+            "description": "The price associated with the fifth quantity pricing tier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "Quantity Price Type": {
+            "description": "The type of pricing for quantity pricing tiers",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "add-delete": {
+            "description": "Indicates if an item should be added or deleted",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "asin1": {
+            "description": "Unique identifier for the first ASIN",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "asin2": {
+            "description": "Unique identifier for the second ASIN",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "asin3": {
+            "description": "Unique identifier for the third ASIN",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "bid-for-featured-placement": {
+            "description": "Bidding information for featured placement",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "dataEndTime": {
+            "description": "The date when the data was last updated",
+            "format": "date",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "expedited-shipping": {
+            "description": "Indicates if expedited shipping is available",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "image-url": {
+            "description": "URL of the item's image",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "item-condition": {
+            "description": "The condition of the item",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "item-description": {
+            "description": "Description of the item",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "item-is-marketplace": {
+            "description": "Indicates if the item is listed on the marketplace",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "item-name": {
+            "description": "The name of the item",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "item-note": {
+            "description": "Additional notes related to the item",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "listing-id": {
+            "description": "Unique identifier for the listing",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "merchant-shipping-group": {
+            "description": "Grouping for merchant shipping preferences",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "open-date": {
+            "description": "The date and time when the listing was opened",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "labelData": {
-            "items": {
-                "properties": {
-                    "content": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "packageIdentifier": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "shipMethod": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "shipMethodName": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "trackingNumber": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "labelFormat": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "purchaseOrderNumber": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "sellingParty": {
-            "properties": {
-                "address": {
-                    "properties": {
-                        "addressLine1": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "addressLine2": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "addressLine3": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "city": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "countryCode": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "county": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "district": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "name": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "phone": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "postalCode": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "stateOrRegion": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "partyId": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "taxRegistrationDetails": {
-                    "items": {
-                        "properties": {
-                            "taxRegistrationAddress": {
-                                "properties": {
-                                    "addressLine1": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "addressLine2": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "addressLine3": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "city": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "countryCode": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "county": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "district": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "name": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "phone": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "postalCode": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "stateOrRegion": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    }
-                                },
-                                "type": [
-                                    "null",
-                                    "object"
-                                ]
-                            },
-                            "taxRegistrationMessages": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "taxRegistrationNumber": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "taxRegistrationType": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": [
-                            "null",
-                            "object"
-                        ]
-                    },
-                    "type": [
-                        "null",
-                        "array"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "shipFromParty": {
-            "properties": {
-                "address": {
-                    "properties": {
-                        "addressLine1": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "addressLine2": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "addressLine3": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "city": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "countryCode": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "county": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "district": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "name": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "phone": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "postalCode": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "stateOrRegion": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "partyId": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "taxRegistrationDetails": {
-                    "items": {
-                        "properties": {
-                            "taxRegistrationAddress": {
-                                "properties": {
-                                    "addressLine1": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "addressLine2": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "addressLine3": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "city": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "countryCode": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "county": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "district": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "name": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "phone": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "postalCode": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "stateOrRegion": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    }
-                                },
-                                "type": [
-                                    "null",
-                                    "object"
-                                ]
-                            },
-                            "taxRegistrationMessages": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "taxRegistrationNumber": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "taxRegistrationType": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": [
-                            "null",
-                            "object"
-                        ]
-                    },
-                    "type": [
-                        "null",
-                        "array"
-                    ]
-                }
-            },
+        "pending-quantity": {
+            "description": "Quantity pending fulfillment",
             "type": [
                 "null",
-                "object"
+                "string"
+            ]
+        },
+        "price": {
+            "description": "The price of the item",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "product-id": {
+            "description": "Unique identifier for the product",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "product-id-type": {
+            "description": "Type of product identifier",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "quantity": {
+            "description": "Available quantity of the item",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "seller-sku": {
+            "description": "Seller-specific SKU for the item",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "will-ship-internationally": {
+            "description": "Indicates if the item will ship internationally",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "zshop-boldface": {
+            "description": "Indicates if the item is displayed in boldface",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "zshop-browse-path": {
+            "description": "Browse path on the Zshop",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "zshop-category1": {
+            "description": "Category of the item on Zshop",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "zshop-shipping-fee": {
+            "description": "Shipping fee on Zshop",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "zshop-storefront-feature": {
+            "description": "Feature on the Zshop storefront",
+            "type": [
+                "null",
+                "string"
             ]
         }
     },
-    "title": "Vendor Direct Fulfillment Shipping",
+    "title": "Open Listings Report",
     "type": "object"
 }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/source.py` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/spec.json` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/streams.py` & `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.1/PKG-INFO` & `airbyte_source_amazon_seller_partner-4.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-amazon-seller-partner
-Version: 4.2.1
+Version: 4.2.2
 Summary: Source implementation for Amazon Seller Partner.
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
+Requires-Dist: airbyte-cdk (==0.80.0)
 Requires-Dist: dateparser (==1.2.0)
 Requires-Dist: xmltodict (>=0.12,<1.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/amazon-seller-partner
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Amazon Seller Partner Source
```

