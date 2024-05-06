# Comparing `tmp/naxtopy-2.0.0.tar.gz` & `tmp/naxtopy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naxtopy-2.0.0.tar", last modified: Fri Apr 19 07:28:20 2024, max compression
+gzip compressed data, was "naxtopy-2.0.1.tar", last modified: Mon May  6 22:16:42 2024, max compression
```

## Comparing `naxtopy-2.0.0.tar` & `naxtopy-2.0.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.808955 naxtopy-2.0.0/
--rw-rw-rw-   0        0        0     5368 2024-04-08 09:50:46.000000 naxtopy-2.0.0/LICENSE
--rw-rw-rw-   0        0        0    21374 2024-04-19 07:28:20.814478 naxtopy-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    14232 2024-03-21 12:25:22.000000 naxtopy-2.0.0/README.md
--rw-rw-rw-   0        0        0     1143 2024-03-04 15:18:14.000000 naxtopy-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 07:28:20.826789 naxtopy-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      462 2024-01-18 10:36:31.000000 naxtopy-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.176955 naxtopy-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.182955 naxtopy-2.0.0/src/NaxToPy/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.193955 naxtopy-2.0.0/src/NaxToPy/Core/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.185955 naxtopy-2.0.0/src/NaxToPy/Core/Classes/
--rw-rw-rw-   0        0        0      765 2024-02-13 12:32:13.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/AllClasses.py
--rw-rw-rw-   0        0        0    24803 2024-03-12 11:50:17.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PComponent.py
--rw-rw-rw-   0        0        0     4555 2023-12-18 10:36:26.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PConnector.py
--rw-rw-rw-   0        0        0     2006 2023-12-18 10:36:26.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PCoord.py
--rw-rw-rw-   0        0        0     6772 2024-03-04 14:59:02.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PElement.py
--rw-rw-rw-   0        0        0     6094 2024-03-04 14:59:02.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PFreeBody.py
--rw-rw-rw-   0        0        0     3351 2024-03-12 11:33:59.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PIncrement.py
--rw-rw-rw-   0        0        0    12323 2024-04-19 07:02:20.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PLoadCase.py
--rw-rw-rw-   0        0        0    16923 2023-12-18 10:36:26.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PMaterial.py
--rw-rw-rw-   0        0        0   355653 2024-04-09 15:09:23.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PModelInputData.py
--rw-rw-rw-   0        0        0     7335 2024-03-04 14:59:02.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PNode.py
--rw-rw-rw-   0        0        0    12012 2023-11-29 11:18:13.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PProperty.py
--rw-rw-rw-   0        0        0     6118 2024-04-12 06:30:49.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PReport.py
--rw-rw-rw-   0        0        0    12237 2024-04-15 08:18:55.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PResult.py
--rw-rw-rw-   0        0        0     2044 2023-12-18 10:36:26.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PSection.py
--rw-rw-rw-   0        0        0     2777 2023-09-21 06:53:42.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PSet.py
--rw-rw-rw-   0        0        0      708 2023-06-14 08:40:16.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/ProgresBar.py
--rw-rw-rw-   0        0        0        2 2023-01-27 14:45:07.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.188955 naxtopy-2.0.0/src/NaxToPy/Core/Constants/
--rw-rw-rw-   0        0        0     1583 2024-04-19 07:27:53.000000 naxtopy-2.0.0/src/NaxToPy/Core/Constants/Constants.py
--rw-rw-rw-   0        0        0        2 2023-01-23 07:52:14.000000 naxtopy-2.0.0/src/NaxToPy/Core/Constants/__init__.py
--rw-rw-rw-   0        0        0    16398 2023-05-30 07:39:47.000000 naxtopy-2.0.0/src/NaxToPy/Core/Constants/librerias.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.191955 naxtopy-2.0.0/src/NaxToPy/Core/Errors/
--rw-rw-rw-   0        0        0     1420 2023-05-25 07:57:17.000000 naxtopy-2.0.0/src/NaxToPy/Core/Errors/N2PColors.py
--rw-rw-rw-   0        0        0     2205 2023-10-19 09:23:23.000000 naxtopy-2.0.0/src/NaxToPy/Core/Errors/N2PFileHandler.py
--rw-rw-rw-   0        0        0    52152 2024-04-19 07:02:20.000000 naxtopy-2.0.0/src/NaxToPy/Core/Errors/N2PLog.py
--rw-rw-rw-   0        0        0        2 2023-01-23 07:52:14.000000 naxtopy-2.0.0/src/NaxToPy/Core/Errors/__init__.py
--rw-rw-rw-   0        0        0    74013 2024-04-19 07:02:20.000000 naxtopy-2.0.0/src/NaxToPy/Core/N2PModelContent.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.193955 naxtopy-2.0.0/src/NaxToPy/Core/Reference_Finder/
--rw-rw-rw-   0        0        0    10217 2024-04-03 13:12:21.000000 naxtopy-2.0.0/src/NaxToPy/Core/Reference_Finder/__Reference_Finder.py
--rw-rw-rw-   0        0        0        2 2023-01-20 07:41:18.000000 naxtopy-2.0.0/src/NaxToPy/Core/Reference_Finder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.196955 naxtopy-2.0.0/src/NaxToPy/Core/_AuxFunc/
--rw-rw-rw-   0        0        0     3627 2024-01-04 10:24:30.000000 naxtopy-2.0.0/src/NaxToPy/Core/_AuxFunc/_NetToPython.py
--rw-rw-rw-   0        0        0        2 2022-11-22 11:07:36.000000 naxtopy-2.0.0/src/NaxToPy/Core/_AuxFunc/__init__.py
--rw-rw-rw-   0        0        0      183 2024-01-18 10:12:28.000000 naxtopy-2.0.0/src/NaxToPy/Core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.205955 naxtopy-2.0.0/src/NaxToPy/Modules/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.202955 naxtopy-2.0.0/src/NaxToPy/Modules/Fasteners/
--rw-rw-rw-   0        0        0    41254 2024-03-05 10:31:16.000000 naxtopy-2.0.0/src/NaxToPy/Modules/Fasteners/N2PUpdateFastener.py
--rw-rw-rw-   0        0        0       50 2024-03-04 09:43:21.000000 naxtopy-2.0.0/src/NaxToPy/Modules/Fasteners/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.205955 naxtopy-2.0.0/src/NaxToPy/Modules/N2PEnvelope/
--rw-rw-rw-   0        0        0     4216 2024-03-04 14:59:02.000000 naxtopy-2.0.0/src/NaxToPy/Modules/N2PEnvelope/N2PEnvelope.py
--rw-rw-rw-   0        0        0        0 2023-07-11 07:33:21.000000 naxtopy-2.0.0/src/NaxToPy/Modules/N2PEnvelope/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.208955 naxtopy-2.0.0/src/NaxToPy/Modules/N2PtoEXE/
--rw-rw-rw-   0        0        0     7791 2024-04-03 09:13:01.000000 naxtopy-2.0.0/src/NaxToPy/Modules/N2PtoEXE/N2PtoEXE.py
--rw-rw-rw-   0        0        0        2 2023-03-30 09:33:43.000000 naxtopy-2.0.0/src/NaxToPy/Modules/N2PtoEXE/__init__.py
--rw-rw-rw-   0        0        0       50 2024-03-04 09:52:33.000000 naxtopy-2.0.0/src/NaxToPy/Modules/__init__.py
--rw-rw-rw-   0        0        0   198996 2023-04-14 09:43:58.000000 naxtopy-2.0.0/src/NaxToPy/NaxToPy.ico
--rw-rw-rw-   0        0        0      487 2024-02-13 12:32:13.000000 naxtopy-2.0.0/src/NaxToPy/__init__.py
--rw-rw-rw-   0        0        0     7882 2024-01-02 09:26:08.000000 naxtopy-2.0.0/src/NaxToPy/user_functions.txt
-drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.179955 naxtopy-2.0.0/src/NaxToPy.egg-info/
--rw-rw-rw-   0        0        0    21374 2024-04-19 07:28:20.000000 naxtopy-2.0.0/src/NaxToPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1813 2024-04-19 07:28:20.000000 naxtopy-2.0.0/src/NaxToPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:28:20.000000 naxtopy-2.0.0/src/NaxToPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-19 07:28:20.000000 naxtopy-2.0.0/src/NaxToPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-19 07:28:20.000000 naxtopy-2.0.0/src/NaxToPy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:44.821787 naxtopy-2.0.1/
+-rw-rw-rw-   0        0        0     5368 2024-04-08 09:50:46.000000 naxtopy-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0    21783 2024-05-06 22:16:45.105085 naxtopy-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14641 2024-05-06 22:08:57.000000 naxtopy-2.0.1/README.md
+-rw-rw-rw-   0        0        0     1143 2024-05-06 22:09:27.000000 naxtopy-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 22:16:46.436812 naxtopy-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      462 2024-01-18 10:36:31.000000 naxtopy-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:15:31.621787 naxtopy-2.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 22:15:40.280787 naxtopy-2.0.1/src/NaxToPy/
+drwxrwxrwx   0        0        0        0 2024-05-06 22:15:46.364787 naxtopy-2.0.1/src/NaxToPy/Core/
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:15.019787 naxtopy-2.0.1/src/NaxToPy/Core/Classes/
+-rw-rw-rw-   0        0        0      765 2024-02-13 12:32:13.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/AllClasses.py
+-rw-rw-rw-   0        0        0    24803 2024-03-12 11:50:17.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PComponent.py
+-rw-rw-rw-   0        0        0     4555 2023-12-18 10:36:26.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PConnector.py
+-rw-rw-rw-   0        0        0     2006 2023-12-18 10:36:26.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PCoord.py
+-rw-rw-rw-   0        0        0     6772 2024-03-04 14:59:02.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PElement.py
+-rw-rw-rw-   0        0        0     6094 2024-03-04 14:59:02.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PFreeBody.py
+-rw-rw-rw-   0        0        0     3351 2024-03-12 11:33:59.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PIncrement.py
+-rw-rw-rw-   0        0        0    13464 2024-05-06 21:55:45.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PLoadCase.py
+-rw-rw-rw-   0        0        0    16923 2023-12-18 10:36:26.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PMaterial.py
+-rw-rw-rw-   0        0        0   355653 2024-04-09 15:09:23.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PModelInputData.py
+-rw-rw-rw-   0        0        0     7335 2024-03-04 14:59:02.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PNode.py
+-rw-rw-rw-   0        0        0    12012 2023-11-29 11:18:13.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PProperty.py
+-rw-rw-rw-   0        0        0     6118 2024-04-12 06:30:49.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PReport.py
+-rw-rw-rw-   0        0        0    12237 2024-04-15 08:18:55.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PResult.py
+-rw-rw-rw-   0        0        0     2044 2023-12-18 10:36:26.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PSection.py
+-rw-rw-rw-   0        0        0     2777 2023-09-21 06:53:42.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PSet.py
+-rw-rw-rw-   0        0        0      708 2023-06-14 08:40:16.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/ProgresBar.py
+-rw-rw-rw-   0        0        0        2 2023-01-27 14:45:07.000000 naxtopy-2.0.1/src/NaxToPy/Core/Classes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:19.344787 naxtopy-2.0.1/src/NaxToPy/Core/Constants/
+-rw-rw-rw-   0        0        0     1594 2024-05-06 14:47:00.000000 naxtopy-2.0.1/src/NaxToPy/Core/Constants/Constants.py
+-rw-rw-rw-   0        0        0        2 2023-01-23 07:52:14.000000 naxtopy-2.0.1/src/NaxToPy/Core/Constants/__init__.py
+-rw-rw-rw-   0        0        0    16398 2023-05-30 07:39:47.000000 naxtopy-2.0.1/src/NaxToPy/Core/Constants/librerias.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:24.626787 naxtopy-2.0.1/src/NaxToPy/Core/Errors/
+-rw-rw-rw-   0        0        0     1420 2023-05-25 07:57:17.000000 naxtopy-2.0.1/src/NaxToPy/Core/Errors/N2PColors.py
+-rw-rw-rw-   0        0        0     2205 2023-10-19 09:23:23.000000 naxtopy-2.0.1/src/NaxToPy/Core/Errors/N2PFileHandler.py
+-rw-rw-rw-   0        0        0    52823 2024-05-06 15:12:31.000000 naxtopy-2.0.1/src/NaxToPy/Core/Errors/N2PLog.py
+-rw-rw-rw-   0        0        0        2 2023-01-23 07:52:14.000000 naxtopy-2.0.1/src/NaxToPy/Core/Errors/__init__.py
+-rw-rw-rw-   0        0        0    77318 2024-04-19 07:10:42.000000 naxtopy-2.0.1/src/NaxToPy/Core/N2PModelContent.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:27.324787 naxtopy-2.0.1/src/NaxToPy/Core/Reference_Finder/
+-rw-rw-rw-   0        0        0    10183 2024-05-06 15:20:39.000000 naxtopy-2.0.1/src/NaxToPy/Core/Reference_Finder/__Reference_Finder.py
+-rw-rw-rw-   0        0        0        2 2023-01-20 07:41:18.000000 naxtopy-2.0.1/src/NaxToPy/Core/Reference_Finder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:31.128787 naxtopy-2.0.1/src/NaxToPy/Core/_AuxFunc/
+-rw-rw-rw-   0        0        0     3627 2024-01-04 10:24:30.000000 naxtopy-2.0.1/src/NaxToPy/Core/_AuxFunc/_NetToPython.py
+-rw-rw-rw-   0        0        0        2 2022-11-22 11:07:36.000000 naxtopy-2.0.1/src/NaxToPy/Core/_AuxFunc/__init__.py
+-rw-rw-rw-   0        0        0      183 2024-01-18 10:12:28.000000 naxtopy-2.0.1/src/NaxToPy/Core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:32.949787 naxtopy-2.0.1/src/NaxToPy/Modules/
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:36.793787 naxtopy-2.0.1/src/NaxToPy/Modules/Fasteners/
+-rw-rw-rw-   0        0        0    41254 2024-03-05 10:31:16.000000 naxtopy-2.0.1/src/NaxToPy/Modules/Fasteners/N2PUpdateFastener.py
+-rw-rw-rw-   0        0        0       50 2024-03-04 09:43:21.000000 naxtopy-2.0.1/src/NaxToPy/Modules/Fasteners/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:39.373787 naxtopy-2.0.1/src/NaxToPy/Modules/N2PEnvelope/
+-rw-rw-rw-   0        0        0     4216 2024-03-04 14:59:02.000000 naxtopy-2.0.1/src/NaxToPy/Modules/N2PEnvelope/N2PEnvelope.py
+-rw-rw-rw-   0        0        0        0 2023-07-11 07:33:21.000000 naxtopy-2.0.1/src/NaxToPy/Modules/N2PEnvelope/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:41.730787 naxtopy-2.0.1/src/NaxToPy/Modules/N2PtoEXE/
+-rw-rw-rw-   0        0        0     7791 2024-04-03 09:13:01.000000 naxtopy-2.0.1/src/NaxToPy/Modules/N2PtoEXE/N2PtoEXE.py
+-rw-rw-rw-   0        0        0        2 2023-03-30 09:33:43.000000 naxtopy-2.0.1/src/NaxToPy/Modules/N2PtoEXE/__init__.py
+-rw-rw-rw-   0        0        0       50 2024-03-04 09:52:33.000000 naxtopy-2.0.1/src/NaxToPy/Modules/__init__.py
+-rw-rw-rw-   0        0        0   198996 2023-04-14 09:43:58.000000 naxtopy-2.0.1/src/NaxToPy/NaxToPy.ico
+-rw-rw-rw-   0        0        0      487 2024-02-13 12:32:13.000000 naxtopy-2.0.1/src/NaxToPy/__init__.py
+-rw-rw-rw-   0        0        0     7882 2024-01-02 09:26:08.000000 naxtopy-2.0.1/src/NaxToPy/user_functions.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 22:16:44.197787 naxtopy-2.0.1/src/NaxToPy.egg-info/
+-rw-rw-rw-   0        0        0    21783 2024-05-06 22:15:27.000000 naxtopy-2.0.1/src/NaxToPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1813 2024-05-06 22:15:30.000000 naxtopy-2.0.1/src/NaxToPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 22:15:28.000000 naxtopy-2.0.1/src/NaxToPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-06 22:15:28.000000 naxtopy-2.0.1/src/NaxToPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 22:15:28.000000 naxtopy-2.0.1/src/NaxToPy.egg-info/top_level.txt
```

### Comparing `naxtopy-2.0.0/LICENSE` & `naxtopy-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/PKG-INFO` & `naxtopy-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NaxToPy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Package for postprocessing FEM results in Python
 Home-page: https://www.idaerosolutions.com/Home/NaxToPy
 Download-URL: https://apps.microsoft.com/detail/XP9MMH0KDKGRJN?hl=en-US&gl=US
 Author-email: Idaero Solutions <manuel.sanchez@idaerosolutions.com>
 License: Copyright (c) 2024 Idaero Solutions
         
         This freeware license agreement (“agreement”) is a legally binding contract
@@ -131,35 +131,38 @@
 
 ![](https://idaerosolutions.com/images/icons/Logo_NaxToPy_Black.svg "NaxToPy")
 
 # NaxToPy
 
 **NaxToPy** is the [**NaxTo**](https://apps.microsoft.com/detail/XP9MMH0KDKGRJN?hl=en-US&gl=US)
 library designed for Python, which allows reading and manipulating FEM
-analysis results files from the most common tools: Nastran (op2, xdb, h5), Abaqus (odb), Optistruct
-(h3d, op2) and Ansys (rst); and stores them in a user-friendly Python structure. Additionally, it
-can read input files from Nastran (bdf, fem) and change it contents.
+analysis results files from the most common tools: Nastran (.op2, .xdb, .h5), Abaqus (odb), Optistruct
+(.h3d, .op2) and Ansys (.rst); and stores them in a user-friendly Python structure. Additionally, it
+can read input files from Nastran (.bdf, .fem) and change their contents.
 
 It could be easily combined with other Python packages as Matplotlib or Pandas. This provides access
 to the full coding power of Python to interpret and process the results, without the need to install
 any additional software other than having NaxTo already installed (see the _Download_ and _Homepage_
 links on the left).
 
 **NaxToPy** is a powerful tool for FEM analysis post-processing!
 
 **CAUTION:** To use NaxToPy, [**NaxTo**](https://apps.microsoft.com/detail/XP9MMH0KDKGRJN?hl=en-US&gl=US) must be installed.
-This version is compatible with **NaxTo 2024.1**. It may be compatible with all the steps of this version (2024.1.0, 2024.1.1, 2024.1.2, etc.).
+This version is compatible with **NaxTo 2024.1**. It is compatible with all the steps of this version (2024.1.0, 2024.1.1, 2024.1.2, etc.).
 Check in _Programs and Features_ the NaxTo version that is installed. 
 
 ## Installation
 
+If python is installed and `pip` is added to the PATH:
 
-If python is callable from the command line:
+`pip install NaxToPy`
+
+An alternative, if Python is callable from the command line:
 
-`py -m pip install NaxToPy`
+`python -m pip install NaxToPy`
 
 For **Visual Studio** users:
 - Open "Python Environments" window
 - Change the "general information" label to "Packages(Pypi)"
 - Write the name of the package and press enter:
 
 - `NaxToPy` + enter
@@ -175,15 +178,15 @@
       import sys
       sys.path.append("...\directory")
       import NaxToPy as n2p
 ## Updating NaxToPy
 
 If python is callable from the command line:
 
-`py -m pip install -U NaxToPy`
+`python -m pip install -U NaxToPy`
 
 For Visual Studio users:
 - Open "Python Environments" window
 - Change the "general information" label to "Packages(Pypi)"
 - Write the following command on the search bar and press enter:
 
   `-U NaxToPy` + enter
@@ -256,14 +259,20 @@
 the LoadCases that are critical or the Increment that is critical instead of the value.
 
 ### v.2.0.0
 1. Changes made to align the library with updates in lower-level dependencies.
 2. New internal methods to look for the compatibility with low-level dependencies.
 3. The name of the .log is now NaxToPy_Year-Month-Day.log.
 
+### v.2.0.1
+1. The compatibility is extended to all NaxTo steps of the same version.
+2. The property N2PLoadCase.ActiveIncrement is subtitued by N2PLoadCase.ActiveN2PIncrement.
+It uses an object instaed of an int.
+3. Update of the examples of some docstrings.
+
 # Documentation
 
 **NaxToPy** is a package developed by Idaero Solutions© as a part of the **NaxTo** software.
 
 NaxToPy only use three dependeces:
 - NumPy: https://numpy.org/
 - PythonNET: https://pythonnet.github.io/
@@ -335,15 +344,15 @@
 # Load the list of load cases as N2PLoadCase object
 loadcaseslist = model.LoadCases
 
 # Look for the Load Case with the name pressure
 pressure_lc = model.get_load_case("pressure")
 
 # Change the active increment (by default is the last one):
-pressure_lc.ActiveIncrement = 10
+pressure_lc.ActiveN2PIncrement = pressure_lc.get_increment(10)
 
 # Look for all results
 all_results = pressure_lc.Results
 
 # Look for the Result with the name DISPLACEMENT
 displacement = pressure_lc.get_result("DISPLACEMENT")
```

### Comparing `naxtopy-2.0.0/README.md` & `naxtopy-2.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,35 +7,38 @@
 
 ![](https://idaerosolutions.com/images/icons/Logo_NaxToPy_Black.svg "NaxToPy")
 
 # NaxToPy
 
 **NaxToPy** is the [**NaxTo**](https://apps.microsoft.com/detail/XP9MMH0KDKGRJN?hl=en-US&gl=US)
 library designed for Python, which allows reading and manipulating FEM
-analysis results files from the most common tools: Nastran (op2, xdb, h5), Abaqus (odb), Optistruct
-(h3d, op2) and Ansys (rst); and stores them in a user-friendly Python structure. Additionally, it
-can read input files from Nastran (bdf, fem) and change it contents.
+analysis results files from the most common tools: Nastran (.op2, .xdb, .h5), Abaqus (odb), Optistruct
+(.h3d, .op2) and Ansys (.rst); and stores them in a user-friendly Python structure. Additionally, it
+can read input files from Nastran (.bdf, .fem) and change their contents.
 
 It could be easily combined with other Python packages as Matplotlib or Pandas. This provides access
 to the full coding power of Python to interpret and process the results, without the need to install
 any additional software other than having NaxTo already installed (see the _Download_ and _Homepage_
 links on the left).
 
 **NaxToPy** is a powerful tool for FEM analysis post-processing!
 
 **CAUTION:** To use NaxToPy, [**NaxTo**](https://apps.microsoft.com/detail/XP9MMH0KDKGRJN?hl=en-US&gl=US) must be installed.
-This version is compatible with **NaxTo 2024.1**. It may be compatible with all the steps of this version (2024.1.0, 2024.1.1, 2024.1.2, etc.).
+This version is compatible with **NaxTo 2024.1**. It is compatible with all the steps of this version (2024.1.0, 2024.1.1, 2024.1.2, etc.).
 Check in _Programs and Features_ the NaxTo version that is installed. 
 
 ## Installation
 
+If python is installed and `pip` is added to the PATH:
 
-If python is callable from the command line:
+`pip install NaxToPy`
+
+An alternative, if Python is callable from the command line:
 
-`py -m pip install NaxToPy`
+`python -m pip install NaxToPy`
 
 For **Visual Studio** users:
 - Open "Python Environments" window
 - Change the "general information" label to "Packages(Pypi)"
 - Write the name of the package and press enter:
 
 - `NaxToPy` + enter
@@ -51,15 +54,15 @@
       import sys
       sys.path.append("...\directory")
       import NaxToPy as n2p
 ## Updating NaxToPy
 
 If python is callable from the command line:
 
-`py -m pip install -U NaxToPy`
+`python -m pip install -U NaxToPy`
 
 For Visual Studio users:
 - Open "Python Environments" window
 - Change the "general information" label to "Packages(Pypi)"
 - Write the following command on the search bar and press enter:
 
   `-U NaxToPy` + enter
@@ -132,14 +135,20 @@
 the LoadCases that are critical or the Increment that is critical instead of the value.
 
 ### v.2.0.0
 1. Changes made to align the library with updates in lower-level dependencies.
 2. New internal methods to look for the compatibility with low-level dependencies.
 3. The name of the .log is now NaxToPy_Year-Month-Day.log.
 
+### v.2.0.1
+1. The compatibility is extended to all NaxTo steps of the same version.
+2. The property N2PLoadCase.ActiveIncrement is subtitued by N2PLoadCase.ActiveN2PIncrement.
+It uses an object instaed of an int.
+3. Update of the examples of some docstrings.
+
 # Documentation
 
 **NaxToPy** is a package developed by Idaero Solutions© as a part of the **NaxTo** software.
 
 NaxToPy only use three dependeces:
 - NumPy: https://numpy.org/
 - PythonNET: https://pythonnet.github.io/
@@ -211,15 +220,15 @@
 # Load the list of load cases as N2PLoadCase object
 loadcaseslist = model.LoadCases
 
 # Look for the Load Case with the name pressure
 pressure_lc = model.get_load_case("pressure")
 
 # Change the active increment (by default is the last one):
-pressure_lc.ActiveIncrement = 10
+pressure_lc.ActiveN2PIncrement = pressure_lc.get_increment(10)
 
 # Look for all results
 all_results = pressure_lc.Results
 
 # Look for the Result with the name DISPLACEMENT
 displacement = pressure_lc.get_result("DISPLACEMENT")
```

### Comparing `naxtopy-2.0.0/pyproject.toml` & `naxtopy-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 733e 3d36 372e 382e 3022  uptools>=67.8.0"
 00000030: 5d0d 0a62 7569 6c64 2d62 6163 6b65 6e64  ]..build-backend
 00000040: 203d 2022 7365 7475 7074 6f6f 6c73 2e62   = "setuptools.b
 00000050: 7569 6c64 5f6d 6574 6122 0d0a 0d0a 5b70  uild_meta"....[p
 00000060: 726f 6a65 6374 5d0d 0a6e 616d 6520 3d20  roject]..name = 
 00000070: 224e 6178 546f 5079 220d 0a76 6572 7369  "NaxToPy"..versi
-00000080: 6f6e 203d 2022 322e 302e 3022 0d0a 6c69  on = "2.0.0"..li
+00000080: 6f6e 203d 2022 322e 302e 3122 0d0a 6c69  on = "2.0.1"..li
 00000090: 6365 6e73 6520 3d20 7b66 696c 6520 3d20  cense = {file = 
 000000a0: 224c 4943 454e 5345 227d 0d0a 6175 7468  "LICENSE"}..auth
 000000b0: 6f72 7320 3d20 5b20 7b20 6e61 6d65 203d  ors = [ { name =
 000000c0: 2022 4964 6165 726f 2053 6f6c 7574 696f   "Idaero Solutio
 000000d0: 6e73 222c 2065 6d61 696c 203d 2022 6d61  ns", email = "ma
 000000e0: 6e75 656c 2e73 616e 6368 657a 4069 6461  nuel.sanchez@ida
 000000f0: 6572 6f73 6f6c 7574 696f 6e73 2e63 6f6d  erosolutions.com
```

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/AllClasses.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/AllClasses.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PComponent.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PComponent.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PConnector.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PConnector.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PCoord.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PCoord.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PElement.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PElement.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PFreeBody.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PFreeBody.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PIncrement.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PIncrement.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PLoadCase.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PLoadCase.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,36 +115,56 @@
     @property
     def Name(self) -> str:
         return(str(self.__namelc__))
     # ------------------------------------------------------------------------------------------------------------------
 
     # Metodo para obtener el incremento activo. Influye en la funcion de llamada a get_result_array
     @property
-    def ActiveIncrement(self) -> str:
-        ''' Returns the active increment of the load case. By default, is the last one.'''
+    def ActiveIncrement(self) -> int:
+        """DEPRECATED PROPERTY. Use ActiveN2PIncrement.ID instaed. Returns the active increment of the load case. By
+        default, is the last one."""
+        N2PLog.Warning.W206()
         return self.__activeIncrement__
     # ------------------------------------------------------------------------------------------------------------------
 
-    # Metodo para obtener el incremento activo. Influye en la funcion de llamada a get_result_array
+    # Metodo para establecer el incremento activo. Influye en la funcion de llamada a get_result_array
     @ActiveIncrement.setter
     def ActiveIncrement(self, id: Union[int, str]) -> None:
-        ''' Sets the active increment of the load case. By defult is the last one.
+        ''' DEPRECATED PROPERTY. Use ActiveN2PIncrement instead. Sets the active increment of the load case. By defult is the last one.
 
         Args:
             id: int | str -> ID or Name of the N2PIncrement
         '''
         activincrement = self.get_increments(id).ID
 
         if activincrement is not None:
             self.__activeIncrement__ = activincrement
             N2PLog.Info.I202(id)
         else:
             N2PLog.Error.E207(id)
     # ------------------------------------------------------------------------------------------------------------------
 
+    # Metodo para obtener el incremento activo. Influye en la funcion de llamada a get_result_array
+    @property
+    def ActiveN2PIncrement(self) -> N2PIncrement:
+        """Returns the active increment of the load case. By default, is the last one."""
+        return self.get_increments(self.__activeIncrement__)
+    # ------------------------------------------------------------------------------------------------------------------
+
+    # Metodo para establecer el incremento activo. Influye en la funcion de llamada a get_result_array
+    @ActiveN2PIncrement.setter
+    def ActiveN2PIncrement(self, incr: N2PIncrement) -> None:
+        """Sets the active increment of the load case. By defult is the last one.
+
+        Args:
+            incr: N2PIncrement -> ID or Name of the N2PIncrement
+        """
+        self.__activeIncrement__ = incr.ID
+    # ------------------------------------------------------------------------------------------------------------------
+
     # Metodo como propiedad que devuelve todos los N2PResult. Es igual que llamar a get_results sin
     # parametros
     @property
     def Results(self) -> dict[str, N2PResult]:
         return self.__results__
 
     # Metodo para obtener el tipo de solucion del modelo ---------------------------------------------------------------
```

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PMaterial.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PMaterial.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PModelInputData.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PModelInputData.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PNode.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PNode.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PProperty.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PProperty.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PReport.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PReport.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PResult.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PResult.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PSection.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PSection.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PSet.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/N2PSet.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Classes/ProgresBar.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Classes/ProgresBar.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Constants/Constants.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Constants/Constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Constants of the NaxToPy package"""
 
 # NaxToPy Version
-VERSION = "2.0.0"
+VERSION = "2.0.1"
 
 # Supported for Naxto:
 NAXTO_VERSION = '2024R1'
-NAXTO_STEP = "0"
+NAXTO_STEP = "2"
 
 # Assembly version of NaxToModel.dll
-VIZZER_COMPATIBILITY = ("4.1.0.0", "4.1.0.1")
+VIZZER_COMPATIBILITY = ("4.1.0.0", "4.1.0.1", "4.1.0.2")
 """Tuple with the compatible versions of NaxToModel.dll"""
 
 # PYTHON EXTERNO ----------------------------------------------------------------------------------
 # Versiones de Python soportadas:
 SUP_PY_VER = (9, 10, 11, 12)
 
 # Librerias Externas de Python
```

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Constants/librerias.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Constants/librerias.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Errors/N2PColors.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Errors/N2PColors.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Errors/N2PFileHandler.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Errors/N2PFileHandler.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Errors/N2PLog.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Errors/N2PLog.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,14 +149,20 @@
         @staticmethod
         def D103(parallel) -> None:
             """Method that shows the parallel option set at low level"""
             message = f"The parallel processing has been set to {parallel}"
             N2PLog._N2PLog__logger.debug(message)
 
         @staticmethod
+        def D200(assembly) -> None:
+            """Message that shows the assembly version of the core library"""
+            message = f"The assembly version is: {assembly}"
+            N2PLog._N2PLog__logger.debug(message)
+
+        @staticmethod
         def D500(current_time,tinit) -> None:
             """ Information given for the extraction time.
             """
             message = f"D500: Extraction time: {current_time-tinit} s"
             N2PLog._N2PLog__logger.info(message)
 
         @staticmethod
@@ -440,14 +446,22 @@
         def W205() -> None:
             """ Warning raised when there the Deprecated function "Initialize" is called.
             """
             message = f"W205: Initialize is a deprecated function. Please, use load_model instead"
             N2PLog._N2PLog__logger.warning(message)
 
         @staticmethod
+        def W206() -> None:
+            """ Warning raised when there the Deprecated property "ActiveIncrement" is called.
+            """
+            message = f"W206: ActiveIncrement is a deprecated property. Please, ActiveN2pIncrement to obtain a " \
+                      f"N2PIncrement or ActiveN2pIncrement.ID to obtain the ID"
+            N2PLog._N2PLog__logger.warning(message)
+
+        @staticmethod
         def W300() -> None:
             """ Warning raised when there are more dimensions than points in n2p.envelope
             """
             message = f"W300: there are more dimensions than points as arguments in n2p.envelope"
             N2PLog._N2PLog__logger.warning(message)
 
         @staticmethod
```

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/N2PModelContent.py` & `naxtopy-2.0.1/src/NaxToPy/Core/N2PModelContent.py`

 * *Files 10% similar despite different names*

```diff
@@ -869,14 +869,22 @@
             nodes: list[N2PNode]
             elements: list[N2PElement]
             outpoint: tuple[float]
             coordsysout: N2PCoord
 
         Returns:
             freebody: N2PFreeBody
+
+        Example:
+            >>> model = load_model("model.op2")
+            >>> lc = model.get_load_case(5)
+            >>> incr = lc.ActiveN2PIncrement
+            >>> node_list = model.get_nodes([1000, 1001, 1002, 1003, 1004, 1005])
+            >>> elem_list = model.get_elements([1000, 1001, 1002, 1003, 1004])
+
         """
 
         if increment is None:
             increment = loadcase.get_increments(loadcase.ActiveIncrement)
 
         return N2PFreeBody(name, loadcase, increment, nodes, elements, self, coordsysout, outpoint)
     # ------------------------------------------------------------------------------------------------------------------
@@ -905,14 +913,21 @@
         """ Method of N2PModelContent that reads an output result file from Nastran, Abaqus, Optistruct or Ansys and
          add the results to the N2PModelContent Object.
 
             Supports .op2, .xdb, .odb, .h5, .h3d and .rst file extensions read from a local filesystem or URL.
 
             Args:
                 results_files: list[str, ...]
+
+            Example:
+                >>> model1 = load_model("model1_lc1.odb")
+                >>> model1.import_results_from_files(["model1_lc2.odb", "mode1l_lc3.odb"])
+
+                >>> model2 = load_model("model2.dat", "InputFileNastran")
+                >>> model2.import_results_from_files(["model2_lc1.op2", "model2_lc2.op2"])
             """
         if isinstance(results_files, str):
             results_files = [results_files]
 
         for result_file in results_files:
             self.__vzmodel.ImportResults(str(result_file))
             self._import_load_cases()
@@ -926,14 +941,22 @@
                               domain: list[N2PElement, N2PConnector, ...] = None) -> list[N2PElement, N2PConnector, ...]:
         """ Method of N2PModelContent that returns a list of N2PElement and N2PConnector that are adjacent to selected
         ones. If a domain is selected, the adjacent elements only will be searched in that domain.
 
         Args:
             cells: list[N2PElement, N2PConnector, ...]
             domain: list[N2PElement, N2PConnector, ...] -> Optional. Set the domain where to look for the adjacent elements
+
+        Returns:
+            list[N2PElement, N2PConnector, ...]
+
+        Example:
+            >>> model = load_model("model.odb")
+            >>> domain_S4 = [e for e in model.get_elements() if e.TypeElement == "S4"]
+            >>> elems_adj = model.get_elements_adjacent(model.get_elements(17500), domain=domain_S4)
             """
         if not isinstance(cells, list):
             cells = [cells]
         inernal_ids = array.array("q", [cell.InternalID for cell in cells])
         if not domain:
             adjacent_ids = N2AdjacencyFunctions.GetAdjacent(self.__vzmodel.UMesh, inernal_ids)
         else:
@@ -958,14 +981,22 @@
                               domain: list[N2PElement, N2PConnector, ...] = None) -> list[N2PElement, N2PConnector, ...]:
         """ Method of N2PModelContent that returns a list of N2PElement and N2PConnector that are attached to selected ones. If a domain
         is selected, the attached elements only will be searched in that domain.
 
         Args:
             cells: list[N2PElement, N2PConnector, ...]
             domain: list[N2PElement, N2PConnector, ...] -> Optional. Set the domain where to look for the adjacent elements
+
+        Returns:
+            list[N2PElement, N2PConnector, ...]
+
+        Example:
+            >>> model = load_model("model.h3d")
+            >>> domain_elems = model.get_elements()
+            >>> elems_att = model.get_elements_attached(model.get_elements(17500), domain=domain_elems)
             """
         if not isinstance(cells, list):
             cells = [cells]
         inernal_ids = array.array("q", [cell.InternalID for cell in cells])
         if not domain:
             adjacent_ids = N2AdjacencyFunctions.GetAttached(self.__vzmodel.UMesh, inernal_ids)
         else:
@@ -993,17 +1024,29 @@
         """ Method of N2PModelContent that returns a list of N2PElement and N2PConnector that are in the same face as
         the selected ones. If a domain is selected, the face elements only will be searched in that domain. To be
         considered in the same face, the adjacent element must share an arist and the angle between the elements must be
         lower than the tolerance angle.
 
         Args:
             cells: list[N2PElement, N2PConnector, ...]
+
             tolerance_angle: float -> Optional (30º by default). Max angle[º] between two elements to be considered in the same face
+
             one_element_adjacent: bool -> Optional (True by default). If true, two elements are connected to arist of a selected element they will no be consisidered.
+
             domain: list[N2PElement, N2PConnector, ...] -> Optional. Set the domain where to look for the adjacent elements
+
+        Returns:
+            list[N2PElement, N2PConnector, ...]
+
+        Example:
+            >>> model = load_model("model.op2")
+            >>> elems1 = model.get_elements_by_face(model.get_elements(17500))
+            >>> domain_cquad = [e for e in model.get_elements() if e.TypeElement == "CQUAD4"]
+            >>> elems2 = model.get_elements_by_face(model.get_elements([17500, 17501]), 25, domain=domain_cquad)
             """
         if not isinstance(cells, list):
             cells = [cells]
         inernal_ids = array.array("q", [cell.InternalID for cell in cells])
         if not domain:
             adjacent_ids = N2AdjacencyFunctions.GetByFace(self.__vzmodel,
                                                           inernal_ids,
@@ -1032,21 +1075,24 @@
 
     ####################################################################################################################
     #########################################     get_free_edges      ##################################################
     ####################################################################################################################
     def get_free_edges(self,
                        domain: list[N2PElement, N2PConnector, ...] = None) -> list[tuple[N2PElement, N2PNode, N2PNode], ...]:
 
-        """ Method of N2PModelContent that returns a list of tuples of N2PElement and two N2PNode of that element. 
+        """ Method of N2PModelContent that returns a list of tuples of a N2PElement and two N2PNode of that element.
         The two nodes define the edge of the element that is contained in the free edge of the mesh If a domain is selected, 
         the tuple will only be searched in that domain. Notice that connectors, although they may be given in the domain,
         they are never included in the free edges.
 
         Args:
-            domain: list[N2PElement, N2PConnector, ...] -> Optional. Set the domain where to look for the adjacent elements
+            domain: list[N2PElement, N2PConnector, ...] -> Optional. Set the domain where to look for the free edges
+
+        Returns:
+            list[tuple[N2PElement, N2PNode, N2PNode], ...]
             """
 
         csharp_bool_array = System.Array.CreateInstance(System.Boolean,
                                                         len(self.__element_dict)+len(self.__connector_dict))
 
         if not domain:
             for i in range(len(self.__element_dict)+len(self.__connector_dict)):
@@ -1072,20 +1118,29 @@
         In order to define the combination a string with the load case and frame and the arithmetical commands as strings
         must be passed as arguments. The name of the new derived loadcase must be set, but the id not. The id will be a
         negative integer. The loadcases|frames must have this structure: <LCXX:FRYY>. Examples of formulas:
             - formula = "<LC1:FR1>+2*<LC2:FR1>+0.5*<LC5:FR3>"
             - formula = "0.5*<LC1:FR2>"
             - formula = "5*<LC2:FR3>-2*<LC3:FR3>"
 
+        Note:
+            The derived load cases will have only one frame/increment with id 0. So it is used in a formula the string
+            will be "<LC-1:FR0>".
+
         Args:
             name: str -> String with the name of the load case.
             formula: str -> String that must have the loadcase|frame is intended to use and the arithmetical opreations.
 
         Returns:
             N2PLoadCase -> Derived load case
+
+        Examples:
+            >>> dev_lc1 = new_derived_loadcase("dev_lc1", "<LC1:FR1>+2*<LC2:FR1>+0.5*<LC5:FR3>")
+            >>> dev_lc2 = new_derived_loadcase("dev_lc2", "0.5*<LC1:FR2>")
+            >>> dev_lc3 = new_derived_loadcase("dev_lc3", "5*<LC-1:FR0>-2*<LC3:FR3>")
         """
         # Comprobamos que el nombre no se repite:
         i = 0
         while name in [lc.Name for lc in self.LoadCases]:
             i += 1
             name += f"-{i}"
 
@@ -1143,14 +1198,18 @@
 
                 - 'ByContour': The data will be the actual value (XX stress for example)
                 - 'ByLoadCaseID': The data will be the id of the original load case that is critical (LC 6363 for example)
                 - 'ByIncrement': The data will be the id of the increment that is critical
 
         Returns:
             N2PLoadCase
+
+        Examples:
+            >>> env_lc1 = new_envelope_loadcase("env_lc1", formula="<LC1:FR1>,<LC2:FR1>")
+            >>> env_lc2 = new_envelope_loadcase("env_lc2", formula="<LC1:FR1>,<LC2:FR8>,<LC-3:FR0>", criteria="Min", envelgroup="ByLoadCaseID")
         """
         # Comprobamos que el nombre no se repite:
         i = 0
         while name in [lc.Name for lc in self.LoadCases]:
             i += 1
             name += f"-{i}"
 
@@ -1278,19 +1337,18 @@
 
             v2: tuple -> Optional. Directions vectors that generate the coordinate system axis:
                 x=v1,
                 z=v1^v2,
                 y=z^x.
 
         Examples:
-            report1 = model.new_report("<LC1:FR1>,<LC2:FR1>", False, "DISPLACEMNETS", "<X:NONE#>,<Y:NONE#>", False,
-            list_n2pnodes, "LC")
+            >>> report1 = model.new_report("<LC1:FR1>,<LC2:FR1>", False, "DISPLACEMNETS", "<X:NONE#>,<Y:NONE#>", False, list_n2pnodes, "LC")
 
-            report2 = model.new_report("<LC1:FR1>,<LC1:FR2>,<LC4:FR6>", False, "STRESSES", "<VON_MISES:Z1#Z2#>,<MAX_SHEAR:Z1#Z2#>",
-            False, list_n2pelements, "IDS", aveSections=-4, coordsys=-1)
+            >>> report2 = model.new_report("<LC1:FR1>,<LC1:FR2>,<LC4:FR6>", False, "STRESSES", "<VON_MISES:Z1#Z2#>,<MAX_SHEAR:Z1#Z2#>", \
+                                           False, list_n2pelements, "IDS", aveSections=-4, coordsys=-1)
         """
         # Here it is checkd if the components, the loadcases and the result exist and the formula is right
         try:
             lcs = [int(lc.split(":")[0][3:]) for lc in lc_incr.split(",")]
             components = [c.split(":")[0][1:] for c in componentssections.split(",")]
             for lc in lcs:
                 all_comps = chain(self.get_load_case(lc).get_result(result).Components.keys(),
@@ -1315,16 +1373,16 @@
                                variation=100, realPolar=0, coordsys: int = -1000, v1: tuple = (1,0,0),
                                v2: tuple = (0,1,0)) -> dict[tuple: "ndarray"]:
         """Method to ask for results of a component in several loadcases and increments. It uses parallel subprocesses
         to speed up the calculus. Returns a dictionary where the keys are tuples with the IDs of LoadCase and Increment
         and the values are numpy arrays.
 
         Examples:
-            vonmises = .get_result_by_LCs_Incr([(1,2),(2,2)], "STRESSES", "VON_MISES")
-            XX = .get_result_by_LCs_Incr([(loadcase1, increment2), (loadcase2, increment2), "STRAINS", "XX"])
+            >>> vonmises = N2PModelContent.get_result_by_LCs_Incr([(1,2),(2,2)], "STRESSES", "VON_MISES")
+            >>> XX = N2PModelContent.get_result_by_LCs_Incr([(loadcase1, increment2), (loadcase2, increment2), "STRAINS", "XX"])
 
         Args:
 
             list_lc_incr: list[tuple] -> list with the tuples of the loadcase|increment asked for the component
 
             result: str -> String with the result
 
@@ -1426,23 +1484,37 @@
 # Metodo para cargar un objeto N2PModelContent desde un archivo de resultados o desde un archivo de texto --------------
 def load_model(path: str, parallelprocessing: bool = False, file_type: str = None) -> N2PModelContent:
     """ Read an output result file in binary format from Nastran, Abaqus, Optistruct or Ansys and transform it into a
     N2PModelContent Object. It also can read models from input files in Nastran format.
 
         Supports .op2, .xdb, .odb, .h5, .h3d and .rst file extensions read from a local filesystem or URL.
 
-        Supports Nastran input files. (Typically .bdf extension)
+        Supports Nastran Input Files. (Typically .bdf extension)
 
         Args:
             path: str
             parallelprocessing: bool -> Optional. If true, the low libraries open the result files in several processes. It is slightly faster.
             file_type: str -> Optional. It specifies if it is Nastran input file ("InputFileNastran") or binary result file ("Binary").
 
         Returns:
             model: N2PModelContent
+
+        Examples:
+            >>> model1 = load_model(r"C:\MODELS\FEM\model1.dat")
+
+            >>> # file_type is not needed. It only helps the program and saves a checking
+            >>> model2 = load_model(r"C:\MODELS\FEM\model2.dat", file_type="InputFileNastran")
+
+            >>> # parallelprocessing is only aviable for Binary files. It is helpful in some big files.
+            >>> model3 = load_model(r"C:\MODELS\RESULTS\model1.op2", parallelprocessing=True)
+
+            >>> model4 = load_model(r"C:\MODELS\RESULTS\model2.xdb", file_type="Binary")
+            >>> model5 = load_model(r"C:\MODELS\RESULTS\model5.h3d")
+            >>> model6 = load_model(r"C:\MODELS\RESULTS\model6.odb", True, "Binary")
+
         """
     if not os.path.exists(path):
         N2PLog.Critical.C108(path)
         return "ERROR"
         # sys.exit()
 
     if path.split(".")[-1] in BINARY_EXTENSIONS and file_type == "InputFileNastran":
```

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/Reference_Finder/__Reference_Finder.py` & `naxtopy-2.0.1/src/NaxToPy/Core/Reference_Finder/__Reference_Finder.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,20 +164,21 @@
 
             # Si alguna es de esta version hay que ver si el assembly, que cambia con cada step es compatible.
             # Previamente se verifica que el archivo existe:
             if os.path.exists(lib_path):
                 versionInfo = FileVersionInfo.GetVersionInfo(lib_path)
                 assemblyVersion = versionInfo.FileVersion
 
-                # Si la version es compatible se devuelve la ruta y un boleano indicando si es compatible
-                if assemblyVersion in VIZZER_COMPATIBILITY:
-                    return lib_path, True
+                N2PLog.Debug.D200(assemblyVersion)
+
+                # Se va a suponer que la todos los steps de una version NaxTo son compatibles con todos los steps de
+                # una version de NaxToPy: NaxTo 2024.1.X <---> 2.0.Y
+                return lib_path, True
 
     N2PLog.Warning.W104(NAXTO_VERSION)
-    # Aunque la version este bien, el assembly no. Puede que de un step a otro no haya compatibilidad.
     backup = ""
 
     # Comprobamos si hay alguna version que contenga una dll compatible
     for lib in vizzer_libs:
         lib_path = lib + "\\" + VIZZER_CLASSES_DLL
         if not os.path.exists(lib_path):
             continue
```

### Comparing `naxtopy-2.0.0/src/NaxToPy/Core/_AuxFunc/_NetToPython.py` & `naxtopy-2.0.1/src/NaxToPy/Core/_AuxFunc/_NetToPython.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Modules/Fasteners/N2PUpdateFastener.py` & `naxtopy-2.0.1/src/NaxToPy/Modules/Fasteners/N2PUpdateFastener.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Modules/N2PEnvelope/N2PEnvelope.py` & `naxtopy-2.0.1/src/NaxToPy/Modules/N2PEnvelope/N2PEnvelope.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/Modules/N2PtoEXE/N2PtoEXE.py` & `naxtopy-2.0.1/src/NaxToPy/Modules/N2PtoEXE/N2PtoEXE.py`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/NaxToPy.ico` & `naxtopy-2.0.1/src/NaxToPy/NaxToPy.ico`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy/user_functions.txt` & `naxtopy-2.0.1/src/NaxToPy/user_functions.txt`

 * *Files identical despite different names*

### Comparing `naxtopy-2.0.0/src/NaxToPy.egg-info/PKG-INFO` & `naxtopy-2.0.1/src/NaxToPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NaxToPy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Package for postprocessing FEM results in Python
 Home-page: https://www.idaerosolutions.com/Home/NaxToPy
 Download-URL: https://apps.microsoft.com/detail/XP9MMH0KDKGRJN?hl=en-US&gl=US
 Author-email: Idaero Solutions <manuel.sanchez@idaerosolutions.com>
 License: Copyright (c) 2024 Idaero Solutions
         
         This freeware license agreement (“agreement”) is a legally binding contract
@@ -131,35 +131,38 @@
 
 ![](https://idaerosolutions.com/images/icons/Logo_NaxToPy_Black.svg "NaxToPy")
 
 # NaxToPy
 
 **NaxToPy** is the [**NaxTo**](https://apps.microsoft.com/detail/XP9MMH0KDKGRJN?hl=en-US&gl=US)
 library designed for Python, which allows reading and manipulating FEM
-analysis results files from the most common tools: Nastran (op2, xdb, h5), Abaqus (odb), Optistruct
-(h3d, op2) and Ansys (rst); and stores them in a user-friendly Python structure. Additionally, it
-can read input files from Nastran (bdf, fem) and change it contents.
+analysis results files from the most common tools: Nastran (.op2, .xdb, .h5), Abaqus (odb), Optistruct
+(.h3d, .op2) and Ansys (.rst); and stores them in a user-friendly Python structure. Additionally, it
+can read input files from Nastran (.bdf, .fem) and change their contents.
 
 It could be easily combined with other Python packages as Matplotlib or Pandas. This provides access
 to the full coding power of Python to interpret and process the results, without the need to install
 any additional software other than having NaxTo already installed (see the _Download_ and _Homepage_
 links on the left).
 
 **NaxToPy** is a powerful tool for FEM analysis post-processing!
 
 **CAUTION:** To use NaxToPy, [**NaxTo**](https://apps.microsoft.com/detail/XP9MMH0KDKGRJN?hl=en-US&gl=US) must be installed.
-This version is compatible with **NaxTo 2024.1**. It may be compatible with all the steps of this version (2024.1.0, 2024.1.1, 2024.1.2, etc.).
+This version is compatible with **NaxTo 2024.1**. It is compatible with all the steps of this version (2024.1.0, 2024.1.1, 2024.1.2, etc.).
 Check in _Programs and Features_ the NaxTo version that is installed. 
 
 ## Installation
 
+If python is installed and `pip` is added to the PATH:
 
-If python is callable from the command line:
+`pip install NaxToPy`
+
+An alternative, if Python is callable from the command line:
 
-`py -m pip install NaxToPy`
+`python -m pip install NaxToPy`
 
 For **Visual Studio** users:
 - Open "Python Environments" window
 - Change the "general information" label to "Packages(Pypi)"
 - Write the name of the package and press enter:
 
 - `NaxToPy` + enter
@@ -175,15 +178,15 @@
       import sys
       sys.path.append("...\directory")
       import NaxToPy as n2p
 ## Updating NaxToPy
 
 If python is callable from the command line:
 
-`py -m pip install -U NaxToPy`
+`python -m pip install -U NaxToPy`
 
 For Visual Studio users:
 - Open "Python Environments" window
 - Change the "general information" label to "Packages(Pypi)"
 - Write the following command on the search bar and press enter:
 
   `-U NaxToPy` + enter
@@ -256,14 +259,20 @@
 the LoadCases that are critical or the Increment that is critical instead of the value.
 
 ### v.2.0.0
 1. Changes made to align the library with updates in lower-level dependencies.
 2. New internal methods to look for the compatibility with low-level dependencies.
 3. The name of the .log is now NaxToPy_Year-Month-Day.log.
 
+### v.2.0.1
+1. The compatibility is extended to all NaxTo steps of the same version.
+2. The property N2PLoadCase.ActiveIncrement is subtitued by N2PLoadCase.ActiveN2PIncrement.
+It uses an object instaed of an int.
+3. Update of the examples of some docstrings.
+
 # Documentation
 
 **NaxToPy** is a package developed by Idaero Solutions© as a part of the **NaxTo** software.
 
 NaxToPy only use three dependeces:
 - NumPy: https://numpy.org/
 - PythonNET: https://pythonnet.github.io/
@@ -335,15 +344,15 @@
 # Load the list of load cases as N2PLoadCase object
 loadcaseslist = model.LoadCases
 
 # Look for the Load Case with the name pressure
 pressure_lc = model.get_load_case("pressure")
 
 # Change the active increment (by default is the last one):
-pressure_lc.ActiveIncrement = 10
+pressure_lc.ActiveN2PIncrement = pressure_lc.get_increment(10)
 
 # Look for all results
 all_results = pressure_lc.Results
 
 # Look for the Result with the name DISPLACEMENT
 displacement = pressure_lc.get_result("DISPLACEMENT")
```

### Comparing `naxtopy-2.0.0/src/NaxToPy.egg-info/SOURCES.txt` & `naxtopy-2.0.1/src/NaxToPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

