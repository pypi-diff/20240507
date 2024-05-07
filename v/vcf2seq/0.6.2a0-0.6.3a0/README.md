# Comparing `tmp/vcf2seq-0.6.2a0.tar.gz` & `tmp/vcf2seq-0.6.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcf2seq-0.6.2a0.tar", last modified: Mon May  6 09:16:05 2024, max compression
+gzip compressed data, was "vcf2seq-0.6.3a0.tar", last modified: Mon May  6 13:02:20 2024, max compression
```

## Comparing `vcf2seq-0.6.2a0.tar` & `vcf2seq-0.6.3a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 09:16:05.541802 vcf2seq-0.6.2a0/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.6.2a0/LICENCE.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.6.2a0/MANIFEST.in
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2331 2024-05-06 09:16:05.541802 vcf2seq-0.6.2a0/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     1708 2024-05-06 09:01:58.000000 vcf2seq-0.6.2a0/README.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-05-06 09:16:05.545802 vcf2seq-0.6.2a0/setup.cfg
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.6.2a0/setup.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 09:16:05.541802 vcf2seq-0.6.2a0/vcf2seq/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      165 2024-05-06 08:56:10.000000 vcf2seq-0.6.2a0/vcf2seq/__init__.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.6.2a0/vcf2seq/ascii.py
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      246 2024-05-06 09:14:13.000000 vcf2seq-0.6.2a0/vcf2seq/info.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    12874 2024-05-06 08:36:49.000000 vcf2seq-0.6.2a0/vcf2seq/vcf2seq.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 09:16:05.541802 vcf2seq-0.6.2a0/vcf2seq.egg-info/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2331 2024-05-06 09:16:05.000000 vcf2seq-0.6.2a0/vcf2seq.egg-info/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-05-06 09:16:05.000000 vcf2seq-0.6.2a0/vcf2seq.egg-info/SOURCES.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-05-06 09:16:05.000000 vcf2seq-0.6.2a0/vcf2seq.egg-info/dependency_links.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-05-06 09:16:05.000000 vcf2seq-0.6.2a0/vcf2seq.egg-info/entry_points.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 09:16:05.000000 vcf2seq-0.6.2a0/vcf2seq.egg-info/requires.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 09:16:05.000000 vcf2seq-0.6.2a0/vcf2seq.egg-info/top_level.txt
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 13:02:20.013090 vcf2seq-0.6.3a0/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.6.3a0/LICENCE.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.6.3a0/MANIFEST.in
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2331 2024-05-06 13:02:20.013090 vcf2seq-0.6.3a0/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     1708 2024-05-06 09:01:58.000000 vcf2seq-0.6.3a0/README.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-05-06 13:02:20.013090 vcf2seq-0.6.3a0/setup.cfg
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.6.3a0/setup.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 13:02:20.013090 vcf2seq-0.6.3a0/vcf2seq/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      165 2024-05-06 08:56:10.000000 vcf2seq-0.6.3a0/vcf2seq/__init__.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.6.3a0/vcf2seq/ascii.py
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      246 2024-05-06 13:01:39.000000 vcf2seq-0.6.3a0/vcf2seq/info.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    13245 2024-05-06 12:52:37.000000 vcf2seq-0.6.3a0/vcf2seq/vcf2seq.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-06 13:02:20.013090 vcf2seq-0.6.3a0/vcf2seq.egg-info/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2331 2024-05-06 13:02:19.000000 vcf2seq-0.6.3a0/vcf2seq.egg-info/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-05-06 13:02:19.000000 vcf2seq-0.6.3a0/vcf2seq.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-05-06 13:02:19.000000 vcf2seq-0.6.3a0/vcf2seq.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-05-06 13:02:19.000000 vcf2seq-0.6.3a0/vcf2seq.egg-info/entry_points.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 13:02:19.000000 vcf2seq-0.6.3a0/vcf2seq.egg-info/requires.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-06 13:02:19.000000 vcf2seq-0.6.3a0/vcf2seq.egg-info/top_level.txt
```

### Comparing `vcf2seq-0.6.2a0/LICENCE.md` & `vcf2seq-0.6.3a0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.2a0/PKG-INFO` & `vcf2seq-0.6.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.6.2a0
+Version: 0.6.3a0
 Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@free.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `vcf2seq-0.6.2a0/README.md` & `vcf2seq-0.6.3a0/README.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.2a0/setup.py` & `vcf2seq-0.6.3a0/setup.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.2a0/vcf2seq/ascii.py` & `vcf2seq-0.6.3a0/vcf2seq/ascii.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.2a0/vcf2seq/vcf2seq.py` & `vcf2seq-0.6.3a0/vcf2seq/vcf2seq.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,16 +167,20 @@
                                 f"at line {num_row} (chr{chr}:{ps_ref2+1}).\n"
                                 f"    - REF in the vcf file: {ref!r}\n"
                                 f"    - Found in the genome: '{seq_ref2}'\n"
                                 "    Please check if the given genome is appropriate.")
             col_sep = ' ' if args.output_format == 'fa' else '\t'
             col_txt =  col_sep.join([fields[num-1] for num in cols_id])
             if len(ref_seq) == args.size == len(alt_seq):
-                res_ref.append(f"{header}_ref{col_sep}{col_txt}\n{ref_seq}")
-                res_alt.append(f"{header}_alt{col_sep}{col_txt}\n{alt_seq}")
+                if args.output_format == "tsv":
+                    res_ref.append(f"{ref_seq}{col_sep}{header}_ref{col_sep}{col_txt}".rstrip(col_sep))
+                    res_alt.append(f"{alt_seq}{col_sep}{header}_alt{col_sep}{col_txt}".rstrip(col_sep))
+                else:
+                    res_ref.append(f">{header}_ref{col_sep}{col_txt}\n{ref_seq}")
+                    res_alt.append(f">{header}_alt{col_sep}{col_txt}\n{alt_seq}")
             elif len(alt_seq) > args.size:
                 warnings.append(f"Warning: ALT length ({len(alt_seq)} bp) larger than sequence "
                                 f"({args.size} bp) at line {num_row}, ignored.")
             else:
                 warnings.append(f"Warning: sequence size not correct at line {num_row}, ignored"
                                 "f({len(alt_seq)} != {args.size}).")
 
@@ -200,21 +204,22 @@
     if not args.output:
         name, _ = os.path.splitext(os.path.basename(args.input.name))
         args.output = f"{name}-vcf2seq.{ext}"
 
     ## write results in file
     if results:
         with open(args.output, 'w') as fh:
-            if ext == 'fa':
-                fh.write(">" + '\n>'.join([a for a in results]) + "\n")
-            else:
-                for row in results:
-                    header, seq = row.split('\n')
-                    fh.write(f"{seq}\t")
-                    fh.write(f"{header}\n")
+            fh.write('\n'.join([a for a in results]) + "\n")
+            # ~ if ext == 'fa':
+                # ~ fh.write('\n>'.join([a for a in results]) + "\n")
+            # ~ else:
+                # ~ for row in results:
+                    # ~ header, seq = row.split('\n')
+                    # ~ fh.write(f"{seq}\t")
+                    # ~ fh.write(f"{header}\n")
 
     ### WARNINGS
     if warnings:
         for warning in warnings:
             color = COL.RED if warning.startswith('Error') else COL.PURPLE
             print(f"{color}{warning}\n")
         print(COL.END)
```

### Comparing `vcf2seq-0.6.2a0/vcf2seq.egg-info/PKG-INFO` & `vcf2seq-0.6.3a0/vcf2seq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.6.2a0
+Version: 0.6.3a0
 Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@free.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

