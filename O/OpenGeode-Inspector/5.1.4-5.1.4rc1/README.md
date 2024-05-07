# Comparing `tmp/OpenGeode_Inspector-5.1.4-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_Inspector-5.1.4rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 352731 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      175 b- defN 24-May-07 00:22 opengeode_inspector/__init__.py
--rw-rw-rw-  2.0 fat     1243 b- defN 24-May-07 00:22 opengeode_inspector/inspector.py
--rw-rw-rw-  2.0 fat   512000 b- defN 24-May-07 00:23 opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
--rw-rw-rw-  2.0 fat   688128 b- defN 24-May-07 00:23 opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     5283 b- defN 24-May-07 00:23 OpenGeode_Inspector-5.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-07 00:23 OpenGeode_Inspector-5.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 24-May-07 00:23 OpenGeode_Inspector-5.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      773 b- defN 24-May-07 00:23 OpenGeode_Inspector-5.1.4.dist-info/RECORD
-8 files, 1207722 bytes uncompressed, 351359 bytes compressed:  70.9%
+Zip file size: 352759 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      175 b- defN 24-May-06 14:15 opengeode_inspector/__init__.py
+-rw-rw-rw-  2.0 fat     1243 b- defN 24-May-06 14:15 opengeode_inspector/inspector.py
+-rw-rw-rw-  2.0 fat   512000 b- defN 24-May-06 14:16 opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
+-rw-rw-rw-  2.0 fat   688128 b- defN 24-May-06 14:16 opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     5286 b- defN 24-May-06 14:16 OpenGeode_Inspector-5.1.4rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-06 14:16 OpenGeode_Inspector-5.1.4rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 24-May-06 14:16 OpenGeode_Inspector-5.1.4rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      785 b- defN 24-May-06 14:16 OpenGeode_Inspector-5.1.4rc1.dist-info/RECORD
+8 files, 1207737 bytes uncompressed, 351363 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
 Comment: 
 
 Filename: opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
 Comment: 
 
-Filename: OpenGeode_Inspector-5.1.4.dist-info/METADATA
+Filename: OpenGeode_Inspector-5.1.4rc1.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_Inspector-5.1.4.dist-info/WHEEL
+Filename: OpenGeode_Inspector-5.1.4rc1.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_Inspector-5.1.4.dist-info/top_level.txt
+Filename: OpenGeode_Inspector-5.1.4rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_Inspector-5.1.4.dist-info/RECORD
+Filename: OpenGeode_Inspector-5.1.4rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180056e48
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue May  7 00:22:40 2024
+Time/Date		Mon May  6 14:15:51 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000059e00
 SizeOfInitializedData	0000000000023400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000056e48
@@ -119268,18 +119268,19 @@
    18005e8ca:	(bad)
    18005e8cb:	(bad)
    18005e8cc:	(bad)
    18005e8cd:	(bad)
    18005e8ce:	(bad)
    18005e8cf:	incl   (%rax)
    18005e8d1:	add    %al,(%rax)
-   18005e8d3:	add    %dl,0x74(%rax)
-   18005e8d6:	cmp    %esp,0x0(%rsi)
-   18005e8d9:	add    %al,(%rax)
-   18005e8db:	add    %cl,0x14000000(%rip)        # 0x19405e8e1
+   18005e8d3:	add    %dl,(%rdi)
+   18005e8d5:	out    %al,$0x38
+   18005e8d7:	data16 add %al,(%rax)
+   18005e8da:	add    %al,(%rax)
+   18005e8dc:	or     $0x14000000,%eax
    18005e8e1:	add    (%rax),%eax
    18005e8e3:	add    %bh,(%rcx,%rax,1)
    18005e8e6:	(bad)
    18005e8e7:	add    %bh,(%rbx,%rsi,8)
    18005e8ea:	add    $0x0,%eax
    18005e8ef:	add    %bh,(%rax)
    18005e8f1:	add    %eax,(%rax)
```

## Comparing `OpenGeode_Inspector-5.1.4.dist-info/METADATA` & `OpenGeode_Inspector-5.1.4rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeode-Inspector
-Version: 5.1.4
+Version: 5.1.4rc1
 Summary: Open source framework for inspecting the validity of geometric models
 Home-page: https://github.com/Geode-solutions/OpenGeode-Inspector
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OpenGeode-Inspector Version: 5.1.4 Summary: Open
+Metadata-Version: 2.1 Name: OpenGeode-Inspector Version: 5.1.4rc1 Summary: Open
 source framework for inspecting the validity of geometric models Home-page:
 https://github.com/Geode-solutions/OpenGeode-Inspector Author: Geode-solutions
 Author-email: contact@geode-solutions.com License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown Requires-Dist: opengeode-core
 ==14.*,>=14.19.3
               ************ OOppeennGGeeooddee--IInnssppeeccttoorrbbyy GGeeooddee--ssoolluuttiioonnss ************
           ******** OOppeennGGeeooddee mmoodduullee ffoorr iinnssppeeccttiinngg mmeesshheess aanndd mmooddeellss ********
```

## Comparing `OpenGeode_Inspector-5.1.4.dist-info/RECORD` & `OpenGeode_Inspector-5.1.4rc1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 opengeode_inspector/__init__.py,sha256=ESjaSG_8bKq1Pgvac3wHQV3kdFbXPgCvl8ROoFwkGbc,175
 opengeode_inspector/inspector.py,sha256=sgoiFAE4sNHbqO7QTK1rVg9T-CCwISvC5sg8m9Vb5nY,1243
-opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll,sha256=zkZ0PwfpKj0LMNbumFzTGp4X4UxSqemGxeho9m0tcNo,512000
-opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd,sha256=6DeW6ZcTd0DndafSPxjoB0LB-vwqGgadAPXIbnpmmCs,688128
-OpenGeode_Inspector-5.1.4.dist-info/METADATA,sha256=ShRT1s3pzw4U2MHrVVlOzpBn8yqy9U0qVJLwmJdGKss,5283
-OpenGeode_Inspector-5.1.4.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
-OpenGeode_Inspector-5.1.4.dist-info/top_level.txt,sha256=HB6mBr33nBKSATXRcJ4Yof7xiFcQAnhw3pFzWTv8zso,20
-OpenGeode_Inspector-5.1.4.dist-info/RECORD,,
+opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll,sha256=B84JvlJw2EQWUgIwITB14Ovg3R9PPHOodoBdi_DoVC4,512000
+opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd,sha256=s-P9eEOkvwwG8Hp26P1HN_49c8bT-J93nehtWkM0OEQ,688128
+OpenGeode_Inspector-5.1.4rc1.dist-info/METADATA,sha256=8N8I53zlm1PXKT12tuap1FyAXyT3x4TcGiAIBGA-ZRw,5286
+OpenGeode_Inspector-5.1.4rc1.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
+OpenGeode_Inspector-5.1.4rc1.dist-info/top_level.txt,sha256=HB6mBr33nBKSATXRcJ4Yof7xiFcQAnhw3pFzWTv8zso,20
+OpenGeode_Inspector-5.1.4rc1.dist-info/RECORD,,
```

