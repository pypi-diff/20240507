# Comparing `tmp/tdrpa.tdworker-1.1.0-py3-none-any.whl.zip` & `tmp/tdrpa.tdworker-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 402064 bytes, number of entries: 10
+Zip file size: 402094 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat  1126912 b- defN 24-May-06 14:16 tdrpa/tdworker.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    15621 b- defN 24-May-06 14:11 tdrpa/tdworker/WinElement.pyi
 -rw-rw-rw-  2.0 fat     4815 b- defN 24-May-06 06:22 tdrpa/tdworker/WinKeyboard.pyi
 -rw-rw-rw-  2.0 fat     6966 b- defN 24-May-06 06:18 tdrpa/tdworker/WinMouse.pyi
 -rw-rw-rw-  2.0 fat     3672 b- defN 24-May-06 06:25 tdrpa/tdworker/WinWindow.pyi
 -rw-rw-rw-  2.0 fat       60 b- defN 24-May-06 07:35 tdrpa/tdworker/__init__.pyi
--rw-rw-rw-  2.0 fat      641 b- defN 24-May-07 10:45 tdrpa.tdworker-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 10:45 tdrpa.tdworker-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-07 10:45 tdrpa.tdworker-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      842 b- defN 24-May-07 10:45 tdrpa.tdworker-1.1.0.dist-info/RECORD
-10 files, 1159627 bytes uncompressed, 400622 bytes compressed:  65.5%
+-rw-rw-rw-  2.0 fat      661 b- defN 24-May-07 10:59 tdrpa.tdworker-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 10:59 tdrpa.tdworker-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-07 10:59 tdrpa.tdworker-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      842 b- defN 24-May-07 10:59 tdrpa.tdworker-1.1.1.dist-info/RECORD
+10 files, 1159647 bytes uncompressed, 400652 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: tdrpa/tdworker/WinWindow.pyi
 Comment: 
 
 Filename: tdrpa/tdworker/__init__.pyi
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.0.dist-info/METADATA
+Filename: tdrpa.tdworker-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.0.dist-info/WHEEL
+Filename: tdrpa.tdworker-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.0.dist-info/top_level.txt
+Filename: tdrpa.tdworker-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.0.dist-info/RECORD
+Filename: tdrpa.tdworker-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tdrpa.tdworker-1.1.0.dist-info/METADATA` & `tdrpa.tdworker-1.1.1.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: tdrpa.tdworker
-Version: 1.1.0
-Summary: RPA SDK for software developers. Supports Python3.7+, Windows x64
+Version: 1.1.1
+Summary: tdworker for tdrpa developers. supports python3.8+, windows x64
 Home-page: https://tdrpa.thingswell.cn
-Author: tdrpa
-Author-email: armstrong.wang@gmail.com
+Author: vx:RPA_CREATOR
+Author-email: oldplayerliu@gmail.com
 License: Apache 2.0
-Keywords: RPA,tdRPA,uiautomation,uia
+Keywords: RPA,tdRPA,tdworker,rpaworker,worker,uiautomation,uia,creator,windows,python,bot,robot,aigc,ai
 Platform: Windows Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Dist: keyboard
-Requires-Dist: psutil
-Requires-Dist: pywin32
-Requires-Dist: Requests
-Requires-Dist: tzlocal
-Requires-Dist: uiautomation
-
-RPA SDK for software developers. Supports Python3.7+, Windows x64
-
+Requires-Dist: tdrpa.tdcore
+Requires-Dist: pyperclip
+Requires-Dist: WMI
+Requires-Dist: pycryptodome
 
+tdworker for tdrpa developers. supports python3.8+, windows x64
```

## Comparing `tdrpa.tdworker-1.1.0.dist-info/RECORD` & `tdrpa.tdworker-1.1.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 tdrpa/tdworker.cp38-win_amd64.pyd,sha256=iQus662RkW8GFRSJUba0cqzUU4ctEig-HXYp9J6FhS4,1126912
 tdrpa/tdworker/WinElement.pyi,sha256=Y6OBYXLr3w1xmRnnVGvbWtlX46v5d87NiOBkq-01O4s,15621
 tdrpa/tdworker/WinKeyboard.pyi,sha256=bRdaR6rM4FNzbIATUXRmt36fm3BhFarzpKruAJHklME,4815
 tdrpa/tdworker/WinMouse.pyi,sha256=H_59kcbqkJwoSfGQxte2Uo_f7J7n1ys2p9MKeZ1tnhU,6966
 tdrpa/tdworker/WinWindow.pyi,sha256=8X9FLtPKbw2rK2Wgc9z2ZmmWUAbogbNK6lmYhQ84dHU,3672
 tdrpa/tdworker/__init__.pyi,sha256=p5gNrSuSvmBtCSEM133tD7XSlW_2LyUB4svpQTlndv8,60
-tdrpa.tdworker-1.1.0.dist-info/METADATA,sha256=PjDzaMDgaceI44oSaGr2WuB5pJYaIHpAW75RRJIgaBI,641
-tdrpa.tdworker-1.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-tdrpa.tdworker-1.1.0.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
-tdrpa.tdworker-1.1.0.dist-info/RECORD,,
+tdrpa.tdworker-1.1.1.dist-info/METADATA,sha256=Iw2zv49ZCoWOWI6p1NuVrxQgbf7c-jziQetCC94xSE8,661
+tdrpa.tdworker-1.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tdrpa.tdworker-1.1.1.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
+tdrpa.tdworker-1.1.1.dist-info/RECORD,,
```

