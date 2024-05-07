# Comparing `tmp/transmission_rpc-7.0.4.tar.gz` & `tmp/transmission_rpc-7.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transmission_rpc-7.0.4.tar", max compression
+gzip compressed data, was "transmission_rpc-7.0.5.tar", max compression
```

## Comparing `transmission_rpc-7.0.4.tar` & `transmission_rpc-7.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1127 2024-04-30 20:39:54.562527 transmission_rpc-7.0.4/LICENSE
--rw-r--r--   0        0        0     2277 2024-04-30 20:39:54.562527 transmission_rpc-7.0.4/README.md
--rw-r--r--   0        0        0     3091 2024-04-30 20:39:54.562527 transmission_rpc-7.0.4/pyproject.toml
--rw-r--r--   0        0        0     1893 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/__init__.py
--rw-r--r--   0        0        0    43856 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/client.py
--rw-r--r--   0        0        0    10069 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/constants.py
--rw-r--r--   0        0        0     1640 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/error.py
--rw-r--r--   0        0        0        0 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/py.typed
--rw-r--r--   0        0        0    12493 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/session.py
--rw-r--r--   0        0        0    23203 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/torrent.py
--rw-r--r--   0        0        0     1484 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/types.py
--rw-r--r--   0        0        0     2669 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/utils.py
--rw-r--r--   0        0        0     3412 1970-01-01 00:00:00.000000 transmission_rpc-7.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1127 2024-05-07 03:54:42.274685 transmission_rpc-7.0.5/LICENSE
+-rw-r--r--   0        0        0     2277 2024-05-07 03:54:42.274685 transmission_rpc-7.0.5/README.md
+-rw-r--r--   0        0        0     3107 2024-05-07 03:54:42.274685 transmission_rpc-7.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1893 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/__init__.py
+-rw-r--r--   0        0        0    44327 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/client.py
+-rw-r--r--   0        0        0    10069 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/constants.py
+-rw-r--r--   0        0        0     1640 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/error.py
+-rw-r--r--   0        0        0        0 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/py.typed
+-rw-r--r--   0        0        0    12506 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/session.py
+-rw-r--r--   0        0        0    23193 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/torrent.py
+-rw-r--r--   0        0        0     1866 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/types.py
+-rw-r--r--   0        0        0     2669 2024-05-07 03:54:42.278685 transmission_rpc-7.0.5/transmission_rpc/utils.py
+-rw-r--r--   0        0        0     3412 1970-01-01 00:00:00.000000 transmission_rpc-7.0.5/PKG-INFO
```

### Comparing `transmission_rpc-7.0.4/LICENSE` & `transmission_rpc-7.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.4/README.md` & `transmission_rpc-7.0.5/README.md`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.4/pyproject.toml` & `transmission_rpc-7.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "transmission-rpc"
-version = "7.0.4"
+version = "7.0.5"
 description = "Python module that implements the Transmission bittorent client JSON-RPC protocol"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'README.md'
 repository = 'https://github.com/Trim21/transmission-rpc'
 license = 'MIT'
 packages = [{ include = 'transmission_rpc' }]
 keywords = ['transmission', 'rpc']
@@ -30,15 +30,15 @@
 python = "^3.8"
 # dependencies
 requests = "^2.23.0"
 typing-extensions = "*"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = { version = "^7.0.0", python = "^3.9" }
-furo = { version = "2024.4.27", python = "^3.9" }
+furo = { version = "2024.5.6", python = "^3.9" }
 
 [tool.poetry.group.dev.dependencies]
 yarl = "==1.9.4"
 # tests
 pytest = "==8.2.0"
 pytest-github-actions-annotate-failures = "==0.2.0"
 coverage = "==7.5.0"
@@ -78,16 +78,19 @@
 
 [tool.black]
 line-length = 120
 target-version = ['py38']
 
 
 [tool.ruff]
+target-version = "py38"
 extend-exclude = ["docs"]
 line-length = 120
+
+[tool.ruff.lint]
 select = [
     "B",
     "C",
     "E",
     "F",
     "G",
     "I",
@@ -146,9 +149,7 @@
     'TRY201',
     'TRY301',
     'PLR0912',
     'PLR0915',
     'PLR2004',
     'PGH003',
 ]
-
-target-version = "py38"
```

### Comparing `transmission_rpc-7.0.4/transmission_rpc/__init__.py` & `transmission_rpc-7.0.5/transmission_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.4/transmission_rpc/client.py` & `transmission_rpc-7.0.5/transmission_rpc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1083,19 +1083,30 @@
 
     def set_group(
         self,
         name: str,
         *,
         timeout: Optional[_Timeout] = None,
         honors_session_limits: Optional[bool] = None,
+        speed_limit_down_enabled: Optional[bool] = None,
         speed_limit_down: Optional[int] = None,
         speed_limit_up_enabled: Optional[bool] = None,
         speed_limit_up: Optional[int] = None,
-        speed_limit_down_enabled: Optional[bool] = None,
     ) -> None:
+        """create or update a Bandwidth group.
+
+        :param name: Bandwidth group name
+        :param honors_session_limits: true if session upload limits are honored
+        :param speed_limit_down_enabled: true means enabled
+        :param speed_limit_down: 	max global download speed (KBps)
+        :param speed_limit_up_enabled: 	true means enabled
+        :param speed_limit_up: max global upload speed (KBps)
+        :param timeout: request timeout
+        """
+
         self._rpc_version_warning(17)
         arguments: Dict[str, Any] = remove_unset_value(
             {
                 "name": name,
                 "honorsSessionLimits": honors_session_limits,
                 "speed-limit-down": speed_limit_down,
                 "speed-limit-up-enabled": speed_limit_up_enabled,
```

### Comparing `transmission_rpc-7.0.4/transmission_rpc/constants.py` & `transmission_rpc-7.0.5/transmission_rpc/constants.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.4/transmission_rpc/error.py` & `transmission_rpc-7.0.5/transmission_rpc/error.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.4/transmission_rpc/session.py` & `transmission_rpc-7.0.5/transmission_rpc/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     Session is a class holding the session data for a Transmission daemon.
 
     Access the session field can be done through attributes.
     The attributes available are the same as the session arguments in the
     Transmission RPC specification, but with underscore instead of hyphen.
 
 
-    get ``'download-dir'`` with ``session.download_dir``.
+    You should use ``session.download_dir`` to get ``'download-dir'``.
 
     .. code-block:: python
 
         session = Client().get_session()
 
         current = session.download_dir
 
@@ -344,15 +344,15 @@
     def trash_original_torrent_files(self) -> bool:
         """true means the .torrent file of added torrents will be deleted"""
         return self.fields["trash-original-torrent-files"]
 
     # see below
     @property
     def units(self) -> Units:
-        return self.fields["units"]
+        return Units(fields=self.fields["units"])
 
     @property
     def utp_enabled(self) -> bool:
         """true means allow utp"""
         return self.fields["utp-enabled"]
 
     @property
@@ -378,15 +378,15 @@
         new at rpc-version 17
         """
         return self.get("rpc-version-semver")
 
     @property
     def script_torrent_added_enabled(self) -> Optional[bool]:
         """
-        whether or not to call the `added` script
+        whether to call the `added` script
         new at rpc-version 17
         """
         return self.get("script-torrent-added-enabled")
 
     @property
     def script_torrent_added_filename(self) -> Optional[str]:
         """
@@ -394,15 +394,15 @@
         new at rpc-version 17
         """
         return self.get("script-torrent-added-filename")
 
     @property
     def script_torrent_done_seeding_enabled(self) -> Optional[bool]:
         """
-        whether or not to call the `seeding-done` script
+        whether to call the `seeding-done` script
         new at rpc-version 17
         """
         return self.get("script-torrent-done-seeding-enabled")
 
     @property
     def script_torrent_done_seeding_filename(self) -> Optional[str]:
         """
```

### Comparing `transmission_rpc-7.0.4/transmission_rpc/torrent.py` & `transmission_rpc-7.0.5/transmission_rpc/torrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
         """
         Byte count of all the piece data we want and don't have yet,
         but that a connected peer does have. [0...leftUntilDone]
         """
         return self.fields["desiredAvailable"]
 
     @property
-    def download_dir(self) -> Optional[str]:
+    def download_dir(self) -> str:
         """The download directory.
 
         :available: transmission version 1.5.
         :available: RPC version 4.
         """
         return self.fields["downloadDir"]
```

### Comparing `transmission_rpc-7.0.4/transmission_rpc/types.py` & `transmission_rpc-7.0.5/transmission_rpc/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,30 +25,40 @@
     completed: int  # bytes completed
     priority: Priority
     selected: bool  # if selected for download
     id: int  # id of the file of this torrent, not should not be used outside the torrent scope.
 
 
 class Group(Container):
+    """
+    https://github.com/transmission/transmission/blob/4.0.5/docs/rpc-spec.md#482-bandwidth-group-accessor-group-get
+    """
+
     @property
     def name(self) -> str:
+        """Bandwidth group name"""
         return self.fields["name"]
 
     @property
     def honors_session_limits(self) -> bool:
+        """true if session upload limits are honored"""
         return self.fields["honorsSessionLimits"]
 
     @property
     def speed_limit_down_enabled(self) -> bool:
+        """true means enabled"""
         return self.fields["speed-limit-down-enabled"]
 
     @property
     def speed_limit_down(self) -> int:
+        """max global download speed (KBps)"""
         return self.fields["speed-limit-down"]
 
     @property
     def speed_limit_up_enabled(self) -> bool:
+        """true means enabled"""
         return self.fields["speed-limit-up-enabled"]
 
     @property
     def speed_limit_up(self) -> int:
+        """max global upload speed (KBps)"""
         return self.fields["speed-limit-up"]
```

### Comparing `transmission_rpc-7.0.4/transmission_rpc/utils.py` & `transmission_rpc-7.0.5/transmission_rpc/utils.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.4/PKG-INFO` & `transmission_rpc-7.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transmission-rpc
-Version: 7.0.4
+Version: 7.0.5
 Summary: Python module that implements the Transmission bittorent client JSON-RPC protocol
 Home-page: https://github.com/Trim21/transmission-rpc
 License: MIT
 Keywords: transmission,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
```

