# Comparing `tmp/refoss_ha-1.2.0-py3-none-any.whl.zip` & `tmp/refoss_ha-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 8705 bytes, number of entries: 14
+Zip file size: 9680 bytes, number of entries: 15
 -rw-r--r--  2.0 unx       12 b- defN 23-Sep-08 02:57 refoss_ha/__init__.py
 -rw-r--r--  2.0 unx     4319 b- defN 23-Oct-17 03:12 refoss_ha/device.py
--rw-r--r--  2.0 unx     3481 b- defN 23-Oct-08 09:33 refoss_ha/device_manager.py
+-rw-r--r--  2.0 unx     3566 b- defN 24-May-06 06:10 refoss_ha/device_manager.py
 -rw-r--r--  2.0 unx     4697 b- defN 23-Oct-10 13:08 refoss_ha/discovery.py
--rw-r--r--  2.0 unx      222 b- defN 23-Sep-03 05:16 refoss_ha/enums.py
+-rw-r--r--  2.0 unx      282 b- defN 24-May-06 06:13 refoss_ha/enums.py
 -rw-r--r--  2.0 unx      153 b- defN 23-Oct-08 09:33 refoss_ha/exceptions.py
 -rw-r--r--  2.0 unx      925 b- defN 23-Oct-08 09:33 refoss_ha/util.py
 -rw-r--r--  2.0 unx       18 b- defN 23-Sep-03 05:34 refoss_ha/controller/__init__.py
 -rw-r--r--  2.0 unx     1354 b- defN 23-Oct-10 13:10 refoss_ha/controller/device.py
+-rw-r--r--  2.0 unx     1917 b- defN 24-May-06 08:14 refoss_ha/controller/electricity.py
 -rw-r--r--  2.0 unx     3146 b- defN 23-Oct-09 12:52 refoss_ha/controller/toggle.py
--rw-r--r--  2.0 unx      126 b- defN 23-Oct-17 03:14 refoss_ha-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Oct-17 03:14 refoss_ha-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Oct-17 03:14 refoss_ha-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1107 b- defN 23-Oct-17 03:14 refoss_ha-1.2.0.dist-info/RECORD
-14 files, 19662 bytes uncompressed, 6869 bytes compressed:  65.1%
+-rw-r--r--  2.0 unx      126 b- defN 24-May-06 10:27 refoss_ha-1.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-06 10:27 refoss_ha-1.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-06 10:27 refoss_ha-1.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1199 b- defN 24-May-06 10:27 refoss_ha-1.2.1.dist-info/RECORD
+15 files, 21816 bytes uncompressed, 7698 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -21,23 +21,26 @@
 
 Filename: refoss_ha/controller/__init__.py
 Comment: 
 
 Filename: refoss_ha/controller/device.py
 Comment: 
 
+Filename: refoss_ha/controller/electricity.py
+Comment: 
+
 Filename: refoss_ha/controller/toggle.py
 Comment: 
 
-Filename: refoss_ha-1.2.0.dist-info/METADATA
+Filename: refoss_ha-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: refoss_ha-1.2.0.dist-info/WHEEL
+Filename: refoss_ha-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: refoss_ha-1.2.0.dist-info/top_level.txt
+Filename: refoss_ha-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: refoss_ha-1.2.0.dist-info/RECORD
+Filename: refoss_ha-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## refoss_ha/device_manager.py

```diff
@@ -2,26 +2,26 @@
 from __future__ import annotations
 
 from functools import lru_cache
 from typing import Optional
 
 from .controller.device import BaseDevice
 from .controller.toggle import ToggleXMix
+from .controller.electricity import ElectricityXMix
 from .enums import Namespace
 from .device import DeviceInfo
 from .exceptions import DeviceTimeoutError
 
 _ABILITY_MATRIX = {
     Namespace.CONTROL_TOGGLEX.value: ToggleXMix,
+    Namespace.CONTROL_ELECTRICITYX.value: ElectricityXMix,
 }
 
 
-async def async_build_base_device(
-        device_info: DeviceInfo
-) -> Optional[BaseDevice]:
+async def async_build_base_device(device_info: DeviceInfo) -> Optional[BaseDevice]:
     """Build base device."""
     try:
         res = await device_info.async_execute_cmd(
             device_uuid=device_info.uuid,
             method="GET",
             namespace=Namespace.SYSTEM_ABILITY,
             payload={},
@@ -43,25 +43,25 @@
 
 
 _dynamic_types: dict[str, type] = {}
 
 
 @lru_cache(maxsize=512)
 def _lookup_cached_type(
-        device_type: str, hardware_version: str, firmware_version: str
+    device_type: str, hardware_version: str, firmware_version: str
 ) -> Optional[type]:
     """Lookup."""
     lookup_string = _caclulate_device_type_name(
         device_type, hardware_version, firmware_version
     ).strip(":")
     return _dynamic_types.get(lookup_string)
 
 
 def build_device_from_abilities(
-        device_info: DeviceInfo, device_abilities: dict
+    device_info: DeviceInfo, device_abilities: dict
 ) -> BaseDevice:
     """build_device_from_abilities."""
     cached_type = _lookup_cached_type(
         device_info.device_type,
         device_info.hdware_version,
         device_info.fmware_version,
     )
@@ -85,22 +85,22 @@
 
     component = cached_type(device=device_info)
 
     return component
 
 
 def _caclulate_device_type_name(
-        device_type: str, hardware_version: str, firmware_version: str
+    device_type: str, hardware_version: str, firmware_version: str
 ) -> str:
     """_caclulate_device_type_name."""
     return f"{device_type}:{hardware_version}:{firmware_version}"
 
 
 def _build_cached_type(
-        type_string: str, device_abilities: dict, base_class: type
+    type_string: str, device_abilities: dict, base_class: type
 ) -> type:
     """_build_cached_type."""
     mixin_classes = set()
 
     for key, _value in device_abilities.items():
         clsx = None
         cls = _ABILITY_MATRIX.get(key)
```

## refoss_ha/enums.py

```diff
@@ -5,7 +5,8 @@
 class Namespace(Enum):
     """A namespace."""
 
     SYSTEM_ALL = "Appliance.System.All"
     SYSTEM_ABILITY = "Appliance.System.Ability"
 
     CONTROL_TOGGLEX = "Appliance.Control.ToggleX"
+    CONTROL_ELECTRICITYX = "Appliance.Control.ElectricityX"
```

## Comparing `refoss_ha-1.2.0.dist-info/RECORD` & `refoss_ha-1.2.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 refoss_ha/__init__.py,sha256=z2nFVvvIzirxklQ9i5-F1nR-WOgcDttYtog_jx4yN5I,12
 refoss_ha/device.py,sha256=rNudmCphYuD_iCw-2d87nWkidoKPe8i32p38CKerSrI,4319
-refoss_ha/device_manager.py,sha256=5Hrpc7yOa3vizXIRmJqUxV6Q143RMEEKcxuMOHiaI9g,3481
+refoss_ha/device_manager.py,sha256=YYQD6o5FXlaFhe8-GpvhLSMyR43cUOVc3_QYdMD4YCQ,3566
 refoss_ha/discovery.py,sha256=wfwFwMEj-o2aF0be_WdLqEZfb-iT0xoe7xYFyH3g_0o,4697
-refoss_ha/enums.py,sha256=q29P7xtKa-TfMtNqdaizJhxDVjlqGOgXiT818tzK3k0,222
+refoss_ha/enums.py,sha256=g91j_FYpc-xmmPNmttFwO3-3ki-_O8akrSLo8pYqyrc,282
 refoss_ha/exceptions.py,sha256=fX8EmaeVklUuAmzRv-buobRfjHrN4SVYAvAGI-vDqZM,153
 refoss_ha/util.py,sha256=9D8AM-R9ASEthh6jmcWbKskUrYBBgJ5pBIZqlYto5wo,925
 refoss_ha/controller/__init__.py,sha256=JnhAs10hGsLXx5g3QMgwwJNEsSFugx06wodRLnHYcJc,18
 refoss_ha/controller/device.py,sha256=5Ur8iuvHkc1CQmhVbV_dSppZToARsoE1f_N4SMlLgfE,1354
+refoss_ha/controller/electricity.py,sha256=MNZb6qONJO3TvOB7qazsHOyRXrJ_KNFpLWS4mPHvhgY,1917
 refoss_ha/controller/toggle.py,sha256=IY2oTaBp8tTNDfU-UxAjF7zThbkb8yInRV_0W85jHQE,3146
-refoss_ha-1.2.0.dist-info/METADATA,sha256=3X77FP1oaUu0Pd_kxAXxdHFRwH6-xhqkQLTz3AGfeb8,126
-refoss_ha-1.2.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-refoss_ha-1.2.0.dist-info/top_level.txt,sha256=GE4dlww_crxGxvz1cACnUjObzDUbg2TvAZqaCxnODnM,10
-refoss_ha-1.2.0.dist-info/RECORD,,
+refoss_ha-1.2.1.dist-info/METADATA,sha256=WeHy_HxpG5XV_CXV1TDCRdQaS34L0o47KstolvRLuuw,126
+refoss_ha-1.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+refoss_ha-1.2.1.dist-info/top_level.txt,sha256=GE4dlww_crxGxvz1cACnUjObzDUbg2TvAZqaCxnODnM,10
+refoss_ha-1.2.1.dist-info/RECORD,,
```

