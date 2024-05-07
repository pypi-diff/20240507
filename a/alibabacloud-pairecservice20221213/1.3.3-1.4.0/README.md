# Comparing `tmp/alibabacloud_pairecservice20221213-1.3.3.tar.gz` & `tmp/alibabacloud_pairecservice20221213-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pairecservice20221213-1.3.3.tar", last modified: Sun Apr 28 01:34:03 2024, max compression
+gzip compressed data, was "dist/alibabacloud_pairecservice20221213-1.4.0.tar", last modified: Tue May  7 01:47:42 2024, max compression
```

## Comparing `alibabacloud_pairecservice20221213-1.3.3.tar` & `alibabacloud_pairecservice20221213-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/
--rw-r--r--   0 root         (0) root         (0)     7354 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2471 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1135 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1220 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213/__init__.py
--rw-r--r--   0 root         (0) root         (0)   348615 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213/client.py
--rw-r--r--   0 root         (0) root         (0)   464329 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2471 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2661 2024-04-28 01:34:03.000000 alibabacloud_pairecservice20221213-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 01:47:42.000000 alibabacloud_pairecservice20221213-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)     7430 2024-05-07 01:47:41.000000 alibabacloud_pairecservice20221213-1.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-07 01:47:41.000000 alibabacloud_pairecservice20221213-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-07 01:47:41.000000 alibabacloud_pairecservice20221213-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2471 2024-05-07 01:47:42.000000 alibabacloud_pairecservice20221213-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-05-07 01:47:41.000000 alibabacloud_pairecservice20221213-1.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1220 2024-05-07 01:47:41.000000 alibabacloud_pairecservice20221213-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 01:47:42.000000 alibabacloud_pairecservice20221213-1.4.0/alibabacloud_pairecservice20221213/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-07 01:47:41.000000 alibabacloud_pairecservice20221213-1.4.0/alibabacloud_pairecservice20221213/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   389595 2024-05-07 01:47:41.000000 alibabacloud_pairecservice20221213-1.4.0/alibabacloud_pairecservice20221213/client.py
+-rw-r--r--   0 root         (0) root         (0)   517136 2024-05-07 01:47:41.000000 alibabacloud_pairecservice20221213-1.4.0/alibabacloud_pairecservice20221213/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 01:47:42.000000 alibabacloud_pairecservice20221213-1.4.0/alibabacloud_pairecservice20221213.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2471 2024-05-07 01:47:42.000000 alibabacloud_pairecservice20221213-1.4.0/alibabacloud_pairecservice20221213.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2024-05-07 01:47:42.000000 alibabacloud_pairecservice20221213-1.4.0/alibabacloud_pairecservice20221213.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 01:47:42.000000 alibabacloud_pairecservice20221213-1.4.0/alibabacloud_pairecservice20221213.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-07 01:47:42.000000 alibabacloud_pairecservice20221213-1.4.0/alibabacloud_pairecservice20221213.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-05-07 01:47:42.000000 alibabacloud_pairecservice20221213-1.4.0/alibabacloud_pairecservice20221213.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-07 01:47:42.000000 alibabacloud_pairecservice20221213-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2661 2024-05-07 01:47:41.000000 alibabacloud_pairecservice20221213-1.4.0/setup.py
```

### Comparing `alibabacloud_pairecservice20221213-1.3.3/ChangeLog.md` & `alibabacloud_pairecservice20221213-1.4.0/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-04-28 Version: 1.3.3
+- Generated python 2022-12-13 for PaiRecService.
+
 2024-03-22 Version: 1.3.2
 - Generated python 2022-12-13 for PaiRecService.
 
 2024-03-20 Version: 1.3.1
 - Update API CreateExperimentGroup: add param RegionId.
 - Update API CreateExperimentGroup: update param body.
 - Update API GetExperimentGroup: add param RegionId.
```

### Comparing `alibabacloud_pairecservice20221213-1.3.3/LICENSE` & `alibabacloud_pairecservice20221213-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pairecservice20221213-1.3.3/PKG-INFO` & `alibabacloud_pairecservice20221213-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pairecservice20221213
-Version: 1.3.3
+Version: 1.4.0
 Summary: Alibaba Cloud PaiRecService (20221213) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pairecservice20221213-1.3.3/README-CN.md` & `alibabacloud_pairecservice20221213-1.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pairecservice20221213-1.3.3/README.md` & `alibabacloud_pairecservice20221213-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213/client.py` & `alibabacloud_pairecservice20221213-1.4.0/alibabacloud_pairecservice20221213/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1893,14 +1893,218 @@
         self,
         request: pai_rec_service_20221213_models.CreateParamRequest,
     ) -> pai_rec_service_20221213_models.CreateParamResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_param_with_options_async(request, headers, runtime)
 
+    def create_resource_rule_with_options(
+        self,
+        request: pai_rec_service_20221213_models.CreateResourceRuleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.CreateResourceRuleResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.description):
+            body['Description'] = request.description
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.metric_operation_type):
+            body['MetricOperationType'] = request.metric_operation_type
+        if not UtilClient.is_unset(request.metric_pull_info):
+            body['MetricPullInfo'] = request.metric_pull_info
+        if not UtilClient.is_unset(request.metric_pull_period):
+            body['MetricPullPeriod'] = request.metric_pull_period
+        if not UtilClient.is_unset(request.name):
+            body['Name'] = request.name
+        if not UtilClient.is_unset(request.rule_computing_definition):
+            body['RuleComputingDefinition'] = request.rule_computing_definition
+        if not UtilClient.is_unset(request.rule_items):
+            body['RuleItems'] = request.rule_items
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateResourceRule',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.CreateResourceRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_resource_rule_with_options_async(
+        self,
+        request: pai_rec_service_20221213_models.CreateResourceRuleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.CreateResourceRuleResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.description):
+            body['Description'] = request.description
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.metric_operation_type):
+            body['MetricOperationType'] = request.metric_operation_type
+        if not UtilClient.is_unset(request.metric_pull_info):
+            body['MetricPullInfo'] = request.metric_pull_info
+        if not UtilClient.is_unset(request.metric_pull_period):
+            body['MetricPullPeriod'] = request.metric_pull_period
+        if not UtilClient.is_unset(request.name):
+            body['Name'] = request.name
+        if not UtilClient.is_unset(request.rule_computing_definition):
+            body['RuleComputingDefinition'] = request.rule_computing_definition
+        if not UtilClient.is_unset(request.rule_items):
+            body['RuleItems'] = request.rule_items
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateResourceRule',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.CreateResourceRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_resource_rule(
+        self,
+        request: pai_rec_service_20221213_models.CreateResourceRuleRequest,
+    ) -> pai_rec_service_20221213_models.CreateResourceRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_resource_rule_with_options(request, headers, runtime)
+
+    async def create_resource_rule_async(
+        self,
+        request: pai_rec_service_20221213_models.CreateResourceRuleRequest,
+    ) -> pai_rec_service_20221213_models.CreateResourceRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_resource_rule_with_options_async(request, headers, runtime)
+
+    def create_resource_rule_item_with_options(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.CreateResourceRuleItemRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.CreateResourceRuleItemResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.description):
+            body['Description'] = request.description
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.max_value):
+            body['MaxValue'] = request.max_value
+        if not UtilClient.is_unset(request.min_value):
+            body['MinValue'] = request.min_value
+        if not UtilClient.is_unset(request.name):
+            body['Name'] = request.name
+        if not UtilClient.is_unset(request.value):
+            body['Value'] = request.value
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateResourceRuleItem',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}/items',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.CreateResourceRuleItemResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_resource_rule_item_with_options_async(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.CreateResourceRuleItemRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.CreateResourceRuleItemResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.description):
+            body['Description'] = request.description
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.max_value):
+            body['MaxValue'] = request.max_value
+        if not UtilClient.is_unset(request.min_value):
+            body['MinValue'] = request.min_value
+        if not UtilClient.is_unset(request.name):
+            body['Name'] = request.name
+        if not UtilClient.is_unset(request.value):
+            body['Value'] = request.value
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateResourceRuleItem',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}/items',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.CreateResourceRuleItemResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_resource_rule_item(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.CreateResourceRuleItemRequest,
+    ) -> pai_rec_service_20221213_models.CreateResourceRuleItemResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_resource_rule_item_with_options(resource_rule_id, request, headers, runtime)
+
+    async def create_resource_rule_item_async(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.CreateResourceRuleItemRequest,
+    ) -> pai_rec_service_20221213_models.CreateResourceRuleItemResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_resource_rule_item_with_options_async(resource_rule_id, request, headers, runtime)
+
     def create_scene_with_options(
         self,
         request: pai_rec_service_20221213_models.CreateSceneRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_rec_service_20221213_models.CreateSceneResponse:
         UtilClient.validate_model(request)
@@ -2169,14 +2373,110 @@
         self,
         request: pai_rec_service_20221213_models.CreateTableMetaRequest,
     ) -> pai_rec_service_20221213_models.CreateTableMetaResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_table_meta_with_options_async(request, headers, runtime)
 
+    def debug_resource_rule_with_options(
+        self,
+        resource_rule_id: str,
+        tmp_req: pai_rec_service_20221213_models.DebugResourceRuleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.DebugResourceRuleResponse:
+        UtilClient.validate_model(tmp_req)
+        request = pai_rec_service_20221213_models.DebugResourceRuleShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.metric_info):
+            request.metric_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.metric_info, 'MetricInfo', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.metric_info_shrink):
+            query['MetricInfo'] = request.metric_info_shrink
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DebugResourceRule',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}/action/debug',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.DebugResourceRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def debug_resource_rule_with_options_async(
+        self,
+        resource_rule_id: str,
+        tmp_req: pai_rec_service_20221213_models.DebugResourceRuleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.DebugResourceRuleResponse:
+        UtilClient.validate_model(tmp_req)
+        request = pai_rec_service_20221213_models.DebugResourceRuleShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.metric_info):
+            request.metric_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.metric_info, 'MetricInfo', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.metric_info_shrink):
+            query['MetricInfo'] = request.metric_info_shrink
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DebugResourceRule',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}/action/debug',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.DebugResourceRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def debug_resource_rule(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.DebugResourceRuleRequest,
+    ) -> pai_rec_service_20221213_models.DebugResourceRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.debug_resource_rule_with_options(resource_rule_id, request, headers, runtime)
+
+    async def debug_resource_rule_async(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.DebugResourceRuleRequest,
+    ) -> pai_rec_service_20221213_models.DebugResourceRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.debug_resource_rule_with_options_async(resource_rule_id, request, headers, runtime)
+
     def delete_abmetric_with_options(
         self,
         abmetric_id: str,
         request: pai_rec_service_20221213_models.DeleteABMetricRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_rec_service_20221213_models.DeleteABMetricResponse:
@@ -2879,14 +3179,178 @@
         param_id: str,
         request: pai_rec_service_20221213_models.DeleteParamRequest,
     ) -> pai_rec_service_20221213_models.DeleteParamResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.delete_param_with_options_async(param_id, request, headers, runtime)
 
+    def delete_resource_rule_with_options(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.DeleteResourceRuleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.DeleteResourceRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteResourceRule',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.DeleteResourceRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_resource_rule_with_options_async(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.DeleteResourceRuleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.DeleteResourceRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteResourceRule',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.DeleteResourceRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_resource_rule(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.DeleteResourceRuleRequest,
+    ) -> pai_rec_service_20221213_models.DeleteResourceRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.delete_resource_rule_with_options(resource_rule_id, request, headers, runtime)
+
+    async def delete_resource_rule_async(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.DeleteResourceRuleRequest,
+    ) -> pai_rec_service_20221213_models.DeleteResourceRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.delete_resource_rule_with_options_async(resource_rule_id, request, headers, runtime)
+
+    def delete_resource_rule_item_with_options(
+        self,
+        resource_rule_id: str,
+        resource_rule_item_id: str,
+        request: pai_rec_service_20221213_models.DeleteResourceRuleItemRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.DeleteResourceRuleItemResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteResourceRuleItem',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}/items/{OpenApiUtilClient.get_encode_param(resource_rule_item_id)}',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.DeleteResourceRuleItemResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_resource_rule_item_with_options_async(
+        self,
+        resource_rule_id: str,
+        resource_rule_item_id: str,
+        request: pai_rec_service_20221213_models.DeleteResourceRuleItemRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.DeleteResourceRuleItemResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteResourceRuleItem',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}/items/{OpenApiUtilClient.get_encode_param(resource_rule_item_id)}',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.DeleteResourceRuleItemResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_resource_rule_item(
+        self,
+        resource_rule_id: str,
+        resource_rule_item_id: str,
+        request: pai_rec_service_20221213_models.DeleteResourceRuleItemRequest,
+    ) -> pai_rec_service_20221213_models.DeleteResourceRuleItemResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.delete_resource_rule_item_with_options(resource_rule_id, resource_rule_item_id, request, headers, runtime)
+
+    async def delete_resource_rule_item_async(
+        self,
+        resource_rule_id: str,
+        resource_rule_item_id: str,
+        request: pai_rec_service_20221213_models.DeleteResourceRuleItemRequest,
+    ) -> pai_rec_service_20221213_models.DeleteResourceRuleItemResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.delete_resource_rule_item_with_options_async(resource_rule_id, resource_rule_item_id, request, headers, runtime)
+
     def delete_scene_with_options(
         self,
         scene_id: str,
         request: pai_rec_service_20221213_models.DeleteSceneRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_rec_service_20221213_models.DeleteSceneResponse:
@@ -4053,14 +4517,94 @@
         layer_id: str,
         request: pai_rec_service_20221213_models.GetLayerRequest,
     ) -> pai_rec_service_20221213_models.GetLayerResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_layer_with_options_async(layer_id, request, headers, runtime)
 
+    def get_resource_rule_with_options(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.GetResourceRuleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.GetResourceRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetResourceRule',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.GetResourceRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_resource_rule_with_options_async(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.GetResourceRuleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.GetResourceRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetResourceRule',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.GetResourceRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_resource_rule(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.GetResourceRuleRequest,
+    ) -> pai_rec_service_20221213_models.GetResourceRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_resource_rule_with_options(resource_rule_id, request, headers, runtime)
+
+    async def get_resource_rule_async(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.GetResourceRuleRequest,
+    ) -> pai_rec_service_20221213_models.GetResourceRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_resource_rule_with_options_async(resource_rule_id, request, headers, runtime)
+
     def get_scene_with_options(
         self,
         scene_id: str,
         request: pai_rec_service_20221213_models.GetSceneRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_rec_service_20221213_models.GetSceneResponse:
@@ -5745,14 +6289,118 @@
         self,
         request: pai_rec_service_20221213_models.ListParamsRequest,
     ) -> pai_rec_service_20221213_models.ListParamsResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_params_with_options_async(request, headers, runtime)
 
+    def list_resource_rules_with_options(
+        self,
+        request: pai_rec_service_20221213_models.ListResourceRulesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.ListResourceRulesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.all):
+            query['All'] = request.all
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.order):
+            query['Order'] = request.order
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_rule_id):
+            query['ResourceRuleId'] = request.resource_rule_id
+        if not UtilClient.is_unset(request.resource_rule_name):
+            query['ResourceRuleName'] = request.resource_rule_name
+        if not UtilClient.is_unset(request.sort_by):
+            query['SortBy'] = request.sort_by
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListResourceRules',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.ListResourceRulesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_resource_rules_with_options_async(
+        self,
+        request: pai_rec_service_20221213_models.ListResourceRulesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.ListResourceRulesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.all):
+            query['All'] = request.all
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.order):
+            query['Order'] = request.order
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.resource_rule_id):
+            query['ResourceRuleId'] = request.resource_rule_id
+        if not UtilClient.is_unset(request.resource_rule_name):
+            query['ResourceRuleName'] = request.resource_rule_name
+        if not UtilClient.is_unset(request.sort_by):
+            query['SortBy'] = request.sort_by
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListResourceRules',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.ListResourceRulesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_resource_rules(
+        self,
+        request: pai_rec_service_20221213_models.ListResourceRulesRequest,
+    ) -> pai_rec_service_20221213_models.ListResourceRulesResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_resource_rules_with_options(request, headers, runtime)
+
+    async def list_resource_rules_async(
+        self,
+        request: pai_rec_service_20221213_models.ListResourceRulesRequest,
+    ) -> pai_rec_service_20221213_models.ListResourceRulesResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_resource_rules_with_options_async(request, headers, runtime)
+
     def list_scenes_with_options(
         self,
         request: pai_rec_service_20221213_models.ListScenesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_rec_service_20221213_models.ListScenesResponse:
         UtilClient.validate_model(request)
@@ -6561,14 +7209,106 @@
         experiment_id: str,
         request: pai_rec_service_20221213_models.PushAllExperimentRequest,
     ) -> pai_rec_service_20221213_models.PushAllExperimentResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.push_all_experiment_with_options_async(experiment_id, request, headers, runtime)
 
+    def push_resource_rule_with_options(
+        self,
+        resource_rule_id: str,
+        tmp_req: pai_rec_service_20221213_models.PushResourceRuleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.PushResourceRuleResponse:
+        UtilClient.validate_model(tmp_req)
+        request = pai_rec_service_20221213_models.PushResourceRuleShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.metric_info):
+            request.metric_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.metric_info, 'MetricInfo', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.metric_info_shrink):
+            query['MetricInfo'] = request.metric_info_shrink
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='PushResourceRule',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}/action/push',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.PushResourceRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def push_resource_rule_with_options_async(
+        self,
+        resource_rule_id: str,
+        tmp_req: pai_rec_service_20221213_models.PushResourceRuleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.PushResourceRuleResponse:
+        UtilClient.validate_model(tmp_req)
+        request = pai_rec_service_20221213_models.PushResourceRuleShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.metric_info):
+            request.metric_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.metric_info, 'MetricInfo', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.metric_info_shrink):
+            query['MetricInfo'] = request.metric_info_shrink
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='PushResourceRule',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}/action/push',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.PushResourceRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def push_resource_rule(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.PushResourceRuleRequest,
+    ) -> pai_rec_service_20221213_models.PushResourceRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.push_resource_rule_with_options(resource_rule_id, request, headers, runtime)
+
+    async def push_resource_rule_async(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.PushResourceRuleRequest,
+    ) -> pai_rec_service_20221213_models.PushResourceRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.push_resource_rule_with_options_async(resource_rule_id, request, headers, runtime)
+
     def report_abmetric_group_with_options(
         self,
         abmetric_group_id: str,
         request: pai_rec_service_20221213_models.ReportABMetricGroupRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_rec_service_20221213_models.ReportABMetricGroupResponse:
@@ -8013,14 +8753,222 @@
         param_id: str,
         request: pai_rec_service_20221213_models.UpdateParamRequest,
     ) -> pai_rec_service_20221213_models.UpdateParamResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.update_param_with_options_async(param_id, request, headers, runtime)
 
+    def update_resource_rule_with_options(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.UpdateResourceRuleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.UpdateResourceRuleResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.description):
+            body['Description'] = request.description
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.metric_operation_type):
+            body['MetricOperationType'] = request.metric_operation_type
+        if not UtilClient.is_unset(request.metric_pull_info):
+            body['MetricPullInfo'] = request.metric_pull_info
+        if not UtilClient.is_unset(request.metric_pull_period):
+            body['MetricPullPeriod'] = request.metric_pull_period
+        if not UtilClient.is_unset(request.name):
+            body['Name'] = request.name
+        if not UtilClient.is_unset(request.rule_computing_definition):
+            body['RuleComputingDefinition'] = request.rule_computing_definition
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateResourceRule',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.UpdateResourceRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def update_resource_rule_with_options_async(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.UpdateResourceRuleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.UpdateResourceRuleResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.description):
+            body['Description'] = request.description
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.metric_operation_type):
+            body['MetricOperationType'] = request.metric_operation_type
+        if not UtilClient.is_unset(request.metric_pull_info):
+            body['MetricPullInfo'] = request.metric_pull_info
+        if not UtilClient.is_unset(request.metric_pull_period):
+            body['MetricPullPeriod'] = request.metric_pull_period
+        if not UtilClient.is_unset(request.name):
+            body['Name'] = request.name
+        if not UtilClient.is_unset(request.rule_computing_definition):
+            body['RuleComputingDefinition'] = request.rule_computing_definition
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateResourceRule',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.UpdateResourceRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_resource_rule(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.UpdateResourceRuleRequest,
+    ) -> pai_rec_service_20221213_models.UpdateResourceRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_resource_rule_with_options(resource_rule_id, request, headers, runtime)
+
+    async def update_resource_rule_async(
+        self,
+        resource_rule_id: str,
+        request: pai_rec_service_20221213_models.UpdateResourceRuleRequest,
+    ) -> pai_rec_service_20221213_models.UpdateResourceRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_resource_rule_with_options_async(resource_rule_id, request, headers, runtime)
+
+    def update_resource_rule_item_with_options(
+        self,
+        resource_rule_id: str,
+        resource_rule_item_id: str,
+        request: pai_rec_service_20221213_models.UpdateResourceRuleItemRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.UpdateResourceRuleItemResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.description):
+            body['Description'] = request.description
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.max_value):
+            body['MaxValue'] = request.max_value
+        if not UtilClient.is_unset(request.min_value):
+            body['MinValue'] = request.min_value
+        if not UtilClient.is_unset(request.name):
+            body['Name'] = request.name
+        if not UtilClient.is_unset(request.value):
+            body['Value'] = request.value
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateResourceRuleItem',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}/items/{OpenApiUtilClient.get_encode_param(resource_rule_item_id)}',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.UpdateResourceRuleItemResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def update_resource_rule_item_with_options_async(
+        self,
+        resource_rule_id: str,
+        resource_rule_item_id: str,
+        request: pai_rec_service_20221213_models.UpdateResourceRuleItemRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_rec_service_20221213_models.UpdateResourceRuleItemResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.description):
+            body['Description'] = request.description
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.max_value):
+            body['MaxValue'] = request.max_value
+        if not UtilClient.is_unset(request.min_value):
+            body['MinValue'] = request.min_value
+        if not UtilClient.is_unset(request.name):
+            body['Name'] = request.name
+        if not UtilClient.is_unset(request.value):
+            body['Value'] = request.value
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateResourceRuleItem',
+            version='2022-12-13',
+            protocol='HTTPS',
+            pathname=f'/api/v1/resourcerules/{OpenApiUtilClient.get_encode_param(resource_rule_id)}/items/{OpenApiUtilClient.get_encode_param(resource_rule_item_id)}',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_rec_service_20221213_models.UpdateResourceRuleItemResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_resource_rule_item(
+        self,
+        resource_rule_id: str,
+        resource_rule_item_id: str,
+        request: pai_rec_service_20221213_models.UpdateResourceRuleItemRequest,
+    ) -> pai_rec_service_20221213_models.UpdateResourceRuleItemResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_resource_rule_item_with_options(resource_rule_id, resource_rule_item_id, request, headers, runtime)
+
+    async def update_resource_rule_item_async(
+        self,
+        resource_rule_id: str,
+        resource_rule_item_id: str,
+        request: pai_rec_service_20221213_models.UpdateResourceRuleItemRequest,
+    ) -> pai_rec_service_20221213_models.UpdateResourceRuleItemResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_resource_rule_item_with_options_async(resource_rule_id, resource_rule_item_id, request, headers, runtime)
+
     def update_scene_with_options(
         self,
         scene_id: str,
         request: pai_rec_service_20221213_models.UpdateSceneRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_rec_service_20221213_models.UpdateSceneResponse:
```

### Comparing `alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213/models.py` & `alibabacloud_pairecservice20221213-1.4.0/alibabacloud_pairecservice20221213/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -2597,14 +2597,347 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateParamResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateResourceRuleRequestRuleItems(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        max_value: float = None,
+        min_value: float = None,
+        name: str = None,
+        value: float = None,
+    ):
+        self.description = description
+        self.max_value = max_value
+        self.min_value = min_value
+        self.name = name
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.max_value is not None:
+            result['MaxValue'] = self.max_value
+        if self.min_value is not None:
+            result['MinValue'] = self.min_value
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('MaxValue') is not None:
+            self.max_value = m.get('MaxValue')
+        if m.get('MinValue') is not None:
+            self.min_value = m.get('MinValue')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class CreateResourceRuleRequest(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        instance_id: str = None,
+        metric_operation_type: str = None,
+        metric_pull_info: str = None,
+        metric_pull_period: str = None,
+        name: str = None,
+        rule_computing_definition: str = None,
+        rule_items: List[CreateResourceRuleRequestRuleItems] = None,
+    ):
+        self.description = description
+        self.instance_id = instance_id
+        self.metric_operation_type = metric_operation_type
+        self.metric_pull_info = metric_pull_info
+        self.metric_pull_period = metric_pull_period
+        self.name = name
+        self.rule_computing_definition = rule_computing_definition
+        self.rule_items = rule_items
+
+    def validate(self):
+        if self.rule_items:
+            for k in self.rule_items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.metric_operation_type is not None:
+            result['MetricOperationType'] = self.metric_operation_type
+        if self.metric_pull_info is not None:
+            result['MetricPullInfo'] = self.metric_pull_info
+        if self.metric_pull_period is not None:
+            result['MetricPullPeriod'] = self.metric_pull_period
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.rule_computing_definition is not None:
+            result['RuleComputingDefinition'] = self.rule_computing_definition
+        result['RuleItems'] = []
+        if self.rule_items is not None:
+            for k in self.rule_items:
+                result['RuleItems'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('MetricOperationType') is not None:
+            self.metric_operation_type = m.get('MetricOperationType')
+        if m.get('MetricPullInfo') is not None:
+            self.metric_pull_info = m.get('MetricPullInfo')
+        if m.get('MetricPullPeriod') is not None:
+            self.metric_pull_period = m.get('MetricPullPeriod')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('RuleComputingDefinition') is not None:
+            self.rule_computing_definition = m.get('RuleComputingDefinition')
+        self.rule_items = []
+        if m.get('RuleItems') is not None:
+            for k in m.get('RuleItems'):
+                temp_model = CreateResourceRuleRequestRuleItems()
+                self.rule_items.append(temp_model.from_map(k))
+        return self
+
+
+class CreateResourceRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        resource_rule_id: str = None,
+    ):
+        self.request_id = request_id
+        self.resource_rule_id = resource_rule_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.resource_rule_id is not None:
+            result['ResourceRuleId'] = self.resource_rule_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ResourceRuleId') is not None:
+            self.resource_rule_id = m.get('ResourceRuleId')
+        return self
+
+
+class CreateResourceRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateResourceRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateResourceRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class CreateResourceRuleItemRequest(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        instance_id: str = None,
+        max_value: float = None,
+        min_value: float = None,
+        name: str = None,
+        value: float = None,
+    ):
+        self.description = description
+        self.instance_id = instance_id
+        self.max_value = max_value
+        self.min_value = min_value
+        self.name = name
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.max_value is not None:
+            result['MaxValue'] = self.max_value
+        if self.min_value is not None:
+            result['MinValue'] = self.min_value
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('MaxValue') is not None:
+            self.max_value = m.get('MaxValue')
+        if m.get('MinValue') is not None:
+            self.min_value = m.get('MinValue')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class CreateResourceRuleItemResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        resource_rule_item_id: str = None,
+    ):
+        self.request_id = request_id
+        self.resource_rule_item_id = resource_rule_item_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.resource_rule_item_id is not None:
+            result['ResourceRuleItemId'] = self.resource_rule_item_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ResourceRuleItemId') is not None:
+            self.resource_rule_item_id = m.get('ResourceRuleItemId')
+        return self
+
+
+class CreateResourceRuleItemResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateResourceRuleItemResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateResourceRuleItemResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateSceneRequestFlows(TeaModel):
     def __init__(
         self,
         flow_code: str = None,
         flow_name: str = None,
     ):
         self.flow_code = flow_code
@@ -3074,14 +3407,172 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateTableMetaResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DebugResourceRuleRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        metric_info: Dict[str, Any] = None,
+        region_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.metric_info = metric_info
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.metric_info is not None:
+            result['MetricInfo'] = self.metric_info
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('MetricInfo') is not None:
+            self.metric_info = m.get('MetricInfo')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class DebugResourceRuleShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        metric_info_shrink: str = None,
+        region_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.metric_info_shrink = metric_info_shrink
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.metric_info_shrink is not None:
+            result['MetricInfo'] = self.metric_info_shrink
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('MetricInfo') is not None:
+            self.metric_info_shrink = m.get('MetricInfo')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class DebugResourceRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        current_values: Dict[str, Any] = None,
+        output_values: Dict[str, Any] = None,
+        request_id: str = None,
+    ):
+        self.current_values = current_values
+        self.output_values = output_values
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_values is not None:
+            result['CurrentValues'] = self.current_values
+        if self.output_values is not None:
+            result['OutputValues'] = self.output_values
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CurrentValues') is not None:
+            self.current_values = m.get('CurrentValues')
+        if m.get('OutputValues') is not None:
+            self.output_values = m.get('OutputValues')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DebugResourceRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DebugResourceRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DebugResourceRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteABMetricRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         self.instance_id = instance_id
 
@@ -3908,14 +4399,204 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteParamResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteResourceRuleRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+    ):
+        self.instance_id = instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        return self
+
+
+class DeleteResourceRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteResourceRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteResourceRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteResourceRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DeleteResourceRuleItemRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+    ):
+        self.instance_id = instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        return self
+
+
+class DeleteResourceRuleItemResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteResourceRuleItemResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteResourceRuleItemResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteResourceRuleItemResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteSceneRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         self.instance_id = instance_id
 
@@ -6407,14 +7088,216 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetLayerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetResourceRuleRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+    ):
+        self.instance_id = instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        return self
+
+
+class GetResourceRuleResponseBodyRuleItems(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        max_value: str = None,
+        min_value: str = None,
+        name: str = None,
+        value: str = None,
+    ):
+        self.description = description
+        self.max_value = max_value
+        self.min_value = min_value
+        self.name = name
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.max_value is not None:
+            result['MaxValue'] = self.max_value
+        if self.min_value is not None:
+            result['MinValue'] = self.min_value
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('MaxValue') is not None:
+            self.max_value = m.get('MaxValue')
+        if m.get('MinValue') is not None:
+            self.min_value = m.get('MinValue')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class GetResourceRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        metric_operation_type: str = None,
+        metric_pull_info: str = None,
+        metric_pull_period: str = None,
+        name: str = None,
+        request_id: str = None,
+        resource_rule_id: str = None,
+        rule_computing_definition: str = None,
+        rule_items: List[GetResourceRuleResponseBodyRuleItems] = None,
+    ):
+        self.description = description
+        self.metric_operation_type = metric_operation_type
+        self.metric_pull_info = metric_pull_info
+        self.metric_pull_period = metric_pull_period
+        self.name = name
+        self.request_id = request_id
+        self.resource_rule_id = resource_rule_id
+        self.rule_computing_definition = rule_computing_definition
+        self.rule_items = rule_items
+
+    def validate(self):
+        if self.rule_items:
+            for k in self.rule_items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.metric_operation_type is not None:
+            result['MetricOperationType'] = self.metric_operation_type
+        if self.metric_pull_info is not None:
+            result['MetricPullInfo'] = self.metric_pull_info
+        if self.metric_pull_period is not None:
+            result['MetricPullPeriod'] = self.metric_pull_period
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.resource_rule_id is not None:
+            result['ResourceRuleId'] = self.resource_rule_id
+        if self.rule_computing_definition is not None:
+            result['RuleComputingDefinition'] = self.rule_computing_definition
+        result['RuleItems'] = []
+        if self.rule_items is not None:
+            for k in self.rule_items:
+                result['RuleItems'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('MetricOperationType') is not None:
+            self.metric_operation_type = m.get('MetricOperationType')
+        if m.get('MetricPullInfo') is not None:
+            self.metric_pull_info = m.get('MetricPullInfo')
+        if m.get('MetricPullPeriod') is not None:
+            self.metric_pull_period = m.get('MetricPullPeriod')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ResourceRuleId') is not None:
+            self.resource_rule_id = m.get('ResourceRuleId')
+        if m.get('RuleComputingDefinition') is not None:
+            self.rule_computing_definition = m.get('RuleComputingDefinition')
+        self.rule_items = []
+        if m.get('RuleItems') is not None:
+            for k in m.get('RuleItems'):
+                temp_model = GetResourceRuleResponseBodyRuleItems()
+                self.rule_items.append(temp_model.from_map(k))
+        return self
+
+
+class GetResourceRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetResourceRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetResourceRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetSceneRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         self.instance_id = instance_id
 
@@ -10695,14 +11578,299 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListParamsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListResourceRulesRequest(TeaModel):
+    def __init__(
+        self,
+        all: bool = None,
+        instance_id: str = None,
+        order: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        resource_rule_id: str = None,
+        resource_rule_name: str = None,
+        sort_by: str = None,
+    ):
+        self.all = all
+        self.instance_id = instance_id
+        self.order = order
+        self.page_number = page_number
+        self.page_size = page_size
+        self.resource_rule_id = resource_rule_id
+        self.resource_rule_name = resource_rule_name
+        self.sort_by = sort_by
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.all is not None:
+            result['All'] = self.all
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.order is not None:
+            result['Order'] = self.order
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.resource_rule_id is not None:
+            result['ResourceRuleId'] = self.resource_rule_id
+        if self.resource_rule_name is not None:
+            result['ResourceRuleName'] = self.resource_rule_name
+        if self.sort_by is not None:
+            result['SortBy'] = self.sort_by
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('All') is not None:
+            self.all = m.get('All')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('Order') is not None:
+            self.order = m.get('Order')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('ResourceRuleId') is not None:
+            self.resource_rule_id = m.get('ResourceRuleId')
+        if m.get('ResourceRuleName') is not None:
+            self.resource_rule_name = m.get('ResourceRuleName')
+        if m.get('SortBy') is not None:
+            self.sort_by = m.get('SortBy')
+        return self
+
+
+class ListResourceRulesResponseBodyResourceRulesRuleItems(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        max_value: str = None,
+        min_value: str = None,
+        name: str = None,
+        value: str = None,
+    ):
+        self.description = description
+        self.max_value = max_value
+        self.min_value = min_value
+        self.name = name
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.max_value is not None:
+            result['MaxValue'] = self.max_value
+        if self.min_value is not None:
+            result['MinValue'] = self.min_value
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('MaxValue') is not None:
+            self.max_value = m.get('MaxValue')
+        if m.get('MinValue') is not None:
+            self.min_value = m.get('MinValue')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListResourceRulesResponseBodyResourceRules(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        metric_operation_type: str = None,
+        metric_pull_info: str = None,
+        metric_pull_period: str = None,
+        name: str = None,
+        resource_rule_id: str = None,
+        rule_computing_definition: str = None,
+        rule_items: List[ListResourceRulesResponseBodyResourceRulesRuleItems] = None,
+    ):
+        self.description = description
+        self.metric_operation_type = metric_operation_type
+        self.metric_pull_info = metric_pull_info
+        self.metric_pull_period = metric_pull_period
+        self.name = name
+        self.resource_rule_id = resource_rule_id
+        self.rule_computing_definition = rule_computing_definition
+        self.rule_items = rule_items
+
+    def validate(self):
+        if self.rule_items:
+            for k in self.rule_items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.metric_operation_type is not None:
+            result['MetricOperationType'] = self.metric_operation_type
+        if self.metric_pull_info is not None:
+            result['MetricPullInfo'] = self.metric_pull_info
+        if self.metric_pull_period is not None:
+            result['MetricPullPeriod'] = self.metric_pull_period
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.resource_rule_id is not None:
+            result['ResourceRuleId'] = self.resource_rule_id
+        if self.rule_computing_definition is not None:
+            result['RuleComputingDefinition'] = self.rule_computing_definition
+        result['RuleItems'] = []
+        if self.rule_items is not None:
+            for k in self.rule_items:
+                result['RuleItems'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('MetricOperationType') is not None:
+            self.metric_operation_type = m.get('MetricOperationType')
+        if m.get('MetricPullInfo') is not None:
+            self.metric_pull_info = m.get('MetricPullInfo')
+        if m.get('MetricPullPeriod') is not None:
+            self.metric_pull_period = m.get('MetricPullPeriod')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('ResourceRuleId') is not None:
+            self.resource_rule_id = m.get('ResourceRuleId')
+        if m.get('RuleComputingDefinition') is not None:
+            self.rule_computing_definition = m.get('RuleComputingDefinition')
+        self.rule_items = []
+        if m.get('RuleItems') is not None:
+            for k in m.get('RuleItems'):
+                temp_model = ListResourceRulesResponseBodyResourceRulesRuleItems()
+                self.rule_items.append(temp_model.from_map(k))
+        return self
+
+
+class ListResourceRulesResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        resource_rules: List[ListResourceRulesResponseBodyResourceRules] = None,
+        total_count: int = None,
+    ):
+        self.request_id = request_id
+        self.resource_rules = resource_rules
+        self.total_count = total_count
+
+    def validate(self):
+        if self.resource_rules:
+            for k in self.resource_rules:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['ResourceRules'] = []
+        if self.resource_rules is not None:
+            for k in self.resource_rules:
+                result['ResourceRules'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.resource_rules = []
+        if m.get('ResourceRules') is not None:
+            for k in m.get('ResourceRules'):
+                temp_model = ListResourceRulesResponseBodyResourceRules()
+                self.resource_rules.append(temp_model.from_map(k))
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListResourceRulesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListResourceRulesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListResourceRulesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListScenesRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         name: str = None,
     ):
         self.instance_id = instance_id
@@ -12045,14 +13213,255 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PushAllExperimentResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class PushResourceRuleRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        metric_info: Dict[str, Any] = None,
+    ):
+        self.instance_id = instance_id
+        self.metric_info = metric_info
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.metric_info is not None:
+            result['MetricInfo'] = self.metric_info
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('MetricInfo') is not None:
+            self.metric_info = m.get('MetricInfo')
+        return self
+
+
+class PushResourceRuleShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        metric_info_shrink: str = None,
+    ):
+        self.instance_id = instance_id
+        self.metric_info_shrink = metric_info_shrink
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.metric_info_shrink is not None:
+            result['MetricInfo'] = self.metric_info_shrink
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('MetricInfo') is not None:
+            self.metric_info_shrink = m.get('MetricInfo')
+        return self
+
+
+class PushResourceRuleResponseBodyRuleItems(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        max_value: str = None,
+        min_value: str = None,
+        name: str = None,
+        value: str = None,
+    ):
+        self.description = description
+        self.max_value = max_value
+        self.min_value = min_value
+        self.name = name
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.max_value is not None:
+            result['MaxValue'] = self.max_value
+        if self.min_value is not None:
+            result['MinValue'] = self.min_value
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('MaxValue') is not None:
+            self.max_value = m.get('MaxValue')
+        if m.get('MinValue') is not None:
+            self.min_value = m.get('MinValue')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class PushResourceRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        metric_operation_type: str = None,
+        metric_pull_info: str = None,
+        metric_pull_period: str = None,
+        name: str = None,
+        request_id: str = None,
+        resource_rule_id: str = None,
+        rule_computing_definition: str = None,
+        rule_items: List[PushResourceRuleResponseBodyRuleItems] = None,
+    ):
+        self.description = description
+        self.metric_operation_type = metric_operation_type
+        self.metric_pull_info = metric_pull_info
+        self.metric_pull_period = metric_pull_period
+        self.name = name
+        self.request_id = request_id
+        self.resource_rule_id = resource_rule_id
+        self.rule_computing_definition = rule_computing_definition
+        self.rule_items = rule_items
+
+    def validate(self):
+        if self.rule_items:
+            for k in self.rule_items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.metric_operation_type is not None:
+            result['MetricOperationType'] = self.metric_operation_type
+        if self.metric_pull_info is not None:
+            result['MetricPullInfo'] = self.metric_pull_info
+        if self.metric_pull_period is not None:
+            result['MetricPullPeriod'] = self.metric_pull_period
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.resource_rule_id is not None:
+            result['ResourceRuleId'] = self.resource_rule_id
+        if self.rule_computing_definition is not None:
+            result['RuleComputingDefinition'] = self.rule_computing_definition
+        result['RuleItems'] = []
+        if self.rule_items is not None:
+            for k in self.rule_items:
+                result['RuleItems'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('MetricOperationType') is not None:
+            self.metric_operation_type = m.get('MetricOperationType')
+        if m.get('MetricPullInfo') is not None:
+            self.metric_pull_info = m.get('MetricPullInfo')
+        if m.get('MetricPullPeriod') is not None:
+            self.metric_pull_period = m.get('MetricPullPeriod')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ResourceRuleId') is not None:
+            self.resource_rule_id = m.get('ResourceRuleId')
+        if m.get('RuleComputingDefinition') is not None:
+            self.rule_computing_definition = m.get('RuleComputingDefinition')
+        self.rule_items = []
+        if m.get('RuleItems') is not None:
+            for k in m.get('RuleItems'):
+                temp_model = PushResourceRuleResponseBodyRuleItems()
+                self.rule_items.append(temp_model.from_map(k))
+        return self
+
+
+class PushResourceRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: PushResourceRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = PushResourceRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ReportABMetricGroupRequest(TeaModel):
     def __init__(
         self,
         base_experiment_id: str = None,
         dimension_fields: str = None,
         end_date: str = None,
         experiment_group_id: str = None,
@@ -13924,14 +15333,270 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateParamResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateResourceRuleRequest(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        instance_id: str = None,
+        metric_operation_type: str = None,
+        metric_pull_info: str = None,
+        metric_pull_period: str = None,
+        name: str = None,
+        rule_computing_definition: str = None,
+    ):
+        self.description = description
+        self.instance_id = instance_id
+        self.metric_operation_type = metric_operation_type
+        self.metric_pull_info = metric_pull_info
+        self.metric_pull_period = metric_pull_period
+        self.name = name
+        self.rule_computing_definition = rule_computing_definition
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.metric_operation_type is not None:
+            result['MetricOperationType'] = self.metric_operation_type
+        if self.metric_pull_info is not None:
+            result['MetricPullInfo'] = self.metric_pull_info
+        if self.metric_pull_period is not None:
+            result['MetricPullPeriod'] = self.metric_pull_period
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.rule_computing_definition is not None:
+            result['RuleComputingDefinition'] = self.rule_computing_definition
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('MetricOperationType') is not None:
+            self.metric_operation_type = m.get('MetricOperationType')
+        if m.get('MetricPullInfo') is not None:
+            self.metric_pull_info = m.get('MetricPullInfo')
+        if m.get('MetricPullPeriod') is not None:
+            self.metric_pull_period = m.get('MetricPullPeriod')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('RuleComputingDefinition') is not None:
+            self.rule_computing_definition = m.get('RuleComputingDefinition')
+        return self
+
+
+class UpdateResourceRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateResourceRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateResourceRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateResourceRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UpdateResourceRuleItemRequest(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        instance_id: str = None,
+        max_value: float = None,
+        min_value: float = None,
+        name: str = None,
+        value: float = None,
+    ):
+        self.description = description
+        self.instance_id = instance_id
+        self.max_value = max_value
+        self.min_value = min_value
+        self.name = name
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.max_value is not None:
+            result['MaxValue'] = self.max_value
+        if self.min_value is not None:
+            result['MinValue'] = self.min_value
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('MaxValue') is not None:
+            self.max_value = m.get('MaxValue')
+        if m.get('MinValue') is not None:
+            self.min_value = m.get('MinValue')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class UpdateResourceRuleItemResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateResourceRuleItemResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateResourceRuleItemResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateResourceRuleItemResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateSceneRequestFlows(TeaModel):
     def __init__(
         self,
         flow_code: str = None,
         flow_name: str = None,
     ):
         self.flow_code = flow_code
```

### Comparing `alibabacloud_pairecservice20221213-1.3.3/alibabacloud_pairecservice20221213.egg-info/PKG-INFO` & `alibabacloud_pairecservice20221213-1.4.0/alibabacloud_pairecservice20221213.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pairecservice20221213
-Version: 1.3.3
+Version: 1.4.0
 Summary: Alibaba Cloud PaiRecService (20221213) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pairecservice20221213-1.3.3/setup.py` & `alibabacloud_pairecservice20221213-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pairecservice20221213.
 
-Created on 28/04/2024
+Created on 07/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pairecservice20221213"
 NAME = "alibabacloud_pairecservice20221213" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud PaiRecService (20221213) SDK Library for Python"
```

