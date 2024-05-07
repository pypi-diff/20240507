# Comparing `tmp/json_ntv-1.3.0.tar.gz` & `tmp/json_ntv-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_ntv-1.3.0.tar", last modified: Tue Feb  6 22:07:11 2024, max compression
+gzip compressed data, was "json_ntv-1.4.0.tar", last modified: Tue May  7 09:39:33 2024, max compression
```

## Comparing `json_ntv-1.3.0.tar` & `json_ntv-1.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-02-06 22:07:11.692635 json_ntv-1.3.0/
--rw-rw-rw-   0        0        0     5912 2024-02-06 22:07:11.692138 json_ntv-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5198 2024-02-06 16:59:26.000000 json_ntv-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-06 22:07:11.676706 json_ntv-1.3.0/json_ntv/
--rw-rw-rw-   0        0        0     2453 2024-02-06 16:59:26.000000 json_ntv-1.3.0/json_ntv/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-06 22:07:11.687160 json_ntv-1.3.0/json_ntv/config/
--rw-rw-rw-   0        0        0      171 2024-01-09 17:39:42.000000 json_ntv-1.3.0/json_ntv/config/NTV_fr_BAN_namespace.ini
--rw-rw-rw-   0        0        0       64 2024-01-09 17:39:42.000000 json_ntv-1.3.0/json_ntv/config/NTV_fr_BAN_test_namespace.ini
--rw-rw-rw-   0        0        0       64 2024-01-09 17:39:42.000000 json_ntv-1.3.0/json_ntv/config/NTV_fr_IRVE_namespace.ini
--rw-rw-rw-   0        0        0      989 2024-01-09 17:39:42.000000 json_ntv-1.3.0/json_ntv/config/NTV_fr_namespace.ini
--rw-rw-rw-   0        0        0    15476 2024-02-06 16:59:26.000000 json_ntv-1.3.0/json_ntv/config/NTV_global_namespace.ini
--rw-rw-rw-   0        0        0      927 2024-01-31 22:59:40.000000 json_ntv-1.3.0/json_ntv/config/NTV_sch_namespace.ini
--rw-rw-rw-   0        0        0       69 2024-01-09 17:39:42.000000 json_ntv-1.3.0/json_ntv/config/NTV_schemaorg_namespace.ini
--rw-rw-rw-   0        0        0    19882 2024-02-06 17:01:43.000000 json_ntv-1.3.0/json_ntv/namespace.py
--rw-rw-rw-   0        0        0    49437 2024-02-06 17:03:32.000000 json_ntv-1.3.0/json_ntv/ntv.py
--rw-rw-rw-   0        0        0     3730 2024-02-06 17:02:04.000000 json_ntv-1.3.0/json_ntv/ntv_comment.py
--rw-rw-rw-   0        0        0    17253 2024-02-06 17:02:24.000000 json_ntv-1.3.0/json_ntv/ntv_connector.py
--rw-rw-rw-   0        0        0    13225 2024-02-06 17:02:40.000000 json_ntv-1.3.0/json_ntv/ntv_patch.py
--rw-rw-rw-   0        0        0    21525 2024-02-06 17:02:56.000000 json_ntv-1.3.0/json_ntv/ntv_util.py
--rw-rw-rw-   0        0        0    16431 2024-02-06 17:03:12.000000 json_ntv-1.3.0/json_ntv/ntv_validate.py
-drwxrwxrwx   0        0        0        0 2024-02-06 22:07:11.690645 json_ntv-1.3.0/json_ntv.egg-info/
--rw-rw-rw-   0        0        0     5912 2024-02-06 22:07:11.000000 json_ntv-1.3.0/json_ntv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      741 2024-02-06 22:07:11.000000 json_ntv-1.3.0/json_ntv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-06 22:07:11.000000 json_ntv-1.3.0/json_ntv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-02-06 22:07:11.000000 json_ntv-1.3.0/json_ntv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-06 22:07:11.000000 json_ntv-1.3.0/json_ntv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-02-06 22:07:11.693133 json_ntv-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1206 2024-02-06 16:59:26.000000 json_ntv-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-06 22:07:11.690147 json_ntv-1.3.0/tests/
--rw-rw-rw-   0        0        0     3982 2023-06-18 13:11:00.000000 json_ntv-1.3.0/tests/test_mongo.py
--rw-rw-rw-   0        0        0     1022 2023-10-07 19:48:58.000000 json_ntv-1.3.0/tests/test_ntvstruct.py
--rw-rw-rw-   0        0        0     5282 2024-01-31 22:59:40.000000 json_ntv-1.3.0/tests/tests_namespace.py
--rw-rw-rw-   0        0        0    50021 2024-02-06 16:59:26.000000 json_ntv-1.3.0/tests/tests_ntv.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:39:32.998565 json_ntv-1.4.0/
+-rw-rw-rw-   0        0        0     6187 2024-05-07 09:39:32.998067 json_ntv-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5473 2024-05-07 09:02:28.000000 json_ntv-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 09:39:32.980642 json_ntv-1.4.0/json_ntv/
+-rw-rw-rw-   0        0        0     2346 2024-05-06 19:57:09.000000 json_ntv-1.4.0/json_ntv/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:39:32.990599 json_ntv-1.4.0/json_ntv/config/
+-rw-rw-rw-   0        0        0      171 2024-01-09 17:39:42.000000 json_ntv-1.4.0/json_ntv/config/NTV_fr_BAN_namespace.ini
+-rw-rw-rw-   0        0        0       64 2024-01-09 17:39:42.000000 json_ntv-1.4.0/json_ntv/config/NTV_fr_BAN_test_namespace.ini
+-rw-rw-rw-   0        0        0       64 2024-01-09 17:39:42.000000 json_ntv-1.4.0/json_ntv/config/NTV_fr_IRVE_namespace.ini
+-rw-rw-rw-   0        0        0      989 2024-01-09 17:39:42.000000 json_ntv-1.4.0/json_ntv/config/NTV_fr_namespace.ini
+-rw-rw-rw-   0        0        0    18195 2024-04-05 21:01:01.000000 json_ntv-1.4.0/json_ntv/config/NTV_global_namespace.ini
+-rw-rw-rw-   0        0        0      927 2024-01-31 22:59:40.000000 json_ntv-1.4.0/json_ntv/config/NTV_sch_namespace.ini
+-rw-rw-rw-   0        0        0       69 2024-01-09 17:39:42.000000 json_ntv-1.4.0/json_ntv/config/NTV_schemaorg_namespace.ini
+-rw-rw-rw-   0        0        0    23512 2024-05-06 20:28:42.000000 json_ntv-1.4.0/json_ntv/namespace.py
+-rw-rw-rw-   0        0        0    49474 2024-05-06 21:37:06.000000 json_ntv-1.4.0/json_ntv/ntv.py
+-rw-rw-rw-   0        0        0     3637 2024-05-06 20:29:17.000000 json_ntv-1.4.0/json_ntv/ntv_comment.py
+-rw-rw-rw-   0        0        0    17380 2024-05-06 20:35:42.000000 json_ntv-1.4.0/json_ntv/ntv_connector.py
+-rw-rw-rw-   0        0        0    13136 2024-05-06 20:37:15.000000 json_ntv-1.4.0/json_ntv/ntv_patch.py
+-rw-rw-rw-   0        0        0    23412 2024-05-06 20:39:52.000000 json_ntv-1.4.0/json_ntv/ntv_util.py
+-rw-rw-rw-   0        0        0    18049 2024-05-06 21:08:52.000000 json_ntv-1.4.0/json_ntv/ntv_validate.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:39:32.997071 json_ntv-1.4.0/json_ntv.egg-info/
+-rw-rw-rw-   0        0        0     6187 2024-05-07 09:39:32.000000 json_ntv-1.4.0/json_ntv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2024-05-07 09:39:32.000000 json_ntv-1.4.0/json_ntv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 09:39:32.000000 json_ntv-1.4.0/json_ntv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-07 09:39:32.000000 json_ntv-1.4.0/json_ntv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 09:39:32.000000 json_ntv-1.4.0/json_ntv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-07 09:39:32.999062 json_ntv-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1206 2024-05-07 09:28:28.000000 json_ntv-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:39:32.996076 json_ntv-1.4.0/tests/
+-rw-rw-rw-   0        0        0     3982 2023-06-18 13:11:00.000000 json_ntv-1.4.0/tests/test_mongo.py
+-rw-rw-rw-   0        0        0     1022 2023-10-07 19:48:58.000000 json_ntv-1.4.0/tests/test_ntvstruct.py
+-rw-rw-rw-   0        0        0     5582 2024-02-21 11:20:50.000000 json_ntv-1.4.0/tests/tests_namespace.py
+-rw-rw-rw-   0        0        0    50035 2024-02-21 14:33:36.000000 json_ntv-1.4.0/tests/tests_ntv.py
```

### Comparing `json_ntv-1.3.0/PKG-INFO` & `json_ntv-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_ntv
-Version: 1.3.0
+Version: 1.4.0
 Summary: JSON-NTV a semantic format for interoperability
 Home-page: https://github.com/loco-philippe/NTV/blob/main/README.md
 Author: Philippe Thomy
 Author-email: philippe@loco-labs.io
 Keywords: JSON-NTV,semantic JSON,development,environmental data
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -84,21 +84,29 @@
 
 > *For example, the type: `ns1.ns2.type_a` means that:*
 >
 > - *`ns1.` is a namespace defined in the global namespace,*
 > - *`ns2.` is a namespace defined in the `ns1.` namespace.,*
 > - *`type_a` is defined in the `ns2.` namespace.*
 
+The type can be extended with additional data.
+
+> *For example, the type: `float[kg]` means that:*
+>
+> - *`float` is a main type of the data,*
+> - *`kg` is an additional type (e.g. an unit),*
+> - *`float[kg]` may represent a Quantity.*
+
 This structuring of type makes it possible to reference any type of data that has a JSON representation and to consolidate all the shared data structures within the same tree of types.
 
 ## NTV uses
 
 Several variations and use cases of the NTV format are defined:
 
-- Tabular data exchange format (e.g. open-data)
+- Tabular and multidimensional data exchange format (e.g. open-data)
 - Compact, reversible and semantic pandas-JSON interface
 - Comment and change management of JSON data
 - visualization of JSON or NTV tree
 - JSON data editor
 - data validation (value conformity to the Datatype)
 
 ## NTV and JSON
@@ -115,15 +123,15 @@
     val--->|JSON dump|text
     val--->|NTV from JSON|ntv
     ntv--->|from NTV|nat
     ntv--->|NTV to JSON|val
     nat--->|to NTV|ntv
 ```
 
-The conversion between native entity and JSON-text is reversible (round trip).
+The conversion between native entity and JSON-text is reversible (lossless round trip).
 
 ```python
 In [6]: loc_and_date = {'newyear': date(2023, 1, 2), 'Paris': Point(2.3, 48.9)}
         json_loc_date = Ntv.obj(loc_and_date).to_obj(encoded=True)
         print(json_loc_date, type(json_loc_date))
 Out[6]: {"newyear:date": "2023-01-02", "Paris:point": [2.3, 48.9]} <class 'str'>
```

### Comparing `json_ntv-1.3.0/README.md` & `json_ntv-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -65,21 +65,29 @@
 
 > *For example, the type: `ns1.ns2.type_a` means that:*
 >
 > - *`ns1.` is a namespace defined in the global namespace,*
 > - *`ns2.` is a namespace defined in the `ns1.` namespace.,*
 > - *`type_a` is defined in the `ns2.` namespace.*
 
+The type can be extended with additional data.
+
+> *For example, the type: `float[kg]` means that:*
+>
+> - *`float` is a main type of the data,*
+> - *`kg` is an additional type (e.g. an unit),*
+> - *`float[kg]` may represent a Quantity.*
+
 This structuring of type makes it possible to reference any type of data that has a JSON representation and to consolidate all the shared data structures within the same tree of types.
 
 ## NTV uses
 
 Several variations and use cases of the NTV format are defined:
 
-- Tabular data exchange format (e.g. open-data)
+- Tabular and multidimensional data exchange format (e.g. open-data)
 - Compact, reversible and semantic pandas-JSON interface
 - Comment and change management of JSON data
 - visualization of JSON or NTV tree
 - JSON data editor
 - data validation (value conformity to the Datatype)
 
 ## NTV and JSON
@@ -96,15 +104,15 @@
     val--->|JSON dump|text
     val--->|NTV from JSON|ntv
     ntv--->|from NTV|nat
     ntv--->|NTV to JSON|val
     nat--->|to NTV|ntv
 ```
 
-The conversion between native entity and JSON-text is reversible (round trip).
+The conversion between native entity and JSON-text is reversible (lossless round trip).
 
 ```python
 In [6]: loc_and_date = {'newyear': date(2023, 1, 2), 'Paris': Point(2.3, 48.9)}
         json_loc_date = Ntv.obj(loc_and_date).to_obj(encoded=True)
         print(json_loc_date, type(json_loc_date))
 Out[6]: {"newyear:date": "2023-01-02", "Paris:point": [2.3, 48.9]} <class 'str'>
```

### Comparing `json_ntv-1.3.0/json_ntv/__init__.py` & `json_ntv-1.4.0/json_ntv/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,13 @@
 """
 from json_ntv.namespace import Namespace, Datatype, str_type, relative_type, agreg_type
 from json_ntv.ntv_patch import NtvOp, NtvPatch, NtvPointer
 from json_ntv.ntv_comment import NtvComment
 from json_ntv.ntv import Ntv, NtvSingle, NtvList
 from json_ntv.ntv_validate import Validator
 from json_ntv.ntv_util import NtvTree, NtvJsonEncoder, NtvConnector, NtvError
-#from json_ntv.pandas_ntv_connector import DataFrameConnec, SeriesConnec, read_json, to_json, as_def_type
 from json_ntv.ntv_connector import from_csv, to_csv
 from json_ntv.ntv_connector import MermaidConnec, CborConnec, ShapelyConnec
 from json_ntv.ntv_connector import NfieldConnec, SfieldConnec
 from json_ntv.ntv_connector import NdatasetConnec, SdatasetConnec
 
 #print('package :', __package__)
```

### Comparing `json_ntv-1.3.0/json_ntv/config/NTV_fr_namespace.ini` & `json_ntv-1.4.0/json_ntv/config/NTV_fr_namespace.ini`

 * *Files identical despite different names*

### Comparing `json_ntv-1.3.0/json_ntv/config/NTV_sch_namespace.ini` & `json_ntv-1.4.0/json_ntv/config/NTV_sch_namespace.ini`

 * *Files identical despite different names*

### Comparing `json_ntv-1.3.0/json_ntv/namespace.py` & `json_ntv-1.4.0/json_ntv/namespace.py`

 * *Files 18% similar despite different names*

```diff
@@ -77,27 +77,27 @@
     config.read(file)
     if not name in config.sections():
         raise DatatypeError(name + ' is not present in ' + str(file))
     _add_namespace(config, schema_nsp)
 
 
 def mapping(typ=None, func=None):
+    '''Affect a validate function (func) to a Datatype (typ) '''
     if typ and func:
-        Datatype.add(typ).validate = func
+        Datatype(typ).validate = func
     else:
         if isinstance(typ, str):
             func_lis = [typ + '_valid']
         elif isinstance(typ, (list, tuple)):
             func_lis = [typ_str + '_valid' for typ_str in typ]
         else:
             func_lis = [typ_str + '_valid' for typ_str in Datatype._types_]
         for func_str in func_lis:
             if func_str in Validator.__dict__:
-                Datatype.add(
-                    func_str[:-6]).validate = Validator.__dict__[func_str]
+                Datatype(func_str[:-6]).validate = Validator.__dict__[func_str]
 
 
 def relative_type(str_def, str_typ):
     '''return relative str_typ string from Datatype or Namespace str_def
 
     *Parameters*
 
@@ -133,15 +133,15 @@
         return None
     if long_name.__class__.__name__ in ['Datatype', 'Namespace']:
         return long_name
     if not isinstance(long_name, str):
         raise DatatypeError('the long_name is not a string')
     if long_name[-1] == '.':
         return Namespace.add(long_name)
-    return Datatype.add(long_name)
+    return Datatype(long_name)
 
 
 def _add_namespace(config, namesp):
     '''create the child Namespace and the child Datatype of the parent namespace'''
     if namesp.name in config.sections():
         confname = config[namesp.name]
         if 'namespace' in confname:
@@ -162,126 +162,127 @@
         idx = namesp_sp.index(str_typ_sp[0])
         if namesp_sp[idx:] != str_typ_sp[:len(namesp_sp[idx:])]:
             idx = -1
     if idx > -1:
         namesp_sp = namesp_sp[:idx]
     return ['.'.join(namesp_sp[:i+1]+str_typ_sp) for i in range(len(namesp_sp)-1, -1, -1)]
 
-    """namesp_split = namesp.split('.')[:-1]
-    for name in str_typ.split('.'):
-        if not name in namesp_split:
-            namesp_split.append(name)
-    return '.'.join(namesp_split)"""
-
 
 def _isin_schemaorg(name, prop=True, typ=None):
     ''' return True if a schema.org Property is present and associated to a Type
     or if a schema.org Type is present'''
     n_org = name if prop else name[:-1]
     t_org = typ[:-1] if typ else None
     req_name = requests.get(
-        SCH_ORG + n_org, allow_redirects=True).content.decode()
+        SCH_ORG + n_org, allow_redirects=True, timeout=10).content.decode()
     if not prop:
         return 'Type</ti' in req_name
     is_prop = 'Property</ti' in req_name
     if not t_org:
         return is_prop
     if is_prop:
-        return '/' + n_org in requests.get(SCH_ORG + t_org, allow_redirects=True
-                                           ).content.decode()
+        return '/' + n_org in requests.get(SCH_ORG + t_org, allow_redirects=True,
+                                           timeout=10).content.decode()
     return False
 
 
-class Datatype(NtvUtil):
+class TypeBase(NtvUtil):
     ''' type of NTV entities.
 
     *Attributes :*
 
     - **name** : String - name of the type
     - **nspace** : Namespace - namespace associated
     - **custom** : boolean - True if not referenced
+    - **validate** : function (default None) - validate function
 
     The methods defined in this class are :
 
     *staticmethods*
     - `types`
     - `add`
 
     *dynamic values (@property)*
+    - `category`
+    - `json_type`
     - `gen_type`
     - `long_name`
 
     *instance methods*
     - `isin_namespace`
-    - `validate`
     '''
 
     @staticmethod
     def types():
-        '''return the list of Datatype created'''
+        '''return the list of TypeBase created'''
         return [nam.long_name for nam in NtvUtil._types_.values()]
 
     @classmethod
     def add(cls, long_name, module=False, force=False, validate=None):
-        '''activate and return a valid Datatype defined by the long name
+        '''activate and return a valid TypeBase defined by the long name
 
         *parameters :*
 
-        - **long_name** : String - absolut name of the Datatype
+        - **long_name** : String - absolut name of the TypeBase
         - **module** : boolean (default False) - if True search data in the
         local .ini file, else in the distant repository
         - **validate** : function (default None) - validate function to include
         '''
         if long_name == '':
             return None
-        if long_name in Datatype.types():
+        if long_name in cls.types():
             return NtvUtil._types_[long_name]
         split_name = long_name.rsplit('.', 1)
         if split_name[-1] == '':
-            raise DatatypeError(long_name + ' is not a valid Datatype')
+            raise DatatypeError(long_name + ' is not a valid TypeBase')
         if len(split_name) == 1:
             return cls(split_name[0], force=force, validate=validate)
         if len(split_name) == 2:
             nspace = Namespace.add(
                 split_name[0]+'.', module=module, force=force)
             return cls(split_name[1], nspace, force=force)
-        raise DatatypeError(long_name + ' is not a valid Datatype')
+        raise DatatypeError(long_name + ' is not a valid TypeBase')
 
     def __init__(self, name, nspace=None, force=False, validate=None):
-        '''Datatype constructor.
+        '''TypeBase constructor.
 
         *Parameters*
 
         - **name** : string - name of the Type
         - **nspace** : Namespace (default None) - namespace associated
         - **force** : boolean (default False) - if True, no Namespace control
         - **validate** : function (default None) - validate function to include'''
-        if isinstance(name, Datatype):
+        if isinstance(name, TypeBase):
             self.name = name.name
             self.nspace = name.nspace
             self.custom = name.custom
             self.validate = name.validate
+            # self.gen_type = name.gen_type
+            # self.long_name = name.long_name
             return
         if not name or not isinstance(name, str):
             raise DatatypeError('null name is not allowed')
         if not name and not nspace:
             name = 'json'
         if not nspace:
             nspace = NtvUtil._namespaces_['']
         if nspace.file and SCH_ORG in nspace.file:
             if not _isin_schemaorg(name, typ=nspace.name):
-                raise DatatypeError(
-                    name + ' is not a schema.org Property associated to the ' + nspace.name + 'Type ')
+                raise DatatypeError(name +
+                                    ' is not a schema.org Property associated to the ' +
+                                    nspace.name + 'Type ')
         else:
             if not (name[0] == '$' or force or name in nspace.content['type']):
                 raise DatatypeError(
                     name + ' is not defined in ' + nspace.long_name)
         self.name = name
         self.nspace = nspace
         self.custom = nspace.custom or name[0] == '$'
+        # self.gen_type = '' if self.custom else self.nspace.content['type'][self.name]
+        # self.long_name = self.nspace.long_name + self.name
         if validate:
             self.validate = validate
         NtvUtil._types_[self.long_name] = self
         return
 
     def __eq__(self, other):
         ''' equal if name and nspace are equal'''
@@ -302,31 +303,146 @@
         return self.long_name
 
     def __repr__(self):
         '''return classname and long name'''
         return self.__class__.__name__ + '(' + self.long_name + ')'
 
     @property
+    def json_type(self):
+        '''return the json type of the TypeBase'''
+        if self.custom:
+            return ''
+        prop = self.nspace.content['type'][self.name]
+        if isinstance(prop, list):
+            return prop[1]
+        return 'json'
+
+    @property
+    def category(self):
+        '''return the category of the TypeBase'''
+        if self.custom:
+            return ''
+        prop = self.nspace.content['type'][self.name]
+        if isinstance(prop, list):
+            return prop[2]
+        return 'local'
+
+    @property
     def gen_type(self):
-        '''return the generic type of the Datatype'''
+        '''return the generic type of the TypeBase'''
         if self.custom:
             return ''
-        return self.nspace.content['type'][self.name]
+        prop = self.nspace.content['type'][self.name]
+        if isinstance(prop, list):
+            return prop[0]
+        return prop
 
     @property
     def long_name(self):
         '''return a string with the absolute name'''
         return self.nspace.long_name + self.name
 
     def isin_namespace(self, long_name):
         '''return the number of level between self and nspace, -1 if None'''
         return self.nspace.is_child(Namespace.add(long_name))
 
-    def validate(self, value):
-        return None
+
+
+class Datatype(TypeBase):
+    ''' The Datatype of NTV entities is composed with a TypeBase and an optional
+    extension.
+
+    *Attributes :*
+
+    - **name** : String - name of the Datatype
+    - **base_name** : String - name of the TypeBase
+    - **nspace** : Namespace - namespace associated
+    - **custom** : boolean - True if not referenced
+    - **validate** : function (default None) - validate function
+    - **typebase** : TypeBase - TypeBase of the Datatype
+    - **extension** : String (default None) - extension of the TypeBase
+
+    The methods defined in this class are :
+
+    *classmethod*
+    - `add`
+
+    *dynamic values (@property)*
+    - `category`
+    - `json_type`
+    - `gen_type`
+    - `long_name` (TypeBase)
+
+    *staticmethods*
+    - `types` (TypeBase)
+
+    *instance methods*
+    - `isin_namespace` (TypeBase)
+    - `validate` (TypeBase)
+    '''
+
+    def __init__(self, full_name, module=False, force=False, validate=None):
+        '''DataType constructor.
+
+        *Parameters*
+
+        - **full_name** : String - absolut name of the Datatype
+        - **module** : boolean (default False) - if True search data in the
+        local .ini file, else in the distant repository
+        - **force** : boolean (default False) - if True, no Namespace control
+        - **validate** : function (default None) - validate function to include'''
+        if isinstance(full_name, Datatype):
+            self.name = full_name.name
+            self.base_name = full_name.base_name
+            self.typebase = full_name.typebase
+            self.extension = full_name.extension
+            return
+        spl_name = full_name.split('[', maxsplit=1)
+        long_base = spl_name[0]
+        self.extension = spl_name[1][:-1] if len(spl_name) == 2 else None
+        self.typebase = TypeBase.add(long_base, module, force, validate)
+        ext_str = '[' + self.extension + ']' if self.extension else ''
+        self.base_name = self.typebase.name
+        self.name = self.typebase.name + ext_str
+        return
+
+    @property
+    def gen_type(self):
+        '''return the generic type of the Datatype'''
+        return self.typebase.gen_type
+
+    @property
+    def json_type(self):
+        '''return the json type of the Datatype'''
+        return self.typebase.json_type
+
+    @property
+    def category(self):
+        '''return the category of the Datatype'''
+        return self.typebase.category
+
+    @property
+    def nspace(self):
+        '''return the nspace of the Datatype'''
+        return self.typebase.nspace
+
+    @property
+    def custom(self):
+        '''return the custom of the Datatype'''
+        return self.typebase.custom
+
+    @property
+    def validate(self):
+        '''return the validate of the Datatype'''
+        return self.typebase.validate
+
+    @classmethod
+    def add(cls, long_name, module=False, force=False, validate=None):
+        '''method eqivalent to the constructor'''
+        return cls(long_name, module, force, validate)
 
 
 class Namespace(NtvUtil):
     ''' Namespace of NTV entities.
 
     *Attributes :*
 
@@ -393,26 +509,21 @@
         - **module** : boolean (default False) - if True search data in the
                         local .ini file, else in the distant repository
         - **content** : dict : {'type': <list of ntv_type names>,
                                 'namespace': <list of namespace names>}
         '''
         if name and not parent:
             parent = NtvUtil._namespaces_['']
-        '''if name and name[0] != '$' and not force and not (
-           name in parent.content['namespace'] or 'schema.org' in parent.file):
-            raise DatatypeError(name + ' is not defined in ' + parent.long_name)'''
-
         if parent and parent.file and SCH_ORG in parent.file:
             if not _isin_schemaorg(name, False):
                 raise DatatypeError(name + ' is not a schema.org Type ')
         else:
             if name and not (name[0] == '$' or force or name in parent.content['namespace']):
                 raise DatatypeError(
                     name + ' is not defined in ' + parent.long_name)
-
         self.name = name
         self.parent = parent
         self.custom = parent.custom or name[0] == '$' if parent else False
         self.file = Namespace._file(
             self.parent, self.name, self.custom, module)
         self.content = Namespace._content(
             self.file, self.name, self.custom, module)
@@ -459,15 +570,15 @@
                 return SCH_ORG
             config = configparser.ConfigParser()
             if module:
                 p_file = Path(parent.file).stem + Path(parent.file).suffix
                 config.read(Path(json_ntv.__file__).parent / 'config' / p_file)
             else:
                 config.read_string(requests.get(
-                    parent.file, allow_redirects=True).content.decode())
+                    parent.file, allow_redirects=True, timeout=10).content.decode())
             return Namespace._pathconfig_ + json.loads(config['data']['namespace'])[name]
         return Namespace._pathconfig_ + Namespace._global_
 
     @staticmethod
     def _content(file, name, custom, module):
         '''return the content of the Namespace configuration
 
@@ -488,15 +599,15 @@
             return {'type': {}, 'namespace': {}}
         config = configparser.ConfigParser()
         if module:
             p_file = Path(file).stem + Path(file).suffix
             config.read(Path(json_ntv.__file__).parent / 'config' / p_file)
         else:
             config.read_string(requests.get(
-                file, allow_redirects=True).content.decode())
+                file, allow_redirects=True, timeout=10).content.decode())
         config_name = config['data']['name']
         if config_name != name:
             raise DatatypeError(file + ' is not correct')
         return {'type': json.loads(config['data']['type']),
                 'namespace': json.loads(config['data']['namespace'])}
 
     @property
@@ -505,36 +616,35 @@
         if self.parent is None or self.parent.name == '':
             return self.name
         return self.parent.long_name + self.name
 
     def is_child(self, nspace):
         '''return the number of level between self and nspace, -1 if None'''
         parent = self.parent
-        if not self.name:
-            return -1
         if self == nspace:
             return 0
+        if not self.name:
+            return -1
         rang = 1
         while parent.name != '' and parent != nspace:
             rang += 1
             parent = parent.parent
         if parent == nspace:
             return rang
-        if parent.name == '':
-            return -1
+        return -1
 
     def is_parent(self, nspace):
         '''return the number of level between self and nspace, -1 if None'''
         return nspace.is_child(self)
 
 
 class DatatypeError(Exception):
     ''' Datatype or Namespace Exception'''
 
 
 nroot = Namespace(module=True)
 for root_typ in nroot.content['type']:
-    #typ = Datatype.add(root_typ, module=True)
-    typ = Datatype.add(root_typ, module=True,
-                       validate=Validator.__dict__[root_typ + '_valid'])
+    # typ = Datatype(root_typ, module=True,
+    Datatype(root_typ, module=True,
+             validate=Validator.__dict__[root_typ + '_valid'])
 # mapping(Datatype.types())
 typ_json = Datatype('json')
```

### Comparing `json_ntv-1.3.0/json_ntv/ntv.py` & `json_ntv-1.4.0/json_ntv/ntv.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         - **ntv_value**: Json entity - value of the entity
         - **ntv_name** : String (default None) - name of the NTV entity
         - **ntv_type**: String or Datatype or Namespace (default None) - type of the entity
         '''
         if ntv_type.__class__.__name__ in ['Datatype', 'Namespace']:
             self.ntv_type = ntv_type
         elif ntv_type and ntv_type[-1] != '.':
-            self.ntv_type = Datatype.add(ntv_type)
+            self.ntv_type = Datatype(ntv_type)
         elif ntv_type and ntv_type[-1] == '.':
             self.ntv_type = Namespace.add(ntv_type)
         else:
             self.ntv_type = None
         if not isinstance(ntv_name, str):
             ntv_name = ''
         self.ntv_name = ntv_name
@@ -141,19 +141,16 @@
             - a tuple with value, name, typ and cat (see `from_att` method)
             - a value to decode (see `from_obj`method)
         - **no_typ** : boolean (default False) - if True, NtvList is with None type
         - **type_auto**: boolean (default False) - if True, default type for NtvList
         is the ntv_type of the first Ntv in the ntv_value
         - **fast** : boolean (default False) - if True, Ntv entity is created without conversion
         - **decode_str**: boolean (default False) - if True, string are loaded in json data'''
-        #print('obj : ', Namespace.namespaces(), '\n')
-
         if isinstance(data, tuple):
             return Ntv.from_att(*data, decode_str=decode_str, fast=fast)
-        # if isinstance(data, str) and data.lstrip() and data.lstrip()[0] in '{[':
         if isinstance(data, str):
             try:
                 data = json.loads(data)
             except json.JSONDecodeError:
                 pass
         return Ntv.from_obj(data, no_typ=no_typ, decode_str=decode_str,
                             typ_auto=typ_auto, fast=fast)
@@ -204,15 +201,14 @@
         if isinstance(ntv_value, (list, dict)) and sep in (None, '::'):
             return Ntv._create_ntvlist(str_typ, def_type, sep, ntv_value,
                                        typ_auto, no_typ, ntv_name, fast)
         if sep == ':' or (sep is None and isinstance(ntv_value, dict)):
             ntv_type = agreg_type(str_typ, def_type, False)
             return NtvSingle(ntv_value, ntv_name, ntv_type, fast=fast)
         if sep is None and not isinstance(ntv_value, dict):
-            #is_single_json = isinstance(value, (int, str, float, bool))
             is_single_json = isinstance(ntv_value, (int, str, float, bool))
             ntv_type = agreg_type(str_typ, def_type, is_single_json)
             return NtvSingle(ntv_value, ntv_name, ntv_type, fast=fast)
         raise NtvError('separator ":" is not compatible with value')
 
     def __len__(self):
         ''' len of ntv_value'''
@@ -222,27 +218,25 @@
 
     def __str__(self):
         '''return string format'''
         return self.to_obj(encoded=True)
 
     def __repr__(self):
         '''return classname and code'''
-        # return json.dumps(self.to_repr(False, False, False, 10), cls=NtvJsonEncoder)
         return self.reduce(obj=False, level=3, maxi=6).to_obj(encoded=True)
 
     def __contains__(self, item):
         ''' item of Ntv entities'''
         if isinstance(self.val, list):
             return item in self.ntv_value
         return item == self.ntv_value
 
     def __iter__(self):
         ''' iterator for Ntv entities'''
         if isinstance(self, NtvSingle):
-            # return iter([self.val])
             return iter([self])
         return iter(self.val)
 
     def __getitem__(self, selec):
         ''' return ntv_value item with selec:
             - String beginning with "#" : json-pointer,
             - string : name of the ntv,
@@ -252,15 +246,15 @@
             return self
         if isinstance(selec, NtvPointer) or isinstance(selec, str) and selec[0] == '#':
             selec = self._pointer_to_list(selec)
         if selec in ([], ()):
             return self
         if isinstance(selec, (list, tuple)) and len(selec) == 1:
             selec = selec[0]
-        if (selec == 0 or selec == self.ntv_name) and isinstance(self, NtvSingle):
+        if selec in (0, self.ntv_name) and isinstance(self, NtvSingle):
             return self.ntv_value
         if isinstance(self, NtvSingle):
             raise NtvError('item not present')
         if isinstance(selec, tuple):
             return [self[i] for i in selec]
         if isinstance(selec, str):
             return self.ntv_value[self._string_to_ind(selec)]
@@ -335,14 +329,21 @@
 
     @property
     def tree(self):
         '''return a tree with included entities (NtvTree object)'''
         return NtvTree(self)
 
     @property
+    def typebase_str(self):
+        '''return a string with the value of the TypeBase of the entity'''
+        if not self.ntv_type:
+            return ''
+        return self.ntv_type.typebase.long_name
+
+    @property
     def type_str(self):
         '''return a string with the value of the NtvType of the entity'''
         if not self.ntv_type:
             return ''
         return self.ntv_type.long_name
 
     @property
@@ -388,15 +389,15 @@
         exp = {ENTITY: self.__class__.__name__} if entity else {}
         if isinstance(self, NtvList) and full:
             return exp | {NAME: self.name, TYPE: self.type_str,
                           VALUE: [ntv.expand(full) for ntv in self.val]}
         if isinstance(self, NtvSingle) and full:
             return exp | {NAME: self.name, TYPE: self.type_str, VALUE: self.val}
         exp |= {} if not self.name else {NAME: self.name}
-        if not self.type_str in ['json', '']:
+        if self.type_str not in ['json', '']:
             exp[TYPE] = self.type_str
         if isinstance(self, NtvList):
             exp[VALUE] = [ntv.expand(full) for ntv in self.val]
         else:
             exp[VALUE] = self.val
         return exp
 
@@ -417,17 +418,18 @@
         if def_type is None:
             def_type = ''
         elif isinstance(def_type, (Datatype, Namespace)):
             def_type = def_type.long_name
         json_name = self.ntv_name if self.ntv_name else ''
         json_type = relative_type(
             def_type, self.type_str) if self.ntv_type else ''
-        implicit = isinstance(self, NtvSingle) and (json_type == 'json'
-                                                    and (not def_type or def_type == 'json' or def_type[-1] == '.')
-                                                    or not NtvConnector.is_json_class(self.val))
+        implicit = isinstance(self, NtvSingle) and (
+            json_type == 'json' and (
+                not def_type or def_type == 'json' or def_type[-1] == '.')
+            or not NtvConnector.is_json_class(self.val))
         if implicit and not explicit:
             json_type = ''
         json_sep = self._obj_sep(json_name, json_type, def_type)
         if string:
             return json_name + json_sep + json_type
         return [json_name, json_sep, json_type]
 
@@ -625,15 +627,15 @@
         if parent:
             idx = parent.ntv_value.index(self)
             parent.insert(idx, ntv)
             del parent[idx+1]
             if not self in parent:
                 self.parent = None
         else:
-            self = ntv
+            raise NtvError('replace is not available for root node')
 
     def set_name(self, name='', nodes='simple'):
         '''set new names to the entity
 
         *Parameters*
 
         - **name**: list or string (default '') - New name values
@@ -825,28 +827,31 @@
         - **encoded** : boolean (default False) - choice for return format
         (string/bytes if True, dict/list/tuple else)
         - **format**  : string (default 'json')- choice for return format
         (json, cbor, obj)
         - **simpleval** : boolean (default False) - if True, only value (without
         name and type) is included
         - **name** : boolean (default true) - if False, name is not included
+        - **type** : boolean (default False) - if True, type is always included
         - **json_array** : boolean (default false) - if True, Json-object is not used for NtvList
         - **fast** : boolean (default False) - if True, json is created without conversion
         - **maxi**: Integer (default -1) - number of values to include for NtvList
         entities. If maxi < 1 all the values are included.
         '''
         option = {'encoded': False, 'format': 'json', 'fast': False, 'maxi': -1,
-                  'simpleval': False, 'name': True, 'json_array': False} | kwargs
+                  'simpleval': False, 'name': True, 'json_array': False,
+                  'type': False} | kwargs
         value = self.obj_value(def_type=def_type, **option)
         obj_name = self.json_name(def_type)
         if not option['name']:
             obj_name[0] = ''
         if option['simpleval']:
             name = ''
-        elif option['format'] in ('cbor', 'obj') and not NtvConnector.is_json_class(value):
+        elif (option['format'] in ('cbor', 'obj') and
+              not NtvConnector.is_json_class(value) and not option['type']):
             name = obj_name[0]
         else:
             name = obj_name[0] + obj_name[1] + obj_name[2]
         value = [value] if not name and isinstance(
             value, dict) and len(value) == 1 else value
         json_obj = {name: value} if name else value
         if option['encoded'] and option['format'] == 'json':
@@ -862,15 +867,15 @@
         for leaf in ntv.tree.leaf_nodes:
             if isinstance(leaf.ntv_value, (NtvSingle, NtvList)):
                 leaf.ntv_value = leaf.ntv_value.to_obj()
                 leaf.ntv_type = Datatype('ntv')
             elif not leaf.is_json:
                 leaf.ntv_value, leaf.ntv_name, type_str = NtvConnector.cast(
                     leaf.ntv_value, leaf.ntv_name, leaf.type_str)
-                leaf.ntv_type = Datatype.add(type_str)
+                leaf.ntv_type = Datatype(type_str)
                 leaf.is_json = True
         return ntv
 
     def to_obj_ntv(self, **kwargs):
         ''' create a copy where ntv-value of the self-tree nodes is converted
         in object-value
 
@@ -879,15 +884,15 @@
         - **kwargs** : parameters used in NtvConnector class (specific for each Connector)'''
         ntv = copy.copy(self)
         for leaf in ntv.tree.leaf_nodes:
             if (leaf.is_json and leaf.type_str in set(NtvConnector.dic_type.values())
                     or leaf.ntv_type is None):
                 leaf.ntv_value, leaf.ntv_name, type_str = NtvConnector.uncast(
                     leaf, **kwargs)
-                leaf.ntv_type = Datatype.add(type_str) if type_str else None
+                leaf.ntv_type = Datatype(type_str) if type_str else None
                 leaf.is_json = NtvConnector.is_json(leaf.ntv_value)
         return ntv
 
     def to_tuple(self, maxi=10):
         '''return a nested tuple representation of the NTV entity
         (NtvList/NtvSingle, ntv_name, ntv_type, ntv_value).
 
@@ -924,24 +929,24 @@
             if not valid:
                 errors.append(str(ntv.pointer()))
                 if unique:
                     return (False, errors)
         return (not errors, errors)
 
     @abstractmethod
-    def obj_value(self):
+    def obj_value(self, def_type=None, **kwargs):
         '''return the ntv_value with different formats defined by kwargs (abstract method)'''
 
     @property
     @abstractmethod
     def json_array(self):
         ''' return the json_array dynamic attribute (abstract method)'''
 
     @abstractmethod
-    def _obj_sep(self, json_type, def_type):
+    def _obj_sep(self, json_name, json_type, def_type=None):
         ''' return separator to include in json_name (abstract method)'''
 
     @staticmethod
     def _from_value(value, decode_str=False):
         '''return a decoded value
 
         *Parameters*
@@ -1061,37 +1066,36 @@
             return ':'
         return ''
 
     @staticmethod
     def _decode_s(ntv_value, ntv_name, ntv_type_str):
         '''return adjusted ntv_value, ntv_name, ntv_type(str)'''
         is_json = NtvConnector.is_json(ntv_value)
+        name = None
         if is_json:
             if isinstance(ntv_value, (list)):
                 ntv_value = [NtvSingle._decode_s(val, '', ntv_type_str)[
                     0] for val in ntv_value]
             elif isinstance(ntv_value, (dict)):
                 ntv_value = {key: NtvSingle._decode_s(val, '', ntv_type_str)[
                     0] for key, val in ntv_value.items()}
         elif isinstance(ntv_value, NtvSingle):
             ntv_value = ntv_value.to_obj()
             return (ntv_value, ntv_name, 'ntv')
         else:
             ntv_value, name, typ_str = NtvConnector.cast(ntv_value, ntv_name)
-            ntv_type_str = Datatype.add(
-                typ_str).name if typ_str else ntv_type_str
+            ntv_type_str = Datatype(typ_str).name if typ_str else ntv_type_str
         if not ntv_type_str:
             if is_json:
                 ntv_type_str = 'json'
             else:
                 ntv_type_str = typ_str
-                if not ntv_name:
-                    ntv_name = name
         elif not is_json and ntv_type_str != typ_str:
             raise NtvError('ntv_value is not compatible with ntv_type')
+        ntv_name = name if not ntv_name else ntv_name
         return (ntv_value, ntv_name, ntv_type_str)
 
 
 class NtvList(Ntv):
     '''A NTV-list entity is a Ntv entity where:
 
     - ntv_value is a list of NTV entities,
@@ -1177,23 +1181,23 @@
         else:
             self.ntv_value.pop(self.ntv_value.index(self[ind]))
 
     def append(self, ntv):
         ''' add ntv at the end of the list of Ntv entities included'''
         old_parent = ntv.parent
         if old_parent:
-            del(old_parent[old_parent.ntv_value.index(ntv)])
+            del old_parent[old_parent.ntv_value.index(ntv)]
         self.ntv_value.append(ntv)
         ntv.parent = self
 
     def insert(self, idx, ntv):
         ''' add ntv at the index idx of the list of Ntv entities included'''
         old_parent = ntv.parent
         if old_parent:
-            del(old_parent[old_parent.ntv_value.index(ntv)])
+            del old_parent[old_parent.ntv_value.index(ntv)]
         self.ntv_value.insert(idx, ntv)
         ntv.parent = self
 
     def _obj_sep(self, json_name, json_type, def_type=None):
         ''' return separator to include in json_name'''
         sep = ':' if (json_type and json_type[-1] == '.') else '::'
         return sep if (json_type and json_type[-1] != '.') or (json_type and json_name) else ''
@@ -1206,10 +1210,10 @@
         opt2 = option | {'encoded': False}
         maxv = len(self.ntv_value) if option['maxi'] < 1 else option['maxi']
         def_type = self.ntv_type.long_name if self.ntv_type else def_type
         values = [ntv.to_obj(def_type=def_type, **opt2)
                   for ntv in self.ntv_value[:maxv]]
         if len(self) == 1 and isinstance(self[0], NtvSingle) and isinstance(values[0], dict):
             return values[0]
-        if self.json_array or option['simpleval'] or option['json_array']:
+        if not NtvUtil.is_dictable(values) or option['simpleval'] or option['json_array']:
             return values
         return {list(val.items())[0][0]: list(val.items())[0][1] for val in values}
```

### Comparing `json_ntv-1.3.0/json_ntv/ntv_comment.py` & `json_ntv-1.4.0/json_ntv/ntv_comment.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     def add(self, comment=None):
         '''add comment in the list of comments
 
         *Parameters*
 
         - **comment**: NtvPatch (default None) - new comment to apply
         '''
-        #comment = comment if isinstance(comment, (NtvPatch, NtvOp)) else NtvPatch(comment)
         self._comments.append(NtvPatch(comment))
         return len(self._comments)-1
 
     def reject(self, all_comment=False):
         '''remove the last or all comments
 
         *Parameters*
```

### Comparing `json_ntv-1.3.0/json_ntv/ntv_connector.py` & `json_ntv-1.4.0/json_ntv/ntv_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     *parameters*
 
     - **file_name** : name of the csv file
     - **single_tab** : boolean (default True) - if True return a 'tab' NtvSingle,
     else return a NtvSet.
     - **dialect, fmtparams** : parameters of csv.DictReader object'''
-    with open(file_name, newline='') as csvfile:
+    with open(file_name, newline='', encoding="utf-8") as csvfile:
         reader = csv.DictReader(csvfile, dialect=dialect, **fmtparams)
         names = reader.fieldnames
         list_ntv_value = [[] for nam in names]
         for row in reader:
             for ind_field, val in enumerate(list(row.values())):
                 list_ntv_value[ind_field].append(json.loads(val))
     list_ntv = []
@@ -70,15 +70,15 @@
     - **args, restval, extrasaction, dialect, kwds** : parameters of csv.DictWriter object'''
     if isinstance(ntv, NtvSingle):
         ntv_set = Ntv.obj(ntv.ntv_value)
     else:
         ntv_set = ntv
     list_ntv = [Ntv.obj(field) for field in ntv_set]
     fieldnames = [ntv_field.json_name(string=True) for ntv_field in list_ntv]
-    with open(file_name, 'w', newline='') as csvfile:
+    with open(file_name, 'w', newline='', encoding="utf-8") as csvfile:
         writer = csv.DictWriter(csvfile, fieldnames=fieldnames, restval=restval,
                                 extrasaction=extrasaction, dialect=dialect, *args, **kwds)
         writer.writeheader()
         for i in range(len(list_ntv[0])):
             writer.writerow({name: field_ntv[i].to_obj(field_ntv.ntv_type, encoded=True)
                              for name, field_ntv in zip(fieldnames, list_ntv)})
     return file_name
@@ -96,15 +96,15 @@
 
         *Parameters*
 
         - **type_geo** : type of geometry (point, multipoint,
         linestring, multilinestring', polygon, multipolygon)
         - **ntv_value** : array - coordinates'''
         from shapely import geometry
-        type_geo = ShapelyConnec.type_geo(ntv_value) if not 'type_geo' in kwargs \
+        type_geo = ShapelyConnec.type_geo(ntv_value) if 'type_geo' not in kwargs \
             or kwargs['type_geo'] == 'geometry' else kwargs['type_geo']
         return geometry.shape({"type": type_geo,
                                "coordinates": ntv_value})
 
     @staticmethod
     def to_json_ntv(value, name=None, typ=None):
         ''' convert NTV object (value, name, type) into NTV json (json-value, name, type).
@@ -132,15 +132,17 @@
         ''' convert geojson string into shapely geometry.'''
         from shapely import geometry
         return geometry.shape(json.loads(geojson))
 
     @staticmethod
     def to_geometry(value):
         '''convert geojson coordinates into shapely geometry'''
-        return ShapelyConnec.to_obj_ntv(value, type_geo=NtvConnector.DIC_GEO[ShapelyConnec.type_geo(value)])
+        return ShapelyConnec.to_obj_ntv(value,
+                                        type_geo=NtvConnector.DIC_GEO[
+                                            ShapelyConnec.type_geo(value)])
 
     @staticmethod
     def type_geo(value):
         '''return geometry type of the value'''
         if not value or not isinstance(value, list):
             return 'not a geometry'
         val = value[0]
@@ -367,19 +369,19 @@
         if not name:
             name = '<b>::</b>\n'
         name = name.replace('"', "'")
         return [str(ntv.pointer(index=True, item_idx=ind)),
                 ['roundedge', name[:-1]]]
 
     @staticmethod
-    def _mermaid_link(ntv, def_typ_str, node_link, row, dic_node, ind):
+    def _mermaid_link(ntv, def_typ_str, node_link, row, dic_node, indic):
         '''add nodes and links from ntv in node_link '''
         num = str(len(node_link['nodes'])) if row else ''
         node_link['nodes'].append(MermaidConnec._mermaid_node(
-            ntv, def_typ_str, num, dic_node, ind))
+            ntv, def_typ_str, num, dic_node, indic))
         if isinstance(ntv, NtvList):
             for ind, ntv_val in enumerate(ntv):
                 MermaidConnec._mermaid_link(ntv_val, ntv.type_str,
                                             node_link, row, dic_node, ind)
                 node_link['links'].append(
                     [str(ntv.pointer(index=True)), 'normalarrow',
                      str(ntv_val.pointer(index=True, item_idx=ind))])
```

### Comparing `json_ntv-1.3.0/json_ntv/ntv_patch.py` & `json_ntv-1.4.0/json_ntv/ntv_patch.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,14 @@
         if self.ope:
             txt += 'op : ' + (self.ope + ',').ljust(8, ' ')
         if self.path:
             txt += ' path : ' + str(self.path)
         if self.comment:
             txt += self.comment
         return txt
-        # return 'op : ' + (self.ope + ',').ljust(8, ' ') + ' path : ' + str(self.path)
 
     def __str__(self):
         '''return json format'''
         return json.dumps(self.json)
 
     def __eq__(self, other):
         ''' equal if all attributes are equal'''
```

### Comparing `json_ntv-1.3.0/json_ntv/ntv_util.py` & `json_ntv-1.4.0/json_ntv/ntv_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,34 +21,47 @@
     NtvUtil is the parent class of `Datatype`, `Namespace`, `Ntv`.
 
     *class variables :*
     - **_namespaces_** : list of Namespace defined
     - **_types_** : list of Datatype defined
 
     *static methods :*
+    - `is_dictable`
     - `from_obj_name`
     - `decode_ntv_tab`
     - `to_ntv_pointer`
 
     '''
     _namespaces_ = {}
     _types_ = {}
 
     @staticmethod
+    def is_dictable(lis):
+        '''check if a list can be translated in a dict'''
+        keys = set()
+        for val in lis:
+            if not isinstance(val, dict):
+                return False
+            if len(val) != 1:
+                return False
+            keys.add(list(val)[0])
+        return len(keys) == len(lis)
+
+    @staticmethod
     def from_obj_name(string):
         '''return a tuple with name, type_str and separator from string'''
         if not isinstance(string, str):
             raise NtvError('a json-name have to be str')
         if string == '':
             return (None, None, None)
         spl = string.rsplit(':', maxsplit=1)
         if len(spl) == 1:
             if string[-1] == '.':
                 return (None, string, None)
-            return(string, None, None)
+            return (string, None, None)
         if spl[0] == '':
             return (None, spl[1], ':')
         if spl[0][-1] == ':':
             sp0 = spl[0][:-1]
             return (None if sp0 == '' else sp0, None if spl[1] == '' else spl[1], '::')
         return (None if spl[0] == '' else spl[0], None if spl[1] == '' else spl[1], ':')
 
@@ -102,15 +115,15 @@
         '''convert a json pointer inter a NTV pointer (string)
 
         *parameters:*
 
         - **jsonpointer**: String - json pointer to convert,
         - **unique_root**: Boolean (default False) - True if the json root length is 1 '''
         single = '/([0-9]+)(/[a-z])'
-        if unique_root and not ('0' <= jsonpointer[1] <= '9'):
+        if unique_root and not '0' <= jsonpointer[1] <= '9':
             return re.sub(single, '\g<2>', jsonpointer)[1:]
         return re.sub(single, '\g<2>', jsonpointer)
 
 
 class NtvConnector(ABC):
     ''' The NtvConnector class is an abstract class used by all NTV connectors
     for conversion between NTV-JSON data and NTV-OBJ data.
@@ -150,14 +163,15 @@
     DIC_GEO = {'point': 'point', 'multipoint': 'multipoint', 'line': 'linestring',
                'multiline': 'multilinestring', 'polygon': 'polygon',
                'multipolygon': 'multipolygon'}
     DIC_CBOR = {'point': False, 'multipoint': False, 'line': False,
                 'multiline': False, 'polygon': False, 'multipolygon': False,
                 'date': True, 'time': False, 'datetime': True}
     DIC_OBJ = {'tab': 'DataFrameConnec', 'field': 'SeriesConnec',
+               'ndarray': 'NdarrayConnec',
                'point': 'ShapelyConnec', 'multipoint': 'ShapelyConnec',
                'line': 'ShapelyConnec', 'multiline': 'ShapelyConnec',
                'polygon': 'ShapelyConnec', 'multipolygon': 'ShapelyConnec',
                'other': None}
 
     @classmethod
     @property
@@ -254,29 +268,31 @@
 
     @staticmethod
     def uncast(value, name=None, type_str=None, **kwargs):
         '''return OBJ-NTV conversion (obj_value, name, type_str) of a NTV entity
 
         *Parameters*
 
-        - **data**: NtvSingle entity or NTVvalue of the NTV entity
+        - **value**: NtvSingle entity or NTVvalue of the NTV entity
         - **name** : String (default None) - name of the NTV entity
         - **type_str**: String (default None) - type of the NTV entity
         '''
         if type_str == 'json':
             return (value, name, type_str)
+        typebase_str = type_str
         if value.__class__.__name__ == 'NtvSingle':
             if not (type_str in set(NtvConnector.dic_type.values()) and
                     NtvConnector.is_json(value) or type_str is None):
                 return (value.ntv_value, value.name, value.type_str)
             type_str = value.type_str if value.ntv_type else None
+            typebase_str = value.typebase_str if value.ntv_type else None
             name = value.ntv_name
             value = value.ntv_value
         option = {'dicobj': {}, 'format': 'json', 'type_obj': False} | kwargs
-        value_obj = NtvConnector._uncast_val(value, type_str, **option)
+        value_obj = NtvConnector._uncast_val(value, typebase_str, **option)
         return (value_obj, name, type_str if type_str else NtvConnector._typ_obj(value_obj))
 
     @staticmethod
     def _typ_obj(value):
         if isinstance(value, dict):
             return NtvConnector._typ_obj(list(value.values()))
         if isinstance(value, (tuple, list)):
@@ -285,15 +301,20 @@
                 if typ:
                     return typ
             return None
         return NtvConnector.dic_type.get(value.__class__.__name__)
 
     @staticmethod
     def _uncast_val(value, type_n, **option):
-        '''return value from ntv value'''
+        '''return value from ntv value
+
+        *Parameters*
+
+        - **value**: NtvSingle entity or NTVvalue of the NTV entity
+        '''
         dic_fct = NtvConnector.DIC_FCT
         dic_geo = NtvConnector.DIC_GEO
         dic_obj = NtvConnector.dic_obj | option['dicobj']
         dic_cbor = NtvConnector.DIC_CBOR
         if not type_n or type_n == 'json' or (option['format'] == 'cbor' and
                                               not dic_cbor.get(type_n, False)):
             return value
@@ -388,14 +409,43 @@
         ''' return a list of keys with periodic structure'''
         if not leng:
             leng = coef * period
         return None if not (coef and period) else [(ind % (coef * period)) // coef
                                                    for ind in range(leng)]
 
     @staticmethod
+    def format_field(lidx_decode, leng):
+        ''' return a list of format'''
+        # name: 0, type: 1, codec: 2, parent: 3, keys: 4, coef: 5, leng: 6
+        field_format = []
+        for field_decode in lidx_decode:
+            name, typ, codec, parent, keys, coef, length = field_decode
+            if (keys, parent, coef) == (None, None, None):  # full or unique
+                if len(codec) == 1:  # unique
+                    field_format.append('unique')
+                elif len(codec) == leng:    # full
+                    field_format.append('full')
+                else:
+                    raise NtvError('impossible to generate keys')
+                continue
+            if keys and len(keys) > 1 and parent is None:  # complete
+                field_format.append('complete')
+                continue
+            if coef:  # primary
+                field_format.append('primary')
+                continue
+            if parent is None:
+                raise NtvError('keys not referenced')
+            if not keys:    # implicit
+                field_format.append('implicit')
+                continue
+            field_format.append('relative')
+        return field_format
+
+    @staticmethod
     def init_ntv_keys(ind, lidx, leng):
         ''' initialization of explicit keys data in lidx object of tabular data'''
         # name: 0, type: 1, codec: 2, parent: 3, keys: 4, coef: 5, leng: 6
         name, typ, codec, parent, keys, coef, length = lidx[ind]
         if (keys, parent, coef) == (None, None, None):  # full or unique
             if len(codec) == 1:  # unique
                 lidx[ind][4] = [0] * leng
```

### Comparing `json_ntv-1.3.0/json_ntv.egg-info/PKG-INFO` & `json_ntv-1.4.0/json_ntv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_ntv
-Version: 1.3.0
+Version: 1.4.0
 Summary: JSON-NTV a semantic format for interoperability
 Home-page: https://github.com/loco-philippe/NTV/blob/main/README.md
 Author: Philippe Thomy
 Author-email: philippe@loco-labs.io
 Keywords: JSON-NTV,semantic JSON,development,environmental data
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -84,21 +84,29 @@
 
 > *For example, the type: `ns1.ns2.type_a` means that:*
 >
 > - *`ns1.` is a namespace defined in the global namespace,*
 > - *`ns2.` is a namespace defined in the `ns1.` namespace.,*
 > - *`type_a` is defined in the `ns2.` namespace.*
 
+The type can be extended with additional data.
+
+> *For example, the type: `float[kg]` means that:*
+>
+> - *`float` is a main type of the data,*
+> - *`kg` is an additional type (e.g. an unit),*
+> - *`float[kg]` may represent a Quantity.*
+
 This structuring of type makes it possible to reference any type of data that has a JSON representation and to consolidate all the shared data structures within the same tree of types.
 
 ## NTV uses
 
 Several variations and use cases of the NTV format are defined:
 
-- Tabular data exchange format (e.g. open-data)
+- Tabular and multidimensional data exchange format (e.g. open-data)
 - Compact, reversible and semantic pandas-JSON interface
 - Comment and change management of JSON data
 - visualization of JSON or NTV tree
 - JSON data editor
 - data validation (value conformity to the Datatype)
 
 ## NTV and JSON
@@ -115,15 +123,15 @@
     val--->|JSON dump|text
     val--->|NTV from JSON|ntv
     ntv--->|from NTV|nat
     ntv--->|NTV to JSON|val
     nat--->|to NTV|ntv
 ```
 
-The conversion between native entity and JSON-text is reversible (round trip).
+The conversion between native entity and JSON-text is reversible (lossless round trip).
 
 ```python
 In [6]: loc_and_date = {'newyear': date(2023, 1, 2), 'Paris': Point(2.3, 48.9)}
         json_loc_date = Ntv.obj(loc_and_date).to_obj(encoded=True)
         print(json_loc_date, type(json_loc_date))
 Out[6]: {"newyear:date": "2023-01-02", "Paris:point": [2.3, 48.9]} <class 'str'>
```

### Comparing `json_ntv-1.3.0/json_ntv.egg-info/SOURCES.txt` & `json_ntv-1.4.0/json_ntv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json_ntv-1.3.0/setup.py` & `json_ntv-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="json_ntv",
-    version="1.3.0",
+    version="1.4.0",
     description="JSON-NTV a semantic format for interoperability",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/loco-philippe/NTV/blob/main/README.md",
     author="Philippe Thomy",
     author_email="philippe@loco-labs.io",
     classifiers=[
```

### Comparing `json_ntv-1.3.0/tests/test_mongo.py` & `json_ntv-1.4.0/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `json_ntv-1.3.0/tests/test_ntvstruct.py` & `json_ntv-1.4.0/tests/test_ntvstruct.py`

 * *Files identical despite different names*

### Comparing `json_ntv-1.3.0/tests/tests_namespace.py` & `json_ntv-1.4.0/tests/tests_namespace.py`

 * *Files 16% similar despite different names*

```diff
@@ -80,31 +80,36 @@
     def test_self_init(self):
         self.assertEqual(Datatype(Datatype('datetime')), Datatype('datetime'))
         
     def test_add(self):
         liststr = ['fr.BAN.lon', 'fr.BAN.$lon', 'year', 'fr.reg', 'fr.BAN.numero',
                    'fr.reg', 'fr.$IRVE.$a', '$a.$c', 'fr.$c']
         for tstr in liststr:
-            self.assertEqual(Datatype.add(tstr).long_name, tstr)
+            self.assertEqual(Datatype(tstr).long_name, tstr)
+            self.assertEqual(Datatype(tstr + '[kg]').long_name, tstr + '[kg]')
         liststr = ['$a.c.c.d', 'fr.$a.b.d']
         for tstr in liststr:
-            self.assertEqual(Datatype.add(tstr, force=True).long_name, tstr)    
+            self.assertEqual(Datatype(tstr, force=True).long_name, tstr)    
+            self.assertEqual(Datatype(tstr + '[kg]', force=True).long_name, tstr + '[kg]')
+            
     def test_add_ko(self):
         liststr = ['fr.BAN.test', 'fr', 'fr.BANN.lon']
         for tstr in liststr:
             with self.assertRaises(DatatypeError):
-                Datatype.add(tstr)        
+                Datatype(tstr)        
 
     def test_isinNamespace(self):
-        lon = Datatype.add("fr.BAN.lon")
+        lon = Datatype("fr.BAN.lon")
         listnsp = ['fr.BAN.', 'fr.', '']
         #listnotnsp = ['fr.IRVE.', 'fr.BAN.test.', 'schemaorg.']
         listnotnsp = ['fr.IRVE.', 'fr.BAN.test.']
         listkonsp = ['fr.BAN.lon', 'fr.BAN.teste.', 'fr', 'fr.BANN.test.']
         res = 0
+        self.assertEqual(Datatype("int").isin_namespace(''), 0)
+        self.assertEqual(Datatype("int[kg]").isin_namespace(''), 0)
         for nsp in listnsp:
             self.assertEqual(lon.isin_namespace(nsp), res)
             res += 1
         for nsp in listnotnsp:
             self.assertTrue(lon.isin_namespace(nsp) == -1)            
         for nsp in listkonsp:
             with self.assertRaises(DatatypeError):
@@ -112,11 +117,11 @@
  
     def test_org(self):
         liststr = ['org.House.']
         for nstr in liststr:
             self.assertEqual(Namespace.add(nstr).long_name, nstr)
         liststr = ['org.House.Country.name']
         for nstr in liststr:
-            self.assertEqual(Datatype.add(nstr).long_name, nstr)
+            self.assertEqual(Datatype(nstr).long_name, nstr)
         
 if __name__ == '__main__':
     unittest.main(verbosity=2)
```

### Comparing `json_ntv-1.3.0/tests/tests_ntv.py` & `json_ntv-1.4.0/tests/tests_ntv.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,16 +205,16 @@
                      [{"truc":  1}, "sN"],
                      [{":point": 1}, "sT"],
                      [[1, 2], {"l": ["s", "s"]}],
                      [{"truc": [1, 2]}, {"lN": ["s", "s"]}],
                      [{":point": [1, 2]}, "sT"],
                      [{"truc:":  [1, 2]}, "sN"],
                      [{":": [1, 2]}, "s"],
-                     [{"::point": [[1, 2], [3, 4]]}, {"lT": ["sT", "sT"]}],
-                     [{"::array": [[1, 2], [3, 4]]}, {"lT": ["sT", "sT"]}],
+                     [{"::point[EPSG4326]": [[1, 2], [3, 4]]}, {"lT": ["sT", "sT"]}],
+                     [{"::array[kg]": [[1, 2], [3, 4]]}, {"lT": ["sT", "sT"]}],
                      [{"::array": [{'a': 3, 'e':5}, {'a': 4, 'e':6}]}, {"lT": ["sT", "sT"]}],
                      [{"a": 2}, "sN"],
                      [{":point": {"a": 2}}, "sT"]
                      ]
         for test in list_repr:
             #print(test)
             self.assertEqual(Ntv.from_obj(test[0]).to_repr(False, False, False, 10), test[1])
```

