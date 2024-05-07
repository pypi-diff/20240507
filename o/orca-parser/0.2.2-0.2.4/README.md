# Comparing `tmp/orca_parser-0.2.2-py3-none-any.whl.zip` & `tmp/orca_parser-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 12217 bytes, number of entries: 11
+Zip file size: 14002 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat     4935 b- defN 24-May-07 13:30 orca_parser/G16_parse.py
 -rw-rw-rw-  2.0 fat     3404 b- defN 23-Dec-03 12:21 orca_parser/HessianTools.py
--rw-rw-rw-  2.0 fat    21052 b- defN 24-Feb-16 19:03 orca_parser/ORCAParse.py
--rw-rw-rw-  2.0 fat     2016 b- defN 24-Mar-14 17:12 orca_parser/__init__.py
+-rw-rw-rw-  2.0 fat    21365 b- defN 24-May-07 13:36 orca_parser/ORCAParse.py
+-rw-rw-rw-  2.0 fat     2053 b- defN 24-Mar-26 14:26 orca_parser/__init__.py
 -rw-rw-rw-  2.0 fat     1696 b- defN 24-Mar-14 17:34 orca_parser/ams_parse.py
 -rw-rw-rw-  2.0 fat     1553 b- defN 24-Jan-08 20:28 orca_parser/parse_engrad.py
--rw-rw-rw-  2.0 fat      217 b- defN 24-Mar-14 17:36 orca_parser/version.py
--rw-rw-rw-  2.0 fat     1235 b- defN 24-Mar-14 17:37 orca_parser-0.2.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1999 b- defN 24-Mar-14 17:37 orca_parser-0.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-14 17:37 orca_parser-0.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Mar-14 17:37 orca_parser-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      895 b- defN 24-Mar-14 17:37 orca_parser-0.2.2.dist-info/RECORD
-11 files, 34171 bytes uncompressed, 10707 bytes compressed:  68.7%
+-rw-rw-rw-  2.0 fat      217 b- defN 24-May-07 12:07 orca_parser/version.py
+-rw-rw-rw-  2.0 fat     1235 b- defN 24-May-07 13:53 orca_parser-0.2.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1999 b- defN 24-May-07 13:53 orca_parser-0.2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 13:53 orca_parser-0.2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-May-07 13:53 orca_parser-0.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      976 b- defN 24-May-07 13:53 orca_parser-0.2.4.dist-info/RECORD
+12 files, 39537 bytes uncompressed, 12368 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -1,7 +1,10 @@
+Filename: orca_parser/G16_parse.py
+Comment: 
+
 Filename: orca_parser/HessianTools.py
 Comment: 
 
 Filename: orca_parser/ORCAParse.py
 Comment: 
 
 Filename: orca_parser/__init__.py
@@ -12,23 +15,23 @@
 
 Filename: orca_parser/parse_engrad.py
 Comment: 
 
 Filename: orca_parser/version.py
 Comment: 
 
-Filename: orca_parser-0.2.2.dist-info/LICENSE
+Filename: orca_parser-0.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: orca_parser-0.2.2.dist-info/METADATA
+Filename: orca_parser-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: orca_parser-0.2.2.dist-info/WHEEL
+Filename: orca_parser-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: orca_parser-0.2.2.dist-info/top_level.txt
+Filename: orca_parser-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: orca_parser-0.2.2.dist-info/RECORD
+Filename: orca_parser-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orca_parser/ORCAParse.py

```diff
@@ -71,23 +71,22 @@
     return rmsd
 
 
 class ORCAParse:
     @property
     def asemol(self):
         """
-        
-
         Returns
         -------
         ase.Atoms
             An ase molecule with the coordinates of the last conformer in the orca output.
 
         """
         self.parse_coords()
+        #print(len(self.atoms), len(self.coords[-1]))
         return Atoms(self.atoms, self.coords[-1])
     
     def ValidateOutput(self):
         if "TOTAL RUN TIME:" in self.raw:
             self.time = self.raw.split("TOTAL RUN TIME:")[1]
             T = self.time.strip().split()
             self.time  = int(T[0]) * 24 *60 * 60
@@ -148,15 +147,14 @@
             if "Starting D4" in E_disp: #Not a results line
                 continue
             self.dispersions[i] = float(E_disp)
         
     def parse_coords(self):
         self.coords = []
         self.atoms = []
-        self.masses = []
         frames = self.raw.split("CARTESIAN COORDINATES (ANGSTROEM)")[1:]
         for i,frame in enumerate(frames):
             positions = []
             frame = frame.split("CARTESIAN COORDINATES (A.U.)")[0]
             for line in frame.split("\n"):
                 line = line.split()
                 if len(line) != 4:
@@ -290,15 +288,16 @@
                     "BasisSet": self.raw.split("Your calculation utilizes the basis:")[1].split("\n")[0].replace(",", "").rstrip().replace(" ", ""), 
                     "Freq": "VIBRATIONAL FREQUENCIES" in self.raw,
                     "RIJCOSX" : "RIJ-COSX (HFX calculated with COS-X)).... on" in self.raw,
                     "def2J": "Your calculation utilizes the auxiliary basis: def2/J" in self.raw,
                     "Solvation": "Gas",
                     "Charge": self.Z,
                     "Multiplicity": self.Multiplicity,
-                    "version": self.orca_version}
+                    "version": self.orca_version,
+                    "software": "ORCA"}
         
         # Finicky functionals
         if "HF-3C" in inp:
             inp_dict["Functional"] = "HF"
         elif "Exchange Functional    Exchange        .... B88" in self.raw and "Correlation Functional Correlation     .... LYP" in self.raw:
             inp_dict["Functional"] = "B3LYP"
         else:
@@ -341,19 +340,21 @@
             inp_dict["Solvation"] = "CPCM"
             eps = float(self.raw.split("Epsilon                                         ...")[1].split("\n")[0].strip())
             refrac = float(self.raw.split("Refrac                                          ...")[1].split("\n")[0].strip())
             if eps == 80.4 and refrac == 1.33:
                 inp_dict["Solvation"] = "CPCM(WATER)"
             elif eps == 7.25 and refrac == 1.407:
                 inp_dict["Solvation"] = "CPCM(THF)"
+            elif eps == 47.2 and refrac == 1.479:
+                inp_dict["Solvation"] = "CPCM(DMSO)"
+            elif eps == 36.6 and refrac == 1.344:
+                inp_dict["Solvation"] = "CPCM(Acetonitrile)"
             else:
                 print(f"Couldnt assign CPCM solvent from eps = {eps} and refrac = {refrac}")
-            
-            
-            
+
         return inp_dict
 
     def convergence(self):
         self.conv = dict()
         self.tol = dict()
         if "Geometry convergence" not in self.raw:
             return 0
@@ -450,14 +451,17 @@
         if self.raw == "Couldnt decode output file as utf-8 or utf-16":
             print(self.raw)
             self.valid = False
             return None
         self.ValidateOutput()
         self.convergence()
         self.TDDFT = False
+        self.coords = []
+        self.atoms = []
+        self.masses = []
         self.Masses = {'H' : 1.008,'He' : 4.003, 'Li' : 6.941, 'Be' : 9.012,\
                  'B' : 10.811, 'C' : 12.011, 'N' : 14.007, 'O' : 15.999,\
                  'F' : 18.998, 'Ne' : 20.180, 'Na' : 22.990, 'Mg' : 24.305,\
                  'Al' : 26.982, 'Si' : 28.086, 'P' : 30.974, 'S' : 32.066,\
                  'Cl' : 35.453, 'Ar' : 39.948, 'K' : 39.098, 'Ca' : 40.078,\
                  'Sc' : 44.956, 'Ti' : 47.867, 'V' : 50.942, 'Cr' : 51.996,\
                  'Mn' : 54.938, 'Fe' : 55.845, 'Co' : 58.933, 'Ni' : 58.693,\
```

## orca_parser/__init__.py

```diff
@@ -11,14 +11,15 @@
 
 # import submodules
 from .version import __version__
 from orca_parser.ORCAParse import *
 from orca_parser.HessianTools import *
 from orca_parser.parse_engrad import *
 from orca_parser.ams_parse import *
+from orca_parser.G16_parse import *
 
 # 1 Bohr = 0.52917724900001 Angstrom
 
 a="""
 
                                            _ __                                          
  ██████╗ ██████╗  ██████╗ █████╗         ██████╗  █████╗ ██████╗ ███████╗███████╗██████╗
```

## orca_parser/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.2.2'
+__version__ = '0.2.4'
```

## Comparing `orca_parser-0.2.2.dist-info/LICENSE` & `orca_parser-0.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `orca_parser-0.2.2.dist-info/METADATA` & `orca_parser-0.2.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orca-parser
-Version: 0.2.2
+Version: 0.2.4
 Summary: A module for parse ORCA output files including hessians (.hess) files
 Home-page: https://github.com/avanteijlingen/ORCA-Parser
 Author: Alexander van Teijlingen
 Author-email: a.vant@linuxmail.org
 License: BSD 2-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `orca_parser-0.2.2.dist-info/RECORD` & `orca_parser-0.2.4.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+orca_parser/G16_parse.py,sha256=i9bN-F1Kf0kMx3PrXkt1WkccK3PQqHmLMpdS51CQUqw,4935
 orca_parser/HessianTools.py,sha256=CcIV7D9bp3UJgOwgyD5FiljNI_xUuF3vzTqAIDKIw3Q,3404
-orca_parser/ORCAParse.py,sha256=8Jt0yNTC1hE8Avq0o8e3PNviqidDSZet08218uO-wFQ,21052
-orca_parser/__init__.py,sha256=uMUpzbPxsK_LqWTzPE0YWw8-XBxbN1QA-8lzteL-VAA,2016
+orca_parser/ORCAParse.py,sha256=6Gq0J2oNYYCLA-n84_UQKpYvK89elHAgFZ2VoGtSxUQ,21365
+orca_parser/__init__.py,sha256=DXOcbyxd1xwNfXcMWl-lj5RDsXQAwYyWTPuT0ymfOIc,2053
 orca_parser/ams_parse.py,sha256=Msfm7vTiiftgux7YunE9QA0gfZO_NVtZjN7ToaQNU8c,1696
 orca_parser/parse_engrad.py,sha256=-XkCudv1I1-lOZfpUQJawn84L_GxRR-IF6r1uXQLdKU,1553
-orca_parser/version.py,sha256=xEqtBrYpsJcJg2G1ebze2d1-Dy_eOtitTcNaka7jPxs,217
-orca_parser-0.2.2.dist-info/LICENSE,sha256=Q2ptU2E48gOsMzhYz_kqVovmJ5d1KzrblLyqD2_-fvY,1235
-orca_parser-0.2.2.dist-info/METADATA,sha256=MivjwyESwTQnVjlSe8AT8rkKZ1iSdfJIcWUsmFhKBRo,1999
-orca_parser-0.2.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-orca_parser-0.2.2.dist-info/top_level.txt,sha256=8n8h8nQznt6NRgMjI0VijQ6cY5Nu7A0UUuc1M-GHe40,12
-orca_parser-0.2.2.dist-info/RECORD,,
+orca_parser/version.py,sha256=9WP2FmOw0i5p-hz_O_j69qKrdhrrlNVm-Q23cfD2LnA,217
+orca_parser-0.2.4.dist-info/LICENSE,sha256=Q2ptU2E48gOsMzhYz_kqVovmJ5d1KzrblLyqD2_-fvY,1235
+orca_parser-0.2.4.dist-info/METADATA,sha256=MDlDOLLz70X1it3pjyu-y4T3_dxhkc0BwSqLsko6XHM,1999
+orca_parser-0.2.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+orca_parser-0.2.4.dist-info/top_level.txt,sha256=8n8h8nQznt6NRgMjI0VijQ6cY5Nu7A0UUuc1M-GHe40,12
+orca_parser-0.2.4.dist-info/RECORD,,
```

