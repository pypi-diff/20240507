# Comparing `tmp/weld_deps-0.6.4.tar.gz` & `tmp/weld_deps-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weld_deps-0.6.4.tar", max compression
+gzip compressed data, was "weld_deps-0.7.0.tar", max compression
```

## Comparing `weld_deps-0.6.4.tar` & `weld_deps-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0     1067 2024-05-03 08:39:34.039106 weld_deps-0.6.4/LICENSE
--rw-r--r--   0        0        0      333 2024-05-03 08:39:56.051428 weld_deps-0.6.4/pyproject.toml
--rw-r--r--   0        0        0       31 2024-05-03 08:39:34.043106 weld_deps-0.6.4/weld_deps/__init__.py
--rw-r--r--   0        0        0     5879 2024-05-03 08:39:34.043106 weld_deps-0.6.4/weld_deps/dep.py
--rw-r--r--   0        0        0      267 2024-05-03 08:39:34.043106 weld_deps-0.6.4/weld_deps/examples/pack1/beet.yaml
--rw-r--r--   0        0        0        0 2024-05-03 08:39:34.043106 weld_deps-0.6.4/weld_deps/examples/pack1/src/data/pack1/functions/test.mcfunction
--rw-r--r--   0        0        0     1858 2024-05-03 08:39:34.043106 weld_deps-0.6.4/weld_deps/main.py
--rw-r--r--   0        0        0     4903 2024-05-03 08:39:34.043106 weld_deps-0.6.4/weld_deps/utils.py
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 weld_deps-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-07 17:28:54.433695 weld_deps-0.7.0/LICENSE
+-rw-r--r--   0        0        0      333 2024-05-07 17:29:13.065493 weld_deps-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/__init__.py
+-rw-r--r--   0        0        0     6076 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/dep.py
+-rw-r--r--   0        0        0      267 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/examples/pack1/beet.yaml
+-rw-r--r--   0        0        0        0 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/examples/pack1/src/data/pack1/functions/test.mcfunction
+-rw-r--r--   0        0        0      261 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/examples/pack_no_versions/beet.yaml
+-rw-r--r--   0        0        0        0 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/examples/pack_no_versions/src/data/pack_not_found/functions/test.mcfunction
+-rw-r--r--   0        0        0      262 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/examples/pack_not_found/beet.yaml
+-rw-r--r--   0        0        0        0 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/examples/pack_not_found/src/data/pack_not_found/functions/test.mcfunction
+-rw-r--r--   0        0        0     1858 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/main.py
+-rw-r--r--   0        0        0     5124 2024-05-07 17:28:54.437695 weld_deps-0.7.0/weld_deps/utils.py
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 weld_deps-0.7.0/PKG-INFO
```

### Comparing `weld_deps-0.6.4/LICENSE` & `weld_deps-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weld_deps-0.6.4/weld_deps/dep.py` & `weld_deps-0.7.0/weld_deps/dep.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,17 +65,22 @@
             return f"https://api.smithed.dev/v2/packs/{self.id}/versions"
         elif self.source == Source.MODRINTH:
             return f"https://api.modrinth.com/v2/project/{self.id}/version"
 
     def get_versions(self) -> List["VersionedDep"]:
         if self.identifier in CACHED_VERSIONS:
             return CACHED_VERSIONS[self.identifier]
-        r = requests.get(self.versions_url)
-        r.raise_for_status()
-        versions = r.json()
+        try:
+            r = requests.get(self.versions_url)
+            r.raise_for_status()
+            versions = r.json()
+        except requests.exceptions.HTTPError as e:
+            raise ValueError(f"Failed to get versions for {self.identifier}, {e}")
+        except e:
+            raise e
 
         l_versions = []
         if self.source == Source.SMITHED:
             for v in versions:
                 l_deps = []
                 for dep in v["dependencies"]:
                     id, slug = get_id_slug(dep["id"], Source.SMITHED)
```

### Comparing `weld_deps-0.6.4/weld_deps/main.py` & `weld_deps-0.7.0/weld_deps/main.py`

 * *Files identical despite different names*

### Comparing `weld_deps-0.6.4/weld_deps/utils.py` & `weld_deps-0.7.0/weld_deps/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,16 @@
                 for v in versions 
                 if not semver.VersionInfo.parse(v.version.lstrip("v")).build
             ]
 
         # filter versions by match
         versions = [v for v in versions if all([semver.match(v.version.lstrip("v"), deps[dep][i]) for i in range(len(deps[dep]))])]
         # append newest version
+        if len(versions) == 0:
+            raise ValueError(f"Could not find a version for {dep.slug} that matches the requirements: {deps[dep]}, available versions: {', '.join([v.version for v in dep.get_versions()])}")
         new_deps[get_identifier(versions[0])] = versions[0]
         # append dependencies
         add_deps(versions[0], new_deps)
     return new_deps.values()
 
 
 def add_deps(dep: VersionedDep, deps: dict[str, VersionedDep]):
```

