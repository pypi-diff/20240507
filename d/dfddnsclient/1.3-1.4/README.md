# Comparing `tmp/dfddnsclient-1.3.tar.gz` & `tmp/dfddnsclient-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfddnsclient-1.3.tar", last modified: Wed May  1 22:14:46 2024, max compression
+gzip compressed data, was "dfddnsclient-1.4.tar", last modified: Tue May  7 19:42:36 2024, max compression
```

## Comparing `dfddnsclient-1.3.tar` & `dfddnsclient-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 22:14:46.060797 dfddnsclient-1.3/
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 17:51:39.000000 dfddnsclient-1.3/LICENSE
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      263 2024-05-01 22:14:46.060660 dfddnsclient-1.3/PKG-INFO
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      248 2024-05-01 22:14:10.000000 dfddnsclient-1.3/README.md
-drwxr-xr-x   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 22:14:46.059444 dfddnsclient-1.3/dfddnsclient/
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 17:50:48.000000 dfddnsclient-1.3/dfddnsclient/__init__.py
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)     2247 2024-05-01 20:44:31.000000 dfddnsclient-1.3/dfddnsclient/app.py
-drwxr-xr-x   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 22:14:46.060437 dfddnsclient-1.3/dfddnsclient.egg-info/
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      263 2024-05-01 22:14:46.000000 dfddnsclient-1.3/dfddnsclient.egg-info/PKG-INFO
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      289 2024-05-01 22:14:46.000000 dfddnsclient-1.3/dfddnsclient.egg-info/SOURCES.txt
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)        1 2024-05-01 22:14:46.000000 dfddnsclient-1.3/dfddnsclient.egg-info/dependency_links.txt
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       56 2024-05-01 22:14:46.000000 dfddnsclient-1.3/dfddnsclient.egg-info/entry_points.txt
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       24 2024-05-01 22:14:46.000000 dfddnsclient-1.3/dfddnsclient.egg-info/requires.txt
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       13 2024-05-01 22:14:46.000000 dfddnsclient-1.3/dfddnsclient.egg-info/top_level.txt
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       38 2024-05-01 22:14:46.060900 dfddnsclient-1.3/setup.cfg
--rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      517 2024-05-01 22:13:46.000000 dfddnsclient-1.3/setup.py
+drwxr-xr-x   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-07 19:42:36.335538 dfddnsclient-1.4/
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 17:51:39.000000 dfddnsclient-1.4/LICENSE
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      263 2024-05-07 19:42:36.335420 dfddnsclient-1.4/PKG-INFO
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      600 2024-05-07 19:32:24.000000 dfddnsclient-1.4/README.md
+drwxr-xr-x   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-07 19:42:36.334310 dfddnsclient-1.4/dfddnsclient/
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-01 17:50:48.000000 dfddnsclient-1.4/dfddnsclient/__init__.py
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)     2966 2024-05-07 19:23:38.000000 dfddnsclient-1.4/dfddnsclient/app.py
+drwxr-xr-x   0 vincentchimdimbaeri   (501) staff       (20)        0 2024-05-07 19:42:36.335206 dfddnsclient-1.4/dfddnsclient.egg-info/
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      263 2024-05-07 19:42:36.000000 dfddnsclient-1.4/dfddnsclient.egg-info/PKG-INFO
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      289 2024-05-07 19:42:36.000000 dfddnsclient-1.4/dfddnsclient.egg-info/SOURCES.txt
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)        1 2024-05-07 19:42:36.000000 dfddnsclient-1.4/dfddnsclient.egg-info/dependency_links.txt
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       56 2024-05-07 19:42:36.000000 dfddnsclient-1.4/dfddnsclient.egg-info/entry_points.txt
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       24 2024-05-07 19:42:36.000000 dfddnsclient-1.4/dfddnsclient.egg-info/requires.txt
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       13 2024-05-07 19:42:36.000000 dfddnsclient-1.4/dfddnsclient.egg-info/top_level.txt
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)       38 2024-05-07 19:42:36.335595 dfddnsclient-1.4/setup.cfg
+-rw-r--r--   0 vincentchimdimbaeri   (501) staff       (20)      517 2024-05-07 19:35:06.000000 dfddnsclient-1.4/setup.py
```

### Comparing `dfddnsclient-1.3/dfddnsclient/app.py` & `dfddnsclient-1.4/dfddnsclient/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,70 +3,94 @@
 import requests
 import os
 import schedule
 import time
 import sys
 
 
-if len(sys.argv) != 3:
+if len(sys.argv) != 4:
     print("Usage: python3 app.py <cname> <passkey>")
     sys.exit(1)
 
 
 app = Flask(__name__)
 app.secret_key = os.urandom(24)
 
 #Parameters#######
-new_ipv4 = ""
-old_ipv4 = ""
-cname = sys.argv[1]
-passkey = sys.argv[2]
-interval = 120
+new_ip = ""
+old_ip = ""
+protocol = ""
+stack = sys.argv[1]
+cname = sys.argv[2]
+passkey = sys.argv[3]
+
+interval = 90
 #####################
 
 
 def get_public_ip():
-    global old_ipv4, new_ipv4
-    try:
-        result = subprocess.run(['curl', '-4', 'ifconfig.me'], capture_output=True, text=True)
-        if result.returncode == 0:
-            new_ipv4 = result.stdout.strip()
-            #print("running...")
-            if new_ipv4 != old_ipv4:
-                print("ipv4 change detected!")
-                return update_dns_record()
-                
-    except Exception as e:
-        return f"Error retrieving public IPv4: {e}"
-    return new_ipv4
+    global old_ip, new_ip, protocol
+    
+    if stack == '-4':
+        try:
+            result = subprocess.run(['curl', '-4', 'ifconfig.me'], capture_output=True, text=True)
+            if result.returncode == 0:
+                new_ip = result.stdout.strip()
+                if new_ip != old_ip:
+                    protocol = 'IPv4'
+                    #print(new_ip)
+                    return update_dns_record()
+                    
+        except Exception as e:
+            return f"Error retrieving public IPv4: {e}"
+        return new_ip
+    
+    elif stack == '-6':
+        try:
+            result = subprocess.run(['curl', '-6', 'ifconfig.me'], capture_output=True, text=True)
+            if result.returncode == 0:
+                new_ip = result.stdout.strip()
+                if new_ip != old_ip:
+                    protocol = 'IPv6'
+                    #print(new_ip)
+                    return update_dns_record()
+                    
+        except Exception as e:
+            return f"Error retrieving public IPv6: {e}"
+        return new_ip
+
+    else:
+        print("protocol not recognized! choose either '-4' for ipv4 or '-6' for ipv6 protocols respectively.")
+
 
 
 
 @app.route('/update_ip', methods=['GET'])
 def update_dns_record():
-    global cname, old_ipv4, new_ipv4, passkey
+    global cname, old_ip, new_ip, passkey, protocol
     url = "https://ddns.dartfox.xyz/update_ip"
 
     payload = {
         "cname": cname,
         "passkey": passkey,
-        "new_ipv4": new_ipv4
+        "new_ip": new_ip,
+        "protocol": protocol
     }
 
     headers = {
         'Content-Type': 'application/json'
     }
 
     response = requests.post(url, json=payload, headers=headers)
     if response.status_code == 200:
-        print("ip change detected and cname records updated!")
-        old_ipv4 = new_ipv4
+        print(response.text)
+        old_ip = new_ip
         return response.text
     else:
-        print(response.text)
+        return response.text
     
 # Function to perform IP check
 schedule.every(interval).seconds.do(get_public_ip)
 
 # Function to start scheduling
 @app.route('/start', methods=['GET'])
 def start_scheduling():
```

### Comparing `dfddnsclient-1.3/setup.py` & `dfddnsclient-1.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dfddnsclient',
-    version='1.3',
+    version='1.4',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'dfddnsclient = dfddnsclient.app:main',
         ],
     },
     install_requires=[
```

