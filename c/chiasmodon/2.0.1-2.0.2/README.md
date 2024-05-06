# Comparing `tmp/chiasmodon-2.0.1.tar.gz` & `tmp/chiasmodon-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-2.0.1.tar", last modified: Tue Apr 30 19:28:48 2024, max compression
+gzip compressed data, was "chiasmodon-2.0.2.tar", last modified: Mon May  6 23:51:19 2024, max compression
```

## Comparing `chiasmodon-2.0.1.tar` & `chiasmodon-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-30 19:28:48.793410 chiasmodon-2.0.1/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-2.0.1/LICENSE.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-04-30 19:28:48.793410 chiasmodon-2.0.1/PKG-INFO
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11584 2024-04-30 19:12:19.000000 chiasmodon-2.0.1/README.md
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-30 19:28:48.793410 chiasmodon-2.0.1/chiasmodon.egg-info/
--rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-04-30 19:28:48.000000 chiasmodon-2.0.1/chiasmodon.egg-info/PKG-INFO
--rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-30 19:28:48.000000 chiasmodon-2.0.1/chiasmodon.egg-info/SOURCES.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-30 19:28:48.000000 chiasmodon-2.0.1/chiasmodon.egg-info/dependency_links.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)       39 2024-04-30 19:28:48.000000 chiasmodon-2.0.1/chiasmodon.egg-info/requires.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-30 19:28:48.000000 chiasmodon-2.0.1/chiasmodon.egg-info/top_level.txt
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-30 19:28:48.793410 chiasmodon-2.0.1/cli/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    21965 2024-04-30 19:16:31.000000 chiasmodon-2.0.1/cli/chiasmodon_cli.py
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    27978 2024-04-30 19:28:34.000000 chiasmodon-2.0.1/pychiasmodon.py
--rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-30 19:28:48.793410 chiasmodon-2.0.1/setup.cfg
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1262 2024-04-30 19:28:38.000000 chiasmodon-2.0.1/setup.py
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-06 23:51:19.982908 chiasmodon-2.0.2/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-2.0.2/LICENSE.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-05-06 23:51:19.982908 chiasmodon-2.0.2/PKG-INFO
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11584 2024-04-30 19:12:19.000000 chiasmodon-2.0.2/README.md
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-06 23:51:19.982908 chiasmodon-2.0.2/chiasmodon.egg-info/
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-05-06 23:51:19.000000 chiasmodon-2.0.2/chiasmodon.egg-info/PKG-INFO
+-rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-05-06 23:51:19.000000 chiasmodon-2.0.2/chiasmodon.egg-info/SOURCES.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-05-06 23:51:19.000000 chiasmodon-2.0.2/chiasmodon.egg-info/dependency_links.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       39 2024-05-06 23:51:19.000000 chiasmodon-2.0.2/chiasmodon.egg-info/requires.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-05-06 23:51:19.000000 chiasmodon-2.0.2/chiasmodon.egg-info/top_level.txt
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-05-06 23:51:19.982908 chiasmodon-2.0.2/cli/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    21908 2024-05-06 23:50:44.000000 chiasmodon-2.0.2/cli/chiasmodon_cli.py
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    27918 2024-05-06 23:50:24.000000 chiasmodon-2.0.2/pychiasmodon.py
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-05-06 23:51:19.982908 chiasmodon-2.0.2/setup.cfg
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1262 2024-05-06 23:50:36.000000 chiasmodon-2.0.2/setup.py
```

### Comparing `chiasmodon-2.0.1/LICENSE.txt` & `chiasmodon-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chiasmodon-2.0.1/PKG-INFO` & `chiasmodon-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 2.0.1
+Version: 2.0.2
 Summary: Chiasmodon is an OSINT tool that allows users to gather information from various sources and conduct targeted searches based on domains, Google Play applications, email addresses, IP addresses, organizations, URLs, and more. It provides comprehensive scanning capabilities, customizable output formats, and additional options for enhanced data analysis and customization.
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-2.0.1/README.md` & `chiasmodon-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `chiasmodon-2.0.1/chiasmodon.egg-info/PKG-INFO` & `chiasmodon-2.0.2/chiasmodon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 2.0.1
+Version: 2.0.2
 Summary: Chiasmodon is an OSINT tool that allows users to gather information from various sources and conduct targeted searches based on domains, Google Play applications, email addresses, IP addresses, organizations, URLs, and more. It provides comprehensive scanning capabilities, customizable output formats, and additional options for enhanced data analysis and customization.
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-2.0.1/cli/chiasmodon_cli.py` & `chiasmodon-2.0.2/cli/chiasmodon_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,15 @@
                 print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'ips.txt')}{T.RESET}\n"
                 
             self.print(f'{T.MAGENTA}{"-"*30}{T.RESET}')
         if self.options.scan_clients.lower() == 'yes':
             client_creds:list[Result] = self.search(
                 query=domain,
                 method='domain.all',
-                view_type='cred',
+                view_type='full',
                 sort=True ,
                 timeout=self.options.timeout,
                 limit=1000000,
                 callback_view_result=self.scan_callback,
                 yaspin=yaspin,
                 search_text=f'Find {T.GREEN+domain+T.RESET} client creds...',
                 err_text=f'Not found clients !'
@@ -252,17 +252,18 @@
 
 
             self.print(f'{T.MAGENTA}{"-"*30}{T.RESET}')
         if self.options.scan_employees.lower() == 'yes':
             employe_creds = self.search(
                 query=domain,
                 method='cred.email.domain',
-                view_type='cred',
+                view_type='full',
                 sort=True,
                 timeout=self.options.timeout,
+                callback_view_result=self.scan_callback,
                 limit=1000000,
                 yaspin=yaspin,
                 search_text=f'Find {T.GREEN+domain+T.RESET} employees creds...',
                 err_text=f'Not found Employees!'
             )
 
             if employe_creds:
@@ -331,25 +332,23 @@
         
     def save_result(self, view_type) -> None:
 
         if self.options.output:
 
             if self.options.output_type == "text":
                 if self.result and view_type != 'cred':
-                    self.result = list(set(self.result))
                     self.result.remove(None) if None in self.result else None
                 
                 ULIT.wFile(
                     self.options.output,
                     '\n'.join([':'.join(i) if type(i) == list else i for i in self.result]) 
                 )
 
             if self.options.output_type == "csv":
                 if self.result and view_type != 'cred':
-                    self.result = list(set(self.result))
                     self.result.remove(None) if None in self.result else None
                 
                 ULIT.wFile(
                     self.options.output,
                     '\n'.join([','.join(['url/app_id','user/email', 'password', 'country', 'date'])]+[','.join(i) if type(i) == list else i for i in self.result])  if view_type == 'cred' else  '\n'.join([view_type]+[','.join(i) if type(i) == list else i for i in self.result]) 
                 )
```

### Comparing `chiasmodon-2.0.1/pychiasmodon.py` & `chiasmodon-2.0.2/pychiasmodon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os 
 import sys
 import time
 import requests
 import tldextract
 from yaspin import Spinner 
 
-VERSION = "2.0.1"
+VERSION = "2.0.2"
 _API_URL = 'https://chiasmodon.com/v2/api/beta'
 _API_HEADERS = {'user-agent':'cli/python'}
 _VIEW_TYPE = {
     'full':[
         'cred.username',
         'cred.phone',
         'cred.password',
@@ -429,28 +429,28 @@
                 timeout=timeout,
             )
 
             if self.err:
                 self.err=False
                 if yaspin:self.print(f"{T.RED}{self.msg}{T.RESET}", YS, ys_err=True);YS.fail("💥 ");YS.stop()
                 return result
-            
+
             for r in beta_result['data']:
                 
                 column :Result = Result(**r)
 
                 if sort and column in self.__result:
                     continue
                 
-                if callback_view_result:
+                if callback_view_result != None:
                     callback_view_result(beta=column, ys=YS)
 
                 result.append(column)
                 self.__result.append(column)
-              
+
                 if len(result) == limit:
                     if yaspin:YS.text='';YS.stop()
                     return result
                 
             if beta_result['done']:
                 if yaspin:YS.text='';YS.stop()
                 return result
@@ -621,18 +621,15 @@
         elif url['ip']:
             return f"{url['proto']}://{url['ip']['ip']}:{url['port']}{url['path']}" 
 
         
         return None 
 
     def __convert_domain(self,domain:dict):
-        if domain['sub']:
-            return f"{domain['sub']}.{domain['name']}.{domain['suffix']}"
-        else:
-            return  f"{domain['name']}.{domain['suffix']}"
+        return f"{(domain['sub']+'.') if domain['sub'] else ''}{domain['name']}{('.'+domain['suffix']) if domain['suffix']  else ''}"
 
 
     def __str__(self) -> str:
         return self.save_format()
 
     def __radd__(self, other):
         if isinstance(other, str):
```

### Comparing `chiasmodon-2.0.1/setup.py` & `chiasmodon-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='chiasmodon',
-      version='2.0.1',
+      version='2.0.2',
       description='Chiasmodon is an OSINT tool that allows users to gather information from various sources and conduct targeted searches based on domains, Google Play applications, email addresses, IP addresses, organizations, URLs, and more. It provides comprehensive scanning capabilities, customizable output formats, and additional options for enhanced data analysis and customization.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='chiasmod0n',
       keywords='intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon',
       url='https://github.com/chiasmod0n/chiasmodon',
       packages=['.'],
```

