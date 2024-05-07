# Comparing `tmp/DesalSim-0.1-py3-none-any.whl.zip` & `tmp/DesalSim-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,8 @@
-Zip file size: 194341 bytes, number of entries: 87
--rw-rw-rw-  2.0 fat     1128 b- defN 24-Apr-29 21:23 Desalsim/__init__.py
--rw-rw-rw-  2.0 fat     1927 b- defN 24-Feb-13 13:45 Desalsim/constants.py
--rw-rw-rw-  2.0 fat      468 b- defN 24-Apr-10 15:15 Desalsim/density_calc.py
--rw-rw-rw-  2.0 fat     8821 b- defN 24-May-06 16:12 Desalsim/economic_f.py
--rw-rw-rw-  2.0 fat     2950 b- defN 24-Apr-29 20:32 Desalsim/ed_unit_f.py
--rw-rw-rw-  2.0 fat    11744 b- defN 24-Apr-29 21:17 Desalsim/edbm_unit_f.py
--rw-rw-rw-  2.0 fat    49286 b- defN 24-Feb-14 10:34 Desalsim/efc_unit_f.py
--rw-rw-rw-  2.0 fat     4494 b- defN 24-Apr-29 20:24 Desalsim/med_unit_f.py
--rw-rw-rw-  2.0 fat    10049 b- defN 24-Apr-29 21:14 Desalsim/mfpfr_unit_f.py
--rw-rw-rw-  2.0 fat     6987 b- defN 24-May-06 08:40 Desalsim/nanofiltration_unit_f.py
--rw-rw-rw-  2.0 fat     4366 b- defN 24-Apr-29 21:19 Desalsim/ro_unit_f.py
--rw-rw-rw-  2.0 fat      347 b- defN 23-Oct-30 09:38 Desalsim/scaleup.py
--rw-rw-rw-  2.0 fat     8692 b- defN 24-Apr-29 19:44 Desalsim/thermal_cryst_f.py
+Zip file size: 166224 bytes, number of entries: 74
 -rw-rw-rw-  2.0 fat     1128 b- defN 24-Apr-29 21:23 desalination_and_brine_treatment/__init__.py
 -rw-rw-rw-  2.0 fat     4531 b- defN 24-Apr-11 13:19 desalination_and_brine_treatment/comparison.py
 -rw-rw-rw-  2.0 fat     1927 b- defN 24-Feb-13 13:45 desalination_and_brine_treatment/constants.py
 -rw-rw-rw-  2.0 fat      468 b- defN 24-Apr-10 15:15 desalination_and_brine_treatment/density_calc.py
 -rw-rw-rw-  2.0 fat     8821 b- defN 24-May-06 16:12 desalination_and_brine_treatment/economic_f.py
 -rw-rw-rw-  2.0 fat     2950 b- defN 24-Apr-29 20:32 desalination_and_brine_treatment/ed_unit_f.py
 -rw-rw-rw-  2.0 fat    11744 b- defN 24-Apr-29 21:17 desalination_and_brine_treatment/edbm_unit_f.py
@@ -77,13 +64,13 @@
 -rw-rw-rw-  2.0 fat    10407 b- defN 24-May-03 12:57 tests/mfpfr_unit_f.py
 -rw-rw-rw-  2.0 fat     2743 b- defN 24-May-03 12:56 tests/mfpfr_unittest.py
 -rw-rw-rw-  2.0 fat     6961 b- defN 24-May-06 08:40 tests/nanofiltration_unit_f.py
 -rw-rw-rw-  2.0 fat     1777 b- defN 24-May-06 08:40 tests/nanofiltration_unittest.py
 -rw-rw-rw-  2.0 fat      347 b- defN 23-Oct-30 09:38 tests/scaleup.py
 -rw-rw-rw-  2.0 fat     8687 b- defN 24-May-05 10:31 tests/thermal_cryst_f.py
 -rw-rw-rw-  2.0 fat     4560 b- defN 24-May-05 10:30 tests/thermal_cryst_unittest.py
--rw-rw-rw-  2.0 fat     1086 b- defN 24-May-07 11:19 DesalSim-0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     8363 b- defN 24-May-07 11:19 DesalSim-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 11:19 DesalSim-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 24-May-07 11:19 DesalSim-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     7307 b- defN 24-May-07 11:19 DesalSim-0.1.dist-info/RECORD
-87 files, 705458 bytes uncompressed, 182903 bytes compressed:  74.1%
+-rw-rw-rw-  2.0 fat     1086 b- defN 24-May-07 09:57 DesalSim-0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     8363 b- defN 24-May-07 09:57 DesalSim-0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 09:57 DesalSim-0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       47 b- defN 24-May-07 09:57 DesalSim-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6266 b- defN 24-May-07 09:57 DesalSim-0.2.dist-info/RECORD
+74 files, 593182 bytes uncompressed, 156372 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -1,46 +1,7 @@
-Filename: Desalsim/__init__.py
-Comment: 
-
-Filename: Desalsim/constants.py
-Comment: 
-
-Filename: Desalsim/density_calc.py
-Comment: 
-
-Filename: Desalsim/economic_f.py
-Comment: 
-
-Filename: Desalsim/ed_unit_f.py
-Comment: 
-
-Filename: Desalsim/edbm_unit_f.py
-Comment: 
-
-Filename: Desalsim/efc_unit_f.py
-Comment: 
-
-Filename: Desalsim/med_unit_f.py
-Comment: 
-
-Filename: Desalsim/mfpfr_unit_f.py
-Comment: 
-
-Filename: Desalsim/nanofiltration_unit_f.py
-Comment: 
-
-Filename: Desalsim/ro_unit_f.py
-Comment: 
-
-Filename: Desalsim/scaleup.py
-Comment: 
-
-Filename: Desalsim/thermal_cryst_f.py
-Comment: 
-
 Filename: desalination_and_brine_treatment/__init__.py
 Comment: 
 
 Filename: desalination_and_brine_treatment/comparison.py
 Comment: 
 
 Filename: desalination_and_brine_treatment/constants.py
@@ -240,23 +201,23 @@
 
 Filename: tests/thermal_cryst_f.py
 Comment: 
 
 Filename: tests/thermal_cryst_unittest.py
 Comment: 
 
-Filename: DesalSim-0.1.dist-info/LICENSE
+Filename: DesalSim-0.2.dist-info/LICENSE
 Comment: 
 
-Filename: DesalSim-0.1.dist-info/METADATA
+Filename: DesalSim-0.2.dist-info/METADATA
 Comment: 
 
-Filename: DesalSim-0.1.dist-info/WHEEL
+Filename: DesalSim-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: DesalSim-0.1.dist-info/top_level.txt
+Filename: DesalSim-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: DesalSim-0.1.dist-info/RECORD
+Filename: DesalSim-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `DesalSim-0.1.dist-info/LICENSE` & `DesalSim-0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `DesalSim-0.1.dist-info/METADATA` & `DesalSim-0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DesalSim
-Version: 0.1
+Version: 0.2
 Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 Author: rodoulak
 Author-email: r.ktori@tudelft.nl
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy >=1.0
```

## Comparing `DesalSim-0.1.dist-info/RECORD` & `DesalSim-0.2.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Desalsim/__init__.py,sha256=PTAeBWx4Rx8k5hFLnPfZqmxQalze6anOFxEYCegjIjM,1128
-Desalsim/constants.py,sha256=7cJcZgjgj6VFC1zPFfGr12-e0BGa1_PEtupeUtpPuRc,1927
-Desalsim/density_calc.py,sha256=3RT1_-ma9jAzrU2ZdNBWcjcOYCmR3VehGP5OmHAmlAk,468
-Desalsim/economic_f.py,sha256=pJU2WlLoU1al-NcRp3_CFhnEPzlEQxP5_QKgMBanCPI,8821
-Desalsim/ed_unit_f.py,sha256=CyEIafmJIv0SVWmZQxX_0i1kn-2YjxILpdoZEc2XJU8,2950
-Desalsim/edbm_unit_f.py,sha256=9idaTDmzfsHqkRB6A7GIaMeF2MKd5MmpdD38H2Av8xs,11744
-Desalsim/efc_unit_f.py,sha256=mX74gp8FtwfW4yThfRGs1fn2hwsGjnyyigU3oFM8wuE,49286
-Desalsim/med_unit_f.py,sha256=ld_xlk_tZzktwYHWKSxfu36fzZoezqD4ShJz-27x5CU,4494
-Desalsim/mfpfr_unit_f.py,sha256=n_B1_RE4SA7W2GDOlxxR16BrGwb_waZ52S07f0ICoMU,10049
-Desalsim/nanofiltration_unit_f.py,sha256=AFLPNGJ7nqmVb9Y_-_ZQP6sADmuKOoA2fyQy8FFyqRQ,6987
-Desalsim/ro_unit_f.py,sha256=skzbsksmTKIzcfZ8rTjwkJS3P_3fdsgBn5QqOiYpsts,4366
-Desalsim/scaleup.py,sha256=NCVBeaOVfZECJuJLpxf_Agkk5AuPsWnr3CTkC_aGvwY,347
-Desalsim/thermal_cryst_f.py,sha256=d5dvWhAsm9ADr4bsPsF8gwipjHjdhYJzSI7rFdXyOwk,8692
 desalination_and_brine_treatment/__init__.py,sha256=PTAeBWx4Rx8k5hFLnPfZqmxQalze6anOFxEYCegjIjM,1128
 desalination_and_brine_treatment/comparison.py,sha256=_Pi9wfQTfgY-Hid2iKz-zM1dJqPVqTne8X2Xl2Ed2HY,4531
 desalination_and_brine_treatment/constants.py,sha256=7cJcZgjgj6VFC1zPFfGr12-e0BGa1_PEtupeUtpPuRc,1927
 desalination_and_brine_treatment/density_calc.py,sha256=3RT1_-ma9jAzrU2ZdNBWcjcOYCmR3VehGP5OmHAmlAk,468
 desalination_and_brine_treatment/economic_f.py,sha256=pJU2WlLoU1al-NcRp3_CFhnEPzlEQxP5_QKgMBanCPI,8821
 desalination_and_brine_treatment/ed_unit_f.py,sha256=CyEIafmJIv0SVWmZQxX_0i1kn-2YjxILpdoZEc2XJU8,2950
 desalination_and_brine_treatment/edbm_unit_f.py,sha256=9idaTDmzfsHqkRB6A7GIaMeF2MKd5MmpdD38H2Av8xs,11744
@@ -76,12 +63,12 @@
 tests/mfpfr_unit_f.py,sha256=vEbbH6V7UzNxNZg9jHJT0QsobxS-N-mx_ys_ISnRpZA,10407
 tests/mfpfr_unittest.py,sha256=45mJ1iH0ezXhB5-Y2r92uIuMbRsqOjmZyp6AHSVQg7k,2743
 tests/nanofiltration_unit_f.py,sha256=91aP0t_2rUYv9xRVAml-gnEU8cF8sdOJaAVJVcuXymc,6961
 tests/nanofiltration_unittest.py,sha256=hT2KWWdXM0tCAgoOsBn0qh02AG_dotjG9tubjkPagcQ,1777
 tests/scaleup.py,sha256=NCVBeaOVfZECJuJLpxf_Agkk5AuPsWnr3CTkC_aGvwY,347
 tests/thermal_cryst_f.py,sha256=R8qlJdDFaF-qF68Ky8bTxcIgcTRmHcKZJ_44G0flW7I,8687
 tests/thermal_cryst_unittest.py,sha256=lj_DodwF9QyUFOv1q3ELT4GxDtrnYEK_LzqL-FIeWE8,4560
-DesalSim-0.1.dist-info/LICENSE,sha256=hYDXcn5byxqE0AMzS0g6beaQ-dAB9-KzchUVrXPrnsI,1086
-DesalSim-0.1.dist-info/METADATA,sha256=YUZheS3mcqxx_7SeDNqkAmxUKpbqzxPcKtIA5F-Jrus,8363
-DesalSim-0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-DesalSim-0.1.dist-info/top_level.txt,sha256=SpyYtI7MSf-XBey9zpWO4QpgbaK4i1M7z7DaaGMNHM8,23
-DesalSim-0.1.dist-info/RECORD,,
+DesalSim-0.2.dist-info/LICENSE,sha256=hYDXcn5byxqE0AMzS0g6beaQ-dAB9-KzchUVrXPrnsI,1086
+DesalSim-0.2.dist-info/METADATA,sha256=SnzabGL0kZckxH2zShpXdRMdrg_FJ1_2LRtBhcsBGCU,8363
+DesalSim-0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+DesalSim-0.2.dist-info/top_level.txt,sha256=C3I_jRcPfO7PKHcAoAr2lTCaKYyCjXbj-9HN4TfYFHY,47
+DesalSim-0.2.dist-info/RECORD,,
```

