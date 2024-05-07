# Comparing `tmp/adls_acl-0.0.7.tar.gz` & `tmp/adls_acl-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adls_acl-0.0.7.tar", last modified: Mon May  6 08:22:21 2024, max compression
+gzip compressed data, was "adls_acl-0.1.0.tar", last modified: Tue May  7 12:15:00 2024, max compression
```

## Comparing `adls_acl-0.0.7.tar` & `adls_acl-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:22:21.477711 adls_acl-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-06 08:22:09.000000 adls_acl-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 08:22:09.000000 adls_acl-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-05-06 08:22:21.477711 adls_acl-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-06 08:22:09.000000 adls_acl-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-06 08:22:09.000000 adls_acl-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:22:21.477711 adls_acl-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-06 08:22:09.000000 adls_acl-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:22:21.473711 adls_acl-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:22:21.477711 adls_acl-0.0.7/src/adls_acl/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:22:21.477711 adls_acl-0.0.7/src/adls_acl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-05-06 08:22:21.000000 adls_acl-0.0.7/src/adls_acl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-06 08:22:21.000000 adls_acl-0.0.7/src/adls_acl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:22:21.000000 adls_acl-0.0.7/src/adls_acl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 08:22:21.000000 adls_acl-0.0.7/src/adls_acl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 08:22:21.000000 adls_acl-0.0.7/src/adls_acl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 08:22:21.000000 adls_acl-0.0.7/src/adls_acl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:22:21.477711 adls_acl-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-06 08:22:09.000000 adls_acl-0.0.7/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-06 08:22:09.000000 adls_acl-0.0.7/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-06 08:22:09.000000 adls_acl-0.0.7/tests/test_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:15:00.503424 adls_acl-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-07 12:14:55.000000 adls_acl-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 12:14:55.000000 adls_acl-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-05-07 12:15:00.503424 adls_acl-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-07 12:14:55.000000 adls_acl-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-07 12:14:55.000000 adls_acl-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 12:15:00.503424 adls_acl-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-07 12:14:55.000000 adls_acl-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:15:00.499424 adls_acl-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:15:00.499424 adls_acl-0.1.0/src/adls_acl/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 12:14:55.000000 adls_acl-0.1.0/src/adls_acl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-07 12:14:55.000000 adls_acl-0.1.0/src/adls_acl/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-07 12:14:55.000000 adls_acl-0.1.0/src/adls_acl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-07 12:14:55.000000 adls_acl-0.1.0/src/adls_acl/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-07 12:14:55.000000 adls_acl-0.1.0/src/adls_acl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-07 12:14:55.000000 adls_acl-0.1.0/src/adls_acl/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-05-07 12:14:55.000000 adls_acl-0.1.0/src/adls_acl/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 12:14:55.000000 adls_acl-0.1.0/src/adls_acl/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:15:00.503424 adls_acl-0.1.0/src/adls_acl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-05-07 12:15:00.000000 adls_acl-0.1.0/src/adls_acl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-07 12:15:00.000000 adls_acl-0.1.0/src/adls_acl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:15:00.000000 adls_acl-0.1.0/src/adls_acl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 12:15:00.000000 adls_acl-0.1.0/src/adls_acl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 12:15:00.000000 adls_acl-0.1.0/src/adls_acl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 12:15:00.000000 adls_acl-0.1.0/src/adls_acl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:15:00.503424 adls_acl-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 12:14:55.000000 adls_acl-0.1.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-07 12:14:55.000000 adls_acl-0.1.0/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-07 12:14:55.000000 adls_acl-0.1.0/tests/test_orchestrator.py
```

### Comparing `adls_acl-0.0.7/LICENSE` & `adls_acl-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.7/PKG-INFO` & `adls_acl-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adls_acl
-Version: 0.0.7
+Version: 0.1.0
 Summary: A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).
 Home-page: https://github.com/karolusz/adls-acl
 Author: Karol Luszczek
 Author-email: karol.luszczek@reinsight.se
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -212,15 +212,16 @@
 A list of objects describing subdirectories.
 
 #### Acl - definition
 ```yaml
 oid: string. # Required. Security principal Object ID in Microsoft Entra ID.
 type: string # Required. Security principal type.
 acl: string 
-scope: string. 
+scope: string
+recursive: bool
 ```
 `oid` string. Required.
 Object ID of the principal (user/group/managed identity/service principal) in Microsoft Entra (former Azure Active Directory).
 
 `type` string. Required.
 Type of the service principal. Allowed values: `user` (for users, service principals, and managed identities), `group` (for Entra ID groups), `other` (for all other users ACLs), `mask` (for setting masks on directories)
 
@@ -228,14 +229,17 @@
 A string defining desired permissions in the short form. [MS DOCS: ADLS ACLs](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-access-control)
 e.g.:
 `r--` for read-only permissions
 
 `scope` string. Optional
 If set to `default` it will set the specified ACLs as `default ACLs` [MS DOCS: Types of ACLs](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-access-control#types-of-acls). If not present, ACLs will be set as `access ACLs`.
 
+`recursive` bool. Optional
+If set to `True` that ACL will be applied recursively to every subdirectroy and file inside the directory this ACL is to be set on.
+
 #### Special ACLs
 
 `adls-acl` also allows for managing ACLs for owning user, owning group, all other users, as well as setting masks. Examples of how to specify each of the above, in the `adls-acl` YAML input file (as [acl](#acl---definition) block) are provided below:
 
 - owning user
 ```yaml
 oid: ""
@@ -267,14 +271,15 @@
 
 The default ACLs defined or set on the higher level directories are pushed down to subdirectories specified in the input file.
 They will not be set on any files that had existed in the directories prior to the execution of `adls-acl`.
 Moreover, any subdirectories that exist in the account but are not specified in the input file remain untouched by `adls-acl`.
 
 Future releases will allow for more control over this behaviour (i.e, updating default ACLs on all files created prior to the change of ACLs).
 
+
 ### Authentication Methods
 
 The Azure Python SDK authentication is by default handled with [`DefaultAzureCredenial`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential?view=azure-python).
 
 In addition, a user can target one of the supported Azure Python SDK, by using `--auth-method` option:
 
 - [`EnvironmentCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential?view=azure-python)
```

### Comparing `adls_acl-0.0.7/README.md` & `adls_acl-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -185,15 +185,16 @@
 A list of objects describing subdirectories.
 
 #### Acl - definition
 ```yaml
 oid: string. # Required. Security principal Object ID in Microsoft Entra ID.
 type: string # Required. Security principal type.
 acl: string 
-scope: string. 
+scope: string
+recursive: bool
 ```
 `oid` string. Required.
 Object ID of the principal (user/group/managed identity/service principal) in Microsoft Entra (former Azure Active Directory).
 
 `type` string. Required.
 Type of the service principal. Allowed values: `user` (for users, service principals, and managed identities), `group` (for Entra ID groups), `other` (for all other users ACLs), `mask` (for setting masks on directories)
 
@@ -201,14 +202,17 @@
 A string defining desired permissions in the short form. [MS DOCS: ADLS ACLs](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-access-control)
 e.g.:
 `r--` for read-only permissions
 
 `scope` string. Optional
 If set to `default` it will set the specified ACLs as `default ACLs` [MS DOCS: Types of ACLs](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-access-control#types-of-acls). If not present, ACLs will be set as `access ACLs`.
 
+`recursive` bool. Optional
+If set to `True` that ACL will be applied recursively to every subdirectroy and file inside the directory this ACL is to be set on.
+
 #### Special ACLs
 
 `adls-acl` also allows for managing ACLs for owning user, owning group, all other users, as well as setting masks. Examples of how to specify each of the above, in the `adls-acl` YAML input file (as [acl](#acl---definition) block) are provided below:
 
 - owning user
 ```yaml
 oid: ""
@@ -240,14 +244,15 @@
 
 The default ACLs defined or set on the higher level directories are pushed down to subdirectories specified in the input file.
 They will not be set on any files that had existed in the directories prior to the execution of `adls-acl`.
 Moreover, any subdirectories that exist in the account but are not specified in the input file remain untouched by `adls-acl`.
 
 Future releases will allow for more control over this behaviour (i.e, updating default ACLs on all files created prior to the change of ACLs).
 
+
 ### Authentication Methods
 
 The Azure Python SDK authentication is by default handled with [`DefaultAzureCredenial`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential?view=azure-python).
 
 In addition, a user can target one of the supported Azure Python SDK, by using `--auth-method` option:
 
 - [`EnvironmentCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential?view=azure-python)
```

### Comparing `adls_acl-0.0.7/pyproject.toml` & `adls_acl-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.0.7"
+current_version = "0.1.0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `adls_acl-0.0.7/setup.py` & `adls_acl-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 readme = open("README.md", encoding="utf-8").read()
 
 setup(
     name="adls_acl",
-    version="0.0.7",
+    version="0.1.0",
     url="https://github.com/karolusz/adls-acl",
     author="Karol Luszczek",
     author_email="karol.luszczek@reinsight.se",
     description="A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `adls_acl-0.0.7/src/adls_acl/auth.py` & `adls_acl-0.1.0/src/adls_acl/auth.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.7/src/adls_acl/cli.py` & `adls_acl-0.1.0/src/adls_acl/cli.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.7/src/adls_acl/input_parser.py` & `adls_acl-0.1.0/src/adls_acl/input_parser.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.7/src/adls_acl/logger.py` & `adls_acl-0.1.0/src/adls_acl/logger.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.7/src/adls_acl/nodes.py` & `adls_acl-0.1.0/src/adls_acl/nodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 @dataclass
 class Acl:
     p_type: str
     oid: str
     permissions: str
     scope: Optional[str] = None
+    recursive: Optional[bool] = False
 
     @classmethod
     def from_str(cls, acl_str: str):
         """Returns an instance of Acl from string from get_access_control call"""
         acl_str = acl_str.split(":")
         if len(acl_str) == 3:
             p_type, oid, permissions = acl_str
@@ -19,22 +20,26 @@
         elif len(acl_str) == 4:
             scope, p_type, oid, permissions = acl_str
             return Acl(p_type, oid, permissions, scope=scope)
 
     @classmethod
     def from_dict(cls, acl_dict: Dict):
         """Returns an instance of Acl from a dict from yaml input"""
+        recursive = False
+        scope = None
         if "acl" in acl_dict:
             acl = acl_dict["acl"]
         if "scope" in acl_dict:
             scope = acl_dict["scope"]
-        else:
-            scope = None
+        if "recursive" in acl_dict:
+            recursive = acl_dict["recursive"]
 
-        acl = Acl(acl_dict["type"], acl_dict["oid"], acl, scope=scope)
+        acl = Acl(
+            acl_dict["type"], acl_dict["oid"], acl, scope=scope, recursive=recursive
+        )
         return acl
 
     def __str__(self):
         if self.scope is None:
             s = f"{self.p_type}:{self.oid}:{self.permissions}"
         else:
             s = f"{self.scope}:{self.p_type}:{self.oid}:{self.permissions}"
@@ -81,14 +86,18 @@
                     self.is_mask(),
                     self.is_other(),
                 ]
             )
             else False
         )
 
+    def is_recursive(self):
+        """Check if the ACL is supposed to be applied recursively"""
+        return self.recursive
+
     def to_yaml(self):
         """Returns a dict reprentaion"""
         data = {
             "oid": self.oid,
             "type": self.p_type,
             "acl": self.permissions,
         }
```

### Comparing `adls_acl-0.0.7/src/adls_acl/orchestrator.py` & `adls_acl-0.1.0/src/adls_acl/orchestrator.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,19 +17,32 @@
     def __init__(
         self, account_name: str, auth_method: str = "default", **auth_kwargs: Any
     ):
         self.sc = get_service_client(account_name, auth_method, **auth_kwargs)
         self.account_name = account_name
 
     def process_tree(self, root):
+        # First pass to set non-recursive ACLs and materialzie new nodes
+        # in the account
         for node in bfs(root):
+            log.info("PROCESSING NODE ===========")
+            log.info(node)
             processor = processor_selector(node)
             dc = processor.get_dir_client(node, self.sc)
             processor.set_acls(node, dc)
 
+        # Second pass to set recursive ACLs
+        for node in bfs(root):
+            processor = processor_selector(node)
+            if any([acl.is_recursive() for acl in node.acls]):
+                log.info("Applying recursive ACLs")
+                log.info(f"Path to node: {node.path}")
+                dc = processor.get_dir_client(node, self.sc)
+                processor.update_acls_recursive(node, dc)
+
     def read_account(self, omit_special: bool = False) -> Dict:
         data = {}
         data["account"] = self.account_name
         data["containers"] = []
         for container in self.sc.list_file_systems():
             # Create a root node
             fc = self.sc.get_file_system_client(container)
@@ -59,17 +72,17 @@
     @abstractmethod
     def get_access_control(): ...
 
     @staticmethod
     @abstractmethod
     def set_access_control(): ...
 
-    # Not needed until update mode is implemented
-    # @abstractmethod
-    # def update_permissions_recursively(): ...
+    @staticmethod
+    @abstractmethod
+    def update_access_control_recursive(): ...
 
 
 def _filter_acls_to_preserve(current_acls: Set[Acl]) -> Set[Acl]:
     """Determines which ACLs in the current Node should be preserved in the update"""
     acls_to_preserve = set()
 
     for acl in current_acls:
@@ -100,14 +113,31 @@
 
 def _pushdown_acls(node: Node, acls: Set[Acl]) -> None:
     """Pushdown selected ACLs to the children of the node"""
     for child_node in node.children:
         child_node.acls.update(acls)
 
 
+def _update_access_control_recursive(
+    client: DataLakeDirectoryClient, acls: Set[Acl], retries: int = 3
+) -> None:
+    """Update ACLs. The easiest way to apply ACLs recusively.
+    https://learn.microsoft.com/en-us/python/api/azure-storage-file-datalake/azure.storage.filedatalake.datalakedirectoryclient?view=azure-python#azure-storage-filedatalake-datalakedirectoryclient-update-access-control-recursive
+    """
+    for acl in acls:
+        continuation_token = None
+        for i in range(0, retries):
+            change_result = client.update_access_control_recursive(
+                acl=acl, continue_on_failure=True, continuation_token=continuation_token
+            )
+            continuation_token = change_result.get("continue")
+            if continuation_token is None:
+                break
+
+
 class Processor(ABC):
     @staticmethod
     @abstractmethod
     def set_acls(node: Node, client: DataLakeDirectoryClient):
         # Get current ACLs to preseve ACLs for
         # Owner, Owner Group, mask, and other
         # they will only change if specifie in input
@@ -122,27 +152,30 @@
         _set_acls(client, new_acls)
         _pushdown_acls(node, acls_to_pushdown)
 
     @staticmethod
     @abstractmethod
     def get_dir_client() -> ClientWithACLSupport: ...
 
-    # @staticmethod
-    # @abstractmethod
-    # def update_acls(): ...
+    @staticmethod
+    @abstractmethod
+    def update_acls_recursive(node: Node, client: DataLakeDirectoryClient) -> None:
+        recursive_acls = set([acl for acl in node.acls if acl.is_recursive()])
+        log.info("Recursive Acls:")
+        for acl in recursive_acls:
+            log.info(f"\t {acl}")
+        _update_access_control_recursive(client, recursive_acls, retries=3)
 
 
 class ProcessorRoot(Processor):
 
     @staticmethod
     def get_dir_client(node: Node, client: DataLakeServiceClient):
         """Creates a container if it doesn't exist and returns a file clietn
         to its root directory."""
-        log.info("PROCESSING NODE ===========")
-        log.info(node)
         if node.is_root == False:
             raise ValueError("Node is not the root!")
 
         try:
             fs_client = client.create_file_system(node.name)
         except ResourceExistsError:
             fs_client = client.get_file_system_client(file_system=node.name)
@@ -150,41 +183,40 @@
         return fs_client._get_root_directory_client()
 
     @staticmethod
     def set_acls(node: Node, client: DataLakeDirectoryClient):
         super(ProcessorRoot, ProcessorRoot).set_acls(node, client)
         client.close()
 
-    # @staticmethod
-    # def update_acls():
-    #    pass
+    @staticmethod
+    def update_acls_recursive(node: Node, client: DataLakeDirectoryClient):
+        super(ProcessorRoot, ProcessorRoot).update_acls_recursive(node, client)
+        client.close()
 
 
 class ProcessorDir(Processor):
 
     @staticmethod
     def get_dir_client(node: Node, client: DataLakeServiceClient):
         """Creates a directory, if it doesn't exist and returns a directory
         client."""
-        log.info("PROCESSING NODE ===========")
-        log.info(node)
-
         folder_client = client.get_file_system_client(file_system=node.get_root().name)
         dir_client = folder_client.get_directory_client(node.path_in_file_system)
         dir_client.create_directory()
 
         return dir_client
 
     @staticmethod
     def set_acls(node: Node, client: DataLakeDirectoryClient):
         super(ProcessorDir, ProcessorDir).set_acls(node, client)
 
-    # @staticmethod
-    # def update_acls():
-    #    pass
+    @staticmethod
+    def update_acls_recursive(node: Node, client: DataLakeDirectoryClient):
+        super(ProcessorDir, ProcessorDir).update_acls_recursive(node, client)
+        client.close()
 
 
 def processor_selector(node):
     if node.is_root:
         return ProcessorRoot()
     else:
         return ProcessorDir()
```

### Comparing `adls_acl-0.0.7/src/adls_acl.egg-info/PKG-INFO` & `adls_acl-0.1.0/src/adls_acl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adls_acl
-Version: 0.0.7
+Version: 0.1.0
 Summary: A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).
 Home-page: https://github.com/karolusz/adls-acl
 Author: Karol Luszczek
 Author-email: karol.luszczek@reinsight.se
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -212,15 +212,16 @@
 A list of objects describing subdirectories.
 
 #### Acl - definition
 ```yaml
 oid: string. # Required. Security principal Object ID in Microsoft Entra ID.
 type: string # Required. Security principal type.
 acl: string 
-scope: string. 
+scope: string
+recursive: bool
 ```
 `oid` string. Required.
 Object ID of the principal (user/group/managed identity/service principal) in Microsoft Entra (former Azure Active Directory).
 
 `type` string. Required.
 Type of the service principal. Allowed values: `user` (for users, service principals, and managed identities), `group` (for Entra ID groups), `other` (for all other users ACLs), `mask` (for setting masks on directories)
 
@@ -228,14 +229,17 @@
 A string defining desired permissions in the short form. [MS DOCS: ADLS ACLs](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-access-control)
 e.g.:
 `r--` for read-only permissions
 
 `scope` string. Optional
 If set to `default` it will set the specified ACLs as `default ACLs` [MS DOCS: Types of ACLs](https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-access-control#types-of-acls). If not present, ACLs will be set as `access ACLs`.
 
+`recursive` bool. Optional
+If set to `True` that ACL will be applied recursively to every subdirectroy and file inside the directory this ACL is to be set on.
+
 #### Special ACLs
 
 `adls-acl` also allows for managing ACLs for owning user, owning group, all other users, as well as setting masks. Examples of how to specify each of the above, in the `adls-acl` YAML input file (as [acl](#acl---definition) block) are provided below:
 
 - owning user
 ```yaml
 oid: ""
@@ -267,14 +271,15 @@
 
 The default ACLs defined or set on the higher level directories are pushed down to subdirectories specified in the input file.
 They will not be set on any files that had existed in the directories prior to the execution of `adls-acl`.
 Moreover, any subdirectories that exist in the account but are not specified in the input file remain untouched by `adls-acl`.
 
 Future releases will allow for more control over this behaviour (i.e, updating default ACLs on all files created prior to the change of ACLs).
 
+
 ### Authentication Methods
 
 The Azure Python SDK authentication is by default handled with [`DefaultAzureCredenial`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential?view=azure-python).
 
 In addition, a user can target one of the supported Azure Python SDK, by using `--auth-method` option:
 
 - [`EnvironmentCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential?view=azure-python)
```

### Comparing `adls_acl-0.0.7/src/adls_acl.egg-info/SOURCES.txt` & `adls_acl-0.1.0/src/adls_acl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.7/tests/test_auth.py` & `adls_acl-0.1.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.7/tests/test_nodes.py` & `adls_acl-0.1.0/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.7/tests/test_orchestrator.py` & `adls_acl-0.1.0/tests/test_orchestrator.py`

 * *Files identical despite different names*

