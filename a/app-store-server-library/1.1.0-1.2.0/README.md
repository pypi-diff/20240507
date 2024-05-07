# Comparing `tmp/app-store-server-library-1.1.0.tar.gz` & `tmp/app_store_server_library-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app-store-server-library-1.1.0.tar", last modified: Sat Mar 16 01:02:21 2024, max compression
+gzip compressed data, was "app_store_server_library-1.2.0.tar", last modified: Tue May  7 05:12:03 2024, max compression
```

## Comparing `app-store-server-library-1.1.0.tar` & `app_store_server_library-1.2.0.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:02:21.826027 app-store-server-library-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    37755 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-03-16 01:02:21.826027 app-store-server-library-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:02:21.826027 app-store-server-library-1.1.0/app_store_server_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-03-16 01:02:21.000000 app-store-server-library-1.1.0/app_store_server_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-03-16 01:02:21.000000 app-store-server-library-1.1.0/app_store_server_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 01:02:21.000000 app-store-server-library-1.1.0/app_store_server_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-16 01:02:21.000000 app-store-server-library-1.1.0/app_store_server_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-16 01:02:21.000000 app-store-server-library-1.1.0/app_store_server_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:02:21.814027 app-store-server-library-1.1.0/appstoreserverlibrary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31162 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:02:21.826027 app-store-server-library-1.1.0/appstoreserverlibrary/models/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/AccountTenure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/AppTransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/AutoRenewStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/CheckTestNotificationResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/ConsumptionRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/ConsumptionStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/Data.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/DeliveryStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/Environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/ExpirationIntent.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/ExtendReasonCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/ExtendRenewalDateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/ExtendRenewalDateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/ExternalPurchaseToken.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/FirstSendAttemptResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/HistoryResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/InAppOwnershipType.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/JWSRenewalInfoDecodedPayload.py
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/JWSTransactionDecodedPayload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/LastTransactionsItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/LibraryUtility.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/LifetimeDollarsPurchased.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/LifetimeDollarsRefunded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/MassExtendRenewalDateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/MassExtendRenewalDateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/MassExtendRenewalDateStatusResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/NotificationHistoryRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/NotificationHistoryResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/NotificationHistoryResponseItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/NotificationTypeV2.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/OfferDiscountType.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/OfferType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/OrderLookupResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/OrderLookupStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/Platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/PlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/PriceIncreaseStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/RefundHistoryResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/ResponseBodyV2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/ResponseBodyV2DecodedPayload.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/RevocationReason.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/SendAttemptItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/SendAttemptResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/SendTestNotificationResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/Status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/StatusResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/SubscriptionGroupIdentifierItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/Subtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/Summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/TransactionHistoryRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/TransactionInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/TransactionReason.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/Type.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/UserStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/promotional_offer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/receipt_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    16845 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/appstoreserverlibrary/signed_data_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 01:02:21.826027 app-store-server-library-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:02:21.826027 app-store-server-library-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    28124 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/tests/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/tests/test_decoded_payloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/tests/test_payload_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/tests/test_promotional_offer_signature_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/tests/test_receipt_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/tests/test_x509_verifiction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-03-16 01:02:11.000000 app-store-server-library-1.1.0/tests/test_xcode_signed_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:03.635512 app_store_server_library-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    37755 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-07 05:12:03.635512 app_store_server_library-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:03.635512 app_store_server_library-1.2.0/app_store_server_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-07 05:12:03.000000 app_store_server_library-1.2.0/app_store_server_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-07 05:12:03.000000 app_store_server_library-1.2.0/app_store_server_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 05:12:03.000000 app_store_server_library-1.2.0/app_store_server_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 05:12:03.000000 app_store_server_library-1.2.0/app_store_server_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 05:12:03.000000 app_store_server_library-1.2.0/app_store_server_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:03.623512 app_store_server_library-1.2.0/appstoreserverlibrary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31918 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:03.631512 app_store_server_library-1.2.0/appstoreserverlibrary/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/AccountTenure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/AppTransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/AutoRenewStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/CheckTestNotificationResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ConsumptionRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ConsumptionRequestReason.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ConsumptionStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/DeliveryStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ExpirationIntent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ExtendReasonCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ExtendRenewalDateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ExtendRenewalDateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ExternalPurchaseToken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/FirstSendAttemptResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/HistoryResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/InAppOwnershipType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/JWSRenewalInfoDecodedPayload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8372 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/JWSTransactionDecodedPayload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/LastTransactionsItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/LibraryUtility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/LifetimeDollarsPurchased.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/LifetimeDollarsRefunded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/MassExtendRenewalDateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/MassExtendRenewalDateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/MassExtendRenewalDateStatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationHistoryRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationHistoryResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationHistoryResponseItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationTypeV2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/OfferDiscountType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/OfferType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/OrderLookupResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/OrderLookupStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/PlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/PriceIncreaseStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/RefundHistoryResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/RefundPreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ResponseBodyV2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/ResponseBodyV2DecodedPayload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/RevocationReason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/SendAttemptItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/SendAttemptResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/SendTestNotificationResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/StatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/SubscriptionGroupIdentifierItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Subtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/TransactionHistoryRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/TransactionInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/TransactionReason.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/Type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/UserStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/promotional_offer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/receipt_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/appstoreserverlibrary/signed_data_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 05:12:03.635512 app_store_server_library-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:12:03.635512 app_store_server_library-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    28548 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16096 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_decoded_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_payload_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_promotional_offer_signature_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_receipt_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_x509_verifiction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-07 05:12:00.000000 app_store_server_library-1.2.0/tests/test_xcode_signed_data.py
```

### Comparing `app-store-server-library-1.1.0/LICENSE.txt` & `app_store_server_library-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/NOTICE.txt` & `app_store_server_library-1.2.0/NOTICE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 _____________________
 
-requests contirbutors (requests)
+requests contributors (requests)
 
              Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `app-store-server-library-1.1.0/PKG-INFO` & `app_store_server_library-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: app-store-server-library
-Version: 1.1.0
+Version: 1.2.0
 Summary: The App Store Server Library
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: PyJWT<3,>=2.6.0
 Requires-Dist: requests<3,>=2.28.0
@@ -35,24 +37,32 @@
 ```
 
 ## Documentation
 
 [Documentation](https://apple.github.io/app-store-server-library-python/)
 
 [WWDC Video](https://developer.apple.com/videos/play/wwdc2023/10143/)
+
+### Obtaining an In-App Purchase key from App Store Connect
+
+To use the App Store Server API or create promotional offer signatures, a signing key downloaded from App Store Connect is required. To obtain this key, you must have the Admin role. Go to Users and Access > Integrations > In-App Purchase. Here you can create and manage keys, as well as find your issuer ID. When using a key, you'll need the key ID and issuer ID as well.
+
+### Obtaining Apple Root Certificates
+
+Download and store the root certificates found in the Apple Root Certificates section of the [Apple PKI](https://www.apple.com/certificateauthority/) site. Provide these certificates as an array to a SignedDataVerifier to allow verifying the signed data comes from Apple.
+
 ## Usage
 
 ### API Usage
 
 ```python
 from appstoreserverlibrary.api_client import AppStoreServerAPIClient, APIException
 from appstoreserverlibrary.models.Environment import Environment
-from appstoreserverlibrary.models.SendTestNotificationResponse import SendTestNotificationResponse
 
-private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implemenation will vary
+private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implementation will vary
 
 key_id = "ABCDEFGHIJ"
 issuer_id = "99b16628-15e4-4668-972b-eeff55eeff55"
 bundle_id = "com.example"
 environment = Environment.SANDBOX
 
 client = AppStoreServerAPIClient(private_key, key_id, issuer_id, bundle_id, environment)
@@ -90,15 +100,15 @@
 ```python
 from appstoreserverlibrary.api_client import AppStoreServerAPIClient, APIException
 from appstoreserverlibrary.models.Environment import Environment
 from appstoreserverlibrary.receipt_utility import ReceiptUtility
 from appstoreserverlibrary.models.HistoryResponse import HistoryResponse
 from appstoreserverlibrary.models.TransactionHistoryRequest import TransactionHistoryRequest, ProductType, Order
 
-private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implemenation will vary
+private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implementation will vary
 
 key_id = "ABCDEFGHIJ"
 issuer_id = "99b16628-15e4-4668-972b-eeff55eeff55"
 bundle_id = "com.example"
 environment = Environment.SANDBOX
 
 client = AppStoreServerAPIClient(private_key, key_id, issuer_id, bundle_id, environment)
@@ -128,15 +138,15 @@
 
 ### Promotional Offer Signature Creation
 
 ```python
 from appstoreserverlibrary.promotional_offer import PromotionalOfferSignatureCreator
 import time
 
-private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implemenation will vary
+private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implementation will vary
 
 key_id = "ABCDEFGHIJ"
 bundle_id = "com.example"
 
 promotion_code_signature_generator = PromotionalOfferSignatureCreator(private_key, key_id, bundle_id)
 
 product_id = "<product_id>"
```

### Comparing `app-store-server-library-1.1.0/README.md` & `app_store_server_library-1.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -19,24 +19,32 @@
 ```
 
 ## Documentation
 
 [Documentation](https://apple.github.io/app-store-server-library-python/)
 
 [WWDC Video](https://developer.apple.com/videos/play/wwdc2023/10143/)
+
+### Obtaining an In-App Purchase key from App Store Connect
+
+To use the App Store Server API or create promotional offer signatures, a signing key downloaded from App Store Connect is required. To obtain this key, you must have the Admin role. Go to Users and Access > Integrations > In-App Purchase. Here you can create and manage keys, as well as find your issuer ID. When using a key, you'll need the key ID and issuer ID as well.
+
+### Obtaining Apple Root Certificates
+
+Download and store the root certificates found in the Apple Root Certificates section of the [Apple PKI](https://www.apple.com/certificateauthority/) site. Provide these certificates as an array to a SignedDataVerifier to allow verifying the signed data comes from Apple.
+
 ## Usage
 
 ### API Usage
 
 ```python
 from appstoreserverlibrary.api_client import AppStoreServerAPIClient, APIException
 from appstoreserverlibrary.models.Environment import Environment
-from appstoreserverlibrary.models.SendTestNotificationResponse import SendTestNotificationResponse
 
-private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implemenation will vary
+private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implementation will vary
 
 key_id = "ABCDEFGHIJ"
 issuer_id = "99b16628-15e4-4668-972b-eeff55eeff55"
 bundle_id = "com.example"
 environment = Environment.SANDBOX
 
 client = AppStoreServerAPIClient(private_key, key_id, issuer_id, bundle_id, environment)
@@ -74,15 +82,15 @@
 ```python
 from appstoreserverlibrary.api_client import AppStoreServerAPIClient, APIException
 from appstoreserverlibrary.models.Environment import Environment
 from appstoreserverlibrary.receipt_utility import ReceiptUtility
 from appstoreserverlibrary.models.HistoryResponse import HistoryResponse
 from appstoreserverlibrary.models.TransactionHistoryRequest import TransactionHistoryRequest, ProductType, Order
 
-private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implemenation will vary
+private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implementation will vary
 
 key_id = "ABCDEFGHIJ"
 issuer_id = "99b16628-15e4-4668-972b-eeff55eeff55"
 bundle_id = "com.example"
 environment = Environment.SANDBOX
 
 client = AppStoreServerAPIClient(private_key, key_id, issuer_id, bundle_id, environment)
@@ -112,15 +120,15 @@
 
 ### Promotional Offer Signature Creation
 
 ```python
 from appstoreserverlibrary.promotional_offer import PromotionalOfferSignatureCreator
 import time
 
-private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implemenation will vary
+private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implementation will vary
 
 key_id = "ABCDEFGHIJ"
 bundle_id = "com.example"
 
 promotion_code_signature_generator = PromotionalOfferSignatureCreator(private_key, key_id, bundle_id)
 
 product_id = "<product_id>"
```

### Comparing `app-store-server-library-1.1.0/app_store_server_library.egg-info/PKG-INFO` & `app_store_server_library-1.2.0/app_store_server_library.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: app-store-server-library
-Version: 1.1.0
+Version: 1.2.0
 Summary: The App Store Server Library
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: PyJWT<3,>=2.6.0
 Requires-Dist: requests<3,>=2.28.0
@@ -35,24 +37,32 @@
 ```
 
 ## Documentation
 
 [Documentation](https://apple.github.io/app-store-server-library-python/)
 
 [WWDC Video](https://developer.apple.com/videos/play/wwdc2023/10143/)
+
+### Obtaining an In-App Purchase key from App Store Connect
+
+To use the App Store Server API or create promotional offer signatures, a signing key downloaded from App Store Connect is required. To obtain this key, you must have the Admin role. Go to Users and Access > Integrations > In-App Purchase. Here you can create and manage keys, as well as find your issuer ID. When using a key, you'll need the key ID and issuer ID as well.
+
+### Obtaining Apple Root Certificates
+
+Download and store the root certificates found in the Apple Root Certificates section of the [Apple PKI](https://www.apple.com/certificateauthority/) site. Provide these certificates as an array to a SignedDataVerifier to allow verifying the signed data comes from Apple.
+
 ## Usage
 
 ### API Usage
 
 ```python
 from appstoreserverlibrary.api_client import AppStoreServerAPIClient, APIException
 from appstoreserverlibrary.models.Environment import Environment
-from appstoreserverlibrary.models.SendTestNotificationResponse import SendTestNotificationResponse
 
-private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implemenation will vary
+private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implementation will vary
 
 key_id = "ABCDEFGHIJ"
 issuer_id = "99b16628-15e4-4668-972b-eeff55eeff55"
 bundle_id = "com.example"
 environment = Environment.SANDBOX
 
 client = AppStoreServerAPIClient(private_key, key_id, issuer_id, bundle_id, environment)
@@ -90,15 +100,15 @@
 ```python
 from appstoreserverlibrary.api_client import AppStoreServerAPIClient, APIException
 from appstoreserverlibrary.models.Environment import Environment
 from appstoreserverlibrary.receipt_utility import ReceiptUtility
 from appstoreserverlibrary.models.HistoryResponse import HistoryResponse
 from appstoreserverlibrary.models.TransactionHistoryRequest import TransactionHistoryRequest, ProductType, Order
 
-private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implemenation will vary
+private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implementation will vary
 
 key_id = "ABCDEFGHIJ"
 issuer_id = "99b16628-15e4-4668-972b-eeff55eeff55"
 bundle_id = "com.example"
 environment = Environment.SANDBOX
 
 client = AppStoreServerAPIClient(private_key, key_id, issuer_id, bundle_id, environment)
@@ -128,15 +138,15 @@
 
 ### Promotional Offer Signature Creation
 
 ```python
 from appstoreserverlibrary.promotional_offer import PromotionalOfferSignatureCreator
 import time
 
-private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implemenation will vary
+private_key = read_private_key("/path/to/key/SubscriptionKey_ABCDEFGHIJ.p8") # Implementation will vary
 
 key_id = "ABCDEFGHIJ"
 bundle_id = "com.example"
 
 promotion_code_signature_generator = PromotionalOfferSignatureCreator(private_key, key_id, bundle_id)
 
 product_id = "<product_id>"
```

### Comparing `app-store-server-library-1.1.0/app_store_server_library.egg-info/SOURCES.txt` & `app_store_server_library-1.2.0/app_store_server_library.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 appstoreserverlibrary/receipt_utility.py
 appstoreserverlibrary/signed_data_verifier.py
 appstoreserverlibrary/models/AccountTenure.py
 appstoreserverlibrary/models/AppTransaction.py
 appstoreserverlibrary/models/AutoRenewStatus.py
 appstoreserverlibrary/models/CheckTestNotificationResponse.py
 appstoreserverlibrary/models/ConsumptionRequest.py
+appstoreserverlibrary/models/ConsumptionRequestReason.py
 appstoreserverlibrary/models/ConsumptionStatus.py
 appstoreserverlibrary/models/Data.py
 appstoreserverlibrary/models/DeliveryStatus.py
 appstoreserverlibrary/models/Environment.py
 appstoreserverlibrary/models/ExpirationIntent.py
 appstoreserverlibrary/models/ExtendReasonCode.py
 appstoreserverlibrary/models/ExtendRenewalDateRequest.py
@@ -48,14 +49,15 @@
 appstoreserverlibrary/models/OfferType.py
 appstoreserverlibrary/models/OrderLookupResponse.py
 appstoreserverlibrary/models/OrderLookupStatus.py
 appstoreserverlibrary/models/Platform.py
 appstoreserverlibrary/models/PlayTime.py
 appstoreserverlibrary/models/PriceIncreaseStatus.py
 appstoreserverlibrary/models/RefundHistoryResponse.py
+appstoreserverlibrary/models/RefundPreference.py
 appstoreserverlibrary/models/ResponseBodyV2.py
 appstoreserverlibrary/models/ResponseBodyV2DecodedPayload.py
 appstoreserverlibrary/models/RevocationReason.py
 appstoreserverlibrary/models/SendAttemptItem.py
 appstoreserverlibrary/models/SendAttemptResult.py
 appstoreserverlibrary/models/SendTestNotificationResponse.py
 appstoreserverlibrary/models/Status.py
```

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/api_client.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,14 +304,23 @@
     """
 
     INVALID_TRANSACTION_NOT_CONSUMABLE = 4000043
     """
     An error that indicates the transaction identifier doesn’t represent a consumable in-app purchase.
     
     https://developer.apple.com/documentation/appstoreserverapi/invalidtransactionnotconsumableerror
+
+    .. deprecated:: 1.11
+    """
+
+    INVALID_TRANSACTION_TYPE_NOT_SUPPORTED = 4000047
+    """
+    An error that indicates the transaction identifier represents an unsupported in-app purchase type.
+    
+    https://developer.apple.com/documentation/appstoreserverapi/invalidtransactiontypenotsupportederror
     """
 
     SUBSCRIPTION_EXTENSION_INELIGIBLE = 4030004
     """
     An error that indicates the subscription doesn't qualify for a renewal-date extension due to its subscription state.
     
     https://developer.apple.com/documentation/appstoreserverapi/subscriptionextensionineligibleerror
@@ -439,16 +448,20 @@
             if raw_api_error is not None:
                 self.api_error = APIError(raw_api_error)
         except ValueError:
             pass
 
 class AppStoreServerAPIClient:
     def __init__(self, signing_key: bytes, key_id: str, issuer_id: str, bundle_id: str, environment: Environment):
+        if environment == Environment.XCODE:
+            raise ValueError("Xcode is not a supported environment for an AppStoreServerAPIClient")
         if environment == Environment.PRODUCTION:
             self._base_url = "https://api.storekit.itunes.apple.com"
+        elif environment == Environment.LOCAL_TESTING:
+            self._base_url = "https://local-testing-base-url"
         else:
             self._base_url = "https://api.storekit-sandbox.itunes.apple.com"
         self._signing_key = serialization.load_pem_private_key(signing_key, password=None, backend=default_backend())
         self._key_id = key_id
         self._issuer_id = issuer_id
         self._bundle_id = bundle_id
 
@@ -464,25 +477,25 @@
             self._signing_key,
             algorithm="ES256",
             headers={"kid": self._key_id},
         )
 
     def _make_request(self, path: str, method: str, queryParameters: Dict[str, Union[str, List[str]]], body, destination_class: Type[T]) -> T:
         url = self._base_url + path
-        c = _get_cattrs_converter(type(body)) if body != None else None
-        json = c.unstructure(body) if body != None else None
+        c = _get_cattrs_converter(type(body)) if body is not None else None
+        json = c.unstructure(body) if body is not None else None
         headers = {
-            'User-Agent': "app-store-server-library/python/1.1.0",
+            'User-Agent': "app-store-server-library/python/1.2.0",
             'Authorization': 'Bearer ' + self._generate_token(),
             'Accept': 'application/json'
         }
         
         response = self._execute_request(method, url, queryParameters, headers, json)
-        if response.status_code >= 200 and response.status_code < 300:
-            if destination_class == None:
+        if 200 <= response.status_code < 300:
+            if destination_class is None:
                 return
             c = _get_cattrs_converter(destination_class)
             response_body = response.json()
             return c.structure(response_body, destination_class)
         else:
             # Best effort parsing of the response body
             if not 'content-type' in response.headers or response.headers['content-type'] != 'application/json':
@@ -517,54 +530,54 @@
         :param original_transaction_id:    The original transaction identifier of the subscription receiving a renewal date extension.
         :param extend_renewal_date_request: The request body containing subscription-renewal-extension data.
         :return: A response that indicates whether an individual renewal-date extension succeeded, and related details.
         :throws APIException: If a response was returned indicating the request could not be processed
         """
         return self._make_request("/inApps/v1/subscriptions/extend/" + original_transaction_id, "PUT", {}, extend_renewal_date_request, ExtendRenewalDateResponse)
     
-    def get_all_subscription_statuses(self, transaction_id: str, status: List[Status] = None) -> StatusResponse:
+    def get_all_subscription_statuses(self, transaction_id: str, status: Optional[List[Status]] = None) -> StatusResponse:
         """
         Get the statuses for all of a customer's auto-renewable subscriptions in your app.
         https://developer.apple.com/documentation/appstoreserverapi/get_all_subscription_statuses
         
         :param transaction_id: The identifier of a transaction that belongs to the customer, and which may be an original transaction identifier.
         :param status: An optional filter that indicates the status of subscriptions to include in the response. Your query may specify more than one status query parameter.
         :return: A response that contains status information for all of a customer's auto-renewable subscriptions in your app.
         :throws APIException: If a response was returned indicating the request could not be processed
         """
         queryParameters: Dict[str, List[str]] = dict()
-        if status != None:
+        if status is not None:
             queryParameters["status"] = [s.value for s in status]
         
         return self._make_request("/inApps/v1/subscriptions/" + transaction_id, "GET", queryParameters, None, StatusResponse)
     
-    def get_refund_history(self, transaction_id: str, revision: str) -> RefundHistoryResponse:
+    def get_refund_history(self, transaction_id: str, revision: Optional[str]) -> RefundHistoryResponse:
         """
         Get a paginated list of all of a customer's refunded in-app purchases for your app.
         https://developer.apple.com/documentation/appstoreserverapi/get_refund_history
 
         :param transaction_id: The identifier of a transaction that belongs to the customer, and which may be an original transaction identifier.
-        :param revision:              A token you provide to get the next set of up to 20 transactions. All responses include a revision token. Use the revision token from the previous RefundHistoryResponse.
+        :param revision: A token you provide to get the next set of up to 20 transactions. All responses include a revision token. Use the revision token from the previous RefundHistoryResponse.
         :return: A response that contains status information for all of a customer's auto-renewable subscriptions in your app.
         :throws APIException: If a response was returned indicating the request could not be processed
         """
 
         queryParameters: Dict[str, List[str]] = dict()
-        if revision != None:
+        if revision is not None:
             queryParameters["revision"] = [revision]
         
         return self._make_request("/inApps/v2/refund/lookup/" + transaction_id, "GET", queryParameters, None, RefundHistoryResponse)
     
     def get_status_of_subscription_renewal_date_extensions(self, request_identifier: str, product_id: str) -> MassExtendRenewalDateStatusResponse:
         """
         Checks whether a renewal date extension request completed, and provides the final count of successful or failed extensions.
         https://developer.apple.com/documentation/appstoreserverapi/get_status_of_subscription_renewal_date_extensions
 
         :param request_identifier: The UUID that represents your request to the Extend Subscription Renewal Dates for All Active Subscribers endpoint.
-        :param product_id:         The product identifier of the auto-renewable subscription that you request a renewal-date extension for.
+        :param product_id: The product identifier of the auto-renewable subscription that you request a renewal-date extension for.
         :return: A response that indicates the current status of a request to extend the subscription renewal date to all eligible subscribers.
         :throws APIException: If a response was returned indicating the request could not be processed
         """
         return self._make_request("/inApps/v1/subscriptions/extend/mass/" + product_id + "/" + request_identifier, "GET", {}, None, MassExtendRenewalDateStatusResponse)
     
     def get_test_notification_status(self, test_notification_token: str) -> CheckTestNotificationResponse:
         """
@@ -573,66 +586,67 @@
 
         :param test_notification_token: The test notification token received from the Request a Test Notification endpoint
         :return: A response that contains the contents of the test notification sent by the App Store server and the result from your server.
         :throws APIException: If a response was returned indicating the request could not be processed
         """
         return self._make_request("/inApps/v1/notifications/test/" + test_notification_token, "GET", {}, None, CheckTestNotificationResponse)
     
-    def get_notification_history(self, pagination_token: str, notification_history_request: NotificationHistoryRequest) -> NotificationHistoryResponse:
+    def get_notification_history(self, pagination_token: Optional[str], notification_history_request: NotificationHistoryRequest) -> NotificationHistoryResponse:
         """
         Get a list of notifications that the App Store server attempted to send to your server.
         https://developer.apple.com/documentation/appstoreserverapi/get_notification_history
 
         :param pagination_token: An optional token you use to get the next set of up to 20 notification history records. All responses that have more records available include a paginationToken. Omit this parameter the first time you call this endpoint.
         :param notification_history_request: The request body that includes the start and end dates, and optional query constraints.
         :return: A response that contains the App Store Server Notifications history for your app.
         :throws APIException: If a response was returned indicating the request could not be processed
         """
         queryParameters: Dict[str, List[str]] = dict()
-        if pagination_token != None:
+        if pagination_token is not None:
             queryParameters["paginationToken"] = [pagination_token]
         
         return self._make_request("/inApps/v1/notifications/history", "POST", queryParameters, notification_history_request, NotificationHistoryResponse)
 
     def get_transaction_history(self, transaction_id: str, revision: Optional[str], transaction_history_request: TransactionHistoryRequest) -> HistoryResponse:
         """
         Get a customer's in-app purchase transaction history for your app.
         https://developer.apple.com/documentation/appstoreserverapi/get_transaction_history
 
         :param transaction_id: The identifier of a transaction that belongs to the customer, and which may be an original transaction identifier.
-        :param revision:              A token you provide to get the next set of up to 20 transactions. All responses include a revision token. Note: For requests that use the revision token, include the same query parameters from the initial request. Use the revision token from the previous HistoryResponse.
+        :param revision: A token you provide to get the next set of up to 20 transactions. All responses include a revision token. Note: For requests that use the revision token, include the same query parameters from the initial request. Use the revision token from the previous HistoryResponse.
+        :param transaction_history_request: The request parameters that includes the startDate,endDate,productIds,productTypes and optional query constraints.
         :return: A response that contains the customer's transaction history for an app.
         :throws APIException: If a response was returned indicating the request could not be processed
         """
         queryParameters: Dict[str, List[str]] = dict()
-        if revision != None:
+        if revision is not None:
             queryParameters["revision"] = [revision]
         
-        if transaction_history_request.startDate != None:
+        if transaction_history_request.startDate is not None:
             queryParameters["startDate"] = [str(transaction_history_request.startDate)]
         
-        if transaction_history_request.endDate != None:
+        if transaction_history_request.endDate is not None:
             queryParameters["endDate"] = [str(transaction_history_request.endDate)]
         
-        if transaction_history_request.productIds != None:
+        if transaction_history_request.productIds is not None:
             queryParameters["productId"] = transaction_history_request.productIds
         
-        if transaction_history_request.productTypes != None:
+        if transaction_history_request.productTypes is not None:
             queryParameters["productType"] = [product_type.value for product_type in transaction_history_request.productTypes]
         
-        if transaction_history_request.sort != None:
+        if transaction_history_request.sort is not None:
             queryParameters["sort"] = [transaction_history_request.sort.value]
         
-        if transaction_history_request.subscriptionGroupIdentifiers != None:
+        if transaction_history_request.subscriptionGroupIdentifiers is not None:
             queryParameters["subscriptionGroupIdentifier"] = transaction_history_request.subscriptionGroupIdentifiers
         
-        if transaction_history_request.inAppOwnershipType != None:
+        if transaction_history_request.inAppOwnershipType is not None:
             queryParameters["inAppOwnershipType"] = [transaction_history_request.inAppOwnershipType.value]
         
-        if transaction_history_request.revoked != None:
+        if transaction_history_request.revoked is not None:
             queryParameters["revoked"] = [str(transaction_history_request.revoked)]
         
         return self._make_request("/inApps/v1/history/" + transaction_id, "GET", queryParameters, None, HistoryResponse)
     
     def get_transaction_info(self, transaction_id: str) -> TransactionInfoResponse:
         """
         Get information about a single transaction for your app.
```

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/AccountTenure.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/AccountTenure.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/AppTransaction.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/AppTransaction.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/CheckTestNotificationResponse.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/CheckTestNotificationResponse.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/ConsumptionRequest.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/ConsumptionRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .ConsumptionStatus import ConsumptionStatus
 from .DeliveryStatus import DeliveryStatus
 from .LibraryUtility import AttrsRawValueAware
 from .LifetimeDollarsPurchased import LifetimeDollarsPurchased
 from .LifetimeDollarsRefunded import LifetimeDollarsRefunded
 from .Platform import Platform
 from .PlayTime import PlayTime
+from .RefundPreference import RefundPreference
 from .UserStatus import UserStatus
 
 @define
 class ConsumptionRequest(AttrsRawValueAware):
     """
     The request body containing consumption information.
     
@@ -133,8 +134,20 @@
     
     https://developer.apple.com/documentation/appstoreserverapi/userstatus
     """
 
     rawUserStatus: Optional[int] = UserStatus.create_raw_attr('userStatus')
     """
     See userStatus
+    """
+
+    refundPreference: Optional[RefundPreference] =  RefundPreference.create_main_attr('rawRefundPreference')
+    """
+    A value that indicates your preference, based on your operational logic, as to whether Apple should grant the refund.
+    
+    https://developer.apple.com/documentation/appstoreserverapi/refundpreference
+    """
+
+    rawRefundPreference: Optional[int] = RefundPreference.create_raw_attr('refundPreference')
+    """
+    See refundPreference
     """
```

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/Data.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/HistoryResponse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,63 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
-from typing import Optional
 
 from attr import define
+from typing import List, Optional
 import attr
 
 from .Environment import Environment
-from .Status import Status
 from .LibraryUtility import AttrsRawValueAware
 
 @define
-class Data(AttrsRawValueAware):
+class HistoryResponse(AttrsRawValueAware):
     """
-    The app metadata and the signed renewal and transaction information.
+    A response that contains the customer's transaction history for an app.
     
-    https://developer.apple.com/documentation/appstoreservernotifications/data
+    https://developer.apple.com/documentation/appstoreserverapi/historyresponse
     """
-    environment: Optional[Environment] = Environment.create_main_attr('rawEnvironment')
+
+    revision: Optional[str] = attr.ib(default=None)
     """
-    The server environment that the notification applies to, either sandbox or production.
+    A token you use in a query to request the next set of transactions for the customer.
     
-    https://developer.apple.com/documentation/appstoreservernotifications/environment
-    """
-    rawEnvironment: Optional[str] = Environment.create_raw_attr('environment')
-    """
-    See environment
+    https://developer.apple.com/documentation/appstoreserverapi/revision
     """
 
-    appAppleId: Optional[int] = attr.ib(default=None)
+    hasMore: Optional[bool] = attr.ib(default=None)
     """
-    The unique identifier of an app in the App Store.
+    A Boolean value indicating whether the App Store has more transaction data.
     
-    https://developer.apple.com/documentation/appstoreservernotifications/appappleid
+    https://developer.apple.com/documentation/appstoreserverapi/hasmore
     """
 
     bundleId: Optional[str] = attr.ib(default=None)
     """
     The bundle identifier of an app.
     
     https://developer.apple.com/documentation/appstoreserverapi/bundleid
     """
 
-    bundleVersion: Optional[str] = attr.ib(default=None)
+    appAppleId: Optional[int] = attr.ib(default=None)
     """
-    The version of the build that identifies an iteration of the bundle.
+    The unique identifier of an app in the App Store.
     
-    https://developer.apple.com/documentation/appstoreservernotifications/bundleversion
+    https://developer.apple.com/documentation/appstoreservernotifications/appappleid
     """
 
-    signedTransactionInfo: Optional[str] = attr.ib(default=None)
+    environment: Optional[Environment] = Environment.create_main_attr('rawEnvironment')
     """
-    Transaction information signed by the App Store, in JSON Web Signature (JWS) format.
+    The server environment in which you're making the request, whether sandbox or production.
     
-    https://developer.apple.com/documentation/appstoreserverapi/jwstransaction
+    https://developer.apple.com/documentation/appstoreserverapi/environment
     """
 
-    signedRenewalInfo: Optional[str] = attr.ib(default=None)
-    """
-    Subscription renewal information, signed by the App Store, in JSON Web Signature (JWS) format.
-    
-    https://developer.apple.com/documentation/appstoreserverapi/jwsrenewalinfo
-    """
-        
-    status: Optional[Status] = Status.create_main_attr('rawStatus')
+    rawEnvironment: Optional[str] = Environment.create_raw_attr('environment')
     """
-    The status of an auto-renewable subscription as of the signedDate in the responseBodyV2DecodedPayload.
-    
-    https://developer.apple.com/documentation/appstoreservernotifications/status
+    See environment
     """
 
-    rawStatus: Optional[int] = Status.create_raw_attr('status')
+    signedTransactions: Optional[List[str]] = attr.ib(default=None)
     """
-    See status
+    An array of in-app purchase transactions for the customer, signed by Apple, in JSON Web Signature format.
+    
+    https://developer.apple.com/documentation/appstoreserverapi/jwstransaction
     """
```

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/DeliveryStatus.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/DeliveryStatus.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/ExpirationIntent.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/ExpirationIntent.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/ExtendRenewalDateRequest.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/ExtendRenewalDateRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     
     https://developer.apple.com/documentation/appstoreserverapi/extendrenewaldaterequest
     """
 
     extendByDays: Optional[int] = attr.ib(default=None)
     """
     The number of days to extend the subscription renewal date.
-    
+
     https://developer.apple.com/documentation/appstoreserverapi/extendbydays
     maximum: 90
     """
 
     extendReasonCode: Optional[ExtendReasonCode] = attr.ib(default=None)
     """
     The reason code for the subscription date extension
```

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/ExtendRenewalDateResponse.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/ExtendRenewalDateResponse.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/ExternalPurchaseToken.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/ExternalPurchaseToken.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/FirstSendAttemptResult.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/FirstSendAttemptResult.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/HistoryResponse.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/StatusResponse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional, List
 
 from attr import define
-from typing import List, Optional
 import attr
 
 from .Environment import Environment
 from .LibraryUtility import AttrsRawValueAware
+from .SubscriptionGroupIdentifierItem import SubscriptionGroupIdentifierItem
 
 @define
-class HistoryResponse(AttrsRawValueAware):
+class StatusResponse(AttrsRawValueAware):
     """
-    A response that contains the customer's transaction history for an app.
+    A response that contains status information for all of a customer's auto-renewable subscriptions in your app.
     
-    https://developer.apple.com/documentation/appstoreserverapi/historyresponse
+    https://developer.apple.com/documentation/appstoreserverapi/statusresponse
     """
 
-    revision: Optional[str] = attr.ib(default=None)
+    environment: Optional[Environment] = Environment.create_main_attr('rawEnvironment')
     """
-    A token you use in a query to request the next set of transactions for the customer.
+    The server environment, sandbox or production, in which the App Store generated the response.
     
-    https://developer.apple.com/documentation/appstoreserverapi/revision
+    https://developer.apple.com/documentation/appstoreserverapi/environment
     """
-
-    hasMore: Optional[bool] = attr.ib(default=None)
+            
+    rawEnvironment: Optional[str] = Environment.create_raw_attr('environment')
     """
-    A Boolean value indicating whether the App Store has more transaction data.
-    
-    https://developer.apple.com/documentation/appstoreserverapi/hasmore
+    See environment
     """
 
     bundleId: Optional[str] = attr.ib(default=None)
     """
     The bundle identifier of an app.
     
     https://developer.apple.com/documentation/appstoreserverapi/bundleid
@@ -39,25 +38,13 @@
     appAppleId: Optional[int] = attr.ib(default=None)
     """
     The unique identifier of an app in the App Store.
     
     https://developer.apple.com/documentation/appstoreservernotifications/appappleid
     """
 
-    environment: Optional[Environment] = Environment.create_main_attr('rawEnvironment')
-    """
-    The server environment in which you're making the request, whether sandbox or production.
-    
-    https://developer.apple.com/documentation/appstoreserverapi/environment
-    """
-
-    rawEnvironment: Optional[str] = Environment.create_raw_attr('environment')
-    """
-    See environment
-    """
-
-    signedTransactions: Optional[List[str]] = attr.ib(default=None)
+    data: Optional[List[SubscriptionGroupIdentifierItem]] = attr.ib(default=None)
     """
-    An array of in-app purchase transactions for the customer, signed by Apple, in JSON Web Signature format.
+    An array of information for auto-renewable subscriptions, including App Store-signed transaction information and App Store-signed renewal information.
     
-    https://developer.apple.com/documentation/appstoreserverapi/jwstransaction
+    https://developer.apple.com/documentation/appstoreserverapi/subscriptiongroupidentifieritem
     """
```

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/JWSRenewalInfoDecodedPayload.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/JWSRenewalInfoDecodedPayload.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/JWSTransactionDecodedPayload.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/JWSTransactionDecodedPayload.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
     An Apple-defined value that uniquely identifies the App Store storefront associated with the purchase.
     
     https://developer.apple.com/documentation/appstoreserverapi/storefrontid
     """
 
     transactionReason: Optional[TransactionReason] = TransactionReason.create_main_attr('rawTransactionReason')
     """
-    The reason for the purchase transaction, which indicates whether it's a customer's purchase or a renewal for an auto-renewable subscription that the system initates.
+    The reason for the purchase transaction, which indicates whether it's a customer's purchase or a renewal for an auto-renewable subscription that the system initiates.
     
     https://developer.apple.com/documentation/appstoreserverapi/transactionreason
     """
 
     rawTransactionReason: Optional[str] = TransactionReason.create_raw_attr('transactionReason')
     """
     See transactionReason
@@ -218,15 +218,15 @@
     The three-letter ISO 4217 currency code for the price of the product.
     
     https://developer.apple.com/documentation/appstoreserverapi/currency
     """
 
     price: Optional[int] = attr.ib(default=None)
     """
-    The price of the in-app purchase or subscription offer that you configured in App Store Connect, as an integer.
+    The price, in milliunits, of the in-app purchase or subscription offer that you configured in App Store Connect.
     
     https://developer.apple.com/documentation/appstoreserverapi/price
     """
 
     offerDiscountType: Optional[OfferDiscountType] = OfferDiscountType.create_main_attr('rawOfferDiscountType')
     """
     The payment mode you configure for an introductory offer, promotional offer, or offer code on an auto-renewable subscription.
```

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/LastTransactionsItem.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/LastTransactionsItem.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/LibraryUtility.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/LibraryUtility.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/LifetimeDollarsPurchased.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/LifetimeDollarsPurchased.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/LifetimeDollarsRefunded.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/LifetimeDollarsRefunded.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/MassExtendRenewalDateRequest.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/MassExtendRenewalDateRequest.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/MassExtendRenewalDateResponse.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/MassExtendRenewalDateResponse.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/MassExtendRenewalDateStatusResponse.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/MassExtendRenewalDateStatusResponse.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/NotificationHistoryRequest.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationHistoryRequest.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/NotificationHistoryResponse.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationHistoryResponse.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,8 +28,9 @@
     https://developer.apple.com/documentation/appstoreserverapi/hasmore
     """
 
     notificationHistory: Optional[List[NotificationHistoryResponseItem]] = attr.ib(default=None)
     """
     An array of App Store server notification history records.
     
+    https://developer.apple.com/documentation/appstoreserverapi/notificationhistoryresponseitem
     """
```

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/NotificationHistoryResponseItem.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationHistoryResponseItem.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/NotificationTypeV2.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/NotificationTypeV2.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from enum import Enum
 
 from .LibraryUtility import AppStoreServerLibraryEnumMeta
 
 class NotificationTypeV2(str, Enum, metaclass=AppStoreServerLibraryEnumMeta):
     """
-    A notification type value that App Store Server Notifications V2 uses.
+    The type that describes the in-app purchase or external purchase event for which the App Store sends the version 2 notification.
     
-    https://developer.apple.com/documentation/appstoreserverapi/notificationtype
+    https://developer.apple.com/documentation/appstoreservernotifications/notificationtype
     """
     SUBSCRIBED = "SUBSCRIBED"
     DID_CHANGE_RENEWAL_PREF = "DID_CHANGE_RENEWAL_PREF"
     DID_CHANGE_RENEWAL_STATUS = "DID_CHANGE_RENEWAL_STATUS"
     OFFER_REDEEMED = "OFFER_REDEEMED"
     DID_RENEW = "DID_RENEW"
     EXPIRED = "EXPIRED"
```

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/OfferDiscountType.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/OfferDiscountType.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/OrderLookupResponse.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/OrderLookupResponse.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,8 +26,10 @@
     """
     See status
     """
 
     signedTransactions: Optional[List[str]] = attr.ib(default=None)
     """
     An array of in-app purchase transactions that are part of order, signed by Apple, in JSON Web Signature format.
+    
+    https://developer.apple.com/documentation/appstoreserverapi/jwstransaction
     """
```

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/PlayTime.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/PlayTime.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/PriceIncreaseStatus.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/PriceIncreaseStatus.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/RefundHistoryResponse.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/RefundHistoryResponse.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     
     https://developer.apple.com/documentation/appstoreserverapi/refundhistoryresponse
     """
 
     signedTransactions: Optional[List[str]] = attr.ib(default=None)
     """
     A list of up to 20 JWS transactions, or an empty array if the customer hasn't received any refunds in your app. The transactions are sorted in ascending order by revocationDate.
+    
+    https://developer.apple.com/documentation/appstoreserverapi/jwstransaction
     """
 
     revision: Optional[str] = attr.ib(default=None)
     """
     A token you use in a query to request the next set of transactions for the customer.
     
     https://developer.apple.com/documentation/appstoreserverapi/revision
```

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/ResponseBodyV2.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/ResponseBodyV2.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/ResponseBodyV2DecodedPayload.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/ResponseBodyV2DecodedPayload.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/SendAttemptItem.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/SendAttemptItem.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/SendAttemptResult.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/SendAttemptResult.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/SendTestNotificationResponse.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/SendTestNotificationResponse.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/StatusResponse.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/SubscriptionGroupIdentifierItem.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,29 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
 from typing import Optional, List
 
 from attr import define
 import attr
 
-from .Environment import Environment
-from .LibraryUtility import AttrsRawValueAware
-from .SubscriptionGroupIdentifierItem import SubscriptionGroupIdentifierItem
+from .LastTransactionsItem import LastTransactionsItem
 
 @define
-class StatusResponse(AttrsRawValueAware):
+class SubscriptionGroupIdentifierItem: 
     """
-    A response that contains status information for all of a customer's auto-renewable subscriptions in your app.
+    Information for auto-renewable subscriptions, including signed transaction information and signed renewal information, for one subscription group.
     
-    https://developer.apple.com/documentation/appstoreserverapi/statusresponse
+    https://developer.apple.com/documentation/appstoreserverapi/subscriptiongroupidentifieritem
     """
 
-    environment: Optional[Environment] = Environment.create_main_attr('rawEnvironment')
+    subscriptionGroupIdentifier: Optional[str] = attr.ib(default=None)
     """
-    The server environment, sandbox or production, in which the App Store generated the response.
+    The identifier of the subscription group that the subscription belongs to.
     
-    https://developer.apple.com/documentation/appstoreserverapi/environment
-    """
-            
-    rawEnvironment: Optional[str] = Environment.create_raw_attr('environment')
-    """
-    See environment
-    """
-
-    bundleId: Optional[str] = attr.ib(default=None)
-    """
-    The bundle identifier of an app.
-    
-    https://developer.apple.com/documentation/appstoreserverapi/bundleid
-    """
+    https://developer.apple.com/documentation/appstoreserverapi/subscriptiongroupidentifier
+    """    
 
-    appAppleId: Optional[int] = attr.ib(default=None)
+    lastTransactions: Optional[List[LastTransactionsItem]] = attr.ib(default=None)
     """
-    The unique identifier of an app in the App Store.
+    An array of the most recent App Store-signed transaction information and App Store-signed renewal information for all auto-renewable subscriptions in the subscription group.
     
-    https://developer.apple.com/documentation/appstoreservernotifications/appappleid
+    https://developer.apple.com/documentation/appstoreserverapi/lasttransactionsitem
     """
-
-    data: Optional[List[SubscriptionGroupIdentifierItem]] = attr.ib(default=None)
-    """
-    An array of information for auto-renewable subscriptions, including App Store-signed transaction information and App Store-signed renewal information.
-    
-    """
```

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/Subtype.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/Subtype.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from enum import Enum
 
 from .LibraryUtility import AppStoreServerLibraryEnumMeta
 
 class Subtype(str, Enum, metaclass=AppStoreServerLibraryEnumMeta):
     """
-    A notification subtype value that App Store Server Notifications 2 uses.
+    A string that provides details about select notification types in version 2.
     
-    https://developer.apple.com/documentation/appstoreserverapi/notificationsubtype
+    https://developer.apple.com/documentation/appstoreservernotifications/subtype
     """
     INITIAL_BUY = "INITIAL_BUY"
     RESUBSCRIBE = "RESUBSCRIBE"
     DOWNGRADE = "DOWNGRADE"
     UPGRADE = "UPGRADE"
     AUTO_RENEW_ENABLED = "AUTO_RENEW_ENABLED"
     AUTO_RENEW_DISABLED = "AUTO_RENEW_DISABLED"
```

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/Summary.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/Summary.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/TransactionHistoryRequest.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/TransactionHistoryRequest.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/TransactionInfoResponse.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/TransactionInfoResponse.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/TransactionReason.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/TransactionReason.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/models/Type.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/models/Type.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/promotional_offer.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/promotional_offer.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/receipt_utility.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/receipt_utility.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/appstoreserverlibrary/signed_data_verifier.py` & `app_store_server_library-1.2.0/appstoreserverlibrary/signed_data_verifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,56 +30,59 @@
     """
     def __init__(
         self,
         root_certificates: List[bytes],
         enable_online_checks: bool,
         environment: Environment,
         bundle_id: str,
-        app_apple_id: int = None,
+        app_apple_id: Optional[int] = None,
     ):
         self._chain_verifier = _ChainVerifier(root_certificates)
         self._environment = environment
         self._bundle_id = bundle_id
         self._app_apple_id = app_apple_id
         self._enable_online_checks = enable_online_checks
         if environment == Environment.PRODUCTION and app_apple_id is None:
             raise ValueError("appAppleId is required when the environment is Production")
 
     def verify_and_decode_renewal_info(self, signed_renewal_info: str) -> JWSRenewalInfoDecodedPayload:
         """
         Verifies and decodes a signedRenewalInfo obtained from the App Store Server API, an App Store Server Notification, or from a device
+        See https://developer.apple.com/documentation/appstoreserverapi/jwsrenewalinfo
 
         :param signed_renewal_info: The signedRenewalInfo field
         :return: The decoded renewal info after verification
         :throws VerificationException: Thrown if the data could not be verified
         """
         
         decoded_renewal_info = _get_cattrs_converter(JWSRenewalInfoDecodedPayload).structure(self._decode_signed_object(signed_renewal_info), JWSRenewalInfoDecodedPayload)
         if decoded_renewal_info.environment != self._environment:
             raise VerificationException(VerificationStatus.INVALID_ENVIRONMENT)
         return decoded_renewal_info
 
     def verify_and_decode_signed_transaction(self, signed_transaction: str) -> JWSTransactionDecodedPayload:
         """
         Verifies and decodes a signedTransaction obtained from the App Store Server API, an App Store Server Notification, or from a device
+        See https://developer.apple.com/documentation/appstoreserverapi/jwstransaction
 
-        :param signed_transaction: The signedRenewalInfo field
+        :param signed_transaction: The signedTransaction field
         :return: The decoded transaction info after verification
         :throws VerificationException: Thrown if the data could not be verified
         """
         decoded_transaction_info = _get_cattrs_converter(JWSTransactionDecodedPayload).structure(self._decode_signed_object(signed_transaction), JWSTransactionDecodedPayload)
         if decoded_transaction_info.bundleId != self._bundle_id:
             raise VerificationException(VerificationStatus.INVALID_APP_IDENTIFIER)
         if decoded_transaction_info.environment != self._environment:
             raise VerificationException(VerificationStatus.INVALID_ENVIRONMENT)
         return decoded_transaction_info
 
     def verify_and_decode_notification(self, signed_payload: str) -> ResponseBodyV2DecodedPayload:
         """
         Verifies and decodes an App Store Server Notification signedPayload
+        See https://developer.apple.com/documentation/appstoreservernotifications/signedpayload
 
         :param signedPayload: The payload received by your server
         :return: The decoded payload after verification
         :throws VerificationException: Thrown if the data could not be verified
         """
         decoded_dict = self._decode_signed_object(signed_payload)
         decoded_signed_notification = _get_cattrs_converter(ResponseBodyV2DecodedPayload).structure(decoded_dict, ResponseBodyV2DecodedPayload)
@@ -109,14 +112,15 @@
             raise VerificationException(VerificationStatus.INVALID_APP_IDENTIFIER)
         if environment != self._environment:
             raise VerificationException(VerificationStatus.INVALID_ENVIRONMENT)
 
     def verify_and_decode_app_transaction(self, signed_app_transaction: str) -> AppTransaction:
         """
         Verifies and decodes a signed AppTransaction
+        See https://developer.apple.com/documentation/storekit/apptransaction
 
         :param signed_app_transaction: The signed AppTransaction
         :return: The decoded AppTransaction after validation
         :throws VerificationException: Thrown if the data could not be verified
         """
         decoded_dict = self._decode_signed_object(signed_app_transaction)
         decoded_app_transaction = _get_cattrs_converter(AppTransaction).structure(decoded_dict, AppTransaction)
```

### Comparing `app-store-server-library-1.1.0/setup.py` & `app_store_server_library-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="app-store-server-library",
-    version="1.1.0",
+    version="1.2.0",
     description="The App Store Server Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=["tests"]),
     python_requires=">=3.7, <4",
     install_requires=["attrs >= 21.3.0", 'PyJWT >= 2.6.0, < 3', 'requests >= 2.28.0, < 3', 'cryptography >= 40.0.0, < 43', 'pyOpenSSL >= 23.1.1, < 25', 'asn1==2.7.0', 'cattrs==23.1.2'],
     package_data={"appstoreserverlibrary": ["py.typed"]},
+    license="MIT",
+    classifiers=["License :: OSI Approved :: MIT License"],
 )
```

### Comparing `app-store-server-library-1.1.0/tests/test_api_client.py` & `app_store_server_library-1.2.0/tests/test_api_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from appstoreserverlibrary.models.NotificationHistoryResponseItem import NotificationHistoryResponseItem
 from appstoreserverlibrary.models.NotificationTypeV2 import NotificationTypeV2
 from appstoreserverlibrary.models.OfferType import OfferType
 from appstoreserverlibrary.models.OrderLookupStatus import OrderLookupStatus
 from appstoreserverlibrary.models.Platform import Platform
 from appstoreserverlibrary.models.PlayTime import PlayTime
 from appstoreserverlibrary.models.PriceIncreaseStatus import PriceIncreaseStatus
+from appstoreserverlibrary.models.RefundPreference import RefundPreference
 from appstoreserverlibrary.models.RevocationReason import RevocationReason
 from appstoreserverlibrary.models.SendAttemptItem import SendAttemptItem
 from appstoreserverlibrary.models.SendAttemptResult import SendAttemptResult
 from appstoreserverlibrary.models.Status import Status
 from appstoreserverlibrary.models.SubscriptionGroupIdentifierItem import SubscriptionGroupIdentifierItem
 from appstoreserverlibrary.models.Subtype import Subtype
 from appstoreserverlibrary.models.TransactionHistoryRequest import Order, ProductType, TransactionHistoryRequest
@@ -42,15 +43,15 @@
 
 from io import BytesIO
 
 class DecodedPayloads(unittest.TestCase):
     def test_extend_renewal_date_for_all_active_subscribers(self):
         client = self.get_client_with_body_from_file('tests/resources/models/extendRenewalDateForAllActiveSubscribersResponse.json',
                                            'POST',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/subscriptions/extend/mass',
+                                           'https://local-testing-base-url/inApps/v1/subscriptions/extend/mass',
                                            {}, 
                                            {'extendByDays': 45, 'extendReasonCode': 1, 'requestIdentifier': 'fdf964a4-233b-486c-aac1-97d8d52688ac', 'storefrontCountryCodes': ['USA', 'MEX'], 'productId': 'com.example.productId'})
         
         extend_renewal_date_request = MassExtendRenewalDateRequest(
              extendByDays=45,
              extendReasonCode=ExtendReasonCode.CUSTOMER_SATISFACTION,
              requestIdentifier='fdf964a4-233b-486c-aac1-97d8d52688ac',
@@ -61,15 +62,15 @@
 
         self.assertIsNotNone(mass_extend_renewal_date_response)
         self.assertEqual('758883e8-151b-47b7-abd0-60c4d804c2f5', mass_extend_renewal_date_response.requestIdentifier)
 
     def test_extend_subscription_renewal_date(self):
         client = self.get_client_with_body_from_file('tests/resources/models/extendSubscriptionRenewalDateResponse.json',
                                            'PUT',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/subscriptions/extend/4124214',
+                                           'https://local-testing-base-url/inApps/v1/subscriptions/extend/4124214',
                                            {},
                                            {'extendByDays': 45, 'extendReasonCode': 1, 'requestIdentifier': 'fdf964a4-233b-486c-aac1-97d8d52688ac'})
 
         extend_renewal_date_request = ExtendRenewalDateRequest(
              extendByDays=45,
              extendReasonCode=ExtendReasonCode.CUSTOMER_SATISFACTION,
              requestIdentifier='fdf964a4-233b-486c-aac1-97d8d52688ac'
@@ -82,15 +83,15 @@
         self.assertEqual('9993', extend_renewal_date_response.webOrderLineItemId)
         self.assertTrue(extend_renewal_date_response.success)
         self.assertEqual(1698148900000, extend_renewal_date_response.effectiveDate)
 
     def test_get_all_subscription_statuses(self):
         client = self.get_client_with_body_from_file('tests/resources/models/getAllSubscriptionStatusesResponse.json',
                                            'GET',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/subscriptions/4321', 
+                                           'https://local-testing-base-url/inApps/v1/subscriptions/4321', 
                                            {'status': [2, 1]},
                                            None)
 
         status_response = client.get_all_subscription_statuses('4321', [Status.EXPIRED, Status.ACTIVE])
 
         self.assertIsNotNone(status_response)
         self.assertEqual(Environment.LOCAL_TESTING, status_response.environment)
@@ -130,29 +131,29 @@
             )
         ]
         self.assertEqual(expected_body, status_response.data)
 
     def test_get_refund_history(self):
         client = self.get_client_with_body_from_file('tests/resources/models/getRefundHistoryResponse.json',
                                            'GET',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v2/refund/lookup/555555', 
+                                           'https://local-testing-base-url/inApps/v2/refund/lookup/555555', 
                                            {'revision': ['revision_input']}, 
                                            None)
 
         refund_history_response = client.get_refund_history('555555', 'revision_input')
 
         self.assertIsNotNone(refund_history_response)
         self.assertEqual(['signed_transaction_one', 'signed_transaction_two'], refund_history_response.signedTransactions)
         self.assertEqual('revision_output', refund_history_response.revision)
         self.assertTrue(refund_history_response.hasMore)
 
     def test_get_status_of_subscription_renewal_date_extensions(self):
         client = self.get_client_with_body_from_file('tests/resources/models/getStatusOfSubscriptionRenewalDateExtensionsResponse.json',
                                            'GET',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/subscriptions/extend/mass/20fba8a0-2b80-4a7d-a17f-85c1854727f8/com.example.product', 
+                                           'https://local-testing-base-url/inApps/v1/subscriptions/extend/mass/20fba8a0-2b80-4a7d-a17f-85c1854727f8/com.example.product', 
                                            {},
                                            None)
 
         mass_extend_renewal_date_status_response = client.get_status_of_subscription_renewal_date_extensions('com.example.product', '20fba8a0-2b80-4a7d-a17f-85c1854727f8')
 
         self.assertIsNotNone(mass_extend_renewal_date_status_response)
         self.assertEqual('20fba8a0-2b80-4a7d-a17f-85c1854727f8', mass_extend_renewal_date_status_response.requestIdentifier)
@@ -160,15 +161,15 @@
         self.assertEqual(1698148900000, mass_extend_renewal_date_status_response.completeDate)
         self.assertEqual(30, mass_extend_renewal_date_status_response.succeededCount)
         self.assertEqual(2, mass_extend_renewal_date_status_response.failedCount)
 
     def test_get_test_notification_status(self):
         client = self.get_client_with_body_from_file('tests/resources/models/getTestNotificationStatusResponse.json',
                                            'GET',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/notifications/test/8cd2974c-f905-492a-bf9a-b2f47c791d19',
+                                           'https://local-testing-base-url/inApps/v1/notifications/test/8cd2974c-f905-492a-bf9a-b2f47c791d19',
                                            {},
                                            None)
 
         check_test_notification_response = client.get_test_notification_status('8cd2974c-f905-492a-bf9a-b2f47c791d19')
 
         self.assertIsNotNone(check_test_notification_response)
         self.assertEqual('signed_payload', check_test_notification_response.signedPayload)
@@ -177,15 +178,15 @@
                                 SendAttemptItem(attemptDate=1698148950000,sendAttemptResult=SendAttemptResult.SUCCESS)
                             ]
         self.assertEqual(sendAttemptItems, check_test_notification_response.sendAttempts)
 
     def test_get_notification_history(self):
         client = self.get_client_with_body_from_file('tests/resources/models/getNotificationHistoryResponse.json',
                                            'POST',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/notifications/history', 
+                                           'https://local-testing-base-url/inApps/v1/notifications/history', 
                                            {'paginationToken': ['a036bc0e-52b8-4bee-82fc-8c24cb6715d6']},
                                            {'startDate': 1698148900000, 'endDate': 1698148950000, 'notificationType': 'SUBSCRIBED', 'notificationSubtype': 'INITIAL_BUY', 'transactionId': '999733843', 'onlyFailures': True})
 
         notification_history_request = NotificationHistoryRequest(
             startDate=1698148900000,
             endDate=1698148950000,
             notificationType=NotificationTypeV2.SUBSCRIBED,
@@ -218,15 +219,15 @@
              ], signedPayload='signed_payload_two')
         ]
         self.assertEqual(expected_notification_history, notification_history_response.notificationHistory)
 
     def test_get_transaction_history(self):
         client = self.get_client_with_body_from_file('tests/resources/models/transactionHistoryResponse.json',
                                            'GET',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/history/1234', 
+                                           'https://local-testing-base-url/inApps/v1/history/1234', 
                                            {'revision': ['revision_input'],
                                             'startDate': ['123455'],
                                             'endDate': ['123456'],
                                             'productId': ['com.example.1', 'com.example.2'],
                                             'productType': ['CONSUMABLE', 'AUTO_RENEWABLE'],
                                             'sort': ['ASCENDING'],
                                             'subscriptionGroupIdentifier': ['sub_group_id', 'sub_group_id_2'],
@@ -255,104 +256,116 @@
         self.assertEqual(Environment.LOCAL_TESTING, history_response.environment)
         self.assertEqual('LocalTesting', history_response.rawEnvironment)
         self.assertEqual(['signed_transaction_value', 'signed_transaction_value2'], history_response.signedTransactions)
 
     def test_get_transaction_info(self):
         client = self.get_client_with_body_from_file('tests/resources/models/transactionInfoResponse.json',
                                            'GET',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/transactions/1234', 
+                                           'https://local-testing-base-url/inApps/v1/transactions/1234', 
                                            {},
                                            None)
 
         transaction_info_response = client.get_transaction_info('1234')
 
         self.assertIsNotNone(transaction_info_response)
         self.assertEqual('signed_transaction_info_value', transaction_info_response.signedTransactionInfo)
 
     def test_look_up_order_id(self):
         client = self.get_client_with_body_from_file('tests/resources/models/lookupOrderIdResponse.json',
                                            'GET',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/lookup/W002182',
+                                           'https://local-testing-base-url/inApps/v1/lookup/W002182',
                                            {},
                                            None)
 
         order_lookup_response = client.look_up_order_id('W002182')
 
         self.assertIsNotNone(order_lookup_response)
         self.assertEqual(OrderLookupStatus.INVALID, order_lookup_response.status)
         self.assertEqual(1, order_lookup_response.rawStatus)
         self.assertEqual(['signed_transaction_one', 'signed_transaction_two'], order_lookup_response.signedTransactions)
 
     def test_request_test_notification(self):
         client = self.get_client_with_body_from_file('tests/resources/models/requestTestNotificationResponse.json',
                                            'POST',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/notifications/test',
+                                           'https://local-testing-base-url/inApps/v1/notifications/test',
                                            {},
                                            None)
 
         send_test_notification_response = client.request_test_notification()
 
         self.assertIsNotNone(send_test_notification_response)
         self.assertEqual('ce3af791-365e-4c60-841b-1674b43c1609', send_test_notification_response.testNotificationToken)
 
     def test_send_consumption_data(self):
         client = self.get_client_with_body(b'',
                                            'PUT',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/transactions/consumption/49571273', 
+                                           'https://local-testing-base-url/inApps/v1/transactions/consumption/49571273', 
                                            {},
                                            {'customerConsented': True,
                                             'consumptionStatus': 1,
                                             'platform': 2,
                                             'sampleContentProvided': False,
                                             'deliveryStatus': 3,
                                             'appAccountToken': '7389a31a-fb6d-4569-a2a6-db7d85d84813',
                                             'accountTenure': 4,
                                             'playTime': 5,
                                             'lifetimeDollarsRefunded': 6,
                                             'lifetimeDollarsPurchased': 7,
-                                            'userStatus': 4})
+                                            'userStatus': 4,
+                                            'refundPreference': 3})
 
         consumptionRequest = ConsumptionRequest(
             customerConsented=True,
             consumptionStatus=ConsumptionStatus.NOT_CONSUMED,
             platform=Platform.NON_APPLE,
             sampleContentProvided=False,
             deliveryStatus=DeliveryStatus.DID_NOT_DELIVER_DUE_TO_SERVER_OUTAGE,
             appAccountToken='7389a31a-fb6d-4569-a2a6-db7d85d84813',
             accountTenure=AccountTenure.THIRTY_DAYS_TO_NINETY_DAYS,
             playTime=PlayTime.ONE_DAY_TO_FOUR_DAYS,
             lifetimeDollarsRefunded=LifetimeDollarsRefunded.ONE_THOUSAND_DOLLARS_TO_ONE_THOUSAND_NINE_HUNDRED_NINETY_NINE_DOLLARS_AND_NINETY_NINE_CENTS,
             lifetimeDollarsPurchased=LifetimeDollarsPurchased.TWO_THOUSAND_DOLLARS_OR_GREATER,
-            userStatus=UserStatus.LIMITED_ACCESS
+            userStatus=UserStatus.LIMITED_ACCESS,
+            refundPreference=RefundPreference.NO_PREFERENCE
         )
 
         client.send_consumption_data('49571273', consumptionRequest)
 
     def test_api_error(self):
         client = self.get_client_with_body_from_file('tests/resources/models/apiException.json',
                                                      'POST',
-                                                     'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/notifications/test',
+                                                     'https://local-testing-base-url/inApps/v1/notifications/test',
                                                      {},
                                                      None,
                                                      500)
         try:
             client.request_test_notification()
         except APIException as e:
             self.assertEqual(500, e.http_status_code)
             self.assertEqual(5000000, e.raw_api_error)
             self.assertEqual(APIError.GENERAL_INTERNAL, e.api_error)
             self.assertEqual("An unknown error occurred.", e.error_message)
             return
         
         self.assertFalse(True)
+
+    def test_xcode_not_supported_error(self):
+        try:
+            signing_key = self.get_signing_key()
+            AppStoreServerAPIClient(signing_key, 'keyId', 'issuerId', 'com.example', Environment.XCODE)
+        except ValueError as e:
+            self.assertEqual("Xcode is not a supported environment for an AppStoreServerAPIClient", e.args[0])
+            return
+
+        self.assertFalse(True)
     
     def test_api_too_many_requests(self):
         client = self.get_client_with_body_from_file('tests/resources/models/apiTooManyRequestsException.json',
                                                      'POST',
-                                                     'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/notifications/test',
+                                                     'https://local-testing-base-url/inApps/v1/notifications/test',
                                                      {},
                                                      None,
                                                      429)
         try:
             client.request_test_notification()
         except APIException as e:
             self.assertEqual(429, e.http_status_code)
@@ -362,15 +375,15 @@
             return
         
         self.assertFalse(True)
 
     def test_unknown_error(self):
         client = self.get_client_with_body_from_file('tests/resources/models/apiUnknownError.json',
                                                      'POST',
-                                                     'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/notifications/test',
+                                                     'https://local-testing-base-url/inApps/v1/notifications/test',
                                                      {},
                                                      None,
                                                      400)
         try:
             client.request_test_notification()
         except APIException as e:
             self.assertEqual(400, e.http_status_code)
@@ -380,15 +393,15 @@
             return
         
         self.assertFalse(True)
 
     def test_get_transaction_history_with_unknown_environment(self):
         client = self.get_client_with_body_from_file('tests/resources/models/transactionHistoryResponseWithMalformedEnvironment.json',
                                            'GET',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/history/1234', 
+                                           'https://local-testing-base-url/inApps/v1/history/1234', 
                                            {'revision': ['revision_input'],
                                             'startDate': ['123455'],
                                             'endDate': ['123456'],
                                             'productId': ['com.example.1', 'com.example.2'],
                                             'productType': ['CONSUMABLE', 'AUTO_RENEWABLE'],
                                             'sort': ['ASCENDING'],
                                             'subscriptionGroupIdentifier': ['sub_group_id', 'sub_group_id_2'],
@@ -411,15 +424,15 @@
 
         self.assertIsNone(history_response.environment)
         self.assertEqual("LocalTestingxxx", history_response.rawEnvironment)
 
     def test_get_transaction_history_with_malformed_app_apple_id(self):
         client = self.get_client_with_body_from_file('tests/resources/models/transactionHistoryResponseWithMalformedAppAppleId.json',
                                            'GET',
-                                           'https://api.storekit-sandbox.itunes.apple.com/inApps/v1/history/1234', 
+                                           'https://local-testing-base-url/inApps/v1/history/1234', 
                                            {'revision': ['revision_input'],
                                             'startDate': ['123455'],
                                             'endDate': ['123456'],
                                             'productId': ['com.example.1', 'com.example.2'],
                                             'productType': ['CONSUMABLE', 'AUTO_RENEWABLE'],
                                             'sort': ['ASCENDING'],
                                             'subscriptionGroupIdentifier': ['sub_group_id', 'sub_group_id_2'],
@@ -441,17 +454,19 @@
         try:
             client.get_transaction_history('1234', 'revision_input', request)
         except Exception:
             return
         
         self.assertFalse(True)
 
+    def get_signing_key(self):
+        return read_data_from_binary_file('tests/resources/certs/testSigningKey.p8')
     
     def get_client_with_body(self, body: str, expected_method: str, expected_url: str, expected_params: Dict[str, Union[str, List[str]]], expected_json: Dict[str, Any], status_code: int = 200):
-        signing_key = read_data_from_binary_file('tests/resources/certs/testSigningKey.p8')
+        signing_key = self.get_signing_key()
         client = AppStoreServerAPIClient(signing_key, 'keyId', 'issuerId', 'com.example', Environment.LOCAL_TESTING)
         def fake_execute_and_validate_inputs(method: bytes, url: str, params: Dict[str, Union[str, List[str]]], headers: Dict[str, str], json: Dict[str, Any]):
             self.assertEqual(expected_method, method)
             self.assertEqual(expected_url, url)
             self.assertEqual(expected_params, params)
             self.assertEqual(['User-Agent', 'Authorization', 'Accept'], list(headers.keys()))
             self.assertEqual('application/json', headers['Accept'])
```

### Comparing `app-store-server-library-1.1.0/tests/test_decoded_payloads.py` & `app_store_server_library-1.2.0/tests/test_decoded_payloads.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
 
 from typing import Optional
 import unittest
 from appstoreserverlibrary.models.AutoRenewStatus import AutoRenewStatus
+from appstoreserverlibrary.models.ConsumptionRequestReason import ConsumptionRequestReason
 from appstoreserverlibrary.models.Environment import Environment
 from appstoreserverlibrary.models.ExpirationIntent import ExpirationIntent
 from appstoreserverlibrary.models.InAppOwnershipType import InAppOwnershipType
 from appstoreserverlibrary.models.NotificationTypeV2 import NotificationTypeV2
 from appstoreserverlibrary.models.OfferDiscountType import OfferDiscountType
 from appstoreserverlibrary.models.OfferType import OfferType
 from appstoreserverlibrary.models.PriceIncreaseStatus import PriceIncreaseStatus
@@ -103,15 +104,15 @@
         self.assertEqual("abc.123", renewal_info.offerIdentifier)
         self.assertEqual(1698148800000, renewal_info.signedDate)
         self.assertEqual(Environment.LOCAL_TESTING, renewal_info.environment)
         self.assertEqual("LocalTesting", renewal_info.rawEnvironment)
         self.assertEqual(1698148800000, renewal_info.recentSubscriptionStartDate)
         self.assertEqual(1698148850000, renewal_info.renewalDate)
 
-    def test_notificaiton_decoding(self):
+    def test_notification_decoding(self):
         signed_notification = create_signed_data_from_json('tests/resources/models/signedNotification.json')
         
         signed_data_verifier = get_default_signed_data_verifier()
 
         notification = signed_data_verifier.verify_and_decode_notification(signed_notification)
 
         self.assertEqual(NotificationTypeV2.SUBSCRIBED, notification.notificationType)
@@ -129,14 +130,45 @@
         self.assertEqual(41234, notification.data.appAppleId)
         self.assertEqual("com.example", notification.data.bundleId)
         self.assertEqual("1.2.3", notification.data.bundleVersion)
         self.assertEqual("signed_transaction_info_value", notification.data.signedTransactionInfo)
         self.assertEqual("signed_renewal_info_value", notification.data.signedRenewalInfo);
         self.assertEqual(Status.ACTIVE, notification.data.status)
         self.assertEqual(1, notification.data.rawStatus)
+        self.assertIsNone(notification.data.consumptionRequestReason)
+        self.assertIsNone(notification.data.rawConsumptionRequestReason)
+
+    def test_consumption_request_notification_decoding(self):
+        signed_notification = create_signed_data_from_json('tests/resources/models/signedConsumptionRequestNotification.json')
+        
+        signed_data_verifier = get_default_signed_data_verifier()
+
+        notification = signed_data_verifier.verify_and_decode_notification(signed_notification)
+
+        self.assertEqual(NotificationTypeV2.CONSUMPTION_REQUEST, notification.notificationType)
+        self.assertEqual("CONSUMPTION_REQUEST", notification.rawNotificationType)
+        self.assertIsNone(notification.subtype)
+        self.assertIsNone(notification.rawSubtype)
+        self.assertEqual("002e14d5-51f5-4503-b5a8-c3a1af68eb20", notification.notificationUUID)
+        self.assertEqual("2.0", notification.version)
+        self.assertEqual(1698148900000, notification.signedDate)
+        self.assertIsNotNone(notification.data)
+        self.assertIsNone(notification.summary)
+        self.assertIsNone(notification.externalPurchaseToken)
+        self.assertEqual(Environment.LOCAL_TESTING, notification.data.environment)
+        self.assertEqual("LocalTesting", notification.data.rawEnvironment)
+        self.assertEqual(41234, notification.data.appAppleId)
+        self.assertEqual("com.example", notification.data.bundleId)
+        self.assertEqual("1.2.3", notification.data.bundleVersion)
+        self.assertEqual("signed_transaction_info_value", notification.data.signedTransactionInfo)
+        self.assertEqual("signed_renewal_info_value", notification.data.signedRenewalInfo);
+        self.assertEqual(Status.ACTIVE, notification.data.status)
+        self.assertEqual(1, notification.data.rawStatus)
+        self.assertEqual(ConsumptionRequestReason.UNINTENDED_PURCHASE, notification.data.consumptionRequestReason)
+        self.assertEqual("UNINTENDED_PURCHASE", notification.data.rawConsumptionRequestReason)
         
     def test_summary_notification_decoding(self):
         signed_summary_notification = create_signed_data_from_json('tests/resources/models/signedSummaryNotification.json')
         
         signed_data_verifier = get_default_signed_data_verifier()
 
         notification = signed_data_verifier.verify_and_decode_notification(signed_summary_notification)
```

### Comparing `app-store-server-library-1.1.0/tests/test_payload_verification.py` & `app_store_server_library-1.2.0/tests/test_payload_verification.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/tests/test_promotional_offer_signature_creator.py` & `app_store_server_library-1.2.0/tests/test_promotional_offer_signature_creator.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/tests/test_receipt_utility.py` & `app_store_server_library-1.2.0/tests/test_receipt_utility.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/tests/test_x509_verifiction.py` & `app_store_server_library-1.2.0/tests/test_x509_verifiction.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-1.1.0/tests/test_xcode_signed_data.py` & `app_store_server_library-1.2.0/tests/test_xcode_signed_data.py`

 * *Files identical despite different names*

