# Comparing `tmp/maritalk-0.2.4.tar.gz` & `tmp/maritalk-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maritalk-0.2.4.tar", last modified: Wed Apr 24 12:03:58 2024, max compression
+gzip compressed data, was "maritalk-0.2.5.tar", last modified: Tue May  7 16:43:29 2024, max compression
```

## Comparing `maritalk-0.2.4.tar` & `maritalk-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:03:58.052019 maritalk-0.2.4/
--rw-rw-r--   0 root         (0) root         (0)     1088 2023-09-04 19:10:06.000000 maritalk-0.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10180 2024-04-24 12:03:58.052019 maritalk-0.2.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8339 2024-04-23 13:50:33.000000 maritalk-0.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:03:58.048020 maritalk-0.2.4/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:03:58.052019 maritalk-0.2.4/examples/local/
--rw-rw-r--   0 root         (0) root         (0)     5374 2024-04-17 16:21:14.000000 maritalk-0.2.4/examples/local/benchmark.py
--rw-rw-r--   0 root         (0) root         (0)      991 2024-04-17 16:21:14.000000 maritalk-0.2.4/examples/local/question_answering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:03:58.052019 maritalk-0.2.4/maritalk/
--rw-rw-r--   0 root         (0) root         (0)      156 2023-12-03 16:28:52.000000 maritalk-0.2.4/maritalk/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1258 2024-04-24 12:00:57.000000 maritalk-0.2.4/maritalk/download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:03:58.052019 maritalk-0.2.4/maritalk/resources/
--rw-rw-r--   0 root         (0) root         (0)     8917 2024-04-17 16:21:11.000000 maritalk-0.2.4/maritalk/resources/api.py
--rw-rw-r--   0 root         (0) root         (0)    14686 2024-04-24 12:00:57.000000 maritalk-0.2.4/maritalk/resources/local.py
--rw-rw-r--   0 root         (0) root         (0)     1050 2024-04-24 12:00:57.000000 maritalk-0.2.4/maritalk/start.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:03:58.052019 maritalk-0.2.4/maritalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10180 2024-04-24 12:03:58.000000 maritalk-0.2.4/maritalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      379 2024-04-24 12:03:58.000000 maritalk-0.2.4/maritalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 12:03:58.000000 maritalk-0.2.4/maritalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-24 12:03:58.000000 maritalk-0.2.4/maritalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-24 12:03:58.000000 maritalk-0.2.4/maritalk.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      721 2024-04-24 12:01:03.000000 maritalk-0.2.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 12:03:58.052019 maritalk-0.2.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)       37 2023-09-04 19:10:06.000000 maritalk-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 16:43:29.923665 maritalk-0.2.5/
+-rw-rw-r--   0 root         (0) root         (0)     1088 2023-09-04 19:10:06.000000 maritalk-0.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10588 2024-05-07 16:43:29.923665 maritalk-0.2.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8746 2024-04-26 10:38:28.000000 maritalk-0.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 16:43:29.919665 maritalk-0.2.5/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 16:43:29.919665 maritalk-0.2.5/examples/local/
+-rw-rw-r--   0 root         (0) root         (0)     5374 2024-04-17 16:21:14.000000 maritalk-0.2.5/examples/local/benchmark.py
+-rw-rw-r--   0 root         (0) root         (0)      991 2024-04-17 16:21:14.000000 maritalk-0.2.5/examples/local/question_answering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 16:43:29.923665 maritalk-0.2.5/maritalk/
+-rw-rw-r--   0 root         (0) root         (0)      156 2023-12-03 16:28:52.000000 maritalk-0.2.5/maritalk/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1284 2024-05-07 16:40:53.000000 maritalk-0.2.5/maritalk/download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 16:43:29.923665 maritalk-0.2.5/maritalk/resources/
+-rw-rw-r--   0 root         (0) root         (0)     8917 2024-04-17 16:21:11.000000 maritalk-0.2.5/maritalk/resources/api.py
+-rw-rw-r--   0 root         (0) root         (0)    14871 2024-05-07 16:40:53.000000 maritalk-0.2.5/maritalk/resources/local.py
+-rw-rw-r--   0 root         (0) root         (0)     1108 2024-05-07 16:40:53.000000 maritalk-0.2.5/maritalk/start.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 16:43:29.923665 maritalk-0.2.5/maritalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10588 2024-05-07 16:43:29.000000 maritalk-0.2.5/maritalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-07 16:43:29.000000 maritalk-0.2.5/maritalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 16:43:29.000000 maritalk-0.2.5/maritalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-07 16:43:29.000000 maritalk-0.2.5/maritalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-07 16:43:29.000000 maritalk-0.2.5/maritalk.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      721 2024-05-07 16:43:18.000000 maritalk-0.2.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 16:43:29.923665 maritalk-0.2.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)       37 2023-09-04 19:10:06.000000 maritalk-0.2.5/setup.py
```

### Comparing `maritalk-0.2.4/LICENSE` & `maritalk-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `maritalk-0.2.4/PKG-INFO` & `maritalk-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maritalk
-Version: 0.2.4
+Version: 0.2.5
 Summary: Client library for the MariTalk API
 Author-email: Maritaca AI <info@maritaca.ai>
 License: The MIT License
         
         Copyright (c) Maritaca AI (https://maritaca.ai)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -227,7 +227,19 @@
 
 # Web Chat
 
 Teste a MariTalk Large via interface web em:
 [chat.maritaca.ai](https://chat.maritaca.ai/)
 
 <img src="https://raw.githubusercontent.com/maritaca-ai/maritalk-api/main/.github/imgs/web-interface.png" width="600">
+
+# Citação
+
+Para referenciar os modelos da família [Sabiá-2](https://www.maritaca.ai/sabia-2), por favor, cite nosso [relatório técnico](https://arxiv.org/abs/2403.09887).
+
+```bibtext
+@article{maritaca2024sabia2,
+  title={Sabi{\'a}-2: A New Generation of Portuguese Large Language Models},
+  author={Sales Almeida, Thales and Abonizio, Hugo and Nogueira, Rodrigo and Pires, Ramon},
+  year={2024}
+}
+```
```

### Comparing `maritalk-0.2.4/README.md` & `maritalk-0.2.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -189,7 +189,19 @@
 
 # Web Chat
 
 Teste a MariTalk Large via interface web em:
 [chat.maritaca.ai](https://chat.maritaca.ai/)
 
 <img src="https://raw.githubusercontent.com/maritaca-ai/maritalk-api/main/.github/imgs/web-interface.png" width="600">
+
+# Citação
+
+Para referenciar os modelos da família [Sabiá-2](https://www.maritaca.ai/sabia-2), por favor, cite nosso [relatório técnico](https://arxiv.org/abs/2403.09887).
+
+```bibtext
+@article{maritaca2024sabia2,
+  title={Sabi{\'a}-2: A New Generation of Portuguese Large Language Models},
+  author={Sales Almeida, Thales and Abonizio, Hugo and Nogueira, Rodrigo and Pires, Ramon},
+  year={2024}
+}
+```
```

### Comparing `maritalk-0.2.4/examples/local/benchmark.py` & `maritalk-0.2.5/examples/local/benchmark.py`

 * *Files identical despite different names*

### Comparing `maritalk-0.2.4/examples/local/question_answering.py` & `maritalk-0.2.5/examples/local/question_answering.py`

 * *Files identical despite different names*

### Comparing `maritalk-0.2.4/maritalk/download.py` & `maritalk-0.2.5/maritalk/download.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,11 +32,12 @@
     dependencies = {"cuda_version": args.cuda or detected_versions["cuda_version"]}
 
     if dependencies["cuda_version"] is None:
         raise Exception(
             "No libcublas.so found. cuBLAS v11 or v12 is required to run MariTalk. You can manually set the version using the `cuda_version` argument."
         )
 
-    bin_folder = os.path.dirname(os.path.expanduser(args.path))
+    args.path = os.path.expanduser(args.path)
+    bin_folder = os.path.dirname(args.path)
     if bin_folder:
         os.makedirs(bin_folder, exist_ok=True)
     download(args.license, args.path, dependencies)
```

### Comparing `maritalk-0.2.4/maritalk/resources/api.py` & `maritalk-0.2.5/maritalk/resources/api.py`

 * *Files identical despite different names*

### Comparing `maritalk-0.2.4/maritalk/resources/local.py` & `maritalk-0.2.5/maritalk/resources/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,26 +183,29 @@
         if bin_folder:
             os.makedirs(bin_folder, exist_ok=True)
         download(license, bin_path, dependencies)
 
     bin_size = _get_file_size(bin_path)
 
     if bin_size:
-        min_memory = 30 if bin_size < 20 else 130
+        min_memory = 20 if bin_size < 20 else 70
         memory_available = _get_total_mem()
         if memory_available and memory_available < min_memory:
             print(
-                "WARNING: Verify that there is enough memory to load the model (at least 30 GB for the small version and 130 GB for the medium version)."
+                "WARNING: Verify that there is enough memory to load the model (at least 20GB for the small version and 70GB for the medium version)."
             )
 
+    env = os.environ.copy()
+    env["DISABLE_LOADING"] = "1"
     args = [bin_path, "--license", license, "--port", str(port)]
     return subprocess.Popen(
         args,
         stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+        env=env,
     )
 
 
 class MariTalkLocal:
     def __init__(self, host: str = "localhost", port: int = 9000):
         self.api_url = f"http://{host}:{port}"
         """@private"""
@@ -240,26 +243,28 @@
                 if self.process.poll() is not None:
                     output, _ = self.process.communicate()
                     output = output.decode("utf-8")
                     raise Exception(
                         f"Failed to start process.\nOutput: {output}\nTry to run it manually: `{' '.join(self.process.args)}`"
                     )
 
-                self.status()
+                response = self.status()
+                if response and response["status"] == "loading":
+                    continue
                 break
             except ConnectionError as ex:
                 time.sleep(1)
 
+        self.loading = False
+        self.loaded = True
+
         if verbose:
             loading_thread.join()
             print()
 
-        self.loading = False
-        self.loaded = True
-
         def terminate():
             print("Stopping MariTalk...")
             self.stop_server()
 
         atexit.register(terminate)
 
     def _show_loading(self):
@@ -270,15 +275,15 @@
         try:
             while self.loading:
                 current_time = time.time()
                 elapsed_time = int(current_time - start_time)
                 minutes, seconds = divmod(elapsed_time, 60)
 
                 output = (
-                    f"\rLoading... {spinner[spinner_index]} ({minutes}min:{seconds}s)"
+                    f"\rLoading... {spinner[spinner_index]} ({minutes}min:{seconds:02d}s)"
                 )
                 sys.stdout.write(output)
                 sys.stdout.flush()
                 spinner_index = (spinner_index + 1) % len(
                     spinner
                 )
                 time.sleep(0.1)
```

### Comparing `maritalk-0.2.4/maritalk/start.py` & `maritalk-0.2.5/maritalk/start.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import atexit
+import time
 import argparse
-from .resources.local import start_server
+from .resources.local import MariTalkLocal
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Start MariTalk Local server.")
     parser.add_argument(
         "--license",
         type=str,
         required=True,
@@ -19,16 +19,20 @@
         choices=[11, 12],
         default=None,
         help="Installed CUDA version.",
     )
     parser.add_argument("--port", type=int, default=9000, help="The HTTP port to bind.")
     args = parser.parse_args()
 
-    process = start_server(args.license, args.path, args.cuda, args.port)
-    atexit.register(lambda: process.terminate())
+    client = MariTalkLocal(port=args.port)
+    client.start_server(
+        license=args.license,
+        bin_path=args.path,
+        cuda_version=args.cuda,
+    )
 
     while True:
-        output = process.stdout.readline()
-        if process.poll() is not None and output == b"":
+        output = client.process.stdout.readline()
+        if client.process.poll() is not None and output == b"":
             break
         if output:
-            print(output.decode().strip(), end='')
+            print(output.decode(), end='', flush=True)
```

### Comparing `maritalk-0.2.4/maritalk.egg-info/PKG-INFO` & `maritalk-0.2.5/maritalk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maritalk
-Version: 0.2.4
+Version: 0.2.5
 Summary: Client library for the MariTalk API
 Author-email: Maritaca AI <info@maritaca.ai>
 License: The MIT License
         
         Copyright (c) Maritaca AI (https://maritaca.ai)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -227,7 +227,19 @@
 
 # Web Chat
 
 Teste a MariTalk Large via interface web em:
 [chat.maritaca.ai](https://chat.maritaca.ai/)
 
 <img src="https://raw.githubusercontent.com/maritaca-ai/maritalk-api/main/.github/imgs/web-interface.png" width="600">
+
+# Citação
+
+Para referenciar os modelos da família [Sabiá-2](https://www.maritaca.ai/sabia-2), por favor, cite nosso [relatório técnico](https://arxiv.org/abs/2403.09887).
+
+```bibtext
+@article{maritaca2024sabia2,
+  title={Sabi{\'a}-2: A New Generation of Portuguese Large Language Models},
+  author={Sales Almeida, Thales and Abonizio, Hugo and Nogueira, Rodrigo and Pires, Ramon},
+  year={2024}
+}
+```
```

### Comparing `maritalk-0.2.4/pyproject.toml` & `maritalk-0.2.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maritalk"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Maritaca AI", email="info@maritaca.ai" },
 ]
 description = "Client library for the MariTalk API"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
```

