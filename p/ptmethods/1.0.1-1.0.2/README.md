# Comparing `tmp/ptmethods-1.0.1.tar.gz` & `tmp/ptmethods-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptmethods-1.0.1.tar", last modified: Fri Aug  4 11:21:12 2023, max compression
+gzip compressed data, was "ptmethods-1.0.2.tar", last modified: Tue May  7 11:43:25 2024, max compression
```

## Comparing `ptmethods-1.0.1.tar` & `ptmethods-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:21:12.462381 ptmethods-1.0.1/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35823 2023-02-16 20:42:08.000000 ptmethods-1.0.1/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3939 2023-08-04 11:21:12.462381 ptmethods-1.0.1/PKG-INFO
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3485 2023-08-04 11:17:17.000000 ptmethods-1.0.1/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:21:12.462381 ptmethods-1.0.1/ptmethods/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-16 20:42:08.000000 ptmethods-1.0.1/ptmethods/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-07-31 19:38:27.000000 ptmethods-1.0.1/ptmethods/_version.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    14564 2023-07-31 19:38:43.000000 ptmethods-1.0.1/ptmethods/ptmethods.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:21:12.462381 ptmethods-1.0.1/ptmethods.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3939 2023-08-04 11:21:12.000000 ptmethods-1.0.1/ptmethods.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      293 2023-08-04 11:21:12.000000 ptmethods-1.0.1/ptmethods.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-08-04 11:21:12.000000 ptmethods-1.0.1/ptmethods.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       55 2023-08-04 11:21:12.000000 ptmethods-1.0.1/ptmethods.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       22 2023-08-04 11:21:12.000000 ptmethods-1.0.1/ptmethods.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       10 2023-08-04 11:21:12.000000 ptmethods-1.0.1/ptmethods.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-08-04 11:21:12.462381 ptmethods-1.0.1/setup.cfg
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      973 2023-04-17 09:01:26.000000 ptmethods-1.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-07 11:43:25.390922 ptmethods-1.0.2/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-05-06 14:28:31.000000 ptmethods-1.0.2/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     4285 2024-05-07 11:43:25.390922 ptmethods-1.0.2/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     3496 2024-05-07 11:39:41.000000 ptmethods-1.0.2/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-07 11:43:25.390922 ptmethods-1.0.2/ptmethods/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 14:28:31.000000 ptmethods-1.0.2/ptmethods/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-07 11:34:00.000000 ptmethods-1.0.2/ptmethods/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    15346 2024-05-07 11:42:23.000000 ptmethods-1.0.2/ptmethods/ptmethods.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-07 11:43:25.390922 ptmethods-1.0.2/ptmethods.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4285 2024-05-07 11:43:25.000000 ptmethods-1.0.2/ptmethods.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      293 2024-05-07 11:43:25.000000 ptmethods-1.0.2/ptmethods.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-07 11:43:25.000000 ptmethods-1.0.2/ptmethods.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       55 2024-05-07 11:43:25.000000 ptmethods-1.0.2/ptmethods.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       26 2024-05-07 11:43:25.000000 ptmethods-1.0.2/ptmethods.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       10 2024-05-07 11:43:25.000000 ptmethods-1.0.2/ptmethods.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-07 11:43:25.390922 ptmethods-1.0.2/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1264 2024-05-07 11:33:57.000000 ptmethods-1.0.2/setup.py
```

### Comparing `ptmethods-1.0.1/LICENSE` & `ptmethods-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ptmethods-1.0.1/PKG-INFO` & `ptmethods-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,106 +1,97 @@
 Metadata-Version: 2.1
 Name: ptmethods
-Version: 1.0.1
-Summary: HTTP methods testing tool
+Version: 1.0.2
+Summary: HTTP Methods Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptmethods
+Project-URL: tracker, https://github.com/penterep/ptmethods/issues
+Project-URL: changelog, https://github.com/penterep/ptmethods/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ptlibs<2,>=1.0.7
+Requires-Dist: requests
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTMETHODS
-> HTTP methods testing tool
+## PTMETHODS - HTTP Methods Testing Tool
 
 - Script retrieves methods offered by server from OPTIONS request
 - Script sends GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD, TRACE, DEBUG, FOO headers and returns server response
 - Script tests CONNECT method by connecting to URL at ports 80, 443
 - Script tests if domain can be used as a proxy
 
 ## Installation
 ```
 pip install ptmethods
 ```
 
-## Add to PATH
-If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+## Adding to PATH
+If you're unable to invoke the script from your terminal, it's likely because it's not included in your PATH. You can resolve this issue by executing the following commands, depending on the shell you're using:
 
-> Add to PATH for Bash
+For Bash Users
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
-> Add to PATH for ZSH
+For ZSH Users
 ```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
-source ~/.zshhrc
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
+source ~/.zshrc
 ```
 
 ## Usage examples
 Optimally use this script against homepage, any image and sources protected by HTTP authentication
 ```
 ptmethods -u https://www.example.com/
 ptmethods -u https://www.example.com/ -r
 ptmethods -u https://www.example.com/index.php -sr -sh
 ptmethods -u https://www.example.com/index.php -c PHPSESSID=abcdef
-ptmethods -f URL_list.txt
+ptmethods -f urlList.txt
 ```
 
 ## Options
 ```
--u   --url            <url>           Test specified URL
--f   --file           <file>          Load URLs from file
--sh  --show-headers                   Show response headers
--sr  --show-response                  Show response text
--p   --proxy          <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--T   --timeout                        Set timeout (default 10)
--c   --cookie         <cookie>        Set cookie
--ua  --user-agent     <ua>            Set User-Agent header
--H   --headers        <header:value>  Set custom header(s)
--r   --redirects                      Follow redirects (default False)
--c   --cache                          Cache requests (load from tmp in future)
--v   --version                        Show script version and exit
--h   --help                           Show this help message and exit
--j   --json                           Output in JSON format
+-u   --url                  <url>           Test specified URL
+-f   --file                 <file>          Load URLs from file
+-sh  --show-headers                         Show response headers
+-sr  --show-response                        Show response text
+-T   --timeout                              Set timeout (default 10)
+-p   --proxy                <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-ua  --user-agent           <ua>            Set User-Agent header
+-c   --cookie               <cookie>        Set cookie
+-H   --headers              <header:value>  Set custom header(s)
+-r   --redirects                            Follow redirects (default False)
+-c   --cache                                Cache requests (load from tmp in future)
+-b   --check-basic-methods                  Skip creating JSON nodes (used with --json option)
+-v   --version                              Show script version and exit
+-h   --help                                 Show this help message and exit
+-j   --json                                 Output in JSON format
 ```
 
 ## Dependencies
 ```
-requests
 ptlibs
 ```
 
-## Version History
-```
-1.0.1
-    - Fix urllib3 error
-1.0.0
-    - Support for ptlibs v1.0.0
-    - Code refactorization
-0.0.2 - 0.0.4
-    - Implemented proxy and connect tests
-0.0.1 - 0.0.3
-    Alpha releases
-```
-
-
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
+Copyright (c) 2024 Penterep Security s.r.o.
 
 ptmethods is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptmethods is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptmethods. If not, see https://www.gnu.org/licenses/.
```

### Comparing `ptmethods-1.0.1/README.md` & `ptmethods-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,89 +1,74 @@
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTMETHODS
-> HTTP methods testing tool
+## PTMETHODS - HTTP Methods Testing Tool
 
 - Script retrieves methods offered by server from OPTIONS request
 - Script sends GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD, TRACE, DEBUG, FOO headers and returns server response
 - Script tests CONNECT method by connecting to URL at ports 80, 443
 - Script tests if domain can be used as a proxy
 
 ## Installation
 ```
 pip install ptmethods
 ```
 
-## Add to PATH
-If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+## Adding to PATH
+If you're unable to invoke the script from your terminal, it's likely because it's not included in your PATH. You can resolve this issue by executing the following commands, depending on the shell you're using:
 
-> Add to PATH for Bash
+For Bash Users
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
-> Add to PATH for ZSH
+For ZSH Users
 ```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
-source ~/.zshhrc
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
+source ~/.zshrc
 ```
 
 ## Usage examples
 Optimally use this script against homepage, any image and sources protected by HTTP authentication
 ```
 ptmethods -u https://www.example.com/
 ptmethods -u https://www.example.com/ -r
 ptmethods -u https://www.example.com/index.php -sr -sh
 ptmethods -u https://www.example.com/index.php -c PHPSESSID=abcdef
-ptmethods -f URL_list.txt
+ptmethods -f urlList.txt
 ```
 
 ## Options
 ```
--u   --url            <url>           Test specified URL
--f   --file           <file>          Load URLs from file
--sh  --show-headers                   Show response headers
--sr  --show-response                  Show response text
--p   --proxy          <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--T   --timeout                        Set timeout (default 10)
--c   --cookie         <cookie>        Set cookie
--ua  --user-agent     <ua>            Set User-Agent header
--H   --headers        <header:value>  Set custom header(s)
--r   --redirects                      Follow redirects (default False)
--c   --cache                          Cache requests (load from tmp in future)
--v   --version                        Show script version and exit
--h   --help                           Show this help message and exit
--j   --json                           Output in JSON format
+-u   --url                  <url>           Test specified URL
+-f   --file                 <file>          Load URLs from file
+-sh  --show-headers                         Show response headers
+-sr  --show-response                        Show response text
+-T   --timeout                              Set timeout (default 10)
+-p   --proxy                <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-ua  --user-agent           <ua>            Set User-Agent header
+-c   --cookie               <cookie>        Set cookie
+-H   --headers              <header:value>  Set custom header(s)
+-r   --redirects                            Follow redirects (default False)
+-c   --cache                                Cache requests (load from tmp in future)
+-b   --check-basic-methods                  Skip creating JSON nodes (used with --json option)
+-v   --version                              Show script version and exit
+-h   --help                                 Show this help message and exit
+-j   --json                                 Output in JSON format
 ```
 
 ## Dependencies
 ```
-requests
 ptlibs
 ```
 
-## Version History
-```
-1.0.1
-    - Fix urllib3 error
-1.0.0
-    - Support for ptlibs v1.0.0
-    - Code refactorization
-0.0.2 - 0.0.4
-    - Implemented proxy and connect tests
-0.0.1 - 0.0.3
-    Alpha releases
-```
-
-
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
+Copyright (c) 2024 Penterep Security s.r.o.
 
 ptmethods is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptmethods is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptmethods. If not, see https://www.gnu.org/licenses/.
```

### Comparing `ptmethods-1.0.1/ptmethods/ptmethods.py` & `ptmethods-1.0.2/ptmethods/ptmethods.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python3
 """
-    Copyright (c) 2023 Penterep Security s.r.o.
+    Copyright (c) 2024 Penterep Security s.r.o.
 
-    ptmethod - HTTP methods testing tool
+    ptmethods - HTTP Methods Testing Tool
 
     ptmethods is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     ptmethods is distributed in the hope that it will be useful,
@@ -28,61 +28,56 @@
 
 from _version import __version__
 from ptlibs import ptjsonlib, ptmisclib, ptnethelper, ptprinthelper
 
 
 class PtMethods:
     def __init__(self, args):
-        self.ptjsonlib          = ptjsonlib.PtJsonLib()
-        self.headers            = ptnethelper.get_request_headers(args)
-        self.proxies            = {"http": args.proxy, "https": args.proxy}
-        self.use_json           = args.json
-        self.redirects          = args.redirects
-        self.cache              = args.cache
-        self.timeout            = args.timeout
-        self.show_headers       = args.show_headers
-        self.show_response      = args.show_response
+        self.ptjsonlib           = ptjsonlib.PtJsonLib()
+        self.headers             = ptnethelper.get_request_headers(args)
+        self.proxies             = {"http": args.proxy, "https": args.proxy}
+        self.use_json            = args.json
+        self.redirects           = args.redirects
+        self.cache               = args.cache
+        self.timeout             = args.timeout
+        self.show_headers        = args.show_headers
+        self.show_response       = args.show_response
+        self.check_basic_methods = args.check_basic_methods
 
         try:
             self.url_list = ptmisclib.read_file(args.file) if args.file else args.url
         except FileNotFoundError:
             self.ptjsonlib.end_error("File not found", self.use_json)
 
         if len(self.url_list) > 1 and self.use_json:
                 self.ptjsonlib.end_error("Cannot test more than 1 URL while --json parameter is present", self.use_json)
 
     def run(self):
-        """Main method"""
         for index, url in enumerate(self.url_list):
             ptprinthelper.ptprint(f"Testing: {url}", "TITLE", not self.use_json, colortext=True)
             try:
                 self.port, url = self._parse_url(url)
-                self._run_tests(url)
-            except (ValueError, requests.exceptions.RequestException) as e:
+                options       = self._get_options(url)
+                methods       = self._check_methods(url)
+                connect_test  = self._test_connect_method(url)
+                proxy_test    = self._check_proxy_method(url)
+
+                self._print_results(url, options, methods, proxy_test, connect_test)
+
+            except (requests.exceptions.RequestException, ValueError) as e:
                 if len(self.url_list) > 1:
                     ptprinthelper.ptprint(f"Error: {e}", "ERROR", not self.use_json, end="\n\n" if not index+1 == len(self.url_list) else "\n")
                     continue
                 else:
                     self.ptjsonlib.end_error(f"{e}", self.use_json)
 
         if self.use_json:
-            self.ptjsonlib.set_status("ok")
+            self.ptjsonlib.set_status("finished")
             ptprinthelper.ptprint(self.ptjsonlib.get_result_json(), "", self.use_json)
 
-    def _run_tests(self, url: str):
-        """Runs all the tests"""
-        try:
-            options       = self._get_options(url)
-            methods       = self._check_methods(url)
-            connect_test  = self._test_connect_method(url)
-            proxy_test    = self._check_proxy_method(url)
-            self._print_results(url, options, methods, proxy_test, connect_test)
-        except requests.exceptions.RequestException as e:
-            raise e
-
     def _test_connect_method(self, url):
         try:
             response = self._get_response("https://www.example.com", "GET", proxies={"https": url+":"+self.port})
         except requests.RequestException as e:
             return False
         if re.search(r"<title>Example Domain</title>", response.text):
             try:
@@ -105,15 +100,15 @@
                 response_localhost = self._get_response("http://127.0.0.1", "GET", {"http": url+":"+self.port})
             except requests.RequestException as e:
                 title = "Error retrieving title from localhost"
                 return title
             title = re.search(r"<title.*?>([\s\S]*?)</title>", response_localhost.text)
             if title:
                 title = title.groups()[0]
-            self.ptjsonlib.add_vulnerability("PTWVPROXY", request=response_dump["request"], response=response_dump["response"], note=f"Title of localhost when proxy is used: {title}")
+            self.ptjsonlib.add_vulnerability("PTWVPROXY", vulm_request=response_dump["request"], vuln_response=response_dump["response"], note=f"Title of localhost when proxy is used: {title}")
             return title
 
     def _get_options(self, url):
         try:
             response = self._get_response(url, "OPTIONS")
             if "Allow" in response.headers:
                 allowed_methods = response.headers["Allow"].split(", ")
@@ -138,17 +133,26 @@
                 method_data.update({"location": response.headers.get("location")})
             if self.show_headers:
                 method_data["headers"].append(dict(response.headers))
             if self.show_response:
                 method_data["response"].append(response.text)
             if response.status_code < 400:
                 methods_result["available_methods"].append(method_data)
-                self.ptjsonlib.add_node(self.ptjsonlib.create_node_object("httpMethod", properties={"name": method, "httpMethodType": method}))
-                if method in ["TRACE"]:
-                    self.ptjsonlib.add_vulnerability("PTWVHTTPTRACE", request=response_dump["request"], response=response_dump["response"])
+
+                if self.use_json:
+                    if self.check_basic_methods:
+                        vuln_code_map = {"PUT": "PTV-WEB-HTTP-METPUT", "PATCH": "PTV-WEB-HTTP-METPTCH", "DELETE": "PTV-WEB-HTTP-METDEL", "OPTIONS": "PTV-WEB-HTTP-METOPT", "HEAD": "PTV-WEB-HTTP-METHEAD", "TRACE": "PTV-WEB-HTTP-METTRC", "DEBUG": "PTV-WEB-HTTP-METDBG", "FOO": "PTV-WEB-HTTP-METNON"}
+                        if vuln_code_map.get(method):
+                            self.ptjsonlib.add_vulnerability(vuln_code_map[method])
+                        self.handle_check_basic_methods(method)
+                    else:
+                        node = self.ptjsonlib.create_node_object("httpMethod", properties={"name": method, "httpMethodType": method})
+                        if method == "TRACE":
+                            node["vulnerabilities"].append({"vulnCode": "PTV-WEB-HTTP-METTRC"})
+                        self.ptjsonlib.add_node(node)
             else:
                 methods_result["not_available_methods"].append(method_data)
         ptprinthelper.ptprint(f"{' '*30}", "", self.use_json == False, end="\r")
 
         return methods_result
 
     def _print_results(self, url, options, methods, proxy_method, connect_method):
@@ -211,56 +215,58 @@
         return port, urllib.parse.urlunparse(o)
 
 
 def get_help():
     return [
         {"description": ["HTTP methods testing tool"]},
         {"usage": ["ptmethods <options>"]},
-        {"Tip": ["Optimally use this script against homepage, any image and sources protected by HTTP authentication"]},
+        {"Tip": ["Use this script against existing sources like homepages, images, or resources protected by HTTP authentication."]},
         {"usage_example": [
             "ptmethods -u https://www.example.com/image.png",
             "ptmethods -u https://www.example.com/index.php",
             "ptmethods -u https://www.example.com/index.php -c PHPSESSID=abcdef",
-            "ptmethods -f URL_list.txt",
+            "ptmethods -f urlList.txt",
         ]},
         {"options": [
             ["-u",  "--url",                    "<url>",            "Test specified URL"],
             ["-f",  "--file",                   "<file>",           "Load URLs from file"],
             ["-sh", "--show-headers",           "",                 "Show response headers"],
             ["-sr", "--show-response",          "",                 "Show response text"],
             ["-T",  "--timeout",                "",                 "Set timeout (default 10)"],
             ["-p",  "--proxy",                  "<proxy>",          "Set proxy (e.g. http://127.0.0.1:8080)"],
             ["-ua", "--user-agent",             "<ua>",             "Set User-Agent header"],
             ["-c",  "--cookie",                 "<cookie>",         "Set cookie"],
             ["-H",  "--headers",                "<header:value>",   "Set custom header(s)"],
             ["-r",  "--redirects",              "",                 "Follow redirects (default False)"],
             ["-c",  "--cache",                  "",                 "Cache requests (load from tmp in future)"],
+            ["-b",  "--check-basic-methods",    "",                 "Skip creating JSON nodes (used with --json option)"],
             ["-v",  "--version",                "",                 "Show script version and exit"],
             ["-h",  "--help",                   "",                 "Show this help message and exit"],
             ["-j",  "--json",                   "",                 "Output in JSON format"],
         ]
         }]
 
 
 def parse_args():
     parser = argparse.ArgumentParser(add_help=False, usage="ptmethods <options>")
     exclusive_group = parser.add_mutually_exclusive_group(required=True)
-    exclusive_group.add_argument("-u", "--url",    type=str, nargs="+")
-    exclusive_group.add_argument("-f", "--file",   type=str)
-    parser.add_argument("-p",  "--proxy",          type=str)
-    parser.add_argument("-ua", "--user-agent",     type=str, default="Penterep Tools")
-    parser.add_argument("-c",  "--cookie",         type=str, nargs="+")
-    parser.add_argument("-T",  "--timeout",        type=int, default=6)
-    parser.add_argument("-H",  "--headers",        type=ptmisclib.pairs, nargs="+")
-    parser.add_argument("-j",  "--json",           action="store_true")
-    parser.add_argument("-r",  "--redirects",      action="store_true")
-    parser.add_argument("-C",  "--cache",          action="store_true")
-    parser.add_argument("-sr", "--show-response",  action="store_true")
-    parser.add_argument("-sh", "--show-headers",   action="store_true")
-    parser.add_argument("-v",  "--version",        action="version", version=f"{SCRIPTNAME} {__version__}")
+    exclusive_group.add_argument("-u", "--url",         type=str, nargs="+")
+    exclusive_group.add_argument("-f", "--file",        type=str)
+    parser.add_argument("-p",  "--proxy",               type=str)
+    parser.add_argument("-ua", "--user-agent",          type=str, default="Penterep Tools")
+    parser.add_argument("-c",  "--cookie",              type=str, nargs="+")
+    parser.add_argument("-T",  "--timeout",             type=int, default=6)
+    parser.add_argument("-H",  "--headers",             type=ptmisclib.pairs, nargs="+")
+    parser.add_argument("-j",  "--json",                action="store_true")
+    parser.add_argument("-r",  "--redirects",           action="store_true")
+    parser.add_argument("-C",  "--cache",               action="store_true")
+    parser.add_argument("-b",  "--check-basic-methods", action="store_true")
+    parser.add_argument("-sr", "--show-response",       action="store_true")
+    parser.add_argument("-sh", "--show-headers",        action="store_true")
+    parser.add_argument("-v",  "--version",             action="version", version=f"{SCRIPTNAME} {__version__}")
 
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
         ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
     args = parser.parse_args()
     ptprinthelper.print_banner(SCRIPTNAME, __version__, args.json, space=0)
     return args
```

### Comparing `ptmethods-1.0.1/ptmethods.egg-info/PKG-INFO` & `ptmethods-1.0.2/ptmethods.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,106 +1,97 @@
 Metadata-Version: 2.1
 Name: ptmethods
-Version: 1.0.1
-Summary: HTTP methods testing tool
+Version: 1.0.2
+Summary: HTTP Methods Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptmethods
+Project-URL: tracker, https://github.com/penterep/ptmethods/issues
+Project-URL: changelog, https://github.com/penterep/ptmethods/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ptlibs<2,>=1.0.7
+Requires-Dist: requests
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTMETHODS
-> HTTP methods testing tool
+## PTMETHODS - HTTP Methods Testing Tool
 
 - Script retrieves methods offered by server from OPTIONS request
 - Script sends GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD, TRACE, DEBUG, FOO headers and returns server response
 - Script tests CONNECT method by connecting to URL at ports 80, 443
 - Script tests if domain can be used as a proxy
 
 ## Installation
 ```
 pip install ptmethods
 ```
 
-## Add to PATH
-If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+## Adding to PATH
+If you're unable to invoke the script from your terminal, it's likely because it's not included in your PATH. You can resolve this issue by executing the following commands, depending on the shell you're using:
 
-> Add to PATH for Bash
+For Bash Users
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
-> Add to PATH for ZSH
+For ZSH Users
 ```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
-source ~/.zshhrc
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
+source ~/.zshrc
 ```
 
 ## Usage examples
 Optimally use this script against homepage, any image and sources protected by HTTP authentication
 ```
 ptmethods -u https://www.example.com/
 ptmethods -u https://www.example.com/ -r
 ptmethods -u https://www.example.com/index.php -sr -sh
 ptmethods -u https://www.example.com/index.php -c PHPSESSID=abcdef
-ptmethods -f URL_list.txt
+ptmethods -f urlList.txt
 ```
 
 ## Options
 ```
--u   --url            <url>           Test specified URL
--f   --file           <file>          Load URLs from file
--sh  --show-headers                   Show response headers
--sr  --show-response                  Show response text
--p   --proxy          <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--T   --timeout                        Set timeout (default 10)
--c   --cookie         <cookie>        Set cookie
--ua  --user-agent     <ua>            Set User-Agent header
--H   --headers        <header:value>  Set custom header(s)
--r   --redirects                      Follow redirects (default False)
--c   --cache                          Cache requests (load from tmp in future)
--v   --version                        Show script version and exit
--h   --help                           Show this help message and exit
--j   --json                           Output in JSON format
+-u   --url                  <url>           Test specified URL
+-f   --file                 <file>          Load URLs from file
+-sh  --show-headers                         Show response headers
+-sr  --show-response                        Show response text
+-T   --timeout                              Set timeout (default 10)
+-p   --proxy                <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-ua  --user-agent           <ua>            Set User-Agent header
+-c   --cookie               <cookie>        Set cookie
+-H   --headers              <header:value>  Set custom header(s)
+-r   --redirects                            Follow redirects (default False)
+-c   --cache                                Cache requests (load from tmp in future)
+-b   --check-basic-methods                  Skip creating JSON nodes (used with --json option)
+-v   --version                              Show script version and exit
+-h   --help                                 Show this help message and exit
+-j   --json                                 Output in JSON format
 ```
 
 ## Dependencies
 ```
-requests
 ptlibs
 ```
 
-## Version History
-```
-1.0.1
-    - Fix urllib3 error
-1.0.0
-    - Support for ptlibs v1.0.0
-    - Code refactorization
-0.0.2 - 0.0.4
-    - Implemented proxy and connect tests
-0.0.1 - 0.0.3
-    Alpha releases
-```
-
-
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
+Copyright (c) 2024 Penterep Security s.r.o.
 
 ptmethods is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptmethods is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptmethods. If not, see https://www.gnu.org/licenses/.
```

