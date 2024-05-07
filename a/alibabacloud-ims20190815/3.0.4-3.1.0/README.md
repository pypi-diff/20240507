# Comparing `tmp/alibabacloud_ims20190815-3.0.4.tar.gz` & `tmp/alibabacloud_ims20190815-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ims20190815-3.0.4.tar", last modified: Thu Dec 14 08:23:02 2023, max compression
+gzip compressed data, was "dist/alibabacloud_ims20190815-3.1.0.tar", last modified: Tue May  7 08:22:53 2024, max compression
```

## Comparing `alibabacloud_ims20190815-3.0.4.tar` & `alibabacloud_ims20190815-3.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/
--rw-r--r--   0 root         (0) root         (0)     1039 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/alibabacloud_ims20190815/
--rw-r--r--   0 root         (0) root         (0)       21 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/alibabacloud_ims20190815/__init__.py
--rw-r--r--   0 root         (0) root         (0)   240332 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/alibabacloud_ims20190815/client.py
--rw-r--r--   0 root         (0) root         (0)   505212 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/alibabacloud_ims20190815/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/alibabacloud_ims20190815.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/alibabacloud_ims20190815.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/alibabacloud_ims20190815.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/alibabacloud_ims20190815.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/alibabacloud_ims20190815.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/alibabacloud_ims20190815.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2023-12-14 08:23:02.000000 alibabacloud_ims20190815-3.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/alibabacloud_ims20190815/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/alibabacloud_ims20190815/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   241702 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/alibabacloud_ims20190815/client.py
+-rw-r--r--   0 root         (0) root         (0)   501332 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/alibabacloud_ims20190815/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/alibabacloud_ims20190815.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/alibabacloud_ims20190815.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/alibabacloud_ims20190815.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/alibabacloud_ims20190815.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/alibabacloud_ims20190815.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/alibabacloud_ims20190815.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-05-07 08:22:53.000000 alibabacloud_ims20190815-3.1.0/setup.py
```

### Comparing `alibabacloud_ims20190815-3.0.4/ChangeLog.md` & `alibabacloud_ims20190815-3.1.0/ChangeLog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-12-14 Version: 3.0.4
+- Generated python 2019-08-15 for Ims.
+
 2023-11-23 Version: 3.0.3
 - Generated python 2019-08-15 for Ims.
 
 2023-09-11 Version: 3.0.2
 - Generated python 2019-08-15 for Ims.
 
 2023-08-11 Version: 3.0.1
```

### Comparing `alibabacloud_ims20190815-3.0.4/LICENSE` & `alibabacloud_ims20190815-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ims20190815-3.0.4/PKG-INFO` & `alibabacloud_ims20190815-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ims20190815
-Version: 3.0.4
+Version: 3.1.0
 Summary: Alibaba Cloud Ims (20190815) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/ims-20190815/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_ims20190815-3.0.4/README-CN.md` & `alibabacloud_ims20190815-3.1.0/README-CN.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/ims-20190815/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_ims20190815-3.0.4/README.md` & `alibabacloud_ims20190815-3.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/ims-20190815/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_ims20190815-3.0.4/alibabacloud_ims20190815/client.py` & `alibabacloud_ims20190815-3.1.0/alibabacloud_ims20190815/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,22 +42,14 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def add_client_id_to_oidcprovider_with_options(
         self,
         request: ims_20190815_models.AddClientIdToOIDCProviderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ims_20190815_models.AddClientIdToOIDCProviderResponse:
-        """
-        ###
-        This topic provides an example on how to add the client ID `598469743454717****` to the OIDC IdP named `TestOIDCProvider`.
-        
-        @param request: AddClientIdToOIDCProviderRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddClientIdToOIDCProviderResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_id):
             query['ClientId'] = request.client_id
         if not UtilClient.is_unset(request.oidcprovider_name):
             query['OIDCProviderName'] = request.oidcprovider_name
         req = open_api_models.OpenApiRequest(
@@ -80,22 +72,14 @@
         )
 
     async def add_client_id_to_oidcprovider_with_options_async(
         self,
         request: ims_20190815_models.AddClientIdToOIDCProviderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ims_20190815_models.AddClientIdToOIDCProviderResponse:
-        """
-        ###
-        This topic provides an example on how to add the client ID `598469743454717****` to the OIDC IdP named `TestOIDCProvider`.
-        
-        @param request: AddClientIdToOIDCProviderRequest
-        @param runtime: runtime options for this request RuntimeOptions
-        @return: AddClientIdToOIDCProviderResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_id):
             query['ClientId'] = request.client_id
         if not UtilClient.is_unset(request.oidcprovider_name):
             query['OIDCProviderName'] = request.oidcprovider_name
         req = open_api_models.OpenApiRequest(
@@ -117,35 +101,21 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def add_client_id_to_oidcprovider(
         self,
         request: ims_20190815_models.AddClientIdToOIDCProviderRequest,
     ) -> ims_20190815_models.AddClientIdToOIDCProviderResponse:
-        """
-        ###
-        This topic provides an example on how to add the client ID `598469743454717****` to the OIDC IdP named `TestOIDCProvider`.
-        
-        @param request: AddClientIdToOIDCProviderRequest
-        @return: AddClientIdToOIDCProviderResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.add_client_id_to_oidcprovider_with_options(request, runtime)
 
     async def add_client_id_to_oidcprovider_async(
         self,
         request: ims_20190815_models.AddClientIdToOIDCProviderRequest,
     ) -> ims_20190815_models.AddClientIdToOIDCProviderResponse:
-        """
-        ###
-        This topic provides an example on how to add the client ID `598469743454717****` to the OIDC IdP named `TestOIDCProvider`.
-        
-        @param request: AddClientIdToOIDCProviderRequest
-        @return: AddClientIdToOIDCProviderResponse
-        """
         runtime = util_models.RuntimeOptions()
         return await self.add_client_id_to_oidcprovider_with_options_async(request, runtime)
 
     def add_fingerprint_to_oidcprovider_with_options(
         self,
         request: ims_20190815_models.AddFingerprintToOIDCProviderRequest,
         runtime: util_models.RuntimeOptions,
@@ -3289,14 +3259,84 @@
         runtime = util_models.RuntimeOptions()
         return self.get_user_sso_settings_with_options(runtime)
 
     async def get_user_sso_settings_async(self) -> ims_20190815_models.GetUserSsoSettingsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_user_sso_settings_with_options_async(runtime)
 
+    def get_verification_info_with_options(
+        self,
+        request: ims_20190815_models.GetVerificationInfoRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ims_20190815_models.GetVerificationInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.user_principal_name):
+            query['UserPrincipalName'] = request.user_principal_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetVerificationInfo',
+            version='2019-08-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ims_20190815_models.GetVerificationInfoResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_verification_info_with_options_async(
+        self,
+        request: ims_20190815_models.GetVerificationInfoRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ims_20190815_models.GetVerificationInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.user_principal_name):
+            query['UserPrincipalName'] = request.user_principal_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetVerificationInfo',
+            version='2019-08-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ims_20190815_models.GetVerificationInfoResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_verification_info(
+        self,
+        request: ims_20190815_models.GetVerificationInfoRequest,
+    ) -> ims_20190815_models.GetVerificationInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_verification_info_with_options(request, runtime)
+
+    async def get_verification_info_async(
+        self,
+        request: ims_20190815_models.GetVerificationInfoRequest,
+    ) -> ims_20190815_models.GetVerificationInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_verification_info_with_options_async(request, runtime)
+
     def list_access_keys_with_options(
         self,
         request: ims_20190815_models.ListAccessKeysRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ims_20190815_models.ListAccessKeysResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_ims20190815-3.0.4/alibabacloud_ims20190815/models.py` & `alibabacloud_ims20190815-3.1.0/alibabacloud_ims20190815/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def __init__(
         self,
         client_id: str = None,
         oidcprovider_name: str = None,
     ):
         # The client ID that you want to add.
         # 
-        # ````
+        # The client ID can contain letters, digits, and special characters and cannot start with the special characters. The special characters are periods (.), hyphens (-), underscores (_), colons (:), and forward slashes (/). 
         # 
         # The client ID can be up to 64 characters in length.
         self.client_id = client_id
         # The name of the OIDC IdP.
         self.oidcprovider_name = oidcprovider_name
 
     def validate(self):
@@ -186,17 +186,14 @@
         body: AddClientIdToOIDCProviderResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -404,17 +401,14 @@
         body: AddFingerprintToOIDCProviderResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -511,17 +505,14 @@
         body: AddUserToGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -638,17 +629,14 @@
         body: BindMFADeviceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -747,17 +735,14 @@
         body: ChangePasswordResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -910,17 +895,14 @@
         body: CreateAccessKeyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1068,17 +1050,14 @@
         body: CreateAppSecretResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1120,15 +1099,15 @@
     ):
         # The validity period of the access token.
         # 
         # Valid values: 900 to 10800. Unit: seconds.
         # 
         # Default value: 3600.
         self.access_token_validity = access_token_validity
-        # The name of the application.
+        # The application name.
         # 
         # The name can be up to 64 characters in length. The name can contain letters, digits, periods (.), underscores (\_), and hyphens (-).
         self.app_name = app_name
         # The type of the application. Valid values:
         # 
         # *   WebApp: a web application that interacts with a browser.
         # *   NativeApp: a native application that runs on an operating system, such as a desktop operating system or a mobile operating system.
@@ -1158,14 +1137,21 @@
         # Valid values: 7200 to 31536000. Unit: seconds.
         # 
         # Default value:
         # 
         # *   For applications of the WebApp and ServerApp types, if this parameter is left empty, the value 2592000 is used. The value 2592000 indicates that the validity period of the refreshed token is 30 days.
         # *   For applications of the NativeApp type, if this parameter is left empty, the value 7776000 is used. The value 7776000 indicates that the validity period of the refreshed token is 90 days.
         self.refresh_token_validity = refresh_token_validity
+        # The required permission.
+        # 
+        # You can specify one or more permissions for the `RequiredScopes` parameter. After you specify this parameter, the required permissions are automatically selected and cannot be revoked when a user grants permissions on the application.
+        # 
+        # If you enter multiple permissions, separate them with semicolons (;).
+        # 
+        # >  If the permission that you specify for the `RequiredScopes` parameter is not included in value of the `PredefinedScopes` parameter, the permission does not take effect.
         self.required_scopes = required_scopes
         # Indicates whether a secret is required. Valid values:
         # 
         # *   true
         # *   false
         # 
         # >- For applications of the WebApp and ServerApp types, this parameter is automatically set to true and cannot be changed.
@@ -1231,18 +1217,24 @@
 class CreateApplicationResponseBodyApplicationDelegatedScopePredefinedScopesPredefinedScope(TeaModel):
     def __init__(
         self,
         description: str = None,
         name: str = None,
         required: bool = None,
     ):
-        # The description of the permission scope.
+        # The description of the permission.
         self.description = description
-        # The name of the scope.
+        # The name of the permission.
         self.name = name
+        # Indicates whether the permission is automatically selected by default when you install the application. Valid values:
+        # 
+        # *   true
+        # *   false
+        # 
+        # `openid` is required by default.
         self.required = required
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1305,15 +1297,15 @@
 
 
 class CreateApplicationResponseBodyApplicationDelegatedScope(TeaModel):
     def __init__(
         self,
         predefined_scopes: CreateApplicationResponseBodyApplicationDelegatedScopePredefinedScopes = None,
     ):
-        # The information of application permissions.
+        # The information about the permissions that are granted on the application.
         self.predefined_scopes = predefined_scopes
 
     def validate(self):
         if self.predefined_scopes:
             self.predefined_scopes.validate()
 
     def to_map(self):
@@ -1380,29 +1372,29 @@
     ):
         # The validity period of the access token. Unit: seconds.
         self.access_token_validity = access_token_validity
         # The ID of the Alibaba Cloud account to which the application belongs.
         self.account_id = account_id
         # The ID of the application.
         self.app_id = app_id
-        # The name of the application.
+        # The application name.
         self.app_name = app_name
-        # The type of the application.
+        # The application type.
         self.app_type = app_type
         # The creation time.
         self.create_date = create_date
-        # The information of application permissions.
+        # The information about the permissions that are granted on the application.
         self.delegated_scope = delegated_scope
         # The display name of the application.
         self.display_name = display_name
         # Indicates whether the application can be installed by using other Alibaba Cloud accounts.
         self.is_multi_tenant = is_multi_tenant
-        # The callback URL.
+        # The callback URLs.
         self.redirect_uris = redirect_uris
-        # The validity period of the refreshed token. Unit: seconds.
+        # The validity period of the refresh token. Unit: seconds.
         self.refresh_token_validity = refresh_token_validity
         # Indicates whether a secret is required.
         self.secret_required = secret_required
         # The update time.
         self.update_date = update_date
 
     def validate(self):
@@ -1480,17 +1472,17 @@
 
 class CreateApplicationResponseBody(TeaModel):
     def __init__(
         self,
         application: CreateApplicationResponseBodyApplication = None,
         request_id: str = None,
     ):
-        # The information of the application.
+        # The information about the application.
         self.application = application
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.application:
             self.application.validate()
 
     def to_map(self):
@@ -1523,17 +1515,14 @@
         body: CreateApplicationResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1715,17 +1704,14 @@
         body: CreateGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1919,17 +1905,14 @@
         body: CreateLoginProfileResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2179,17 +2162,14 @@
         body: CreateOIDCProviderResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2362,17 +2342,14 @@
         body: CreateSAMLProviderResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2747,17 +2724,14 @@
         body: CreateUserResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2900,17 +2874,14 @@
         body: CreateVirtualMFADeviceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3009,17 +2980,14 @@
         body: DeleteAccessKeyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3116,17 +3084,14 @@
         body: DeleteAppSecretResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3216,17 +3181,14 @@
         body: DeleteApplicationResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3316,17 +3278,14 @@
         body: DeleteGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3416,17 +3375,14 @@
         body: DeleteLoginProfileResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3516,17 +3472,14 @@
         body: DeleteOIDCProviderResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3616,17 +3569,14 @@
         body: DeleteSAMLProviderResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3727,17 +3677,14 @@
         body: DeleteUserResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3827,17 +3774,14 @@
         body: DeleteVirtualMFADeviceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3927,17 +3871,14 @@
         body: DisableVirtualMFAResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4010,17 +3951,14 @@
         body: GenerateCredentialReportResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4163,17 +4101,14 @@
         body: GetAccessKeyLastUsedResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4245,17 +4180,14 @@
         body: GetAccountMFAInfoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4454,17 +4386,14 @@
         body: GetAccountSecurityPracticeReportResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4703,17 +4632,14 @@
         body: GetAccountSummaryResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4868,17 +4794,14 @@
         body: GetAppSecretResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4939,14 +4862,20 @@
         name: str = None,
         required: bool = None,
     ):
         # The description of the permission.
         self.description = description
         # The name of the permission.
         self.name = name
+        # Indicates whether the permission is automatically selected by default when you install the application. Valid values:
+        # 
+        # *   true
+        # *   false
+        # 
+        # `openid` is required by default.
         self.required = required
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5188,15 +5117,15 @@
 
 class GetApplicationResponseBody(TeaModel):
     def __init__(
         self,
         application: GetApplicationResponseBodyApplication = None,
         request_id: str = None,
     ):
-        # The configuration information about the application.
+        # The information about the application.
         self.application = application
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.application:
             self.application.validate()
@@ -5231,17 +5160,14 @@
         body: GetApplicationResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5373,17 +5299,14 @@
         body: GetCredentialReportResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5452,17 +5375,14 @@
         body: GetDefaultDomainResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5624,17 +5544,14 @@
         body: GetGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5796,17 +5713,14 @@
         body: GetLoginProfileResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6003,17 +5917,14 @@
         body: GetOIDCProviderResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6182,17 +6093,14 @@
         body: GetPasswordPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6354,17 +6262,14 @@
         body: GetSAMLProviderResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6702,17 +6607,14 @@
         body: GetSecurityPreferenceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7013,17 +6915,14 @@
         body: GetUserResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7173,17 +7072,14 @@
         body: GetUserMFAInfoResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7296,17 +7192,14 @@
         body: GetUserSsoSettingsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7328,14 +7221,198 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetUserSsoSettingsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetVerificationInfoRequest(TeaModel):
+    def __init__(
+        self,
+        user_principal_name: str = None,
+    ):
+        self.user_principal_name = user_principal_name
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
+        if self.user_principal_name is not None:
+            result['UserPrincipalName'] = self.user_principal_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('UserPrincipalName') is not None:
+            self.user_principal_name = m.get('UserPrincipalName')
+        return self
+
+
+class GetVerificationInfoResponseBodySecurityEmailDevice(TeaModel):
+    def __init__(
+        self,
+        email: str = None,
+        status: str = None,
+    ):
+        self.email = email
+        self.status = status
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
+        if self.email is not None:
+            result['Email'] = self.email
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Email') is not None:
+            self.email = m.get('Email')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class GetVerificationInfoResponseBodySecurityPhoneDevice(TeaModel):
+    def __init__(
+        self,
+        area_code: str = None,
+        phone_number: str = None,
+        status: str = None,
+    ):
+        self.area_code = area_code
+        self.phone_number = phone_number
+        self.status = status
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
+        if self.area_code is not None:
+            result['AreaCode'] = self.area_code
+        if self.phone_number is not None:
+            result['PhoneNumber'] = self.phone_number
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AreaCode') is not None:
+            self.area_code = m.get('AreaCode')
+        if m.get('PhoneNumber') is not None:
+            self.phone_number = m.get('PhoneNumber')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class GetVerificationInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        security_email_device: GetVerificationInfoResponseBodySecurityEmailDevice = None,
+        security_phone_device: GetVerificationInfoResponseBodySecurityPhoneDevice = None,
+    ):
+        self.request_id = request_id
+        self.security_email_device = security_email_device
+        self.security_phone_device = security_phone_device
+
+    def validate(self):
+        if self.security_email_device:
+            self.security_email_device.validate()
+        if self.security_phone_device:
+            self.security_phone_device.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.security_email_device is not None:
+            result['SecurityEmailDevice'] = self.security_email_device.to_map()
+        if self.security_phone_device is not None:
+            result['SecurityPhoneDevice'] = self.security_phone_device.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('SecurityEmailDevice') is not None:
+            temp_model = GetVerificationInfoResponseBodySecurityEmailDevice()
+            self.security_email_device = temp_model.from_map(m['SecurityEmailDevice'])
+        if m.get('SecurityPhoneDevice') is not None:
+            temp_model = GetVerificationInfoResponseBodySecurityPhoneDevice()
+            self.security_phone_device = temp_model.from_map(m['SecurityPhoneDevice'])
+        return self
+
+
+class GetVerificationInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetVerificationInfoResponseBody = None,
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
+            temp_model = GetVerificationInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListAccessKeysRequest(TeaModel):
     def __init__(
         self,
         user_principal_name: str = None,
     ):
         # The logon name of the RAM user.
         # 
@@ -7494,17 +7571,14 @@
         body: ListAccessKeysResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7680,17 +7754,14 @@
         body: ListAppSecretIdsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7723,14 +7794,20 @@
         name: str = None,
         required: bool = None,
     ):
         # The description of the permission.
         self.description = description
         # The name of the permission.
         self.name = name
+        # Indicates whether the permission is automatically selected by default when you install the application. Valid values:
+        # 
+        # *   true
+        # *   false
+        # 
+        # `openid` is required by default.
         self.required = required
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7793,15 +7870,15 @@
 
 
 class ListApplicationsResponseBodyApplicationsApplicationDelegatedScope(TeaModel):
     def __init__(
         self,
         predefined_scopes: ListApplicationsResponseBodyApplicationsApplicationDelegatedScopePredefinedScopes = None,
     ):
-        # An array consisting of the information about the permissions that are granted on the application.
+        # The information about the permissions that are granted on the application.
         self.predefined_scopes = predefined_scopes
 
     def validate(self):
         if self.predefined_scopes:
             self.predefined_scopes.validate()
 
     def to_map(self):
@@ -7868,31 +7945,31 @@
     ):
         # The validity period of the access token. Unit: seconds.
         self.access_token_validity = access_token_validity
         # The ID of the Alibaba Cloud account to which the application belongs.
         self.account_id = account_id
         # The ID of the application.
         self.app_id = app_id
-        # The name of the application.
+        # The application name.
         self.app_name = app_name
-        # The type of the application. Valid values:
+        # The application type. Valid values:
         # 
         # *   WebApp: a web application.
         # *   NativeApp: a native application that runs on an operating system, such as a desktop or mobile operating system.
         # *   ServerApp: an application that can access Alibaba Cloud services without the need for user logon. Only applications that synchronize user information based on the System for Cross-domain Identity Management (SCIM) protocol are supported.
         self.app_type = app_type
         # The creation time.
         self.create_date = create_date
         # The information about the permissions that are granted on the application.
         self.delegated_scope = delegated_scope
         # The display name of the application.
         self.display_name = display_name
         # Indicates whether the application can be installed by using other Alibaba Cloud accounts.
         self.is_multi_tenant = is_multi_tenant
-        # The callback URL.
+        # The callback URLs.
         self.redirect_uris = redirect_uris
         # The validity period of the refresh token. Unit: seconds.
         self.refresh_token_validity = refresh_token_validity
         # Indicates whether a secret is required.
         self.secret_required = secret_required
         # The update time.
         self.update_date = update_date
@@ -8050,17 +8127,14 @@
         body: ListApplicationsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -8283,17 +8357,14 @@
         body: ListGroupsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -8483,17 +8554,14 @@
         body: ListGroupsForUserResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -8751,17 +8819,14 @@
         body: ListOIDCProvidersResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -8936,17 +9001,14 @@
         body: ListPredefinedScopesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9162,17 +9224,14 @@
         body: ListSAMLProvidersResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9468,17 +9527,14 @@
         body: ListTagResourcesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -9734,17 +9790,14 @@
         body: ListUserBasicInfosResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -10136,17 +10189,14 @@
         body: ListUsersResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -10362,17 +10412,14 @@
         body: ListUsersForGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -10618,17 +10665,14 @@
         body: ListVirtualMFADevicesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -10836,17 +10880,14 @@
         body: RemoveClientIdFromOIDCProviderResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -11050,17 +11091,14 @@
         body: RemoveFingerprintFromOIDCProviderResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -11157,17 +11195,14 @@
         body: RemoveUserFromGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -11270,17 +11305,14 @@
         body: SetDefaultDomainResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -11583,17 +11615,14 @@
         body: SetPasswordPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -12157,17 +12186,14 @@
         body: SetSecurityPreferenceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -12327,17 +12353,14 @@
         body: SetUserSsoSettingsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -12505,17 +12528,14 @@
         body: TagResourcesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -12642,17 +12662,14 @@
         body: UnbindMFADeviceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -12787,17 +12804,14 @@
         body: UntagResourcesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -12906,17 +12920,14 @@
         body: UpdateAccessKeyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -12953,41 +12964,52 @@
         new_redirect_uris: str = None,
         new_refresh_token_validity: int = None,
         new_required_scopes: str = None,
         new_secret_required: bool = None,
     ):
         # The ID of the application.
         self.app_id = app_id
-        # The validity period of the new access token.
+        # The validity period of the access token.
         # 
         # Valid values: 900 to 10800. Unit: seconds.
         self.new_access_token_validity = new_access_token_validity
-        # The new display name of the application.
+        # The display name.
         self.new_display_name = new_display_name
         # Specifies whether the application can be installed by using other Alibaba Cloud accounts. Valid values:
         # 
         # *   true
         # *   false
         self.new_is_multi_tenant = new_is_multi_tenant
-        # The new scope of application permissions.
+        # The permission that is granted on the application.
         # 
-        # For more information about the application permission scope, see [Open authorization scope](~~93693~~). You can also call the [ListPredefinedScopes](~~187206~~) operation to obtain the permission scopes supported by different types of applications.
+        # For more information about the application permission scope, see [OAuth scopes](~~93693~~). You can also call the [ListPredefinedScopes](~~187206~~) operation to query the permissions that are supported by different types of applications.
         # 
-        # Separate multiple permission scopes with semicolons (;).
+        # If you enter multiple permissions, separate them with semicolons (;).
         # 
-        # If you specify a new permission scope, the new permission scope takes effect. For example, if the original permission scope is `/acs/ccc`, and the new permission scope is `/acs/alidns`, `/acs/alidns` takes effect. If you want to retain the original permission scope, set the new permission scope to `/acs/ccc;/acs/alidns`.
+        # The new value of this parameter overwrites the original value, and the permission specified by the new value takes effect. For example, if the original value is `/acs/ccc`, and the new value is `/acs/alidns`, `/acs/alidns` takes effect. If you want to retain the original permission and the `/acs/alidns` permission, set the value to `/acs/ccc;/acs/alidns`.
         self.new_predefined_scopes = new_predefined_scopes
-        # The new callback URL.
+        # The callback URL.
         # 
-        # Separate multiple callback URLs with semicolons (;).
+        # If you enter multiple callback URLs, separate them with semicolons (;).
         self.new_redirect_uris = new_redirect_uris
-        # The validity period of the refreshed token.
+        # The validity period of the refresh token.
         # 
         # Valid values: 7200 to 31536000. Unit: seconds.
         self.new_refresh_token_validity = new_refresh_token_validity
+        # The required permission.
+        # 
+        # You can specify one or more permissions for the `RequiredScopes` parameter. After you specify this parameter, the required permissions are automatically selected and cannot be revoked when a user grants permissions on the application.
+        # 
+        # If you also specify the `NewPredefinedScopes` parameter, the `NewPredefinedScopes` parameter specifies the permissions that can be granted on the application, and this parameter specifies the required permissions.
+        # 
+        # If you enter multiple permissions, separate them with semicolons (;).
+        # 
+        # The new value of this parameter overwrites the original value, and the required permission specified by the new value takes effect.
+        # 
+        # >  If the permission that you specify for the `RequiredScopes` parameter is not included in value of the `PredefinedScopes` parameter, the permission does not take effect.
         self.new_required_scopes = new_required_scopes
         # Specifies whether a secret is required. Valid values:
         # 
         # *   true
         # *   false
         # 
         # > 
@@ -13051,18 +13073,24 @@
 class UpdateApplicationResponseBodyApplicationDelegatedScopePredefinedScopesPredefinedScope(TeaModel):
     def __init__(
         self,
         description: str = None,
         name: str = None,
         required: bool = None,
     ):
-        # The description of the permission scope.
+        # The description of the permission.
         self.description = description
-        # The name of the scope.
+        # The name of the permission.
         self.name = name
+        # Indicates whether the permission is automatically selected by default when you install the application. Valid values:
+        # 
+        # *   true
+        # *   false
+        # 
+        # `openid` is required by default.
         self.required = required
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13125,15 +13153,15 @@
 
 
 class UpdateApplicationResponseBodyApplicationDelegatedScope(TeaModel):
     def __init__(
         self,
         predefined_scopes: UpdateApplicationResponseBodyApplicationDelegatedScopePredefinedScopes = None,
     ):
-        # The information of application permissions.
+        # The information about the permissions that are granted on the application.
         self.predefined_scopes = predefined_scopes
 
     def validate(self):
         if self.predefined_scopes:
             self.predefined_scopes.validate()
 
     def to_map(self):
@@ -13200,29 +13228,29 @@
     ):
         # The validity period of the access token. Unit: seconds.
         self.access_token_validity = access_token_validity
         # The ID of the Alibaba Cloud account to which the application belongs.
         self.account_id = account_id
         # The ID of the application.
         self.app_id = app_id
-        # The name of the application.
+        # The application name.
         self.app_name = app_name
-        # The type of the application.
+        # The application type.
         self.app_type = app_type
         # The creation time.
         self.create_date = create_date
-        # The information of application permissions.
+        # The information about the permissions that are granted on the application.
         self.delegated_scope = delegated_scope
         # The display name of the application.
         self.display_name = display_name
         # Indicates whether the application can be installed by using other Alibaba Cloud accounts.
         self.is_multi_tenant = is_multi_tenant
-        # The callback URL.
+        # The callback URLs.
         self.redirect_uris = redirect_uris
-        # The validity period of the refreshed token. Unit: seconds.
+        # The validity period of the refresh token. Unit: seconds.
         self.refresh_token_validity = refresh_token_validity
         # Indicates whether a secret is required.
         self.secret_required = secret_required
         # The update time.
         self.update_date = update_date
 
     def validate(self):
@@ -13300,17 +13328,17 @@
 
 class UpdateApplicationResponseBody(TeaModel):
     def __init__(
         self,
         application: UpdateApplicationResponseBodyApplication = None,
         request_id: str = None,
     ):
-        # The information of the application.
+        # The information about the application.
         self.application = application
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.application:
             self.application.validate()
 
     def to_map(self):
@@ -13343,17 +13371,14 @@
         body: UpdateApplicationResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -13542,17 +13567,14 @@
         body: UpdateGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -13746,17 +13768,14 @@
         body: UpdateLoginProfileResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -13982,17 +14001,14 @@
         body: UpdateOIDCProviderResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -14165,17 +14181,14 @@
         body: UpdateSAMLProviderResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -14433,17 +14446,14 @@
         body: UpdateUserResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_ims20190815-3.0.4/alibabacloud_ims20190815.egg-info/PKG-INFO` & `alibabacloud_ims20190815-3.1.0/alibabacloud_ims20190815.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ims20190815
-Version: 3.0.4
+Version: 3.1.0
 Summary: Alibaba Cloud Ims (20190815) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/ims-20190815/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_ims20190815-3.0.4/setup.py` & `alibabacloud_ims20190815-3.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ims20190815.
 
-Created on 14/12/2023
+Created on 07/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ims20190815"
 NAME = "alibabacloud_ims20190815" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Ims (20190815) SDK Library for Python"
```

