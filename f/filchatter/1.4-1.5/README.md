# Comparing `tmp/filchatter-1.4.tar.gz` & `tmp/filchatter-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filchatter-1.4.tar", last modified: Sun May  5 04:05:27 2024, max compression
+gzip compressed data, was "filchatter-1.5.tar", last modified: Tue May  7 09:21:29 2024, max compression
```

## Comparing `filchatter-1.4.tar` & `filchatter-1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 04:05:27.048339 filchatter-1.4/
-drwxrwxrwx   0        0        0        0 2024-05-05 04:05:27.030175 filchatter-1.4/Filchatter/
--rw-rw-rw-   0        0        0       62 2024-05-04 06:42:16.000000 filchatter-1.4/Filchatter/__init__.py
--rw-rw-rw-   0        0        0     1031 2024-05-05 04:05:22.000000 filchatter-1.4/Filchatter/filchatter.py
--rw-rw-rw-   0        0        0     1070 2024-05-04 05:07:58.000000 filchatter-1.4/LICENSE.md
--rw-rw-rw-   0        0        0      106 2024-05-05 04:05:27.045135 filchatter-1.4/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-04 05:10:02.000000 filchatter-1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 04:05:27.044139 filchatter-1.4/filchatter.egg-info/
--rw-rw-rw-   0        0        0      106 2024-05-05 04:05:26.000000 filchatter-1.4/filchatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-05-05 04:05:26.000000 filchatter-1.4/filchatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 04:05:26.000000 filchatter-1.4/filchatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-05 04:05:26.000000 filchatter-1.4/filchatter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-05 04:05:26.000000 filchatter-1.4/filchatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-05 04:05:26.000000 filchatter-1.4/filchatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 04:05:27.048339 filchatter-1.4/setup.cfg
--rw-rw-rw-   0        0        0      278 2024-05-05 04:03:32.000000 filchatter-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:21:29.318900 filchatter-1.5/
+drwxrwxrwx   0        0        0        0 2024-05-07 09:21:29.289013 filchatter-1.5/Filchatter/
+-rw-rw-rw-   0        0        0       62 2024-05-04 06:42:16.000000 filchatter-1.5/Filchatter/__init__.py
+-rw-rw-rw-   0        0        0     1035 2024-05-07 09:19:17.000000 filchatter-1.5/Filchatter/filchatter.py
+-rw-rw-rw-   0        0        0     1070 2024-05-04 05:07:58.000000 filchatter-1.5/LICENSE.md
+-rw-rw-rw-   0        0        0      106 2024-05-07 09:21:29.317902 filchatter-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-04 05:10:02.000000 filchatter-1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 09:21:29.316907 filchatter-1.5/filchatter.egg-info/
+-rw-rw-rw-   0        0        0      106 2024-05-07 09:21:29.000000 filchatter-1.5/filchatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-05-07 09:21:29.000000 filchatter-1.5/filchatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 09:21:29.000000 filchatter-1.5/filchatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-07 09:21:29.000000 filchatter-1.5/filchatter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 09:21:29.000000 filchatter-1.5/filchatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-07 09:21:29.000000 filchatter-1.5/filchatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 09:21:29.319897 filchatter-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      278 2024-05-07 09:20:04.000000 filchatter-1.5/setup.py
```

### Comparing `filchatter-1.4/Filchatter/filchatter.py` & `filchatter-1.5/Filchatter/filchatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def get_api_key(self, name):
         target_url = self.url + "/api/generate_key_post"
         response = self.session.post(target_url, json={'name': name})
         return response
         
     # JSON 데이터를 보내는 POST 요청
     def send_json_request(self, chat, option = 0):
-        target_url = self.url +"/receive_json"
+        target_url = self.url +"/api/receive_json"
         if self.api_key == None:
             print("You should set api key with set_api_key() method.")
             return
         elif chat == None:
             print("Invalid request.")
             return
         # 서버의 IP 주소와 포트
```

### Comparing `filchatter-1.4/LICENSE.md` & `filchatter-1.5/LICENSE.md`

 * *Files identical despite different names*

