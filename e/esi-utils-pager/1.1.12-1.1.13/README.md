# Comparing `tmp/esi_utils_pager-1.1.12.tar.gz` & `tmp/esi_utils_pager-1.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esi_utils_pager-1.1.12.tar", last modified: Tue Apr 30 15:41:35 2024, max compression
+gzip compressed data, was "esi_utils_pager-1.1.13.tar", last modified: Tue May  7 17:13:47 2024, max compression
```

## Comparing `esi_utils_pager-1.1.12.tar` & `esi_utils_pager-1.1.13.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:41:35.478279 esi_utils_pager-1.1.12/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/LICENSE.md
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     8128 2024-04-30 15:41:35.478279 esi_utils_pager-1.1.12/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4988 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1254 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-04-30 15:41:35.478279 esi_utils_pager-1.1.12/setup.cfg
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:41:35.466279 esi_utils_pager-1.1.12/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:41:35.466279 esi_utils_pager-1.1.12/src/esi_utils_pager/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:41:35.470279 esi_utils_pager-1.1.12/src/esi_utils_pager/bin/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     9973 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/bin/pagerlite.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10037 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/calc.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2629 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/config.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4444 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/country.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:41:35.478279 esi_utils_pager-1.1.12/src/esi_utils_pager/data/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   288256 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   366080 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   974848 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    44597 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/countries.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    54009 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/economic.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/economy.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    33076 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/fatality.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/fatality.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   176744 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_casualty.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   218436 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_casualty.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   260968 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_collapse_mmi.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   198134 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_collapse_mmi.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)  1006280 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_inventory.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   290497 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_inventory.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27120 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_workforce.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14527 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_workforce.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7424 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/econexposure.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24334 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/emploss.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8367 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/exposure.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7078 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/growth.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      422 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/pandas_container.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2467 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/probs.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27500 2024-04-30 15:40:23.000000 esi_utils_pager-1.1.12/src/esi_utils_pager/semimodel.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-30 15:41:35.478279 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     8128 2024-04-30 15:41:35.000000 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1441 2024-04-30 15:41:35.000000 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-04-30 15:41:35.000000 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       65 2024-04-30 15:41:35.000000 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/entry_points.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      281 2024-04-30 15:41:35.000000 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       16 2024-04-30 15:41:35.000000 esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:13:47.591933 esi_utils_pager-1.1.13/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/LICENSE.md
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)    10517 2024-05-07 17:13:47.591933 esi_utils_pager-1.1.13/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7377 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1254 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-05-07 17:13:47.591933 esi_utils_pager-1.1.13/setup.cfg
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:13:47.575933 esi_utils_pager-1.1.13/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:13:47.579933 esi_utils_pager-1.1.13/src/esi_utils_pager/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:12:39.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:13:47.583933 esi_utils_pager-1.1.13/src/esi_utils_pager/bin/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    10661 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/bin/pagerlite.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11717 2024-05-07 16:55:36.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/calc.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2629 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/config.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4444 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/country.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:13:47.587933 esi_utils_pager-1.1.13/src/esi_utils_pager/data/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   288256 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   366080 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   974848 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    44597 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/countries.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    54009 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/economic.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/economy.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    33076 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/fatality.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/fatality.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   176744 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_casualty.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   218436 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_casualty.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   260968 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_collapse_mmi.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   198134 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_collapse_mmi.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)  1006280 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_inventory.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   290497 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_inventory.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27120 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_workforce.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14527 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_workforce.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7424 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/econexposure.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24334 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/emploss.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8367 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/exposure.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7078 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/growth.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      422 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/pandas_container.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2467 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/probs.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27500 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/semimodel.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:13:47.587933 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)    10517 2024-05-07 17:13:47.000000 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1441 2024-05-07 17:13:47.000000 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-05-07 17:13:47.000000 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       65 2024-05-07 17:13:47.000000 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/entry_points.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      281 2024-05-07 17:13:47.000000 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       16 2024-05-07 17:13:47.000000 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/top_level.txt
```

### Comparing `esi_utils_pager-1.1.12/LICENSE.md` & `esi_utils_pager-1.1.13/LICENSE.md`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/PKG-INFO` & `esi_utils_pager-1.1.13/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-utils-pager
-Version: 1.1.12
+Version: 1.1.13
 Summary: USGS PAGER loss modeling functionality
 Author-email: Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -153,53 +153,107 @@
   - {population_grid: /data/pagerdata/model_data/population/lspop2018.flt, population_year: 2018}
   urban_rural_grid: /data/pagerdata/model_data/glurextents.bil
 ```
 
 
 # Command Line Usage
 The command line program made available by this repository is `pagerlite`. This program outputs detailed empirical
-(fatality/economic) PAGER model results to a tabular format. To see the help for this program:
+(fatality/economic) PAGER model results to a tabular format. The help for this program (`pagerlite -h`):
 
-`pagerlite -h`
+```
+positional arguments:
+  {event,batch}         Sub-commands are available below.
+    event               Run a single event through pagerlite
+    batch               Run many events through pagerlite
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -s, --run-semi        Calculate semi-empirical model results as well.
+  -o OUTFILE, --outfile OUTFILE
+                        Specify output file (.xlsx for Excel, .csv for CSV)
+  -v, --verbose         Print progress output to the screen
+  -f FATALITY_FILE, --fatality-file FATALITY_FILE
+                        Path to custom fatality Excel file
+  -e ECONOMIC_FILE, --economic-file ECONOMIC_FILE
+                        Path to custom economic Excel file
+  --semi-folder SEMI_FOLDER
+                        Path to folder containing custom semi-empirical Excel files. These files MUST be named
+                        semi_inventory.xlsx, semi_collapse_mmi.xlsx, semi_casualty.xlsx and semi_workforce.xlsx.
+```
 
-There are three input modes for pagerlite:
+There are two subcommands for pagerlite:
 
- - `pagerlite -e <eventid>` Run pagerlite on a single event specified by a ComCat event ID.
- - `pagerlite -g <grid.xml>` Run pagerlite on a single grid.xml file.
- - `pagerlite -f <gridfolder>` Run pagerlite on a directory containing many grid.xml files 
+ - `pagerlite event` Run on a single event specified by ComCat event ID OR path to grid.xml.
+ - `pagerlite batch` Run pagerlite on a directory containing many grid.xml files 
     (these files can be in sub-directories).
 
+The event subcommand is straightforward (`pagerlite event -h`):
+
+```
+usage: pagerlite event [-h] file_or_url
+
+positional arguments:
+  file_or_url  Path to local ShakeMap grid XML OR ComCat event ID.
+
+optional arguments:
+  -h, --help   show this help message and exit
+```
+
+The `batch` subcommand has a number of optional arguments (`pagerlite batch -h`):
+
+```
+usage: pagerlite batch [-h] [-f FOLDER] [-t TIME_RANGE TIME_RANGE] [-b lonmin lonmax latmin latmax]
+                       [-d depthmin depthmax] [-m minmag maxmag]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -f FOLDER, --folder FOLDER
+                        A folder containing many ShakeMap *grid.xml files.
+  -t TIME_RANGE TIME_RANGE, --time-range TIME_RANGE TIME_RANGE
+                        Only process events within given time range.
+  -b lonmin lonmax latmin latmax, --bounds lonmin lonmax latmin latmax
+                        Only process events within spatial boundary [lonmin lonmax latmin latmax].
+  -d depthmin depthmax, --depth-range depthmin depthmax
+                        Only process events within depth range [depthmin depthmax].
+  -m minmag maxmag, --mag-range minmag maxmag
+                        Minimum and maximum (authoritative) magnitude to restrict search.
+```
+
 ## Examples
 
 To run the PAGER empirical models *only* on a ShakeMap grid.xml file in the current directory and write the results to an Excel file:
 
-`pagerlite -g grid.xml -o output.xlsx`
+`pagerlite -o output.xlsx event grid.xml`
 
 To run the PAGER empirical models *only* on a directory containing (potentially) many sub-directories with 
 files ending in "grid.xml":
 
-`pagerlite -f /data/shakemap_output/ -o output.xlsx`
+`pagerlite -o output.xlsx batch -f /data/shakemap_output/`
 
 To run the PAGER empirical models *only* on a ComCat event ID (this will download the authoritative 
 ShakeMap grid.xml file from ComCat):
 
-`pagerlite -e us7000lz23 -o output.xlsx`
+`pagerlite -o output.xlsx batch us7000lz23 `
 
 To run the PAGER empirical AND semi-empirical models, simply add the `-s` flag to any of the above commands:
 
-`pagerlite -e us7000lz23 -s -o output.xlsx`
+`pagerlite -s -o output.xlsx batch us7000lz23`
 
 To run the PAGER empirical models on a folder but only for events between 2010 and 2017:
 
-`pagerlite -f /data/shakemap_output/ -t 2010-01-01 2017-12-31T23:59:59 -o output.xlsx`
+`pagerlite -o output.xlsx batch -f /data/shakemap_output/ -t 2010-01-01 2017-12-31T23:59:59`
+
+To run PAGER empirical models on a folder but only for events in Japan:
+`pagerlite -o output.xlsx batch -f /data/shakemap_output/ -b 30.844021 44.762578 128.336525  149.031827`
 
-See the help for more options (spatial bounds and magnitude range) on restricting processing of ShakeMap
+See the help for more options (depth and magnitude ranges) on restricting processing of ShakeMap
 grids.
 
 
 
+
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi_utils_pager-1.1.12/README.md` & `esi_utils_pager-1.1.13/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -69,53 +69,107 @@
   - {population_grid: /data/pagerdata/model_data/population/lspop2018.flt, population_year: 2018}
   urban_rural_grid: /data/pagerdata/model_data/glurextents.bil
 ```
 
 
 # Command Line Usage
 The command line program made available by this repository is `pagerlite`. This program outputs detailed empirical
-(fatality/economic) PAGER model results to a tabular format. To see the help for this program:
+(fatality/economic) PAGER model results to a tabular format. The help for this program (`pagerlite -h`):
 
-`pagerlite -h`
+```
+positional arguments:
+  {event,batch}         Sub-commands are available below.
+    event               Run a single event through pagerlite
+    batch               Run many events through pagerlite
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -s, --run-semi        Calculate semi-empirical model results as well.
+  -o OUTFILE, --outfile OUTFILE
+                        Specify output file (.xlsx for Excel, .csv for CSV)
+  -v, --verbose         Print progress output to the screen
+  -f FATALITY_FILE, --fatality-file FATALITY_FILE
+                        Path to custom fatality Excel file
+  -e ECONOMIC_FILE, --economic-file ECONOMIC_FILE
+                        Path to custom economic Excel file
+  --semi-folder SEMI_FOLDER
+                        Path to folder containing custom semi-empirical Excel files. These files MUST be named
+                        semi_inventory.xlsx, semi_collapse_mmi.xlsx, semi_casualty.xlsx and semi_workforce.xlsx.
+```
 
-There are three input modes for pagerlite:
+There are two subcommands for pagerlite:
 
- - `pagerlite -e <eventid>` Run pagerlite on a single event specified by a ComCat event ID.
- - `pagerlite -g <grid.xml>` Run pagerlite on a single grid.xml file.
- - `pagerlite -f <gridfolder>` Run pagerlite on a directory containing many grid.xml files 
+ - `pagerlite event` Run on a single event specified by ComCat event ID OR path to grid.xml.
+ - `pagerlite batch` Run pagerlite on a directory containing many grid.xml files 
     (these files can be in sub-directories).
 
+The event subcommand is straightforward (`pagerlite event -h`):
+
+```
+usage: pagerlite event [-h] file_or_url
+
+positional arguments:
+  file_or_url  Path to local ShakeMap grid XML OR ComCat event ID.
+
+optional arguments:
+  -h, --help   show this help message and exit
+```
+
+The `batch` subcommand has a number of optional arguments (`pagerlite batch -h`):
+
+```
+usage: pagerlite batch [-h] [-f FOLDER] [-t TIME_RANGE TIME_RANGE] [-b lonmin lonmax latmin latmax]
+                       [-d depthmin depthmax] [-m minmag maxmag]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -f FOLDER, --folder FOLDER
+                        A folder containing many ShakeMap *grid.xml files.
+  -t TIME_RANGE TIME_RANGE, --time-range TIME_RANGE TIME_RANGE
+                        Only process events within given time range.
+  -b lonmin lonmax latmin latmax, --bounds lonmin lonmax latmin latmax
+                        Only process events within spatial boundary [lonmin lonmax latmin latmax].
+  -d depthmin depthmax, --depth-range depthmin depthmax
+                        Only process events within depth range [depthmin depthmax].
+  -m minmag maxmag, --mag-range minmag maxmag
+                        Minimum and maximum (authoritative) magnitude to restrict search.
+```
+
 ## Examples
 
 To run the PAGER empirical models *only* on a ShakeMap grid.xml file in the current directory and write the results to an Excel file:
 
-`pagerlite -g grid.xml -o output.xlsx`
+`pagerlite -o output.xlsx event grid.xml`
 
 To run the PAGER empirical models *only* on a directory containing (potentially) many sub-directories with 
 files ending in "grid.xml":
 
-`pagerlite -f /data/shakemap_output/ -o output.xlsx`
+`pagerlite -o output.xlsx batch -f /data/shakemap_output/`
 
 To run the PAGER empirical models *only* on a ComCat event ID (this will download the authoritative 
 ShakeMap grid.xml file from ComCat):
 
-`pagerlite -e us7000lz23 -o output.xlsx`
+`pagerlite -o output.xlsx batch us7000lz23 `
 
 To run the PAGER empirical AND semi-empirical models, simply add the `-s` flag to any of the above commands:
 
-`pagerlite -e us7000lz23 -s -o output.xlsx`
+`pagerlite -s -o output.xlsx batch us7000lz23`
 
 To run the PAGER empirical models on a folder but only for events between 2010 and 2017:
 
-`pagerlite -f /data/shakemap_output/ -t 2010-01-01 2017-12-31T23:59:59 -o output.xlsx`
+`pagerlite -o output.xlsx batch -f /data/shakemap_output/ -t 2010-01-01 2017-12-31T23:59:59`
+
+To run PAGER empirical models on a folder but only for events in Japan:
+`pagerlite -o output.xlsx batch -f /data/shakemap_output/ -b 30.844021 44.762578 128.336525  149.031827`
 
-See the help for more options (spatial bounds and magnitude range) on restricting processing of ShakeMap
+See the help for more options (depth and magnitude ranges) on restricting processing of ShakeMap
 grids.
 
 
 
+
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi_utils_pager-1.1.12/pyproject.toml` & `esi_utils_pager-1.1.13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/bin/pagerlite.py` & `esi_utils_pager-1.1.13/src/esi_utils_pager/bin/pagerlite.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 import tempfile
 from datetime import datetime
 from urllib.request import urlopen
 
 # third party imports
 import numpy as np
 import pandas as pd
-import rasterio
 
 # local imports
 from esi_utils_pager.calc import calc_pager_event, calc_pager_events
-from esi_utils_pager.config import read_config
+from esi_utils_pager.config import get_config_file, read_config
+from mapio.shake import getHeaderData
 
 EVENT_TEMPLATE = (
     "https://earthquake.usgs.gov/earthquakes/feed/v1.0/detail/{eventid}.geojson"
 )
 
 TIMEFMT1 = "%Y-%m-%dT%H:%M:%S"
 TIMEFMT2 = "%Y-%m-%dT%H:%M:%S.%f"
@@ -39,14 +39,144 @@
             try:
                 outtime = datetime.strptime(timestring, DATEFMT)
             except Exception:
                 raise Exception("Could not parse time or date from %s" % timestring)
     return outtime
 
 
+def set_logging(args):
+    if args.verbose:
+        loglevel = logging.INFO
+    else:
+        loglevel = logging.CRITICAL
+    logging.basicConfig(
+        level=loglevel,
+        format="%(asctime)s %(message)s",
+        handlers=[logging.StreamHandler()],
+    )
+
+
+def check_input_files(args):
+    # check to make sure that any input fatality/econ/semi files/folders actually exist
+    file_errors = []
+
+    if args.fatality_file is not None:
+        fatpath = pathlib.Path(args.fatality).resolve()
+        if not fatpath.exists():
+            file_errors.append(f"Input file {fatpath} does not exist.")
+
+    if args.economic_file is not None:
+        ecopath = pathlib.Path(args.economic).resolve()
+        if not ecopath.exists():
+            file_errors.append(f"Input file {ecopath} does not exist.")
+
+    if args.semi_folder is not None:
+        semipath = pathlib.Path(args.semi_folder).resolve()
+        if not semipath.exists() or not semipath.is_dir():
+            file_errors.append(
+                f"Input file {semipath} does not exist or is not a directory."
+            )
+        else:
+            inventory_file = semipath / "semi_inventory.xlsx"
+            collapse_file = semipath / "semi_collapse_mmi.xlsx"
+            casualty_file = semipath / "semi_casualty.xlsx"
+            workforce_file = semipath / "semi_workforce.xlsx"
+            files_present = 0
+            files_present += int(inventory_file.exists())
+            files_present += int(collapse_file.exists())
+            files_present += int(casualty_file.exists())
+            files_present += int(workforce_file.exists())
+            if files_present < 4:
+                file_errors.append(
+                    (
+                        "One or more of the required semi-empirical "
+                        f"files in {args.semi_folder} are missing."
+                    )
+                )
+    if len(file_errors):
+        print("The following file errors have been detected:")
+        for file_error in file_errors:
+            print(file_error)
+        print("Exiting.")
+        sys.exit(1)
+
+
+def write_output(args, dataframe):
+    if args.outfile:
+        print(f"Saving {len(dataframe)} rows to {args.outfile}")
+        if args.outfile.endswith(".xlsx"):
+            dataframe.to_excel(args.outfile, index=False)
+        else:
+            dataframe.to_csv(args.outfile, index=False)
+        sys.exit(0)
+    else:
+        print(dataframe.to_string(index=False))
+
+
+def run_event(args):
+    set_logging(args)
+    check_input_files(args)
+    config = read_config()
+    file_or_url = pathlib.Path(args.file_or_url)
+    if file_or_url.exists():
+        dataframe = calc_pager_event(
+            args.grid_xml,
+            config,
+            args.semimodel,
+            args.fatality_file,
+            args.economic_file,
+            args.semi_folder,
+        )
+    else:
+        url = EVENT_TEMPLATE.format(eventid=args.eventid)
+        with tempfile.TemporaryDirectory() as tempdir:
+            with urlopen(url) as fh:
+                data = fh.read().decode("utf8")
+                jdict = json.loads(data)
+                if "shakemap" not in jdict["properties"]["types"]:
+                    print(f"No ShakeMap for event {args.eventid}. Exiting.")
+                    sys.exit(1)
+                shakemap = jdict["properties"]["products"]["shakemap"][0]
+                grid_url = shakemap["contents"]["download/grid.xml"]["url"]
+                with urlopen(grid_url) as fh2:
+                    xdata = fh2.read().decode("utf8")
+
+                tmpgridfile = pathlib.Path(tempdir) / "tmp.xml"
+                with open(tmpgridfile, "wt") as fout:
+                    fout.write(xdata)
+                config = read_config()
+                dataframe = calc_pager_event(
+                    tmpgridfile,
+                    config,
+                    args.semimodel,
+                    args.fatality_file,
+                    args.economic_file,
+                    args.semi_folder,
+                )
+        write_output(args, dataframe)
+
+
+def run_batch(args):
+    set_logging(args)
+    check_input_files(args)
+    dataframe = calc_pager_events(
+        args.folder,
+        args.verbose,
+        args.run_semi,
+        args.fatality_file,
+        args.economic_file,
+        args.semi_folder,
+        timerange=args.time_range,
+        bounds=args.bounds,
+        magrange=args.mag_range,
+        depthrange=args.depth_range,
+    )
+    write_output(args, dataframe)
+
+
 def main():
     helpstr = (
         "Render complete empirical/semi-empirical PAGER results.\n\n"
         "Default behavior renders PAGER results for a set of earthquakes\n"
         "as a formatted DataFrame with multiple rows of exposure and loss,\n"
         "one row per country, plus a final row with totals. \n"
         "The empirical models are described in the following papers:\n"
@@ -82,27 +212,17 @@
         "<BuildingType1>: Many building type columns described in Jaiswal 2011.\n"
         "TotalSemiFatalities: Final column summing fatalities across all building types."
     )
     parser = argparse.ArgumentParser(
         description=helpstr,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
-    group = parser.add_mutually_exclusive_group(required=True)
-    group.add_argument(
-        "-f", "--folder", help="A folder containing many ShakeMap *grid.xml files."
-    )
-    group.add_argument("-g", "--grid-xml", help="A ShakeMap grid.xml file.")
-    group.add_argument(
-        "-e",
-        "--eventid",
-        help="ComCat event ID - preferred ShakeMap grid.xml will be used.",
-    )
     parser.add_argument(
         "-s",
-        "--semimodel",
+        "--run-semi",
         help="Calculate semi-empirical model results as well.",
         action="store_true",
         default=False,
     )
     parser.add_argument(
         "-o", "--outfile", help="Specify output file (.xlsx for Excel, .csv for CSV)"
     )
@@ -110,174 +230,83 @@
         "-v",
         "--verbose",
         default=False,
         action="store_true",
         help="Print progress output to the screen",
     )
     parser.add_argument(
-        "--fatality", default=None, help="Path to custom fatality Excel file"
+        "-f", "--fatality-file", default=None, help="Path to custom fatality Excel file"
     )
     parser.add_argument(
-        "--economic", default=None, help="Path to custom economic Excel file"
+        "-e", "--economic-file", default=None, help="Path to custom economic Excel file"
     )
     parser.add_argument(
-        "--semifolder",
+        "--semi-folder",
         default=None,
         help=(
             "Path to folder containing custom semi-empirical Excel files. "
             "These files MUST be named semi_inventory.xlsx, "
             "semi_collapse_mmi.xlsx, semi_casualty.xlsx and "
             "semi_workforce.xlsx."
         ),
     )
-    parser.add_argument(
+
+    subparsers = parser.add_subparsers(help="Sub-commands are available below.")
+    event_cmd = subparsers.add_parser(
+        "event", help="Run a single event through pagerlite"
+    )
+    event_cmd.add_argument(
+        "file_or_url", help="Path to local ShakeMap grid XML OR ComCat event ID."
+    )
+    event_cmd.set_defaults(func=run_event)
+
+    batch_cmd = subparsers.add_parser("batch", help="Run many events through pagerlite")
+    batch_cmd.add_argument(
+        "-f", "--folder", help="A folder containing many ShakeMap *grid.xml files."
+    )
+
+    batch_cmd.add_argument(
         "-t",
         "--time-range",
         help="Only process events within given time range.",
         default=None,
         type=maketime,
         nargs=2,
     )
     helpstr = (
         "Only process events within spatial boundary [lonmin lonmax latmin latmax]."
     )
-    parser.add_argument(
+    batch_cmd.add_argument(
         "-b",
         "--bounds",
         metavar=("lonmin", "lonmax", "latmin", "latmax"),
         dest="bounds",
         type=float,
         nargs=4,
         help=helpstr,
     )
+    helpstr = "Only process events within depth range [depthmin depthmax]."
+    batch_cmd.add_argument(
+        "-d",
+        "--depth-range",
+        metavar=("depthmin", "depthmax"),
+        type=float,
+        nargs=2,
+        help=helpstr,
+    )
     helpstr = "Minimum and maximum (authoritative) magnitude to restrict search."
-    parser.add_argument(
+    batch_cmd.add_argument(
         "-m",
         "--mag-range",
         metavar=("minmag", "maxmag"),
-        dest="magrange",
         type=float,
         nargs=2,
         help=helpstr,
     )
+    batch_cmd.set_defaults(func=run_batch)
 
     args = parser.parse_args()
-
-    if args.verbose:
-        loglevel = logging.INFO
-    else:
-        loglevel = logging.CRITICAL
-    logging.basicConfig(
-        level=loglevel,
-        format="%(asctime)s %(message)s",
-        handlers=[logging.StreamHandler()],
-    )
-
-    # check to make sure that any input fatality/econ/semi files/folders actually exist
-    file_errors = []
-
-    if args.fatality is not None:
-        fatpath = pathlib.Path(args.fatality).resolve()
-        if not fatpath.exists():
-            file_errors.append(f"Input file {fatpath} does not exist.")
-
-    if args.economic is not None:
-        ecopath = pathlib.Path(args.economic).resolve()
-        if not ecopath.exists():
-            file_errors.append(f"Input file {ecopath} does not exist.")
-
-    if args.semifolder is not None:
-        semipath = pathlib.Path(args.semifolder).resolve()
-        if not semipath.exists() or not semipath.is_dir():
-            file_errors.append(
-                f"Input file {semipath} does not exist or is not a directory."
-            )
-        else:
-            inventory_file = semipath / "semi_inventory.xlsx"
-            collapse_file = semipath / "semi_collapse_mmi.xlsx"
-            casualty_file = semipath / "semi_casualty.xlsx"
-            workforce_file = semipath / "semi_workforce.xlsx"
-            files_present = 0
-            files_present += int(inventory_file.exists())
-            files_present += int(collapse_file.exists())
-            files_present += int(casualty_file.exists())
-            files_present += int(workforce_file.exists())
-            if files_present < 4:
-                file_errors.append(
-                    (
-                        "One or more of the required semi-empirical "
-                        f"files in {args.semifolder} are missing."
-                    )
-                )
-    if len(file_errors):
-        print("The following file errors have been detected:")
-        for file_error in file_errors:
-            print(file_error)
-        print("Exiting.")
-        sys.exit(1)
-
-    starttime = None
-    endtime = None
-    if args.time_range is not None:
-        starttime = args.time_range[0]
-        endtime = args.time_range[1]
-
-    if args.folder:
-        dataframe = calc_pager_events(
-            args.folder,
-            args.verbose,
-            args.semimodel,
-            args.fatality,
-            args.economic,
-            args.semifolder,
-            starttime=starttime,
-            endtime=endtime,
-            bounds=args.bounds,
-            magrange=args.magrange,
-        )
-    elif args.eventid:
-        url = EVENT_TEMPLATE.format(eventid=args.eventid)
-        with tempfile.TemporaryDirectory() as tempdir:
-            with urlopen(url) as fh:
-                data = fh.read().decode("utf8")
-                jdict = json.loads(data)
-                if "shakemap" not in jdict["properties"]["types"]:
-                    print(f"No ShakeMap for event {args.eventid}. Exiting.")
-                    sys.exit(1)
-                shakemap = jdict["properties"]["products"]["shakemap"][0]
-                grid_url = shakemap["contents"]["download/grid.xml"]["url"]
-                with urlopen(grid_url) as fh2:
-                    xdata = fh2.read().decode("utf8")
-
-                tmpgridfile = pathlib.Path(tempdir) / "tmp.xml"
-                with open(tmpgridfile, "wt") as fout:
-                    fout.write(xdata)
-                config = read_config()
-                dataframe = calc_pager_event(
-                    tmpgridfile,
-                    config,
-                    args.semimodel,
-                    args.fatality,
-                    args.economic,
-                    args.semifolder,
-                    starttime=starttime,
-                    endtime=endtime,
-                    bounds=args.bounds,
-                    magrange=args.magrange,
-                )
-    else:
-        config = read_config()
-        dataframe = calc_pager_event(args.grid_xml, config, args.semimodel)
-
-    if args.outfile:
-        print(f"Saving {len(dataframe)} rows to {args.outfile}")
-        if args.outfile.endswith(".xlsx"):
-            dataframe.to_excel(args.outfile, index=False)
-        else:
-            dataframe.to_csv(args.outfile, index=False)
-        sys.exit(0)
-    else:
-        print(dataframe.to_string(index=False))
+    args.func(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/calc.py` & `esi_utils_pager-1.1.13/src/esi_utils_pager/calc.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # stdlib imports
 import logging
 import pathlib
 import sys
 import warnings
+from datetime import datetime
 
 # third party imports
 import pandas as pd
 import rasterio
 from esi_utils_time.timeutils import LocalTime
 from mapio.shake import getHeaderData
 from rasterio.sample import sample_gen
 
 # local imports
-from esi_utils_pager.config import read_config
+from esi_utils_pager.config import get_config_file, read_config
 from esi_utils_pager.country import Country
 from esi_utils_pager.econexposure import EconExposure
 from esi_utils_pager.emploss import EmpiricalLoss
 from esi_utils_pager.exposure import Exposure
 from esi_utils_pager.semimodel import SemiEmpiricalFatality
 
 
@@ -154,46 +155,24 @@
 def calc_pager_event(
     gridfile,
     config,
     run_semi,
     fatality_file,
     economic_file,
     semi_folder,
-    starttime=None,
-    endtime=None,
-    bounds=None,
-    magrange=None,
 ):
     # get all the basic event information and print it, if requested
     shake_tuple = getHeaderData(gridfile)
     local_time = get_local_time(
         shake_tuple[1]["event_timestamp"],
         config["model_data"]["timezones_file"],
         shake_tuple[1]["lat"],
         shake_tuple[1]["lon"],
     )
-    empty_dataframe = pd.DataFrame()
     eventid = shake_tuple[1]["event_id"]
-    if (
-        shake_tuple[1]["event_timestamp"] < starttime
-        or shake_tuple[1]["event_timestamp"] > endtime
-    ):
-        print(f"Skipping event {eventid} (out of time range)")
-        return empty_dataframe
-    outside_lat = shake_tuple[1]["lat"] < bounds[2] or shake_tuple[1]["lat"] > bounds[3]
-    outside_lon = shake_tuple[1]["lon"] < bounds[0] or shake_tuple[1]["lon"] > bounds[1]
-    if outside_lat or outside_lon:
-        print(f"Skipping event {eventid} (out of spatial range)")
-        return empty_dataframe
-    if (
-        shake_tuple[1]["magnitude"] < magrange[0]
-        or shake_tuple[1]["magnitude"] > magrange[1]
-    ):
-        print(f"Skipping event {eventid} (out of magnitude range)")
-        return empty_dataframe
     print(f"Processing event {eventid}...")
     master_row = {}
     master_row["EventID"] = shake_tuple[1]["event_id"]
     master_row["Time"] = shake_tuple[1]["event_timestamp"]
     master_row["LocalTime"] = local_time
     master_row["Latitude"] = shake_tuple[1]["lat"]
     master_row["Longitude"] = shake_tuple[1]["lon"]
@@ -238,43 +217,104 @@
 def calc_pager_events(
     gridfolder,
     verbose,
     run_semi,
     fatality_file,
     economic_file,
     semi_folder,
-    starttime=None,
-    endtime=None,
+    timerange=None,
     bounds=None,
     magrange=None,
+    depthrange=None,
 ):
     gridfolder = pathlib.Path(gridfolder)
     # read config file
     config = read_config()
     # Make sure grid.xml file exists
     if not gridfolder.is_dir():
         print(f"ShakeMap Grid folder {gridfolder} does not exist.")
         sys.exit(1)
 
-    gridfiles = gridfolder.glob("**/*grid.xml")
+    gridfiles = list(gridfolder.glob("**/*grid.xml"))
+    config_dir = pathlib.Path(get_config_file()).parent
+    index_file = config_dir / (str(gridfolder).lstrip("/").replace("/", "_") + ".csv")
+
+    if index_file.exists():
+        grid_index = pd.read_csv(index_file, parse_dates=["time"])
+    else:
+        logging.info(f"Building index of input folder {gridfolder}...")
+        events = []
+        for gridfile in gridfiles:
+            # On some systems, there may be backup directories - we don't want these
+            # by default, so we'll skip them if we detect backup000 in the path
+            if "backup000" in str(gridfile):
+                continue
+            # get all the basic event information and print it, if requested
+            shake_tuple = getHeaderData(gridfile)
+            etime = shake_tuple[1]["event_timestamp"]
+            eventid = shake_tuple[1]["event_id"]
+            elat = shake_tuple[1]["lat"]
+            elon = shake_tuple[1]["lon"]
+            edepth = shake_tuple[1]["depth"]
+            emag = shake_tuple[1]["magnitude"]
+            row = {
+                "eventid": eventid,
+                "time": etime,
+                "latitude": elat,
+                "longitude": elon,
+                "depth": edepth,
+                "magnitude": emag,
+                "gridfile": gridfile,
+            }
+            events.append(row)
+
+        grid_index = pd.DataFrame(data=events)
+        grid_index["time"] = grid_index["time"].astype("datetime64[ns]")
+        grid_index.to_csv(index_file, index=False)
+        logging.info("Built index file containing {len(index)} events.")
+
+    timeidx = grid_index["magnitude"] > 0
+    boundsidx = grid_index["magnitude"] > 0
+    depthidx = grid_index["magnitude"] > 0
+    magidx = grid_index["magnitude"] > 0
+
+    if timerange is not None:
+        t1 = timerange[0]
+        t2 = timerange[1]
+        timeidx = (grid_index["time"] >= t1) & (grid_index["time"] < t2)
+
+    if bounds is not None:
+        latidx = (grid_index["latitude"] >= bounds[2]) & (
+            grid_index["latitude"] < bounds[3]
+        )
+        lonidx = (grid_index["longitude"] >= bounds[0]) & (
+            grid_index["longitude"] < bounds[1]
+        )
+        boundsidx = latidx & lonidx
+    if depthrange is not None:
+        depthidx = (grid_index["depth"] >= depthrange[0]) & (
+            grid_index["depth"] < depthrange[1]
+        )
+    if magrange is not None:
+        magidx = (grid_index["magnitude"] >= magrange[0]) & (
+            grid_index["magnitude"] < magrange[1]
+        )
+    events = grid_index[timeidx & boundsidx & depthidx & magidx]
     dataframes = []
-    for gridfile in gridfiles:
+    for idx, row in events.iterrows():
+        gridfile = row["gridfile"]
         if verbose:
             logging.info(f"Parsing {gridfile}...")
         dataframe = calc_pager_event(
             gridfile,
             config,
             run_semi,
             fatality_file,
             economic_file,
             semi_folder,
-            starttime=starttime,
-            endtime=endtime,
-            bounds=bounds,
-            magrange=magrange,
         )
         dataframes.append(dataframe)
 
     dataframe = pd.concat(dataframes)
     if run_semi:
         # make TotalSemiFatalities column the last one, if it exists
         fatcol = dataframe.pop("TotalSemiFatalities")
```

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/config.py` & `esi_utils_pager-1.1.13/src/esi_utils_pager/config.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/country.py` & `esi_utils_pager-1.1.13/src/esi_utils_pager/country.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/countries.xlsx` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/countries.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/economic.xlsx` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/economic.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/economy.xml` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/economy.xml`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/fatality.xlsx` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/fatality.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/fatality.xml` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/fatality.xml`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_casualty.hdf` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_casualty.hdf`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_casualty.xlsx` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_casualty.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_collapse_mmi.hdf` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_collapse_mmi.hdf`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_collapse_mmi.xlsx` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_collapse_mmi.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_inventory.hdf` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_inventory.hdf`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_inventory.xlsx` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_inventory.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_workforce.hdf` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_workforce.hdf`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/data/semi_workforce.xlsx` & `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_workforce.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/econexposure.py` & `esi_utils_pager-1.1.13/src/esi_utils_pager/econexposure.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/emploss.py` & `esi_utils_pager-1.1.13/src/esi_utils_pager/emploss.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/exposure.py` & `esi_utils_pager-1.1.13/src/esi_utils_pager/exposure.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/growth.py` & `esi_utils_pager-1.1.13/src/esi_utils_pager/growth.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/probs.py` & `esi_utils_pager-1.1.13/src/esi_utils_pager/probs.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager/semimodel.py` & `esi_utils_pager-1.1.13/src/esi_utils_pager/semimodel.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/PKG-INFO` & `esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-utils-pager
-Version: 1.1.12
+Version: 1.1.13
 Summary: USGS PAGER loss modeling functionality
 Author-email: Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -153,53 +153,107 @@
   - {population_grid: /data/pagerdata/model_data/population/lspop2018.flt, population_year: 2018}
   urban_rural_grid: /data/pagerdata/model_data/glurextents.bil
 ```
 
 
 # Command Line Usage
 The command line program made available by this repository is `pagerlite`. This program outputs detailed empirical
-(fatality/economic) PAGER model results to a tabular format. To see the help for this program:
+(fatality/economic) PAGER model results to a tabular format. The help for this program (`pagerlite -h`):
 
-`pagerlite -h`
+```
+positional arguments:
+  {event,batch}         Sub-commands are available below.
+    event               Run a single event through pagerlite
+    batch               Run many events through pagerlite
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -s, --run-semi        Calculate semi-empirical model results as well.
+  -o OUTFILE, --outfile OUTFILE
+                        Specify output file (.xlsx for Excel, .csv for CSV)
+  -v, --verbose         Print progress output to the screen
+  -f FATALITY_FILE, --fatality-file FATALITY_FILE
+                        Path to custom fatality Excel file
+  -e ECONOMIC_FILE, --economic-file ECONOMIC_FILE
+                        Path to custom economic Excel file
+  --semi-folder SEMI_FOLDER
+                        Path to folder containing custom semi-empirical Excel files. These files MUST be named
+                        semi_inventory.xlsx, semi_collapse_mmi.xlsx, semi_casualty.xlsx and semi_workforce.xlsx.
+```
 
-There are three input modes for pagerlite:
+There are two subcommands for pagerlite:
 
- - `pagerlite -e <eventid>` Run pagerlite on a single event specified by a ComCat event ID.
- - `pagerlite -g <grid.xml>` Run pagerlite on a single grid.xml file.
- - `pagerlite -f <gridfolder>` Run pagerlite on a directory containing many grid.xml files 
+ - `pagerlite event` Run on a single event specified by ComCat event ID OR path to grid.xml.
+ - `pagerlite batch` Run pagerlite on a directory containing many grid.xml files 
     (these files can be in sub-directories).
 
+The event subcommand is straightforward (`pagerlite event -h`):
+
+```
+usage: pagerlite event [-h] file_or_url
+
+positional arguments:
+  file_or_url  Path to local ShakeMap grid XML OR ComCat event ID.
+
+optional arguments:
+  -h, --help   show this help message and exit
+```
+
+The `batch` subcommand has a number of optional arguments (`pagerlite batch -h`):
+
+```
+usage: pagerlite batch [-h] [-f FOLDER] [-t TIME_RANGE TIME_RANGE] [-b lonmin lonmax latmin latmax]
+                       [-d depthmin depthmax] [-m minmag maxmag]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -f FOLDER, --folder FOLDER
+                        A folder containing many ShakeMap *grid.xml files.
+  -t TIME_RANGE TIME_RANGE, --time-range TIME_RANGE TIME_RANGE
+                        Only process events within given time range.
+  -b lonmin lonmax latmin latmax, --bounds lonmin lonmax latmin latmax
+                        Only process events within spatial boundary [lonmin lonmax latmin latmax].
+  -d depthmin depthmax, --depth-range depthmin depthmax
+                        Only process events within depth range [depthmin depthmax].
+  -m minmag maxmag, --mag-range minmag maxmag
+                        Minimum and maximum (authoritative) magnitude to restrict search.
+```
+
 ## Examples
 
 To run the PAGER empirical models *only* on a ShakeMap grid.xml file in the current directory and write the results to an Excel file:
 
-`pagerlite -g grid.xml -o output.xlsx`
+`pagerlite -o output.xlsx event grid.xml`
 
 To run the PAGER empirical models *only* on a directory containing (potentially) many sub-directories with 
 files ending in "grid.xml":
 
-`pagerlite -f /data/shakemap_output/ -o output.xlsx`
+`pagerlite -o output.xlsx batch -f /data/shakemap_output/`
 
 To run the PAGER empirical models *only* on a ComCat event ID (this will download the authoritative 
 ShakeMap grid.xml file from ComCat):
 
-`pagerlite -e us7000lz23 -o output.xlsx`
+`pagerlite -o output.xlsx batch us7000lz23 `
 
 To run the PAGER empirical AND semi-empirical models, simply add the `-s` flag to any of the above commands:
 
-`pagerlite -e us7000lz23 -s -o output.xlsx`
+`pagerlite -s -o output.xlsx batch us7000lz23`
 
 To run the PAGER empirical models on a folder but only for events between 2010 and 2017:
 
-`pagerlite -f /data/shakemap_output/ -t 2010-01-01 2017-12-31T23:59:59 -o output.xlsx`
+`pagerlite -o output.xlsx batch -f /data/shakemap_output/ -t 2010-01-01 2017-12-31T23:59:59`
+
+To run PAGER empirical models on a folder but only for events in Japan:
+`pagerlite -o output.xlsx batch -f /data/shakemap_output/ -b 30.844021 44.762578 128.336525  149.031827`
 
-See the help for more options (spatial bounds and magnitude range) on restricting processing of ShakeMap
+See the help for more options (depth and magnitude ranges) on restricting processing of ShakeMap
 grids.
 
 
 
+
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi_utils_pager-1.1.12/src/esi_utils_pager.egg-info/SOURCES.txt` & `esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

