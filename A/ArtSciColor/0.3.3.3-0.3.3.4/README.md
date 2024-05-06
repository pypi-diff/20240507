# Comparing `tmp/ArtSciColor-0.3.3.3.tar.gz` & `tmp/ArtSciColor-0.3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ArtSciColor-0.3.3.3.tar", last modified: Fri Mar 29 15:57:34 2024, max compression
+gzip compressed data, was "ArtSciColor-0.3.3.4.tar", last modified: Mon May  6 22:57:35 2024, max compression
```

## Comparing `ArtSciColor-0.3.3.3.tar` & `ArtSciColor-0.3.3.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-03-29 15:57:34.389800 ArtSciColor-0.3.3.3/
-drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-03-29 15:57:34.387879 ArtSciColor-0.3.3.3/ArtSciColor/
--rw-r--r--   0 chipdelmal   (501) staff       (20)      246 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.3/ArtSciColor/__init__.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)       23 2024-03-29 15:57:34.000000 ArtSciColor-0.3.3.3/ArtSciColor/_version.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     2574 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.3/ArtSciColor/auxiliary.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     2770 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.3/ArtSciColor/color.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     2736 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.3/ArtSciColor/constants.py
-drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-03-29 15:57:34.389024 ArtSciColor-0.3.3.3/ArtSciColor/data/
--rw-r--r--   0 chipdelmal   (501) staff       (20)    19020 2024-03-29 15:57:04.000000 ArtSciColor-0.3.3.3/ArtSciColor/data/DB.bz
--rw-r--r--   0 chipdelmal   (501) staff       (20)    53787 2024-03-29 15:57:04.000000 ArtSciColor-0.3.3.3/ArtSciColor/data/DB.csv
--rw-r--r--   0 chipdelmal   (501) staff       (20)     9572 2024-03-29 15:57:27.000000 ArtSciColor-0.3.3.3/ArtSciColor/data/SWATCHES.bz
--rw-r--r--   0 chipdelmal   (501) staff       (20)     8601 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.3/ArtSciColor/fingerprint.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     1425 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.3/ArtSciColor/fingerprintWrappers.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     1758 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.3/ArtSciColor/image.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     1097 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.3/ArtSciColor/paths.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)      355 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.3/ArtSciColor/superscale.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     1160 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.3/ArtSciColor/swatches.py
-drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-03-29 15:57:34.388627 ArtSciColor-0.3.3.3/ArtSciColor.egg-info/
--rw-r--r--   0 chipdelmal   (501) staff       (20)     7164 2024-03-29 15:57:34.000000 ArtSciColor-0.3.3.3/ArtSciColor.egg-info/PKG-INFO
--rw-r--r--   0 chipdelmal   (501) staff       (20)      549 2024-03-29 15:57:34.000000 ArtSciColor-0.3.3.3/ArtSciColor.egg-info/SOURCES.txt
--rw-r--r--   0 chipdelmal   (501) staff       (20)        1 2024-03-29 15:57:34.000000 ArtSciColor-0.3.3.3/ArtSciColor.egg-info/dependency_links.txt
--rw-r--r--   0 chipdelmal   (501) staff       (20)      115 2024-03-29 15:57:34.000000 ArtSciColor-0.3.3.3/ArtSciColor.egg-info/requires.txt
--rw-r--r--   0 chipdelmal   (501) staff       (20)       12 2024-03-29 15:57:34.000000 ArtSciColor-0.3.3.3/ArtSciColor.egg-info/top_level.txt
--rw-r--r--   0 chipdelmal   (501) staff       (20)    35149 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.3/LICENSE
--rw-r--r--   0 chipdelmal   (501) staff       (20)     7164 2024-03-29 15:57:34.389484 ArtSciColor-0.3.3.3/PKG-INFO
--rw-r--r--   0 chipdelmal   (501) staff       (20)     6442 2024-03-27 23:57:54.000000 ArtSciColor-0.3.3.3/README.md
--rw-r--r--   0 chipdelmal   (501) staff       (20)       38 2024-03-29 15:57:34.389846 ArtSciColor-0.3.3.3/setup.cfg
--rw-r--r--   0 chipdelmal   (501) staff       (20)     1722 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.3/setup.py
+drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-05-06 22:57:35.670656 ArtSciColor-0.3.3.4/
+drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-05-06 22:57:35.668533 ArtSciColor-0.3.3.4/ArtSciColor/
+-rw-r--r--   0 chipdelmal   (501) staff       (20)      246 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.4/ArtSciColor/__init__.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)       23 2024-05-06 22:57:35.000000 ArtSciColor-0.3.3.4/ArtSciColor/_version.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     2574 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.4/ArtSciColor/auxiliary.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     2770 2024-04-01 23:37:06.000000 ArtSciColor-0.3.3.4/ArtSciColor/color.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     2736 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.4/ArtSciColor/constants.py
+drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-05-06 22:57:35.669820 ArtSciColor-0.3.3.4/ArtSciColor/data/
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    19215 2024-05-06 22:57:07.000000 ArtSciColor-0.3.3.4/ArtSciColor/data/DB.bz
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    54263 2024-05-06 22:57:07.000000 ArtSciColor-0.3.3.4/ArtSciColor/data/DB.csv
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     9682 2024-05-06 22:57:30.000000 ArtSciColor-0.3.3.4/ArtSciColor/data/SWATCHES.bz
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     8601 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.4/ArtSciColor/fingerprint.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     1425 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.4/ArtSciColor/fingerprintWrappers.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     1758 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.4/ArtSciColor/image.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     1097 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.4/ArtSciColor/paths.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)      355 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.4/ArtSciColor/superscale.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     1160 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.4/ArtSciColor/swatches.py
+drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-05-06 22:57:35.669388 ArtSciColor-0.3.3.4/ArtSciColor.egg-info/
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     7164 2024-05-06 22:57:35.000000 ArtSciColor-0.3.3.4/ArtSciColor.egg-info/PKG-INFO
+-rw-r--r--   0 chipdelmal   (501) staff       (20)      549 2024-05-06 22:57:35.000000 ArtSciColor-0.3.3.4/ArtSciColor.egg-info/SOURCES.txt
+-rw-r--r--   0 chipdelmal   (501) staff       (20)        1 2024-05-06 22:57:35.000000 ArtSciColor-0.3.3.4/ArtSciColor.egg-info/dependency_links.txt
+-rw-r--r--   0 chipdelmal   (501) staff       (20)      115 2024-05-06 22:57:35.000000 ArtSciColor-0.3.3.4/ArtSciColor.egg-info/requires.txt
+-rw-r--r--   0 chipdelmal   (501) staff       (20)       12 2024-05-06 22:57:35.000000 ArtSciColor-0.3.3.4/ArtSciColor.egg-info/top_level.txt
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    35149 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.4/LICENSE
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     7164 2024-05-06 22:57:35.670301 ArtSciColor-0.3.3.4/PKG-INFO
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     6442 2024-03-27 23:57:54.000000 ArtSciColor-0.3.3.4/README.md
+-rw-r--r--   0 chipdelmal   (501) staff       (20)       38 2024-05-06 22:57:35.670700 ArtSciColor-0.3.3.4/setup.cfg
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     1722 2024-02-19 01:32:34.000000 ArtSciColor-0.3.3.4/setup.py
```

### Comparing `ArtSciColor-0.3.3.3/ArtSciColor/auxiliary.py` & `ArtSciColor-0.3.3.4/ArtSciColor/auxiliary.py`

 * *Files identical despite different names*

### Comparing `ArtSciColor-0.3.3.3/ArtSciColor/color.py` & `ArtSciColor-0.3.3.4/ArtSciColor/color.py`

 * *Files identical despite different names*

### Comparing `ArtSciColor-0.3.3.3/ArtSciColor/constants.py` & `ArtSciColor-0.3.3.4/ArtSciColor/constants.py`

 * *Files identical despite different names*

### Comparing `ArtSciColor-0.3.3.3/ArtSciColor/data/DB.csv` & `ArtSciColor-0.3.3.4/ArtSciColor/data/DB.csv`

 * *Files 0% similar despite different names*

```diff
@@ -307,27 +307,30 @@
 VanGogh,"""Starry Night""","#1A1D1C,#2B3853,#637C94,#737E63,#A2AA91,#3E5682",9B381C78A14EF84DA14C,6,AgglomerativeClustering,https://www.wikiart.org/en/vincent-van-gogh/the-starry-night-1889,183461.png
 Warhol,"""Flowers""","#2A3219,#8BCFD0,#FF9293,#7CA33B,#A54E91",4A99CCAC4382E886AF03,5,AgglomerativeClustering,https://www.nga.gov/collection/art-object-page.144934.html,183385.png
 Warhol,"""Portraits of the Artists""","#1E1414,#163D3C,#558070,#BDB1AB,#F2F2F2,#C39021,#7F5D19",4813F188B626AA278E1E,7,AgglomerativeClustering,https://www.nga.gov/collection/art-object-page.136329.html,183384.png
 chipdelmal,Maps,"#75393E,#58586B,#9BBFCE,#F0E6D9,#FAF9F9",50B5EF4C1FA7176BFAA2,5,None,https://chipdelmal.github.io/,None
 chipdelmal,Motherland,"#F72585,#2614ED,#5DDEB1,#F038FF,#E2EF70,#9381FF",55337043132A3AD872D7,6,None,https://chipdelmal.github.io/,None
 chipdelmal,Muted,"#02AD9A,#B36FA0,#E16D5D,#E84E73,#C8C4E4,#89C074,#6F566B,#FF9293,#1541AE,#9DB4AF",A76B606323F453C37FC6,10,None,https://chipdelmal.github.io/,None
 chipdelmal,Pastel,"#A0C4FF,#E0C3FC,#FFD6A5,#CAFFBF,#D0D1FF",EF69F32ECABBBA994F39,5,None,https://chipdelmal.github.io/,None
+chipdelmal,Risk Levels,"#FFF,#DEFFD7,#D3F6B8,#E9E1A7,#F7C176,#FF9E50,#FF7A4C,#F25655,#DA3263,#B21D71,#711676",F65C5DBE94D9C2799D26,11,None,https://chipdelmal.github.io/,None
 coolors,Blue-Brown,"#9381FF,#B8B8FF,#F8F7FF,#FED,#FFD8BE",73E965B0E644BA4427A1,5,None,https://coolors.co/palette/9381ff-b8b8ff-f8f7ff-ffeedd-ffd8be,None
 coolors,Blue-Pink,"#2D00F7,#6A00F4,#8900F2,#A100F2,#B100E8,#BC00DD,#D100D1,#DB00B6,#E500A4,#F20089",166EA4EC4BC2A8592EB1,10,None,https://coolors.co/palette/2d00f7-6a00f4-8900f2-a100f2-b100e8-bc00dd-d100d1-db00b6-e500a4-f20089,None
 coolors,Blues,"#0A369D,#4472CA,#5E7CE2,#92B4F4,#CFDEE7",C945CDEA9050AC581A03,5,None,https://coolors.co/palette/0a369d-4472ca-5e7ce2-92b4f4-cfdee7,None
 coolors,California Coast,"#49A596,#86C3B4,#C8DCC3,#F0E1C5,#BAD2DD",7BF3D1049B1B1E054856,5,None,https://www.color-hex.com/color-palette/10908,None
 coolors,California English,"#875346,#F5565B,#FB9274,#F7E4C6,#CDDBC2",F24EF0EF74502BCBC26D,5,None,https://www.color-hex.com/color-palette/2895,None
 coolors,California Sunset,"#EA4073,#EA8246,#EAB42E,#ECD915,#8AC2E5",390DD776D793067EEFB2,5,None,https://www.schemecolor.com/california-sunset.php,None
 coolors,California Wine Sunset,"#1E1A75,#A11477,#E13661,#FF6F4B,#FFA951",F9F87A79C88892581071,5,None,https://www.color-hex.com/color-palette/107525,None
 coolors,Divergent,"#0FA3B1,#B5E2FA,#F9F7F3,#EDDEA4,#F7A072",74C64062DA28140FCD21,5,None,https://coolors.co/0fa3b1-b5e2fa-f9f7f3-eddea4-f7a072,None
+coolors,Dusty Sunset,"#BE6F6F,#DA9B88,#E9C3AE,#E9D9B9,#B5AED2,#9979AC",71D28E13607886972B0F,6,None,https://www.schemecolor.com/dusty-sunset.php,None
+coolors,Gentle Sunset,"#DDC4F7,#F1D4FA,#FDB0C5,#FB8CAA,#9550A3",5B5CB596DC453AF06D5F,5,None,https://www.schemecolor.com/gentle-sunset-color-combination.php,None
 coolors,Light Sunset,"#9492AD,#A9A7BC,#C6B6C0,#DFCCC8,#F4DBC5,#FDF6EE",2E2A3C6C7EC58431F8A7,6,None,https://www.schemecolor.com/light-sunset.php,None
 coolors,Pastel,"#D8E2DC,#FFE5D9,#FFCAD4,#F4ACB7,#9D8189",EA8FA562E72404DCD56D,5,None,https://coolors.co/palette/d8e2dc-ffe5d9-ffcad4-f4acb7-9d8189,None
 coolors,Pastel Galaxy,"#C1D0F9,#D6F6F6,#FBFBF7,#FEF0FB,#FEDEF7,#E1CCEE",241F760B69F5EB165706,6,None,https://www.schemecolor.com/pastel-galaxy.php,None
 coolors,Pastel Leaves,"#B199BF,#E6AFC3,#FFCC9C,#FEEEB9,#C5D9AB",9E79A68593686AF29781,5,None,https://www.schemecolor.com/pastel-leaves.php,None
-coolors,Pastels of Blue & Violet,"#A2A2E0,#C9B4ED,#DFCCED,#BFD9FF,#BFD9FF,#AAC4F2",AA283C907CA536A43862,6,None,https://www.schemecolor.com/pastels-of-blue-violet.php,None
+coolors,Pastels of Blue & Violet,"#A2A2E0,#C9B4ED,#DFCCED,#BFD9FF,#AAC4F2",AA283C907CA536A43862,5,None,https://www.schemecolor.com/pastels-of-blue-violet.php,None
 coolors,Pink-Blue,"#FF499E,#D264B6,#A480CF,#779BE7,#49B6FF",CF85BE8342E9BDA5CF59,5,None,https://coolors.co/palette/ff499e-d264b6-a480cf-779be7-49b6ff,None
 coolors,Soft Unicorn,"#D4C4E9,#EED3E5,#F7E7DC,#F4F3EA,#C2CBE4,#C0DEDA",C933FB9E8771E5CE7988,6,None,https://www.schemecolor.com/soft-unicorn-2.php,None
 coolors,Sunset Beach Music,"#6B41BF,#A25ED9,#F978A7,#FFBA5E,#EC835C,#C83F53",6A6B50126CB783C65BEA,6,None,https://www.schemecolor.com/sunset-beach-music.php,None
 coolors,Wine,"#FFCDB2,#FFB4A2,#E5989B,#B5838D,#6D6875",111D7E0E6C7ED8EDB41F,5,None,https://coolors.co/palette/ffcdb2-ffb4a2-e5989b-b5838d-6d6875,None
 lospec,Ammo,"#040C06,#112318,#1E3A29,#305D42,#4D8061,#89A257,#BEDC7F,#EFC",6BFDE5C8F3896AFDC4A6,8,None,https://lospec.com/palette-list/ammo-8,None
 lospec,Blessing,"#74569B,#96FBC7,#F7FFAE,#FFB3CB,#D8BFD8",EF25353485DA196E4155,5,None,https://lospec.com/palette-list/blessing,None
 lospec,CoolWood,"#372E4D,#5F699C,#65AED6,#A4EBCC,#EFFAE6,#F0B38D,#B56D7F,#614363",F834AC5977233DA080F6,8,None,https://lospec.com/palette-list/coldwood8,None
```

### Comparing `ArtSciColor-0.3.3.3/ArtSciColor/fingerprint.py` & `ArtSciColor-0.3.3.4/ArtSciColor/fingerprint.py`

 * *Files identical despite different names*

### Comparing `ArtSciColor-0.3.3.3/ArtSciColor/fingerprintWrappers.py` & `ArtSciColor-0.3.3.4/ArtSciColor/fingerprintWrappers.py`

 * *Files identical despite different names*

### Comparing `ArtSciColor-0.3.3.3/ArtSciColor/image.py` & `ArtSciColor-0.3.3.4/ArtSciColor/image.py`

 * *Files identical despite different names*

### Comparing `ArtSciColor-0.3.3.3/ArtSciColor/paths.py` & `ArtSciColor-0.3.3.4/ArtSciColor/paths.py`

 * *Files identical despite different names*

### Comparing `ArtSciColor-0.3.3.3/ArtSciColor/swatches.py` & `ArtSciColor-0.3.3.4/ArtSciColor/swatches.py`

 * *Files identical despite different names*

### Comparing `ArtSciColor-0.3.3.3/ArtSciColor.egg-info/PKG-INFO` & `ArtSciColor-0.3.3.4/ArtSciColor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArtSciColor
-Version: 0.3.3.3
+Version: 0.3.3.4
 Summary: Color palettes for scientific purposes
 Home-page: https://github.com/Chipdelmal/ArtSciColor
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ArtSciColor Version: 0.3.3.3 Summary: Color
+Metadata-Version: 2.1 Name: ArtSciColor Version: 0.3.3.4 Summary: Color
 palettes for scientific purposes Home-page: https://github.com/Chipdelmal/
 ArtSciColor Author: chipdelmal Author-email: chipdelmal@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: matplotlib>=3.3.2 Requires-Dist: colour>=0.1.5 Requires-
 Dist: colorir Requires-Dist: Pillow Requires-Dist: opencv-python Requires-Dist:
```

### Comparing `ArtSciColor-0.3.3.3/ArtSciColor.egg-info/SOURCES.txt` & `ArtSciColor-0.3.3.4/ArtSciColor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ArtSciColor-0.3.3.3/LICENSE` & `ArtSciColor-0.3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ArtSciColor-0.3.3.3/PKG-INFO` & `ArtSciColor-0.3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArtSciColor
-Version: 0.3.3.3
+Version: 0.3.3.4
 Summary: Color palettes for scientific purposes
 Home-page: https://github.com/Chipdelmal/ArtSciColor
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ArtSciColor Version: 0.3.3.3 Summary: Color
+Metadata-Version: 2.1 Name: ArtSciColor Version: 0.3.3.4 Summary: Color
 palettes for scientific purposes Home-page: https://github.com/Chipdelmal/
 ArtSciColor Author: chipdelmal Author-email: chipdelmal@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: matplotlib>=3.3.2 Requires-Dist: colour>=0.1.5 Requires-
 Dist: colorir Requires-Dist: Pillow Requires-Dist: opencv-python Requires-Dist:
```

### Comparing `ArtSciColor-0.3.3.3/README.md` & `ArtSciColor-0.3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ArtSciColor-0.3.3.3/setup.py` & `ArtSciColor-0.3.3.4/setup.py`

 * *Files identical despite different names*

