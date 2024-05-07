# Comparing `tmp/netbox-gateways-0.4.3.tar.gz` & `tmp/netbox_gateways-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-gateways-0.4.3.tar", last modified: Mon Apr 25 09:23:40 2022, max compression
+gzip compressed data, was "netbox_gateways-0.5.0.tar", last modified: Tue May  7 11:22:25 2024, max compression
```

## Comparing `netbox-gateways-0.4.3.tar` & `netbox_gateways-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2022-04-25 09:23:40.397646 netbox-gateways-0.4.3/
--rw-r--r--   0 jamie.murphy   (501) staff       (20)       58 2022-04-11 09:01:47.000000 netbox-gateways-0.4.3/MANIFEST.in
--rw-r--r--   0 jamie.murphy   (501) staff       (20)     2144 2022-04-25 09:18:18.000000 netbox-gateways-0.4.3/Makefile
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      151 2022-04-25 09:23:40.397492 netbox-gateways-0.4.3/PKG-INFO
--rw-r--r--   0 jamie.murphy   (501) staff       (20)     1007 2022-04-25 09:18:18.000000 netbox-gateways-0.4.3/README.md
-drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2022-04-25 09:23:40.360959 netbox-gateways-0.4.3/netbox_gateways/
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      289 2022-04-25 09:22:36.000000 netbox-gateways-0.4.3/netbox_gateways/__init__.py
-drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2022-04-25 09:23:40.395938 netbox-gateways-0.4.3/netbox_gateways/api/
--rw-r--r--   0 jamie.murphy   (501) staff       (20)        0 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/api/__init__.py
--rw-r--r--   0 jamie.murphy   (501) staff       (20)     1155 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/api/serializers.py
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      195 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/api/urls.py
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      371 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/api/views.py
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      449 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/filtersets.py
--rw-r--r--   0 jamie.murphy   (501) staff       (20)     1189 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/forms.py
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      455 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/graphql.py
-drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2022-04-25 09:23:40.396538 netbox-gateways-0.4.3/netbox_gateways/migrations/
--rw-r--r--   0 jamie.murphy   (501) staff       (20)     1564 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/migrations/0001_netbox_gateways.py
--rw-r--r--   0 jamie.murphy   (501) staff       (20)        0 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/migrations/__init__.py
--rw-r--r--   0 jamie.murphy   (501) staff       (20)     1101 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/models.py
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      588 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/navigation.py
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      489 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/tables.py
--rw-r--r--   0 jamie.murphy   (501) staff       (20)     3140 2022-04-25 09:18:18.000000 netbox-gateways-0.4.3/netbox_gateways/template_content.py
-drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2022-04-25 09:23:40.356716 netbox-gateways-0.4.3/netbox_gateways/templates/
-drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2022-04-25 09:23:40.397280 netbox-gateways-0.4.3/netbox_gateways/templates/netbox_gateways/
--rw-r--r--   0 jamie.murphy   (501) staff       (20)     1310 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/templates/netbox_gateways/gateway.html
--rw-r--r--   0 jamie.murphy   (501) staff       (20)     1451 2022-04-25 09:18:18.000000 netbox-gateways-0.4.3/netbox_gateways/templates/netbox_gateways/ip_card.html
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      960 2022-04-25 09:18:18.000000 netbox-gateways-0.4.3/netbox_gateways/templates/netbox_gateways/prefix_card.html
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      776 2022-04-25 09:16:30.000000 netbox-gateways-0.4.3/netbox_gateways/urls.py
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      890 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/netbox_gateways/views.py
-drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2022-04-25 09:23:40.394598 netbox-gateways-0.4.3/netbox_gateways.egg-info/
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      151 2022-04-25 09:23:40.000000 netbox-gateways-0.4.3/netbox_gateways.egg-info/PKG-INFO
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      908 2022-04-25 09:23:40.000000 netbox-gateways-0.4.3/netbox_gateways.egg-info/SOURCES.txt
--rw-r--r--   0 jamie.murphy   (501) staff       (20)        1 2022-04-25 09:23:40.000000 netbox-gateways-0.4.3/netbox_gateways.egg-info/dependency_links.txt
--rw-r--r--   0 jamie.murphy   (501) staff       (20)        1 2022-04-11 08:35:28.000000 netbox-gateways-0.4.3/netbox_gateways.egg-info/not-zip-safe
--rw-r--r--   0 jamie.murphy   (501) staff       (20)       16 2022-04-25 09:23:40.000000 netbox-gateways-0.4.3/netbox_gateways.egg-info/top_level.txt
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      101 2022-04-11 08:34:41.000000 netbox-gateways-0.4.3/pyproject.toml
--rw-r--r--   0 jamie.murphy   (501) staff       (20)       38 2022-04-25 09:23:40.397699 netbox-gateways-0.4.3/setup.cfg
--rw-r--r--   0 jamie.murphy   (501) staff       (20)      266 2022-04-25 09:22:45.000000 netbox-gateways-0.4.3/setup.py
+drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2024-05-07 11:22:25.894402 netbox_gateways-0.5.0/
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)       58 2022-04-11 09:01:47.000000 netbox_gateways-0.5.0/MANIFEST.in
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)     2144 2022-04-25 09:18:18.000000 netbox_gateways-0.5.0/Makefile
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      106 2024-05-07 11:22:25.894180 netbox_gateways-0.5.0/PKG-INFO
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)     1045 2024-05-07 10:55:12.000000 netbox_gateways-0.5.0/README.md
+drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2024-05-07 11:22:25.891681 netbox_gateways-0.5.0/netbox_gateways/
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      289 2024-05-07 11:04:34.000000 netbox_gateways-0.5.0/netbox_gateways/__init__.py
+drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2024-05-07 11:22:25.893164 netbox_gateways-0.5.0/netbox_gateways/api/
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)        0 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/netbox_gateways/api/__init__.py
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)     1155 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/netbox_gateways/api/serializers.py
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      195 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/netbox_gateways/api/urls.py
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      371 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/netbox_gateways/api/views.py
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      449 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/netbox_gateways/filtersets.py
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)     1189 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/netbox_gateways/forms.py
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      455 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/netbox_gateways/graphql.py
+drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2024-05-07 11:22:25.893433 netbox_gateways-0.5.0/netbox_gateways/migrations/
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)     1564 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/netbox_gateways/migrations/0001_netbox_gateways.py
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)        0 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/netbox_gateways/migrations/__init__.py
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)     1101 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/netbox_gateways/models.py
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      499 2024-05-07 11:20:55.000000 netbox_gateways-0.5.0/netbox_gateways/navigation.py
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      489 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/netbox_gateways/tables.py
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)     3140 2024-05-07 11:18:08.000000 netbox_gateways-0.5.0/netbox_gateways/template_content.py
+drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2024-05-07 11:22:25.889525 netbox_gateways-0.5.0/netbox_gateways/templates/
+drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2024-05-07 11:22:25.893793 netbox_gateways-0.5.0/netbox_gateways/templates/netbox_gateways/
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)     1310 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/netbox_gateways/templates/netbox_gateways/gateway.html
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)     1451 2022-04-25 09:18:18.000000 netbox_gateways-0.5.0/netbox_gateways/templates/netbox_gateways/ip_card.html
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      960 2022-04-25 09:18:18.000000 netbox_gateways-0.5.0/netbox_gateways/templates/netbox_gateways/prefix_card.html
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      776 2022-04-25 09:16:30.000000 netbox_gateways-0.5.0/netbox_gateways/urls.py
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      890 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/netbox_gateways/views.py
+drwxr-xr-x   0 jamie.murphy   (501) staff       (20)        0 2024-05-07 11:22:25.893970 netbox_gateways-0.5.0/netbox_gateways.egg-info/
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      106 2024-05-07 11:22:25.000000 netbox_gateways-0.5.0/netbox_gateways.egg-info/PKG-INFO
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      908 2024-05-07 11:22:25.000000 netbox_gateways-0.5.0/netbox_gateways.egg-info/SOURCES.txt
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)        1 2024-05-07 11:22:25.000000 netbox_gateways-0.5.0/netbox_gateways.egg-info/dependency_links.txt
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)        1 2022-04-11 08:35:28.000000 netbox_gateways-0.5.0/netbox_gateways.egg-info/not-zip-safe
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)       16 2024-05-07 11:22:25.000000 netbox_gateways-0.5.0/netbox_gateways.egg-info/top_level.txt
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      101 2022-04-11 08:34:41.000000 netbox_gateways-0.5.0/pyproject.toml
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)       38 2024-05-07 11:22:25.894453 netbox_gateways-0.5.0/setup.cfg
+-rw-r--r--   0 jamie.murphy   (501) staff       (20)      266 2024-05-07 11:21:02.000000 netbox_gateways-0.5.0/setup.py
```

### Comparing `netbox-gateways-0.4.3/Makefile` & `netbox_gateways-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `netbox-gateways-0.4.3/README.md` & `netbox_gateways-0.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # NetBox Gateways Plugin
 [Netbox](https://github.com/netbox-community/netbox) plugin  to Manage simple default gateways for prefixes.
 
 ## Compatibility
 
 |      Netbox Version       |   Plugin Version    |
 |---------------------------|-------|
+| NetBox 4.0                | 0.5.0 |
 | NetBox 3.2                | 0.4.2 |
 
 ## Installation
 
 1. The plugin is available as a Python package in pypi and can be installed with pip  
 
 ```
```

### Comparing `netbox-gateways-0.4.3/netbox_gateways/api/serializers.py` & `netbox_gateways-0.5.0/netbox_gateways/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-gateways-0.4.3/netbox_gateways/forms.py` & `netbox_gateways-0.5.0/netbox_gateways/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-gateways-0.4.3/netbox_gateways/migrations/0001_netbox_gateways.py` & `netbox_gateways-0.5.0/netbox_gateways/migrations/0001_netbox_gateways.py`

 * *Files identical despite different names*

### Comparing `netbox-gateways-0.4.3/netbox_gateways/models.py` & `netbox_gateways-0.5.0/netbox_gateways/models.py`

 * *Files identical despite different names*

### Comparing `netbox-gateways-0.4.3/netbox_gateways/template_content.py` & `netbox_gateways-0.5.0/netbox_gateways/template_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from extras.plugins import PluginTemplateExtension
+from netbox.plugins import PluginTemplateExtension
 from ipam.models import Prefix
 from .models import Gateway
 from ipaddress import IPv4Address
 
 
 class IPGatewayTemplate(PluginTemplateExtension):
     model = "ipam.ipaddress"
```

### Comparing `netbox-gateways-0.4.3/netbox_gateways/templates/netbox_gateways/gateway.html` & `netbox_gateways-0.5.0/netbox_gateways/templates/netbox_gateways/gateway.html`

 * *Files identical despite different names*

### Comparing `netbox-gateways-0.4.3/netbox_gateways/templates/netbox_gateways/ip_card.html` & `netbox_gateways-0.5.0/netbox_gateways/templates/netbox_gateways/ip_card.html`

 * *Files identical despite different names*

### Comparing `netbox-gateways-0.4.3/netbox_gateways/templates/netbox_gateways/prefix_card.html` & `netbox_gateways-0.5.0/netbox_gateways/templates/netbox_gateways/prefix_card.html`

 * *Files identical despite different names*

### Comparing `netbox-gateways-0.4.3/netbox_gateways/urls.py` & `netbox_gateways-0.5.0/netbox_gateways/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-gateways-0.4.3/netbox_gateways/views.py` & `netbox_gateways-0.5.0/netbox_gateways/views.py`

 * *Files identical despite different names*

### Comparing `netbox-gateways-0.4.3/netbox_gateways.egg-info/SOURCES.txt` & `netbox_gateways-0.5.0/netbox_gateways.egg-info/SOURCES.txt`

 * *Files identical despite different names*

