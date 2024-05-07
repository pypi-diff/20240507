# Comparing `tmp/runtool-1.0.7.tar.gz` & `tmp/runtool-1.0.8.tar.gz`

## Comparing `runtool-1.0.7.tar` & `runtool-1.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0    46956 2020-02-02 00:00:00.000000 runtool-1.0.7/runtool/__init__.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 runtool-1.0.7/runtool/_additional_cli.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 runtool-1.0.7/runtool/_types.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 runtool-1.0.7/runtool/_version.py
--rw-r--r--   0        0        0    20999 2020-02-02 00:00:00.000000 runtool-1.0.7/runtool/runtool.ini
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 runtool-1.0.7/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 runtool-1.0.7/LICENSE
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 runtool-1.0.7/README.md
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 runtool-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 runtool-1.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0    47182 2020-02-02 00:00:00.000000 runtool-1.0.8/runtool/__init__.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 runtool-1.0.8/runtool/_additional_cli.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 runtool-1.0.8/runtool/_types.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 runtool-1.0.8/runtool/_version.py
+-rw-r--r--   0        0        0    21157 2020-02-02 00:00:00.000000 runtool-1.0.8/runtool/runtool.ini
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 runtool-1.0.8/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 runtool-1.0.8/LICENSE
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 runtool-1.0.8/README.md
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 runtool-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 runtool-1.0.8/PKG-INFO
```

### Comparing `runtool-1.0.7/runtool/__init__.py` & `runtool-1.0.8/runtool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,19 @@
 
                 env_name = domain_env_name(urlparse(r.url).netloc)
                 if env_name in os.environ:
                     r.headers["Authorization"] = f"token {os.environ[env_name]}"
             return r
 
     ret = requests.Session()
+    verify = os.environ.get("RUNTOOL_CA_BUNDLE", None)
+    if verify and os.path.exists(verify):
+        ret.verify = verify
+    elif "RUNTOOL_VERIFY" in os.environ:
+        ret.verify = int(os.environ["RUNTOOL_VERIFY"]) != 0
     ret.auth = MyAuth()
     return ret
 
 
 # def m_requests(url: str, headers: dict[str, str] | None = None) -> _UrlopenRet:
 #     import urllib.request
```

### Comparing `runtool-1.0.7/runtool/_additional_cli.py` & `runtool-1.0.8/runtool/_additional_cli.py`

 * *Files identical despite different names*

### Comparing `runtool-1.0.7/runtool/_types.py` & `runtool-1.0.8/runtool/_types.py`

 * *Files identical despite different names*

### Comparing `runtool-1.0.7/runtool/runtool.ini` & `runtool-1.0.8/runtool/runtool.ini`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,19 @@
 
 [docker-machine]
 class = GithubReleaseLinks
 binary = docker-machine
 description = Machine management for a container-centric world
 url = https://github.com/docker/machine
 
+[duckdb]
+class = GithubReleaseLinks
+description = DuckDB is an embeddable SQL OLAP database management system
+url = https://github.com/duckdb/duckdb
+
 [gdu]
 class = GithubReleaseLinks
 description = Fast disk usage analyzer with console interface written in Go
 url = https://github.com/dundee/gdu
 
 [watchman]
 class = GithubReleaseLinks
@@ -308,15 +313,15 @@
 description = Launch a subprocess with environment variables using data from @hashicorp Consul and Vault.
 
 [,miniconda-installer.sh]
 class = LinkScraperInstaller
 binary = ,miniconda-installer.sh
 url = https://repo.anaconda.com/miniconda/
 link_contains = Miniconda3-latest-
-description = ,run miniconda-installer.sh -b -u -p ~/miniconda3 && ~/miniconda3/bin/conda init bash
+description = runtool run ,miniconda-installer.sh -b -u -p ~/miniconda3 && ~/miniconda3/bin/conda init bash
 
 [ampy]
 class = PipxInstallSource
 package = adafruit-ampy
 command = ampy
 description = ampy (Adafruit MicroPython tool) is a command line tool to interact with a CircuitPython or MicroPython board over a serial connection.
```

### Comparing `runtool-1.0.7/.gitignore` & `runtool-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `runtool-1.0.7/LICENSE` & `runtool-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `runtool-1.0.7/README.md` & `runtool-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `runtool-1.0.7/pyproject.toml` & `runtool-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `runtool-1.0.7/PKG-INFO` & `runtool-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: runtool
-Version: 1.0.7
+Version: 1.0.8
 Summary: Install binary from github release.
 Project-URL: Documentation, https://github.com/FlavioAmurrioCS/runtool#readme
 Project-URL: Issues, https://github.com/FlavioAmurrioCS/runtool/issues
 Project-URL: Source, https://github.com/FlavioAmurrioCS/runtool
 Author-email: Flavio Amurrio <25621374+FlavioAmurrioCS@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
```

