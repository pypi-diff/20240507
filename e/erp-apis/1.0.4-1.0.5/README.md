# Comparing `tmp/erp_apis-1.0.4-py3-none-any.whl.zip` & `tmp/erp_apis-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9599 bytes, number of entries: 13
+Zip file size: 9613 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat      403 b- defN 24-May-06 06:32 erp_apis/config.py
--rw-rw-rw-  2.0 fat     3492 b- defN 24-May-06 07:28 erp_apis/request.py
+-rw-rw-rw-  2.0 fat     3490 b- defN 24-May-07 03:18 erp_apis/erpRequest.py
 -rw-rw-rw-  2.0 fat      141 b- defN 24-Apr-29 06:37 erp_apis/apis/__init__.py
--rw-rw-rw-  2.0 fat     2566 b- defN 24-May-07 01:25 erp_apis/apis/afterSales.py
--rw-rw-rw-  2.0 fat     1517 b- defN 24-May-07 02:48 erp_apis/apis/goods.py
--rw-rw-rw-  2.0 fat     1010 b- defN 24-Apr-30 10:14 erp_apis/apis/inventory.py
--rw-rw-rw-  2.0 fat     3680 b- defN 24-May-05 08:01 erp_apis/apis/order.py
--rw-rw-rw-  2.0 fat     1953 b- defN 24-May-07 02:48 erp_apis/apis/test.py
--rw-rw-rw-  2.0 fat      777 b- defN 24-Apr-30 11:33 erp_apis/apis/user.py
--rw-rw-rw-  2.0 fat     1580 b- defN 24-May-07 03:01 erp_apis-1.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 03:01 erp_apis-1.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 24-May-07 03:01 erp_apis-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1013 b- defN 24-May-07 03:01 erp_apis-1.0.4.dist-info/RECORD
-13 files, 18247 bytes uncompressed, 7923 bytes compressed:  56.6%
+-rw-rw-rw-  2.0 fat     2569 b- defN 24-May-07 03:18 erp_apis/apis/afterSales.py
+-rw-rw-rw-  2.0 fat     1520 b- defN 24-May-07 03:18 erp_apis/apis/goods.py
+-rw-rw-rw-  2.0 fat     1013 b- defN 24-May-07 03:18 erp_apis/apis/inventory.py
+-rw-rw-rw-  2.0 fat     3683 b- defN 24-May-07 03:18 erp_apis/apis/order.py
+-rw-rw-rw-  2.0 fat     1956 b- defN 24-May-07 03:18 erp_apis/apis/test.py
+-rw-rw-rw-  2.0 fat      780 b- defN 24-May-07 03:18 erp_apis/apis/user.py
+-rw-rw-rw-  2.0 fat     1580 b- defN 24-May-07 03:19 erp_apis-1.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 03:19 erp_apis-1.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 24-May-07 03:19 erp_apis-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1016 b- defN 24-May-07 03:19 erp_apis-1.0.5.dist-info/RECORD
+13 files, 18266 bytes uncompressed, 7931 bytes compressed:  56.6%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: erp_apis/config.py
 Comment: 
 
-Filename: erp_apis/request.py
+Filename: erp_apis/erpRequest.py
 Comment: 
 
 Filename: erp_apis/apis/__init__.py
 Comment: 
 
 Filename: erp_apis/apis/afterSales.py
 Comment: 
@@ -21,20 +21,20 @@
 
 Filename: erp_apis/apis/test.py
 Comment: 
 
 Filename: erp_apis/apis/user.py
 Comment: 
 
-Filename: erp_apis-1.0.4.dist-info/METADATA
+Filename: erp_apis-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: erp_apis-1.0.4.dist-info/WHEEL
+Filename: erp_apis-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: erp_apis-1.0.4.dist-info/top_level.txt
+Filename: erp_apis-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: erp_apis-1.0.4.dist-info/RECORD
+Filename: erp_apis-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
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
-from request import Request
+from erpRequest import Request
 from utils.util import dumps, getDefaultParams, JTable1, generateChangeBatchItems
 
 
 def AftersaleRequest(data: dict, method: str = 'LoadDataToJSON',
                  url: str = '/app/Service/aftersale/aftersale.aspx', **kwargs) -> Request:
     params = getDefaultParams({'defaultParams': ["ts___"], 'am___': method})
     if kwargs.get('params'):
```

## erp_apis/apis/goods.py

```diff
@@ -2,15 +2,15 @@
 # Project：erp_sdk_python
 # File：itemtool.py
 # Author：李福成
 # Date ：2024/5/7 上午10:42
 # IDE：PyCharm
 from typing import Optional
 
-from request import Request
+from erpRequest import Request
 from utils.util import getDefaultParams, JTable1, dumps
 
 
 def ItemtoolRequest(
         data: dict,
         method: str = 'LoadDataToJSON',
         url: str = '/app/item/itemtool/itemContrast.aspx', **kwargs
```

## erp_apis/apis/inventory.py

```diff
@@ -2,15 +2,15 @@
 # Project：erp_out_of_stock
 # File：inventory.py
 # Author：李福成
 # Date ：2024-04-28 18:27
 # IDE：PyCharm
 # 库存
 from typing import Optional
-from request import Request
+from erpRequest import Request
 from utils.util import getDefaultParams, dumps, JTable1
 
 
 # 查询库存
 def WmsSkuStock(queryData: Optional[list] = None, page_num: int = 1, page_size: int = 500):
     '''
     查询库存(分仓)
```

## erp_apis/apis/order.py

```diff
@@ -2,15 +2,15 @@
 # Project：erp_out_of_stock
 # File：order.py
 # Author：李福成
 # Date ：2024-04-28 18:23
 # IDE：PyCharm
 # 订单API
 from typing import Optional, Union
-from request import Request
+from erpRequest import Request
 from utils.util import dumps, getDefaultParams, JTable1, generateChangeBatchItems
 def OrderRequest(data: dict, method: str = 'LoadDataToJSON') -> Request:
     return Request(
         method='POST',
         url='/app/order/order/list.aspx',
         params=getDefaultParams({'defaultParams': ["ts___", "_c"], 'am___': method}),
         data={
```

## erp_apis/apis/test.py

```diff
@@ -5,15 +5,15 @@
 # Date ：2024-04-28 18:24
 # IDE：PyCharm
 from apis.inventory import WmsSkuStock
 from apis.order import OrderList, ChangeBatchItems
 from apis.user import login
 from apis.afterSales import aftersaleList, aftersaleCommon, clearException
 from apis.goods import ItemList
-from request import Session
+from erpRequest import Session
 
 if __name__ == '__main__':
     session = Session()
     session.erpSend(login(
         username="",
         password=""
     ))
```

## erp_apis/apis/user.py

```diff
@@ -2,15 +2,15 @@
 # Project：erp_out_of_stock
 # File：user.py
 # Author：李福成
 # Date ：2024-04-28 18:23
 # IDE：PyCharm
 # 用户API
 
-from request import Request
+from erpRequest import Request
 
 def login(username: str, password: str):
     '''
     登录
     :param username: 账号
     :param password: 密码
     :return:
```

## Comparing `erp_apis/request.py` & `erp_apis/erpRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # Author：李福成
 # Date ：2024-04-09 11:20
 # IDE：PyCharm
 import os
 from dataclasses import dataclass
 from typing import Optional
 from urllib.parse import urljoin
-
 from lxml import etree
 from requests import Session as S, Request as R
 import time, json as j
 from config import DEFAULT_HEADERS, Erp321BaseUrl, ErpApiBaseUrl
 
 
 @dataclass
```

## Comparing `erp_apis-1.0.4.dist-info/METADATA` & `erp_apis-1.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erp-apis
-Version: 1.0.4
+Version: 1.0.5
 Summary: erp_apis
 Home-page: https://gitee.com/li_fucheng/erp_sdk_python
 Author: 李福成
 Author-email: lfct@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://gitee.com/li_fucheng/erp_sdk_python/issues
 Project-URL: Documentation, https://gitee.com/li_fucheng/erp_sdk_python
```

## Comparing `erp_apis-1.0.4.dist-info/RECORD` & `erp_apis-1.0.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 erp_apis/config.py,sha256=tXtGQtsW-Wdbhh2X1AKyGx_X8B_ShMvdVF4rOXf8zDg,403
-erp_apis/request.py,sha256=GUvu9so9yn8VegOO6_EBRdlQAw5FvagkXlV33cFd4Ng,3492
+erp_apis/erpRequest.py,sha256=LPW_CjrZcwD0f7zwItOTUUqFE-hRggbFG-ZO9yP1TgU,3490
 erp_apis/apis/__init__.py,sha256=mP4VQl6EDhiYFTvOeAO7G4N6a5xtWXrXG5gRyW4HfQg,141
-erp_apis/apis/afterSales.py,sha256=zLQPY_P4D7rot_NxkSk845pBru1qGfbxOdbDo4qf84o,2566
-erp_apis/apis/goods.py,sha256=JggkrGbgSeVZQ1N9I56xBIs1LqBZVVssUpC4-CTF_Qk,1517
-erp_apis/apis/inventory.py,sha256=sLPIvOdKHIdfC0lAxtoK3ey8-n5OEbUsjFPX-_c6yY4,1010
-erp_apis/apis/order.py,sha256=6Z9HEfYeomktbIqGmQgEFYADa-XkBZEcVIeR-eLudco,3680
-erp_apis/apis/test.py,sha256=7xg6YNGhwp6UJiXCkL_KKnILyy9-WotbUnoYvHl8sp0,1953
-erp_apis/apis/user.py,sha256=Wcqqb8YWG7XsWWaTzSmF-N4FDO98L_Z4ECXSeWhKf_8,777
-erp_apis-1.0.4.dist-info/METADATA,sha256=874D-ogXx8lG38CuHjuBbubWG_-GAgDjFXyTold1PZ8,1580
-erp_apis-1.0.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-erp_apis-1.0.4.dist-info/top_level.txt,sha256=i_r33fdpLh_LFdzZEdgEk4155_iw3lEof10yhsc5_MA,23
-erp_apis-1.0.4.dist-info/RECORD,,
+erp_apis/apis/afterSales.py,sha256=MzXkqjpkA4ufZsp9-aVLAWjmgMWQLs9Uy8RwGbT0iVI,2569
+erp_apis/apis/goods.py,sha256=ms8XCmxYEgrtmWsaaRny7NF9nXJKfgh30U5oo06hbvE,1520
+erp_apis/apis/inventory.py,sha256=ktCBMrKRdHKSOKZIgCCWan0cTYNKm-ddpFNe1hkxgGk,1013
+erp_apis/apis/order.py,sha256=QeKVC_N5K1sNtKBP1LF09JgLHC2-HE-XWujbS8SFvFs,3683
+erp_apis/apis/test.py,sha256=h1mhASQedjK70saeZr2bpa31Nm6W2a6LLuFJOi68mSc,1956
+erp_apis/apis/user.py,sha256=JTdaWgG4Ly4KQdA2-Z3tdDiiNMJDy4LCKBbIa2BKNqs,780
+erp_apis-1.0.5.dist-info/METADATA,sha256=UiJkmOCrsj6JAKZOuj5ggVw_w-CbC46Sor2wtRBT5j8,1580
+erp_apis-1.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+erp_apis-1.0.5.dist-info/top_level.txt,sha256=i_r33fdpLh_LFdzZEdgEk4155_iw3lEof10yhsc5_MA,23
+erp_apis-1.0.5.dist-info/RECORD,,
```

