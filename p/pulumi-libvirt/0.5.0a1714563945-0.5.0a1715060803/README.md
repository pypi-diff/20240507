# Comparing `tmp/pulumi_libvirt-0.5.0a1714563945.tar.gz` & `tmp/pulumi_libvirt-0.5.0a1715060803.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_libvirt-0.5.0a1714563945.tar", last modified: Wed May  1 11:51:26 2024, max compression
+gzip compressed data, was "pulumi_libvirt-0.5.0a1715060803.tar", last modified: Tue May  7 05:53:46 2024, max compression
```

## Comparing `pulumi_libvirt-0.5.0a1714563945.tar` & `pulumi_libvirt-0.5.0a1715060803.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:51:26.228586 pulumi_libvirt-0.5.0a1714563945/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-01 11:51:26.228586 pulumi_libvirt-0.5.0a1714563945/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:51:26.228586 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42947 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/cloud_init_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:51:26.228586 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    70503 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/get_network_dns_host_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/get_network_dns_srv_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/get_network_dnsmasq_options_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/ignition.py
--rw-r--r--   0 runner    (1001) docker     (127)    31821 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    36652 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:51:26.228586 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-01 11:51:26.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-01 11:51:26.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:51:26.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 11:51:26.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 11:51:26.000000 pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-01 11:51:19.000000 pulumi_libvirt-0.5.0a1714563945/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 11:51:26.228586 pulumi_libvirt-0.5.0a1714563945/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:53:46.541269 pulumi_libvirt-0.5.0a1715060803/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-07 05:53:46.541269 pulumi_libvirt-0.5.0a1715060803/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:53:46.537269 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42947 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/cloud_init_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:53:46.541269 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70503 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/get_network_dns_host_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/get_network_dns_srv_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/get_network_dnsmasq_options_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/ignition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31821 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36652 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:53:46.541269 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-07 05:53:46.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-07 05:53:46.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 05:53:46.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 05:53:46.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 05:53:46.000000 pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-07 05:53:39.000000 pulumi_libvirt-0.5.0a1715060803/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 05:53:46.541269 pulumi_libvirt-0.5.0a1715060803/setup.cfg
```

### Comparing `pulumi_libvirt-0.5.0a1714563945/PKG-INFO` & `pulumi_libvirt-0.5.0a1715060803/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_libvirt
-Version: 0.5.0a1714563945
+Version: 0.5.0a1715060803
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi,libvirt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_libvirt-0.5.0a1714563945/README.md` & `pulumi_libvirt-0.5.0a1715060803/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/__init__.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/_inputs.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/_utilities.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/cloud_init_disk.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/cloud_init_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/config/vars.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/domain.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/get_network_dns_host_template.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/get_network_dns_host_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/get_network_dns_srv_template.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/get_network_dns_srv_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/get_network_dnsmasq_options_template.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/get_network_dnsmasq_options_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/ignition.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/ignition.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/network.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/outputs.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/pool.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/provider.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt/volume.py` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt.egg-info/PKG-INFO` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_libvirt
-Version: 0.5.0a1714563945
+Version: 0.5.0a1715060803
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi,libvirt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_libvirt-0.5.0a1714563945/pulumi_libvirt.egg-info/SOURCES.txt` & `pulumi_libvirt-0.5.0a1715060803/pulumi_libvirt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.5.0a1714563945/pyproject.toml` & `pulumi_libvirt-0.5.0a1715060803/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_libvirt"
   description = "A Pulumi package for creating and managing libvirt cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "libvirt"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.5.0a1714563945"
+  version = "0.5.0a1715060803"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-libvirt"
 
 [build-system]
```
