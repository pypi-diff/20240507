# Comparing `tmp/garpix_order-1.0.0rc3.tar.gz` & `tmp/garpix_order-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_order-1.0.0rc3.tar", last modified: Thu Sep 14 09:05:54 2023, max compression
+gzip compressed data, was "garpix_order-1.0.0rc4.tar", last modified: Tue May  7 10:32:24 2024, max compression
```

## Comparing `garpix_order-1.0.0rc3.tar` & `garpix_order-1.0.0rc4.tar`

### file list

```diff
@@ -1,101 +1,72 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.126942 garpix_order-1.0.0rc3/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       64 2023-09-14 09:05:54.000000 garpix_order-1.0.0rc3/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1531 2023-09-14 09:05:54.126082 garpix_order-1.0.0rc3/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.096485 garpix_order-1.0.0rc3/garpix_order/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       64 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc3/garpix_order/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      963 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      462 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc3/garpix_order/README.rst
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       59 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.098795 garpix_order-1.0.0rc3/garpix_order/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      225 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      499 2023-07-04 08:03:22.000000 garpix_order-1.0.0rc3/garpix_order/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      744 2023-09-14 09:05:53.000000 garpix_order-1.0.0rc3/garpix_order/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      452 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/__pycache__/utils.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.099199 garpix_order-1.0.0rc3/garpix_order/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc3/garpix_order/admin/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.099331 garpix_order-1.0.0rc3/garpix_order/admin/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      173 2023-07-03 13:24:04.000000 garpix_order-1.0.0rc3/garpix_order/admin/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc3/garpix_order/admin/home_page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      207 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/admin/recurring.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      184 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc3/garpix_order/apps.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.102198 garpix_order-1.0.0rc3/garpix_order/migrations/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6932 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/migrations/0001_initial.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2607 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/migrations/0002_auto_20230703_1624.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      803 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/migrations/0003_robokassainvoice.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc3/garpix_order/migrations/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.103000 garpix_order-1.0.0rc3/garpix_order/migrations/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3139 2023-07-03 13:24:04.000000 garpix_order-1.0.0rc3/garpix_order/migrations/__pycache__/0001_squashed_0008_auto_20211105_1533.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2000 2023-07-03 13:30:54.000000 garpix_order-1.0.0rc3/garpix_order/migrations/__pycache__/0002_auto_20230703_1624.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      939 2023-07-03 13:31:02.000000 garpix_order-1.0.0rc3/garpix_order/migrations/__pycache__/0003_robokassainvoice.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      178 2023-07-03 13:24:04.000000 garpix_order-1.0.0rc3/garpix_order/migrations/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.103745 garpix_order-1.0.0rc3/garpix_order/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      209 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/models/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.104617 garpix_order-1.0.0rc3/garpix_order/models/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      435 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      856 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/models/__pycache__/config.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4227 2023-07-03 13:23:09.000000 garpix_order-1.0.0rc3/garpix_order/models/__pycache__/invoice.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4433 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/models/__pycache__/order.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1438 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/models/__pycache__/order_item.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5559 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/models/__pycache__/payment.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      468 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/models/config.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4210 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/models/order.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      789 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/models/order_item.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5279 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/models/payment.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.109365 garpix_order-1.0.0rc3/garpix_order/models/payments/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      149 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/models/payments/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.111618 garpix_order-1.0.0rc3/garpix_order/models/payments/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      372 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/models/payments/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      685 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/models/payments/__pycache__/bank_card.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      642 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/models/payments/__pycache__/cash.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1581 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/models/payments/__pycache__/cloudpayments.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2297 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/models/payments/__pycache__/recurring.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1996 2023-09-14 09:05:53.000000 garpix_order-1.0.0rc3/garpix_order/models/payments/__pycache__/robokassa.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      241 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/models/payments/bank_card.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      207 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/models/payments/cash.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1338 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/models/payments/cloudpayments.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1874 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/models/payments/recurring.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1559 2023-07-27 15:18:50.000000 garpix_order-1.0.0rc3/garpix_order/models/payments/robokassa.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      100 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc3/garpix_order/pyproject.toml
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.111884 garpix_order-1.0.0rc3/garpix_order/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/serializers/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.112239 garpix_order-1.0.0rc3/garpix_order/serializers/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      275 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/serializers/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      952 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/serializers/__pycache__/robokassa.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      419 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/serializers/robokassa.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.112517 garpix_order-1.0.0rc3/garpix_order/services/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/services/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.113519 garpix_order-1.0.0rc3/garpix_order/services/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/services/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3716 2023-09-14 09:05:53.000000 garpix_order-1.0.0rc3/garpix_order/services/__pycache__/robokassa.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3536 2023-07-27 15:18:50.000000 garpix_order-1.0.0rc3/garpix_order/services/robokassa.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1151 2023-09-14 09:05:34.000000 garpix_order-1.0.0rc3/garpix_order/setup.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     7708 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/tests.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      584 2023-09-14 09:04:26.000000 garpix_order-1.0.0rc3/garpix_order/urls.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/utils.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.113897 garpix_order-1.0.0rc3/garpix_order/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       37 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/views/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.114456 garpix_order-1.0.0rc3/garpix_order/views/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      220 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/views/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.121443 garpix_order-1.0.0rc3/garpix_order/views/cloudpayments/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5754 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/views/cloudpayments/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.121588 garpix_order-1.0.0rc3/garpix_order/views/cloudpayments/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5051 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/views/cloudpayments/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1239 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/views/cloudpayments/default_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       98 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc3/garpix_order/views/cloudpayments/fail.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       97 2023-06-28 21:07:27.000000 garpix_order-1.0.0rc3/garpix_order/views/cloudpayments/pay.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/views/cloudpayments/payment_data.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.121904 garpix_order-1.0.0rc3/garpix_order/views/robokassa/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/views/robokassa/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.123687 garpix_order-1.0.0rc3/garpix_order/views/robokassa/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      228 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/views/robokassa/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2053 2023-07-27 14:04:06.000000 garpix_order-1.0.0rc3/garpix_order/views/robokassa/__pycache__/payment.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1553 2023-07-27 14:02:51.000000 garpix_order-1.0.0rc3/garpix_order/views/robokassa/payment.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-09-14 09:05:54.097435 garpix_order-1.0.0rc3/garpix_order.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1531 2023-09-14 09:05:54.000000 garpix_order-1.0.0rc3/garpix_order.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3379 2023-09-14 09:05:54.000000 garpix_order-1.0.0rc3/garpix_order.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-09-14 09:05:54.000000 garpix_order-1.0.0rc3/garpix_order.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-09-14 09:05:54.000000 garpix_order-1.0.0rc3/garpix_order.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       56 2023-09-14 09:05:54.000000 garpix_order-1.0.0rc3/garpix_order.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       13 2023-09-14 09:05:54.000000 garpix_order-1.0.0rc3/garpix_order.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-09-14 09:05:54.128447 garpix_order-1.0.0rc3/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1151 2023-09-14 09:05:54.000000 garpix_order-1.0.0rc3/setup.py
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.649078 garpix_order-1.0.0rc4/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       64 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/MANIFEST.in
+-rw-r--r--   0 crusat    (1000) crusat    (1000)      638 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/PKG-INFO
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.637078 garpix_order-1.0.0rc4/garpix_order/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       64 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/MANIFEST.in
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      462 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/README.rst
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       59 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/__init__.py
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.637078 garpix_order-1.0.0rc4/garpix_order/admin/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/admin/__init__.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       77 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/admin/home_page.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      207 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/admin/recurring.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      184 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/apps.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      531 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/exceptions.py
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.637078 garpix_order-1.0.0rc4/garpix_order/logging/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       23 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/logging/__init__.py
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.637078 garpix_order-1.0.0rc4/garpix_order/logging/filters/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       60 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/logging/filters/__init__.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      365 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/logging/filters/payment_auth_data_filter.py
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.641078 garpix_order-1.0.0rc4/garpix_order/migrations/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     6932 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/migrations/0001_initial.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     2607 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/migrations/0002_auto_20230703_1624.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      803 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/migrations/0003_robokassainvoice.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/migrations/__init__.py
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.641078 garpix_order-1.0.0rc4/garpix_order/models/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      257 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/__init__.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      468 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/config.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     4210 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/order.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      789 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/order_item.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     5279 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payment.py
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.641078 garpix_order-1.0.0rc4/garpix_order/models/payments/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      206 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/__init__.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      241 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/bank_card.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      207 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/cash.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     1338 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/cloudpayments.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     1874 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/recurring.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     1589 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/robokassa.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     1612 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/sber.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      100 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/pyproject.toml
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.641078 garpix_order-1.0.0rc4/garpix_order/serializers/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       77 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/serializers/__init__.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      419 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/serializers/robokassa.py
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/garpix_order/services/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/services/__init__.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     3577 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/services/robokassa.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     9124 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/services/sber.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     1154 2024-05-07 10:28:21.000000 garpix_order-1.0.0rc4/garpix_order/setup.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     7708 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/tests.py
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/garpix_order/types/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       20 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/types/__init__.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     1285 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/types/sber.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      515 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/urls.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      219 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/utils.py
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/garpix_order/views/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       37 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/__init__.py
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     5754 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/__init__.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     1239 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/default_view.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       98 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/fail.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       97 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/pay.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)      710 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/payment_data.py
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/garpix_order/views/robokassa/
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       35 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/robokassa/__init__.py
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     1553 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/robokassa/payment.py
+drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/garpix_order.egg-info/
+-rw-r--r--   0 crusat    (1000) crusat    (1000)      638 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/garpix_order.egg-info/PKG-INFO
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     1884 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/garpix_order.egg-info/SOURCES.txt
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)        1 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/garpix_order.egg-info/dependency_links.txt
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)        1 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/garpix_order.egg-info/not-zip-safe
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       38 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/garpix_order.egg-info/requires.txt
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       13 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/garpix_order.egg-info/top_level.txt
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)       38 2024-05-07 10:32:24.649078 garpix_order-1.0.0rc4/setup.cfg
+-rw-rw-r--   0 crusat    (1000) crusat    (1000)     1154 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/setup.py
```

### Comparing `garpix_order-1.0.0rc3/garpix_order/migrations/0001_initial.py` & `garpix_order-1.0.0rc4/garpix_order/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc3/garpix_order/migrations/0002_auto_20230703_1624.py` & `garpix_order-1.0.0rc4/garpix_order/migrations/0002_auto_20230703_1624.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc3/garpix_order/migrations/0003_robokassainvoice.py` & `garpix_order-1.0.0rc4/garpix_order/migrations/0003_robokassainvoice.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc3/garpix_order/models/order.py` & `garpix_order-1.0.0rc4/garpix_order/models/order.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc3/garpix_order/models/order_item.py` & `garpix_order-1.0.0rc4/garpix_order/models/order_item.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc3/garpix_order/models/payment.py` & `garpix_order-1.0.0rc4/garpix_order/models/payment.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc3/garpix_order/models/payments/cloudpayments.py` & `garpix_order-1.0.0rc4/garpix_order/models/payments/cloudpayments.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc3/garpix_order/models/payments/recurring.py` & `garpix_order-1.0.0rc4/garpix_order/models/payments/recurring.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc3/garpix_order/models/payments/robokassa.py` & `garpix_order-1.0.0rc4/garpix_order/models/payments/robokassa.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from datetime import datetime
+
 from ..payment import BasePayment
-from garpix_order.services.robokassa import RobokassaService
+from garpix_order.services.robokassa import robokassa_service
 
 
 class RobokassaPayment(BasePayment):
     class Meta:
         verbose_name = 'Платеж Robokassa'
         verbose_name_plural = 'Платежи Robokassa'
 
@@ -15,15 +17,15 @@
         if self.amount == 0:
             msg = 'It is not possible to pay 0 amount'
             self.set_provider_data({'msg': msg})
             self.failed()
             self.save()
             return False, msg
 
-        res, msg = RobokassaService().check_success_payment(self, data)
+        res, msg = robokassa_service.check_success_payment(self, data)
         if not res:
             self.set_provider_data({'msg': msg})
             self.failed()
             self.save()
             return False, msg
         self.succeeded()
         self.order.pay(self.amount)
@@ -41,8 +43,8 @@
 
     def cancel(self):
         self.set_provider_data({'msg': 'Payment is canceled'})
         self.canceled()
         self.save()
 
     def generate_payment_link(self):
-        return RobokassaService().generate_payment_link(self)
+        return robokassa_service.generate_payment_link(self)
```

### Comparing `garpix_order-1.0.0rc3/garpix_order/services/robokassa.py` & `garpix_order-1.0.0rc4/garpix_order/services/robokassa.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,7 +81,10 @@
         recurring_objs = Recurring.active_objects.filter(payment_system=Recurring.RecurringPaymentSystem.ROBOKASSA,
                                                          end_at__gt=datetime.now())
         orders_to_pay = BaseOrder.objects.filter(recurring__in=recurring_objs, next_payment_date=datetime.now())
 
         for obj in orders_to_pay:
             payment = RobokassaPayment.objects.create(order=obj, amount=obj.total_amount, payment_type=RobokassaPayment.PaymentType.AUTO)
             payment.pay(data={}, auto=True)
+
+
+robokassa_service = RobokassaService()
```

### Comparing `garpix_order-1.0.0rc3/garpix_order/setup.py` & `garpix_order-1.0.0rc4/garpix_order/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 from os import path
+#from m2r import convert
+from django.conf import settings
 
 
-here = path.join(path.abspath(path.dirname(__file__)), 'garpix_order')
-
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
+#with open(path.join(settings.BASE_DIR, '..', 'README.md'), encoding='utf-8') as f:
+#    long_description = convert(f.read())
 
 setup(
     name='garpix_order',
-    version='1.0.0-rc3',
+    version='1.0.0-rc4',
     description='',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
+#    long_description=long_description,
+    long_description='https://github.com/garpixcms/garpix_order',
     url='https://github.com/garpixcms/garpix_order',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(exclude=['testproject', 'testproject.*']),
     classifiers=[
         'Development Status :: 4 - Beta',
@@ -29,10 +29,9 @@
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 1.11',
         'djangorestframework >= 3.8',
-        'django-fsm >= 2.8.1'
     ],
-)
+)
```

### Comparing `garpix_order-1.0.0rc3/garpix_order/tests.py` & `garpix_order-1.0.0rc4/garpix_order/tests.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc3/garpix_order/views/cloudpayments/__init__.py` & `garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc3/garpix_order/views/cloudpayments/default_view.py` & `garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/default_view.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc3/garpix_order/views/cloudpayments/payment_data.py` & `garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/payment_data.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc3/garpix_order/views/robokassa/payment.py` & `garpix_order-1.0.0rc4/garpix_order/views/robokassa/payment.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc3/setup.py` & `garpix_order-1.0.0rc4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 from os import path
+#from m2r import convert
+from django.conf import settings
 
 
-here = path.join(path.abspath(path.dirname(__file__)), 'garpix_order')
-
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
+#with open(path.join(settings.BASE_DIR, '..', 'README.md'), encoding='utf-8') as f:
+#    long_description = convert(f.read())
 
 setup(
     name='garpix_order',
-    version='1.0.0-rc3',
+    version='1.0.0-rc4',
     description='',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
+#    long_description=long_description,
+    long_description='https://github.com/garpixcms/garpix_order',
     url='https://github.com/garpixcms/garpix_order',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(exclude=['testproject', 'testproject.*']),
     classifiers=[
         'Development Status :: 4 - Beta',
@@ -29,10 +29,9 @@
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 1.11',
         'djangorestframework >= 3.8',
-        'django-fsm >= 2.8.1'
     ],
-)
+)
```

