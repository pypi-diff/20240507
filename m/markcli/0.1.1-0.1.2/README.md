# Comparing `tmp/markcli-0.1.1.tar.gz` & `tmp/markcli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markcli-0.1.1.tar", last modified: Sun May  5 06:07:14 2024, max compression
+gzip compressed data, was "markcli-0.1.2.tar", last modified: Tue May  7 04:55:30 2024, max compression
```

## Comparing `markcli-0.1.1.tar` & `markcli-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:07:14.815812 markcli-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 06:07:11.000000 markcli-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16603 2024-05-05 06:07:14.815812 markcli-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-05-05 06:07:11.000000 markcli-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:07:14.815812 markcli-0.1.1/markcli/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-05 06:07:11.000000 markcli-0.1.1/markcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-05 06:07:11.000000 markcli-0.1.1/markcli/markcli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:07:14.815812 markcli-0.1.1/markcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16603 2024-05-05 06:07:14.000000 markcli-0.1.1/markcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-05 06:07:14.000000 markcli-0.1.1/markcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 06:07:14.000000 markcli-0.1.1/markcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 06:07:14.000000 markcli-0.1.1/markcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 06:07:14.000000 markcli-0.1.1/markcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 06:07:14.000000 markcli-0.1.1/markcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 06:07:14.815812 markcli-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-05 06:07:11.000000 markcli-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:55:30.259361 markcli-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 04:55:26.000000 markcli-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17565 2024-05-07 04:55:30.259361 markcli-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16974 2024-05-07 04:55:26.000000 markcli-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:55:30.259361 markcli-0.1.2/markcli/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 04:55:26.000000 markcli-0.1.2/markcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-07 04:55:26.000000 markcli-0.1.2/markcli/markcli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:55:30.259361 markcli-0.1.2/markcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17565 2024-05-07 04:55:30.000000 markcli-0.1.2/markcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-07 04:55:30.000000 markcli-0.1.2/markcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 04:55:30.000000 markcli-0.1.2/markcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 04:55:30.000000 markcli-0.1.2/markcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 04:55:30.000000 markcli-0.1.2/markcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 04:55:30.000000 markcli-0.1.2/markcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 04:55:30.259361 markcli-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 04:55:26.000000 markcli-0.1.2/setup.py
```

### Comparing `markcli-0.1.1/LICENSE` & `markcli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markcli-0.1.1/PKG-INFO` & `markcli-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markcli
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Jupyter-inspired tool to create documentation of CLI tools.
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -32,15 +32,15 @@
 ```json
 {
     "command": "some bash command"
 }
 ```
 
  with the following properties (first option is default)
-```json
+```javascript
 {
     "command": "ls -lt",
     "print_command": false/true             // print the command in the document
     "output-format": "bash"/code block id   // Any value supported by md code blocks (e.g. json, python, etc.)
     "limit": 0/any number                   // limit the number of lines printed
     "error-strategy": "ignore"\"exit",      // Behavior on error
     "skip": false/true,                     // If true, this command is not run. If true, it is run, and if the following block is an output (of a previous command), it is updated.
@@ -57,21 +57,20 @@
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 ls -lt
 ```
 ```bash
-total 40
--rw-r--r--  1 danielnebenzahl  staff      0 May  5 09:02 README.md
--rw-r--r--  1 danielnebenzahl  staff   2776 May  5 09:02 template.md
-drwxr-xr-x  4 danielnebenzahl  staff    128 May  5 08:56 templates
--rw-r--r--  1 danielnebenzahl  staff   1065 May  5 08:55 setup.py
-drwxr-xr-x  4 danielnebenzahl  staff    128 May  5 08:55 markcli
--rw-r--r--  1 danielnebenzahl  staff  11357 May  5 08:55 LICENSE
+total 24
+-rw-r--r-- 1 runner docker     0 May  7 04:54 README.md
+-rw-r--r-- 1 runner docker 11357 May  7 04:54 LICENSE
+drwxr-xr-x 2 runner docker  4096 May  7 04:54 markcli
+-rw-r--r-- 1 runner docker  1065 May  7 04:54 setup.py
+-rw-r--r-- 1 runner docker  2982 May  7 04:54 template.md
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 Commands can use environment variables, the parser assumes that any capitalized word is an environemnt variable. Example:
 <!--
 {
@@ -80,15 +79,15 @@
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 echo $HOME
 ```
 ```bash
-/Users/danielnebenzahl
+/home/runner
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 There are two options to handle errors: To include the error code as the result of running the command, or to exit the document creation process. 
 <!--
 {
@@ -97,15 +96,15 @@
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 ec ho $HOME
 ```
 ```bash
-/bin/sh: ec: command not found
+/bin/sh: 1: ec: not found
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 Using the `"skip": true` option, the command is not run. This is useful for commands that consume a lot of time or resources, and is adequate for cases where the work on the file is interactive (the inputfile is also the outputfile)
 
 The output-fomat can be any format supported by markdown code blocks like `json`, `yml`. The default is `bash`. The output can be limited to a specific number of lines, using the `limit` option. Following is an example of using the `python` format and a limit:
@@ -145,23 +144,47 @@
 ```
 
 Then the command `markcli` will be available.
 
 # A real-world example: document the valint command:
 
 ## Intall valint
-To install valint run:
+To install valint run (Note that the -- 2>&1 is required to capture the output in this setting, but is not required in a normal shell):
+<!--
+{
+    "command": "curl -sSfL https://get.scribesecurity.com/install.sh  | sh -s -- -t valint -D -- 2>&1",
+    "print_command": true
+}
+-->
+<!-- { "object-type": "command-output-start" } -->
 ```bash
-curl -sSfL https://get.scribesecurity.com/install.sh  | sh -s -- -t valint -D",
+curl -sSfL https://get.scribesecurity.com/install.sh  | sh -s -- -t valint -D -- 2>&1
 ```
+```bash
+scribe info Installer - Scribe CLI tools
+scribe info Selected, tool=valint, version=latest
+scribe info Trying to download, tool=valint, version=latest
+scribe info Using dev artifacts, subpath='dev/valint/linux/amd64', ENV=dev
+scribe info Downloading, Version=1.4.0-6
+  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
+                                 Dload  Upload   Total   Spent    Left  Speed
+
+  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
+ 85 28.5M   85 24.4M    0     0  44.1M      0 --:--:-- --:--:-- --:--:-- 44.1M
+100 28.5M  100 28.5M    0     0  47.0M      0 --:--:-- --:--:-- --:--:-- 46.9M
+scribe info Installed /home/runner/.scribe/bin/valint
+
+```
+<!-- { "object-type": "command-output-end" } -->
+
 
 ## General options
 <!--
 {
-    "command": "valint --help"
+    "command": "$HOME/.scribe/bin/valint --help"
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 Command Line Interpreter (CLI) tool,that empowers supply chain stakeholders to ensure supply chain integrity, verify compliance, and generate and manage evidence.
 
 Usage:
@@ -205,15 +228,15 @@
       --key string                    x509 Private key path
   -L, --label strings                 Add Custom labels
   -D, --level string                  Log depth level, options=[panic fatal error warning info debug trace]
       --log-context                   Attach context to all logs
       --log-file string               Output log to file
       --oci                           Enable OCI store
   -R, --oci-repo string               Select OCI custom attestation repo
-  -d, --output-directory string       Output directory path (default "/Users/danielnebenzahl/Library/Caches/valint")
+  -d, --output-directory string       Output directory path (default "/home/runner/.cache/valint")
   -O, --output-file string            Output file name
   -p, --pipeline-name string          Pipeline name
       --platform string               Select target platform, examples=windows/armv6, arm64 ..)
       --predicate-type string         Custom Predicate type (generic evidence format) (default "http://scribesecurity.com/evidence/generic/v0.1")
   -n, --product-key string            Product Key
   -V, --product-version string        Product Version
   -q, --quiet                         Suppress all logging output
@@ -232,15 +255,15 @@
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 ## Bom command
 <!--
 {
-    "command": "valint bom --help"
+    "command": "$HOME/.scribe/bin/valint bom --help"
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 Collect, Create and Store evidence for artifacts (SBOMs,SLSA provenance) or any third-party tools.
 
 Usage:
@@ -336,15 +359,15 @@
       --key string                    x509 Private key path
   -L, --label strings                 Add Custom labels
   -D, --level string                  Log depth level, options=[panic fatal error warning info debug trace]
       --log-context                   Attach context to all logs
       --log-file string               Output log to file
       --oci                           Enable OCI store
   -R, --oci-repo string               Select OCI custom attestation repo
-  -d, --output-directory string       Output directory path (default "/Users/danielnebenzahl/Library/Caches/valint")
+  -d, --output-directory string       Output directory path (default "/home/runner/.cache/valint")
   -O, --output-file string            Output file name
   -p, --pipeline-name string          Pipeline name
       --platform string               Select target platform, examples=windows/armv6, arm64 ..)
       --predicate-type string         Custom Predicate type (generic evidence format) (default "http://scribesecurity.com/evidence/generic/v0.1")
   -n, --product-key string            Product Key
   -V, --product-version string        Product Version
   -q, --quiet                         Suppress all logging output
```

### Comparing `markcli-0.1.1/README.md` & `markcli-0.1.2/markcli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: markcli
+Version: 0.1.2
+Summary: A Jupyter-inspired tool to create documentation of CLI tools.
+Home-page: UNKNOWN
+License: Apache License 2.0
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # `markcli` - An Jupyter-inspired CLI Documentation Tool
 
 ## Description
 Run markcli to fill a template that results from running the cli command included inside.
 
 CLI commands are written in html comments (here with sapces added to avoid rendering) using the following syntax:
 
@@ -15,15 +32,15 @@
 ```json
 {
     "command": "some bash command"
 }
 ```
 
  with the following properties (first option is default)
-```json
+```javascript
 {
     "command": "ls -lt",
     "print_command": false/true             // print the command in the document
     "output-format": "bash"/code block id   // Any value supported by md code blocks (e.g. json, python, etc.)
     "limit": 0/any number                   // limit the number of lines printed
     "error-strategy": "ignore"\"exit",      // Behavior on error
     "skip": false/true,                     // If true, this command is not run. If true, it is run, and if the following block is an output (of a previous command), it is updated.
@@ -40,21 +57,20 @@
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 ls -lt
 ```
 ```bash
-total 40
--rw-r--r--  1 danielnebenzahl  staff      0 May  5 09:02 README.md
--rw-r--r--  1 danielnebenzahl  staff   2776 May  5 09:02 template.md
-drwxr-xr-x  4 danielnebenzahl  staff    128 May  5 08:56 templates
--rw-r--r--  1 danielnebenzahl  staff   1065 May  5 08:55 setup.py
-drwxr-xr-x  4 danielnebenzahl  staff    128 May  5 08:55 markcli
--rw-r--r--  1 danielnebenzahl  staff  11357 May  5 08:55 LICENSE
+total 24
+-rw-r--r-- 1 runner docker     0 May  7 04:54 README.md
+-rw-r--r-- 1 runner docker 11357 May  7 04:54 LICENSE
+drwxr-xr-x 2 runner docker  4096 May  7 04:54 markcli
+-rw-r--r-- 1 runner docker  1065 May  7 04:54 setup.py
+-rw-r--r-- 1 runner docker  2982 May  7 04:54 template.md
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 Commands can use environment variables, the parser assumes that any capitalized word is an environemnt variable. Example:
 <!--
 {
@@ -63,15 +79,15 @@
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 echo $HOME
 ```
 ```bash
-/Users/danielnebenzahl
+/home/runner
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 There are two options to handle errors: To include the error code as the result of running the command, or to exit the document creation process. 
 <!--
 {
@@ -80,15 +96,15 @@
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 ec ho $HOME
 ```
 ```bash
-/bin/sh: ec: command not found
+/bin/sh: 1: ec: not found
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 Using the `"skip": true` option, the command is not run. This is useful for commands that consume a lot of time or resources, and is adequate for cases where the work on the file is interactive (the inputfile is also the outputfile)
 
 The output-fomat can be any format supported by markdown code blocks like `json`, `yml`. The default is `bash`. The output can be limited to a specific number of lines, using the `limit` option. Following is an example of using the `python` format and a limit:
@@ -128,23 +144,47 @@
 ```
 
 Then the command `markcli` will be available.
 
 # A real-world example: document the valint command:
 
 ## Intall valint
-To install valint run:
+To install valint run (Note that the -- 2>&1 is required to capture the output in this setting, but is not required in a normal shell):
+<!--
+{
+    "command": "curl -sSfL https://get.scribesecurity.com/install.sh  | sh -s -- -t valint -D -- 2>&1",
+    "print_command": true
+}
+-->
+<!-- { "object-type": "command-output-start" } -->
 ```bash
-curl -sSfL https://get.scribesecurity.com/install.sh  | sh -s -- -t valint -D",
+curl -sSfL https://get.scribesecurity.com/install.sh  | sh -s -- -t valint -D -- 2>&1
 ```
+```bash
+scribe info Installer - Scribe CLI tools
+scribe info Selected, tool=valint, version=latest
+scribe info Trying to download, tool=valint, version=latest
+scribe info Using dev artifacts, subpath='dev/valint/linux/amd64', ENV=dev
+scribe info Downloading, Version=1.4.0-6
+  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
+                                 Dload  Upload   Total   Spent    Left  Speed
+
+  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
+ 85 28.5M   85 24.4M    0     0  44.1M      0 --:--:-- --:--:-- --:--:-- 44.1M
+100 28.5M  100 28.5M    0     0  47.0M      0 --:--:-- --:--:-- --:--:-- 46.9M
+scribe info Installed /home/runner/.scribe/bin/valint
+
+```
+<!-- { "object-type": "command-output-end" } -->
+
 
 ## General options
 <!--
 {
-    "command": "valint --help"
+    "command": "$HOME/.scribe/bin/valint --help"
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 Command Line Interpreter (CLI) tool,that empowers supply chain stakeholders to ensure supply chain integrity, verify compliance, and generate and manage evidence.
 
 Usage:
@@ -188,15 +228,15 @@
       --key string                    x509 Private key path
   -L, --label strings                 Add Custom labels
   -D, --level string                  Log depth level, options=[panic fatal error warning info debug trace]
       --log-context                   Attach context to all logs
       --log-file string               Output log to file
       --oci                           Enable OCI store
   -R, --oci-repo string               Select OCI custom attestation repo
-  -d, --output-directory string       Output directory path (default "/Users/danielnebenzahl/Library/Caches/valint")
+  -d, --output-directory string       Output directory path (default "/home/runner/.cache/valint")
   -O, --output-file string            Output file name
   -p, --pipeline-name string          Pipeline name
       --platform string               Select target platform, examples=windows/armv6, arm64 ..)
       --predicate-type string         Custom Predicate type (generic evidence format) (default "http://scribesecurity.com/evidence/generic/v0.1")
   -n, --product-key string            Product Key
   -V, --product-version string        Product Version
   -q, --quiet                         Suppress all logging output
@@ -215,15 +255,15 @@
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 ## Bom command
 <!--
 {
-    "command": "valint bom --help"
+    "command": "$HOME/.scribe/bin/valint bom --help"
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 Collect, Create and Store evidence for artifacts (SBOMs,SLSA provenance) or any third-party tools.
 
 Usage:
@@ -319,15 +359,15 @@
       --key string                    x509 Private key path
   -L, --label strings                 Add Custom labels
   -D, --level string                  Log depth level, options=[panic fatal error warning info debug trace]
       --log-context                   Attach context to all logs
       --log-file string               Output log to file
       --oci                           Enable OCI store
   -R, --oci-repo string               Select OCI custom attestation repo
-  -d, --output-directory string       Output directory path (default "/Users/danielnebenzahl/Library/Caches/valint")
+  -d, --output-directory string       Output directory path (default "/home/runner/.cache/valint")
   -O, --output-file string            Output file name
   -p, --pipeline-name string          Pipeline name
       --platform string               Select target platform, examples=windows/armv6, arm64 ..)
       --predicate-type string         Custom Predicate type (generic evidence format) (default "http://scribesecurity.com/evidence/generic/v0.1")
   -n, --product-key string            Product Key
   -V, --product-version string        Product Version
   -q, --quiet                         Suppress all logging output
@@ -340,7 +380,9 @@
       --structured                    Enable structured logger
       --timeout string                Timeout duration (default "120s")
   -v, --verbose count                 Log verbosity level [-v,--verbose=1] = info, [-vv,--verbose=2] = debug
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
+
+
```

### Comparing `markcli-0.1.1/markcli/markcli.py` & `markcli-0.1.2/markcli/markcli.py`

 * *Files identical despite different names*

### Comparing `markcli-0.1.1/markcli.egg-info/PKG-INFO` & `markcli-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: markcli
-Version: 0.1.1
-Summary: A Jupyter-inspired tool to create documentation of CLI tools.
-Home-page: UNKNOWN
-License: Apache License 2.0
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # `markcli` - An Jupyter-inspired CLI Documentation Tool
 
 ## Description
 Run markcli to fill a template that results from running the cli command included inside.
 
 CLI commands are written in html comments (here with sapces added to avoid rendering) using the following syntax:
 
@@ -32,15 +15,15 @@
 ```json
 {
     "command": "some bash command"
 }
 ```
 
  with the following properties (first option is default)
-```json
+```javascript
 {
     "command": "ls -lt",
     "print_command": false/true             // print the command in the document
     "output-format": "bash"/code block id   // Any value supported by md code blocks (e.g. json, python, etc.)
     "limit": 0/any number                   // limit the number of lines printed
     "error-strategy": "ignore"\"exit",      // Behavior on error
     "skip": false/true,                     // If true, this command is not run. If true, it is run, and if the following block is an output (of a previous command), it is updated.
@@ -57,21 +40,20 @@
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 ls -lt
 ```
 ```bash
-total 40
--rw-r--r--  1 danielnebenzahl  staff      0 May  5 09:02 README.md
--rw-r--r--  1 danielnebenzahl  staff   2776 May  5 09:02 template.md
-drwxr-xr-x  4 danielnebenzahl  staff    128 May  5 08:56 templates
--rw-r--r--  1 danielnebenzahl  staff   1065 May  5 08:55 setup.py
-drwxr-xr-x  4 danielnebenzahl  staff    128 May  5 08:55 markcli
--rw-r--r--  1 danielnebenzahl  staff  11357 May  5 08:55 LICENSE
+total 24
+-rw-r--r-- 1 runner docker     0 May  7 04:54 README.md
+-rw-r--r-- 1 runner docker 11357 May  7 04:54 LICENSE
+drwxr-xr-x 2 runner docker  4096 May  7 04:54 markcli
+-rw-r--r-- 1 runner docker  1065 May  7 04:54 setup.py
+-rw-r--r-- 1 runner docker  2982 May  7 04:54 template.md
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 Commands can use environment variables, the parser assumes that any capitalized word is an environemnt variable. Example:
 <!--
 {
@@ -80,15 +62,15 @@
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 echo $HOME
 ```
 ```bash
-/Users/danielnebenzahl
+/home/runner
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 There are two options to handle errors: To include the error code as the result of running the command, or to exit the document creation process. 
 <!--
 {
@@ -97,15 +79,15 @@
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 ec ho $HOME
 ```
 ```bash
-/bin/sh: ec: command not found
+/bin/sh: 1: ec: not found
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 Using the `"skip": true` option, the command is not run. This is useful for commands that consume a lot of time or resources, and is adequate for cases where the work on the file is interactive (the inputfile is also the outputfile)
 
 The output-fomat can be any format supported by markdown code blocks like `json`, `yml`. The default is `bash`. The output can be limited to a specific number of lines, using the `limit` option. Following is an example of using the `python` format and a limit:
@@ -145,23 +127,47 @@
 ```
 
 Then the command `markcli` will be available.
 
 # A real-world example: document the valint command:
 
 ## Intall valint
-To install valint run:
+To install valint run (Note that the -- 2>&1 is required to capture the output in this setting, but is not required in a normal shell):
+<!--
+{
+    "command": "curl -sSfL https://get.scribesecurity.com/install.sh  | sh -s -- -t valint -D -- 2>&1",
+    "print_command": true
+}
+-->
+<!-- { "object-type": "command-output-start" } -->
 ```bash
-curl -sSfL https://get.scribesecurity.com/install.sh  | sh -s -- -t valint -D",
+curl -sSfL https://get.scribesecurity.com/install.sh  | sh -s -- -t valint -D -- 2>&1
 ```
+```bash
+scribe info Installer - Scribe CLI tools
+scribe info Selected, tool=valint, version=latest
+scribe info Trying to download, tool=valint, version=latest
+scribe info Using dev artifacts, subpath='dev/valint/linux/amd64', ENV=dev
+scribe info Downloading, Version=1.4.0-6
+  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
+                                 Dload  Upload   Total   Spent    Left  Speed
+
+  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
+ 85 28.5M   85 24.4M    0     0  44.1M      0 --:--:-- --:--:-- --:--:-- 44.1M
+100 28.5M  100 28.5M    0     0  47.0M      0 --:--:-- --:--:-- --:--:-- 46.9M
+scribe info Installed /home/runner/.scribe/bin/valint
+
+```
+<!-- { "object-type": "command-output-end" } -->
+
 
 ## General options
 <!--
 {
-    "command": "valint --help"
+    "command": "$HOME/.scribe/bin/valint --help"
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 Command Line Interpreter (CLI) tool,that empowers supply chain stakeholders to ensure supply chain integrity, verify compliance, and generate and manage evidence.
 
 Usage:
@@ -205,15 +211,15 @@
       --key string                    x509 Private key path
   -L, --label strings                 Add Custom labels
   -D, --level string                  Log depth level, options=[panic fatal error warning info debug trace]
       --log-context                   Attach context to all logs
       --log-file string               Output log to file
       --oci                           Enable OCI store
   -R, --oci-repo string               Select OCI custom attestation repo
-  -d, --output-directory string       Output directory path (default "/Users/danielnebenzahl/Library/Caches/valint")
+  -d, --output-directory string       Output directory path (default "/home/runner/.cache/valint")
   -O, --output-file string            Output file name
   -p, --pipeline-name string          Pipeline name
       --platform string               Select target platform, examples=windows/armv6, arm64 ..)
       --predicate-type string         Custom Predicate type (generic evidence format) (default "http://scribesecurity.com/evidence/generic/v0.1")
   -n, --product-key string            Product Key
   -V, --product-version string        Product Version
   -q, --quiet                         Suppress all logging output
@@ -232,15 +238,15 @@
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
 ## Bom command
 <!--
 {
-    "command": "valint bom --help"
+    "command": "$HOME/.scribe/bin/valint bom --help"
 }
 -->
 <!-- { "object-type": "command-output-start" } -->
 ```bash
 Collect, Create and Store evidence for artifacts (SBOMs,SLSA provenance) or any third-party tools.
 
 Usage:
@@ -336,15 +342,15 @@
       --key string                    x509 Private key path
   -L, --label strings                 Add Custom labels
   -D, --level string                  Log depth level, options=[panic fatal error warning info debug trace]
       --log-context                   Attach context to all logs
       --log-file string               Output log to file
       --oci                           Enable OCI store
   -R, --oci-repo string               Select OCI custom attestation repo
-  -d, --output-directory string       Output directory path (default "/Users/danielnebenzahl/Library/Caches/valint")
+  -d, --output-directory string       Output directory path (default "/home/runner/.cache/valint")
   -O, --output-file string            Output file name
   -p, --pipeline-name string          Pipeline name
       --platform string               Select target platform, examples=windows/armv6, arm64 ..)
       --predicate-type string         Custom Predicate type (generic evidence format) (default "http://scribesecurity.com/evidence/generic/v0.1")
   -n, --product-key string            Product Key
   -V, --product-version string        Product Version
   -q, --quiet                         Suppress all logging output
@@ -357,9 +363,7 @@
       --structured                    Enable structured logger
       --timeout string                Timeout duration (default "120s")
   -v, --verbose count                 Log verbosity level [-v,--verbose=1] = info, [-vv,--verbose=2] = debug
 ```
 <!-- { "object-type": "command-output-end" } -->
 
 
-
-
```

### Comparing `markcli-0.1.1/setup.py` & `markcli-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as readme:
         description = readme.read()
 
 setup(
     name='markcli',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'jsonargparse',
     ],
     python_requires='>=3.8',
     description="A Jupyter-inspired tool to create documentation of CLI tools.",
     license='Apache License 2.0',
```

