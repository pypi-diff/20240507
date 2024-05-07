# Comparing `tmp/reaxfit-0.2.3.tar.gz` & `tmp/reaxfit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaxfit-0.2.3.tar", last modified: Fri Dec  8 10:34:52 2023, max compression
+gzip compressed data, was "reaxfit-0.3.0.tar", last modified: Tue May  7 03:06:07 2024, max compression
```

## Comparing `reaxfit-0.2.3.tar` & `reaxfit-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.104347 reaxfit-0.2.3/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.092347 reaxfit-0.2.3/.github/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       48 2023-03-03 06:38:54.000000 reaxfit-0.2.3/.github/release.yml
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.092347 reaxfit-0.2.3/.github/workflows/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      251 2023-03-03 06:38:54.000000 reaxfit-0.2.3/.github/workflows/tagpr.yml
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      111 2023-04-12 04:40:21.000000 reaxfit-0.2.3/.gitignore
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     1794 2023-03-03 06:38:54.000000 reaxfit-0.2.3/.tagpr
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     1067 2023-03-01 01:38:22.000000 reaxfit-0.2.3/LICENSE
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-12-08 10:34:52.104347 reaxfit-0.2.3/PKG-INFO
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      732 2023-06-09 06:14:50.000000 reaxfit-0.2.3/README.md
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.096347 reaxfit-0.2.3/example/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.100347 reaxfit-0.2.3/example/CoCO/
--rw-r--r--   0 ykane     (1000) ykane     (1000)     1892 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/0.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2151 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/1.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/2.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/3.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/4.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/5.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/6.xyz
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      189 2023-02-28 13:43:09.000000 reaxfit-0.2.3/example/CoCO/batch.sh
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      374 2023-02-28 13:52:46.000000 reaxfit-0.2.3/example/CoCO/chk.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      260 2023-03-03 02:56:27.000000 reaxfit-0.2.3/example/CoCO/config.json
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2310 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/data0
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    22606 2023-06-09 06:14:50.000000 reaxfit-0.2.3/example/CoCO/ffield.reax
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    22677 2023-03-02 14:08:20.000000 reaxfit-0.2.3/example/CoCO/ffield.temp
--rw-r--r--   0 ykane     (1000) ykane     (1000)       58 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/refE
--rw-r--r--   0 ykane     (1000) ykane     (1000)       56 2023-02-22 04:48:36.000000 reaxfit-0.2.3/example/CoCO/refF
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      127 2023-02-28 13:40:22.000000 reaxfit-0.2.3/example/CoCO/run.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      235 2023-03-01 02:14:34.000000 reaxfit-0.2.3/example/README.md
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    61858 2023-06-09 06:14:50.000000 reaxfit-0.2.3/reaxfit_sample.ipynb
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       38 2023-12-08 10:34:52.104347 reaxfit-0.2.3/setup.cfg
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      723 2023-06-09 06:14:50.000000 reaxfit-0.2.3/setup.py
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.092347 reaxfit-0.2.3/src/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.100347 reaxfit-0.2.3/src/reaxfit/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       30 2023-02-22 05:23:36.000000 reaxfit-0.2.3/src/reaxfit/__init__.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     2185 2023-06-20 03:09:07.000000 reaxfit-0.2.3/src/reaxfit/__main__.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      160 2023-03-03 07:37:02.000000 reaxfit-0.2.3/src/reaxfit/_version.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    10391 2023-12-08 09:01:38.000000 reaxfit-0.2.3/src/reaxfit/reaxfit.py
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-12-08 10:34:52.104347 reaxfit-0.2.3/src/reaxfit.egg-info/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-12-08 10:34:51.000000 reaxfit-0.2.3/src/reaxfit.egg-info/PKG-INFO
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      691 2023-12-08 10:34:52.000000 reaxfit-0.2.3/src/reaxfit.egg-info/SOURCES.txt
--rw-rw-r--   0 ykane     (1000) ykane     (1000)        1 2023-12-08 10:34:51.000000 reaxfit-0.2.3/src/reaxfit.egg-info/dependency_links.txt
--rw-rw-r--   0 ykane     (1000) ykane     (1000)        8 2023-12-08 10:34:51.000000 reaxfit-0.2.3/src/reaxfit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:06:07.083556 reaxfit-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:06:07.079556 reaxfit-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 03:05:56.000000 reaxfit-0.3.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:06:07.079556 reaxfit-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-07 03:05:56.000000 reaxfit-0.3.0/.github/workflows/pyrelease.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-07 03:05:56.000000 reaxfit-0.3.0/.github/workflows/tagpr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-07 03:05:56.000000 reaxfit-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-07 03:05:56.000000 reaxfit-0.3.0/.tagpr
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 03:05:56.000000 reaxfit-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-07 03:06:07.083556 reaxfit-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-07 03:05:56.000000 reaxfit-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:06:07.079556 reaxfit-0.3.0/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:06:07.083556 reaxfit-0.3.0/example/CoCO/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/0.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/1.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/2.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/3.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/4.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/5.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/6.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/batch.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/chk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/data0
+-rw-r--r--   0 runner    (1001) docker     (127)    22606 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/ffield.reax
+-rw-r--r--   0 runner    (1001) docker     (127)    22677 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/ffield.temp
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/refE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/refF
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/CoCO/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-07 03:05:56.000000 reaxfit-0.3.0/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 03:05:56.000000 reaxfit-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    61858 2024-05-07 03:05:56.000000 reaxfit-0.3.0/reaxfit_sample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:06:07.083556 reaxfit-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 03:05:56.000000 reaxfit-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:06:07.075556 reaxfit-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:06:07.083556 reaxfit-0.3.0/src/reaxfit/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 03:05:56.000000 reaxfit-0.3.0/src/reaxfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-07 03:05:56.000000 reaxfit-0.3.0/src/reaxfit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 03:06:07.000000 reaxfit-0.3.0/src/reaxfit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-05-07 03:05:56.000000 reaxfit-0.3.0/src/reaxfit/reaxfit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:06:07.083556 reaxfit-0.3.0/src/reaxfit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-07 03:06:07.000000 reaxfit-0.3.0/src/reaxfit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-07 03:06:07.000000 reaxfit-0.3.0/src/reaxfit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 03:06:07.000000 reaxfit-0.3.0/src/reaxfit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 03:06:07.000000 reaxfit-0.3.0/src/reaxfit.egg-info/top_level.txt
```

### Comparing `reaxfit-0.2.3/.tagpr` & `reaxfit-0.3.0/.tagpr`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/LICENSE` & `reaxfit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/PKG-INFO` & `reaxfit-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxfit
-Version: 0.2.3
+Version: 0.3.0
 Summary: parameter fitting for ReaxFF
 Home-page: https://github.com/ykanematsu/reaxfit
 Author: ykanematsu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `reaxfit-0.2.3/README.md` & `reaxfit-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/example/CoCO/0.xyz` & `reaxfit-0.3.0/example/CoCO/0.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/example/CoCO/1.xyz` & `reaxfit-0.3.0/example/CoCO/1.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/example/CoCO/2.xyz` & `reaxfit-0.3.0/example/CoCO/2.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/example/CoCO/3.xyz` & `reaxfit-0.3.0/example/CoCO/3.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/example/CoCO/4.xyz` & `reaxfit-0.3.0/example/CoCO/4.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/example/CoCO/5.xyz` & `reaxfit-0.3.0/example/CoCO/5.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/example/CoCO/6.xyz` & `reaxfit-0.3.0/example/CoCO/6.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/example/CoCO/data0` & `reaxfit-0.3.0/example/CoCO/data0`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/example/CoCO/ffield.reax` & `reaxfit-0.3.0/example/CoCO/ffield.reax`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/example/CoCO/ffield.temp` & `reaxfit-0.3.0/example/CoCO/ffield.temp`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/reaxfit_sample.ipynb` & `reaxfit-0.3.0/reaxfit_sample.ipynb`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/setup.py` & `reaxfit-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.3/src/reaxfit/__main__.py` & `reaxfit-0.3.0/src/reaxfit/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json,os,sys,re
 import numpy as np
 from ._version import __version__
 from .reaxfit import reaxfit, default_option
 from argparse import ArgumentParser
 
 if len(sys.argv) <2:
-    print("useage: python3 -m reaxfit [init|fit|check]")
+    print("useage: python3 -m reaxfit [init|fit|check|version]")
     sys.exit()
 parser = ArgumentParser()
 parser.add_argument('runtype')
 parser.add_argument('others', nargs='*')
 for k,v in default_option.items():
     parser.add_argument('--'+k ,type=type(v))
 args=parser.parse_args()
@@ -20,17 +20,17 @@
 if args.runtype == "fit":
     reax=reaxfit()
     if newopts: reax.config(**newopts)
     result=reax.fit()
     print("parameters after fitting")
     print(*[f'{p:.5f}' for p in result.x])
     print("fitted energy and force")
-    print(*[f'{s:.5f}' for s in reax.E-reax.E[reax.baseIdx]])
+    print(*[f'{s:.5f}' for s in reax.E-reax.E[reax.base_indices]])
     fns=reax.F
-    if reax.relative_force: fns-=fns[reax.baseIdx]
+    if reax.relative_force: fns-=fns[reax.base_indices]
     print(*[f'{f:.3f}' for f in fns])
 elif args.runtype == "init":
     cfile="config.json"
     if os.path.isfile(cfile): os.replace(cfile,cfile+".bk")
     with open(cfile,"w") as f:
         print("create config.json")
         json.dump(default_option,f,indent=1)
@@ -40,19 +40,29 @@
     if len(args.others) > 0: target_file = args.others[0]
     if not os.path.isfile(target_file):
         print(f"{target_file} not found")
         sys.exit(1)
     reax=reaxfit()
     reax.config(initfile=target_file,**newopts)
     pes,fns=reax.reax()
-    print(f"absolute energy and force norm for {target_file} at base points (kcal/mol)")
-    print(*[f'E: {s:.5f}' for s in pes[np.unique(reax.baseIdx)]])
-    print(*[f'F: {s:.3f}' for s in fns[np.unique(reax.baseIdx)]])
-    print(f"relative energy and force for {target_file} without optimization (kcal/mol)")
-    print(*[f'{s:.5f}' for s in pes-pes[reax.baseIdx]])
-    if reax.relative_force: fns-=fns[reax.baseIdx]
-    print(*[f'{f:.3f}' for f in fns])
-    print(f"reference energy and force (kcal/mol)")
-    print(*[f'{s:.5f}' for s in reax.refE])
-    print(*[f'{s:.3f}' for s in reax.refF])
+    print(f"reaxff absolute energy and force norm for {target_file}  (kcal/mol)")
+    print('E:',*[f'{s:.5f}' for s in pes])
+    print('F:',*[f'{s:.3f}' for s in fns])
+    print(f"reaxff relative energy and force norm for {target_file}  (kcal/mol)")
+    print('E:',*[f'{s:8.3f}' for s in pes-pes[reax.base_indices]])
+    if reax.relative_force: fns-=fns[reax.base_indices]
+    print('F:',*[f'{s:8.3f}' for s in fns])
+    print(f"reference relative energy and force norm")
+    print('E:',*[f'{s:8.3f}' for s in reax.refE_relative])
+    print('F:',*[f'{s:8.3f}' for s in reax.refF_relative])
+elif args.runtype == "version":
+    if __version__ == '0.0.1':
+        from subprocess import check_output
+        dir_path=os.path.dirname(__file__)
+        try:
+            __version__=check_output(['git', 'describe', '--tags'],cwd=dir_path)
+            __version__=__version__.decode('ascii').strip()
+        except:
+            pass
+    print(__version__)
 else:
     print(f"unknown runtype: {args.runtype}")
```

### Comparing `reaxfit-0.2.3/src/reaxfit/reaxfit.py` & `reaxfit-0.3.0/src/reaxfit/reaxfit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from lammps import lammps
 import json,os,sys,re
 import numpy as np
 from scipy.optimize import differential_evolution, minimize
 
 # global parameters are required for multiprocessing
 def wrap_eval(): pass
-def dump_best(): pass
+
 default_option={
             "refE_file":"refE", # reference energy file
             "refF_file":"refF", # reference force norm file
             "ref_eV":True, # units for reference energy is in eV
             "relative_force":True, # force norms are relative as refE
             "force_weight":1e-6, # penalty weight for force norms
             "harmonic":0, # harmonic constraint on initial parameters
@@ -20,17 +20,18 @@
             "bound":0.1, # define range of parameters with "{"
             "bound2":0.1, # define range of parameters  with "["
             "stopfile":"STOP", # file for early stopping
             "seed":None, # seed for random number
             "tol":0.01, # tolerance for convergence
             "workers":4, # number of cpus
             "maxiter":1000, # maximum number of iteration
+            "popsize":16, # popsize for differential_evolution
             "optimizer":"differential_evolution", # maximum number of iteration
             "scrdir":"scr", # scratch directory
-            "uniform":"False"
+            "uniform":False
 }
 
 class reaxfit():
   def __init__(self,cfile="config.json"):
     self.cfile=cfile
     self.option=default_option
     return
@@ -99,15 +100,14 @@
         l = f.readlines()
     del l[gyou]
     l.insert(gyou,f"{result}\n")
     with open(file_name,mode="w")as f:
         f.writelines(l)
 
   def config(self,**kwargs):
-    global dump_best
     if hasattr(kwargs,"cfile"): self.cfile=kwargs["cfile"]
     opt=self.option
     isconfig=os.path.isfile(self.cfile)
     if isconfig:
         print(f"read {self.cfile}")
         with open(self.cfile) as f:
             jwargs=json.load(f)
@@ -118,113 +118,117 @@
     # overwrite options if given
     if kwargs:
         optk=opt.keys()&kwargs.keys()
         opt.update(**{k:kwargs[k] for k in optk})
         if(optk != kwargs.keys()): 
             print("unrecognized options: ",*(kwargs.keys()-optk))
     self.option=opt
-    midfile=opt["midfile"]
-    stopfile=opt["stopfile"]
+    #midfile=opt["midfile"]
+    #stopfile=opt["stopfile"]
     for k in opt:
         setattr(self,k,opt[k])
     # create scratch directory
     os.makedirs(self.scrdir,exist_ok=True)
-    # conver eV to kcal/mol if refE is in eV
+    # convert eV to kcal/mol if refE is in eV
     _coeff = 1.0/0.043364124 if self.ref_eV else 1.0
+    # define the base points for relative energy
     if os.path.isfile(self.refE_file):
       with open(self.refE_file) as f:
         refE=f.read().split()
         _idx=[ i for i,v in enumerate(refE) if "*" in v ]+[len(refE)]
-        if _idx[0] != 0: _idx = [0] + _idx # initial snapshot must be reference
-        self.baseIdx=np.hstack([[_idx[i]]*(_idx[i+1]-_idx[i]) for i in range(len(_idx)-1)])
+        if _idx[0] != 0: _idx = [0] + _idx # initial snapshot must be base
+        _diff=[(i,j-i) for i,j in zip(_idx[:-1],_idx[1:])]
+        self.base_indices=np.hstack([[i]*d for i,d in _diff])
+        _idx2=[ i for i,v in enumerate(refE) if "**" in v ]
+        # set diff mode
+        if _idx2:
+          self.base_indices+=[j*(i in _idx2) for i,d in _diff for j in np.roll(range(d),1)]
         refE=[en.replace("*","") for en in refE]
     else:
-      self.baseIdx=np.array([0])
+      self.base_indices=np.array([0])
       refE=[0.0]
     if os.path.isfile(self.refF_file):
       with open(self.refF_file) as f:
         refF=f.read().split()
     else:
       refF=[0.0]
-    refE=np.array(refE,dtype=float)*_coeff # relative energy
-    refE-=refE[self.baseIdx]
-    refF=np.array(refF,dtype=float)*_coeff
-    if self.relative_force: refF-=refF[self.baseIdx]
+    self.refE=np.array(refE,dtype=float)*_coeff # raw energy
+    self.refF=np.array(refF,dtype=float)*_coeff # raw force norm
+    self.refE_relative = self.refE - self.refE[self.base_indices]
+    self.refF_relative = self.refF.copy()
+    if self.relative_force: self.refF_relative-=self.refF[self.base_indices]
     # read template and x0
     with open(self.initfile) as f:
       _template=f.read()
+    # with open("0.xyz") as f:
+    #   _xyz=f.read()
     regex=re.compile("[\{\[][\d.-]+")
     x0=regex.findall(_template)
-    isBound1=[]
-    x1 = 0
-    for x1 in range(len(x0)):
-        if x0[x1].startswith("{"):
-            isBound1.append("True")
-            x0[x1]=x0[x1].strip("{")
-        else:
-            isBound1.append("False")
-            x0[x1]=x0[x1].strip("[")
-        x1+=1
+    isBound1=[x.startswith("{") for x in x0]
     #print(x0)
-    self.x0=[float(x) for x in x0]
+    self.x0=[float(x.strip("{").strip("[")) for x in x0]
     #print(x1)
     self.template = _template
     # change {S
     # define bounds
-    for x in self.x0:
-        if x==0:
-            print("error:0 cannot be used as a parameter.")
-            sys.exit(1)
-        else:
-            pass
+    if 0 in self.x0:
+      sys.exit("error:0 cannot be used as a ffield parameter.")
     bounds=[]
     for i,x in enumerate(self.x0):
-        if isBound1[i] =="True":
+        if isBound1[i]:
             delta = abs(float(self.bound)*x)
             t = (x-delta,x+delta)
             bounds.append(t)
         else:
             sigma = abs(float(self.bound2)*x)
             k=(x-sigma,x+sigma)
             bounds.append(k)
     #print(bounds)
     self.bounds=bounds
     template=regex.sub("{}",_template)
     self.template=template
     # get elements from templates
-    eles=re.findall(r"\n *(:?[A-Z][a-z]?)",template)
+    eles=re.findall(r"\n *(:?[A-Z][a-z]?) ",template)
+    #idxs=sorted(set(re.findall("\n *\d+ +(\d+) +",_xyz)))
+    #eles=re.findall(r"\n *(:?[A-Z][a-z]?)",_xyz)
+    #eles=sorted(set(eles),key=eles.index)
+    #idxs=[int(i) for i in idxs]
+    #eles=[eles[i-1] for i in idxs]
     self.elements=" ".join(eles)
-    self.refE=refE
-    self.refF=refF
-    def callbackF(xk,convergence=False,fout=None):
-      fname=midfile
-      sys.stdout.flush()
-      if fout: fname=fout
-      with open(fname,"w") as f:
-          _x=np.round(xk,5)
-          y=[f"{{{xx}" for xx in _x]
-          f.write(template.format(*y))
-      if os.path.isfile(stopfile):
-          print("optimization will be stopped by the stop file")
-          os.remove(stopfile)
-          return True
-    dump_best=callbackF
+    #dump_best=self.callbackF
     return
+
+  def callbackF(self,xk,convergence=False,fout=None):
+    fname=self.option["midfile"]
+    stopfile=self.option["stopfile"]
+    sys.stdout.flush()
+    if fout: fname=fout
+    with open(fname,"w") as f:
+        _x=np.round(xk,5)
+        y=[f"{{{xx}" for xx in _x]
+        f.write(self.template.format(*y))
+    if os.path.isfile(stopfile):
+        print("optimization will be stopped by the stop file")
+        os.remove(stopfile)
+        return True
+
   def set_eval(self,func):
     global wrap_eval
+    if not hasattr(self,"x0"): self.config()
     _x0=np.array(self.x0)
     def wrap_eval(*args,**kwargs):
       pid=os.getpid()
       pes,fns=self.reax(*args,pid=pid)
       output = func(pes,fns,self.refE,self.refF) 
       if self.harmonic > 0:
         deltax=(np.array(args[0])-_x0)/(_x0+0.01)
         output+=deltax@deltax*self.harmonic
       return output
     return wrap_eval
+
   def reax(self,xk=None,pid=0):
       x=xk if xk is not None else self.x0
       ffname=f"{self.scrdir}/ffield.reax.{pid}"
       elements=self.elements
       pes,fns=[],[]
       with open(ffname,"w") as f:
           f.write(self.template.format(*np.round(x,6)))
@@ -233,61 +237,63 @@
           cmds=["units real",
               "atom_style charge",
               f"read_data {self.datafile}",
               "pair_style      reaxff NULL",
               f"pair_coeff      * * {ffname} {elements}",
               "fix             1 all qeq/reaxff 1 0.0 10.0 1.0e-6 reaxff"]
           lmp.commands_list(cmds)
-          lmp.command("run 0")
+          lmp.command("run 0 post no")
           pes.append(lmp.get_thermo("pe"))
           fns.append(lmp.get_thermo("fnorm"))
-      if self.uniform == "False":
+      if self.uniform == "False" or not self.uniform:
         b="add yes purge yes replace no "
       else:
         b=""
       for i in range(1,len(self.refE)):
         a=f"read_dump {i}.xyz 0 x y z box no "
         c="format xyz"
         lmp.command(a+b+c)
-        lmp.command("run 0")
+        lmp.command("run 0 post no")
         pes.append(lmp.get_thermo("pe"))
         fns.append(lmp.get_thermo("fnorm"))
       lmp.close()
       pes=np.array(pes)
       fns=np.array(fns)
       return pes,fns
 
-  def fit(self,func=None):
-      global dump_best
+  def default_func(self,*args,**kwargs):
+    _x0=np.array(self.x0)
+    pid=os.getpid()
+    pes,fns=self.reax(*args,pid=pid)
+    pes-=pes[self.base_indices] # initial structure is base by default
+    pes-=self.refE_relative
+    if self.relative_force: fns-=fns[self.base_indices]
+    fns-=self.refF_relative
+    fns*=self.force_weight
+    fmax=np.abs(fns).max()
+    output = pes@pes + np.linalg.norm(fns)+np.abs(pes).max()*np.abs(fns).max()+fmax**2
+    if self.harmonic > 0:
+      deltax=(np.array(args[0])-_x0)/(np.abs(_x0)+0.01)
+      output+=deltax@deltax*self.harmonic
+    return output
+
+  def fit(self,myfunc=None):
+      #global dump_best
       if not hasattr(self,"x0"): self.config()
       print("config parameters for fitting")
       json.dump(self.option,sys.stdout)
       print("")
-      #refE,refF=self.refE,self.refF
       print(f"initial {len(self.x0)} parameters : {self.x0}")
-      if not func:
-          @self.set_eval
-          def default_eval(pes,fns,refE,refF):
-            pes0=pes[0]
-            pes-=pes[self.baseIdx] # initial structure is reference by default
-            pes-=refE
-            if self.relative_force: fns-=fns[self.baseIdx]
-            fns-=refF
-            fns*=self.force_weight
-            fmax=np.abs(fns).max()
-            #return np.sign(pes0)*np.log10(np.abs(pes0)+1) + np.log10(fns@fns+1)
-            return pes@pes + np.linalg.norm(fns)+np.abs(pes).max()*np.abs(fns).max()+fmax**2
-            #return pes@pes + np.linalg.norm(fns)/len(fns)/10+fns[0]*fns[0]/10
-          func=default_eval
+      func = myfunc if myfunc else self.default_func
       if self.optimizer == "differential_evolution":
         result = differential_evolution(func, self.bounds,workers=self.workers,x0=self.x0,updating='deferred',
-                                  disp=True,maxiter=self.maxiter,tol=self.tol,callback=dump_best,popsize=16,seed=self.seed)
+                                  disp=True,maxiter=self.maxiter,tol=self.tol,callback=self.callbackF,popsize=self.popsize,seed=self.seed)
       else:
-        result = minimize(func,x0=self.x0,method=self.optimizer,tol=self.tol,callback=dump_best,jac='3-point') 
+        result = minimize(func,x0=self.x0,method=self.optimizer,tol=self.tol,callback=self.callbackF,jac='3-point') 
       print(result)
-      dump_best(result.x,fout=self.endfile)
+      self.callbackF(result.x,fout=self.endfile)
       self.result=result
       self.E,self.F=self.reax(result.x)
       return result
 
 if __name__ =='__main__':
-    pass
+  pass
```

### Comparing `reaxfit-0.2.3/src/reaxfit.egg-info/PKG-INFO` & `reaxfit-0.3.0/src/reaxfit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxfit
-Version: 0.2.3
+Version: 0.3.0
 Summary: parameter fitting for ReaxFF
 Home-page: https://github.com/ykanematsu/reaxfit
 Author: ykanematsu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `reaxfit-0.2.3/src/reaxfit.egg-info/SOURCES.txt` & `reaxfit-0.3.0/src/reaxfit.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .gitignore
 .tagpr
 LICENSE
 README.md
+pyproject.toml
 reaxfit_sample.ipynb
 setup.py
 .github/release.yml
+.github/workflows/pyrelease.yml
 .github/workflows/tagpr.yml
 example/README.md
 example/CoCO/0.xyz
 example/CoCO/1.xyz
 example/CoCO/2.xyz
 example/CoCO/3.xyz
 example/CoCO/4.xyz
```

