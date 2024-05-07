# Comparing `tmp/MobileInventoryCLI-0.4.96.tar.gz` & `tmp/MobileInventoryCLI-0.4.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.96.tar", last modified: Mon May  6 23:07:16 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.97.tar", last modified: Tue May  7 14:50:59 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.96.tar` & `MobileInventoryCLI-0.4.97.tar`

### file list

```diff
@@ -1,112 +1,115 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.914796 MobileInventoryCLI-0.4.96/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.901463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.901463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.904796 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.904796 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.904796 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.904796 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.908130 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)    10261 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   117305 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
--rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.908130 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.908130 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.908130 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.908130 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.908130 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.908130 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     7211 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.908130 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.908130 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.908130 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.911463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)     4349 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
--rw-r--r--   0 carl      (1000) carl      (1000)    18881 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    22046 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.911463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    84220 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.911463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.911463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    29618 2024-05-06 23:06:27.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.911463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
--rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-05-06 23:07:10.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2781 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.911463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.911463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.911463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.911463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.911463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.911463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.911463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.911463 MobileInventoryCLI-0.4.96/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-05-06 22:54:11.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:16.914796 MobileInventoryCLI-0.4.96/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-06 23:07:16.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-05-06 23:07:16.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-05-06 23:07:16.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-05-06 23:07:16.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-05-06 23:07:16.000000 MobileInventoryCLI-0.4.96/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-06 23:07:16.914796 MobileInventoryCLI-0.4.96/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-06 23:07:16.914796 MobileInventoryCLI-0.4.96/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-05-06 23:07:16.000000 MobileInventoryCLI-0.4.96/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.067457 MobileInventoryCLI-0.4.97/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.044124 MobileInventoryCLI-0.4.97/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.044124 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.050790 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.050790 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.050790 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.054123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.054123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)    10261 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2559 2024-05-07 14:42:30.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/SMLabelImporter.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   117305 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.054123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.054123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.054123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.054123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.054123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.057457 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     7211 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.060790 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.060790 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.060790 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.060790 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4349 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    18881 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    22046 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+-rw-rw----   0 carl      (1000) carl      (1000)      122 2024-05-06 23:18:28.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.064123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    84220 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.064123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.064123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    29832 2024-05-07 14:44:56.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.064123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-05-07 14:50:53.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2781 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5953 2024-05-07 14:49:17.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.064123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.064123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.064123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-rw----   0 carl      (1000) carl      (1000)        6 2024-05-06 23:18:28.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/version.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.064123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.064123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.064123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.064123 MobileInventoryCLI-0.4.97/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.067457 MobileInventoryCLI-0.4.97/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-05-06 23:07:27.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:50:59.067457 MobileInventoryCLI-0.4.97/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-07 14:50:58.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5568 2024-05-07 14:50:58.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-05-07 14:50:58.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-05-07 14:50:58.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-05-07 14:50:58.000000 MobileInventoryCLI-0.4.97/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-07 14:50:59.067457 MobileInventoryCLI-0.4.97/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-07 14:50:59.067457 MobileInventoryCLI-0.4.97/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-05-07 14:50:58.000000 MobileInventoryCLI-0.4.97/setup.py
```

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pathlib import Path
 import upcean
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ExtractPkg.ExtractPkg2 import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.Lookup.Lookup import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DayLog.DayLogger import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.db import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.Prompt import *
+from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.SMLabelImporter import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.ResetTools import *
 
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ConvertCode.ConvertCode import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.setCode.setCode import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.Locator.Locator import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.ListMode2.ListMode2 import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.TasksMode.Tasks import *
@@ -712,14 +713,17 @@
 							session.commit()
 							session.refresh(ne)
 							print(f"{ne}\n{num+1}/{len(dt)} - {r}")
 
 						session.commit()
 				print(f"Remember CSV must have {Style.underline}'Barcode,Code,Name'{Style.reset} headers as first line")
 			return Prompt(func=import_csv_lcl,ptext="File Path",helpText=self.help(print_no=True),data=self).state
+		elif args[0].lower() in ['import_smartlabel_html','ish']:
+			ScrapeLocalSmartLabelList(engine=self.engine)
+			return True
 		elif args[0].lower() in ['set_all_inlist_0','sai0']:
 			with Session(self.engine) as session:
 				result=session.query(Entry).all()
 				ct=len(result)
 				for num,r in enumerate(result):
 					print(f"{Fore.green}{num+1}{Style.reset}/{Fore.red}{ct}{Style.reset}")
 					r.InList=False
```

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,8 +40,9 @@
 {Fore.green}sau1|set_all_userUpdated_1{Style.reset} - {Fore.cyan}set all Entry's to userUpdated=True{Style.reset}
 {Fore.green}lau0|list_all_userUpdated_0{Style.reset} - {Fore.cyan}list all Entry's with userUpdated=False{Style.reset}
 {Fore.green}lau1|list_all_userUpdated_1{Style.reset} - {Fore.cyan}list all Entry's with userUpdated=True{Style.reset}
 {Fore.green}import_csv{Style.reset} - {Fore.cyan}Import CSV data, must have Barcode,Code,Name headers and if other Entry Fields are specified, then those will be used too, icluding valid image paths.{Style.reset}
 {Fore.green}ie|item_editor|itm_edt{Style.reset}-{Fore.cyan}Use the Item Editor,auto-scaling for new fields when new fields are added!{Style.reset}
 {Fore.green}export_list_field|elf{Style.reset}-{Fore.cyan}Export specified field to QREncoded Img from Entry.InList==True{Style.reset}
 {Fore.green}total_entries|te|count_all|cta{Style.reset}-{Fore.cyan}count all Entry's{Style.reset}
-{Fore.green}qsl|quick_show_list{Style.reset}-{Fore.cyan}Briefly display list contents{Style.reset}
+{Fore.green}qsl|quick_show_list{Style.reset}-{Fore.cyan}Briefly display list contents{Style.reset}
+{Fore.green}import_smartlabel_html|ish{Style.reset}-{Fore.cyan}import content from {Fore.light_green}'https://smartlabel.org/product-search/?br=all&product=all&perPage=500'{Style.reset}
```

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.96
+Version: 0.4.97
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.96/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.97/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,33 +6,36 @@
 MobileInventoryCLI.egg-info/__init__.py
 MobileInventoryCLI.egg-info/dependency_links.txt
 MobileInventoryCLI.egg-info/requires.txt
 MobileInventoryCLI.egg-info/top_level.txt
 MobileInventoryCLI/CodeProcessing/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/version.txt
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/SMLabelImporter.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
```

### Comparing `MobileInventoryCLI-0.4.96/PKG-INFO` & `MobileInventoryCLI-0.4.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.96
+Version: 0.4.97
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.96/setup.py` & `MobileInventoryCLI-0.4.97/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.96'
+version='0.4.97'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

