# Comparing `tmp/alibabacloud_linkedmall20230930-2.2.0.tar.gz` & `tmp/alibabacloud_linkedmall20230930-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_linkedmall20230930-2.2.0.tar", last modified: Wed Apr 17 02:54:43 2024, max compression
+gzip compressed data, was "dist/alibabacloud_linkedmall20230930-2.2.1.tar", last modified: Tue May  7 05:58:35 2024, max compression
```

## Comparing `alibabacloud_linkedmall20230930-2.2.0.tar` & `alibabacloud_linkedmall20230930-2.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2450 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1123 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1208 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65926 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930/client.py
--rw-r--r--   0 root         (0) root         (0)   159384 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2450 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2646 2024-04-17 02:54:43.000000 alibabacloud_linkedmall20230930-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/
+-rw-r--r--   0 root         (0) root         (0)      662 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    83946 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930/client.py
+-rw-r--r--   0 root         (0) root         (0)   161626 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-07 05:58:35.000000 alibabacloud_linkedmall20230930-2.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2646 2024-05-07 05:58:34.000000 alibabacloud_linkedmall20230930-2.2.1/setup.py
```

### Comparing `alibabacloud_linkedmall20230930-2.2.0/ChangeLog.md` & `alibabacloud_linkedmall20230930-2.2.1/ChangeLog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-04-17 Version: 2.2.0
+- Support API SplitPurchaseOrder.
+
+
 2024-04-12 Version: 2.1.4
 - Generated python 2023-09-30 for linkedmall.
 
 2024-04-08 Version: 2.1.3
 - Generated python 2023-09-30 for linkedmall.
 
 2024-03-29 Version: 2.1.2
```

### Comparing `alibabacloud_linkedmall20230930-2.2.0/LICENSE` & `alibabacloud_linkedmall20230930-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.2.0/PKG-INFO` & `alibabacloud_linkedmall20230930-2.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_linkedmall20230930
-Version: 2.2.0
+Version: 2.2.1
 Summary: Alibaba Cloud linkedmall (20230930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmall20230930-2.2.0/README-CN.md` & `alibabacloud_linkedmall20230930-2.2.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.2.0/README.md` & `alibabacloud_linkedmall20230930-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930/client.py` & `alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -99,14 +99,21 @@
 
     def cancel_refund_order_with_options(
         self,
         dispute_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.CancelRefundOrderResponse:
+        """
+        @summary 取消逆向单
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CancelRefundOrderResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='CancelRefundOrder',
             version='2023-09-30',
             protocol='HTTPS',
@@ -124,14 +131,21 @@
 
     async def cancel_refund_order_with_options_async(
         self,
         dispute_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.CancelRefundOrderResponse:
+        """
+        @summary 取消逆向单
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CancelRefundOrderResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='CancelRefundOrder',
             version='2023-09-30',
             protocol='HTTPS',
@@ -147,32 +161,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def cancel_refund_order(
         self,
         dispute_id: str,
     ) -> linkedmall_20230930_models.CancelRefundOrderResponse:
+        """
+        @summary 取消逆向单
+        
+        @return: CancelRefundOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.cancel_refund_order_with_options(dispute_id, headers, runtime)
 
     async def cancel_refund_order_async(
         self,
         dispute_id: str,
     ) -> linkedmall_20230930_models.CancelRefundOrderResponse:
+        """
+        @summary 取消逆向单
+        
+        @return: CancelRefundOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.cancel_refund_order_with_options_async(dispute_id, headers, runtime)
 
     def confirm_disburse_with_options(
         self,
         request: linkedmall_20230930_models.ConfirmDisburseRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ConfirmDisburseResponse:
+        """
+        @summary 确认收货（订单）
+        
+        @param request: ConfirmDisburseRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfirmDisburseResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='ConfirmDisburse',
@@ -192,14 +224,22 @@
 
     async def confirm_disburse_with_options_async(
         self,
         request: linkedmall_20230930_models.ConfirmDisburseRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ConfirmDisburseResponse:
+        """
+        @summary 确认收货（订单）
+        
+        @param request: ConfirmDisburseRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfirmDisburseResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='ConfirmDisburse',
@@ -217,32 +257,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def confirm_disburse(
         self,
         request: linkedmall_20230930_models.ConfirmDisburseRequest,
     ) -> linkedmall_20230930_models.ConfirmDisburseResponse:
+        """
+        @summary 确认收货（订单）
+        
+        @param request: ConfirmDisburseRequest
+        @return: ConfirmDisburseResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.confirm_disburse_with_options(request, headers, runtime)
 
     async def confirm_disburse_async(
         self,
         request: linkedmall_20230930_models.ConfirmDisburseRequest,
     ) -> linkedmall_20230930_models.ConfirmDisburseResponse:
+        """
+        @summary 确认收货（订单）
+        
+        @param request: ConfirmDisburseRequest
+        @return: ConfirmDisburseResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.confirm_disburse_with_options_async(request, headers, runtime)
 
     def create_goods_shipping_notice_with_options(
         self,
         request: linkedmall_20230930_models.CreateGoodsShippingNoticeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.CreateGoodsShippingNoticeResponse:
+        """
+        @summary 提交运单信息
+        
+        @param request: CreateGoodsShippingNoticeRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateGoodsShippingNoticeResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateGoodsShippingNotice',
@@ -262,14 +322,22 @@
 
     async def create_goods_shipping_notice_with_options_async(
         self,
         request: linkedmall_20230930_models.CreateGoodsShippingNoticeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.CreateGoodsShippingNoticeResponse:
+        """
+        @summary 提交运单信息
+        
+        @param request: CreateGoodsShippingNoticeRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateGoodsShippingNoticeResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateGoodsShippingNotice',
@@ -287,32 +355,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_goods_shipping_notice(
         self,
         request: linkedmall_20230930_models.CreateGoodsShippingNoticeRequest,
     ) -> linkedmall_20230930_models.CreateGoodsShippingNoticeResponse:
+        """
+        @summary 提交运单信息
+        
+        @param request: CreateGoodsShippingNoticeRequest
+        @return: CreateGoodsShippingNoticeResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_goods_shipping_notice_with_options(request, headers, runtime)
 
     async def create_goods_shipping_notice_async(
         self,
         request: linkedmall_20230930_models.CreateGoodsShippingNoticeRequest,
     ) -> linkedmall_20230930_models.CreateGoodsShippingNoticeResponse:
+        """
+        @summary 提交运单信息
+        
+        @param request: CreateGoodsShippingNoticeRequest
+        @return: CreateGoodsShippingNoticeResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_goods_shipping_notice_with_options_async(request, headers, runtime)
 
     def create_purchase_order_with_options(
         self,
         request: linkedmall_20230930_models.CreatePurchaseOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.CreatePurchaseOrderResponse:
+        """
+        @summary 创建采购单
+        
+        @param request: CreatePurchaseOrderRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreatePurchaseOrderResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreatePurchaseOrder',
@@ -332,14 +420,22 @@
 
     async def create_purchase_order_with_options_async(
         self,
         request: linkedmall_20230930_models.CreatePurchaseOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.CreatePurchaseOrderResponse:
+        """
+        @summary 创建采购单
+        
+        @param request: CreatePurchaseOrderRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreatePurchaseOrderResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreatePurchaseOrder',
@@ -357,32 +453,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_purchase_order(
         self,
         request: linkedmall_20230930_models.CreatePurchaseOrderRequest,
     ) -> linkedmall_20230930_models.CreatePurchaseOrderResponse:
+        """
+        @summary 创建采购单
+        
+        @param request: CreatePurchaseOrderRequest
+        @return: CreatePurchaseOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_purchase_order_with_options(request, headers, runtime)
 
     async def create_purchase_order_async(
         self,
         request: linkedmall_20230930_models.CreatePurchaseOrderRequest,
     ) -> linkedmall_20230930_models.CreatePurchaseOrderResponse:
+        """
+        @summary 创建采购单
+        
+        @param request: CreatePurchaseOrderRequest
+        @return: CreatePurchaseOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_purchase_order_with_options_async(request, headers, runtime)
 
     def create_refund_order_with_options(
         self,
         request: linkedmall_20230930_models.CreateRefundOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.CreateRefundOrderResponse:
+        """
+        @summary 创建逆向单
+        
+        @param request: CreateRefundOrderRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateRefundOrderResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateRefundOrder',
@@ -402,14 +518,22 @@
 
     async def create_refund_order_with_options_async(
         self,
         request: linkedmall_20230930_models.CreateRefundOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.CreateRefundOrderResponse:
+        """
+        @summary 创建逆向单
+        
+        @param request: CreateRefundOrderRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateRefundOrderResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateRefundOrder',
@@ -427,32 +551,51 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_refund_order(
         self,
         request: linkedmall_20230930_models.CreateRefundOrderRequest,
     ) -> linkedmall_20230930_models.CreateRefundOrderResponse:
+        """
+        @summary 创建逆向单
+        
+        @param request: CreateRefundOrderRequest
+        @return: CreateRefundOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_refund_order_with_options(request, headers, runtime)
 
     async def create_refund_order_async(
         self,
         request: linkedmall_20230930_models.CreateRefundOrderRequest,
     ) -> linkedmall_20230930_models.CreateRefundOrderResponse:
+        """
+        @summary 创建逆向单
+        
+        @param request: CreateRefundOrderRequest
+        @return: CreateRefundOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_refund_order_with_options_async(request, headers, runtime)
 
     def get_order_with_options(
         self,
         order_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.GetOrderResponse:
+        """
+        @summary 查询主单详情
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOrderResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetOrder',
             version='2023-09-30',
             protocol='HTTPS',
@@ -470,14 +613,21 @@
 
     async def get_order_with_options_async(
         self,
         order_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.GetOrderResponse:
+        """
+        @summary 查询主单详情
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOrderResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetOrder',
             version='2023-09-30',
             protocol='HTTPS',
@@ -493,32 +643,49 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_order(
         self,
         order_id: str,
     ) -> linkedmall_20230930_models.GetOrderResponse:
+        """
+        @summary 查询主单详情
+        
+        @return: GetOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_order_with_options(order_id, headers, runtime)
 
     async def get_order_async(
         self,
         order_id: str,
     ) -> linkedmall_20230930_models.GetOrderResponse:
+        """
+        @summary 查询主单详情
+        
+        @return: GetOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_order_with_options_async(order_id, headers, runtime)
 
     def get_purchase_order_status_with_options(
         self,
         purchase_order_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.GetPurchaseOrderStatusResponse:
+        """
+        @summary 查询采购单状态
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPurchaseOrderStatusResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetPurchaseOrderStatus',
             version='2023-09-30',
             protocol='HTTPS',
@@ -536,14 +703,21 @@
 
     async def get_purchase_order_status_with_options_async(
         self,
         purchase_order_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.GetPurchaseOrderStatusResponse:
+        """
+        @summary 查询采购单状态
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPurchaseOrderStatusResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetPurchaseOrderStatus',
             version='2023-09-30',
             protocol='HTTPS',
@@ -559,32 +733,49 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_purchase_order_status(
         self,
         purchase_order_id: str,
     ) -> linkedmall_20230930_models.GetPurchaseOrderStatusResponse:
+        """
+        @summary 查询采购单状态
+        
+        @return: GetPurchaseOrderStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_purchase_order_status_with_options(purchase_order_id, headers, runtime)
 
     async def get_purchase_order_status_async(
         self,
         purchase_order_id: str,
     ) -> linkedmall_20230930_models.GetPurchaseOrderStatusResponse:
+        """
+        @summary 查询采购单状态
+        
+        @return: GetPurchaseOrderStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_purchase_order_status_with_options_async(purchase_order_id, headers, runtime)
 
     def get_purchaser_shop_with_options(
         self,
         purchaser_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.GetPurchaserShopResponse:
+        """
+        @summary 查询分销商店铺
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPurchaserShopResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetPurchaserShop',
             version='2023-09-30',
             protocol='HTTPS',
@@ -602,14 +793,21 @@
 
     async def get_purchaser_shop_with_options_async(
         self,
         purchaser_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.GetPurchaserShopResponse:
+        """
+        @summary 查询分销商店铺
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPurchaserShopResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetPurchaserShop',
             version='2023-09-30',
             protocol='HTTPS',
@@ -625,32 +823,49 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_purchaser_shop(
         self,
         purchaser_id: str,
     ) -> linkedmall_20230930_models.GetPurchaserShopResponse:
+        """
+        @summary 查询分销商店铺
+        
+        @return: GetPurchaserShopResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_purchaser_shop_with_options(purchaser_id, headers, runtime)
 
     async def get_purchaser_shop_async(
         self,
         purchaser_id: str,
     ) -> linkedmall_20230930_models.GetPurchaserShopResponse:
+        """
+        @summary 查询分销商店铺
+        
+        @return: GetPurchaserShopResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_purchaser_shop_with_options_async(purchaser_id, headers, runtime)
 
     def get_refund_order_with_options(
         self,
         dispute_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.GetRefundOrderResponse:
+        """
+        @summary 查询逆向单详情
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetRefundOrderResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetRefundOrder',
             version='2023-09-30',
             protocol='HTTPS',
@@ -668,14 +883,21 @@
 
     async def get_refund_order_with_options_async(
         self,
         dispute_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.GetRefundOrderResponse:
+        """
+        @summary 查询逆向单详情
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetRefundOrderResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetRefundOrder',
             version='2023-09-30',
             protocol='HTTPS',
@@ -691,33 +913,51 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_refund_order(
         self,
         dispute_id: str,
     ) -> linkedmall_20230930_models.GetRefundOrderResponse:
+        """
+        @summary 查询逆向单详情
+        
+        @return: GetRefundOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_refund_order_with_options(dispute_id, headers, runtime)
 
     async def get_refund_order_async(
         self,
         dispute_id: str,
     ) -> linkedmall_20230930_models.GetRefundOrderResponse:
+        """
+        @summary 查询逆向单详情
+        
+        @return: GetRefundOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_refund_order_with_options_async(dispute_id, headers, runtime)
 
     def get_selection_product_with_options(
         self,
         product_id: str,
         request: linkedmall_20230930_models.GetSelectionProductRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.GetSelectionProductResponse:
+        """
+        @summary 查询选品池商品详情
+        
+        @param request: GetSelectionProductRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSelectionProductResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.division_code):
             query['divisionCode'] = request.division_code
         if not UtilClient.is_unset(request.purchaser_id):
             query['purchaserId'] = request.purchaser_id
         req = open_api_models.OpenApiRequest(
@@ -743,14 +983,22 @@
     async def get_selection_product_with_options_async(
         self,
         product_id: str,
         request: linkedmall_20230930_models.GetSelectionProductRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.GetSelectionProductResponse:
+        """
+        @summary 查询选品池商品详情
+        
+        @param request: GetSelectionProductRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSelectionProductResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.division_code):
             query['divisionCode'] = request.division_code
         if not UtilClient.is_unset(request.purchaser_id):
             query['purchaserId'] = request.purchaser_id
         req = open_api_models.OpenApiRequest(
@@ -774,34 +1022,54 @@
         )
 
     def get_selection_product(
         self,
         product_id: str,
         request: linkedmall_20230930_models.GetSelectionProductRequest,
     ) -> linkedmall_20230930_models.GetSelectionProductResponse:
+        """
+        @summary 查询选品池商品详情
+        
+        @param request: GetSelectionProductRequest
+        @return: GetSelectionProductResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_selection_product_with_options(product_id, request, headers, runtime)
 
     async def get_selection_product_async(
         self,
         product_id: str,
         request: linkedmall_20230930_models.GetSelectionProductRequest,
     ) -> linkedmall_20230930_models.GetSelectionProductResponse:
+        """
+        @summary 查询选品池商品详情
+        
+        @param request: GetSelectionProductRequest
+        @return: GetSelectionProductResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_selection_product_with_options_async(product_id, request, headers, runtime)
 
     def get_selection_product_sale_info_with_options(
         self,
         product_id: str,
         request: linkedmall_20230930_models.GetSelectionProductSaleInfoRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.GetSelectionProductSaleInfoResponse:
+        """
+        @summary 查询选品池商品库存
+        
+        @param request: GetSelectionProductSaleInfoRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSelectionProductSaleInfoResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.division_code):
             query['divisionCode'] = request.division_code
         if not UtilClient.is_unset(request.purchaser_id):
             query['purchaserId'] = request.purchaser_id
         req = open_api_models.OpenApiRequest(
@@ -827,14 +1095,22 @@
     async def get_selection_product_sale_info_with_options_async(
         self,
         product_id: str,
         request: linkedmall_20230930_models.GetSelectionProductSaleInfoRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.GetSelectionProductSaleInfoResponse:
+        """
+        @summary 查询选品池商品库存
+        
+        @param request: GetSelectionProductSaleInfoRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSelectionProductSaleInfoResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.division_code):
             query['divisionCode'] = request.division_code
         if not UtilClient.is_unset(request.purchaser_id):
             query['purchaserId'] = request.purchaser_id
         req = open_api_models.OpenApiRequest(
@@ -858,33 +1134,53 @@
         )
 
     def get_selection_product_sale_info(
         self,
         product_id: str,
         request: linkedmall_20230930_models.GetSelectionProductSaleInfoRequest,
     ) -> linkedmall_20230930_models.GetSelectionProductSaleInfoResponse:
+        """
+        @summary 查询选品池商品库存
+        
+        @param request: GetSelectionProductSaleInfoRequest
+        @return: GetSelectionProductSaleInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_selection_product_sale_info_with_options(product_id, request, headers, runtime)
 
     async def get_selection_product_sale_info_async(
         self,
         product_id: str,
         request: linkedmall_20230930_models.GetSelectionProductSaleInfoRequest,
     ) -> linkedmall_20230930_models.GetSelectionProductSaleInfoResponse:
+        """
+        @summary 查询选品池商品库存
+        
+        @param request: GetSelectionProductSaleInfoRequest
+        @return: GetSelectionProductSaleInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_selection_product_sale_info_with_options_async(product_id, request, headers, runtime)
 
     def list_categories_with_options(
         self,
         request: linkedmall_20230930_models.ListCategoriesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ListCategoriesResponse:
+        """
+        @summary 查询类目
+        
+        @param request: ListCategoriesRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListCategoriesResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='ListCategories',
@@ -904,14 +1200,22 @@
 
     async def list_categories_with_options_async(
         self,
         request: linkedmall_20230930_models.ListCategoriesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ListCategoriesResponse:
+        """
+        @summary 查询类目
+        
+        @param request: ListCategoriesRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListCategoriesResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='ListCategories',
@@ -929,32 +1233,51 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_categories(
         self,
         request: linkedmall_20230930_models.ListCategoriesRequest,
     ) -> linkedmall_20230930_models.ListCategoriesResponse:
+        """
+        @summary 查询类目
+        
+        @param request: ListCategoriesRequest
+        @return: ListCategoriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_categories_with_options(request, headers, runtime)
 
     async def list_categories_async(
         self,
         request: linkedmall_20230930_models.ListCategoriesRequest,
     ) -> linkedmall_20230930_models.ListCategoriesResponse:
+        """
+        @summary 查询类目
+        
+        @param request: ListCategoriesRequest
+        @return: ListCategoriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_categories_with_options_async(request, headers, runtime)
 
     def list_logistics_orders_with_options(
         self,
         order_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ListLogisticsOrdersResponse:
+        """
+        @summary 查询物流信息（订单）
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListLogisticsOrdersResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListLogisticsOrders',
             version='2023-09-30',
             protocol='HTTPS',
@@ -972,14 +1295,21 @@
 
     async def list_logistics_orders_with_options_async(
         self,
         order_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ListLogisticsOrdersResponse:
+        """
+        @summary 查询物流信息（订单）
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListLogisticsOrdersResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListLogisticsOrders',
             version='2023-09-30',
             protocol='HTTPS',
@@ -995,32 +1325,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_logistics_orders(
         self,
         order_id: str,
     ) -> linkedmall_20230930_models.ListLogisticsOrdersResponse:
+        """
+        @summary 查询物流信息（订单）
+        
+        @return: ListLogisticsOrdersResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_logistics_orders_with_options(order_id, headers, runtime)
 
     async def list_logistics_orders_async(
         self,
         order_id: str,
     ) -> linkedmall_20230930_models.ListLogisticsOrdersResponse:
+        """
+        @summary 查询物流信息（订单）
+        
+        @return: ListLogisticsOrdersResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_logistics_orders_with_options_async(order_id, headers, runtime)
 
     def list_purchaser_shops_with_options(
         self,
         request: linkedmall_20230930_models.ListPurchaserShopsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ListPurchaserShopsResponse:
+        """
+        @summary 采购方店铺列表查询
+        
+        @param request: ListPurchaserShopsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPurchaserShopsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['pageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
@@ -1045,14 +1393,22 @@
 
     async def list_purchaser_shops_with_options_async(
         self,
         request: linkedmall_20230930_models.ListPurchaserShopsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ListPurchaserShopsResponse:
+        """
+        @summary 采购方店铺列表查询
+        
+        @param request: ListPurchaserShopsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPurchaserShopsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['pageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
@@ -1075,32 +1431,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_purchaser_shops(
         self,
         request: linkedmall_20230930_models.ListPurchaserShopsRequest,
     ) -> linkedmall_20230930_models.ListPurchaserShopsResponse:
+        """
+        @summary 采购方店铺列表查询
+        
+        @param request: ListPurchaserShopsRequest
+        @return: ListPurchaserShopsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_purchaser_shops_with_options(request, headers, runtime)
 
     async def list_purchaser_shops_async(
         self,
         request: linkedmall_20230930_models.ListPurchaserShopsRequest,
     ) -> linkedmall_20230930_models.ListPurchaserShopsResponse:
+        """
+        @summary 采购方店铺列表查询
+        
+        @param request: ListPurchaserShopsRequest
+        @return: ListPurchaserShopsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_purchaser_shops_with_options_async(request, headers, runtime)
 
     def list_selection_product_sale_infos_with_options(
         self,
         request: linkedmall_20230930_models.ListSelectionProductSaleInfosRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ListSelectionProductSaleInfosResponse:
+        """
+        @summary 批量查询选品池商品库存
+        
+        @param request: ListSelectionProductSaleInfosRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSelectionProductSaleInfosResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='ListSelectionProductSaleInfos',
@@ -1120,14 +1496,22 @@
 
     async def list_selection_product_sale_infos_with_options_async(
         self,
         request: linkedmall_20230930_models.ListSelectionProductSaleInfosRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ListSelectionProductSaleInfosResponse:
+        """
+        @summary 批量查询选品池商品库存
+        
+        @param request: ListSelectionProductSaleInfosRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSelectionProductSaleInfosResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='ListSelectionProductSaleInfos',
@@ -1145,32 +1529,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_selection_product_sale_infos(
         self,
         request: linkedmall_20230930_models.ListSelectionProductSaleInfosRequest,
     ) -> linkedmall_20230930_models.ListSelectionProductSaleInfosResponse:
+        """
+        @summary 批量查询选品池商品库存
+        
+        @param request: ListSelectionProductSaleInfosRequest
+        @return: ListSelectionProductSaleInfosResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_selection_product_sale_infos_with_options(request, headers, runtime)
 
     async def list_selection_product_sale_infos_async(
         self,
         request: linkedmall_20230930_models.ListSelectionProductSaleInfosRequest,
     ) -> linkedmall_20230930_models.ListSelectionProductSaleInfosResponse:
+        """
+        @summary 批量查询选品池商品库存
+        
+        @param request: ListSelectionProductSaleInfosRequest
+        @return: ListSelectionProductSaleInfosResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_selection_product_sale_infos_with_options_async(request, headers, runtime)
 
     def list_selection_products_with_options(
         self,
         request: linkedmall_20230930_models.ListSelectionProductsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ListSelectionProductsResponse:
+        """
+        @summary 查询商品列表
+        
+        @param request: ListSelectionProductsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSelectionProductsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['pageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
         if not UtilClient.is_unset(request.purchaser_id):
@@ -1197,14 +1601,22 @@
 
     async def list_selection_products_with_options_async(
         self,
         request: linkedmall_20230930_models.ListSelectionProductsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ListSelectionProductsResponse:
+        """
+        @summary 查询商品列表
+        
+        @param request: ListSelectionProductsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSelectionProductsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['pageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['pageSize'] = request.page_size
         if not UtilClient.is_unset(request.purchaser_id):
@@ -1229,32 +1641,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_selection_products(
         self,
         request: linkedmall_20230930_models.ListSelectionProductsRequest,
     ) -> linkedmall_20230930_models.ListSelectionProductsResponse:
+        """
+        @summary 查询商品列表
+        
+        @param request: ListSelectionProductsRequest
+        @return: ListSelectionProductsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_selection_products_with_options(request, headers, runtime)
 
     async def list_selection_products_async(
         self,
         request: linkedmall_20230930_models.ListSelectionProductsRequest,
     ) -> linkedmall_20230930_models.ListSelectionProductsResponse:
+        """
+        @summary 查询商品列表
+        
+        @param request: ListSelectionProductsRequest
+        @return: ListSelectionProductsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_selection_products_with_options_async(request, headers, runtime)
 
     def list_selection_sku_sale_infos_with_options(
         self,
         request: linkedmall_20230930_models.ListSelectionSkuSaleInfosRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ListSelectionSkuSaleInfosResponse:
+        """
+        @summary 批量查询选品池商品SKU库存
+        
+        @param request: ListSelectionSkuSaleInfosRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSelectionSkuSaleInfosResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='ListSelectionSkuSaleInfos',
@@ -1274,14 +1706,22 @@
 
     async def list_selection_sku_sale_infos_with_options_async(
         self,
         request: linkedmall_20230930_models.ListSelectionSkuSaleInfosRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.ListSelectionSkuSaleInfosResponse:
+        """
+        @summary 批量查询选品池商品SKU库存
+        
+        @param request: ListSelectionSkuSaleInfosRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSelectionSkuSaleInfosResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='ListSelectionSkuSaleInfos',
@@ -1299,32 +1739,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_selection_sku_sale_infos(
         self,
         request: linkedmall_20230930_models.ListSelectionSkuSaleInfosRequest,
     ) -> linkedmall_20230930_models.ListSelectionSkuSaleInfosResponse:
+        """
+        @summary 批量查询选品池商品SKU库存
+        
+        @param request: ListSelectionSkuSaleInfosRequest
+        @return: ListSelectionSkuSaleInfosResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_selection_sku_sale_infos_with_options(request, headers, runtime)
 
     async def list_selection_sku_sale_infos_async(
         self,
         request: linkedmall_20230930_models.ListSelectionSkuSaleInfosRequest,
     ) -> linkedmall_20230930_models.ListSelectionSkuSaleInfosResponse:
+        """
+        @summary 批量查询选品池商品SKU库存
+        
+        @param request: ListSelectionSkuSaleInfosRequest
+        @return: ListSelectionSkuSaleInfosResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_selection_sku_sale_infos_with_options_async(request, headers, runtime)
 
     def query_child_division_code_with_options(
         self,
         request: linkedmall_20230930_models.QueryChildDivisionCodeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.QueryChildDivisionCodeResponse:
+        """
+        @summary 查询地址divisionCode
+        
+        @param request: QueryChildDivisionCodeRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryChildDivisionCodeResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='QueryChildDivisionCode',
@@ -1344,14 +1804,22 @@
 
     async def query_child_division_code_with_options_async(
         self,
         request: linkedmall_20230930_models.QueryChildDivisionCodeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.QueryChildDivisionCodeResponse:
+        """
+        @summary 查询地址divisionCode
+        
+        @param request: QueryChildDivisionCodeRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryChildDivisionCodeResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='QueryChildDivisionCode',
@@ -1369,32 +1837,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_child_division_code(
         self,
         request: linkedmall_20230930_models.QueryChildDivisionCodeRequest,
     ) -> linkedmall_20230930_models.QueryChildDivisionCodeResponse:
+        """
+        @summary 查询地址divisionCode
+        
+        @param request: QueryChildDivisionCodeRequest
+        @return: QueryChildDivisionCodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.query_child_division_code_with_options(request, headers, runtime)
 
     async def query_child_division_code_async(
         self,
         request: linkedmall_20230930_models.QueryChildDivisionCodeRequest,
     ) -> linkedmall_20230930_models.QueryChildDivisionCodeResponse:
+        """
+        @summary 查询地址divisionCode
+        
+        @param request: QueryChildDivisionCodeRequest
+        @return: QueryChildDivisionCodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.query_child_division_code_with_options_async(request, headers, runtime)
 
     def query_orders_with_options(
         self,
         request: linkedmall_20230930_models.QueryOrdersRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.QueryOrdersResponse:
+        """
+        @summary 查询主单列表
+        
+        @param request: QueryOrdersRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryOrdersResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='QueryOrders',
@@ -1414,14 +1902,22 @@
 
     async def query_orders_with_options_async(
         self,
         request: linkedmall_20230930_models.QueryOrdersRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.QueryOrdersResponse:
+        """
+        @summary 查询主单列表
+        
+        @param request: QueryOrdersRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryOrdersResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='QueryOrders',
@@ -1439,32 +1935,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_orders(
         self,
         request: linkedmall_20230930_models.QueryOrdersRequest,
     ) -> linkedmall_20230930_models.QueryOrdersResponse:
+        """
+        @summary 查询主单列表
+        
+        @param request: QueryOrdersRequest
+        @return: QueryOrdersResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.query_orders_with_options(request, headers, runtime)
 
     async def query_orders_async(
         self,
         request: linkedmall_20230930_models.QueryOrdersRequest,
     ) -> linkedmall_20230930_models.QueryOrdersResponse:
+        """
+        @summary 查询主单列表
+        
+        @param request: QueryOrdersRequest
+        @return: QueryOrdersResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.query_orders_with_options_async(request, headers, runtime)
 
     def render_purchase_order_with_options(
         self,
         request: linkedmall_20230930_models.RenderPurchaseOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.RenderPurchaseOrderResponse:
+        """
+        @summary 渲染采购单
+        
+        @param request: RenderPurchaseOrderRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RenderPurchaseOrderResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='RenderPurchaseOrder',
@@ -1484,14 +2000,22 @@
 
     async def render_purchase_order_with_options_async(
         self,
         request: linkedmall_20230930_models.RenderPurchaseOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.RenderPurchaseOrderResponse:
+        """
+        @summary 渲染采购单
+        
+        @param request: RenderPurchaseOrderRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RenderPurchaseOrderResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='RenderPurchaseOrder',
@@ -1509,32 +2033,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def render_purchase_order(
         self,
         request: linkedmall_20230930_models.RenderPurchaseOrderRequest,
     ) -> linkedmall_20230930_models.RenderPurchaseOrderResponse:
+        """
+        @summary 渲染采购单
+        
+        @param request: RenderPurchaseOrderRequest
+        @return: RenderPurchaseOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.render_purchase_order_with_options(request, headers, runtime)
 
     async def render_purchase_order_async(
         self,
         request: linkedmall_20230930_models.RenderPurchaseOrderRequest,
     ) -> linkedmall_20230930_models.RenderPurchaseOrderResponse:
+        """
+        @summary 渲染采购单
+        
+        @param request: RenderPurchaseOrderRequest
+        @return: RenderPurchaseOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.render_purchase_order_with_options_async(request, headers, runtime)
 
     def render_refund_order_with_options(
         self,
         request: linkedmall_20230930_models.RenderRefundOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.RenderRefundOrderResponse:
+        """
+        @summary 逆向单渲染
+        
+        @param request: RenderRefundOrderRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RenderRefundOrderResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='RenderRefundOrder',
@@ -1554,14 +2098,22 @@
 
     async def render_refund_order_with_options_async(
         self,
         request: linkedmall_20230930_models.RenderRefundOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.RenderRefundOrderResponse:
+        """
+        @summary 逆向单渲染
+        
+        @param request: RenderRefundOrderRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RenderRefundOrderResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='RenderRefundOrder',
@@ -1579,32 +2131,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def render_refund_order(
         self,
         request: linkedmall_20230930_models.RenderRefundOrderRequest,
     ) -> linkedmall_20230930_models.RenderRefundOrderResponse:
+        """
+        @summary 逆向单渲染
+        
+        @param request: RenderRefundOrderRequest
+        @return: RenderRefundOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.render_refund_order_with_options(request, headers, runtime)
 
     async def render_refund_order_async(
         self,
         request: linkedmall_20230930_models.RenderRefundOrderRequest,
     ) -> linkedmall_20230930_models.RenderRefundOrderResponse:
+        """
+        @summary 逆向单渲染
+        
+        @param request: RenderRefundOrderRequest
+        @return: RenderRefundOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.render_refund_order_with_options_async(request, headers, runtime)
 
     def split_purchase_order_with_options(
         self,
         request: linkedmall_20230930_models.SplitPurchaseOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.SplitPurchaseOrderResponse:
+        """
+        @summary 渲染拆分采购单
+        
+        @param request: SplitPurchaseOrderRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SplitPurchaseOrderResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='SplitPurchaseOrder',
@@ -1624,14 +2196,22 @@
 
     async def split_purchase_order_with_options_async(
         self,
         request: linkedmall_20230930_models.SplitPurchaseOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> linkedmall_20230930_models.SplitPurchaseOrderResponse:
+        """
+        @summary 渲染拆分采购单
+        
+        @param request: SplitPurchaseOrderRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SplitPurchaseOrderResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='SplitPurchaseOrder',
@@ -1649,18 +2229,30 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def split_purchase_order(
         self,
         request: linkedmall_20230930_models.SplitPurchaseOrderRequest,
     ) -> linkedmall_20230930_models.SplitPurchaseOrderResponse:
+        """
+        @summary 渲染拆分采购单
+        
+        @param request: SplitPurchaseOrderRequest
+        @return: SplitPurchaseOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.split_purchase_order_with_options(request, headers, runtime)
 
     async def split_purchase_order_async(
         self,
         request: linkedmall_20230930_models.SplitPurchaseOrderRequest,
     ) -> linkedmall_20230930_models.SplitPurchaseOrderResponse:
+        """
+        @summary 渲染拆分采购单
+        
+        @param request: SplitPurchaseOrderRequest
+        @return: SplitPurchaseOrderResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.split_purchase_order_with_options_async(request, headers, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930/models.py` & `alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,21 @@
         address_detail: str = None,
         address_id: int = None,
         division_code: str = None,
         receiver: str = None,
         receiver_phone: str = None,
         town_division_code: str = None,
     ):
+        # This parameter is required.
         self.address_detail = address_detail
         self.address_id = address_id
         self.division_code = division_code
+        # This parameter is required.
         self.receiver = receiver
+        # This parameter is required.
         self.receiver_phone = receiver_phone
         self.town_division_code = town_division_code
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -495,14 +498,15 @@
 
 
 class DivisionQuery(TeaModel):
     def __init__(
         self,
         division_code: str = None,
     ):
+        # This parameter is required.
         self.division_code = division_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -902,16 +906,19 @@
 class GoodsShippingNoticeCreateCmd(TeaModel):
     def __init__(
         self,
         cp_code: str = None,
         dispute_id: str = None,
         logistics_no: str = None,
     ):
+        # This parameter is required.
         self.cp_code = cp_code
+        # This parameter is required.
         self.dispute_id = dispute_id
+        # This parameter is required.
         self.logistics_no = logistics_no
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1374,15 +1381,17 @@
         self,
         order_id_list: List[str] = None,
         page_number: int = None,
         page_size: int = None,
         purchase_order_id: str = None,
     ):
         self.order_id_list = order_id_list
+        # This parameter is required.
         self.page_number = page_number
+        # This parameter is required.
         self.page_size = page_size
         self.purchase_order_id = purchase_order_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1505,17 +1514,21 @@
     def __init__(
         self,
         product_id: str = None,
         purchaser_id: str = None,
         quantity: int = None,
         sku_id: str = None,
     ):
+        # This parameter is required.
         self.product_id = product_id
+        # This parameter is required.
         self.purchaser_id = purchaser_id
+        # This parameter is required.
         self.quantity = quantity
+        # This parameter is required.
         self.sku_id = sku_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2097,17 +2110,21 @@
         price: int = None,
         product_id: str = None,
         purchaser_id: str = None,
         quantity: int = None,
         sku_id: str = None,
     ):
         self.price = price
+        # This parameter is required.
         self.product_id = product_id
+        # This parameter is required.
         self.purchaser_id = purchaser_id
+        # This parameter is required.
         self.quantity = quantity
+        # This parameter is required.
         self.sku_id = sku_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2147,18 +2164,21 @@
         self,
         page_number: int = None,
         page_size: int = None,
         products: List[Product] = None,
         request_id: str = None,
         total: int = None,
     ):
+        # This parameter is required.
         self.page_number = page_number
+        # This parameter is required.
         self.page_size = page_size
         self.products = products
         self.request_id = request_id
+        # This parameter is required.
         self.total = total
 
     def validate(self):
         if self.products:
             for k in self.products:
                 if k:
                     k.validate()
@@ -2230,14 +2250,15 @@
 
 class ProductQuery(TeaModel):
     def __init__(
         self,
         distributor_shop_id: str = None,
         division_code: str = None,
     ):
+        # This parameter is required.
         self.distributor_shop_id = distributor_shop_id
         self.division_code = division_code
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2441,15 +2462,17 @@
     def __init__(
         self,
         division_code: str = None,
         product_ids: List[str] = None,
         purchaser_id: str = None,
     ):
         self.division_code = division_code
+        # This parameter is required.
         self.product_ids = product_ids
+        # This parameter is required.
         self.purchaser_id = purchaser_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2519,14 +2542,15 @@
 
 class ProductSaleInfoQuery(TeaModel):
     def __init__(
         self,
         distributor_shop_id: str = None,
         division_code: str = None,
     ):
+        # This parameter is required.
         self.distributor_shop_id = distributor_shop_id
         self.division_code = division_code
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2555,18 +2579,22 @@
         self,
         buyer_id: str = None,
         delivery_address: AddressInfo = None,
         ext_info: Dict[str, Any] = None,
         outer_purchase_order_id: str = None,
         product_list: List[ProductDTO] = None,
     ):
+        # This parameter is required.
         self.buyer_id = buyer_id
+        # This parameter is required.
         self.delivery_address = delivery_address
         self.ext_info = ext_info
+        # This parameter is required.
         self.outer_purchase_order_id = outer_purchase_order_id
+        # This parameter is required.
         self.product_list = product_list
 
     def validate(self):
         if self.delivery_address:
             self.delivery_address.validate()
         if self.product_list:
             for k in self.product_list:
@@ -2649,17 +2677,20 @@
     def __init__(
         self,
         buyer_id: str = None,
         delivery_address: AddressInfo = None,
         ext_info: Dict[str, Any] = None,
         product_list: List[OrderRenderProductDTO] = None,
     ):
+        # This parameter is required.
         self.buyer_id = buyer_id
+        # This parameter is required.
         self.delivery_address = delivery_address
         self.ext_info = ext_info
+        # This parameter is required.
         self.product_list = product_list
 
     def validate(self):
         if self.delivery_address:
             self.delivery_address.validate()
         if self.product_list:
             for k in self.product_list:
@@ -2865,22 +2896,28 @@
         apply_refund_fee: int = None,
         biz_claim_type: int = None,
         goods_status: int = None,
         leave_message: str = None,
         leave_picture_lists: List[LeavePictureList] = None,
         order_line_id: str = None,
     ):
+        # This parameter is required.
         self.apply_reason_text_id = apply_reason_text_id
         self.apply_reason_tips = apply_reason_tips
+        # This parameter is required.
         self.apply_refund_count = apply_refund_count
+        # This parameter is required.
         self.apply_refund_fee = apply_refund_fee
+        # This parameter is required.
         self.biz_claim_type = biz_claim_type
+        # This parameter is required.
         self.goods_status = goods_status
         self.leave_message = leave_message
         self.leave_picture_lists = leave_picture_lists
+        # This parameter is required.
         self.order_line_id = order_line_id
 
     def validate(self):
         if self.leave_picture_lists:
             for k in self.leave_picture_lists:
                 if k:
                     k.validate()
@@ -3032,16 +3069,19 @@
 class RefundRenderCmd(TeaModel):
     def __init__(
         self,
         biz_claim_type: int = None,
         goods_status: int = None,
         order_line_id: str = None,
     ):
+        # This parameter is required.
         self.biz_claim_type = biz_claim_type
+        # This parameter is required.
         self.goods_status = goods_status
+        # This parameter is required.
         self.order_line_id = order_line_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3503,15 +3543,17 @@
 
 class SkuQueryParam(TeaModel):
     def __init__(
         self,
         product_id: str = None,
         sku_id: str = None,
     ):
+        # This parameter is required.
         self.product_id = product_id
+        # This parameter is required.
         self.sku_id = sku_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3538,15 +3580,17 @@
     def __init__(
         self,
         division_code: str = None,
         purchaser_id: str = None,
         sku_query_params: List[SkuQueryParam] = None,
     ):
         self.division_code = division_code
+        # This parameter is required.
         self.purchaser_id = purchaser_id
+        # This parameter is required.
         self.sku_query_params = sku_query_params
 
     def validate(self):
         if self.sku_query_params:
             for k in self.sku_query_params:
                 if k:
                     k.validate()
@@ -3664,14 +3708,15 @@
 
 
 class ConfirmDisburseRequest(TeaModel):
     def __init__(
         self,
         body: ConfirmDisburseCmd = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -3734,14 +3779,15 @@
 
 
 class CreateGoodsShippingNoticeRequest(TeaModel):
     def __init__(
         self,
         body: GoodsShippingNoticeCreateCmd = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -3804,14 +3850,15 @@
 
 
 class CreatePurchaseOrderRequest(TeaModel):
     def __init__(
         self,
         body: PurchaseOrderCreateCmd = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -3874,14 +3921,15 @@
 
 
 class CreateRefundOrderRequest(TeaModel):
     def __init__(
         self,
         body: RefundOrderCmd = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -4110,14 +4158,15 @@
 class GetSelectionProductRequest(TeaModel):
     def __init__(
         self,
         division_code: str = None,
         purchaser_id: str = None,
     ):
         self.division_code = division_code
+        # This parameter is required.
         self.purchaser_id = purchaser_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4184,14 +4233,15 @@
 class GetSelectionProductSaleInfoRequest(TeaModel):
     def __init__(
         self,
         division_code: str = None,
         purchaser_id: str = None,
     ):
         self.division_code = division_code
+        # This parameter is required.
         self.purchaser_id = purchaser_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4441,14 +4491,15 @@
 
 
 class ListSelectionProductSaleInfosRequest(TeaModel):
     def __init__(
         self,
         body: ProductSaleInfoListQuery = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -4513,16 +4564,19 @@
 class ListSelectionProductsRequest(TeaModel):
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         purchaser_id: str = None,
     ):
+        # This parameter is required.
         self.page_number = page_number
+        # This parameter is required.
         self.page_size = page_size
+        # This parameter is required.
         self.purchaser_id = purchaser_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4591,14 +4645,15 @@
 
 
 class ListSelectionSkuSaleInfosRequest(TeaModel):
     def __init__(
         self,
         body: SkuSaleInfoListQuery = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -4661,14 +4716,15 @@
 
 
 class QueryChildDivisionCodeRequest(TeaModel):
     def __init__(
         self,
         body: DivisionQuery = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -4731,14 +4787,15 @@
 
 
 class QueryOrdersRequest(TeaModel):
     def __init__(
         self,
         body: OrderPageQuery = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -4801,14 +4858,15 @@
 
 
 class RenderPurchaseOrderRequest(TeaModel):
     def __init__(
         self,
         body: PurchaseOrderRenderQuery = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -4871,14 +4929,15 @@
 
 
 class RenderRefundOrderRequest(TeaModel):
     def __init__(
         self,
         body: RefundRenderCmd = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
```

### Comparing `alibabacloud_linkedmall20230930-2.2.0/alibabacloud_linkedmall20230930.egg-info/PKG-INFO` & `alibabacloud_linkedmall20230930-2.2.1/alibabacloud_linkedmall20230930.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-linkedmall20230930
-Version: 2.2.0
+Version: 2.2.1
 Summary: Alibaba Cloud linkedmall (20230930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmall20230930-2.2.0/setup.py` & `alibabacloud_linkedmall20230930-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_linkedmall20230930.
 
-Created on 17/04/2024
+Created on 07/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_linkedmall20230930"
 NAME = "alibabacloud_linkedmall20230930" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud linkedmall (20230930) SDK Library for Python"
```

