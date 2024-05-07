# Comparing `tmp/quantylf-0.0.6.tar.gz` & `tmp/quantylf-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantylf-0.0.6.tar", last modified: Sun May  5 05:54:12 2024, max compression
+gzip compressed data, was "quantylf-0.0.7.tar", last modified: Tue May  7 16:13:47 2024, max compression
```

## Comparing `quantylf-0.0.6.tar` & `quantylf-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:54:12.411840 quantylf-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-05 05:54:08.000000 quantylf-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-05 05:54:08.000000 quantylf-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-05 05:54:12.411840 quantylf-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-05 05:54:08.000000 quantylf-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-05 05:54:08.000000 quantylf-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-05 05:54:12.411840 quantylf-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:54:12.407839 quantylf-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:54:12.407839 quantylf-0.0.6/src/QuantyLF/
--rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-05-05 05:54:08.000000 quantylf-0.0.6/src/QuantyLF/QuantyLF.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 05:54:08.000000 quantylf-0.0.6/src/QuantyLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:54:12.407839 quantylf-0.0.6/src/QuantyLF/cases/
--rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-05-05 05:54:08.000000 quantylf-0.0.6/src/QuantyLF/cases/Td_3d.lua
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 05:54:08.000000 quantylf-0.0.6/src/QuantyLF/cases/Td_3d.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 05:54:12.407839 quantylf-0.0.6/src/QuantyLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-05 05:54:12.000000 quantylf-0.0.6/src/QuantyLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-05 05:54:12.000000 quantylf-0.0.6/src/QuantyLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 05:54:12.000000 quantylf-0.0.6/src/QuantyLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 05:54:12.000000 quantylf-0.0.6/src/QuantyLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 05:54:12.000000 quantylf-0.0.6/src/QuantyLF.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:47.296063 quantylf-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 16:13:43.000000 quantylf-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 16:13:43.000000 quantylf-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 16:13:47.296063 quantylf-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 16:13:43.000000 quantylf-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 16:13:43.000000 quantylf-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-07 16:13:47.296063 quantylf-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:47.292063 quantylf-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:47.292063 quantylf-0.0.7/src/QuantyLF/
+-rw-r--r--   0 runner    (1001) docker     (127)    18673 2024-05-07 16:13:43.000000 quantylf-0.0.7/src/QuantyLF/QuantyLF.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:43.000000 quantylf-0.0.7/src/QuantyLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:47.296063 quantylf-0.0.7/src/QuantyLF/cases/
+-rw-r--r--   0 runner    (1001) docker     (127)    18821 2024-05-07 16:13:43.000000 quantylf-0.0.7/src/QuantyLF/cases/Td_3d.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-07 16:13:43.000000 quantylf-0.0.7/src/QuantyLF/cases/Td_3d.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:47.296063 quantylf-0.0.7/src/QuantyLF/cases/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-07 16:13:43.000000 quantylf-0.0.7/src/QuantyLF/cases/utils/slater_integrals.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:13:47.296063 quantylf-0.0.7/src/QuantyLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 16:13:47.000000 quantylf-0.0.7/src/QuantyLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-07 16:13:47.000000 quantylf-0.0.7/src/QuantyLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:13:47.000000 quantylf-0.0.7/src/QuantyLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 16:13:47.000000 quantylf-0.0.7/src/QuantyLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 16:13:47.000000 quantylf-0.0.7/src/QuantyLF.egg-info/top_level.txt
```

### Comparing `quantylf-0.0.6/LICENSE` & `quantylf-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `quantylf-0.0.6/PKG-INFO` & `quantylf-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantyLF
-Version: 0.0.6
+Version: 0.0.7
 Summary: QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quantylf-0.0.6/setup.cfg` & `quantylf-0.0.7/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = QuantyLF
-version = 0.0.6
+version = 0.0.7
 author = Carl Magnus Meier
 author_email = magnus.meier@outook.de
 description = QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CMM02/XPlotLib
 classifiers =
```

### Comparing `quantylf-0.0.6/src/QuantyLF/QuantyLF.py` & `quantylf-0.0.7/src/QuantyLF/QuantyLF.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,19 +469,21 @@
 
 
     """
     Set the path to the Quanty executable
 
     ----------------
     Parameters:
-    platform: Platform for which the path is being set
     command: Path to the Quanty executable
+    platform: Platform for which the path is being set, if not set the current platform is used
     """
-    def set_quanty_command(self, command, platform='default'):
-        self.quanty_command[platform] = command
+    def set_quanty_command(self, command, for_platform=None):
+        if for_platform is None:
+            for_platform = platform.system()
+        self.quanty_command[for_platform] = command
 
 
     """
     Set custom path to the parameter file (default: ParVals.txt)
 
     ----------------
     Parameters:
```

### Comparing `quantylf-0.0.6/src/QuantyLF/cases/Td_3d.lua` & `quantylf-0.0.7/src/QuantyLF/cases/Td_3d.lua`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+-- import slater integral values
+require "src.QuantyLF.cases.utils.slater_integrals"
+
 TimeStart("LF_RIXS")
 -- this example calculates the resonant inelastic x-ray scattering in Transition Metal 3d we look at the
 -- L-L23M45 edge, i.e. we make an excitation from 2p to 3d (L23) and decay from the
 -- 3d shell back to the 2p shell (final "hole" in the 3d shell M45 edge). These spectra
 -- measure d-d excitations and or magnons.
 
 -- As magnons are not localised the final state will be dispersive. Both the energy as
@@ -12,238 +15,160 @@
 -- large enough clusters in a full many-body calculation to capture dispersion....
 
 -- We here take a route where we define an effective low energy operator that only allows
 -- to make magnetic excitations, but has the same resonant energy and polarisation dependence
 -- as the RIXS scattering. We then can use this effective operator to calculate the dispersive
 -- magnons using linear spin-wave theory. (Or any other level of theory you want)
 -- The local moment is alligned in the cluster due to an exchange field
-Hex        = 0--6*0.084--0.027
-HexDir     = {1,1,1}
+Hex = 0 -- 6*0.084--0.027
+HexDir = {1, 1, 1}
 
 -- We calculate the resonant energy dependence in the following window.
-Emin1  = -10
-Emax1  =  20
-NE1    = 120
+Emin1 = -10
+Emax1 = 20
+NE1 = 120
 Gamma1 = 1.0
 
 ----------------------------------------------------------------------------
 ----------- some functions used
 ----------------------------------------------------------------------------
 -- calculates x^2
 function sqr(x)
-  return (x*x)
+    return (x * x)
 end
 
---Read in parameters from ParVals file
+-- Read in parameters from ParVals file
 function ReadParameters()
 
-  local pars = {}
-  local NSites = 0
+    local pars = {}
+    local NSites = 0
 
-  local citylist = {}
-  for line in io.lines("ParVals.txt") do
+    local citylist = {}
+    for line in io.lines("ParVals.txt") do
 
-      local iter = string.gmatch(line, "[^%s]+")
-      local name = iter()
-      local val = 0
-      if name == "RIXS_Broad" or name == "XAS_Broad" then
-        val = {tonumber(iter()), tonumber(iter())}
-      else
-        val = tonumber(iter())
-      end
-      pars[#pars + 1] = { name = name, val = val }
-  end
-  print(pars)
+        local iter = string.gmatch(line, "[^%s]+")
+        local name = iter()
+        local val = 0
+        if name == "RIXS_Broad" or name == "XAS_Broad" then
+            val = {tonumber(iter()), tonumber(iter())}
+        else
+            val = tonumber(iter())
+        end
+        pars[#pars + 1] = {
+            name = name,
+            val = val
+        }
+    end
+    print(pars)
 
-  return pars --table of values, indexed by name
+    return pars -- table of values, indexed by name
 end
 
 pars = ReadParameters()
 
-NF=26;
-NB=0;
-IndexUp_2p={0,2,4};
-IndexDn_2p={1,3,5};
-IndexUp_3d={6,8,10,12,14};
-IndexDn_3d={7,9,11,13,15};
-IndexUp_Ld={16,18,20,22,24}
-IndexDn_Ld={17,19,21,23,25}
+NF = 26;
+NB = 0;
+IndexUp_2p = {0, 2, 4};
+IndexDn_2p = {1, 3, 5};
+IndexUp_3d = {6, 8, 10, 12, 14};
+IndexDn_3d = {7, 9, 11, 13, 15};
+IndexUp_Ld = {16, 18, 20, 22, 24}
+IndexDn_Ld = {17, 19, 21, 23, 25}
 
 -- Setup the ion and formal valence
 -- Setup the ion and formal valence
 ion = 0
 oxy = 0
 
-for i=1,#pars do
-  if(pars[i].name == "oxy") then oxy = pars[i].val end
-  if(pars[i].name == "ion") then ion = pars[i].val end
-end
-
--- Slater integral values
-
-if ion==29 then
-  if oxy == 1 then nd = 10
-    elseif oxy == 2 then nd = 9 
-      elseif oxy == 3 then nd = 8 
-        elseif oxy == 4 then nd = 7 end
-zeta_3d=0.102  ; F2dd=12.854 ; F4dd=7.980                  --- initial state parameters
-zeta_2p=13.498 ; F2pd=8.177  ; G1pd=6.169 ; G3pd=3.510     ---  final  state parameters
-Xzeta_3d=0.124  ; XF2dd=13.611 ; XF4dd=8.457               ---  final  state parameters
-
-elseif ion==28 then
-  if oxy == 2 then nd = 8
-    elseif oxy == 3 then nd = 7 
-      elseif oxy == 4 then nd = 6 end
-zeta_3d=0.083  ; F2dd=12.233 ; F4dd=7.597
-zeta_2p=11.507 ; F2pd=7.720  ; G1pd=5.783 ; G3pd=3.290
-Xzeta_3d=0.102  ; XF2dd=13.005 ; XF4dd=8.084
-
-elseif ion==27 then
-   if oxy == 2 then nd = 7
-     elseif oxy == 3 then nd = 6 
-       elseif oxy == 4 then nd = 5 end
-zeta_3d=0.066  ; F2dd=11.604 ; F4dd=7.209
-zeta_2p=9.748 ; F2pd=7.259  ; G1pd=5.394 ; G3pd=3.068
-Xzeta_3d=0.083  ; XF2dd=12.395 ; XF4dd=7.707
-
-elseif ion==26 then
-  if oxy == 2 then nd = 6
-    zeta_3d=0.052  ; F2dd=10.965 ; F4dd=6.815
-zeta_2p=8.200 ; F2pd=6.792  ; G1pd=5.0 ; G3pd=2.843
-Xzeta_3d=0.067  ; XF2dd=11.778 ; XF4dd=7.327
-    elseif oxy == 3 then nd = 5 
-      zeta_3d= 0.059 ; F2dd= 12.043 ; F4dd=7.535
-zeta_2p= 8.199; F2pd=7.446  ; G1pd=5.566 ; G3pd=3.166
-Xzeta_3d= 0.074 ; XF2dd= 12.818; XF4dd=8.023
-      elseif oxy == 4 then nd = 4 end
-
-
-elseif ion==25 then
-    if oxy == 2 then nd = 5
-    zeta_3d=0.040  ; F2dd=10.315 ; F4dd=6.413
-    zeta_2p=6.846 ; F2pd=6.320  ; G1pd=4.603 ; G3pd=2.617
-    Xzeta_3d=0.053  ; XF2dd=11.154 ; XF4dd=6.942
-    elseif oxy == 3 then nd = 4 
-      zeta_3d=0.046 ; F2dd= 11.415 ; F4dd=7.148 ;
-        zeta_2p=6.845 ; F2pd=6.988  ; G1pd=5.179 ; G3pd=2.945 ; 
-        Xzeta_3d=0.059  ; XF2dd=12.210 ; XF4dd=7.649
-        elseif oxy == 4 then nd = 3
-        zeta_3d=0.052 ; F2dd=12.416 ; F4dd=7.820 ;
-          zeta_2p=6.845; F2pd=7.658  ; G1pd=5.776; G3pd=3.288
-          Xzeta_3d=0.066  ; XF2dd=13.177 ; XF4dd=8.299 ;
-                   elseif oxy == 7 then nd = 2 end
-                   
-elseif ion==24 then
-  if oxy == 2 then nd = 4
-  	zeta_3d=0.030  ; F2dd=9.469 ; F4dd=6.002
-	zeta_2p=5.668 ; F2pd=5.841  ; G1pd=4.204 ; G3pd=2.388
-	Xzeta_3d=0.041  ; XF2dd=10.521 ; XF4dd=6.522
-    elseif oxy == 3 then nd = 3 
-    	zeta_3d=0.035  ; F2dd=10.777 ; F4dd=6.755
-		zeta_2p=5.667 ; F2pd=6.526  ; G1pd=4.788 ; G3pd=2.722
-		Xzeta_3d=0.047 ; XF2dd=11.596 ; XF4dd=7.270
-      elseif oxy == 4 then nd = 2 end
-
-elseif ion==23 then
-  if oxy == 2 then nd = 3
-    elseif oxy == 3 then nd = 2 
-      elseif oxy == 4 then nd = 1 end
-zeta_3d=0.022  ; F2dd=8.961 ; F4dd=5.576
-zeta_2p=4.650 ; F2pd=5.351  ; G1pd=3.792 ; G3pd=2.154
-Xzeta_3d=0.031  ; XF2dd=9.875 ; XF4dd=6.152
-
-elseif ion==22 then
-if oxy == 2 then nd = 2
-    elseif oxy == 3 then nd = 1 
-      elseif oxy == 4 then nd = 0 end
-zeta_3d=0.016  ; F2dd=8.243 ; F4dd=5.132
-zeta_2p=3.776 ; F2pd=4.849  ; G1pd=3.376 ; G3pd=1.917
-Xzeta_3d=0.023  ; XF2dd=9.213 ; XF4dd=5.744
-
-
-elseif ion==21 then
-  if oxy == 2 then nd = 1
-    elseif oxy == 3 then nd = 2 end
-zeta_3d=0.010  ; F2dd=0 ; F4dd=0
-zeta_2p=3.032 ; F2pd=4.332  ; G1pd=2.950 ; G3pd=1.674
-Xzeta_3d=0.017  ; XF2dd=8.530 ; XF4dd=5.321
-
-else 
-print("Could not recognize the ion name...")
-os.exit()
+for i = 1, #pars do
+    if (pars[i].name == "oxy") then
+        oxy = pars[i].val
+    end
+    if (pars[i].name == "ion") then
+        ion = pars[i].val
+    end
 end
 
+-- Configure slater integrals
+nd, zeta_3d, F2dd, F4dd, zeta_2p, F2pd, G1pd, G3pd, Xzeta_3d, XF2dd, XF4dd = get_slater_integrals(ion, oxy)
+
 -- Setup the hybridization
 Va1g = 0
 Veg = 0
 
---setup initial parameters for fitting values to initialize variables
+-- setup initial parameters for fitting values to initialize variables
 tenDq = 1
 tenDqFs = 0
 VfScale = 1
 
 ----overwrite init variables with ParVals values
-for i=1,#pars do
-  if(pars[i].name == "tenDq") then tenDq = pars[i].val end
-  if(pars[i].name == "tenDqF") then tenDqFs = pars[i].val end
-  if(pars[i].name == "VfScale") then VfScale = pars[i].val end
+for i = 1, #pars do
+    if (pars[i].name == "tenDq") then
+        tenDq = pars[i].val
+    end
+    if (pars[i].name == "tenDqF") then
+        tenDqFs = pars[i].val
+    end
+    if (pars[i].name == "VfScale") then
+        VfScale = pars[i].val
+    end
 end
 tenDqF = tenDqFs * tenDq
 
-Va1g = -0.6*tenDq 
-Veg =  0.4*tenDq
+Va1g = -0.6 * tenDq
+Veg = 0.4 * tenDq
 
-Va1gF = Va1g*VfScale
-VegF = Veg*VfScale
+Va1gF = Va1g * VfScale
+VegF = Veg * VfScale
 
-OppSx_3d   =NewOperator("Sx"   ,NF,IndexUp_3d,IndexDn_3d);
-OppSy_3d   =NewOperator("Sy"   ,NF,IndexUp_3d,IndexDn_3d);
-OppSz_3d   =NewOperator("Sz"   ,NF,IndexUp_3d,IndexDn_3d);
-OppSsqr_3d =NewOperator("Ssqr" ,NF,IndexUp_3d,IndexDn_3d);
-OppSplus_3d=NewOperator("Splus",NF,IndexUp_3d,IndexDn_3d);
-OppSmin_3d =NewOperator("Smin" ,NF,IndexUp_3d,IndexDn_3d);
-
-OppLx_3d   =NewOperator("Lx"   ,NF,IndexUp_3d,IndexDn_3d);
-OppLy_3d   =NewOperator("Ly"   ,NF,IndexUp_3d,IndexDn_3d);
-OppLz_3d   =NewOperator("Lz"   ,NF,IndexUp_3d,IndexDn_3d);
-OppLsqr_3d =NewOperator("Lsqr" ,NF,IndexUp_3d,IndexDn_3d);
-OppLplus_3d=NewOperator("Lplus",NF,IndexUp_3d,IndexDn_3d);
-OppLmin_3d =NewOperator("Lmin" ,NF,IndexUp_3d,IndexDn_3d);
-
-OppJx_3d   =NewOperator("Jx"   ,NF,IndexUp_3d,IndexDn_3d);
-OppJy_3d   =NewOperator("Jy"   ,NF,IndexUp_3d,IndexDn_3d);
-OppJz_3d   =NewOperator("Jz"   ,NF,IndexUp_3d,IndexDn_3d);
-OppJsqr_3d =NewOperator("Jsqr" ,NF,IndexUp_3d,IndexDn_3d);
-OppJplus_3d=NewOperator("Jplus",NF,IndexUp_3d,IndexDn_3d);
-OppJmin_3d =NewOperator("Jmin" ,NF,IndexUp_3d,IndexDn_3d);
+OppSx_3d = NewOperator("Sx", NF, IndexUp_3d, IndexDn_3d);
+OppSy_3d = NewOperator("Sy", NF, IndexUp_3d, IndexDn_3d);
+OppSz_3d = NewOperator("Sz", NF, IndexUp_3d, IndexDn_3d);
+OppSsqr_3d = NewOperator("Ssqr", NF, IndexUp_3d, IndexDn_3d);
+OppSplus_3d = NewOperator("Splus", NF, IndexUp_3d, IndexDn_3d);
+OppSmin_3d = NewOperator("Smin", NF, IndexUp_3d, IndexDn_3d);
+
+OppLx_3d = NewOperator("Lx", NF, IndexUp_3d, IndexDn_3d);
+OppLy_3d = NewOperator("Ly", NF, IndexUp_3d, IndexDn_3d);
+OppLz_3d = NewOperator("Lz", NF, IndexUp_3d, IndexDn_3d);
+OppLsqr_3d = NewOperator("Lsqr", NF, IndexUp_3d, IndexDn_3d);
+OppLplus_3d = NewOperator("Lplus", NF, IndexUp_3d, IndexDn_3d);
+OppLmin_3d = NewOperator("Lmin", NF, IndexUp_3d, IndexDn_3d);
+
+OppJx_3d = NewOperator("Jx", NF, IndexUp_3d, IndexDn_3d);
+OppJy_3d = NewOperator("Jy", NF, IndexUp_3d, IndexDn_3d);
+OppJz_3d = NewOperator("Jz", NF, IndexUp_3d, IndexDn_3d);
+OppJsqr_3d = NewOperator("Jsqr", NF, IndexUp_3d, IndexDn_3d);
+OppJplus_3d = NewOperator("Jplus", NF, IndexUp_3d, IndexDn_3d);
+OppJmin_3d = NewOperator("Jmin", NF, IndexUp_3d, IndexDn_3d);
 
-Oppldots_3d=NewOperator("ldots",NF,IndexUp_3d,IndexDn_3d);
+Oppldots_3d = NewOperator("ldots", NF, IndexUp_3d, IndexDn_3d);
 
 -- Angular momentum operators on the Ligand shell
 
-OppSx_Ld   =NewOperator("Sx"   ,NF,IndexUp_Ld,IndexDn_Ld);
-OppSy_Ld   =NewOperator("Sy"   ,NF,IndexUp_Ld,IndexDn_Ld);
-OppSz_Ld   =NewOperator("Sz"   ,NF,IndexUp_Ld,IndexDn_Ld);
-OppSsqr_Ld =NewOperator("Ssqr" ,NF,IndexUp_Ld,IndexDn_Ld);
-OppSplus_Ld=NewOperator("Splus",NF,IndexUp_Ld,IndexDn_Ld);
-OppSmin_Ld =NewOperator("Smin" ,NF,IndexUp_Ld,IndexDn_Ld);
-
-OppLx_Ld   =NewOperator("Lx"   ,NF,IndexUp_Ld,IndexDn_Ld);
-OppLy_Ld   =NewOperator("Ly"   ,NF,IndexUp_Ld,IndexDn_Ld);
-OppLz_Ld   =NewOperator("Lz"   ,NF,IndexUp_Ld,IndexDn_Ld);
-OppLsqr_Ld =NewOperator("Lsqr" ,NF,IndexUp_Ld,IndexDn_Ld);
-OppLplus_Ld=NewOperator("Lplus",NF,IndexUp_Ld,IndexDn_Ld);
-OppLmin_Ld =NewOperator("Lmin" ,NF,IndexUp_Ld,IndexDn_Ld);
-
-OppJx_Ld   =NewOperator("Jx"   ,NF,IndexUp_Ld,IndexDn_Ld);
-OppJy_Ld   =NewOperator("Jy"   ,NF,IndexUp_Ld,IndexDn_Ld);
-OppJz_Ld   =NewOperator("Jz"   ,NF,IndexUp_Ld,IndexDn_Ld);
-OppJsqr_Ld =NewOperator("Jsqr" ,NF,IndexUp_Ld,IndexDn_Ld);
-OppJplus_Ld=NewOperator("Jplus",NF,IndexUp_Ld,IndexDn_Ld);
-OppJmin_Ld =NewOperator("Jmin" ,NF,IndexUp_Ld,IndexDn_Ld);
+OppSx_Ld = NewOperator("Sx", NF, IndexUp_Ld, IndexDn_Ld);
+OppSy_Ld = NewOperator("Sy", NF, IndexUp_Ld, IndexDn_Ld);
+OppSz_Ld = NewOperator("Sz", NF, IndexUp_Ld, IndexDn_Ld);
+OppSsqr_Ld = NewOperator("Ssqr", NF, IndexUp_Ld, IndexDn_Ld);
+OppSplus_Ld = NewOperator("Splus", NF, IndexUp_Ld, IndexDn_Ld);
+OppSmin_Ld = NewOperator("Smin", NF, IndexUp_Ld, IndexDn_Ld);
+
+OppLx_Ld = NewOperator("Lx", NF, IndexUp_Ld, IndexDn_Ld);
+OppLy_Ld = NewOperator("Ly", NF, IndexUp_Ld, IndexDn_Ld);
+OppLz_Ld = NewOperator("Lz", NF, IndexUp_Ld, IndexDn_Ld);
+OppLsqr_Ld = NewOperator("Lsqr", NF, IndexUp_Ld, IndexDn_Ld);
+OppLplus_Ld = NewOperator("Lplus", NF, IndexUp_Ld, IndexDn_Ld);
+OppLmin_Ld = NewOperator("Lmin", NF, IndexUp_Ld, IndexDn_Ld);
+
+OppJx_Ld = NewOperator("Jx", NF, IndexUp_Ld, IndexDn_Ld);
+OppJy_Ld = NewOperator("Jy", NF, IndexUp_Ld, IndexDn_Ld);
+OppJz_Ld = NewOperator("Jz", NF, IndexUp_Ld, IndexDn_Ld);
+OppJsqr_Ld = NewOperator("Jsqr", NF, IndexUp_Ld, IndexDn_Ld);
+OppJplus_Ld = NewOperator("Jplus", NF, IndexUp_Ld, IndexDn_Ld);
+OppJmin_Ld = NewOperator("Jmin", NF, IndexUp_Ld, IndexDn_Ld);
 
 -- total angular momentum
 
 OppSx = OppSx_3d + OppSx_Ld
 OppSy = OppSy_3d + OppSy_Ld
 OppSz = OppSz_3d + OppSz_Ld
 OppSsqr = OppSx * OppSx + OppSy * OppSy + OppSz * OppSz
@@ -256,76 +181,75 @@
 OppJz = OppJz_3d + OppJz_Ld
 OppJsqr = OppJx * OppJx + OppJy * OppJy + OppJz * OppJz
 
 -- define the coulomb operator
 -- we here define the part depending on F0 seperately from the part depending on F2
 -- when summing we can put in the numerical values of the slater integrals
 
-OppF0_3d =NewOperator("U",NF,IndexUp_3d,IndexDn_3d,{1,0,0});
-OppF2_3d =NewOperator("U",NF,IndexUp_3d,IndexDn_3d,{0,1,0});
-OppF4_3d =NewOperator("U",NF,IndexUp_3d,IndexDn_3d,{0,0,1});
+OppF0_3d = NewOperator("U", NF, IndexUp_3d, IndexDn_3d, {1, 0, 0});
+OppF2_3d = NewOperator("U", NF, IndexUp_3d, IndexDn_3d, {0, 1, 0});
+OppF4_3d = NewOperator("U", NF, IndexUp_3d, IndexDn_3d, {0, 0, 1});
 
 --- Crystal field operator for the d-shell
-Akm = PotentialExpandedOnClm("Oh",2,{0.6, -0.4});
+Akm = PotentialExpandedOnClm("Oh", 2, {0.6, -0.4});
 OpptenDq_3d = NewOperator("CF", NF, IndexUp_3d, IndexDn_3d, Akm)
 OpptenDq_Ld = NewOperator("CF", NF, IndexUp_Ld, IndexDn_Ld, Akm)
 
 -- define L-d interaction
 
-Akm = PotentialExpandedOnClm("Oh",2,{1,0});
-OppVa1g  = NewOperator("CF", NF, IndexUp_3d,IndexDn_3d, IndexUp_Ld,IndexDn_Ld,Akm) +  NewOperator("CF", NF, IndexUp_Ld,IndexDn_Ld, IndexUp_3d,IndexDn_3d,Akm)
-Akm = PotentialExpandedOnClm("Oh",2,{0,1});
-OppVeg = NewOperator("CF", NF, IndexUp_3d,IndexDn_3d, IndexUp_Ld,IndexDn_Ld,Akm) +  NewOperator("CF", NF, IndexUp_Ld,IndexDn_Ld, IndexUp_3d,IndexDn_3d,Akm)
+Akm = PotentialExpandedOnClm("Oh", 2, {1, 0});
+OppVa1g = NewOperator("CF", NF, IndexUp_3d, IndexDn_3d, IndexUp_Ld, IndexDn_Ld, Akm) +
+              NewOperator("CF", NF, IndexUp_Ld, IndexDn_Ld, IndexUp_3d, IndexDn_3d, Akm)
+Akm = PotentialExpandedOnClm("Oh", 2, {0, 1});
+OppVeg = NewOperator("CF", NF, IndexUp_3d, IndexDn_3d, IndexUp_Ld, IndexDn_Ld, Akm) +
+             NewOperator("CF", NF, IndexUp_Ld, IndexDn_Ld, IndexUp_3d, IndexDn_3d, Akm)
 
 OppNeg_Ld = NewOperator("CF", NF, IndexUp_Ld, IndexDn_Ld, Akm)
 OppNt2g_Ld = NewOperator("CF", NF, IndexUp_Ld, IndexDn_Ld, Akm)
 
-OppNUp_2p = NewOperator("Number", NF, IndexUp_2p,IndexUp_2p,{1,1,1})
-OppNDn_2p = NewOperator("Number", NF, IndexDn_2p,IndexDn_2p,{1,1,1})
+OppNUp_2p = NewOperator("Number", NF, IndexUp_2p, IndexUp_2p, {1, 1, 1})
+OppNDn_2p = NewOperator("Number", NF, IndexDn_2p, IndexDn_2p, {1, 1, 1})
 OppN_2p = OppNUp_2p + OppNDn_2p
-OppNUp_3d = NewOperator("Number", NF, IndexUp_3d,IndexUp_3d,{1,1,1,1,1})
-OppNDn_3d = NewOperator("Number", NF, IndexDn_3d,IndexDn_3d,{1,1,1,1,1})
+OppNUp_3d = NewOperator("Number", NF, IndexUp_3d, IndexUp_3d, {1, 1, 1, 1, 1})
+OppNDn_3d = NewOperator("Number", NF, IndexDn_3d, IndexDn_3d, {1, 1, 1, 1, 1})
 OppN_3d = OppNUp_3d + OppNDn_3d
-OppNUp_Ld = NewOperator("Number", NF, IndexUp_Ld,IndexUp_Ld,{1,1,1,1,1})
-OppNDn_Ld = NewOperator("Number", NF, IndexDn_Ld,IndexDn_Ld,{1,1,1,1,1})
+OppNUp_Ld = NewOperator("Number", NF, IndexUp_Ld, IndexUp_Ld, {1, 1, 1, 1, 1})
+OppNDn_Ld = NewOperator("Number", NF, IndexDn_Ld, IndexDn_Ld, {1, 1, 1, 1, 1})
 OppN_Ld = OppNUp_Ld + OppNDn_Ld
 
 -- Number of electrons in each of the 3d orbitals
-Akm = PotentialExpandedOnClm("Oh",2,{1,0});
-OppNa1g  = NewOperator("CF", NF, IndexUp_3d,IndexDn_3d,Akm)
-Akm = PotentialExpandedOnClm("Oh",2,{0,1});
-OppNeg = NewOperator("CF", NF, IndexUp_3d,IndexDn_3d,Akm)
-
+Akm = PotentialExpandedOnClm("Oh", 2, {1, 0});
+OppNa1g = NewOperator("CF", NF, IndexUp_3d, IndexDn_3d, Akm)
+Akm = PotentialExpandedOnClm("Oh", 2, {0, 1});
+OppNeg = NewOperator("CF", NF, IndexUp_3d, IndexDn_3d, Akm)
 
 -- In order te describe the resonance we need the interaction on the 2p shell (spin-orbit)
-Oppcldots= NewOperator("ldots",NF,IndexUp_2p,IndexDn_2p);
-OppUpdF0 = NewOperator("U",NF,IndexUp_2p,IndexDn_2p,IndexUp_3d,IndexDn_3d,{1,0},{0,0});
-OppUpdF2 = NewOperator("U",NF,IndexUp_2p,IndexDn_2p,IndexUp_3d,IndexDn_3d,{0,1},{0,0});
-OppUpdG1 = NewOperator("U",NF,IndexUp_2p,IndexDn_2p,IndexUp_3d,IndexDn_3d,{0,0},{1,0});
-OppUpdG3 = NewOperator("U",NF,IndexUp_2p,IndexDn_2p,IndexUp_3d,IndexDn_3d,{0,0},{0,1});
-
-
+Oppcldots = NewOperator("ldots", NF, IndexUp_2p, IndexDn_2p);
+OppUpdF0 = NewOperator("U", NF, IndexUp_2p, IndexDn_2p, IndexUp_3d, IndexDn_3d, {1, 0}, {0, 0});
+OppUpdF2 = NewOperator("U", NF, IndexUp_2p, IndexDn_2p, IndexUp_3d, IndexDn_3d, {0, 1}, {0, 0});
+OppUpdG1 = NewOperator("U", NF, IndexUp_2p, IndexDn_2p, IndexUp_3d, IndexDn_3d, {0, 0}, {1, 0});
+OppUpdG3 = NewOperator("U", NF, IndexUp_2p, IndexDn_2p, IndexUp_3d, IndexDn_3d, {0, 0}, {0, 1});
 
 -- next we define the dipole operator. The dipole operator is given as epsilon.r
 -- with epsilon the polarization vector of the light and r the unit position vector
 -- We can expand the position vector on (renormalized) spherical harmonics and use
 -- the crystal-field operator to create the dipole operator.
 -- dipole transition
 
-t=math.sqrt(1/2);
+t = math.sqrt(1 / 2);
 
-Akm = {{1,-1,t},{1, 1,-t}};
+Akm = {{1, -1, t}, {1, 1, -t}};
 TXASx = NewOperator("CF", NF, IndexUp_3d, IndexDn_3d, IndexUp_2p, IndexDn_2p, Akm);
-Akm = {{1,-1,t*I},{1, 1,t*I}};
+Akm = {{1, -1, t * I}, {1, 1, t * I}};
 TXASy = NewOperator("CF", NF, IndexUp_3d, IndexDn_3d, IndexUp_2p, IndexDn_2p, Akm);
-Akm = {{1,0,1}};
+Akm = {{1, 0, 1}};
 TXASz = NewOperator("CF", NF, IndexUp_3d, IndexDn_3d, IndexUp_2p, IndexDn_2p, Akm);
 
-TXASr = t*(TXASx - I * TXASy);
-TXASl =-t*(TXASx + I * TXASy);
+TXASr = t * (TXASx - I * TXASy);
+TXASl = -t * (TXASx + I * TXASy);
 
 TXASr.Chop()
 TXASl.Chop()
 
 TXASxdag = ConjugateTranspose(TXASx);
 TXASydag = ConjugateTranspose(TXASy);
 TXASzdag = ConjugateTranspose(TXASz);
@@ -334,216 +258,245 @@
 
 -- Setup parameters
 Udd = 0
 Upd = 0
 tenDqL = 0
 Delta = 0
 
---overwrite init variables with ParVals values
-for i=1,#pars do
-  if(pars[i].name == "Udd") then Udd = pars[i].val end
-  if(pars[i].name == "Upd_Udd") then Upd = Udd + pars[i].val end
-  if(pars[i].name == "tenDqL") then tenDqL = pars[i].val end
-  if(pars[i].name == "Delta") then Delta = pars[i].val end
+-- overwrite init variables with ParVals values
+for i = 1, #pars do
+    if (pars[i].name == "Udd") then
+        Udd = pars[i].val
+    end
+    if (pars[i].name == "Upd_Udd") then
+        Upd = Udd + pars[i].val
+    end
+    if (pars[i].name == "tenDqL") then
+        tenDqL = pars[i].val
+    end
+    if (pars[i].name == "Delta") then
+        Delta = pars[i].val
+    end
 end
 
 Fdd = 0.8
 Fpd = 0.8
 Gpd = 0.8
 
 --- scaling with beta factor as specified in py file
-for i=1,#pars do
-if(pars[i].name == "Fdd") then
-    F2dd = F2dd * pars[i].val
-    F4dd = F4dd * pars[i].val
-end
+for i = 1, #pars do
+    if (pars[i].name == "Fdd") then
+        F2dd = F2dd * pars[i].val
+        F4dd = F4dd * pars[i].val
+    end
 
-if(pars[i].name == "XFdd") then
-    XF2dd = XF2dd * pars[i].val
-    XF4dd = XF4dd * pars[i].val
-end
+    if (pars[i].name == "XFdd") then
+        XF2dd = XF2dd * pars[i].val
+        XF4dd = XF4dd * pars[i].val
+    end
 
-if(pars[i].name == "Fpd") then
-    F2pd = F2pd * pars[i].val
-end
+    if (pars[i].name == "Fpd") then
+        F2pd = F2pd * pars[i].val
+    end
 
-if(pars[i].name == "Gpd") then
-    G1pd = G1pd * pars[i].val
-    G3pd = G3pd * pars[i].val
-end
+    if (pars[i].name == "Gpd") then
+        G1pd = G1pd * pars[i].val
+        G3pd = G3pd * pars[i].val
+    end
 
-if(pars[i].name == "zeta_3d") then
-    zeta_3d = zeta_3d * pars[i].val
-end
+    if (pars[i].name == "zeta_3d") then
+        zeta_3d = zeta_3d * pars[i].val
+    end
 
-if(pars[i].name == "zeta_2p") then
-    zeta_2p = zeta_2p * pars[i].val
-end
+    if (pars[i].name == "zeta_2p") then
+        zeta_2p = zeta_2p * pars[i].val
+    end
 
-if(pars[i].name == "Xzeta_3d") then
-    Xzeta_3d = Xzeta_3d * pars[i].val
-end
+    if (pars[i].name == "Xzeta_3d") then
+        Xzeta_3d = Xzeta_3d * pars[i].val
+    end
 
 end
 
-F0dd    = Udd + (F2dd+F4dd)*(2/63)
-XF0dd    = Udd + (XF2dd+XF4dd)*(2/63)
-F0pd    =  Upd + G1pd*(1/15) + G3pd*(3/70)
-Bz      = 0.000001
-Hz      = 0.120
-
-ed      = (10*Delta-nd*(19+nd)*Udd/2)/(10+nd)
-eL      = nd*((1+nd)*Udd/2-Delta)/(10+nd)
-
-epfinal = (10*Delta+(1+nd)*(nd*Udd/2-(10+nd)*Upd))/(16+nd)
-edfinal = (10*Delta-nd*(31+nd)*Udd/2-90*Upd)/(16+nd)
-eLfinal = ((1+nd)*(nd*Udd/2+6*Upd)-(6+nd)*Delta)/(16+nd)
+F0dd = Udd + (F2dd + F4dd) * (2 / 63)
+XF0dd = Udd + (XF2dd + XF4dd) * (2 / 63)
+F0pd = Upd + G1pd * (1 / 15) + G3pd * (3 / 70)
+Bz = 0.000001
+Hz = 0.120
+
+ed = (10 * Delta - nd * (19 + nd) * Udd / 2) / (10 + nd)
+eL = nd * ((1 + nd) * Udd / 2 - Delta) / (10 + nd)
+
+epfinal = (10 * Delta + (1 + nd) * (nd * Udd / 2 - (10 + nd) * Upd)) / (16 + nd)
+edfinal = (10 * Delta - nd * (31 + nd) * Udd / 2 - 90 * Upd) / (16 + nd)
+eLfinal = ((1 + nd) * (nd * Udd / 2 + 6 * Upd) - (6 + nd) * Delta) / (16 + nd)
 
 ----------------------------------------------
 -- From here on it becomes different again
 ----------------------------------------------
 
 -- we need two Hamiltonians, one to calculate the fundamental spectra (HEff) and one to
 -- calculate the RIXS with the field in an arbitrary direction
 
-HexDirNorm = sqrt( sqr(HexDir[1]) + sqr(HexDir[2]) + sqr(HexDir[3]) )
-HExchange = ( Hex * HexDir[1] / HexDirNorm ) * OppSx + ( Hex * HexDir[2] / HexDirNorm ) * OppSy + ( Hex * HexDir[3] / HexDirNorm ) * OppSz
-
-Hamiltonian    = HExchange + F0dd*OppF0_3d + F2dd*OppF2_3d + F4dd*OppF4_3d + tenDq*OpptenDq_3d + zeta_3d*Oppldots_3d + Bz*(2*OppSz_3d + OppLz_3d) + Hz * OppSz_3d + tenDqL*OpptenDq_Ld + Veg * OppVeg + Va1g * OppVa1g + ed * OppN_3d + eL * OppN_Ld;
-
-XASHamiltonian = XF0dd*OppF0_3d + XF2dd*OppF2_3d + XF4dd*OppF4_3d + tenDqF*OpptenDq_3d + zeta_3d*Oppldots_3d + Bz*(2*OppSz_3d + OppLz_3d) + Hz * OppSz_3d + tenDqL*OpptenDq_Ld + VegF * OppVeg + Va1gF * OppVa1g + edfinal * OppN_3d + eLfinal * OppN_Ld + epfinal * OppN_2p + zeta_2p * Oppcldots + F0pd * OppUpdF0 + F2pd * OppUpdF2 + G1pd * OppUpdG1 + G3pd * OppUpdG3;
-
+HexDirNorm = sqrt(sqr(HexDir[1]) + sqr(HexDir[2]) + sqr(HexDir[3]))
+HExchange = (Hex * HexDir[1] / HexDirNorm) * OppSx + (Hex * HexDir[2] / HexDirNorm) * OppSy +
+                (Hex * HexDir[3] / HexDirNorm) * OppSz
+
+Hamiltonian = HExchange + F0dd * OppF0_3d + F2dd * OppF2_3d + F4dd * OppF4_3d + tenDq * OpptenDq_3d + zeta_3d *
+                  Oppldots_3d + Bz * (2 * OppSz_3d + OppLz_3d) + Hz * OppSz_3d + tenDqL * OpptenDq_Ld + Veg * OppVeg +
+                  Va1g * OppVa1g + ed * OppN_3d + eL * OppN_Ld;
+
+XASHamiltonian = XF0dd * OppF0_3d + XF2dd * OppF2_3d + XF4dd * OppF4_3d + tenDqF * OpptenDq_3d + zeta_3d * Oppldots_3d +
+                     Bz * (2 * OppSz_3d + OppLz_3d) + Hz * OppSz_3d + tenDqL * OpptenDq_Ld + VegF * OppVeg + Va1gF *
+                     OppVa1g + edfinal * OppN_3d + eLfinal * OppN_Ld + epfinal * OppN_2p + zeta_2p * Oppcldots + F0pd *
+                     OppUpdF0 + F2pd * OppUpdF2 + G1pd * OppUpdG1 + G3pd * OppUpdG3;
 
 -- we now can create the lowest Npsi eigenstates:
 -- the calculation to the lowest 3 eigenstates.
-Npsi=3;
---Npsi=math.fact(14)/math.fact(nd)/math.fact(14-nd)
+Npsi = 3;
+-- Npsi=math.fact(14)/math.fact(nd)/math.fact(14-nd)
 -- in order to make sure we have a filling of 2 electrons we need to define some restrictions
 res3d = "000000 1111111111 0000000000"
 resL = "000000 0000000000 1111111111"
 res2p = "111111 0000000000 0000000000"
-StartRestrictions = {NF, NB, {res3d,nd,nd}, {res2p, 6, 6}, {resL, 10, 10}}
---psiListEff = Eigensystem(HamiltonianEff, StartRestrictions, Npsi)
-psiList = Eigensystem(Hamiltonian, StartRestrictions, Npsi, {{"restrictions", {NF,NB,{res3d,nd,nd+1}}}})
-oppList={Hamiltonian, HExchange, OppSsqr, OppLsqr, OppJsqr, OppSz, OppLz, Oppldots_3d, OppNa1g, OppNeg, OppN_3d, OppN_Ld, OppN_2p};
-print( '\n');
-print( '================================================================================================\n');
-print( 'Analysis of the initial Hamiltonian:\n');
+StartRestrictions = {NF, NB, {res3d, nd, nd}, {res2p, 6, 6}, {resL, 10, 10}}
+-- psiListEff = Eigensystem(HamiltonianEff, StartRestrictions, Npsi)
+psiList = Eigensystem(Hamiltonian, StartRestrictions, Npsi, {{"restrictions", {NF, NB, {res3d, nd, nd + 1}}}})
+oppList = {Hamiltonian, HExchange, OppSsqr, OppLsqr, OppJsqr, OppSz, OppLz, Oppldots_3d, OppNa1g, OppNeg, OppN_3d,
+           OppN_Ld, OppN_2p};
+print('\n');
+print('================================================================================================\n');
+print('Analysis of the initial Hamiltonian:\n');
 print(' <E>  <E_ex> <S^2> <L^2>   <J^2>  <S_z> <L_z>  <l.s> Neg Nt2g N_3d   N_L N_2p');
-for i = 1,#psiList do
-  for j = 1,#oppList do
-    expectationvalue = Chop(psiList[i]*oppList[j]*psiList[i])
-    io.write(string.format("%4.3f ",expectationvalue))
-  end
-  io.write("\n")
-end
-print( '================================================================================================\n');
---print( '\n');
-print( '=============================================\n');
-print( 'Analysis of the Calculated orbitals energies:\n');
+for i = 1, #psiList do
+    for j = 1, #oppList do
+        expectationvalue = Chop(psiList[i] * oppList[j] * psiList[i])
+        io.write(string.format("%4.3f ", expectationvalue))
+    end
+    io.write("\n")
+end
+print('================================================================================================\n');
+-- print( '\n');
+print('=============================================\n');
+print('Analysis of the Calculated orbitals energies:\n');
 print("Veg =", Va1g)
 print("Vt2g =", Veg)
-print( '=============================================\n');
+print('=============================================\n');
 -- spectra XAS
 doXAS = false
-for i=1,#pars do
-  if(pars[i].name == "XAS") then doXAS = true end
+for i = 1, #pars do
+    if (pars[i].name == "XAS") then
+        doXAS = true
+    end
 end
 
-if(doXAS) then
+if (doXAS) then
 
+    XAS_Broad = {}
+    XAS_Gamma = 0
+    for i = 1, #pars do
+        if (pars[i].name == "XAS_Broad") then
+            XAS_Broad[#XAS_Broad + 1] = pars[i].val
+        end
+        if (pars[i].name == "XAS_Gamma") then
+            XAS_Gamma = pars[i].val
+        end
+    end
 
-XAS_Broad = {}
-XAS_Gamma = 0
-for i=1,#pars do 
-  if(pars[i].name == "XAS_Broad") then
-    XAS_Broad[#XAS_Broad+1] = pars[i].val
-  end
-  if(pars[i].name == "XAS_Gamma") then
-    XAS_Gamma = pars[i].val
-  end
-end
-
-XASRestrictions = {"restrictions",{NF,NB,{res3d,nd+1,nd+2}}}
---XASSpectra = CreateSpectra(XASHamiltonian   , Tin, psiList[1],{{"Emin",-10},{"Emax",20},{"NE",2000},{"Gamma",0.1},XASRestrictions});
-Spectra_x = CreateSpectra(XASHamiltonian,TXASx,psiList[1],{{"Emin",-10},{"Emax",20},{"NE",2000},{"Gamma",0.1},XASRestrictions});
-Spectra_z = CreateSpectra(XASHamiltonian,TXASz,psiList[1],{{"Emin",-10},{"Emax",20},{"NE",2000},{"Gamma",0.1},XASRestrictions});
-XASSpectra = 1/2 * (Spectra_x + Spectra_z)
--- workaround for case where only Gaussian broadening is used ()
-if #XAS_Broad == 0 then
-  XAS_Broad = {{0, 0}}
-end
-XASSpectra.Broaden(XAS_Gamma,XAS_Broad)
-local file = assert(io.open("XAS_Calc.dat","w"))
-
-SpecTables = Spectra.ToTable(XASSpectra)
-
-for i=1,#SpecTables[1] do
-    file:write(string.format("%14.7E ",SpecTables[1][i][1]))--+853-peakE
-    for j=1,#SpecTables do
-      file:write(string.format("%14.7E ",-SpecTables[j][i][2].Im))
-    end
-    file:write("\n")
-  end
-  file:close()
+    XASRestrictions = {"restrictions", {NF, NB, {res3d, nd + 1, nd + 2}}}
+    -- XASSpectra = CreateSpectra(XASHamiltonian   , Tin, psiList[1],{{"Emin",-10},{"Emax",20},{"NE",2000},{"Gamma",0.1},XASRestrictions});
+    Spectra_x = CreateSpectra(XASHamiltonian, TXASx, psiList[1],
+        {{"Emin", -10}, {"Emax", 20}, {"NE", 2000}, {"Gamma", 0.1}, XASRestrictions});
+    Spectra_z = CreateSpectra(XASHamiltonian, TXASz, psiList[1],
+        {{"Emin", -10}, {"Emax", 20}, {"NE", 2000}, {"Gamma", 0.1}, XASRestrictions});
+    XASSpectra = 1 / 2 * (Spectra_x + Spectra_z)
+    -- workaround for case where only Gaussian broadening is used ()
+    if #XAS_Broad == 0 then
+        XAS_Broad = {{0, 0}}
+    end
+    XASSpectra.Broaden(XAS_Gamma, XAS_Broad)
+    local file = assert(io.open("XAS_Calc.dat", "w"))
+
+    SpecTables = Spectra.ToTable(XASSpectra)
+
+    for i = 1, #SpecTables[1] do
+        file:write(string.format("%14.7E ", SpecTables[1][i][1])) -- +853-peakE
+        for j = 1, #SpecTables do
+            file:write(string.format("%14.7E ", -SpecTables[j][i][2].Im))
+        end
+        file:write("\n")
+    end
+    file:close()
 end
 -- And we want to copare the effective operator RIXS calculation to the full RIXS calculation
 
 -- spectra RIXS
 doRIXS = false
 RIXSEners = {}
-for i=1,#pars do
-  if(pars[i].name == "RIXS") then
-    doRIXS = true
-    RIXSEners[#RIXSEners+1] = pars[i].val
-  end
+for i = 1, #pars do
+    if (pars[i].name == "RIXS") then
+        doRIXS = true
+        RIXSEners[#RIXSEners + 1] = pars[i].val
+    end
 end
 
 RIXS_Broad = {}
-for i=1,#pars do 
-  if(pars[i].name == "RIXS_Broad") then
-    RIXS_Broad[#RIXS_Broad+1] = pars[i].val
-  end
+for i = 1, #pars do
+    if (pars[i].name == "RIXS_Broad") then
+        RIXS_Broad[#RIXS_Broad + 1] = pars[i].val
+    end
 end
 
 Gamma1 = 1
 
-for i=1,#pars do
-if(pars[i].name == "Gamma1") then
-    Gamma1 = pars[i].val
-end
+for i = 1, #pars do
+    if (pars[i].name == "Gamma1") then
+        Gamma1 = pars[i].val
+    end
 end
 
-if(doRIXS) then
-
-RIXSRestrictions1  = {"restrictions1",{NF,NB,{res3d,nd+1,nd+2}}}
-RIXSRestrictions2  = {"restrictions2",{NF, NB, {resL,9,10}}}
-
-  RIXSSpectra_zx = {}; RIXSSpectra_zy = {}; RIXSSpectra_xz = {}; RIXSSpectra_xy = {}; RIXSSpectra = {}
-  RIXSTables = {}
-  for i=1,#RIXSEners do
-    RIXSSpectra_zx[i] = CreateResonantSpectra(XASHamiltonian, Hamiltonian, TXASz, TXASxdag, psiList[1], {{"Emin1",RIXSEners[i]}, {"Emax1",RIXSEners[i]}, {"NE1",1}, {"Gamma1",Gamma1}, {"Emin2",-2}, {"Emax2",20}, {"NE2",2000}, {"Gamma2",0.01},RIXSRestrictions1,RIXSRestrictions2})
-    RIXSSpectra_zy[i] = CreateResonantSpectra(XASHamiltonian, Hamiltonian, TXASz, TXASydag, psiList[1], {{"Emin1",RIXSEners[i]}, {"Emax1",RIXSEners[i]}, {"NE1",1}, {"Gamma1",Gamma1}, {"Emin2",-2}, {"Emax2",20}, {"NE2",2000}, {"Gamma2",0.01},RIXSRestrictions1,RIXSRestrictions2})
-    RIXSSpectra_xz[i] = CreateResonantSpectra(XASHamiltonian, Hamiltonian, TXASx, TXASzdag, psiList[1], {{"Emin1",RIXSEners[i]}, {"Emax1",RIXSEners[i]}, {"NE1",1}, {"Gamma1",Gamma1}, {"Emin2",-2}, {"Emax2",20}, {"NE2",2000}, {"Gamma2",0.01},RIXSRestrictions1,RIXSRestrictions2})
-    RIXSSpectra_xy[i] = CreateResonantSpectra(XASHamiltonian, Hamiltonian, TXASx, TXASydag, psiList[1], {{"Emin1",RIXSEners[i]}, {"Emax1",RIXSEners[i]}, {"NE1",1}, {"Gamma1",Gamma1}, {"Emin2",-2}, {"Emax2",20}, {"NE2",2000}, {"Gamma2",0.01},RIXSRestrictions1,RIXSRestrictions2})
-    RIXSSpectra[i] = 0.25*(RIXSSpectra_zx[i] + RIXSSpectra_zy[i] + RIXSSpectra_xz[i] + RIXSSpectra_xy[i])
-    if #RIXS_Broad > 0 then
-      RIXSSpectra[i].Broaden(0,RIXS_Broad)
-    end
-    RIXSTables[i] =   Spectra.ToTable(RIXSSpectra[i])
-  end
-  --Now write to file
-  local file = assert(io.open("RIXS_Calc.dat","w"))
-  for i=1,#RIXSTables[1][1] do --loop over RIXS energy
-    file:write(string.format("%14.7E ",RIXSTables[1][1][i][1]))
-    for j=1,#RIXSTables do --loop over incident energy
-      file:write(string.format("%14.7E ",-RIXSTables[j][1][i][2].Im))
-    end
-    file:write("\n")
-  end
-  file:close()
+if (doRIXS) then
+
+    RIXSRestrictions1 = {"restrictions1", {NF, NB, {res3d, nd + 1, nd + 2}}}
+    RIXSRestrictions2 = {"restrictions2", {NF, NB, {resL, 9, 10}}}
+
+    RIXSSpectra_zx = {};
+    RIXSSpectra_zy = {};
+    RIXSSpectra_xz = {};
+    RIXSSpectra_xy = {};
+    RIXSSpectra = {}
+    RIXSTables = {}
+    for i = 1, #RIXSEners do
+        RIXSSpectra_zx[i] = CreateResonantSpectra(XASHamiltonian, Hamiltonian, TXASz, TXASxdag, psiList[1],
+            {{"Emin1", RIXSEners[i]}, {"Emax1", RIXSEners[i]}, {"NE1", 1}, {"Gamma1", Gamma1}, {"Emin2", -2},
+             {"Emax2", 20}, {"NE2", 2000}, {"Gamma2", 0.01}, RIXSRestrictions1, RIXSRestrictions2})
+        RIXSSpectra_zy[i] = CreateResonantSpectra(XASHamiltonian, Hamiltonian, TXASz, TXASydag, psiList[1],
+            {{"Emin1", RIXSEners[i]}, {"Emax1", RIXSEners[i]}, {"NE1", 1}, {"Gamma1", Gamma1}, {"Emin2", -2},
+             {"Emax2", 20}, {"NE2", 2000}, {"Gamma2", 0.01}, RIXSRestrictions1, RIXSRestrictions2})
+        RIXSSpectra_xz[i] = CreateResonantSpectra(XASHamiltonian, Hamiltonian, TXASx, TXASzdag, psiList[1],
+            {{"Emin1", RIXSEners[i]}, {"Emax1", RIXSEners[i]}, {"NE1", 1}, {"Gamma1", Gamma1}, {"Emin2", -2},
+             {"Emax2", 20}, {"NE2", 2000}, {"Gamma2", 0.01}, RIXSRestrictions1, RIXSRestrictions2})
+        RIXSSpectra_xy[i] = CreateResonantSpectra(XASHamiltonian, Hamiltonian, TXASx, TXASydag, psiList[1],
+            {{"Emin1", RIXSEners[i]}, {"Emax1", RIXSEners[i]}, {"NE1", 1}, {"Gamma1", Gamma1}, {"Emin2", -2},
+             {"Emax2", 20}, {"NE2", 2000}, {"Gamma2", 0.01}, RIXSRestrictions1, RIXSRestrictions2})
+        RIXSSpectra[i] = 0.25 * (RIXSSpectra_zx[i] + RIXSSpectra_zy[i] + RIXSSpectra_xz[i] + RIXSSpectra_xy[i])
+        if #RIXS_Broad > 0 then
+            RIXSSpectra[i].Broaden(0, RIXS_Broad)
+        end
+        RIXSTables[i] = Spectra.ToTable(RIXSSpectra[i])
+    end
+    -- Now write to file
+    local file = assert(io.open("RIXS_Calc.dat", "w"))
+    for i = 1, #RIXSTables[1][1] do -- loop over RIXS energy
+        file:write(string.format("%14.7E ", RIXSTables[1][1][i][1]))
+        for j = 1, #RIXSTables do -- loop over incident energy
+            file:write(string.format("%14.7E ", -RIXSTables[j][1][i][2].Im))
+        end
+        file:write("\n")
+    end
+    file:close()
 end
 
 print("Finished calculating the spectra");
 
 TimeEnd("LF_RIXS")
 TimePrint()
```

### Comparing `quantylf-0.0.6/src/QuantyLF.egg-info/PKG-INFO` & `quantylf-0.0.7/src/QuantyLF.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantyLF
-Version: 0.0.6
+Version: 0.0.7
 Summary: QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

