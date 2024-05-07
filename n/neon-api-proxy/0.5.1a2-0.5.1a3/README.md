# Comparing `tmp/neon-api-proxy-0.5.1a2.tar.gz` & `tmp/neon-api-proxy-0.5.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-api-proxy-0.5.1a2.tar", last modified: Thu Apr 25 16:29:17 2024, max compression
+gzip compressed data, was "neon-api-proxy-0.5.1a3.tar", last modified: Tue May  7 16:45:55 2024, max compression
```

## Comparing `neon-api-proxy-0.5.1a2.tar` & `neon-api-proxy-0.5.1a3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:17.626588 neon-api-proxy-0.5.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-25 16:29:17.626588 neon-api-proxy-0.5.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:17.622588 neon-api-proxy-0.5.1a2/neon_api_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/alpha_vantage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/api_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/cached_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:17.622588 neon-api-proxy-0.5.1a2/neon_api_proxy/client/
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/client/alpha_vantage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/client/financial_modeling_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/client/map_maker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/client/open_weather_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/client/wolfram_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/owm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:17.626588 neon-api-proxy-0.5.1a2/neon_api_proxy/services/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/services/alpha_vantage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/services/map_maker_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/services/owm_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/services/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/services/wolfram_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/socket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/neon_api_proxy/wolfram_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:17.622588 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:29:17.000000 neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:29:17.626588 neon-api-proxy-0.5.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-25 16:29:13.000000 neon-api-proxy-0.5.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:45:55.158191 neon-api-proxy-0.5.1a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-07 16:45:55.158191 neon-api-proxy-0.5.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:45:55.154191 neon-api-proxy-0.5.1a3/neon_api_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/alpha_vantage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/api_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/cached_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:45:55.158191 neon-api-proxy-0.5.1a3/neon_api_proxy/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/client/alpha_vantage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/client/financial_modeling_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/client/map_maker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/client/open_weather_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/client/wolfram_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/owm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:45:55.158191 neon-api-proxy-0.5.1a3/neon_api_proxy/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/services/alpha_vantage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/services/map_maker_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/services/owm_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/services/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/services/wolfram_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/socket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/neon_api_proxy/wolfram_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:45:55.158191 neon-api-proxy-0.5.1a3/neon_api_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-07 16:45:55.000000 neon-api-proxy-0.5.1a3/neon_api_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-07 16:45:55.000000 neon-api-proxy-0.5.1a3/neon_api_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:45:55.000000 neon-api-proxy-0.5.1a3/neon_api_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 16:45:55.000000 neon-api-proxy-0.5.1a3/neon_api_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 16:45:55.000000 neon-api-proxy-0.5.1a3/neon_api_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 16:45:55.000000 neon-api-proxy-0.5.1a3/neon_api_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:45:55.000000 neon-api-proxy-0.5.1a3/neon_api_proxy.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:45:55.158191 neon-api-proxy-0.5.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-07 16:45:49.000000 neon-api-proxy-0.5.1a3/setup.py
```

### Comparing `neon-api-proxy-0.5.1a2/LICENSE.md` & `neon-api-proxy-0.5.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/PKG-INFO` & `neon-api-proxy-0.5.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-api-proxy
-Version: 0.5.1a2
+Version: 0.5.1a3
 Summary: Neon Proxy for external API Calls
 Home-page: https://github.com/NeonGeckoCom/neon_api_proxy
 Author: Neongecko
 Author-email: developers@neon.ai
 License: NeonAI License v1.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon-api-proxy-0.5.1a2/README.md` & `neon-api-proxy-0.5.1a3/README.md`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/__init__.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/__main__.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/alpha_vantage_api.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/alpha_vantage_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/api_connector.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/api_connector.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/cached_api.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/cached_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/client/__init__.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/client/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/client/alpha_vantage.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/client/alpha_vantage.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/client/financial_modeling_prep.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/client/financial_modeling_prep.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/client/map_maker.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/client/map_maker.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/client/open_weather_map.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/client/open_weather_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,11 +100,14 @@
     resp = request_api(NeonAPI.OPEN_WEATHER_MAP, query_params)
 
     try:
         data = json.loads(resp["content"])
     except JSONDecodeError:
         data = {"error": "Error decoding response",
                 "response": resp}
+    if data.get('cod') == "400":
+        # Backwards-compat. Put error response under `error` key
+        data["error"] = data.get("message")
     if data.get('cod'):
         data['cod'] = str(data['cod'])
         # TODO: Handle failures
     return data
```

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/client/wolfram_alpha.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/client/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/config.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/config.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/controller.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,16 +85,17 @@
                 and instance of python class representing it
         """
         service_mapping = dict()
         for item in service_class_mapping:
             api_key = self.config.get(item, {}).get("api_key") if self.config \
                 else None
             try:
-                if api_key is None:
-                    LOG.warning(f"No API key for {item} in {self.config}")
+                if api_key is None and item != 'api_test_endpoint':
+                    LOG.warning(f"No API key for {item} in "
+                                f"{list(self.config.keys())}")
                 service_mapping[item] = \
                     service_class_mapping[item](api_key=api_key)
             except Exception as e:
                 LOG.error(e)
         return service_mapping
 
     def resolve_query(self, query: dict) -> dict:
```

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/owm_api.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/owm_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/services/__init__.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/services/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/services/alpha_vantage_api.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/services/alpha_vantage_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/services/map_maker_api.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/services/map_maker_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/services/owm_api.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/services/owm_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import urllib.parse
 from datetime import timedelta
 
 from requests import Response
 
 from neon_api_proxy.cached_api import CachedAPI
-from ovos_utils.log import LOG
+from ovos_utils.log import LOG, log_deprecation
 from neon_utils.authentication_utils import find_neon_owm_key
 
 
 class OpenWeatherAPI(CachedAPI):
     """
     API for querying Open Weather Map.
     """
@@ -70,27 +70,35 @@
         try:
             resp = self._get_api_response(lat, lng, units, api, lang)
         except Exception as e:
             return {"status_code": -1,
                     "content": repr(e),
                     "encoding": None}
         if not resp.ok:
-            LOG.error(f"Bad response code: {resp.status_code}")
+            LOG.error(f"Bad response code: {resp.status_code}: "
+                      f"content={resp.content}")
         return {"status_code": resp.status_code,
                 "content": resp.content,
                 "encoding": resp.encoding}
 
     def _get_api_response(self, lat: str, lng: str, units: str,
                           api: str = "onecall", lang: str = "en") -> Response:
-        str(float(lat))
-        str(float(lng))
+        try:
+            assert isinstance(float(lat), float), f"Invalid latitude: {lat}"
+            assert isinstance(float(lng), float), f"Invalid longitude: {lng}"
+        except AssertionError as e:
+            raise ValueError(e)
+        if api != "onecall":
+            log_deprecation(f"{api} was requested but only `onecall` "
+                            f"is supported", "1.0.0")
+            api = "onecall"
         assert units in ("metric", "imperial", "standard")
         query_params = {"lat": lat,
                         "lon": lng,
                         "appid": self._api_key,
                         "units": units,
                         "lang": lang}
         query_str = urllib.parse.urlencode(query_params)
-        base_url = "http://api.openweathermap.org/data/2.5"
+        base_url = "http://api.openweathermap.org/data/3.0"
         resp = self.get_with_cache_timeout(f"{base_url}/{api}?{query_str}",
                                            self.cache_timeout)
         return resp
```

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/services/test_api.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/services/test_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/services/wolfram_api.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/services/wolfram_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         :return: URL encoded query string used to build a request URL
         """
         if not kwargs.get("query"):
             raise ValueError(f"No query in request: {kwargs}")
         query_params = dict()
         query_params['i'] = kwargs.get("query")
         query_params['units'] = kwargs.get("units") if \
-            kwargs.get("units") == "metric" else "nonmetric"
+            kwargs.get("units") == "metric" else "imperial"
         lat = kwargs.get("lat")
         lng = kwargs.get("lng")
         if kwargs.get("latlong"):
             query_params["latlong"] = kwargs.get("latlong")
         elif lat and lng:
             query_params["latlong"] = f"{lat},{lng}"
         else:
@@ -152,14 +152,15 @@
         """
         Queries the Wolfram|Alpha API and returns a dict with:
             status, content, and encoding
         :param query: URL to query
         :return: dict response containing:
             `status_code`, `content`, and `encoding`
         """
+        LOG.debug(f"query={query}")
         result = self.get_with_cache_timeout(query, timeout=self.cache_time)
         if not result.ok:
             # 501 = Wolfram couldn't understand
             # 403 = Invalid API Key Provided
             LOG.warning(f"API Query error ({result.status_code}): {query}")
         return {"status_code": result.status_code,
                 "content": result.content,
```

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/socket_handler.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/socket_handler.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/test_api.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/test_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy/wolfram_api.py` & `neon-api-proxy-0.5.1a3/neon_api_proxy/wolfram_api.py`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/PKG-INFO` & `neon-api-proxy-0.5.1a3/neon_api_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-api-proxy
-Version: 0.5.1a2
+Version: 0.5.1a3
 Summary: Neon Proxy for external API Calls
 Home-page: https://github.com/NeonGeckoCom/neon_api_proxy
 Author: Neongecko
 Author-email: developers@neon.ai
 License: NeonAI License v1.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon-api-proxy-0.5.1a2/neon_api_proxy.egg-info/SOURCES.txt` & `neon-api-proxy-0.5.1a3/neon_api_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-api-proxy-0.5.1a2/setup.py` & `neon-api-proxy-0.5.1a3/setup.py`

 * *Files identical despite different names*

