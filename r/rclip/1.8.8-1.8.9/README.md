# Comparing `tmp/rclip-1.8.8.tar.gz` & `tmp/rclip-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.8.8.tar", max compression
+gzip compressed data, was "rclip-1.8.9.tar", max compression
```

## Comparing `rclip-1.8.8.tar` & `rclip-1.8.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2024-04-14 10:01:58.634620 rclip-1.8.8/LICENSE
--rw-r--r--   0        0        0     7269 2024-04-14 10:01:58.638620 rclip-1.8.8/README.md
--rw-r--r--   0        0        0     1747 2024-04-14 10:01:58.638620 rclip-1.8.8/pyproject.toml
--rw-r--r--   0        0        0      158 2024-04-14 10:01:58.638620 rclip-1.8.8/rclip/const.py
--rw-r--r--   0        0        0     3895 2024-04-14 10:01:58.638620 rclip-1.8.8/rclip/db.py
--rw-r--r--   0        0        0      993 2024-04-14 10:01:58.638620 rclip-1.8.8/rclip/fs.py
--rw-r--r--   0        0        0     7093 2024-04-14 10:01:58.638620 rclip-1.8.8/rclip/main.py
--rw-r--r--   0        0        0     5412 2024-04-14 10:01:58.638620 rclip-1.8.8/rclip/model.py
--rw-r--r--   0        0        0     7230 2024-04-14 10:01:58.638620 rclip-1.8.8/rclip/utils/helpers.py
--rw-r--r--   0        0        0     1169 2024-04-14 10:01:58.638620 rclip-1.8.8/rclip/utils/preview.py
--rw-r--r--   0        0        0     1726 2024-04-14 10:01:58.638620 rclip-1.8.8/rclip/utils/snap.py
--rw-r--r--   0        0        0     8911 1970-01-01 00:00:00.000000 rclip-1.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-05 09:02:05.474130 rclip-1.8.9/LICENSE
+-rw-r--r--   0        0        0     7313 2024-05-05 09:02:05.474130 rclip-1.8.9/README.md
+-rw-r--r--   0        0        0     1747 2024-05-05 09:02:05.474130 rclip-1.8.9/pyproject.toml
+-rw-r--r--   0        0        0      158 2024-05-05 09:02:05.474130 rclip-1.8.9/rclip/const.py
+-rw-r--r--   0        0        0     3895 2024-05-05 09:02:05.478131 rclip-1.8.9/rclip/db.py
+-rw-r--r--   0        0        0      993 2024-05-05 09:02:05.478131 rclip-1.8.9/rclip/fs.py
+-rw-r--r--   0        0        0     7093 2024-05-05 09:02:05.478131 rclip-1.8.9/rclip/main.py
+-rw-r--r--   0        0        0     5412 2024-05-05 09:02:05.478131 rclip-1.8.9/rclip/model.py
+-rw-r--r--   0        0        0     7230 2024-05-05 09:02:05.478131 rclip-1.8.9/rclip/utils/helpers.py
+-rw-r--r--   0        0        0     1169 2024-05-05 09:02:05.478131 rclip-1.8.9/rclip/utils/preview.py
+-rw-r--r--   0        0        0     1726 2024-05-05 09:02:05.478131 rclip-1.8.9/rclip/utils/snap.py
+-rw-r--r--   0        0        0     8955 1970-01-01 00:00:00.000000 rclip-1.8.9/PKG-INFO
```

### Comparing `rclip-1.8.8/LICENSE` & `rclip-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.8.8/README.md` & `rclip-1.8.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -132,19 +132,17 @@
   I prefer to use **feh**'s thumbnail mode to preview multiple results:
 
   ```bash
   rclip -f -t 5 kitty | feh -f - -t
   ```
 </details>
 
-## Help
+## Get help
 
-```bash
-rclip --help
-```
+https://github.com/yurijmikhalevich/rclip/discussions/new/choose
 
 ## Contributing
 
 This repository follows the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) standard.
 
 ### Running locally from the source code
```

### Comparing `rclip-1.8.8/pyproject.toml` & `rclip-1.8.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.8.8"
+version = "1.8.9"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
```

### Comparing `rclip-1.8.8/rclip/db.py` & `rclip-1.8.9/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.8/rclip/fs.py` & `rclip-1.8.9/rclip/fs.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.8/rclip/main.py` & `rclip-1.8.9/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.8/rclip/model.py` & `rclip-1.8.9/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.8/rclip/utils/helpers.py` & `rclip-1.8.9/rclip/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.8/rclip/utils/preview.py` & `rclip-1.8.9/rclip/utils/preview.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.8/rclip/utils/snap.py` & `rclip-1.8.9/rclip/utils/snap.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.8/PKG-INFO` & `rclip-1.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.8.8
+Version: 1.8.9
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.9,<3.13
@@ -166,19 +166,17 @@
   I prefer to use **feh**'s thumbnail mode to preview multiple results:
 
   ```bash
   rclip -f -t 5 kitty | feh -f - -t
   ```
 </details>
 
-## Help
+## Get help
 
-```bash
-rclip --help
-```
+https://github.com/yurijmikhalevich/rclip/discussions/new/choose
 
 ## Contributing
 
 This repository follows the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) standard.
 
 ### Running locally from the source code
```

