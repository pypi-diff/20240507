# Comparing `tmp/netbox_sp_addon-0.9.0.tar.gz` & `tmp/netbox_sp_addon-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_sp_addon-0.9.0.tar", max compression
+gzip compressed data, was "netbox_sp_addon-0.9.1.tar", max compression
```

## Comparing `netbox_sp_addon-0.9.0.tar` & `netbox_sp_addon-0.9.1.tar`

### file list

```diff
@@ -1,17 +1,14 @@
--rw-r--r--   0        0        0    10174 2021-06-10 08:52:45.251404 netbox_sp_addon-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0       18 2024-01-05 07:45:10.462708 netbox_sp_addon-0.9.0/README.md
--rw-r--r--   0        0        0      859 2024-02-23 07:51:57.974018 netbox_sp_addon-0.9.0/netbox_sp_addon/__init__.py
--rw-r--r--   0        0        0       33 2021-06-10 08:52:45.251404 netbox_sp_addon-0.9.0/netbox_sp_addon/admin.py
--rw-r--r--   0        0        0        0 2021-06-10 08:52:45.251404 netbox_sp_addon-0.9.0/netbox_sp_addon/api/serializers.py
--rw-r--r--   0        0        0       96 2021-06-10 08:52:45.251404 netbox_sp_addon-0.9.0/netbox_sp_addon/api/urls.py
--rw-r--r--   0        0        0        0 2021-06-10 08:52:45.251404 netbox_sp_addon-0.9.0/netbox_sp_addon/api/views.py
--rw-r--r--   0        0        0      314 2024-01-05 07:49:32.630149 netbox_sp_addon-0.9.0/netbox_sp_addon/filters.py
--rw-r--r--   0        0        0     1185 2024-01-05 07:51:56.195178 netbox_sp_addon-0.9.0/netbox_sp_addon/forms.py
--rw-r--r--   0        0        0        0 2021-06-10 08:52:45.251404 netbox_sp_addon-0.9.0/netbox_sp_addon/migrations/__init__.py
--rw-r--r--   0        0        0       29 2021-06-10 08:52:45.251404 netbox_sp_addon-0.9.0/netbox_sp_addon/models.py
--rw-r--r--   0        0        0      340 2024-01-05 07:49:32.630149 netbox_sp_addon-0.9.0/netbox_sp_addon/navigation.py
--rw-r--r--   0        0        0      203 2024-01-25 07:31:24.062810 netbox_sp_addon-0.9.0/netbox_sp_addon/template_content.py
--rw-r--r--   0        0        0      292 2021-06-10 08:52:45.251404 netbox_sp_addon-0.9.0/netbox_sp_addon/urls.py
--rw-r--r--   0        0        0      326 2024-01-05 07:49:32.630149 netbox_sp_addon-0.9.0/netbox_sp_addon/views.py
--rw-r--r--   0        0        0      733 2024-01-25 07:51:58.401189 netbox_sp_addon-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 netbox_sp_addon-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    10174 2024-05-07 05:46:15.997722 netbox_sp_addon-0.9.1/LICENSE.txt
+-rw-r--r--   0        0        0       18 2024-05-07 05:46:15.997722 netbox_sp_addon-0.9.1/README.md
+-rw-r--r--   0        0        0      855 2024-05-07 05:46:15.997722 netbox_sp_addon-0.9.1/netbox_sp_addon/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 05:46:15.997722 netbox_sp_addon-0.9.1/netbox_sp_addon/api/serializers.py
+-rw-r--r--   0        0        0       96 2024-05-07 05:46:15.997722 netbox_sp_addon-0.9.1/netbox_sp_addon/api/urls.py
+-rw-r--r--   0        0        0        0 2024-05-07 05:46:15.997722 netbox_sp_addon-0.9.1/netbox_sp_addon/api/views.py
+-rw-r--r--   0        0        0      314 2024-05-07 05:46:15.997722 netbox_sp_addon-0.9.1/netbox_sp_addon/filters.py
+-rw-r--r--   0        0        0     1330 2024-05-07 05:46:15.997722 netbox_sp_addon-0.9.1/netbox_sp_addon/forms.py
+-rw-r--r--   0        0        0        0 2024-05-07 05:46:15.997722 netbox_sp_addon-0.9.1/netbox_sp_addon/migrations/__init__.py
+-rw-r--r--   0        0        0      273 2024-05-07 05:46:15.997722 netbox_sp_addon-0.9.1/netbox_sp_addon/navigation.py
+-rw-r--r--   0        0        0      292 2024-05-07 05:46:15.997722 netbox_sp_addon-0.9.1/netbox_sp_addon/urls.py
+-rw-r--r--   0        0        0      232 2024-05-07 05:46:15.998723 netbox_sp_addon-0.9.1/netbox_sp_addon/views.py
+-rw-r--r--   0        0        0      733 2024-05-07 05:46:15.998723 netbox_sp_addon-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 netbox_sp_addon-0.9.1/PKG-INFO
```

### Comparing `netbox_sp_addon-0.9.0/LICENSE.txt` & `netbox_sp_addon-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `netbox_sp_addon-0.9.0/netbox_sp_addon/__init__.py` & `netbox_sp_addon-0.9.1/netbox_sp_addon/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     name = "netbox_sp_addon"
 
     # Human-friendly name and description
     verbose_name = "qbeyond Addon"
     description = "Add functions used by qbeyond AG"
 
     # Plugin version
-    version = "0.9.0"
+    version = "0.9.1"
 
     # Plugin author
     author = "Tobias Genannt"
     author_email = "tobias.genannt@qbeyond.de"
 
     # Configuration parameters that MUST be defined by the user (if any)
     required_settings = []
@@ -26,11 +26,11 @@
     # Default configuration parameter values, if not set by the user
     default_settings = {}
 
     # Base URL path. If not set, the plugin name will be used.
     base_url = "sp-addon"
 
     # Minimun Netbox version
-    min_version = "4.0.0-dev"
+    min_version = "4.0.0"
 
 
 config = SPAddonConfig
```

### Comparing `netbox_sp_addon-0.9.0/netbox_sp_addon/forms.py` & `netbox_sp_addon-0.9.1/netbox_sp_addon/forms.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from dcim.forms import DeviceFilterForm
 from dcim.models import RackRole
 from django.utils.translation import gettext_lazy as _
 from utilities.forms.fields import DynamicModelMultipleChoiceField
-
+from utilities.forms.rendering import FieldSet
 
 class SPDeviceFilterForm(DeviceFilterForm):
     fieldsets = (
-        (None, ('q', 'filter_id', 'tag')),
-        (_('Location'), ('region_id', 'site_group_id', 'site_id', 'location_id', 'rack_role', 'rack_id')),
-        (_('Operation'), ('status', 'role_id', 'airflow', 'serial', 'asset_tag', 'mac_address')),
-        (_('Hardware'), ('manufacturer_id', 'device_type_id', 'platform_id')),
-        (_('Tenant'), ('tenant_group_id', 'tenant_id')),
-        (_('Contacts'), ('contact', 'contact_role', 'contact_group')),
-        (_('Components'), (
+        FieldSet('q', 'filter_id', 'tag'),
+        FieldSet('region_id', 'site_group_id', 'site_id', 'location_id', 'rack_role', 'rack_id', name=_('Location')),
+        FieldSet('status', 'role_id', 'airflow', 'serial', 'asset_tag', 'mac_address', name=_('Operation')),
+        FieldSet('manufacturer_id', 'device_type_id', 'platform_id', name=_('Hardware')),
+        FieldSet('tenant_group_id', 'tenant_id', name=_('Tenant')),
+        FieldSet('contact', 'contact_role', 'contact_group', name=_('Contacts')),
+        FieldSet(
             'console_ports', 'console_server_ports', 'power_ports', 'power_outlets', 'interfaces', 'pass_through_ports',
-        )),
-        (_('Miscellaneous'), (
+            name=_('Components')
+        ),
+        FieldSet(
             'has_primary_ip', 'has_oob_ip', 'virtual_chassis_member', 'config_template_id', 'local_context_data',
-        ))
+            name=_('Miscellaneous')
+        )
     )
 
     rack_role = DynamicModelMultipleChoiceField(
         queryset=RackRole.objects.all(),
         required=False,
         label="Rack role",
     )
```

### Comparing `netbox_sp_addon-0.9.0/pyproject.toml` & `netbox_sp_addon-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "Topic :: System :: Systems Administration"
 ]
 description = "Adds some functions used by scanplus GmbH"
 license = "Apache-2.0"
 name = "netbox-sp-addon"
 readme = "README.md"
 repository = "https://github.com/scanplus/netbox-sp-addon"
-version = "0.9.0"
+version = "0.9.1"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
```

### Comparing `netbox_sp_addon-0.9.0/PKG-INFO` & `netbox_sp_addon-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-sp-addon
-Version: 0.9.0
+Version: 0.9.1
 Summary: Adds some functions used by scanplus GmbH
 Home-page: https://github.com/scanplus/netbox-sp-addon
 License: Apache-2.0
 Author: Tobias Genannt
 Author-email: tobias.genannt@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Plugins
```

