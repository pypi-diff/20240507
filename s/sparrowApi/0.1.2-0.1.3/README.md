# Comparing `tmp/sparrowApi-0.1.2.tar.gz` & `tmp/sparrowApi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparrowApi-0.1.2.tar", last modified: Tue Apr 16 07:04:04 2024, max compression
+gzip compressed data, was "sparrowApi-0.1.3.tar", last modified: Tue May  7 08:54:09 2024, max compression
```

## Comparing `sparrowApi-0.1.2.tar` & `sparrowApi-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 07:04:04.233822 sparrowApi-0.1.2/
--rw-rw-rw-   0        0        0      142 2024-04-16 07:04:04.232300 sparrowApi-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-16 07:04:04.233949 sparrowApi-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      248 2024-04-16 07:04:00.000000 sparrowApi-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 07:04:04.220798 sparrowApi-0.1.2/sparrowApi/
--rw-rw-rw-   0        0        0      504 2024-04-15 01:27:32.000000 sparrowApi-0.1.2/sparrowApi/__init__.py
--rw-rw-rw-   0        0        0    16269 2024-04-16 07:04:00.000000 sparrowApi-0.1.2/sparrowApi/api.py
--rw-rw-rw-   0        0        0      825 2024-04-12 08:45:23.000000 sparrowApi-0.1.2/sparrowApi/constant.py
--rw-rw-rw-   0        0        0     5357 2024-04-15 02:46:23.000000 sparrowApi-0.1.2/sparrowApi/tool_class.py
-drwxrwxrwx   0        0        0        0 2024-04-16 07:04:04.230403 sparrowApi-0.1.2/sparrowApi.egg-info/
--rw-rw-rw-   0        0        0      142 2024-04-16 07:04:04.000000 sparrowApi-0.1.2/sparrowApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-16 07:04:04.000000 sparrowApi-0.1.2/sparrowApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 07:04:04.000000 sparrowApi-0.1.2/sparrowApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-16 07:04:04.000000 sparrowApi-0.1.2/sparrowApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-16 07:04:04.000000 sparrowApi-0.1.2/sparrowApi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 08:54:09.634190 sparrowApi-0.1.3/
+-rw-rw-rw-   0        0        0      142 2024-05-07 08:54:09.632916 sparrowApi-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-07 08:54:09.634744 sparrowApi-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      248 2024-05-07 08:54:04.000000 sparrowApi-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:54:09.624507 sparrowApi-0.1.3/sparrowApi/
+-rw-rw-rw-   0        0        0      504 2024-04-15 01:27:32.000000 sparrowApi-0.1.3/sparrowApi/__init__.py
+-rw-rw-rw-   0        0        0    16326 2024-05-07 08:52:49.000000 sparrowApi-0.1.3/sparrowApi/api.py
+-rw-rw-rw-   0        0        0      825 2024-04-12 08:45:23.000000 sparrowApi-0.1.3/sparrowApi/constant.py
+-rw-rw-rw-   0        0        0     5357 2024-04-15 02:46:23.000000 sparrowApi-0.1.3/sparrowApi/tool_class.py
+drwxrwxrwx   0        0        0        0 2024-05-07 08:54:09.631914 sparrowApi-0.1.3/sparrowApi.egg-info/
+-rw-rw-rw-   0        0        0      142 2024-05-07 08:54:09.000000 sparrowApi-0.1.3/sparrowApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-05-07 08:54:09.000000 sparrowApi-0.1.3/sparrowApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 08:54:09.000000 sparrowApi-0.1.3/sparrowApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 08:54:09.000000 sparrowApi-0.1.3/sparrowApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-07 08:54:09.000000 sparrowApi-0.1.3/sparrowApi.egg-info/top_level.txt
```

### Comparing `sparrowApi-0.1.2/sparrowApi/api.py` & `sparrowApi-0.1.3/sparrowApi/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,21 @@
         """
         self._is_cors_ = is_cors
         self._is_save_log_ = is_save_log
         self._content_type_ = content_type
         self._default_listen_ = default_listen
         self._host_ = host
         self._port_ = port
+        if self._is_save_log_:
+            if log_file == "%s.log":
+                self._log_file_ = "%s.log" % (str(datetime.datetime.now()).split('.')[0].split(' ')[0])
+            else:
+                self._log_file_ = log_file
+            file = open(self._log_file_, "a")
+            file.close()
         if show_register:
             pprint.pprint(self._show_routes_)
         if try_model:
             print(f"* try_model is True")
         else:
             print(Fore.RED + "try_model is False please change True")
         print(f"* {str(datetime.datetime.now()).split('.')[0]} Server SparrowApi started on {self._name_}")
@@ -281,18 +288,14 @@
                 if try_model:
                     try:
                         self._handle_request_(client_socket, addr)
                     except Exception as e:
                         response = 'HTTP/1.1 404 Not Found\r\nContent-Type: */*\r\n\r\nParameter Not Bad'
                         client_socket.sendall(response.encode('utf-8'))
                         client_socket.close()
-                        if log_file == "%s.log":
-                            self._log_file_ = "%s.log" % (str(datetime.datetime.now()).split('.')[0].split(' ')[0])
-                        else:
-                            self._log_file_ = log_file
                         if show_error:
                             print(f"{str(datetime.datetime.now()).split('.')[0]} {e}")
                         self._log_(f"{str(datetime.datetime.now()).split('.')[0]} {e}")
                 else:
                     self._handle_request_(client_socket, addr)
 
     def _decode_url_parameter_(self, url_parameter: str):
```

### Comparing `sparrowApi-0.1.2/sparrowApi/constant.py` & `sparrowApi-0.1.3/sparrowApi/constant.py`

 * *Files identical despite different names*

### Comparing `sparrowApi-0.1.2/sparrowApi/tool_class.py` & `sparrowApi-0.1.3/sparrowApi/tool_class.py`

 * *Files identical despite different names*

