# Comparing `tmp/way2dssat-0.0.5.tar.gz` & `tmp/way2dssat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "way2dssat-0.0.5.tar", last modified: Mon Apr 29 04:43:14 2024, max compression
+gzip compressed data, was "way2dssat-0.0.6.tar", last modified: Tue May  7 03:27:56 2024, max compression
```

## Comparing `way2dssat-0.0.5.tar` & `way2dssat-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 04:43:14.645462 way2dssat-0.0.5/
--rw-rw-rw-   0        0        0      668 2024-04-29 04:43:14.637894 way2dssat-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       67 2024-04-28 03:48:31.000000 way2dssat-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 04:43:14.574535 way2dssat-0.0.5/Way2DSSAT/
--rw-rw-rw-   0        0        0      803 2024-04-29 04:41:55.000000 way2dssat-0.0.5/Way2DSSAT/__init__.py
--rw-rw-rw-   0        0        0     6858 2024-04-29 04:27:54.000000 way2dssat-0.0.5/Way2DSSAT/gssurgo2soil.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:43:14.637894 way2dssat-0.0.5/Way2DSSAT.egg-info/
--rw-rw-rw-   0        0        0      668 2024-04-29 04:43:14.000000 way2dssat-0.0.5/Way2DSSAT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-29 04:43:14.000000 way2dssat-0.0.5/Way2DSSAT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 04:43:14.000000 way2dssat-0.0.5/Way2DSSAT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-29 04:43:14.000000 way2dssat-0.0.5/Way2DSSAT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-29 04:43:14.000000 way2dssat-0.0.5/Way2DSSAT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      699 2024-04-29 04:42:01.000000 way2dssat-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 04:43:14.645462 way2dssat-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      476 2024-04-28 06:04:18.000000 way2dssat-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:27:56.375572 way2dssat-0.0.6/
+-rw-rw-rw-   0        0        0      667 2024-05-07 03:27:56.375572 way2dssat-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2024-04-28 03:48:31.000000 way2dssat-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 03:27:56.242369 way2dssat-0.0.6/Way2DSSAT/
+-rw-rw-rw-   0        0        0     4264 2024-05-07 03:15:55.000000 way2dssat-0.0.6/Way2DSSAT/WTH.py
+-rw-rw-rw-   0        0        0       93 2024-05-07 03:13:16.000000 way2dssat-0.0.6/Way2DSSAT/__init__.py
+-rw-rw-rw-   0        0        0     8080 2024-05-07 03:16:28.000000 way2dssat-0.0.6/Way2DSSAT/gssurgo2soil.py
+-rw-rw-rw-   0        0        0     6920 2024-05-07 03:05:29.000000 way2dssat-0.0.6/Way2DSSAT/xfiles.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:27:56.375572 way2dssat-0.0.6/Way2DSSAT.egg-info/
+-rw-rw-rw-   0        0        0      667 2024-05-07 03:27:56.000000 way2dssat-0.0.6/Way2DSSAT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-07 03:27:56.000000 way2dssat-0.0.6/Way2DSSAT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 03:27:56.000000 way2dssat-0.0.6/Way2DSSAT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-07 03:27:56.000000 way2dssat-0.0.6/Way2DSSAT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-07 03:27:56.000000 way2dssat-0.0.6/Way2DSSAT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      698 2024-05-07 03:15:53.000000 way2dssat-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 03:27:56.375572 way2dssat-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      481 2024-05-07 03:15:22.000000 way2dssat-0.0.6/setup.py
```

### Comparing `way2dssat-0.0.5/PKG-INFO` & `way2dssat-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Way2DSSAT
-Version: 0.0.5
-Summary: Package to handle input output files
+Version: 0.0.6
+Summary: Package to handle input DSSAT files
 Author: Manavjot Singh
 Author-email: Manavjot <manavjotsingh97@gmail.com>
 Project-URL: Homepage, https://github.com/ManavjotSingh97/Way2DSSAT
 Project-URL: Issues, https://github.com/ManavjotSingh97/Way2DSSAT/issues
 Keywords: python,DSSAT,Input,gSSURGO
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `way2dssat-0.0.5/Way2DSSAT/gssurgo2soil.py` & `way2dssat-0.0.6/Way2DSSAT/gssurgo2soil.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,46 @@
-def SOL(path,path2):
+    """
+    Converts gSSURGO format into DSSAT .SOL format.
+    
+    Inputs
+    ------
+        path: string
+            path to your .csv file containing the data from gSSURGO. Must have the following columns(and other related depths)
+            WC15Bar_DCP_0to5
+            WC3rdbar_DCP_0to5
+            Clay_DCP_0to5
+            Silt_DCP_0to5
+            pHwater_DCP_0to5
+            CEC_DCP_0to5
+            Db3rdbar_DCP_0to5
+            Ksat_DCP_0to5
+            OrgMatter_DCP_0to5
+            MUKEY_DCP_0to5
+        
+           
+            
+    Output
+    ------
+            SG.SOL file in cwd
+            
+            a py dictionary of format:
+                dictionary = {MUKEY :{depth:SH2O}}
+            
+            a list of all the Mukeys
+            
+    Example
+    -------
+            path = 'Username/pathtothecsv'
+            A,B = ssurgo2soil(path)
+        
+   
+          
+    """
+
+def SOL(path):
     
     import pandas
     import math
     """
     Converts gSSURGO format into DSSAT .SOL format.
     
     Inputs
@@ -19,24 +57,35 @@
             Ksat_DCP_0to5
             OrgMatter_DCP_0to5
             MUKEY_DCP_0to5
         
         path2: string
             path where u want to save files
             
-    Example 
+            
+    Output
+    ------
+            SG.SOL file in cwd
+            
+            a py dictionary of format:
+                dictionary = {MUKEY :{depth:SH2O}}
+            
+            a list of all the Mukeys
+            
+    Example
     -------
             path = 'Username/pathtothecsv'
-            path2 = 'Username/pathtosavingfolder'
-            ssurgo2soil(path,path2)
-            
+            A,B = ssurgo2soil(path)
+        
+   
+          
     """
     #Reading csv  
     
-    df_soil=pandas.read_csv(path)
+    df_soil = pandas.read_csv(path)
     #Returns list of columns not required with specific keyword
     # data from ssurgo contains columns suchas pct_Silt** which aren't required
     # Removing those columns form the dataframe
     # These have column name are duplicate of the required soil properties with additional pct in 
     # the name. Thus posing difficulty in calling the column name with keyword
     columns_not_req = list(df_soil.columns.array[list(df_soil.columns.str.contains('pct'))])
 
@@ -53,16 +102,17 @@
     SLSI_columns = list(df.columns.array[list(df.columns.str.contains('Silt'))])
     SLHW_columns = list(df.columns.array[list(df.columns.str.contains('pHwater'))])
     SCEC_columns = list(df.columns.array[list(df.columns.str.contains('CEC'))])
     SBDM_columns = list(df.columns.array[list(df.columns.str.contains('Db3rdbar'))])
     SSKS_columns = list(df.columns.array[list(df.columns.str.contains('Ksat_'))])
     SLOC_columns = list(df.columns.array[list(df.columns.str.contains('OrgMatter'))])
     Mukey_columns = list(df.columns.array[list(df.columns.str.contains('MUKEY'))])
-    # CODING LINES IN THE FILE AS PER SYNTAX OF .SOL FILE
     
+    # CODING LINES IN .SOL FILE FORMAT
+    Mukey=0
     line1 = "*Soils: Created by py2Sol library\n"
     line2="\n"
     #CL is the texture which needed to be specified later in the soil profile
     #200 is the maximum depth of soil
     # seriesname can have spaces upto this length "but ca"
     
     line4='@SITE        COUNTRY          LAT     LONG SCS FAMILY\n'  
@@ -107,21 +157,26 @@
     # SLHB     pH in buffer                                                         
     # SCEC     Cation exchange capacity, cmol kg-1                                 
     # SADC     Anion adsorption coefficient (reduced nitrate flow), cm3 
     # Writing lines to the text documents
 
     #Initialize empty string
     Soil=''
+     
+    SH20 = {}
+    soil_for_X={}
+    MU_key=[]
 
     for j in range(0,len(df)):
         Mukey = df[Mukey_columns].loc[j,Mukey_columns[0]]
+        MU_key.append(Mukey)
         # Appending teh empty string
         Soil+=line1
         Soil+=line2
-        Soil+=f'*IIE{Mukey:>7}  SSURGO      CL         200 seriesname can have spaces upto this length but ca\n'
+        Soil+=f'*GSS{Mukey:07}  SSURGO      CL         200 seriesname can have spaces upto this length but ca\n'
         Soil+=line4
         Soil+=line5
         Soil+=line6
         Soil+=line7
         Soil+=line8
 
         #adding the data to the file 
@@ -143,12 +198,14 @@
             SSAT= round(0.3332 + (-0.000725)*(SLSI)+0.12768*math.log10(SLCL) , 3) #from DSSAT mannual
             SLHW=round(df[SLHW_columns].loc[j,SLHW_columns[i]],3)
             SCEC=round(df[SCEC_columns].loc[j,SCEC_columns[i]],3)
             SBDM= round(df[SBDM_columns].loc[j,SBDM_columns[i]],3)
             SSKS=round(df[SSKS_columns].loc[j,SSKS_columns[i]]*0.36,2) #from micrometer /second to cm /hour
             SLOC=round(df[SLOC_columns].loc[j,SLOC_columns[i]],3)
             Soil+= f'{SLB:>6}{SLMH:>6}{SLLL:>6}{SDUL:>6}{SSAT:>6}{SRGF:>6}{SSKS:>6}{SBDM:>6}{SLOC:>6}{SLCL:>6}{SLSI:>6}{SLCF:>6}{SLNI:>6}{SLHW:>6}{SLHB:>6}{SCEC:>6}{SADC:>6}\n'
-        Soil+='\n'     
+            SH20[SLB] = SDUL
+        Soil+='\n'
+        soil_for_X[f'GSS{Mukey}']=SH20
     # Write to a .SOL file
-    destination=path2
-    with open(f'{destination}SG.SOL', 'w') as file:
-        file.write(Soil)
+    with open(f'SG.SOL', 'w') as file:
+        file.write(Soil)
+    return soil_for_X,MU_key
```

### Comparing `way2dssat-0.0.5/Way2DSSAT.egg-info/PKG-INFO` & `way2dssat-0.0.6/Way2DSSAT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Way2DSSAT
-Version: 0.0.5
-Summary: Package to handle input output files
+Version: 0.0.6
+Summary: Package to handle input DSSAT files
 Author: Manavjot Singh
 Author-email: Manavjot <manavjotsingh97@gmail.com>
 Project-URL: Homepage, https://github.com/ManavjotSingh97/Way2DSSAT
 Project-URL: Issues, https://github.com/ManavjotSingh97/Way2DSSAT/issues
 Keywords: python,DSSAT,Input,gSSURGO
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `way2dssat-0.0.5/pyproject.toml` & `way2dssat-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0","pandas"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = [ "pandas"]
 name = "Way2DSSAT"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Manavjot", email="manavjotsingh97@gmail.com" },
 ]
-description = "Package to handle input output files"
+description = "Package to handle input DSSAT files"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

