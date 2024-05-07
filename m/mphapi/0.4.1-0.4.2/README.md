# Comparing `tmp/mphapi-0.4.1.tar.gz` & `tmp/mphapi-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mphapi-0.4.1.tar", max compression
+gzip compressed data, was "mphapi-0.4.2.tar", max compression
```

## Comparing `mphapi-0.4.1.tar` & `mphapi-0.4.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      210 2024-04-10 01:49:16.715908 mphapi-0.4.1/mphapi/__init__.py
--rw-r--r--   0        0        0    11527 2024-05-01 02:45:34.995249 mphapi-0.4.1/mphapi/claim.py
--rw-r--r--   0        0        0     6297 2024-04-10 01:49:16.715908 mphapi-0.4.1/mphapi/client.py
--rw-r--r--   0        0        0     1504 2024-04-10 01:49:16.715908 mphapi-0.4.1/mphapi/date.py
--rw-r--r--   0        0        0      604 2024-05-01 02:21:58.782494 mphapi-0.4.1/mphapi/fields.py
--rw-r--r--   0        0        0    10159 2024-05-01 02:21:58.782494 mphapi-0.4.1/mphapi/pricing.py
--rw-r--r--   0        0        0     2958 2024-04-10 01:49:16.715908 mphapi-0.4.1/mphapi/response.py
--rw-r--r--   0        0        0      342 2024-05-01 02:45:34.995249 mphapi-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 mphapi-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      210 2024-04-10 01:49:16.715908 mphapi-0.4.2/mphapi/__init__.py
+-rw-r--r--   0        0        0    11527 2024-05-03 01:56:17.906614 mphapi-0.4.2/mphapi/claim.py
+-rw-r--r--   0        0        0     6297 2024-04-10 01:49:16.715908 mphapi-0.4.2/mphapi/client.py
+-rw-r--r--   0        0        0     1504 2024-04-10 01:49:16.715908 mphapi-0.4.2/mphapi/date.py
+-rw-r--r--   0        0        0      604 2024-05-03 01:56:17.906614 mphapi-0.4.2/mphapi/fields.py
+-rw-r--r--   0        0        0    10343 2024-05-07 13:56:29.702410 mphapi-0.4.2/mphapi/pricing.py
+-rw-r--r--   0        0        0     2958 2024-04-10 01:49:16.715908 mphapi-0.4.2/mphapi/response.py
+-rw-r--r--   0        0        0      342 2024-05-07 13:56:29.702410 mphapi-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 mphapi-0.4.2/PKG-INFO
```

### Comparing `mphapi-0.4.1/mphapi/claim.py` & `mphapi-0.4.2/mphapi/claim.py`

 * *Files identical despite different names*

### Comparing `mphapi-0.4.1/mphapi/client.py` & `mphapi-0.4.2/mphapi/client.py`

 * *Files identical despite different names*

### Comparing `mphapi-0.4.1/mphapi/date.py` & `mphapi-0.4.2/mphapi/date.py`

 * *Files identical despite different names*

### Comparing `mphapi-0.4.1/mphapi/fields.py` & `mphapi-0.4.2/mphapi/fields.py`

 * *Files identical despite different names*

### Comparing `mphapi-0.4.1/mphapi/pricing.py` & `mphapi-0.4.2/mphapi/pricing.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,17 @@
 
     readmission_adjustment_amount: Optional[float] = None
     """Adjustment amount for hospitals with high readmission rates"""
 
     value_based_purchasing_amount: Optional[float] = None
     """Adjustment for hospitals based on quality measures"""
 
+    wage_index: Optional[float] = None
+    """Wage index used for geographic adjustment"""
+
 
 class OutpatientPriceDetail(BaseModel):
     """OutpatientPriceDetail contains pricing details for an outpatient claim"""
 
     model_config = camel_case_model_config
 
     outlier_amount: float
@@ -110,14 +113,17 @@
 
     full_or_partial_device_credit_offset_amount: float
     """Credit for devices that are supplied for free or at a reduced cost"""
 
     terminated_device_procedure_offset_amount: float
     """Credit for devices that are not used due to a terminated procedure"""
 
+    wage_index: Optional[float] = None
+    """Wage index used for geographic adjustment"""
+
 
 class ProviderDetail(BaseModel):
     """
     ProviderDetail contains basic information about the provider and/or locality used for pricing.
     Not all fields are returned with every pricing request. For example, the CMS Certification
     Number (CCN) is only returned for facilities which have a CCN such as hospitals.
     """
```

### Comparing `mphapi-0.4.1/mphapi/response.py` & `mphapi-0.4.2/mphapi/response.py`

 * *Files identical despite different names*

