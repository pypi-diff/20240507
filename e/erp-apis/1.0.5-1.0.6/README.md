# Comparing `tmp/erp_apis-1.0.5-py3-none-any.whl.zip` & `tmp/erp_apis-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,17 @@
-Zip file size: 9613 bytes, number of entries: 13
+Zip file size: 10979 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat      403 b- defN 24-May-06 06:32 erp_apis/config.py
--rw-rw-rw-  2.0 fat     3490 b- defN 24-May-07 03:18 erp_apis/erpRequest.py
--rw-rw-rw-  2.0 fat      141 b- defN 24-Apr-29 06:37 erp_apis/apis/__init__.py
--rw-rw-rw-  2.0 fat     2569 b- defN 24-May-07 03:18 erp_apis/apis/afterSales.py
+-rw-rw-rw-  2.0 fat     3490 b- defN 24-May-07 06:01 erp_apis/erpRequest.py
+-rw-rw-rw-  2.0 fat      143 b- defN 24-May-07 03:26 erp_apis/apis/__init__.py
+-rw-rw-rw-  2.0 fat     2578 b- defN 24-May-07 03:26 erp_apis/apis/afterSales.py
 -rw-rw-rw-  2.0 fat     1520 b- defN 24-May-07 03:18 erp_apis/apis/goods.py
 -rw-rw-rw-  2.0 fat     1013 b- defN 24-May-07 03:18 erp_apis/apis/inventory.py
 -rw-rw-rw-  2.0 fat     3683 b- defN 24-May-07 03:18 erp_apis/apis/order.py
--rw-rw-rw-  2.0 fat     1956 b- defN 24-May-07 03:18 erp_apis/apis/test.py
+-rw-rw-rw-  2.0 fat     1976 b- defN 24-May-07 03:19 erp_apis/apis/test.py
 -rw-rw-rw-  2.0 fat      780 b- defN 24-May-07 03:18 erp_apis/apis/user.py
--rw-rw-rw-  2.0 fat     1580 b- defN 24-May-07 03:19 erp_apis-1.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 03:19 erp_apis-1.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 24-May-07 03:19 erp_apis-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1016 b- defN 24-May-07 03:19 erp_apis-1.0.5.dist-info/RECORD
-13 files, 18266 bytes uncompressed, 7931 bytes compressed:  56.6%
+-rw-rw-rw-  2.0 fat      141 b- defN 24-Apr-30 10:11 erp_apis/utils/__init__.py
+-rw-rw-rw-  2.0 fat     2042 b- defN 24-May-06 03:23 erp_apis/utils/util.py
+-rw-rw-rw-  2.0 fat     1580 b- defN 24-May-07 06:02 erp_apis-1.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 06:02 erp_apis-1.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       38 b- defN 24-May-07 06:02 erp_apis-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1177 b- defN 24-May-07 06:02 erp_apis-1.0.6.dist-info/RECORD
+15 files, 20656 bytes uncompressed, 9049 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -21,20 +21,26 @@
 
 Filename: erp_apis/apis/test.py
 Comment: 
 
 Filename: erp_apis/apis/user.py
 Comment: 
 
-Filename: erp_apis-1.0.5.dist-info/METADATA
+Filename: erp_apis/utils/__init__.py
 Comment: 
 
-Filename: erp_apis-1.0.5.dist-info/WHEEL
+Filename: erp_apis/utils/util.py
 Comment: 
 
-Filename: erp_apis-1.0.5.dist-info/top_level.txt
+Filename: erp_apis-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: erp_apis-1.0.5.dist-info/RECORD
+Filename: erp_apis-1.0.6.dist-info/WHEEL
+Comment: 
+
+Filename: erp_apis-1.0.6.dist-info/top_level.txt
+Comment: 
+
+Filename: erp_apis-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## erp_apis/apis/__init__.py

```diff
@@ -1,6 +1,7 @@
 # coding: utf-8
 # Project：erp_sdk_python
 # File：__init__.py.py
 # Author：李福成
 # Date ：2024/4/29 下午2:37
 # IDE：PyCharm
+
```

## erp_apis/apis/afterSales.py

```diff
@@ -2,15 +2,15 @@
 # Project：erp_out_of_stock
 # File：order.py
 # Author：李福成
 # Date ：2024-04-28 18:23
 # IDE：PyCharm
 # 订单API
 from typing import Optional, Union
-from erpRequest import Request
+from erp_apis.erpRequest import Request
 from utils.util import dumps, getDefaultParams, JTable1, generateChangeBatchItems
 
 
 def AftersaleRequest(data: dict, method: str = 'LoadDataToJSON',
                  url: str = '/app/Service/aftersale/aftersale.aspx', **kwargs) -> Request:
     params = getDefaultParams({'defaultParams': ["ts___"], 'am___': method})
     if kwargs.get('params'):
```

## erp_apis/apis/test.py

```diff
@@ -10,16 +10,16 @@
 from apis.afterSales import aftersaleList, aftersaleCommon, clearException
 from apis.goods import ItemList
 from erpRequest import Session
 
 if __name__ == '__main__':
     session = Session()
     session.erpSend(login(
-        username="",
-        password=""
+        username="18986660202",
+        password="lfc199968"
     ))
     # 获取分仓库存
     # order = session.erpSend(OrderList(queryData=[{"k": "o_id", "v": "39104496", "c": "@="}])).json()['ReturnValue']['datas'][0]
     # print(order)
     # res = session.erpSend(ChangeBatchItems(
     #     oid = order['o_id'],
     #     items = order['items'],
```

## Comparing `erp_apis-1.0.5.dist-info/METADATA` & `erp_apis-1.0.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erp-apis
-Version: 1.0.5
+Version: 1.0.6
 Summary: erp_apis
 Home-page: https://gitee.com/li_fucheng/erp_sdk_python
 Author: 李福成
 Author-email: lfct@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://gitee.com/li_fucheng/erp_sdk_python/issues
 Project-URL: Documentation, https://gitee.com/li_fucheng/erp_sdk_python
```

## Comparing `erp_apis-1.0.5.dist-info/RECORD` & `erp_apis-1.0.6.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 erp_apis/config.py,sha256=tXtGQtsW-Wdbhh2X1AKyGx_X8B_ShMvdVF4rOXf8zDg,403
 erp_apis/erpRequest.py,sha256=LPW_CjrZcwD0f7zwItOTUUqFE-hRggbFG-ZO9yP1TgU,3490
-erp_apis/apis/__init__.py,sha256=mP4VQl6EDhiYFTvOeAO7G4N6a5xtWXrXG5gRyW4HfQg,141
-erp_apis/apis/afterSales.py,sha256=MzXkqjpkA4ufZsp9-aVLAWjmgMWQLs9Uy8RwGbT0iVI,2569
+erp_apis/apis/__init__.py,sha256=L6HaO-zN2-mMbaZUFJ8YFFgFScFE4aizJCVPed8CluY,143
+erp_apis/apis/afterSales.py,sha256=ucr1jLUZ3-Rozj1DPmA_pipiJew1aBkvqQZDzSFHcSw,2578
 erp_apis/apis/goods.py,sha256=ms8XCmxYEgrtmWsaaRny7NF9nXJKfgh30U5oo06hbvE,1520
 erp_apis/apis/inventory.py,sha256=ktCBMrKRdHKSOKZIgCCWan0cTYNKm-ddpFNe1hkxgGk,1013
 erp_apis/apis/order.py,sha256=QeKVC_N5K1sNtKBP1LF09JgLHC2-HE-XWujbS8SFvFs,3683
-erp_apis/apis/test.py,sha256=h1mhASQedjK70saeZr2bpa31Nm6W2a6LLuFJOi68mSc,1956
+erp_apis/apis/test.py,sha256=vSVMHKRcq1tjNShaJ6QZPAvSKx6sgw6GQX1FCK8RXQ0,1976
 erp_apis/apis/user.py,sha256=JTdaWgG4Ly4KQdA2-Z3tdDiiNMJDy4LCKBbIa2BKNqs,780
-erp_apis-1.0.5.dist-info/METADATA,sha256=UiJkmOCrsj6JAKZOuj5ggVw_w-CbC46Sor2wtRBT5j8,1580
-erp_apis-1.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-erp_apis-1.0.5.dist-info/top_level.txt,sha256=i_r33fdpLh_LFdzZEdgEk4155_iw3lEof10yhsc5_MA,23
-erp_apis-1.0.5.dist-info/RECORD,,
+erp_apis/utils/__init__.py,sha256=4OS0q-GbgI0b14i4ErUYKUo-t1jzw8wSvtJZu3nXSMM,141
+erp_apis/utils/util.py,sha256=FL8-Mo2CZWR-Pv09hqxgTE7oQVhNt6tl2AJolFdZE30,2042
+erp_apis-1.0.6.dist-info/METADATA,sha256=SdeCOPf587SvF0ASfR4O2YdbHXQR4TqlHHgz41RrfMw,1580
+erp_apis-1.0.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+erp_apis-1.0.6.dist-info/top_level.txt,sha256=vqDQIzqoC9jLUmJwUdHu1qRTGhYD1SxQ5BsetWAnMrs,38
+erp_apis-1.0.6.dist-info/RECORD,,
```

