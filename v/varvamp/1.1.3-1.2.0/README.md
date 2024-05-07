# Comparing `tmp/varvamp-1.1.3.tar.gz` & `tmp/varvamp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varvamp-1.1.3.tar", last modified: Fri Apr 26 09:56:00 2024, max compression
+gzip compressed data, was "varvamp-1.2.0.tar", last modified: Tue May  7 09:53:06 2024, max compression
```

## Comparing `varvamp-1.1.3.tar` & `varvamp-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:56:00.671611 varvamp-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-26 09:56:00.671611 varvamp-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-26 09:55:49.000000 varvamp-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:56:00.671611 varvamp-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-26 09:55:49.000000 varvamp-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:56:00.667611 varvamp-1.1.3/varvamp/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:56:00.671611 varvamp-1.1.3/varvamp/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/blast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/consensus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/default_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/param_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/primers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/qpcr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21338 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-04-26 09:55:49.000000 varvamp-1.1.3/varvamp/scripts/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:56:00.671611 varvamp-1.1.3/varvamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 09:56:00.000000 varvamp-1.1.3/varvamp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:53:06.229498 varvamp-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-07 09:53:06.229498 varvamp-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-07 09:52:55.000000 varvamp-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:53:06.229498 varvamp-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-07 09:52:55.000000 varvamp-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:53:06.225498 varvamp-1.2.0/varvamp/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:53:06.229498 varvamp-1.2.0/varvamp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/scripts/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/scripts/blast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/scripts/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/scripts/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/scripts/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20318 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/scripts/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/scripts/param_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/scripts/primers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/scripts/qpcr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/scripts/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22528 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/scripts/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16198 2024-05-07 09:52:55.000000 varvamp-1.2.0/varvamp/scripts/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:53:06.229498 varvamp-1.2.0/varvamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-07 09:53:06.000000 varvamp-1.2.0/varvamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-07 09:53:06.000000 varvamp-1.2.0/varvamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:53:06.000000 varvamp-1.2.0/varvamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 09:53:06.000000 varvamp-1.2.0/varvamp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:53:06.000000 varvamp-1.2.0/varvamp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-07 09:53:06.000000 varvamp-1.2.0/varvamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 09:53:06.000000 varvamp-1.2.0/varvamp.egg-info/top_level.txt
```

### Comparing `varvamp-1.1.3/PKG-INFO` & `varvamp-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 1.1.3
+Version: 1.2.0
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `varvamp-1.1.3/README.md` & `varvamp-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.3/setup.py` & `varvamp-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.3/varvamp/command.py` & `varvamp-1.2.0/varvamp/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -310,43 +310,41 @@
         progress=0.8,
         job="Finding potential amplicons.",
         progress_text=f"{len(amplicons)} potential amplicons"
     )
 
     if args.database is not None:
         # create blast query
-        query_path = blast.create_BLAST_query(all_primers, amplicons, data_dir)
+        query_path = blast.create_BLAST_query(amplicons, data_dir)
         # perform primer blast
-        amplicons, off_target_amplicons = blast.primer_blast(
+        amplicons = blast.primer_blast(
             data_dir,
             args.database,
             query_path,
             amplicons,
             args.max_length,
             args.threads,
             log_file,
             mode="single_tiled"
         )
-    else:
-        off_target_amplicons = []
 
-    return all_primers, amplicons, off_target_amplicons
+    return all_primers, amplicons
 
 
 def single_workflow(args, amplicons, all_primers, log_file):
     """
     workflow part specific for single mode
     """
 
-    amplicon_scheme = scheme.find_single_amplicons(amplicons, all_primers, args.report_n)
+    amplicon_scheme = scheme.find_single_amplicons(amplicons, args.report_n)
     logging.varvamp_progress(
         log_file,
         progress=0.9,
         job="Finding amplicons with low penalties.",
-        progress_text=f"{len(amplicon_scheme[0])} amplicons."
+        progress_text=f"{len(amplicon_scheme)} amplicons."
     )
 
     return amplicon_scheme
 
 
 def tiled_workflow(args, amplicons, left_primer_candidates, right_primer_candidates, all_primers, ambiguous_consensus, log_file, results_dir):
     """
@@ -355,16 +353,15 @@
 
     # create graph
     amplicon_graph = scheme.create_amplicon_graph(amplicons, args.overlap)
 
     # search for amplicon scheme
     coverage, amplicon_scheme = scheme.find_best_covering_scheme(
         amplicons,
-        amplicon_graph,
-        all_primers
+        amplicon_graph
     )
 
     # check for dimers
     dimers_not_solved = scheme.check_and_solve_heterodimers(
         amplicon_scheme,
         left_primer_candidates,
         right_primer_candidates,
@@ -373,20 +370,21 @@
         logging.raise_error(
             f"varVAMP found {len(dimers_not_solved)} primer dimers without replacements. Check the dimer file and perform the PCR for incomaptible amplicons in a sperate reaction.",
             log_file
         )
         reporting.write_dimers(results_dir, dimers_not_solved)
 
     # evaluate coverage
+    # ATTENTION: Genome coverage of the scheme might still change slightly through resolution of primer dimers, but this potential, minor inaccuracy is currently accepted.
     percent_coverage = round(coverage/len(ambiguous_consensus)*100, 2)
     logging.varvamp_progress(
         log_file,
         progress=0.9,
         job="Creating amplicon scheme.",
-        progress_text=f"{percent_coverage} % total coverage with {len(amplicon_scheme[0]) + len(amplicon_scheme[1])} amplicons"
+        progress_text=f"{percent_coverage} % total coverage with {len(amplicon_scheme)} amplicons"
     )
     if percent_coverage < 70:
         logging.raise_error(
             "coverage < 70 %. Possible solutions:\n"
             "\t - lower threshold\n"
             "\t - increase amplicons lengths\n"
             "\t - increase number of ambiguous nucleotides\n"
@@ -446,17 +444,17 @@
         progress=0.8,
         job="Finding unique amplicons with probe.",
         progress_text=f"{len(qpcr_scheme_candidates)} unique amplicons with internal probe"
     )
     # run blast if db is given
     if args.database is not None:
         # create blast query
-        query_path = blast.create_BLAST_query_qpcr(qpcr_scheme_candidates, data_dir)
+        query_path = blast.create_BLAST_query(qpcr_scheme_candidates, data_dir, mode="qpcr")
         # perform primer blast
-        amplicons, off_target_amplicons = blast.primer_blast(
+        qpcr_scheme_candidates = blast.primer_blast(
             data_dir,
             args.database,
             query_path,
             qpcr_scheme_candidates,
             config.QAMPLICON_LENGTH[1],
             args.threads,
             log_file,
@@ -466,17 +464,14 @@
     final_schemes = qpcr.test_amplicon_deltaG_parallel(qpcr_scheme_candidates, majority_consensus, args.test_n, args.deltaG, args.threads)
     if not final_schemes:
         logging.raise_error(
             "no qPCR amplicon passed the deltaG threshold\n",
             log_file,
             exit=True
         )
-    # report potential blast warnings
-    if args.database is not None:
-        blast.write_BLAST_warning(off_target_amplicons, final_schemes, log_file)
     logging.varvamp_progress(
         log_file,
         progress=0.9,
         job="Filtering amplicons for deltaG.",
         progress_text=f"{len(final_schemes)} non-overlapping qPCR schemes that passed deltaG cutoff"
     )
     return probe_regions, final_schemes
@@ -502,17 +497,29 @@
 
     # write files that are shared in all modes
     reporting.write_regions_to_bed(primer_regions, data_dir)
     reporting.write_alignment(data_dir, alignment_cleaned)
     reporting.write_fasta(data_dir, "majority_consensus", majority_consensus)
     reporting.write_fasta(results_dir, "ambiguous_consensus", ambiguous_consensus)
 
+    # Functions called from here on return lists of amplicons that are refined step-wise into final schemes.
+    # These lists that are passed between functions and later used for reporting consist of dictionary elemnts,
+    # which represent individual amplicons. A minimal amplicon dict could take the form:
+    # {
+    #     "id": amplicon_name,
+    #     "penalty": amplicon_cost,
+    #     "length": amplicon_length,
+    #     "LEFT": [left primer data],
+    #     "RIGHT": [right primer data]
+    # }
+    # to which different functions may add additional information.
+
     # SINGLE/TILED mode
     if args.mode == "tiled" or args.mode == "single":
-        all_primers, amplicons, off_target_amplicons = single_and_tiled_shared_workflow(
+        all_primers, amplicons = single_and_tiled_shared_workflow(
             args,
             left_primer_candidates,
             right_primer_candidates,
             data_dir,
             log_file
         )
         if args.mode == "single":
@@ -529,23 +536,30 @@
                 left_primer_candidates,
                 right_primer_candidates,
                 all_primers,
                 ambiguous_consensus,
                 log_file,
                 results_dir
             )
-        if args.database is not None:
-            blast.write_BLAST_warning(off_target_amplicons, amplicon_scheme, log_file)
+
         # write files
+
+        if args.mode == "tiled":
+            # assign amplicon numbers from 5' to 3' along the genome
+            amplicon_scheme.sort(key=lambda x: x["LEFT"][1])
+        else:
+            # make sure amplicons with no off-target products and with low penalties get the lowest numbers
+            amplicon_scheme.sort(key=lambda x: (x.get("off_targets", False), x["penalty"]))
         reporting.write_all_primers(data_dir, all_primers)
         reporting.write_scheme_to_files(
             results_dir,
             amplicon_scheme,
             ambiguous_consensus,
-            args.mode
+            args.mode,
+            log_file
         )
         reporting.varvamp_plot(
             results_dir,
             alignment_cleaned,
             primer_regions,
             all_primers=all_primers,
             amplicon_scheme=amplicon_scheme,
@@ -560,17 +574,21 @@
             alignment_cleaned,
             ambiguous_consensus,
             majority_consensus,
             left_primer_candidates,
             right_primer_candidates,
             log_file
         )
+
         # write files
+
+        # make sure amplicons with no off-target products and with low penalties get the lowest numbers
+        final_schemes.sort(key=lambda x: (x.get("off_targets", False), x["penalty"]))
         reporting.write_regions_to_bed(probe_regions, data_dir, "probe")
-        reporting.write_qpcr_to_files(results_dir, final_schemes, ambiguous_consensus)
+        reporting.write_qpcr_to_files(results_dir, final_schemes, ambiguous_consensus, log_file)
         reporting.varvamp_plot(
             results_dir,
             alignment_cleaned,
             primer_regions,
             probe_regions=probe_regions,
             amplicon_scheme=final_schemes
         )
```

### Comparing `varvamp-1.1.3/varvamp/scripts/alignment.py` & `varvamp-1.2.0/varvamp/scripts/alignment.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.3/varvamp/scripts/blast.py` & `varvamp-1.2.0/varvamp/scripts/blast.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,49 +25,32 @@
     """
     if which("blastn") is not None:
         print("\nINFO: BLASTN is installed.")
     else:
         logging.raise_error("BLASTN is not installed", log_file, exit=True)
 
 
-def create_BLAST_query(all_primers, amplicons, data_dir):
+def create_BLAST_query(amplicons, data_dir, mode="single_tiled"):
     """
-    create a query for the BLAST search (tiled, single mode)
+    create a query for the BLAST search
     """
-    already_written = []
-
     query_path = os.path.join(data_dir, "BLAST_query.fasta")
-    with open(query_path, "w") as query:
-        for amp in amplicons:
-            fw_primer, rv_primer = amplicons[amp][2], amplicons[amp][3]
-            if fw_primer not in already_written:
-                print(f">{fw_primer}\n{all_primers['+'][fw_primer][0]}", file=query)
-                already_written.append(fw_primer)
-            if rv_primer not in already_written:
-                print(f">{rv_primer}\n{all_primers['-'][rv_primer][0]}", file=query)
-                already_written.append(rv_primer)
-
-    return query_path
-
-
-def create_BLAST_query_qpcr(qpcr_scheme_candidates, data_dir):
-    """
-    create a query for the BLAST search (qpcr mode)
-    """
-    already_written = []
+    if mode == "single_tiled":
+        primer_types = ["LEFT", "RIGHT"]
+    elif mode == "qpcr":
+        primer_types = ["PROBE", "LEFT", "RIGHT"]
+    already_written = set()
 
-    query_path = os.path.join(data_dir, "BLAST_query.fasta")
     with open(query_path, "w") as query:
-        for amp in qpcr_scheme_candidates:
-            for primer_type in ["PROBE", "LEFT", "RIGHT"]:
-                name = f"{primer_type}_{qpcr_scheme_candidates[amp][primer_type][1]}_{qpcr_scheme_candidates[amp][primer_type][2]}"
-                if name in already_written:
-                    continue
-                print(f">{name}\n{qpcr_scheme_candidates[amp][primer_type][0]}", file=query)
-                already_written.append(name)
+        for amp in amplicons:
+            for primer_type in primer_types:
+                name = f"{primer_type}_{amp[primer_type][1]}_{amp[primer_type][2]}"
+                if name not in already_written:
+                    print(f">{name}\n{amp[primer_type][0]}", file=query)
+                    already_written.add(name)
     return query_path
 
 
 def run_BLAST(query, blast_db, data_dir, n_threads):
     """
     runs a BLAST search on a search query.
     """
@@ -164,52 +147,49 @@
     return False
 
 
 def predict_non_specific_amplicons_worker(amp, blast_df, max_length, mode):
     """
     Worker function to predict unspecific targets for a single amplicon.
     """
-    name, data = amp
     # get correct primers
     if mode == "single_tiled":
-        primers = [data[2], data[3]]
+        primer_types = ["LEFT", "RIGHT"]
     elif mode == "qpcr":
-        primers = []
-        for primer_type in ["PROBE", "LEFT", "RIGHT"]:
-            primers.append(f"{primer_type}_{data[primer_type][1]}_{data[primer_type][2]}")
+        primer_types = ["PROBE", "LEFT", "RIGHT"]
+    primers = []
+    for primer_type in primer_types:
+        primers.append(f"{primer_type}_{amp[primer_type][1]}_{amp[primer_type][2]}")
     # subset df for primers
     df_amp_primers = blast_df[blast_df["query"].isin(primers)]
     # sort by reference and ref start
     df_amp_primers_sorted = df_amp_primers.sort_values(["ref", "ref_start"])
     # check for off-targets for specific primers
     if check_off_targets(df_amp_primers_sorted, max_length, primers):
-        return name
+        amp["off_targets"] = True
+    else:
+        amp["off_targets"] = False
+    return amp
 
 
 def predict_non_specific_amplicons(amplicons, blast_df, max_length, mode, n_threads):
     """
     Main function to predict unspecific targets within a size range and give
     these primers a high penalty. Uses multiprocessing for parallelization.
     """
-    off_targets = []
     # process amplicons concurrently
     with multiprocessing.Pool(processes=n_threads) as pool:
-        amp_items = amplicons.items()
-        results = pool.starmap(predict_non_specific_amplicons_worker, [(amp, blast_df, max_length, mode) for amp in amp_items])
-    # check results
-    for off_target in results:
-        if off_target is None:
-            continue
-        off_targets.append(off_target)
-        if mode == "single_tiled":
-            amplicons[off_target][5] = amplicons[off_target][5] + config.BLAST_PENALTY
-        elif mode == "qpcr":
-            amplicons[off_target]["penalty"] = amplicons[off_target]["penalty"] + config.BLAST_PENALTY
-
-    return off_targets, amplicons
+        annotated_amps = [
+            result for result in pool.starmap(
+                predict_non_specific_amplicons_worker,
+                [(amp, blast_df, max_length, mode) for amp in amplicons]
+            ) if result is not None
+        ]
+    n_off_targets = sum(amp["off_targets"] for amp in annotated_amps)
+    return n_off_targets, annotated_amps
 
 
 def primer_blast(data_dir, db, query_path, amplicons, max_length, n_threads, log_file, mode):
     """
     performs the blast search for the single or tiled workflow
     """
     print("\n#### Starting varVAMP primerBLAST. ####\n")
@@ -233,38 +213,28 @@
         )
     finally:
         # remove query input
         os.remove(query_path)
 
     blast_df = parse_and_filter_BLAST_output(blast_out)
     print("Predicting non-specific amplicons...")
-    off_target_amplicons, amplicons = predict_non_specific_amplicons(
+    n_off_targets, amplicons = predict_non_specific_amplicons(
         amplicons,
         blast_df,
         max_length,
         mode,
         n_threads
     )
-    success_text = f"varVAMP successfully predicted non-specific amplicons:\n\t> {len(off_target_amplicons)}/{len(amplicons)} amplicons could produce amplicons with the blast db.\n\t> raised their amplicon penalty by {config.BLAST_PENALTY}"
+    if n_off_targets > 0:
+        success_text = f"varVAMP predicted non-specific amplicons:\n\t> {n_off_targets}/{len(amplicons)} amplicons could produce amplicons with the blast db.\n\t> will attempt to avoid them in the final list of amplicons"
+    else:
+        success_text = f"NO off-target amplicons found with the blast db and a total of {len(amplicons)} amplicons"
     print(success_text)
     with open(log_file, 'a') as f:
         print(
             f"\nBLAST results: {success_text}",
             file=f
         )
     print("\n#### off-target search finished ####\n")
 
-    return amplicons, off_target_amplicons
-
+    return amplicons
 
-def write_BLAST_warning(off_target_amplicons, amplicon_scheme, log_file):
-    """
-    for each primer pair that has potential unspecific amplicons
-    write warnings to file.
-    """
-    for amp in off_target_amplicons:
-        if amp in amplicon_scheme:
-            logging.raise_error(
-                f"{amp} could produce off-targets. No better amplicon in this area was found.",
-                log_file,
-                exit=False,
-            )
```

### Comparing `varvamp-1.1.3/varvamp/scripts/consensus.py` & `varvamp-1.2.0/varvamp/scripts/consensus.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.3/varvamp/scripts/default_config.py` & `varvamp-1.2.0/varvamp/scripts/default_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This contains all varVAMP parameters.
 """
 
 # List of all known parameters. DO NOT CHANGE!
 __all__ = [
-    'BLAST_MAX_DIFF', 'BLAST_PENALTY', 'BLAST_SETTINGS', 'BLAST_SIZE_MULTI',
+    'BLAST_MAX_DIFF', 'BLAST_SETTINGS', 'BLAST_SIZE_MULTI',
     'END_OVERLAP',
     'PCR_DNA_CONC', 'PCR_DNTP_CONC', 'PCR_DV_CONC', 'PCR_MV_CONC',
     'PRIMER_3_PENALTY', 'PRIMER_GC_END', 'PRIMER_GC_PENALTY',
     'PRIMER_GC_RANGE', 'PRIMER_HAIRPIN', 'PRIMER_MAX_BASE_PENALTY',
     'PRIMER_MAX_DIMER_TMP', 'PRIMER_MAX_DINUC_REPEATS', 'PRIMER_MAX_POLYX',
     'PRIMER_MIN_3_WITHOUT_AMB', 'PRIMER_PERMUTATION_PENALTY',
     'PRIMER_SIZES', 'PRIMER_SIZE_PENALTY',
@@ -70,15 +70,14 @@
     "reward": 1,
     "penalty": -1,
     "gapopen": 2,
     "gapextend": 1
 }
 BLAST_MAX_DIFF = 0.5  # min percent match between primer and BLAST hit (coverage and/or mismatches)
 BLAST_SIZE_MULTI = 2  # multiplier for the max_amp size of off targets (in relation to max amp size)
-BLAST_PENALTY = 50  # amplicon penalty increase -> considered only if no other possibilities
 
 # nucleotide definitions, do NOT change
 NUCS = set("atcg")
 AMBIG_NUCS = {
     "r": ["a", "g"],
     "y": ["c", "t"],
     "s": ["g", "c"],
```

### Comparing `varvamp-1.1.3/varvamp/scripts/get_config.py` & `varvamp-1.2.0/varvamp/scripts/get_config.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.3/varvamp/scripts/logging.py` & `varvamp-1.2.0/varvamp/scripts/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,14 @@
             "QAMPLICON_LENGTH",
             "QAMPLICON_GC",
             "QAMPLICON_DEL_CUTOFF"
         ),
         (
             "BLAST_MAX_DIFF",
             "BLAST_SIZE_MULTI",
-            "BLAST_PENALTY"
         )
     ]
 
     for tup in all_vars:
         for var in tup:
             if var not in vars(config):
                 raise_error(
@@ -380,15 +379,14 @@
         ("max base penalty", config.PRIMER_MAX_BASE_PENALTY),
         ("primer permutation penalty", config.PRIMER_PERMUTATION_PENALTY),
         ("qpcr flanking primer difference", config.QPRIMER_DIFF),
         ("probe and primer end overlap", config.END_OVERLAP),
         ("qpcr deletion size still considered for deltaG calculation", config.QAMPLICON_DEL_CUTOFF),
         ("maximum difference between primer and blast db", config.BLAST_MAX_DIFF),
         ("multiplier of the maximum length for non-specific amplicons", config.BLAST_SIZE_MULTI),
-        ("blast penalty for off targets", config.BLAST_PENALTY)
     ]
     for var_type, var in non_negative_var:
         if var < 0:
             raise_error(
                 f"{var_type} can not be negative!",
                 log_file
             )
@@ -464,19 +462,14 @@
         )
     if config.BLAST_SIZE_MULTI < 1:
         raise_error(
             "off-targets should be considered at least in the range of the maximal amplicon length.",
             log_file,
             exit=True
         )
-    if config.BLAST_PENALTY < 10:
-        raise_error(
-            "giving a too small penalty could result in the selection of off-target producing amplicons in the final scheme.",
-            log_file,
-        )
     # confirm proper BLAST settings in dictionary
     if not isinstance(config.BLAST_SETTINGS, dict):
         raise_error(
             "BLAST settings have to be in a dictionary format!",
             log_file,
             exit=True
         )
```

### Comparing `varvamp-1.1.3/varvamp/scripts/param_estimation.py` & `varvamp-1.2.0/varvamp/scripts/param_estimation.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.3/varvamp/scripts/primers.py` & `varvamp-1.2.0/varvamp/scripts/primers.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,21 +382,21 @@
     all_primers = {}
 
     for direction, primer_candidates in [("+", left_primer_candidates), ("-", right_primer_candidates)]:
         # sort the primers by penalty, and if same penalty by start
         primer_candidates.sort(key=lambda x: (x[3], x[1]))
         # ini everything with the primer with the lowest penalty
         to_retain = [primer_candidates[0]]
-        primer_ranges = list(range(primer_candidates[0][1], primer_candidates[0][2]+1))
+        primer_ranges = list(range(primer_candidates[0][1], primer_candidates[0][2]))
         primer_set = set(primer_ranges)
 
         for primer in primer_candidates:
             # get the thirds of the primer, only consider the middle
             thirds_len = int((primer[2] - primer[1])/3)
-            primer_positions = list(range(primer[1] + thirds_len, primer[2] - thirds_len + 1))
+            primer_positions = list(range(primer[1] + thirds_len, primer[2] - thirds_len))
             # check if none of the nucleotides of the next primer
             # are already covered by a better primer
             if not any(x in primer_positions for x in primer_set):
                 # update the primer set
                 primer_set.update(primer_positions)
                 # append this primer as it has a low penalty and is not overlapping
                 # with another already retained primer
```

### Comparing `varvamp-1.1.3/varvamp/scripts/qpcr.py` & `varvamp-1.2.0/varvamp/scripts/qpcr.py`

 * *Files 3% similar despite different names*

```diff
@@ -207,21 +207,21 @@
             # ... the amplicon is large enough and is in gc range, ...
             if not hardfilter_amplicon(majority_consensus, left_primer, right_primer):
                 continue
             # ... the probe is close enough to the primer on the same strand
             if "LEFT" in probe:
                 if not qpcr_probes[probe][1] in range(
                         left_primer[2] + config.QPROBE_DISTANCE[0],
-                        left_primer[2] + config.QPROBE_DISTANCE[1] + 1
+                        left_primer[2] + config.QPROBE_DISTANCE[1]
                 ):
                     continue
             elif "RIGHT" in probe:
                 if not right_primer[1] in range(
                         qpcr_probes[probe][2] + config.QPROBE_DISTANCE[0],
-                        qpcr_probes[probe][2] + config.QPROBE_DISTANCE[1] + 1
+                        qpcr_probes[probe][2] + config.QPROBE_DISTANCE[1]
 
                 ):
                     continue
             # ... the primer temps do not differ too much, ...
             primer_temps = (primers.calc_temp(right_primer[0]), primers.calc_temp(left_primer[0]))
             if abs(primer_temps[0] - primer_temps[1]) > config.QPRIMER_DIFF:
                 continue
@@ -254,15 +254,15 @@
     lowest penalty. however, probes are overlapping and there is a high chance that
     left and right primers are found multiple times. to consider only one primer-probe
     combination the probes are also sorted by penalty. therefore, if a primer
     combination has been found already the optimal probe was already selected and
     there is no need to consider this primer probe combination.
     """
 
-    qpcr_scheme_candidates = {}
+    qpcr_scheme_candidates = []
     found_amplicons = []
     amplicon_nr = -1
 
     for probe in qpcr_probes:
         left_subset = flanking_primer_subset(left_primer_candidates, "+", qpcr_probes[probe])
         right_subset = flanking_primer_subset(right_primer_candidates, "-", qpcr_probes[probe])
         # consider if there are primers flanking the probe ...
@@ -275,73 +275,75 @@
             continue
         # ...and this combi is not already present for a probe with a better penalty.
         if primer_combination in found_amplicons:
             continue
         # populate the primer dictionary:
         amplicon_nr += 1
         found_amplicons.append(primer_combination)
-        qpcr_scheme_candidates[f"AMPLICON_{amplicon_nr}"] = {
-            "penalty": qpcr_probes[probe][3] + primer_combination[0][3] + primer_combination[1][3],
-            "PROBE": qpcr_probes[probe],
-            "LEFT": primer_combination[0],
-            "RIGHT": primer_combination[1]
-        }
+        qpcr_scheme_candidates.append(
+            {
+                "id": f"AMPLICON_{amplicon_nr}",
+                "penalty": qpcr_probes[probe][3] + primer_combination[0][3] + primer_combination[1][3],
+                "PROBE": qpcr_probes[probe],
+                "LEFT": primer_combination[0],
+                "RIGHT": primer_combination[1]
+            }
+        )
     # and again sort by total penalty (left + right + probe)
-    qpcr_scheme_candidates = dict(sorted(qpcr_scheme_candidates.items(), key=lambda x: x[1]["penalty"]))
-
     return qpcr_scheme_candidates
 
 
 def process_single_amplicon_deltaG(amplicon, majority_consensus):
     """
     Process a single amplicon to test its deltaG and apply filtering.
     This function will be called concurrently by multiple threads.
     """
-    name, data = amplicon
-    start = data["LEFT"][1]
-    stop = data["RIGHT"][2]
-    seq = majority_consensus[start:stop]
+    seq = majority_consensus[amplicon["LEFT"][1]:amplicon["RIGHT"][2]]
     seq = seq.replace("N", "")
     seq = seq.replace("n", "")
-    amp_positions = list(range(start, stop + 1))
     # check if the amplicon overlaps with an amplicon that was previously
     # found and had a high enough deltaG
-    min_temp = min((primers.calc_temp(data["LEFT"][0]),
-                    primers.calc_temp(data["RIGHT"][0])))
+    min_temp = min((primers.calc_temp(amplicon["LEFT"][0]),
+                    primers.calc_temp(amplicon["RIGHT"][0])))
     # calculate deltaG at the minimal primer temp
-    deltaG = seqfold.dg(seq, min_temp)
+    amplicon["deltaG"] = seqfold.dg(seq, min_temp)
 
-    return deltaG, amp_positions, name
+    return amplicon
 
 
 def test_amplicon_deltaG_parallel(qpcr_schemes_candidates, majority_consensus, n_to_test, deltaG_cutoff, n_threads):
     """
     Test all amplicon deltaGs for the top n hits at the lowest primer temperature
     and filters if they fall below the cutoff. Multiple processes are used
     for processing amplicons in parallel.
     """
-    final_schemes = {}
-    passed_counter = 0  # counter for re-naming amplicons that passed deltaG cutoff
-    amplicon_set = set()
+    final_amplicons = []
 
     # Create a pool of processes to handle the concurrent processing
     with multiprocessing.Pool(processes=n_threads) as pool:
         # Create a list of the first n amplicon tuples for processing
-        amplicons = itertools.islice(qpcr_schemes_candidates.items(), n_to_test)
+        # The list is sorted first on whether offset targets were predicted for the amplicon,
+        # then by penalty. This ensures that amplicons with offset targets are always considered last
+        amplicons = itertools.islice(
+            sorted(qpcr_schemes_candidates, key=lambda x: (x.get("offset_targets", False), x["penalty"])),
+            n_to_test
+        )
         # process amplicons concurrently
         results = pool.starmap(process_single_amplicon_deltaG, [(amp, majority_consensus) for amp in amplicons])
         # Process the results
-        for deltaG, amp_positions, amp_name in results:
+        retained_ranges = []
+        for amp in results:
             # check if the amplicon overlaps with an amplicon that was previously
             # found and had a high enough deltaG
-            if any(x in amp_positions for x in amplicon_set):
+            if amp["deltaG"] <= deltaG_cutoff:
                 continue
-            # and if this passes cutoff make a dict entry and do not allow further
-            # amplicons in that region (they will have a lower penalty)
-            if deltaG > deltaG_cutoff:
-                new_name = f"QPCR_SCHEME_{passed_counter}"
-                final_schemes[new_name] = qpcr_schemes_candidates[amp_name]
-                final_schemes[new_name]["deltaG"] = deltaG
-                amplicon_set.update(amp_positions)
-                passed_counter += 1
+            amp_range = range(amp["LEFT"][1], amp["RIGHT"][2])
+            overlaps_retained = False
+            for r in retained_ranges:
+                if amp_range.start < r.stop and r.start < amp_range.stop:
+                    overlaps_retained = True
+                    break
+            if not overlaps_retained:
+                final_amplicons.append(amp)
+                retained_ranges.append(amp_range)
 
-    return final_schemes
+    return final_amplicons
```

### Comparing `varvamp-1.1.3/varvamp/scripts/regions.py` & `varvamp-1.2.0/varvamp/scripts/regions.py`

 * *Files identical despite different names*

### Comparing `varvamp-1.1.3/varvamp/scripts/reporting.py` & `varvamp-1.2.0/varvamp/scripts/reporting.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_pdf import PdfPages
 
 
 # varVAMP
 from varvamp.scripts import primers
 from varvamp.scripts import config
+from varvamp.scripts import logging
 
 
 def write_fasta(path, seq_id, seq):
     """
     write fasta files
     """
     name = f"{seq_id}.fasta"
@@ -44,27 +45,25 @@
     write primer regions as bed file
     """
 
     if mode == "probe":
         outfile = f"{path}probe_regions.bed"
     else:
         outfile = f"{path}primer_regions.bed"
-    counter = 0
 
     with open(outfile, 'w') as o:
-        for region in primer_regions:
+        for counter, region in enumerate(primer_regions):
             print(
                 "ambiguous_consensus",
                 region[0],
                 region[1],
                 "REGION_"+str(counter),
                 sep="\t",
                 file=o
             )
-            counter += 1
 
 
 def write_primers_to_bed(outfile, primer_name, primer_properties, direction):
     """
     write primers as bed file
     """
     with open(outfile, 'a') as o:
@@ -117,158 +116,173 @@
     for permutation in permutations:
         gc += primers.calc_gc(permutation)
         temp += primers.calc_temp(permutation)
 
     return round(gc/len(permutations), 1), round(temp/len(permutations), 1)
 
 
-def write_qpcr_to_files(path, final_schemes, ambiguous_consensus):
+def write_qpcr_to_files(path, final_schemes, ambiguous_consensus, log_file):
     """
     write all relevant bed files and tsv file for the qPCR design
     """
 
     tsv_file = os.path.join(path, "qpcr_design.tsv")
     tsv_file_2 = os.path.join(path, "qpcr_primers.tsv")
     primer_bed_file = os.path.join(path, "primers.bed")
     amplicon_bed_file = os.path.join(path, "amplicons.bed")
     primer_fasta_file = os.path.join(path, "oligos.fasta")
 
     with open(tsv_file, "w") as tsv, open(tsv_file_2, "w") as tsv2, open(amplicon_bed_file, "w") as bed, open(primer_fasta_file, "w") as fasta:
         print(
-            "qpcr_scheme\toligo_type\tstart\tstop\tseq\tsize\tgc_best\ttemp_best\tmean_gc\tmean_temp\tpenalty",
+            "qpcr_scheme\toligo_type\tstart\tstop\tseq\tsize\tgc_best\ttemp_best\tmean_gc\tmean_temp\tpenalty\toff_target_amplicons",
             file=tsv2
         )
         print(
-            "qpcr_scheme\tpenalty\tdeltaG\tlength\tstart\tstop\tseq",
+            "qpcr_scheme\toff_target_amplicons\tpenalty\tdeltaG\tlength\tstart\tstop\tseq",
             file=tsv
         )
-        for scheme in final_schemes:
+        for n, amp in enumerate(final_schemes):
+            amp_name = f"QPCR_SCHEME_{n}"
             # write bed amplicon file
             print(
                 "ambiguous_consensus",
-                final_schemes[scheme]["LEFT"][1],
-                final_schemes[scheme]["RIGHT"][2],
-                scheme,
-                round(final_schemes[scheme]["penalty"], 1),
+                amp["LEFT"][1],
+                amp["RIGHT"][2],
+                amp_name,
+                round(amp["penalty"], 1),
+                ".",
                 sep="\t",
                 file=bed
             )
             # write tsv
-            amplicon_start = final_schemes[scheme]["LEFT"][1]
-            amplicon_stop = final_schemes[scheme]["RIGHT"][2]
+            amplicon_start = amp["LEFT"][1]
+            amplicon_stop = amp["RIGHT"][2]
+            if "off_targets" in amp:
+                if amp["off_targets"]:
+                    amplicon_has_off_target = "Yes"
+                    write_BLAST_warning(amp_name, log_file)
+                else:
+                    amplicon_has_off_target = "No"
+            else:
+                amplicon_has_off_target = "n.d."
             amplicon_seq = ambiguous_consensus[amplicon_start:amplicon_stop]
             print(
-                scheme,
-                round(final_schemes[scheme]["penalty"], 1),
-                final_schemes[scheme]["deltaG"],
+                amp_name,
+                amplicon_has_off_target,
+                round(amp["penalty"], 1),
+                amp["deltaG"],
                 len(amplicon_seq),
                 amplicon_start + 1,
                 amplicon_stop,
                 amplicon_seq,
                 sep="\t",
                 file=tsv
             )
             # write tsv2
-            for oligo_type in final_schemes[scheme]:
-                if oligo_type == "penalty" or oligo_type == "deltaG":
-                    continue
-                seq = ambiguous_consensus[final_schemes[scheme][oligo_type][1]:final_schemes[scheme][oligo_type][2]]
-                if oligo_type == "RIGHT" or all([oligo_type == "PROBE", final_schemes[scheme]["PROBE"][5] == "-"]):
+            for oligo_type in ["LEFT", "PROBE", "RIGHT"]:
+                seq = ambiguous_consensus[amp[oligo_type][1]:amp[oligo_type][2]]
+                if oligo_type == "RIGHT" or (oligo_type == "PROBE" and amp["PROBE"][5] == "-"):
                     seq = primers.rev_complement(seq)
                     direction = "-"
                 else:
                     direction = "+"
 
                 permutations = get_permutations(seq)
                 gc, temp = calc_mean_stats(permutations)
 
                 print(
-                    scheme,
+                    amp_name,
                     oligo_type,
-                    final_schemes[scheme][oligo_type][1] + 1,
-                    final_schemes[scheme][oligo_type][2],
+                    amp[oligo_type][1] + 1,
+                    amp[oligo_type][2],
                     seq.upper(),
                     len(seq),
-                    round(primers.calc_gc(final_schemes[scheme][oligo_type][0]), 1),
-                    round(primers.calc_temp(final_schemes[scheme][oligo_type][0]), 1),
+                    round(primers.calc_gc(amp[oligo_type][0]), 1),
+                    round(primers.calc_temp(amp[oligo_type][0]), 1),
                     gc,
                     temp,
-                    round(final_schemes[scheme][oligo_type][3], 1),
+                    round(amp[oligo_type][3], 1),
+                    amplicon_has_off_target,
                     sep="\t",
                     file=tsv2
                 )
                 # write primer bed file
                 write_primers_to_bed(
                     primer_bed_file,
-                    f"{scheme}_{oligo_type}",
-                    final_schemes[scheme][oligo_type],
+                    f"{amp_name}_{oligo_type}",
+                    amp[oligo_type],
                     direction
                 )
                 # write fasta
-                print(f">{scheme}_{oligo_type}\n{seq.upper()}", file=fasta)
+                print(f">{amp_name}_{oligo_type}\n{seq.upper()}", file=fasta)
 
 
-def write_scheme_to_files(path, amplicon_scheme, ambiguous_consensus, mode):
+def write_scheme_to_files(path, amplicon_scheme, ambiguous_consensus, mode, log_file):
     """
     write all relevant bed files and a tsv file with all primer stats
     """
     tsv_file = os.path.join(path, "primers.tsv")
     primer_bed_file = os.path.join(path, "primers.bed")
     amplicon_bed_file = os.path.join(path, "amplicons.bed")
     tabular_file = os.path.join(path, "primer_to_amplicon_assignment.tabular")
 
-    counter = 0
-
     # open files to write
     with open(tsv_file, "w") as tsv, open(amplicon_bed_file, "w") as bed, open(tabular_file, "w") as tabular:
         # write header for primer tsv
         print(
-            "amlicon_name\tamplicon_length\tprimer_name\talternate_primer_name\tpool\tstart\tstop\tseq\tsize\tgc_best\ttemp_best\tmean_gc\tmean_temp\tpenalty",
+            "amlicon_name\tamplicon_length\tprimer_name\talternate_primer_name\tpool\tstart\tstop\tseq\tsize\tgc_best\ttemp_best\tmean_gc\tmean_temp\tpenalty\toff_target_amplicons",
             file=tsv
         )
-
-        for pool in amplicon_scheme:
+        amplicon_bed_records = []
+        primer_bed_records = []
+        primer_assignment_records = []
+        pools = {amp.get("pool", 0) for amp in amplicon_scheme}
+        for pool in pools:
             if mode == "single":
                 primer_fasta_file = os.path.join(path, "primers.fasta")
             else:
                 primer_fasta_file = os.path.join(path, f"primers_pool_{pool}.fasta")
             with open(primer_fasta_file, "w") as primer_fasta:
-                for amp in amplicon_scheme[pool]:
+                for counter, amp in enumerate(amplicon_scheme[pool::len(pools)]):
                     # give a new amplicon name
-                    new_name = f"AMPLICON_{str(counter)}"
-                    counter += 1
+                    amplicon_index = counter*len(pools) + pool
+                    new_name = f"AMPLICON_{amplicon_index}"
                     # get left and right primers and their names
-                    primer_names = list(amplicon_scheme[pool][amp].keys())
-                    left = (primer_names[0], amplicon_scheme[pool][amp][primer_names[0]])
-                    right = (primer_names[1], amplicon_scheme[pool][amp][primer_names[1]])
-                    amp_length = right[1][2] - left[1][1]
+                    amp_length = amp["RIGHT"][2] - amp["LEFT"][1]
+                    if "off_targets" in amp:
+                        if amp["off_targets"]:
+                            amplicon_has_off_target = "Yes"
+                            write_BLAST_warning(amp_name, log_file)
+                        else:
+                            amplicon_has_off_target = "No"
+                    else:
+                        amplicon_has_off_target = "n.d."
                     # write amplicon bed
                     if mode == "tiled":
                         bed_score = pool
                     elif mode == "single":
-                        bed_score = round(left[1][3] + right[1][3], 1)
-                    print(
-                        "ambiguous_consensus",
-                        left[1][1],
-                        right[1][2],
-                        new_name,
-                        bed_score,
-                        sep="\t",
-                        file=bed
+                        bed_score = round(amp["LEFT"][3] + amp["RIGHT"][3], 1)
+                    amplicon_bed_records.append(
+                        (
+                            amp["LEFT"][1],
+                            amp["RIGHT"][2],
+                            new_name,
+                            bed_score
+                        )
                     )
-                    # write primer assignments tabular file
-                    print(
-                        f"{new_name}_LEFT",
-                        f"{new_name}_RIGHT",
-                        sep="\t",
-                        file=tabular
+                    primer_assignment_records.append(
+                        (
+                            # will need amplicon_index for sorting
+                            amplicon_index,
+                            (f"{new_name}_LEFT", f"{new_name}_RIGHT")
+                        )
                     )
                     # write primer tsv and primer bed
-                    for direction, primer in [("+", left), ("-", right)]:
-                        seq = ambiguous_consensus[primer[1][1]:primer[1][2]]
+                    for direction, primer in [("+", amp["LEFT"]), ("-", amp["RIGHT"])]:
+                        seq = ambiguous_consensus[primer[1]:primer[2]]
                         if direction == "-":
                             seq = primers.rev_complement(seq)
                             primer_name = f"{new_name}_RIGHT"
                         else:
                             primer_name = f"{new_name}_LEFT"
                         # write primers to fasta pool file
                         print(f">{primer_name}\n{seq.upper()}", file=primer_fasta)
@@ -276,53 +290,76 @@
                         permutations = get_permutations(seq)
                         gc, temp = calc_mean_stats(permutations)
                         # write tsv file
                         print(
                             new_name,
                             amp_length,
                             primer_name,
-                            primer[0],
+                            primer[-1],
                             pool,
-                            primer[1][1] + 1,
-                            primer[1][2],
+                            primer[1] + 1,
+                            primer[2],
                             seq.upper(),
-                            len(primer[1][0]),
-                            round(primers.calc_gc(primer[1][0]), 1),
-                            round(primers.calc_temp(primer[1][0]), 1),
+                            len(primer[0]),
+                            round(primers.calc_gc(primer[0]), 1),
+                            round(primers.calc_temp(primer[0]), 1),
                             gc,
                             temp,
-                            round(primer[1][3], 1),
+                            round(primer[3], 1),
+                            amplicon_has_off_target,
                             sep="\t",
                             file=tsv
                         )
-                        # write primer bed file
-                        write_primers_to_bed(
-                            primer_bed_file,
-                            primer_name,
-                            primer[1],
-                            direction
+                        primer_bed_records.append(
+                            (
+                                # will need amplicon_index for sorting
+                                amplicon_index,
+                                (primer_name, primer, direction)
+                            )
                         )
+        # write amplicon bed with amplicons sorted by start position
+        for record in sorted(amplicon_bed_records, key=lambda x: x[0]):
+            print(
+                "ambiguous_consensus",
+                *record,
+                ".",
+                sep="\t",
+                file=bed
+            )
+        # use sorting by amplicon index for primer assignment file
+        for record in sorted(primer_assignment_records):
+            print(
+                *record[1],
+                sep="\t",
+                file=tabular
+            )
+        # same for primer bed
+        for record in sorted(primer_bed_records):
+            write_primers_to_bed(
+                primer_bed_file,
+                *record[1]
+            )
 
 
 def write_dimers(path, primer_dimers):
     """
     write dimers for which no replacement was found to file
     """
     tsv_file = os.path.join(path, "unsolvable_primer_dimers.tsv")
     with open(tsv_file, "w") as tsv:
         print(
             "pool\tprimer_name_1\tprimer_name_2\tdimer melting temp",
             file=tsv
         )
-        for dimers in primer_dimers:
+        for pool, primer1, primer2 in primer_dimers:
             print(
-                dimers[0][0],
-                dimers[0][2],
-                dimers[1][2],
-                round(primers.calc_dimer(dimers[0][3][0], dimers[1][3][0]).tm, 1),
+                pool,
+                primer1[1],
+                primer2[1],
+                round(primers.calc_dimer(primer1[2][0], primer2[2][0]).tm, 1),
                 sep="\t",
                 file=tsv
             )
 
 def entropy(chars, states):
     """
     input is a list of characters or numbers.
@@ -414,60 +451,54 @@
         ax[1].hlines(primer_position, all_primers[direction][primer][1], all_primers[direction][primer][2], linewidth=5, color=primer_color, label=primer_label)
 
 
 def amplicon_subplot(ax, amplicon_scheme):
     """
     creates the amplicon subplot
     """
-    counter = 0
-    for pool in amplicon_scheme:
-        for amp in amplicon_scheme[pool]:
-            if pool == 0:
-                position_amp = 0.7
-                position_text = 0.6
-            elif pool == 1:
-                position_amp = 0.6
-                position_text = 0.65
-            primer_names = [i for i in amplicon_scheme[pool][amp]]
-            left = amplicon_scheme[pool][amp][primer_names[0]]
-            right = amplicon_scheme[pool][amp][primer_names[1]]
-            # amplicons
-            ax[1].hlines(position_amp, left[1], right[2], linewidth=5)
-            # text
-            ax[1].text(right[2] - (right[2]-left[1])/2, position_text, str(counter), fontsize=8)
-            # primers
-            ax[1].hlines(position_amp, left[1], left[2], linewidth=5, color="red")
-            ax[1].hlines(position_amp, right[1], right[2], linewidth=5, color="red")
-            counter += 1
+    for counter, amp in enumerate(amplicon_scheme):
+        pool = amp.get("pool", 0)
+        if pool == 0:
+            position_amp = 0.7
+            position_text = 0.6
+        elif pool == 1:
+            position_amp = 0.6
+            position_text = 0.65
+        left = amp["LEFT"]
+        right = amp["RIGHT"]
+        # amplicons
+        ax[1].hlines(position_amp, left[1], right[2], linewidth=5)
+        # text
+        ax[1].text(right[2] - (right[2]-left[1])/2, position_text, str(counter), fontsize=8)
+        # primers
+        ax[1].hlines(position_amp, left[1], left[2], linewidth=5, color="red")
+        ax[1].hlines(position_amp, right[1], right[2], linewidth=5, color="red")
     # legends
     ax[1].hlines(position_amp, left[1]+config.PRIMER_SIZES[1], right[2]-config.PRIMER_SIZES[1], linewidth=5, label="amplicons")
     ax[1].hlines(position_amp, left[1], left[2], linewidth=5, color="red", label="primers")
 
 
 def qpcr_subplot(ax, amplicon_scheme):
     """
     creates the qpcr subplot
     """
-    counter = 0
-
-    for scheme in amplicon_scheme:
-        left = amplicon_scheme[scheme]["LEFT"]
-        right = amplicon_scheme[scheme]["RIGHT"]
-        probe = amplicon_scheme[scheme]["PROBE"]
+    for counter, amp in enumerate(amplicon_scheme):
+        left = amp["LEFT"]
+        right = amp["RIGHT"]
+        probe = amp["PROBE"]
         # amplicons
         ax[1].hlines(0.8, left[1], right[2], linewidth=5)
         # text
         ax[1].text(right[2] - (right[2]-left[1])/2, 0.65, str(counter), fontsize=8)
         # primers
         ax[1].hlines(0.8, left[1], left[2], linewidth=5, color="red")
         ax[1].hlines(0.8, right[1], right[2], linewidth=5, color="red")
         # probe
         ax[1].hlines(0.75, probe[1], probe[2], linewidth=5, color="darkgrey")
 
-        counter += 1
     # legends
     ax[1].hlines(0.8, left[1]+config.PRIMER_SIZES[1], right[2]-config.PRIMER_SIZES[1], linewidth=5, label="amplicons")
     ax[1].hlines(0.8, left[1], left[2], linewidth=5, color="red", label="primers")
     ax[1].hlines(0.75, probe[1], probe[2], linewidth=5, color="darkgrey", label="probe")
 
 
 def varvamp_plot(path, alignment_cleaned, primer_regions, all_primers=None, amplicon_scheme=None, probe_regions=None):
@@ -511,37 +542,32 @@
 
 def get_SINGLE_TILED_primers_for_plot(amplicon_scheme):
     """
     get the primers for per base pair plot (single, tiled)
     """
     amplicon_primers = []
 
-    for pool in amplicon_scheme:
-        for amp in amplicon_scheme[pool]:
-            primer_names = [i for i in amplicon_scheme[pool][amp]]
-            left = amplicon_scheme[pool][amp][primer_names[0]]
-            right = amplicon_scheme[pool][amp][primer_names[1]]
-            amplicon_primers.append((primer_names[0], left))
-            amplicon_primers.append((primer_names[1], right))
+    for counter, amp in enumerate(amplicon_scheme):
+        for type in ["LEFT", "RIGHT"]:
+            primer_name = f"AMPLICON_{counter}_{type}"
+            amplicon_primers.append((primer_name, amp[type]))
 
     return amplicon_primers
 
 
 def get_QPCR_primers_for_plot(amplicon_schemes):
     """
     get the primers for per base pair plot (qpcr)
     """
     amplicon_primers = []
 
-    for scheme in amplicon_schemes:
-        for type in amplicon_schemes[scheme]:
-            if type == "penalty" or type == "deltaG":
-                continue
-            primer_name = f"{scheme}_{type}"
-            amplicon_primers.append((primer_name, amplicon_schemes[scheme][type]))
+    for counter, amp in enumerate(amplicon_schemes):
+        for type in ["PROBE", "LEFT", "RIGHT"]:
+            primer_name = f"QPCR_SCHEME_{counter}_{type}"
+            amplicon_primers.append((primer_name, amp[type]))
 
     return amplicon_primers
 
 
 def per_base_mismatch_plot(path, amplicon_scheme, threshold, mode="SINGLE/TILED"):
     """
     per base pair mismatch multiplot
@@ -577,7 +603,19 @@
                 if threshold < 1:
                     ax[idx].set_ylim(0, 1-threshold)
                 else:
                     ax[idx].set_ylim(0, 0.001)
             # - to pdf
             pdf.savefig(fig, bbox_inches='tight')
             plt.close()
+
+
+def write_BLAST_warning(amplicon_name, log_file):
+    """
+    for each primer pair that has potential unspecific amplicons
+    write warnings to file.
+    """
+    logging.raise_error(
+        f"{amplicon_name} could produce off-targets. No better amplicon in this area was found.",
+        log_file,
+        exit=False,
+    )
```

### Comparing `varvamp-1.1.3/varvamp/scripts/scheme.py` & `varvamp-1.2.0/varvamp/scripts/scheme.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,20 +17,18 @@
     never goes to an amplicon that is in the wrong direction.
     """
     graph = {}
     for node in nodes:
         graph[node] = {}
 
     graph.update(init_graph)
-
     for node, neighbors in graph.items():
         for neighbor in neighbors.keys():
             if graph[neighbor].get(node, False) is False:
-                graph[neighbor][node] = float("infinity")
-
+                graph[neighbor][node] = (float("infinity"), 0)
     return graph
 
 
 class Graph(object):
     """
     a graph class
     """
@@ -57,100 +55,109 @@
 
     def value(self, node1, node2):
         """
         Returns the value of an edge between two nodes.
         """
         return self.graph[node1][node2]
 
-
 def find_amplicons(all_primers, opt_len, max_len):
     """
     finds all possible amplicons, creates a dictionary
     """
     amplicon_number = 0
-    amplicon_dict = {}
+    amplicons = []
 
     for left_name in all_primers["+"]:
         left_primer = all_primers["+"][left_name]
         for right_name in all_primers["-"]:
             right_primer = all_primers["-"][right_name]
             amplicon_length = right_primer[2] - left_primer[1]
             if not opt_len <= amplicon_length <= max_len:
                 continue
             if primers.calc_dimer(left_primer[0], right_primer[0]).tm > config.PRIMER_MAX_DIMER_TMP:
                 continue
             # calculate length dependend amplicon costs as the cumulative primer
             # penalty multiplied by the e^(fold length of the optimal length).
             amplicon_costs = (right_primer[3] + left_primer[3])*math.exp(amplicon_length/opt_len)
             amplicon_name = "AMPLICON_"+str(amplicon_number)
-            amplicon_dict[amplicon_name] = [
-                left_primer[1],  # start
-                right_primer[2],  # stop
-                left_name,  # name left primer
-                right_name,  # name right primer
-                amplicon_length,  # amplicon length
-                amplicon_costs  # costs
-            ]
+            amplicons.append(
+                {
+                    "id": amplicon_name,
+                    "penalty": amplicon_costs,
+                    "length": amplicon_length,
+                    "LEFT": left_primer + [left_name],
+                    "RIGHT": right_primer + [right_name],
+                }
+            )
             amplicon_number += 1
-
-    return amplicon_dict
+    return amplicons
 
 
 def create_amplicon_graph(amplicons, min_overlap):
     """
     creates the amplicon graph.
     """
     # ini graph and vertices
     amplicon_graph = {}
     nodes = []
 
     # add the maximum len of a primer to ensure that possible amplicon starts
     # before the min overlap
     min_overlap = min_overlap + config.PRIMER_SIZES[2]
 
-    for current in amplicons:
+    for current_amplicon in amplicons:
         # remember all vertices
-        nodes.append(current)
-        current_amplicon = amplicons[current]
-        start = current_amplicon[0] + current_amplicon[4]/2
-        stop = current_amplicon[1] - min_overlap
-        for next_amp in amplicons:
-            next_amplicon = amplicons[next_amp]
+        amplicon_id = current_amplicon["id"]
+        nodes.append(amplicon_id)
+        start = current_amplicon["LEFT"][1] + current_amplicon["length"]/2
+        stop = current_amplicon["RIGHT"][2] - min_overlap
+        for next_amplicon in amplicons:
             # check if the next amplicon lies within the start/stop range of
             # the current amplicon and if its non-overlapping part is large
             # enough to ensure space for a primer and the min overlap of the
             # following amplicon.
-            if not all([start <= next_amplicon[0] <= stop, next_amplicon[1] > current_amplicon[1] + next_amplicon[4]/2]):
-                continue
-            if current not in amplicon_graph:
-                amplicon_graph[current] = {next_amp: next_amplicon[5]}
-            else:
-                amplicon_graph[current][next_amp] = next_amplicon[5]
+            if start <= next_amplicon["LEFT"][1] <= stop and next_amplicon["RIGHT"][2] > current_amplicon["RIGHT"][2] + next_amplicon["length"]/2:
+                if amplicon_id not in amplicon_graph:
+                    amplicon_graph[amplicon_id] = {
+                        next_amplicon["id"]: (
+                            next_amplicon.get("off_targets", False),
+                            next_amplicon["penalty"]
+                        )
+                    }
+                else:
+                    amplicon_graph[amplicon_id][next_amplicon["id"]] = (
+                        next_amplicon.get("off_targets", False),
+                        next_amplicon["penalty"]
+                    )
 
     # return a graph object
     return Graph(nodes, amplicon_graph)
 
 
 def dijkstra_algorithm(graph, start_node):
     """
     implementation of the dijkstra algorithm
     """
 
     previous_nodes = {}
-    shortest_path = {node: float('infinity') for node in graph.get_nodes()}
-    shortest_path[start_node] = 0
+    shortest_path = {node: (float('infinity'), 0) for node in graph.get_nodes()}
+    shortest_path[start_node] = (0, 0)
 
-    nodes_to_test = [(0, start_node)]
+    nodes_to_test = [((0, 0), start_node)]
 
     while nodes_to_test:
         current_distance, current_node = heapq.heappop(nodes_to_test)
         if current_distance > shortest_path[current_node]:
             continue
         for neighbor in graph.get_neighbors(current_node):
-            distance = current_distance + graph.value(current_node, neighbor)
+            off_targets, base_penalty = graph.value(current_node, neighbor)
+            distance = (
+                current_distance[0] + off_targets,
+                current_distance[1] + base_penalty
+            )
             # Only consider this new path if it's a better path
             if not distance < shortest_path[neighbor]:
                 continue
             shortest_path[neighbor] = distance
             previous_nodes[neighbor] = current_node
             heapq.heappush(nodes_to_test, (distance, neighbor))
 
@@ -163,19 +170,20 @@
     nodes that have the same maximum end position
     """
     stop_nucleotide, possible_end_nodes = 0, {}
 
     for node in previous_nodes.keys():
         # check if a node has a larger stop -> empty dict and set new
         # best stop nucleotide
-        if amplicons[node][1] > stop_nucleotide:
+        amplicon_stop = amplicons[node]["RIGHT"][2]
+        if amplicon_stop > stop_nucleotide:
             possible_end_nodes = {node: shortest_path[node]}
-            stop_nucleotide = amplicons[node][1]
+            stop_nucleotide = amplicon_stop
         # if nodes have the same stop nucleotide, add to dictionary
-        elif amplicons[node][1] == stop_nucleotide:
+        elif amplicon_stop == stop_nucleotide:
             possible_end_nodes[node] = shortest_path[node]
 
     # return the end node with the lowest penalty costs
     return min(possible_end_nodes.items(), key=lambda x: x[1])
 
 
 def get_min_path(previous_nodes, start_node, target_node):
@@ -192,109 +200,107 @@
     # Add the start node manually
     path.append(start_node)
 
     # return the inverse list
     return path[::-1]
 
 
-def create_scheme_dic(amplicon_scheme, amplicons, all_primers):
+def create_scheme(amplicon_path, amplicons_by_id):
     """
-    creates the final scheme dictionary
+    creates the final tiled-amplicon scheme
     """
-
-    scheme_dictionary = {
-        0: {},
-        1: {}
-    }
+    amplicon_scheme = []
 
     for pool in (0, 1):
-        for amp in amplicon_scheme[pool::2]:
-            scheme_dictionary[pool][amp] = {}
-            primer_pair = [amplicons[amp][2], amplicons[amp][3]]
-            scheme_dictionary[pool][amp][primer_pair[0]] = all_primers["+"][primer_pair[0]]
-            scheme_dictionary[pool][amp][primer_pair[1]] = all_primers["-"][primer_pair[1]]
+        for amp_id in amplicon_path[pool::2]:
+            amplicons_by_id[amp_id]["pool"] = pool
+            amplicon_scheme.append(amplicons_by_id[amp_id])
 
-    return scheme_dictionary
+    return amplicon_scheme
 
 
-def find_best_covering_scheme(amplicons, amplicon_graph, all_primers):
+def find_best_covering_scheme(amplicons, amplicon_graph):
     """
     this brute forces the amplicon scheme search until the largest
     coverage with the minimal costs is achieved.
     """
     # ini
     best_coverage = 0
-    max_stop = max(amplicons.items(), key=lambda x: x[1])[1][1]
-    lowest_costs = float('infinity')
-
-    for start_node in amplicons:
+    max_stop = max(amplicons, key=lambda x: x["RIGHT"][2])["RIGHT"][2]
+    lowest_costs = (float('infinity'),)
+    # a dict for fast access to amplicons by their ID
+    amps_by_id = {amp["id"]: amp for amp in amplicons}
+    for amplicon in amplicons:
         # if the currently best coverage + start nucleotide of the currently tested amplicon
         # is smaller than the maximal stop nucleotide there might be a better amplicon
         # scheme that covers more of the genome
-        if amplicons[start_node][0] + best_coverage <= max_stop:
-            previous_nodes, shortest_path = dijkstra_algorithm(amplicon_graph, start_node)
+        if amplicon["LEFT"][1] + best_coverage <= max_stop:
+            previous_nodes, shortest_path = dijkstra_algorithm(amplicon_graph, amplicon["id"])
             # only continue if there are previous_nodes
             if previous_nodes:
-                target_node, costs = get_end_node(previous_nodes, shortest_path, amplicons)
-                coverage = amplicons[target_node][1] - amplicons[start_node][0]
+                target_node, costs = get_end_node(previous_nodes, shortest_path, amps_by_id)
+                coverage = amps_by_id[target_node]["RIGHT"][2] - amplicon["LEFT"][1]
                 # if the new coverage is larger, go for the larger coverage
                 if coverage > best_coverage:
-                    best_start_node = start_node
+                    best_start_node = amplicon["id"]
                     best_target_node = target_node
                     best_previous_nodes = previous_nodes
                     lowest_costs = costs
                     best_coverage = coverage
                 # if the coverages are identical, go for the lowest costs
                 elif coverage == best_coverage:
                     if costs < lowest_costs:
-                        best_start_node = start_node
+                        best_start_node = amplicon["id"]
                         best_target_node = target_node
                         best_previous_nodes = previous_nodes
                         lowest_costs = costs
                         best_coverage = coverage
             else:
                 # check if the single amplicon has the largest coverage so far
-                coverage = amplicons[start_node][1] - amplicons[start_node][0]
+                coverage = amplicon["length"]
                 if coverage > best_coverage:
-                    best_start_node = start_node
+                    best_start_node = amplicon["id"]
                     best_previous_nodes = previous_nodes
-                    lowest_costs = amplicons[start_node][5]
+                    lowest_costs = (
+                        amplicon.get("off_targets", False), amplicon["penalty"])
                     best_coverage = coverage
         # no need to check more, the best covering amplicon scheme was found and
         # has the minimal costs compared to the schemes with the same coverage
         else:
             break
 
     if best_previous_nodes:
-        amplicon_scheme = get_min_path(best_previous_nodes, best_start_node, best_target_node)
+        amplicon_path = get_min_path(best_previous_nodes, best_start_node, best_target_node)
     else:
         # if no previous nodes are found but the single amplicon results in the largest
         # coverage - return as the best scheme
-        amplicon_scheme = [best_start_node]
-
-    return best_coverage, create_scheme_dic(amplicon_scheme, amplicons, all_primers)
+        amplicon_path = [best_start_node]
+    return best_coverage, create_scheme(amplicon_path, amps_by_id)
 
 
 def test_scheme_for_dimers(amplicon_scheme):
     """
     test the lowest-cost scheme for primer dimers
     """
 
     primer_dimers = []
-
-    for pool in amplicon_scheme:
+    pools = {amp["pool"] for amp in amplicon_scheme}
+    for pool in pools:
         # test the primer dimers only within the respective pools
         tested_primers = []
-        for amp in amplicon_scheme[pool]:
-            for primer in amplicon_scheme[pool][amp]:
+        for amp_index, amp in enumerate(amplicon_scheme):
+            if amp["pool"] != pool:
+                continue
+            for primer in ["LEFT", "RIGHT"]:
                 # remember where the currrent primer was in the scheme
-                current_primer = (pool, amp, primer, amplicon_scheme[pool][amp][primer])
-                current_seq = current_primer[3][0]
+                # store the amplicon's index in the scheme, the current primer's original name and its details
+                current_primer = (amp_index, amp[primer][-1], amp[primer][:-1])
+                current_seq = current_primer[2][0]
                 for tested in tested_primers:
-                    tested_seq = tested[3][0]
+                    tested_seq = tested[2][0]
                     if primers.calc_dimer(current_seq, tested_seq).tm <= config.PRIMER_MAX_DIMER_TMP:
                         continue
                     primer_dimers.append((current_primer, tested))
                 # and remember all tested primers
                 tested_primers.append(current_primer)
 
     return primer_dimers
@@ -305,45 +311,45 @@
     get overlapping primers of a primer dimer pair that have been previously
     excluded. returns list of list with possible primers for each primer
     in primer dimer.
     """
 
     overlapping_primers = []
     # test each primer in dimer
-    for primer in dimer:
+    for amp_index, primer_name, primer in dimer:
         overlapping_primers_temp = []
-        thirds_len = int((primer[3][2] - primer[3][1]) / 3)
+        thirds_len = int((primer[2] - primer[1]) / 3)
         # get the middle third of the primer (here are the previously excluded primers)
-        overlap_set = set(range(primer[3][1] + thirds_len, primer[3][2] - thirds_len + 1))
+        overlap_set = set(range(primer[1] + thirds_len, primer[2] - thirds_len))
         # check in which list to look for them
-        if "RIGHT" in primer[2]:
+        if "RIGHT" in primer_name:
             primers_to_test = right_primer_candidates
         else:
             primers_to_test = left_primer_candidates
         # and check this list for all primers that overlap
         for potential_new in primers_to_test:
-            primer_positions = list(range(potential_new[1], potential_new[2]+1))
+            primer_positions = list(range(potential_new[1], potential_new[2]))
             if not any(x in primer_positions for x in overlap_set):
                 continue
-            overlapping_primers_temp.append((primer[0], primer[1], primer[2], potential_new))
+            overlapping_primers_temp.append((amp_index, primer_name, potential_new))
 
         overlapping_primers.append(overlapping_primers_temp)
 
     return overlapping_primers
 
 
 def test_overlaps_for_dimers(overlapping_primers):
     """
     test the overlapping primers for dimers. return new primers.
     """
     for first_overlap in overlapping_primers[0]:
         for second_overlap in overlapping_primers[1]:
             # return the first match. primers are sorted by penalty.
             # first pair that makes it has the lowest penalty
-            if primers.calc_dimer(first_overlap[3][0], second_overlap[3][0]).tm <= config.PRIMER_MAX_DIMER_TMP:
+            if primers.calc_dimer(first_overlap[2][0], second_overlap[2][0]).tm <= config.PRIMER_MAX_DIMER_TMP:
                 return [first_overlap, second_overlap]
 
 
 def check_and_solve_heterodimers(amplicon_scheme, left_primer_candidates, right_primer_candidates, all_primers):
     """
     check scheme for heterodimers, try to find
     new primers that overlap and replace the existing ones.
@@ -356,57 +362,59 @@
 
     if primer_dimers:
         print(f"varVAMP found {len(primer_dimers)} dimer pairs in scheme ... trying to find replacements")
     else:
         return []
 
     for dimer in primer_dimers:
-        # get overlapping primers that have not been considere
+        # get overlapping primers that have not been considered
         overlapping_primers = get_overlapping_primers(dimer, left_primer_candidates, right_primer_candidates)
         # test all possible primers against each other for dimers
         new_primers = test_overlaps_for_dimers(overlapping_primers)
         # now change these primers in the scheme
         if new_primers:
-            for new in new_primers:
+            for amp_index, primer_name, primer in new_primers:
                 # overwrite in final scheme
-                amplicon_scheme[new[0]][new[1]][new[2]] = new[3]
-                # and in all primers
-                if "LEFT" in new[2]:
+                # ATTENTION: doesn't update the amplicon penalty currently
+                # This is ok only because that value isn't used after and doesn't get reported anywhere.
+                if "LEFT" in primer_name:
                     strand = "+"
+                    amplicon_scheme[amp_index]["LEFT"] = primer + [primer_name]
                 else:
                     strand = "-"
-                all_primers[strand][new[2]] = new[3]
-
-    primer_dimers = test_scheme_for_dimers(amplicon_scheme)
+                    amplicon_scheme[amp_index]["RIGHT"] = primer + [primer_name]
+                amplicon_scheme[amp_index]["length"] = amplicon_scheme[amp_index]["RIGHT"][2] - amplicon_scheme[amp_index]["LEFT"][1]
+                # and in all primers
+                all_primers[strand][primer_name] = primer
+    # get remaining dimers in the revised scheme and add pool identifier for reporting
+    primer_dimers = [
+        (amplicon_scheme[primer1[0]]["pool"], primer1, primer2)
+        for primer1, primer2 in test_scheme_for_dimers(amplicon_scheme)
+    ]
 
     return primer_dimers
 
 
-def find_single_amplicons(amplicons, all_primers, n):
+def find_single_amplicons(amplicons, n):
     """
     find non-overlapping amplicons with low penalties
     from all found amplicons. only for the SINGLE mode.
     """
     # sort amplicons
-    sorted_amplicons = sorted(amplicons.items(), key=lambda x: x[1][5])
-    to_retain = [sorted_amplicons[0]]
-    amplicon_range = list(range(sorted_amplicons[0][1][0], sorted_amplicons[0][1][1]+1))
-    amplicon_set = set(amplicon_range)
+    sorted_amplicons = sorted(amplicons, key=lambda x: (x.get("off_targets", False), x["penalty"]))
+    to_retain = []
+    retained_ranges = []
     # find lowest non-overlapping
     for amp in sorted_amplicons:
-        amp_positions = list(range(amp[1][0], amp[1][1]+1))
-        if not any(x in amp_positions for x in amplicon_set):
-            amplicon_set.update(amp_positions)
+        overlaps_retained = False
+        amp_range = range(amp["LEFT"][1], amp["RIGHT"][2])
+        for r in retained_ranges:
+            if amp_range.start < r.stop and r.start < amp_range.stop:
+                overlaps_retained = True
+                break
+        if not overlaps_retained:
+            retained_ranges.append(amp_range)
             to_retain.append(amp)
-    # build the final dictionary
-    scheme_dictionary = {0: {}}
-    counter = 1
-    for amp in to_retain:
-        scheme_dictionary[0][amp[0]] = {}
-        scheme_dictionary[0][amp[0]][amp[1][2]] = all_primers["+"][amp[1][2]]
-        scheme_dictionary[0][amp[0]][amp[1][3]] = all_primers["-"][amp[1][3]]
-        if n != float("inf"):
-            if counter == n:
+            if len(to_retain) == n:
                 break
-            counter += 1
 
-    return scheme_dictionary
+    return to_retain
```

### Comparing `varvamp-1.1.3/varvamp.egg-info/PKG-INFO` & `varvamp-1.2.0/varvamp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 1.1.3
+Version: 1.2.0
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `varvamp-1.1.3/varvamp.egg-info/SOURCES.txt` & `varvamp-1.2.0/varvamp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

