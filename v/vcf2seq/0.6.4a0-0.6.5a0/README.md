# Comparing `tmp/vcf2seq-0.6.4a0.tar.gz` & `tmp/vcf2seq-0.6.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcf2seq-0.6.4a0.tar", last modified: Tue May  7 12:38:27 2024, max compression
+gzip compressed data, was "vcf2seq-0.6.5a0.tar", last modified: Tue May  7 14:14:49 2024, max compression
```

## Comparing `vcf2seq-0.6.4a0.tar` & `vcf2seq-0.6.5a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-07 12:38:26.996664 vcf2seq-0.6.4a0/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.6.4a0/LICENCE.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.6.4a0/MANIFEST.in
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2331 2024-05-07 12:38:26.996664 vcf2seq-0.6.4a0/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     1708 2024-05-06 09:01:58.000000 vcf2seq-0.6.4a0/README.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-05-07 12:38:26.996664 vcf2seq-0.6.4a0/setup.cfg
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.6.4a0/setup.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-07 12:38:26.996664 vcf2seq-0.6.4a0/vcf2seq/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      165 2024-05-06 08:56:10.000000 vcf2seq-0.6.4a0/vcf2seq/__init__.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.6.4a0/vcf2seq/ascii.py
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      246 2024-05-07 12:25:21.000000 vcf2seq-0.6.4a0/vcf2seq/info.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    14026 2024-05-07 11:59:54.000000 vcf2seq-0.6.4a0/vcf2seq/vcf2seq.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-07 12:38:26.996664 vcf2seq-0.6.4a0/vcf2seq.egg-info/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2331 2024-05-07 12:38:26.000000 vcf2seq-0.6.4a0/vcf2seq.egg-info/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-05-07 12:38:26.000000 vcf2seq-0.6.4a0/vcf2seq.egg-info/SOURCES.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-05-07 12:38:26.000000 vcf2seq-0.6.4a0/vcf2seq.egg-info/dependency_links.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-05-07 12:38:26.000000 vcf2seq-0.6.4a0/vcf2seq.egg-info/entry_points.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-07 12:38:26.000000 vcf2seq-0.6.4a0/vcf2seq.egg-info/requires.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-07 12:38:26.000000 vcf2seq-0.6.4a0/vcf2seq.egg-info/top_level.txt
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-07 14:14:49.499539 vcf2seq-0.6.5a0/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.6.5a0/LICENCE.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.6.5a0/MANIFEST.in
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2331 2024-05-07 14:14:49.499539 vcf2seq-0.6.5a0/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     1708 2024-05-06 09:01:58.000000 vcf2seq-0.6.5a0/README.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-05-07 14:14:49.499539 vcf2seq-0.6.5a0/setup.cfg
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.6.5a0/setup.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-07 14:14:49.499539 vcf2seq-0.6.5a0/vcf2seq/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      165 2024-05-06 08:56:10.000000 vcf2seq-0.6.5a0/vcf2seq/__init__.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.6.5a0/vcf2seq/ascii.py
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      246 2024-05-07 14:13:54.000000 vcf2seq-0.6.5a0/vcf2seq/info.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    14023 2024-05-07 14:12:48.000000 vcf2seq-0.6.5a0/vcf2seq/vcf2seq.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-07 14:14:49.499539 vcf2seq-0.6.5a0/vcf2seq.egg-info/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2331 2024-05-07 14:14:49.000000 vcf2seq-0.6.5a0/vcf2seq.egg-info/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-05-07 14:14:49.000000 vcf2seq-0.6.5a0/vcf2seq.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-05-07 14:14:49.000000 vcf2seq-0.6.5a0/vcf2seq.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-05-07 14:14:49.000000 vcf2seq-0.6.5a0/vcf2seq.egg-info/entry_points.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-07 14:14:49.000000 vcf2seq-0.6.5a0/vcf2seq.egg-info/requires.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-07 14:14:49.000000 vcf2seq-0.6.5a0/vcf2seq.egg-info/top_level.txt
```

### Comparing `vcf2seq-0.6.4a0/LICENCE.md` & `vcf2seq-0.6.5a0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.4a0/PKG-INFO` & `vcf2seq-0.6.5a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.6.4a0
+Version: 0.6.5a0
 Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@free.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `vcf2seq-0.6.4a0/README.md` & `vcf2seq-0.6.5a0/README.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.4a0/setup.py` & `vcf2seq-0.6.5a0/setup.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.4a0/vcf2seq/ascii.py` & `vcf2seq-0.6.5a0/vcf2seq/ascii.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.4a0/vcf2seq/vcf2seq.py` & `vcf2seq-0.6.5a0/vcf2seq/vcf2seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 
     if args.type == 'alt':
         res += res_alt
     elif args.type == 'ref':
         res += res_ref
     else:
         if args.output_format == 'fa':
-            for i in range(0, len(res_alt)//2, 2):
+            for i in range(0, len(res_alt), 2):
                 res += [res_ref[i], res_ref[i+1]]
                 res += [res_alt[i], res_alt[i+1]]
         else:
             for i,_ in enumerate(res_alt):
                 res.append(res_ref[i])
                 res.append(res_alt[i])
     return res, warnings
```

### Comparing `vcf2seq-0.6.4a0/vcf2seq.egg-info/PKG-INFO` & `vcf2seq-0.6.5a0/vcf2seq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.6.4a0
+Version: 0.6.5a0
 Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@free.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

