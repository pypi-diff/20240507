# Comparing `tmp/opyngpt-0.2.0.tar.gz` & `tmp/opyngpt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opyngpt-0.2.0.tar", last modified: Mon May  6 17:46:34 2024, max compression
+gzip compressed data, was "opyngpt-0.3.0.tar", last modified: Tue May  7 05:04:37 2024, max compression
```

## Comparing `opyngpt-0.2.0.tar` & `opyngpt-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 17:46:34.733947 opyngpt-0.2.0/
--rw-rw-rw-   0        0        0     3429 2024-05-06 17:46:34.732941 opyngpt-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3102 2024-05-06 17:44:38.000000 opyngpt-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 17:46:34.727637 opyngpt-0.2.0/opyngpt/
--rw-rw-rw-   0        0        0       26 2024-05-06 17:12:53.000000 opyngpt-0.2.0/opyngpt/__init__.py
--rw-rw-rw-   0        0        0     1626 2024-05-06 17:27:21.000000 opyngpt-0.2.0/opyngpt/chat.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:46:34.731506 opyngpt-0.2.0/opyngpt.egg-info/
--rw-rw-rw-   0        0        0     3429 2024-05-06 17:46:34.000000 opyngpt-0.2.0/opyngpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-06 17:46:34.000000 opyngpt-0.2.0/opyngpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 17:46:34.000000 opyngpt-0.2.0/opyngpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-06 17:46:34.000000 opyngpt-0.2.0/opyngpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-06 17:46:34.000000 opyngpt-0.2.0/opyngpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 17:46:34.733947 opyngpt-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     3615 2024-05-06 17:42:24.000000 opyngpt-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:04:37.555589 opyngpt-0.3.0/
+-rw-rw-rw-   0        0        0     5283 2024-05-07 05:04:37.555589 opyngpt-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4653 2024-05-07 05:00:49.000000 opyngpt-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 05:04:37.548752 opyngpt-0.3.0/opyngpt/
+-rw-rw-rw-   0        0        0       26 2024-05-06 17:12:53.000000 opyngpt-0.3.0/opyngpt/__init__.py
+-rw-rw-rw-   0        0        0     2094 2024-05-07 04:48:03.000000 opyngpt-0.3.0/opyngpt/chat.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:04:37.554633 opyngpt-0.3.0/opyngpt.egg-info/
+-rw-rw-rw-   0        0        0     5283 2024-05-07 05:04:37.000000 opyngpt-0.3.0/opyngpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-07 05:04:37.000000 opyngpt-0.3.0/opyngpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 05:04:37.000000 opyngpt-0.3.0/opyngpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-07 05:04:37.000000 opyngpt-0.3.0/opyngpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 05:04:37.000000 opyngpt-0.3.0/opyngpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 05:04:37.000000 opyngpt-0.3.0/opyngpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 05:04:37.555589 opyngpt-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     5585 2024-05-07 05:02:57.000000 opyngpt-0.3.0/setup.py
```

### Comparing `opyngpt-0.2.0/opyngpt/chat.py` & `opyngpt-0.3.0/opyngpt/chat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
-
 import requests
-
+import sys
 
 def prompt(input_message):
     url = "https://https.extension.phind.com/agent/"
     headers = {
         "Content-Type": "application/json",
         "User-Agent": "",
         "Accept": "*/*",
@@ -40,7 +39,23 @@
                 pass
         return "".join(content_values)
     elif response.status_code == 401 or response.status_code == 429:
         print(f"Error: {response.status_code}, Trying again.")
         response = prompt(input_message)
     else:
         return f"Error: {response.status_code}, {response.text}"
+
+def main():
+    if len(sys.argv) == 1:
+        while True:
+            input_message = input("Enter your message (type 'exit' to quit): ")
+            if input_message.lower() == 'exit':
+                break
+            response = prompt(input_message)
+            print(response)
+    else:
+        input_message = ' '.join(sys.argv[1:])
+        response = prompt(input_message)
+        print(response)
+
+if __name__ == "__main__":
+    main()
```

