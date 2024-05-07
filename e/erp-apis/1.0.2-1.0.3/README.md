# Comparing `tmp/erp_apis-1.0.2-py3-none-any.whl.zip` & `tmp/erp_apis-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 8666 bytes, number of entries: 12
+Zip file size: 9599 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat      403 b- defN 24-May-06 06:32 erp_apis/config.py
--rw-rw-rw-  2.0 fat     3486 b- defN 24-May-06 05:56 erp_apis/request.py
+-rw-rw-rw-  2.0 fat     3492 b- defN 24-May-06 07:28 erp_apis/request.py
 -rw-rw-rw-  2.0 fat      141 b- defN 24-Apr-29 06:37 erp_apis/apis/__init__.py
--rw-rw-rw-  2.0 fat     2550 b- defN 24-May-06 06:31 erp_apis/apis/afterSales.py
+-rw-rw-rw-  2.0 fat     2566 b- defN 24-May-07 01:25 erp_apis/apis/afterSales.py
+-rw-rw-rw-  2.0 fat     1517 b- defN 24-May-07 02:48 erp_apis/apis/goods.py
 -rw-rw-rw-  2.0 fat     1010 b- defN 24-Apr-30 10:14 erp_apis/apis/inventory.py
 -rw-rw-rw-  2.0 fat     3680 b- defN 24-May-05 08:01 erp_apis/apis/order.py
--rw-rw-rw-  2.0 fat     1817 b- defN 24-May-06 06:32 erp_apis/apis/test.py
+-rw-rw-rw-  2.0 fat     1953 b- defN 24-May-07 02:48 erp_apis/apis/test.py
 -rw-rw-rw-  2.0 fat      777 b- defN 24-Apr-30 11:33 erp_apis/apis/user.py
--rw-rw-rw-  2.0 fat     1580 b- defN 24-May-06 06:33 erp_apis-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-06 06:33 erp_apis-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 24-May-06 06:33 erp_apis-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      934 b- defN 24-May-06 06:33 erp_apis-1.0.2.dist-info/RECORD
-12 files, 16493 bytes uncompressed, 7110 bytes compressed:  56.9%
+-rw-rw-rw-  2.0 fat     1580 b- defN 24-May-07 02:49 erp_apis-1.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 02:49 erp_apis-1.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 24-May-07 02:49 erp_apis-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1013 b- defN 24-May-07 02:49 erp_apis-1.0.3.dist-info/RECORD
+13 files, 18247 bytes uncompressed, 7923 bytes compressed:  56.6%
```

## zipnote {}

```diff
@@ -6,32 +6,35 @@
 
 Filename: erp_apis/apis/__init__.py
 Comment: 
 
 Filename: erp_apis/apis/afterSales.py
 Comment: 
 
+Filename: erp_apis/apis/goods.py
+Comment: 
+
 Filename: erp_apis/apis/inventory.py
 Comment: 
 
 Filename: erp_apis/apis/order.py
 Comment: 
 
 Filename: erp_apis/apis/test.py
 Comment: 
 
 Filename: erp_apis/apis/user.py
 Comment: 
 
-Filename: erp_apis-1.0.2.dist-info/METADATA
+Filename: erp_apis-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: erp_apis-1.0.2.dist-info/WHEEL
+Filename: erp_apis-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: erp_apis-1.0.2.dist-info/top_level.txt
+Filename: erp_apis-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: erp_apis-1.0.2.dist-info/RECORD
+Filename: erp_apis-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## erp_apis/request.py

```diff
@@ -33,15 +33,15 @@
         self.headers.update(DEFAULT_HEADERS)
         self.proxies = {'http': "", 'https': ""}
         self.viewstateItems = dict()
         self.userInfo : Optional[UserInfoType]
 
 
 
-    def erpSend(self, request:R, **kwargs):
+    def erpSend(self, request:R, **kwargs) -> R:
         if not request.headers: request.headers = self.headers
         hostType = getattr(request, 'hostType', None)
         if hostType:
             resp = getattr(self, hostType + "Send", None)(request, **kwargs)
             if resp is None:
                 raise Exception(f"{hostType}没有这个域的send方法")
             return resp
@@ -54,15 +54,15 @@
             request.headers.update({'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8'})
             request.data.update({k: v for k, v in self.get_viewstate(request.url).items() if k and k != "updateTime"})
         res = super().send(self.prepare_request(request), **kwargs)
         if request.callback:
             return request.callback(res)
         return res
 
-    def erpApiSend(self, request, **kwargs):
+    def erpApiSend(self, request, **kwargs) :
         request.url = urljoin(ErpApiBaseUrl, request.url)
         res = super().send(self.prepare_request(request), **kwargs)
         if request.callback:
             if request.callback == 'login':
                 self.userInfo = UserInfoType(**res.json().get('cookie'))
             else:
                 return request.callback(res)
```

## erp_apis/apis/afterSales.py

```diff
@@ -6,15 +6,15 @@
 # IDE：PyCharm
 # 订单API
 from typing import Optional, Union
 from request import Request
 from utils.util import dumps, getDefaultParams, JTable1, generateChangeBatchItems
 
 
-def OrderRequest(data: dict, method: str = 'LoadDataToJSON',
+def AftersaleRequest(data: dict, method: str = 'LoadDataToJSON',
                  url: str = '/app/Service/aftersale/aftersale.aspx', **kwargs) -> Request:
     params = getDefaultParams({'defaultParams': ["ts___"], 'am___': method})
     if kwargs.get('params'):
         params.update(kwargs.get('params'))
     return Request(
         method='POST',
         url=url,
@@ -32,15 +32,15 @@
     获取订单
     :param page_num: 页数
     :param page_size:  每页条数
     :param queryData:  查询条件
     :return: 查询结果
     '''
     if queryData is None: queryData = []
-    return OrderRequest({
+    return AftersaleRequest({
         '_jt_page_size': page_size,
         "__CALLBACKID": "JTable1",
         '__CALLBACKPARAM': dumps(
             {
                 "Method": "LoadDataToJSON",
                 "Args": [
                     page_num,
@@ -58,15 +58,15 @@
 # 确认售后订单
 def aftersaleCommon(afterId: Union[str, int]):
     '''
     确认售后订单
     :param oid:  内部订单号
     :return: 执行结果
     '''
-    return OrderRequest({
+    return AftersaleRequest({
         'isCB': '0',
         '__CALLBACKID': 'ACall1',
         '__CALLBACKPARAM': dumps(
             {
                 "Method": "Confirms",
                 "Args": [str(afterId), "false", "true", "false", "false", "false"],
              "CallControl": "{page}"
@@ -81,12 +81,12 @@
 # 售后单转转成
 def clearException(afterId: Union[str, int]):
     '''
     售后单转转成
     :param oid:  内部订单号
     :return: 执行结果
     '''
-    return OrderRequest({
+    return AftersaleRequest({
         '__CALLBACKID': 'JTable1',
         '__CALLBACKPARAM': dumps({"Method":"ClearException","Args":[afterId],"CallControl":"{page}"}),
     },
         method='ClearException')
```

## erp_apis/apis/test.py

```diff
@@ -4,15 +4,15 @@
 # Author：李福成
 # Date ：2024-04-28 18:24
 # IDE：PyCharm
 from apis.inventory import WmsSkuStock
 from apis.order import OrderList, ChangeBatchItems
 from apis.user import login
 from apis.afterSales import aftersaleList, aftersaleCommon, clearException
-
+from apis.goods import ItemList
 from request import Session
 
 if __name__ == '__main__':
     session = Session()
     session.erpSend(login(
         username="",
         password=""
@@ -34,9 +34,12 @@
     #     "k": "shop_id",
     #     "v": "15429635,14421166,14129300,14409794,13077664,11288284,12151690,12391281,11288291,10341596,15581347,13116222,14242518,14163461,14163558,15517378,15297892,15513593,14420990,14699171,15982786,15748932,14699049,13530518,13445299,14421297,11700009,11725757,14484991,13168313,14418703,13168328",
     #     "c": "@="}, {"k": "status", "v": "waitconfirm", "c": "@="}, {"k": "type", "v": "换货", "c": "@="},
     #     {"k": "shop_type", "v": "换货", "c": "@="}, {"k": "as_date", "v": "30天前", "c": ">=", "t": "date"},
     #     {"k": "as_date", "v": "今天 23:59:59.999", "c": "<=", "t": "date"}])
     # )
     # res = session.erpSend(aftersaleCommon(1452451077))
-    res = session.erpSend(clearException(1452451077))
+    # res = session.erpSend(clearException(1452451077))
+
+
+    res = session.erp321Send(ItemList(queryData=[{"k":"shop_i_id","v":"793265551325","c":"@="}]))
     print(res.json())
```

## Comparing `erp_apis-1.0.2.dist-info/METADATA` & `erp_apis-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erp-apis
-Version: 1.0.2
+Version: 1.0.3
 Summary: erp_apis
 Home-page: https://gitee.com/li_fucheng/erp_sdk_python
 Author: 李福成
 Author-email: lfct@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://gitee.com/li_fucheng/erp_sdk_python/issues
 Project-URL: Documentation, https://gitee.com/li_fucheng/erp_sdk_python
```

