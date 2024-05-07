# Comparing `tmp/selenium_authenticated_proxy-1.0.1-py3-none-any.whl.zip` & `tmp/selenium_authenticated_proxy-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 5502 bytes, number of entries: 8
--rw-r--r--  2.0 unx      125 b- defN 23-Sep-08 06:35 selenium_authenticated_proxy/__init__.py
--rw-r--r--  2.0 unx     2248 b- defN 23-Sep-08 06:35 selenium_authenticated_proxy/selenium_authenticated_proxy.py
--rw-r--r--  2.0 unx     1710 b- defN 23-Sep-08 06:35 selenium_authenticated_proxy/selenium_extension_generator.py
--rw-r--r--  2.0 unx     1076 b- defN 23-Sep-08 06:36 selenium_authenticated_proxy-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2931 b- defN 23-Sep-08 06:36 selenium_authenticated_proxy-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Sep-08 06:36 selenium_authenticated_proxy-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       29 b- defN 23-Sep-08 06:36 selenium_authenticated_proxy-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      821 b- defN 23-Sep-08 06:36 selenium_authenticated_proxy-1.0.1.dist-info/RECORD
-8 files, 9032 bytes uncompressed, 4024 bytes compressed:  55.4%
+Zip file size: 6979 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      125 b- defN 24-May-07 11:23 selenium_authenticated_proxy/__init__.py
+-rw-r--r--  2.0 unx     2111 b- defN 24-May-07 11:23 selenium_authenticated_proxy/selenium_authenticated_proxy.py
+-rw-r--r--  2.0 unx     3163 b- defN 24-May-07 11:23 selenium_authenticated_proxy/selenium_extension_generator.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-07 11:23 test/__init__.py
+-rw-r--r--  2.0 unx     1699 b- defN 24-May-07 11:23 test/test_proxy.py
+-rw-r--r--  2.0 unx     1076 b- defN 24-May-07 11:23 selenium_authenticated_proxy-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3208 b- defN 24-May-07 11:23 selenium_authenticated_proxy-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 11:23 selenium_authenticated_proxy-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       34 b- defN 24-May-07 11:23 selenium_authenticated_proxy-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      966 b- defN 24-May-07 11:23 selenium_authenticated_proxy-1.1.0.dist-info/RECORD
+10 files, 12474 bytes uncompressed, 5281 bytes compressed:  57.7%
```

## zipnote {}

```diff
@@ -3,23 +3,29 @@
 
 Filename: selenium_authenticated_proxy/selenium_authenticated_proxy.py
 Comment: 
 
 Filename: selenium_authenticated_proxy/selenium_extension_generator.py
 Comment: 
 
-Filename: selenium_authenticated_proxy-1.0.1.dist-info/LICENSE
+Filename: test/__init__.py
 Comment: 
 
-Filename: selenium_authenticated_proxy-1.0.1.dist-info/METADATA
+Filename: test/test_proxy.py
 Comment: 
 
-Filename: selenium_authenticated_proxy-1.0.1.dist-info/WHEEL
+Filename: selenium_authenticated_proxy-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: selenium_authenticated_proxy-1.0.1.dist-info/top_level.txt
+Filename: selenium_authenticated_proxy-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: selenium_authenticated_proxy-1.0.1.dist-info/RECORD
+Filename: selenium_authenticated_proxy-1.1.0.dist-info/WHEEL
+Comment: 
+
+Filename: selenium_authenticated_proxy-1.1.0.dist-info/top_level.txt
+Comment: 
+
+Filename: selenium_authenticated_proxy-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## selenium_authenticated_proxy/selenium_authenticated_proxy.py

```diff
@@ -1,18 +1,23 @@
-import os
 import hashlib
+import os
+from urllib.parse import urlparse
+
+from selenium_authenticated_proxy.selenium_extension_generator import (
+    SeleniumExtensionGenerator,
+)
 
-import urllib3
-from selenium_authenticated_proxy.selenium_extension_generator import SeleniumExtensionGenerator
 
 class SeleniumAuthenticatedProxy:
     def __init__(self, proxy_url=None, tmp_folder=None):
         """Constructor for initializing proxy_url and tmp_folder."""
         self.proxy_url = proxy_url
-        self.tmp_folder = tmp_folder or os.path.abspath(os.path.join(os.path.dirname(__file__), "tmp"))
+        self.tmp_folder = tmp_folder or os.path.abspath(
+            os.path.join(os.path.dirname(__file__), "tmp")
+        )
 
     def _get_zip_filename(self):
         input_string = f"{self.proxy_url}"
 
         hasher = hashlib.sha256()
         hasher.update(input_string.encode())
 
@@ -25,37 +30,36 @@
         return f"{hex_digest}"
 
     def _get_zip_filepath(self):
         """Get the full file path for the ZIP file to be stored."""
         if not os.path.exists(self.tmp_folder):
             os.mkdir(self.tmp_folder)
         return os.path.join(self.tmp_folder, self._get_zip_filename())
-    
-    def _generate_plugin_file(self):
+
+    def _generate_plugin_file(self) -> str:
         """Generate the proxy authentication plugin ZIP file."""
-        SeleniumExtensionGenerator().generate_extension_zip(self.proxy_url, self._get_zip_filepath())
+        return SeleniumExtensionGenerator().generate_extension_zip(
+            self.proxy_url, self._get_zip_filepath()
+        )
 
-    def get_or_generate_plugin_file(self):
-        """
-        Check if the plugin file already exists.
-        If not, generate a new plugin file.
-        """
-        if not os.path.exists(self._get_zip_filepath()):
-            self._generate_plugin_file()
+    def _get_unauthenticated_url(self):
+        result = urlparse(self.proxy_url)
+        return f"{result.hostname}:{result.port}"
 
-        # Return path to plugin file
-        return self._get_zip_filepath()
+    def _get_scheme(self):
+        result = urlparse(self.proxy_url)
+        return result.scheme
 
-    def _get_unauthenticated_url(self):
-        result = urllib3.util.parse_url(self.proxy_url)
-        return f'{result.scheme}://{result.host}:{result.port}'
-    
     def _is_authenticated_url(self):
-        result = urllib3.util.parse_url(self.proxy_url)
-        return result.auth is not None
+        result = urlparse(self.proxy_url)
+        return result.username is not None
 
     def enrich_chrome_options(self, chrome_options):
         """Add the generated extension to Chrome options."""
+        if not self.proxy_url:
+            return chrome_options
         if self._is_authenticated_url():
-            chrome_options.add_argument(f"--load-extension={self.get_or_generate_plugin_file()}")
-        chrome_options.add_argument(f"--proxy-server={self._get_unauthenticated_url()}")
+            chrome_options.add_extension(self._generate_plugin_file())
+        chrome_options.add_argument(
+            f"--proxy-server={self._get_unauthenticated_url()}"
+        )
         return chrome_options
```

## selenium_authenticated_proxy/selenium_extension_generator.py

```diff
@@ -1,67 +1,120 @@
-
-from urllib.parse import urlparse
 import os
+from typing import Optional
+from urllib.parse import urlparse
+import zipfile
 
 # Thanks to https://bugs.chromium.org/p/chromium/issues/detail?id=1135492
+# Latest changes required that the proxy is specified in the extension
+# the --proxy-server flag is not enough anymore
+# https://www.browserstack.com/guide/set-proxy-in-selenium
 
 DEFAULT_MANIFEST = """
 {
     "version": "1.0.0",
     "manifest_version": 3,
     "name": "Chrome Proxy",
     "permissions": [
+        "proxy",
+        "tabs",
+        "unlimitedStorage",
+        "storage",
         "webRequest",
         "webRequestAuthProvider"
     ],
     "background": {
         "service_worker": "background.js"
     },
     "host_permissions": [
         "<all_urls>"
     ],
     "minimum_chrome_version":"22.0.0"
 }
 """
 
-DEFAULT_BACKGROUND_JS = """
+DEFAULT_BACKGROUND_JS_PROXY = """
+const config = {
+    mode: "fixed_servers",
+    rules: {
+        singleProxy: {
+            scheme: "%s",
+            host: "%s",
+            port: %s
+        }
+    }
+}
+chrome.proxy.settings.set({
+    value: config,
+    scope: 'regular'
+}, () => {});
+"""
+
+DEFAULT_BACKGROUND_AUTO_AUTH = """
 chrome.webRequest.onAuthRequired.addListener(
   (details, callback) => {
     const authCredentials = {
       username: "%s",
       password: "%s",
     };
     setTimeout(() => {
       callback({ authCredentials });
-    }, 20);
+    }, 200);
   },
   { urls: ["<all_urls>"] },
   ["asyncBlocking"]
 );
 
 """
 
 
-
 class SeleniumExtensionGenerator:
-    @classmethod
-    def generate_extension_zip(self, proxy_url=None, plugin_file_path=None):
-        os.mkdir(plugin_file_path)
-        with open(os.path.join(plugin_file_path, "manifest.json"), 'w') as f:
+    def generate_extension_zip(
+        self,
+        proxy_url: Optional[str] = None,
+        plugin_file_path: Optional[str] = None,
+    ) -> str:
+        if not plugin_file_path:
+            return
+
+        if not os.path.isdir(plugin_file_path):
+            os.makedirs(plugin_file_path)
+
+        with open(os.path.join(plugin_file_path, "manifest.json"), "w") as f:
             f.write(DEFAULT_MANIFEST)
         with open(os.path.join(plugin_file_path, "background.js"), "w") as f:
             f.write(self._get_background_js(proxy_url))
 
-    @classmethod
+        # make zip file
+        with zipfile.ZipFile(f"{plugin_file_path}.zip", "w") as zipf:
+            for root, _, files in os.walk(plugin_file_path):
+                for file in files:
+                    zipf.write(
+                        os.path.join(root, file),
+                        os.path.relpath(
+                            os.path.join(root, file), plugin_file_path
+                        ),
+                    )
+
+        return f"{plugin_file_path}.zip"
+
     def _get_background_js(self, proxy_url):
         urlparse_result = urlparse(proxy_url)
         scheme = urlparse_result.scheme
-        host = urlparse_result.hostname
         port = urlparse_result.port
         username = urlparse_result.username
         password = urlparse_result.password
         if not port:
-            if 'https' in scheme:
-                port = '443'
+            if "https" in scheme:
+                port = "443"
             else:
-                port = '80'
-        return DEFAULT_BACKGROUND_JS % (username, password)
+                port = "80"
+        BACKGROUND_JS = DEFAULT_BACKGROUND_JS_PROXY % (
+            scheme,
+            urlparse_result.hostname,
+            port,
+        )
+        if username and password:
+            BACKGROUND_JS += DEFAULT_BACKGROUND_AUTO_AUTH % (
+                username,
+                password,
+            )
+        return BACKGROUND_JS
```

## Comparing `selenium_authenticated_proxy-1.0.1.dist-info/LICENSE` & `selenium_authenticated_proxy-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `selenium_authenticated_proxy-1.0.1.dist-info/METADATA` & `selenium_authenticated_proxy-1.1.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-authenticated-proxy
-Version: 1.0.1
+Version: 1.1.0
 Summary: A python package to add authenticated proxy support to selenium.
 Home-page: https://github.com/bubblegumsoldier/selenium-authenticated-proxy
 Author: Henry Müssemann
 Author-email: hm@freezingdata.de
 License: MIT
 Keywords: proxy,selenium,auth,selenium
 Platform: UNKNOWN
@@ -70,14 +70,22 @@
 ```python
 proxy_helper = SeleniumAuthenticatedProxy(proxy_url="http://username:password@proxy-server.com", tmp_folder="/path/to/tmp/folder")
 ```
 
 To enable the authentication to work properly a chrome extension is being generated (Thanks to [itsmnthn](https://stackoverflow.com/a/55582859/3691763) with an [improvement for manifest v3](https://bugs.chromium.org/p/chromium/issues/detail?id=1135492)).
 If the URl doesn't change the extension will not be regenerated. The URL is hashed so that only when the URL has changed (or the tmp folder has changed) a new zip file will be generated.
 
+### Specific issues with headless chrome
+
+If you want to use headless chrome, this functionality only works if you use the following method:
+
+```python
+ops.add_argument('--headless=new')
+```
+
+The `--headless` method or also the `--headless=chrome` method does not work anymore!
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE.md file for details.
 
 
-
```

## Comparing `selenium_authenticated_proxy-1.0.1.dist-info/RECORD` & `selenium_authenticated_proxy-1.1.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 selenium_authenticated_proxy/__init__.py,sha256=G3TCTIpfeaMSW8sGgEms5tTjJ7X6N9LMIE3YfAFOyQk,125
-selenium_authenticated_proxy/selenium_authenticated_proxy.py,sha256=9h0aPbiVZaGzEaoLFjpTc0Vcz5Z_EO9ptbPWU8ny6eE,2248
-selenium_authenticated_proxy/selenium_extension_generator.py,sha256=Sgp-zlaeaXyjkgbhw1vOYLx8M5MmQyAiHenFd0dHId8,1710
-selenium_authenticated_proxy-1.0.1.dist-info/LICENSE,sha256=bhs5U3qqHxnr1T_NkQbie2dwXfWZLJdvzJvXfu__GlU,1076
-selenium_authenticated_proxy-1.0.1.dist-info/METADATA,sha256=3ZV9yh-qvVu0bakt2mZD34fMceEGZUGMCI2fAp8Dc1w,2931
-selenium_authenticated_proxy-1.0.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-selenium_authenticated_proxy-1.0.1.dist-info/top_level.txt,sha256=8UbRMzKTZ4Nze-K5XPp-qalZ_Z30dJMzHAx3SY9IdBA,29
-selenium_authenticated_proxy-1.0.1.dist-info/RECORD,,
+selenium_authenticated_proxy/selenium_authenticated_proxy.py,sha256=xuC_Mxy7CxHdgodJ6b0SCLXOsfjsTtZLYzxoPUP5eSo,2111
+selenium_authenticated_proxy/selenium_extension_generator.py,sha256=yOJnidQ3fwmVN9wPvm1gczA3T2MV5JFmX15_USlCDlk,3163
+test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+test/test_proxy.py,sha256=BUIs0fthkAealjqyazzWt8kBGAp9CKe7MNNwgbspGi4,1699
+selenium_authenticated_proxy-1.1.0.dist-info/LICENSE,sha256=bhs5U3qqHxnr1T_NkQbie2dwXfWZLJdvzJvXfu__GlU,1076
+selenium_authenticated_proxy-1.1.0.dist-info/METADATA,sha256=YEHnaU1ZyZEpioilmJTboRLP-Hvg-TEFkWc1HjO5ync,3208
+selenium_authenticated_proxy-1.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+selenium_authenticated_proxy-1.1.0.dist-info/top_level.txt,sha256=GjQaO_8ocTo1xFNJ6rIqnC5SlVTfZkbI-3QK6ZNQSHM,34
+selenium_authenticated_proxy-1.1.0.dist-info/RECORD,,
```

