# Comparing `tmp/t0-3.1.6.tar.gz` & `tmp/t0-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t0-3.1.6.tar", last modified: Mon Apr 22 19:10:57 2024, max compression
+gzip compressed data, was "t0-4.0.1.tar", last modified: Tue May  7 11:25:38 2024, max compression
```

## Comparing `t0-3.1.6.tar` & `t0-4.0.1.tar`

### file list

```diff
@@ -1,201 +1,272 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.059049 t0-3.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-22 19:10:45.000000 t0-3.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 19:10:45.000000 t0-3.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-22 19:10:45.000000 t0-3.1.6/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    13787 2024-04-22 19:10:57.059049 t0-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:10:45.000000 t0-3.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-22 19:10:54.000000 t0-3.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 19:10:45.000000 t0-3.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:10:57.059049 t0-3.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.027049 t0-3.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.027049 t0-3.1.6/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.027049 t0-3.1.6/src/python/T0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.031049 t0-3.1.6/src/python/T0/ConditionUpload/
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/ConditionUpload/ConditionUploadAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/ConditionUpload/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29389 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/ConditionUpload/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.031049 t0-3.1.6/src/python/T0/JobSplitting/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/JobSplitting/AlcaHarvest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/JobSplitting/Condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/JobSplitting/Express.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/JobSplitting/ExpressMerge.py
--rw-r--r--   0 runner    (1001) docker     (127)    12570 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/JobSplitting/Repack.py
--rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/JobSplitting/RepackMerge.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/JobSplitting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.031049 t0-3.1.6/src/python/T0/RunConfig/
--rw-r--r--   0 runner    (1001) docker     (127)    61588 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/RunConfig/RunConfigAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)    47342 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/RunConfig/Tier0Config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/RunConfig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.031049 t0-3.1.6/src/python/T0/RunLumiCloseout/
--rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/RunLumiCloseout/RunLumiCloseoutAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/RunLumiCloseout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.031049 t0-3.1.6/src/python/T0/StorageManager/
--rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/StorageManager/StorageManagerAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/StorageManager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.031049 t0-3.1.6/src/python/T0/WMBS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.031049 t0-3.1.6/src/python/T0/WMBS/Oracle/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.035049 t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/CompleteFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/FinishPCLforEmptyExpress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/GetConditions.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/GetRunStopTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/IsPromptCalibrationFinished.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/MarkPromptCalibrationFinished.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38733 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.035049 t0-3.1.6/src/python/T0/WMBS/Oracle/JobSplitting/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/JobSplitting/InsertPromptCalibrationFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/JobSplitting/InsertSplitLumis.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/JobSplitting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.039049 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/FindRecoRelease.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/FindRecoReleaseDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetExpressConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetHLTConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetPhEDExConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetRecoConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetRepackConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetRunInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasetTriggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetStreamOnlineVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetStreamStyle.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertCMSSWVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetScenario.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetTrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertExpressConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertLumiSection.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertPhEDExConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertPrimaryDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertPromptCalibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoReleaseConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertRepackConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertRun.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertRunStreamDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertSpecialDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStorageNode.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamCMSSWVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamFileset.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamStyle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamer.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertTrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertWorkflowMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/ReleasePromptReco.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/UpdateRun.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.043049 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckActiveSplitLumis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckClosedLumis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckEndOfRunRecords.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRunStreamFilesets.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/DeleteStreamers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FinalCloseLumi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindActiveRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedLumis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindHighContLumi.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindOpenRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindStoppedRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/ForceCloseLumi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetClosedLumisForStream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFileCountOnOpenLumis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFilesForStreamLumi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetOpenRunStreamLumicount.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/InsertClosedLumi.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/StopRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.047049 t0-3.1.6/src/python/T0/WMBS/Oracle/SMNotification/
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/SMNotification/GetFinishedStreamers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/SMNotification/InsertOfflineFileStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/SMNotification/MarkStreamersFinished.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/SMNotification/UpdateOfflineFileStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/SMNotification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.047049 t0-3.1.6/src/python/T0/WMBS/Oracle/StorageManager/
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/StorageManager/GetNewData.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/StorageManager/GetRunInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/StorageManager/GetRunSetup.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/StorageManager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.047049 t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetAllFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableConditionFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressMergeFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackMergeFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepackMerge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetUsedLumis.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/HaveAvailableFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/HaveJobGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.051049 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetDatasetLocked.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetExpressConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetNewRun.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetPromptRecoStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetRecoConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetRunStreamDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetSkippedStreamers.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertDatasetLocked.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertExpressConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertNewRun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoLocked.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunDatasetDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunStreamDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertSkippedStreamers.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateDatasetLocked.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateExpressConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateNewRun.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoLocked.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunDatasetDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunStreamDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateSkippedStreamers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.055049 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/FeedStreamers.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewExpressRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRunStreams.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetDeploymentID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetExpressReadyRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetNotClosedOutWorkflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetPromptRecoWorkflowsForMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetNew.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetReleased.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetStreamerWorkflowsForMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkCloseoutWorkflowMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkTrackedWorkflowMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkWorkflowsInjected.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/ReleaseExpress.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/SetDeploymentID.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/UpdateRecoReleaseConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/Oracle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMBS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.055049 t0-3.1.6/src/python/T0/WMSpec/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.055049 t0-3.1.6/src/python/T0/WMSpec/StdSpecs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMSpec/StdSpecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/WMSpec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.055049 t0-3.1.6/src/python/T0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13787 2024-04-22 19:10:57.000000 t0-3.1.6/src/python/T0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-04-22 19:10:57.000000 t0-3.1.6/src/python/T0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:10:57.000000 t0-3.1.6/src/python/T0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 19:10:57.000000 t0-3.1.6/src/python/T0.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.055049 t0-3.1.6/src/python/T0Component/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.055049 t0-3.1.6/src/python/T0Component/Tier0Auditor/
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0Component/Tier0Auditor/Tier0Auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0Component/Tier0Auditor/Tier0AuditorPoller.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0Component/Tier0Auditor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:57.055049 t0-3.1.6/src/python/T0Component/Tier0Feeder/
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0Component/Tier0Feeder/Tier0Feeder.py
--rw-r--r--   0 runner    (1001) docker     (127)    31322 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0Component/Tier0Feeder/Tier0FeederPoller.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0Component/Tier0Feeder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:10:45.000000 t0-3.1.6/src/python/T0Component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.538797 t0-4.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.494797 t0-4.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.498797 t0-4.0.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-07 11:25:24.000000 t0-4.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-07 11:25:24.000000 t0-4.0.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-07 11:25:24.000000 t0-4.0.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.498797 t0-4.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-07 11:25:24.000000 t0-4.0.1/.github/workflows/pypiReleaseUpload.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 11:25:24.000000 t0-4.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    72975 2024-05-07 11:25:24.000000 t0-4.0.1/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 11:25:24.000000 t0-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 11:25:24.000000 t0-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-07 11:25:24.000000 t0-4.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-07 11:25:38.538797 t0-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:25:24.000000 t0-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.498797 t0-4.0.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12588 2024-05-07 11:25:24.000000 t0-4.0.1/bin/00_deploy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13192 2024-05-07 11:25:24.000000 t0-4.0.1/bin/00_deploy_prod.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13970 2024-05-07 11:25:24.000000 t0-4.0.1/bin/00_deploy_replay.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1422 2024-05-07 11:25:24.000000 t0-4.0.1/bin/00_patches.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2147 2024-05-07 11:25:24.000000 t0-4.0.1/bin/00_software.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4602 2024-05-07 11:25:24.000000 t0-4.0.1/bin/buildrelease.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7118 2024-05-07 11:25:24.000000 t0-4.0.1/bin/cmst0_backlog_wma
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8335 2024-05-07 11:25:24.000000 t0-4.0.1/bin/cmst0_late_workflows
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11425 2024-05-07 11:25:24.000000 t0-4.0.1/bin/cmst0_long_jobs
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6694 2024-05-07 11:25:24.000000 t0-4.0.1/bin/cmst0_paused_jobs
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11745 2024-05-07 11:25:24.000000 t0-4.0.1/bin/diagnoseActiveRuns
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8094 2024-05-07 11:25:24.000000 t0-4.0.1/bin/forceCloseRuns
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5211 2024-05-07 11:25:24.000000 t0-4.0.1/bin/tier0-mod-config
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.498797 t0-4.0.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-07 11:25:24.000000 t0-4.0.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.502797 t0-4.0.1/doc/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-07 11:25:24.000000 t0-4.0.1/doc/sphinx/changelog.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.490797 t0-4.0.1/doc/sphinx/code/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.502797 t0-4.0.1/doc/sphinx/code/T0/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-07 11:25:24.000000 t0-4.0.1/doc/sphinx/code/T0/JobSplitting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 11:25:24.000000 t0-4.0.1/doc/sphinx/code/T0/RunConfig.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-07 11:25:24.000000 t0-4.0.1/doc/sphinx/code/T0/WMBS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 11:25:24.000000 t0-4.0.1/doc/sphinx/code/T0/WMSpecs.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.502797 t0-4.0.1/doc/sphinx/code/T0Component/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-07 11:25:24.000000 t0-4.0.1/doc/sphinx/code/T0Component/Tier0Feeder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-07 11:25:24.000000 t0-4.0.1/doc/sphinx/code.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-05-07 11:25:24.000000 t0-4.0.1/doc/sphinx/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-07 11:25:24.000000 t0-4.0.1/doc/sphinx/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 11:25:24.000000 t0-4.0.1/doc/sphinx/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-07 11:25:24.000000 t0-4.0.1/doc/sphinx/references.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.502797 t0-4.0.1/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-07 11:25:24.000000 t0-4.0.1/etc/ContainterConfig.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    72655 2024-05-07 11:25:24.000000 t0-4.0.1/etc/HIProdOfflineConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65615 2024-05-07 11:25:24.000000 t0-4.0.1/etc/HIReplayOfflineConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60169 2024-05-07 11:25:24.000000 t0-4.0.1/etc/ProdOfflineConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54268 2024-05-07 11:25:24.000000 t0-4.0.1/etc/ReplayOfflineConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-05-07 11:25:24.000000 t0-4.0.1/etc/ReplayOfflineConfigurationRun1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-07 11:25:24.000000 t0-4.0.1/etc/SLSAlarmsConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-07 11:25:24.000000 t0-4.0.1/etc/Tier0Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77152 2024-05-07 11:25:24.000000 t0-4.0.1/etc/XeXeProdOfflineConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70892 2024-05-07 11:25:24.000000 t0-4.0.1/etc/XeXeReplayOfflineConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 11:25:24.000000 t0-4.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:25:38.538797 t0-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-07 11:25:24.000000 t0-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.490797 t0-4.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.494797 t0-4.0.1/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.506797 t0-4.0.1/src/python/T0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.506797 t0-4.0.1/src/python/T0/ConditionUpload/
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/ConditionUpload/ConditionUploadAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/ConditionUpload/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29389 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/ConditionUpload/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.506797 t0-4.0.1/src/python/T0/JobSplitting/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/JobSplitting/AlcaHarvest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/JobSplitting/Condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/JobSplitting/Express.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/JobSplitting/ExpressMerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12570 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/JobSplitting/Repack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/JobSplitting/RepackMerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/JobSplitting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.506797 t0-4.0.1/src/python/T0/RunConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)    61626 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/RunConfig/RunConfigAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48913 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/RunConfig/Tier0Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/RunConfig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.510797 t0-4.0.1/src/python/T0/RunLumiCloseout/
+-rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/RunLumiCloseout/RunLumiCloseoutAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/RunLumiCloseout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.510797 t0-4.0.1/src/python/T0/StorageManager/
+-rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/StorageManager/StorageManagerAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/StorageManager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.510797 t0-4.0.1/src/python/T0/WMBS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.510797 t0-4.0.1/src/python/T0/WMBS/Oracle/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.510797 t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/CompleteFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/FinishPCLforEmptyExpress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/GetConditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/GetRunStopTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/IsPromptCalibrationFinished.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/MarkPromptCalibrationFinished.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38733 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.510797 t0-4.0.1/src/python/T0/WMBS/Oracle/JobSplitting/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/JobSplitting/InsertPromptCalibrationFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/JobSplitting/InsertSplitLumis.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/JobSplitting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.518797 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/FindRecoRelease.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/FindRecoReleaseDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetExpressConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetHLTConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetPhEDExConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetRecoConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetRepackConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetRunInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasetTriggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetStreamOnlineVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetStreamStyle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertCMSSWVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetScenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetTrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertExpressConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertLumiSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertPhEDExConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertPrimaryDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertPromptCalibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoReleaseConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertRepackConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertRunStreamDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertSpecialDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStorageNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamCMSSWVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamFileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamStyle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertTrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertWorkflowMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/ReleasePromptReco.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/UpdateRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.522797 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckActiveSplitLumis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckClosedLumis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckEndOfRunRecords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRunStreamFilesets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/DeleteStreamers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FinalCloseLumi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindActiveRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedLumis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindHighContLumi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindOpenRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindStoppedRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/ForceCloseLumi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetClosedLumisForStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFileCountOnOpenLumis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFilesForStreamLumi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetOpenRunStreamLumicount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/InsertClosedLumi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/StopRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.522797 t0-4.0.1/src/python/T0/WMBS/Oracle/SMNotification/
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/SMNotification/GetFinishedStreamers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/SMNotification/InsertOfflineFileStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/SMNotification/MarkStreamersFinished.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/SMNotification/UpdateOfflineFileStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/SMNotification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.522797 t0-4.0.1/src/python/T0/WMBS/Oracle/StorageManager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/StorageManager/GetNewData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/StorageManager/GetRunInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/StorageManager/GetRunSetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/StorageManager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.526797 t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetAllFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableConditionFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressMergeFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackMergeFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepackMerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetUsedLumis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/HaveAvailableFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/HaveJobGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.530797 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetDatasetLocked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetExpressConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetNewRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetPromptRecoStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetRecoConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetRunStreamDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetSkippedStreamers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertDatasetLocked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertExpressConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertNewRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoLocked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunDatasetDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunStreamDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertSkippedStreamers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateDatasetLocked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateExpressConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateNewRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoLocked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunDatasetDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunStreamDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateSkippedStreamers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.534797 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/FeedStreamers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewExpressRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRunStreams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetDeploymentID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetExpressReadyRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetNotClosedOutWorkflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetPromptRecoWorkflowsForMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetNew.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetReleased.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetStreamerWorkflowsForMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkCloseoutWorkflowMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkTrackedWorkflowMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkWorkflowsInjected.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/ReleaseExpress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/SetDeploymentID.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/UpdateRecoReleaseConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/Oracle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMBS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.534797 t0-4.0.1/src/python/T0/WMSpec/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.534797 t0-4.0.1/src/python/T0/WMSpec/StdSpecs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMSpec/StdSpecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/WMSpec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.538797 t0-4.0.1/src/python/T0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-07 11:25:38.000000 t0-4.0.1/src/python/T0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11085 2024-05-07 11:25:38.000000 t0-4.0.1/src/python/T0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:25:38.000000 t0-4.0.1/src/python/T0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 11:25:38.000000 t0-4.0.1/src/python/T0.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 11:25:38.000000 t0-4.0.1/src/python/T0.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.534797 t0-4.0.1/src/python/T0Component/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.534797 t0-4.0.1/src/python/T0Component/Tier0Auditor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0Component/Tier0Auditor/Tier0Auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0Component/Tier0Auditor/Tier0AuditorPoller.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0Component/Tier0Auditor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.534797 t0-4.0.1/src/python/T0Component/Tier0Feeder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0Component/Tier0Feeder/Tier0Feeder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31635 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0Component/Tier0Feeder/Tier0FeederPoller.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0Component/Tier0Feeder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:24.000000 t0-4.0.1/src/python/T0Component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.494797 t0-4.0.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.494797 t0-4.0.1/test/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.494797 t0-4.0.1/test/python/T0Component_t/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.534797 t0-4.0.1/test/python/T0Component_t/Tier0Feeder_t/
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-07 11:25:24.000000 t0-4.0.1/test/python/T0Component_t/Tier0Feeder_t/ExampleConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118523 2024-05-07 11:25:24.000000 t0-4.0.1/test/python/T0Component_t/Tier0Feeder_t/Tier0Feeder_t.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.494797 t0-4.0.1/test/python/T0_t/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.538797 t0-4.0.1/test/python/T0_t/RunConfig_t/
+-rw-r--r--   0 runner    (1001) docker     (127)    29995 2024-05-07 11:25:24.000000 t0-4.0.1/test/python/T0_t/RunConfig_t/Tier0Config_t.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.494797 t0-4.0.1/test/python/T0_t/WMBS_t/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.538797 t0-4.0.1/test/python/T0_t/WMBS_t/JobSplitting_t/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9117 2024-05-07 11:25:24.000000 t0-4.0.1/test/python/T0_t/WMBS_t/JobSplitting_t/Condition_t.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13792 2024-05-07 11:25:24.000000 t0-4.0.1/test/python/T0_t/WMBS_t/JobSplitting_t/ExpressMerge_t.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10553 2024-05-07 11:25:24.000000 t0-4.0.1/test/python/T0_t/WMBS_t/JobSplitting_t/Express_t.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27474 2024-05-07 11:25:24.000000 t0-4.0.1/test/python/T0_t/WMBS_t/JobSplitting_t/RepackMerge_t.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21397 2024-05-07 11:25:24.000000 t0-4.0.1/test/python/T0_t/WMBS_t/JobSplitting_t/Repack_t.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:25:38.538797 t0-4.0.1/test/python/T0_t/WMBS_t/RunConfig_t/
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-07 11:25:24.000000 t0-4.0.1/test/python/T0_t/WMBS_t/RunConfig_t/ExampleConfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   115065 2024-05-07 11:25:24.000000 t0-4.0.1/test/python/T0_t/WMBS_t/RunConfig_t/RunConfig_t.py
```

### Comparing `t0-3.1.6/LICENSE` & `t0-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/NOTICE` & `t0-4.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/ConditionUpload/ConditionUploadAPI.py` & `t0-4.0.1/src/python/T0/ConditionUpload/ConditionUploadAPI.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/ConditionUpload/upload.py` & `t0-4.0.1/src/python/T0/ConditionUpload/upload.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/JobSplitting/AlcaHarvest.py` & `t0-4.0.1/src/python/T0/JobSplitting/AlcaHarvest.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/JobSplitting/Condition.py` & `t0-4.0.1/src/python/T0/JobSplitting/Condition.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/JobSplitting/Express.py` & `t0-4.0.1/src/python/T0/JobSplitting/Express.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/JobSplitting/ExpressMerge.py` & `t0-4.0.1/src/python/T0/JobSplitting/ExpressMerge.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/JobSplitting/Repack.py` & `t0-4.0.1/src/python/T0/JobSplitting/Repack.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/JobSplitting/RepackMerge.py` & `t0-4.0.1/src/python/T0/JobSplitting/RepackMerge.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/RunConfig/RunConfigAPI.py` & `t0-4.0.1/src/python/T0/RunConfig/RunConfigAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,15 +442,16 @@
 
         for dataset, paths in list(datasetTriggers.items()):
 
             datasetConfig = retrieveDatasetConfig(tier0Config, dataset)
 
             selectEvents = []
             for path in sorted(paths):
-                selectEvents.append("%s:%s" % (path, runInfo['process']))
+                if path != "All":
+                    selectEvents.append("%s:%s" % (path, runInfo['process']))
 
             if streamConfig.ProcessingStyle == "Bulk":
                 dataTier = streamConfig.Repack.DataTier
                 outputModuleDetails.append( { 'dataTier' : dataTier,
                                               'eventContent' : "ALL",
                                               'selectEvents' : selectEvents,
                                               'primaryDataset' : dataset } )
```

### Comparing `t0-3.1.6/src/python/T0/RunConfig/Tier0Config.py` & `t0-4.0.1/src/python/T0/RunConfig/Tier0Config.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,21 +67,31 @@
 | |       |                             time trigger based on the run stop_time.
 | |       |
 | |       |--> DropBoxHost - Machine where we upload the PCL conditions to
 | |       |
 | |       |--> ValidationMode - Whether or not we upload conditions for immediate use
 | |       |                     in PromptReco or just for validation checks.
 | |       |
-| |       |--> ScramArches - Dictionary containig CMSSW release and corresponding ScramArch
+| |       |--> ScramArches - Dictionary containing CMSSW release and corresponding ScramArch
 | |       |
 | |       |--> DefaultScramArch - Default ScramArch if nothing else is specified for release
 | |       |
 | |       |--> BaseRequestPriority - Base for request priorities for PromptReco/Repack/Express
 | |       |
 | |       |--> DeploymentID - Unique identifier for every T0 Agent deployment
+| |       |
+| |       |--> extraStreamDatasetMap - Additional mapping to be applied on top of HLT menu. Unspecified
+| |       |                            path, means no event selection for this stream-dataset pair.
+| |       |                          mapping = {
+| |                                                 Stream0: {"Dataset": Dataset0}, 
+| |                                                 Stream1: {"Dataset": Dataset1
+| |                                                           "Path": Path1},
+| |                                                 Stream1: {"Dataset": Dataset2
+| |                                                           "Path": Path2},
+| |                                            }
 | |
 | |
 | |--> Streams - Configuration parameters that belong to a particular stream
 |       |
 |       | |--> Default - Configuration section for repacking defaults
 |       |                (configured just like a repack stream)
 |       |      
@@ -289,14 +299,16 @@
     tier0Config.Global.DQMDataTier = "DQMIO"
 
     tier0Config.Global.BaseRequestPriority = 150000
 
     tier0Config.Global.EnableUniqueWorkflowName = False
 
     tier0Config.Global.DeploymentID = 1
+    
+    tier0Config.Global.extraStreamDatasetMap = None
 
     return tier0Config
 
 def retrieveStreamConfig(config, streamName):
     """
     _retrieveStreamConfig_
     
@@ -695,14 +707,43 @@
     _setOverrideCatalog_
 
     Set the catalog to use in case override is necessary.
     """
     config.Global.overrideCatalog = overrideCatalog
     return
 
+def setExtraStreamDatasetMap(config, mapping):
+    """
+    _setExtraStreamDatasetMap_
+
+    Adds extra entries to HLT stream dataset mapping
+    """
+    
+    mapDict={}
+
+    for stream, description in list(mapping.items()):
+        dataset=description["Dataset"]
+        # Create dictionary for new streams
+        if stream not in mapDict:
+            mapDict[stream] = {}
+
+        # Add new datasets to stream
+        if dataset not in mapDict[stream]:
+            mapDict[stream][dataset] = []
+
+        # If defined, add path for event selection. "All" otherwise.
+        if "Path" in description:
+            mapDict[stream][dataset].append(description["Path"])
+        else:
+            mapDict[stream][dataset].append("All")
+
+
+    config.Global.extraStreamDatasetMap = mapDict
+    return
+
 
 def setSiteLocalConfig(config, siteLocalConfig):
     """
     _setSiteLocalConfig_
 
     Set the site local config file to use in case override is necessary.
     """
```

### Comparing `t0-3.1.6/src/python/T0/RunLumiCloseout/RunLumiCloseoutAPI.py` & `t0-4.0.1/src/python/T0/RunLumiCloseout/RunLumiCloseoutAPI.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/StorageManager/StorageManagerAPI.py` & `t0-4.0.1/src/python/T0/StorageManager/StorageManagerAPI.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/CompleteFiles.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/CompleteFiles.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/FinishPCLforEmptyExpress.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/FinishPCLforEmptyExpress.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/GetConditions.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/GetConditions.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/GetRunStopTime.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/GetRunStopTime.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/IsPromptCalibrationFinished.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/IsPromptCalibrationFinished.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/ConditionUpload/MarkPromptCalibrationFinished.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/ConditionUpload/MarkPromptCalibrationFinished.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Create.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Create.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/JobSplitting/InsertPromptCalibrationFile.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/JobSplitting/InsertPromptCalibrationFile.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/JobSplitting/InsertSplitLumis.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/JobSplitting/InsertSplitLumis.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/FindRecoRelease.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/FindRecoRelease.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/FindRecoReleaseDatasets.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/FindRecoReleaseDatasets.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetExpressConfig.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetExpressConfig.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetHLTConfig.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetHLTConfig.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetPhEDExConfig.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetPhEDExConfig.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetRecoConfig.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetRecoConfig.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetRepackConfig.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetRepackConfig.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetRunInfo.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetRunInfo.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasetTriggers.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasetTriggers.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasets.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasets.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetStreamOnlineVersion.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetStreamOnlineVersion.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/GetStreamStyle.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/GetStreamStyle.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertCMSSWVersion.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertCMSSWVersion.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetScenario.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetScenario.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetTrigger.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetTrigger.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertExpressConfig.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertExpressConfig.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertLumiSection.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertLumiSection.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertPhEDExConfig.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertPhEDExConfig.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertPrimaryDataset.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertPrimaryDataset.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertPromptCalibration.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertPromptCalibration.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoConfig.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoConfig.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoReleaseConfig.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoReleaseConfig.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertRepackConfig.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertRepackConfig.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertRun.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertRun.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertRunStreamDone.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertRunStreamDone.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertSpecialDataset.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertSpecialDataset.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStorageNode.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStorageNode.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStream.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStream.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamCMSSWVersion.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamCMSSWVersion.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamDataset.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamDataset.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamFileset.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamFileset.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamStyle.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamStyle.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamer.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamer.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertTrigger.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertTrigger.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/InsertWorkflowMonitoring.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/InsertWorkflowMonitoring.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/ReleasePromptReco.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/ReleasePromptReco.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunConfig/UpdateRun.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunConfig/UpdateRun.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckActiveSplitLumis.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckActiveSplitLumis.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckClosedLumis.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckClosedLumis.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckEndOfRunRecords.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckEndOfRunRecords.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRunStreamFilesets.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRunStreamFilesets.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRuns.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRuns.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/DeleteStreamers.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/DeleteStreamers.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FinalCloseLumi.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FinalCloseLumi.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindActiveRuns.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindActiveRuns.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedLumis.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedLumis.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedRuns.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedRuns.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindHighContLumi.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindHighContLumi.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindOpenRuns.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindOpenRuns.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindStoppedRuns.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindStoppedRuns.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/ForceCloseLumi.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/ForceCloseLumi.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetClosedLumisForStream.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetClosedLumisForStream.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFileCountOnOpenLumis.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFileCountOnOpenLumis.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFilesForStreamLumi.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFilesForStreamLumi.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetOpenRunStreamLumicount.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetOpenRunStreamLumicount.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/InsertClosedLumi.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/InsertClosedLumi.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/RunLumiCloseout/StopRuns.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/RunLumiCloseout/StopRuns.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/SMNotification/GetFinishedStreamers.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/SMNotification/GetFinishedStreamers.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/SMNotification/InsertOfflineFileStatus.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/SMNotification/InsertOfflineFileStatus.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/SMNotification/MarkStreamersFinished.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/SMNotification/MarkStreamersFinished.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/SMNotification/UpdateOfflineFileStatus.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/SMNotification/UpdateOfflineFileStatus.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/StorageManager/GetNewData.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/StorageManager/GetNewData.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/StorageManager/GetRunInfo.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/StorageManager/GetRunInfo.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/StorageManager/GetRunSetup.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/StorageManager/GetRunSetup.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetAllFiles.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetAllFiles.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableConditionFiles.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableConditionFiles.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressFiles.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressFiles.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressMergeFiles.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressMergeFiles.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackFiles.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackFiles.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackMergeFiles.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackMergeFiles.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepack.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepack.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepackMerge.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepackMerge.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/GetUsedLumis.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/GetUsedLumis.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/HaveAvailableFile.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/HaveAvailableFile.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Subscriptions/HaveJobGroup.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Subscriptions/HaveJobGroup.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetDatasetLocked.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetDatasetLocked.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetExpressConfigs.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetExpressConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetNewRun.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetNewRun.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetPromptRecoStatus.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetPromptRecoStatus.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetRecoConfigs.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetRecoConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetRunStreamDone.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetRunStreamDone.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/GetSkippedStreamers.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/GetSkippedStreamers.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertDatasetLocked.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertDatasetLocked.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertExpressConfigs.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertExpressConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertNewRun.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertNewRun.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoConfigs.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoLocked.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoLocked.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunDatasetDone.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunDatasetDone.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunStreamDone.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunStreamDone.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/InsertSkippedStreamers.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/InsertSkippedStreamers.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateDatasetLocked.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateDatasetLocked.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateExpressConfigs.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateExpressConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateNewRun.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateNewRun.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoConfigs.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoLocked.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoLocked.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunDatasetDone.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunDatasetDone.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunStreamDone.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunStreamDone.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateSkippedStreamers.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateSkippedStreamers.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/FeedStreamers.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/FeedStreamers.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewExpressRuns.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewExpressRuns.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRunStreams.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRunStreams.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRuns.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRuns.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetDeploymentID.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetDeploymentID.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetExpressReadyRuns.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetExpressReadyRuns.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetNotClosedOutWorkflows.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetNotClosedOutWorkflows.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetPromptRecoWorkflowsForMonitoring.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetPromptRecoWorkflowsForMonitoring.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetDone.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetDone.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetNew.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetNew.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetReleased.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetReleased.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/GetStreamerWorkflowsForMonitoring.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/GetStreamerWorkflowsForMonitoring.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkCloseoutWorkflowMonitoring.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkCloseoutWorkflowMonitoring.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkTrackedWorkflowMonitoring.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkTrackedWorkflowMonitoring.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkWorkflowsInjected.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkWorkflowsInjected.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/ReleaseExpress.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/ReleaseExpress.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/SetDeploymentID.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/SetDeploymentID.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0/WMBS/Oracle/Tier0Feeder/UpdateRecoReleaseConfigs.py` & `t0-4.0.1/src/python/T0/WMBS/Oracle/Tier0Feeder/UpdateRecoReleaseConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0Component/Tier0Auditor/Tier0Auditor.py` & `t0-4.0.1/src/python/T0Component/Tier0Auditor/Tier0Auditor.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0Component/Tier0Auditor/Tier0AuditorPoller.py` & `t0-4.0.1/src/python/T0Component/Tier0Auditor/Tier0AuditorPoller.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0Component/Tier0Feeder/Tier0Feeder.py` & `t0-4.0.1/src/python/T0Component/Tier0Feeder/Tier0Feeder.py`

 * *Files identical despite different names*

### Comparing `t0-3.1.6/src/python/T0Component/Tier0Feeder/Tier0FeederPoller.py` & `t0-4.0.1/src/python/T0Component/Tier0Feeder/Tier0FeederPoller.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,18 @@
 
                 # local runs have no hltkey and are configured differently
                 if hltkey != None:
 
                     # retrieve HLT configuration and make sure it's usable
                     try:
                         hltConfig = self.getHLTConfigDAO.execute(hltkey, transaction = False)
+                        # If defined, add additional mapping entries
+                        if tier0Config.Global.extraStreamDatasetMap:
+                            hltConfig['mapping'].update(tier0Config.Global.extraStreamDatasetMap)
+                            logging.debug("Modified Mapping: %s", hltConfig)
                         if hltConfig['process'] == None or len(hltConfig['mapping']) == 0:
                             raise RuntimeError("HLTConfDB query returned no process or mapping")
                     except:
                         logging.exception("Can't retrieve hltkey %s for run %d" % (hltkey, run))
                         continue
 
                 try:
```

