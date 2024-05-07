# Comparing `tmp/alphascreen-1.8.tar.gz` & `tmp/alphascreen-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alphascreen-1.8.tar", last modified: Sun Oct 30 11:45:11 2022, max compression
+gzip compressed data, was "dist/alphascreen-1.9.tar", last modified: Mon Oct 31 21:05:34 2022, max compression
```

## Comparing `alphascreen-1.8.tar` & `alphascreen-1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 sami      (1000) sami      (1000)        0 2022-10-30 11:45:11.000000 alphascreen-1.8/
-drwxrwxrwx   0 sami      (1000) sami      (1000)        0 2022-10-30 11:45:11.000000 alphascreen-1.8/alphascreen/
--rwxrwxrwx   0 sami      (1000) sami      (1000)    19331 2022-10-30 09:49:50.000000 alphascreen-1.8/alphascreen/analyze.py
--rwxrwxrwx   0 sami      (1000) sami      (1000)     6116 2022-10-30 10:28:17.000000 alphascreen-1.8/alphascreen/argparser.py
--rwxrwxrwx   0 sami      (1000) sami      (1000)     6346 2022-10-30 10:48:19.000000 alphascreen-1.8/alphascreen/decisiontree.py
--rwxrwxrwx   0 sami      (1000) sami      (1000)    12555 2022-10-30 10:52:57.000000 alphascreen-1.8/alphascreen/jobsetup.py
--rwxrwxrwx   0 sami      (1000) sami      (1000)       84 2022-10-30 11:44:32.000000 alphascreen-1.8/alphascreen/__init__.py
--rwxrwxrwx   0 sami      (1000) sami      (1000)      128 2022-09-18 14:19:09.000000 alphascreen-1.8/alphascreen/__main__.py
-drwxrwxrwx   0 sami      (1000) sami      (1000)        0 2022-10-30 11:45:11.000000 alphascreen-1.8/alphascreen.egg-info/
--rwxrwxrwx   0 sami      (1000) sami      (1000)        1 2022-10-30 11:45:09.000000 alphascreen-1.8/alphascreen.egg-info/dependency_links.txt
--rwxrwxrwx   0 sami      (1000) sami      (1000)       59 2022-10-30 11:45:09.000000 alphascreen-1.8/alphascreen.egg-info/entry_points.txt
--rwxrwxrwx   0 sami      (1000) sami      (1000)      308 2022-10-30 11:45:09.000000 alphascreen-1.8/alphascreen.egg-info/PKG-INFO
--rwxrwxrwx   0 sami      (1000) sami      (1000)       58 2022-10-30 11:45:09.000000 alphascreen-1.8/alphascreen.egg-info/requires.txt
--rwxrwxrwx   0 sami      (1000) sami      (1000)      378 2022-10-30 11:45:09.000000 alphascreen-1.8/alphascreen.egg-info/SOURCES.txt
--rwxrwxrwx   0 sami      (1000) sami      (1000)       12 2022-10-30 11:45:09.000000 alphascreen-1.8/alphascreen.egg-info/top_level.txt
--rwxrwxrwx   0 sami      (1000) sami      (1000)      308 2022-10-30 11:45:11.000000 alphascreen-1.8/PKG-INFO
--rwxrwxrwx   0 sami      (1000) sami      (1000)     9215 2022-10-30 10:58:21.000000 alphascreen-1.8/README.md
--rwxrwxrwx   0 sami      (1000) sami      (1000)       38 2022-10-30 11:45:11.000000 alphascreen-1.8/setup.cfg
--rwxrwxrwx   0 sami      (1000) sami      (1000)      964 2022-09-18 14:19:09.000000 alphascreen-1.8/setup.py
+drwxrwxrwx   0 sami      (1000) sami      (1000)        0 2022-10-31 21:05:34.000000 alphascreen-1.9/
+drwxrwxrwx   0 sami      (1000) sami      (1000)        0 2022-10-31 21:05:34.000000 alphascreen-1.9/alphascreen/
+-rwxrwxrwx   0 sami      (1000) sami      (1000)    19262 2022-10-31 20:38:00.000000 alphascreen-1.9/alphascreen/analyze.py
+-rwxrwxrwx   0 sami      (1000) sami      (1000)     6190 2022-10-31 21:04:47.000000 alphascreen-1.9/alphascreen/argparser.py
+-rwxrwxrwx   0 sami      (1000) sami      (1000)     6346 2022-10-30 10:48:19.000000 alphascreen-1.9/alphascreen/decisiontree.py
+-rwxrwxrwx   0 sami      (1000) sami      (1000)    12876 2022-10-31 21:02:44.000000 alphascreen-1.9/alphascreen/jobsetup.py
+-rwxrwxrwx   0 sami      (1000) sami      (1000)       84 2022-10-31 21:03:32.000000 alphascreen-1.9/alphascreen/__init__.py
+-rwxrwxrwx   0 sami      (1000) sami      (1000)      128 2022-09-18 14:19:09.000000 alphascreen-1.9/alphascreen/__main__.py
+drwxrwxrwx   0 sami      (1000) sami      (1000)        0 2022-10-31 21:05:34.000000 alphascreen-1.9/alphascreen.egg-info/
+-rwxrwxrwx   0 sami      (1000) sami      (1000)        1 2022-10-31 21:05:30.000000 alphascreen-1.9/alphascreen.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sami      (1000) sami      (1000)       59 2022-10-31 21:05:30.000000 alphascreen-1.9/alphascreen.egg-info/entry_points.txt
+-rwxrwxrwx   0 sami      (1000) sami      (1000)      308 2022-10-31 21:05:30.000000 alphascreen-1.9/alphascreen.egg-info/PKG-INFO
+-rwxrwxrwx   0 sami      (1000) sami      (1000)       58 2022-10-31 21:05:30.000000 alphascreen-1.9/alphascreen.egg-info/requires.txt
+-rwxrwxrwx   0 sami      (1000) sami      (1000)      378 2022-10-31 21:05:30.000000 alphascreen-1.9/alphascreen.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sami      (1000) sami      (1000)       12 2022-10-31 21:05:30.000000 alphascreen-1.9/alphascreen.egg-info/top_level.txt
+-rwxrwxrwx   0 sami      (1000) sami      (1000)      308 2022-10-31 21:05:34.000000 alphascreen-1.9/PKG-INFO
+-rwxrwxrwx   0 sami      (1000) sami      (1000)     9311 2022-10-31 21:04:32.000000 alphascreen-1.9/README.md
+-rwxrwxrwx   0 sami      (1000) sami      (1000)       38 2022-10-31 21:05:34.000000 alphascreen-1.9/setup.cfg
+-rwxrwxrwx   0 sami      (1000) sami      (1000)      964 2022-09-18 14:19:09.000000 alphascreen-1.9/setup.py
```

### Comparing `alphascreen-1.8/alphascreen/analyze.py` & `alphascreen-1.9/alphascreen/analyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,35 +358,35 @@
 #     #view.addLabel(nameprotB,{'fontOpacity':1, 'fontSize':12, 'fontColor':'black','backgroundOpacity':0.2, 'backgroundColor':'magenta'},{'resi':lenprotA+10})
 
 #     view.zoomTo()
 #     return view
 
 def write_top(df, threshold, rankby):
     
+    print("\n>> Writing " + excelname + " and " + csvname)
+
     if threshold == 0:
         basename = "Results"
     else:
         basename = "Results-"+rankby+"-above-" + str(threshold).replace(".", "p")
         
     excelname = basename + ".xlsx"
     csvname = basename + ".csv"
     
     with pd.ExcelWriter(excelname) as writer:  
         df[df[rankby]>threshold].to_excel(writer)
         
     df.to_csv(csvname)
-    
-    print("\n>> Wrote " + excelname + " and " + csvname)
         
         
 def write_modelpngs(df, threshold, rankby, overwrite=False):
 
     print("\n>> Writing model snapshots...")
 
-    pymol.finish_launching(['pymol', '-qc']) #-Q will suppress render outputs too
+    pymol.finish_launching(['pymol', '-qc']) #-Q will suppress render outputs too if you want
 
     total=0
 
     for i,result in df[df[rankby]>threshold].iterrows():
         
         model=result["Model"]
         png1 = model[:-4]+".png"
@@ -423,16 +423,14 @@
 
         waitfor(png2)
 
         cmd.delete("current")
         
         total+=1
         
-    #print("\n>> Wrote png-snapshots for " + str(total) + " pdbs.")
-        
 def waitfor(filename):
     pngexists=False
     tic = time.perf_counter()
     while not pngexists:
         if os.path.exists(filename):
             pngexists=True
         time.sleep(0.25)
```

### Comparing `alphascreen-1.8/alphascreen/argparser.py` & `alphascreen-1.9/alphascreen/argparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     jobsetup_opts.add_option("--dimerize_all",
         action="store_true", dest="dimerize_all", default=False,
         help="Dimerize all proteins.")
 
     jobsetup_opts.add_option("--dimerize_all_except",
         action="store", dest="dimerize_except", type="string", default="", metavar='ids-not-to-dimerize',
-        help="Provide a text file (.txt) with a single column list of uniprot IDs to NOT dimerize. Everything else will be dimerized.")
+        help="Dimerize all proteins except the uniprot ID provided here. Alternatively, provide a text file (.txt) with a single column list of uniprot IDs to NOT dimerize. Everything else will be dimerized.")
 
     jobsetup_opts.add_option("--consider",
         action="store", dest="consider", type="string", default="", metavar='sequence-to-consider',
         help="Uniprot ID and sequence range to consider. Example: \"Q86VS8/1/200\" only considers amino acids 1-200 for uniprot ID Q86VS8. Alternatively, provide a text file with a single column list of sequences to consider with a similar syntax (id/start/end).")
 
     jobsetup_opts.add_option("--alphafold_exec",
         action="store", dest="alphafold_exec", type="string", default="colabfold2", metavar='executable',
```

### Comparing `alphascreen-1.8/alphascreen/decisiontree.py` & `alphascreen-1.9/alphascreen/decisiontree.py`

 * *Files identical despite different names*

### Comparing `alphascreen-1.8/alphascreen/jobsetup.py` & `alphascreen-1.9/alphascreen/jobsetup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         table = pd.read_table(file, usecols=[columnA, columnB])
     elif filetype == "excel":
         table = pd.read_excel(file, usecols=[columnA, columnB])
     
     Ainteractors = table[columnA].tolist()
     Binteractors = table[columnB].tolist()
 
+    Ainteractors = [s.strip() for s in Ainteractors]
+    Binteractors = [s.strip() for s in Binteractors]
+
     if focus != "":
         if focus not in Ainteractors or focus not in Binteractors:
             sys.exit("!! Error: the uniprot ID " + focus + " to focus on was not found.\n")
         Ainteractors_fixed = []
         Binteractors_fixed = []
         for A, B in zip(Ainteractors,Binteractors):
             if B == focus:
@@ -56,17 +59,21 @@
     dimerizelst = []
     dontdimerizelst = []
 
     if dimerize_all:
         print(">> Dimerizing all proteins...\n")
 
     elif dimerize_except:
-        print(">> Dimerizing all proteins except those in " + dimerize_except + "...\n")
-        with open(dimerize_except) as f:
-            dontdimerizelst=[line.strip() for line in f.readlines()]
+        if dimerize_except[-4:] == ".txt":
+            print(">> Dimerizing all proteins except those in " + dimerize_except + "...\n")
+            with open(dimerize_except) as f:
+                dontdimerizelst=[line.strip() for line in f.readlines()]
+        else:
+            dontdimerzelst = [dimerize_except]
+            print(">> Dimerizing all proteins except " + dimerize_except + "...\n")
 
     elif dimerize != "":
         if dimerize[-4:] == ".txt":
             print(">> Dimerizing uniprot IDs in " + dimerize + "...\n")
             with open(dimerize) as f:
                 dimerizelst=[line.strip() for line in f.readlines()]
         else:
@@ -106,15 +113,15 @@
 
     print(">> Getting sequences...\n")
 
     Unis_found = []
     Names_found = []
     Seqs_found = []
 
-    notconsidered = consideruniprot #fully populated and will be removed one by one to check that all were found
+    notconsidered = consideruniprot.copy() #fully populated and will be removed one by one to check that all were found
     for A, B in zip(Ainteractors, Binteractors):
 
         try:
             if A in Unis_found:
                 Aindex = Unis_found.index(A)
                 Aname = Names_found[Aindex]
                 Aseq = Seqs_found[Aindex]
```

### Comparing `alphascreen-1.8/README.md` & `alphascreen-1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -99,17 +99,17 @@
 
 Uniprot ID to dimerize. Alternatively, provide a text file (.txt) with a single column list of uniprot IDs to dimerize.
 
 **```--dimerize_all```**
 
 Dimerize all proteins. You may have to reduce the fragment length if the total sequence length becomes too big.
 
-**```--dimerize_all_except```** *```uniprot-ids.txt```*
+**```--dimerize_all_except```** *```uniprot-id```* or *```uniprot-ids.txt```*
 
-Provide a text file (.txt) with a single column list of uniprot IDs to NOT dimerize. Everything else will be dimerized.
+Dimerize all proteins except the uniprot ID provided here. Alternatively, provide a text file (.txt) with a single column list of uniprot IDs to NOT dimerize. Everything else will be dimerized.
 
 **```--consider```** *```uniprot/start/end```* or *```consider.txt```*
 
 Uniprot ID and sequence range to consider. Example: *Q86VS8/1/200* only considers amino acids 1-200 for uniprot ID Q86VS8. Alternatively, provide a text file with a single column list of sequences to consider with a similar syntax (*id/start/end*).
 
 **```--alphafold_exec```** *```alphafold-executable```*
```

### Comparing `alphascreen-1.8/setup.py` & `alphascreen-1.9/setup.py`

 * *Files identical despite different names*

