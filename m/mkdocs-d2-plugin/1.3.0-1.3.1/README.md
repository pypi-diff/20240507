# Comparing `tmp/mkdocs-d2-plugin-1.3.0.tar.gz` & `tmp/mkdocs_d2_plugin-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-d2-plugin-1.3.0.tar", last modified: Sun Mar 31 10:12:32 2024, max compression
+gzip compressed data, was "mkdocs_d2_plugin-1.3.1.tar", last modified: Tue May  7 15:46:30 2024, max compression
```

## Comparing `mkdocs-d2-plugin-1.3.0.tar` & `mkdocs_d2_plugin-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-03-31 10:12:32.022076 mkdocs-d2-plugin-1.3.0/
--rw-r--r--   0 landmaj    (501) staff       (20)     1061 2023-10-13 12:03:14.000000 mkdocs-d2-plugin-1.3.0/LICENSE
--rw-r--r--   0 landmaj    (501) staff       (20)     2170 2024-03-31 10:12:32.021798 mkdocs-d2-plugin-1.3.0/PKG-INFO
--rw-r--r--   0 landmaj    (501) staff       (20)     1153 2023-12-22 12:42:30.000000 mkdocs-d2-plugin-1.3.0/README.md
-drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-03-31 10:12:32.019986 mkdocs-d2-plugin-1.3.0/d2/
--rw-r--r--   0 landmaj    (501) staff       (20)      318 2023-12-22 12:42:30.000000 mkdocs-d2-plugin-1.3.0/d2/__init__.py
--rw-r--r--   0 landmaj    (501) staff       (20)     1729 2024-03-31 09:59:35.000000 mkdocs-d2-plugin-1.3.0/d2/config.py
--rw-r--r--   0 landmaj    (501) staff       (20)     1713 2023-12-22 12:42:30.000000 mkdocs-d2-plugin-1.3.0/d2/fence.py
--rw-r--r--   0 landmaj    (501) staff       (20)     2554 2023-12-22 12:42:30.000000 mkdocs-d2-plugin-1.3.0/d2/img.py
--rw-r--r--   0 landmaj    (501) staff       (20)     3674 2024-03-21 19:04:06.000000 mkdocs-d2-plugin-1.3.0/d2/plugin.py
-drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-03-31 10:12:32.021511 mkdocs-d2-plugin-1.3.0/mkdocs_d2_plugin.egg-info/
--rw-r--r--   0 landmaj    (501) staff       (20)     2170 2024-03-31 10:12:32.000000 mkdocs-d2-plugin-1.3.0/mkdocs_d2_plugin.egg-info/PKG-INFO
--rw-r--r--   0 landmaj    (501) staff       (20)      331 2024-03-31 10:12:32.000000 mkdocs-d2-plugin-1.3.0/mkdocs_d2_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 landmaj    (501) staff       (20)        1 2024-03-31 10:12:32.000000 mkdocs-d2-plugin-1.3.0/mkdocs_d2_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 landmaj    (501) staff       (20)       93 2024-03-31 10:12:32.000000 mkdocs-d2-plugin-1.3.0/mkdocs_d2_plugin.egg-info/entry_points.txt
--rw-r--r--   0 landmaj    (501) staff       (20)       62 2024-03-31 10:12:32.000000 mkdocs-d2-plugin-1.3.0/mkdocs_d2_plugin.egg-info/requires.txt
--rw-r--r--   0 landmaj    (501) staff       (20)        3 2024-03-31 10:12:32.000000 mkdocs-d2-plugin-1.3.0/mkdocs_d2_plugin.egg-info/top_level.txt
--rw-r--r--   0 landmaj    (501) staff       (20)       38 2024-03-31 10:12:32.022130 mkdocs-d2-plugin-1.3.0/setup.cfg
--rw-r--r--   0 landmaj    (501) staff       (20)     1492 2024-03-31 10:10:48.000000 mkdocs-d2-plugin-1.3.0/setup.py
+drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-07 15:46:30.104122 mkdocs_d2_plugin-1.3.1/
+-rw-r--r--   0 landmaj    (501) staff       (20)     1061 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.3.1/LICENSE
+-rw-r--r--   0 landmaj    (501) staff       (20)     2170 2024-05-07 15:46:30.103923 mkdocs_d2_plugin-1.3.1/PKG-INFO
+-rw-r--r--   0 landmaj    (501) staff       (20)     1153 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.3.1/README.md
+drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-07 15:46:30.102620 mkdocs_d2_plugin-1.3.1/d2/
+-rw-r--r--   0 landmaj    (501) staff       (20)      318 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.3.1/d2/__init__.py
+-rw-r--r--   0 landmaj    (501) staff       (20)     1729 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.3.1/d2/config.py
+-rw-r--r--   0 landmaj    (501) staff       (20)     1713 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.3.1/d2/fence.py
+-rw-r--r--   0 landmaj    (501) staff       (20)     2556 2024-05-07 15:26:23.000000 mkdocs_d2_plugin-1.3.1/d2/img.py
+-rw-r--r--   0 landmaj    (501) staff       (20)     3674 2024-05-03 14:53:55.000000 mkdocs_d2_plugin-1.3.1/d2/plugin.py
+drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-07 15:46:30.103720 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/
+-rw-r--r--   0 landmaj    (501) staff       (20)     2170 2024-05-07 15:46:30.000000 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 landmaj    (501) staff       (20)      331 2024-05-07 15:46:30.000000 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)        1 2024-05-07 15:46:30.000000 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)       93 2024-05-07 15:46:30.000000 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)       62 2024-05-07 15:46:30.000000 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/requires.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)        3 2024-05-07 15:46:30.000000 mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/top_level.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)       38 2024-05-07 15:46:30.104167 mkdocs_d2_plugin-1.3.1/setup.cfg
+-rw-r--r--   0 landmaj    (501) staff       (20)     1492 2024-05-07 15:27:11.000000 mkdocs_d2_plugin-1.3.1/setup.py
```

### Comparing `mkdocs-d2-plugin-1.3.0/LICENSE` & `mkdocs_d2_plugin-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-d2-plugin-1.3.0/PKG-INFO` & `mkdocs_d2_plugin-1.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-d2-plugin
-Version: 1.3.0
+Version: 1.3.1
 Summary: MkDocs plugin for D2
 Home-page: https://github.com/landmaj/mkdocs-d2-plugin
 Author: Michał Wieluński
 Author-email: michal@wielunski.net
 License: MIT
 Keywords: mkdocs python markdown d2 diagram
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-d2-plugin-1.3.0/README.md` & `mkdocs_d2_plugin-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-d2-plugin-1.3.0/d2/config.py` & `mkdocs_d2_plugin-1.3.1/d2/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs-d2-plugin-1.3.0/d2/fence.py` & `mkdocs_d2_plugin-1.3.1/d2/fence.py`

 * *Files identical despite different names*

### Comparing `mkdocs-d2-plugin-1.3.0/d2/img.py` & `mkdocs_d2_plugin-1.3.1/d2/img.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     def run(self, root: etree.Element) -> etree.Element | None:
         for elem in root.iter("img"):
             src = Path(elem.get("src", ""))
             if src.suffix == ".d2":
                 diagram = Path(self.base_dir, src).resolve()
                 if not diagram.exists():
-                    error(f"File not found: {diagram}")
+                    warning(f"File not found: {diagram}")
                     continue
                 with diagram.open("rb") as f:
                     source = f.read()
 
                 if source.strip() == b"":
                     warning(f"{src}: empty diagram file")
                     continue
```

### Comparing `mkdocs-d2-plugin-1.3.0/d2/plugin.py` & `mkdocs_d2_plugin-1.3.1/d2/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-d2-plugin-1.3.0/mkdocs_d2_plugin.egg-info/PKG-INFO` & `mkdocs_d2_plugin-1.3.1/mkdocs_d2_plugin.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-d2-plugin
-Version: 1.3.0
+Version: 1.3.1
 Summary: MkDocs plugin for D2
 Home-page: https://github.com/landmaj/mkdocs-d2-plugin
 Author: Michał Wieluński
 Author-email: michal@wielunski.net
 License: MIT
 Keywords: mkdocs python markdown d2 diagram
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-d2-plugin-1.3.0/setup.py` & `mkdocs_d2_plugin-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 PROJ_DIR = Path(__file__).resolve().parent
 with open(PROJ_DIR / "README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mkdocs-d2-plugin",
-    version="1.3.0",
+    version="1.3.1",
     description="MkDocs plugin for D2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs python markdown d2 diagram",
     url="https://github.com/landmaj/mkdocs-d2-plugin",
     author="Michał Wieluński",
     author_email="michal@wielunski.net",
```

