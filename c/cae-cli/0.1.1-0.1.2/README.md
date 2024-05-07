# Comparing `tmp/cae_cli-0.1.1.tar.gz` & `tmp/cae_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.1.1.tar", last modified: Sun May  5 20:27:05 2024, max compression
+gzip compressed data, was "cae_cli-0.1.2.tar", last modified: Tue May  7 01:58:57 2024, max compression
```

## Comparing `cae_cli-0.1.1.tar` & `cae_cli-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 20:27:05.168235 cae_cli-0.1.1/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      408 2024-05-05 20:27:05.167235 cae_cli-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 20:27:05.138651 cae_cli-0.1.1/cae/
--rw-rw-rw-   0        0        0     7618 2024-05-05 04:35:29.000000 cae_cli-0.1.1/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.1.1/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.1.1/cae/__init__.py
--rw-rw-rw-   0        0        0     7302 2024-05-05 04:35:29.000000 cae_cli-0.1.1/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-05 20:27:05.153300 cae_cli-0.1.1/cae/templates/
--rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.1.1/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.1.1/cae/templates/dependency_wrapper.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.1.1/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.1.1/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1061 2024-05-04 02:53:55.000000 cae_cli-0.1.1/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1133 2024-05-04 03:01:34.000000 cae_cli-0.1.1/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1288 2024-05-04 03:02:00.000000 cae_cli-0.1.1/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.1.1/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.1.1/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.1.1/cae/templates/use_case_factory.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.1.1/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.1.1/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      397 2024-05-04 04:16:15.000000 cae_cli-0.1.1/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.1.1/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-05 20:27:05.166236 cae_cli-0.1.1/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      408 2024-05-05 20:27:05.000000 cae_cli-0.1.1/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      705 2024-05-05 20:27:05.000000 cae_cli-0.1.1/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 20:27:05.000000 cae_cli-0.1.1/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-05 20:27:05.000000 cae_cli-0.1.1/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-05 20:27:05.000000 cae_cli-0.1.1/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 20:27:05.168235 cae_cli-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      603 2024-05-05 20:27:02.000000 cae_cli-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:58:57.689340 cae_cli-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      415 2024-05-07 01:58:57.687343 cae_cli-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 01:58:57.579767 cae_cli-0.1.2/cae/
+-rw-rw-rw-   0        0        0     7618 2024-05-05 04:35:29.000000 cae_cli-0.1.2/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.1.2/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.1.2/cae/__init__.py
+-rw-rw-rw-   0        0        0     8062 2024-05-07 01:51:42.000000 cae_cli-0.1.2/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-07 01:58:57.663298 cae_cli-0.1.2/cae/templates/
+-rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.1.2/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.1.2/cae/templates/dependency_wrapper.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.1.2/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.1.2/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1717 2024-05-07 01:56:38.000000 cae_cli-0.1.2/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1789 2024-05-07 01:56:38.000000 cae_cli-0.1.2/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1944 2024-05-07 01:56:38.000000 cae_cli-0.1.2/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.1.2/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.1.2/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.1.2/cae/templates/use_case_factory.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.1.2/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.1.2/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      397 2024-05-04 04:16:15.000000 cae_cli-0.1.2/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.1.2/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 01:58:57.686342 cae_cli-0.1.2/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-05-07 01:58:57.000000 cae_cli-0.1.2/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2024-05-07 01:58:57.000000 cae_cli-0.1.2/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 01:58:57.000000 cae_cli-0.1.2/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-07 01:58:57.000000 cae_cli-0.1.2/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-07 01:58:57.000000 cae_cli-0.1.2/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 01:58:57.689340 cae_cli-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      610 2024-05-07 01:58:54.000000 cae_cli-0.1.2/setup.py
```

### Comparing `cae_cli-0.1.1/LICENSE` & `cae_cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.1/README.md` & `cae_cli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.1/cae/ArchFlowJavaWeb.py` & `cae_cli-0.1.2/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.1/cae/db.json` & `cae_cli-0.1.2/cae/db.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9047619047619048%*

 * *Differences: {"'functions'": "{'clear': OrderedDict([('steps', [OrderedDict([('clear_layer', ['core'])]), "*

 * *                "OrderedDict([('clear_layer', ['adapters'])]), OrderedDict([('clear_layer', "*

 * *                "['assemblers'])])])]), 'install': OrderedDict([('steps', "*

 * *                "[OrderedDict([('clear_layer', ['core'])]), OrderedDict([('clear_layer', "*

 * *                "['adapters'])]), OrderedDict([('clear_layer', ['assemblers'])])])]), "*

 * *                "'clear_layer': OrderedDict([('steps', [OrderedDict( […]*

```diff
@@ -20,21 +20,55 @@
                     "clear_all": "None"
                 },
                 {
                     "install_all": "None"
                 }
             ]
         },
+        "clear": {
+            "steps": [
+                {
+                    "clear_layer": [
+                        "core"
+                    ]
+                },
+                {
+                    "clear_layer": [
+                        "adapters"
+                    ]
+                },
+                {
+                    "clear_layer": [
+                        "assemblers"
+                    ]
+                }
+            ]
+        },
         "clear_all": {
             "steps": [
                 {
                     "clear_all": "None"
                 }
             ]
         },
+        "clear_layer": {
+            "steps": [
+                {
+                    "walk_to_use_case_layer": [
+                        "args[0]"
+                    ]
+                },
+                {
+                    "clear_all": "None"
+                },
+                {
+                    "return_root_path": "None"
+                }
+            ]
+        },
         "core_basic_dir": {
             "steps": [
                 {
                     "create_folder": [
                         "factories"
                     ]
                 },
@@ -137,21 +171,55 @@
                         [
                             "args[1]"
                         ]
                     ]
                 }
             ]
         },
+        "install": {
+            "steps": [
+                {
+                    "clear_layer": [
+                        "core"
+                    ]
+                },
+                {
+                    "clear_layer": [
+                        "adapters"
+                    ]
+                },
+                {
+                    "clear_layer": [
+                        "assemblers"
+                    ]
+                }
+            ]
+        },
         "install_all": {
             "steps": [
                 {
                     "install_all_project": "None"
                 }
             ]
         },
+        "install_layer": {
+            "steps": [
+                {
+                    "walk_to_use_case_layer": [
+                        "args[0]"
+                    ]
+                },
+                {
+                    "install_all_project": "None"
+                },
+                {
+                    "return_root_path": "None"
+                }
+            ]
+        },
         "new_cuc": {
             "steps": [
                 {
                     "walk_to_use_case_layer": [
                         "core"
                     ]
                 },
```

### Comparing `cae_cli-0.1.1/cae/templates/assembler.txt` & `cae_cli-0.1.2/cae/templates/assembler.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.1/cae/templates/implementation_cuc.txt` & `cae_cli-0.1.2/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.1/cae/templates/implementation_suc.txt` & `cae_cli-0.1.2/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.1/cae/templates/pom-adapters.txt` & `cae_cli-0.1.2/cae/templates/pom-assemblers.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,63 +5,108 @@
 00000040: 3031 2f58 4d4c 5363 6865 6d61 2d69 6e73  01/XMLSchema-ins
 00000050: 7461 6e63 6522 2078 7369 3a73 6368 656d  tance" xsi:schem
 00000060: 614c 6f63 6174 696f 6e3d 2268 7474 703a  aLocation="http:
 00000070: 2f2f 6d61 7665 6e2e 6170 6163 6865 2e6f  //maven.apache.o
 00000080: 7267 2f50 4f4d 2f34 2e30 2e30 2068 7474  rg/POM/4.0.0 htt
 00000090: 703a 2f2f 6d61 7665 6e2e 6170 6163 6865  p://maven.apache
 000000a0: 2e6f 7267 2f6d 6176 656e 2d76 345f 305f  .org/maven-v4_0_
-000000b0: 302e 7873 6422 3e0d 0a0d 0a20 2020 203c  0.xsd">....    <
-000000c0: 6d6f 6465 6c56 6572 7369 6f6e 3e34 2e30  modelVersion>4.0
-000000d0: 2e30 3c2f 6d6f 6465 6c56 6572 7369 6f6e  .0</modelVersion
-000000e0: 3e0d 0a0d 0a20 2020 203c 6772 6f75 7049  >....    <groupI
-000000f0: 643e 6172 6773 5b30 5d3c 2f67 726f 7570  d>args[0]</group
-00000100: 4964 3e0d 0a20 2020 203c 6172 7469 6661  Id>..    <artifa
-00000110: 6374 4964 3e61 7267 735b 315d 6172 6773  ctId>args[1]args
-00000120: 5b33 5d3c 2f61 7274 6966 6163 7449 643e  [3]</artifactId>
-00000130: 0d0a 2020 2020 3c70 6163 6b61 6769 6e67  ..    <packaging
-00000140: 3e6a 6172 3c2f 7061 636b 6167 696e 673e  >jar</packaging>
-00000150: 0d0a 2020 2020 3c76 6572 7369 6f6e 3e31  ..    <version>1
-00000160: 2e30 2d53 4e41 5053 484f 543c 2f76 6572  .0-SNAPSHOT</ver
-00000170: 7369 6f6e 3e0d 0a20 2020 203c 6e61 6d65  sion>..    <name
-00000180: 3e61 7267 735b 315d 6172 6773 5b33 5d3c  >args[1]args[3]<
-00000190: 2f6e 616d 653e 0d0a 0d0a 2020 2020 3c70  /name>....    <p
-000001a0: 726f 7065 7274 6965 733e 0d0a 2020 2020  roperties>..    
-000001b0: 2020 2020 3c6d 6176 656e 2e63 6f6d 7069      <maven.compi
-000001c0: 6c65 722e 736f 7572 6365 3e31 313c 2f6d  ler.source>11</m
-000001d0: 6176 656e 2e63 6f6d 7069 6c65 722e 736f  aven.compiler.so
-000001e0: 7572 6365 3e0d 0a20 2020 2020 2020 203c  urce>..        <
-000001f0: 6d61 7665 6e2e 636f 6d70 696c 6572 2e74  maven.compiler.t
-00000200: 6172 6765 743e 3131 3c2f 6d61 7665 6e2e  arget>11</maven.
-00000210: 636f 6d70 696c 6572 2e74 6172 6765 743e  compiler.target>
-00000220: 0d0a 2020 2020 2020 2020 3c70 726f 6a65  ..        <proje
-00000230: 6374 2e62 7569 6c64 2e73 6f75 7263 6545  ct.build.sourceE
-00000240: 6e63 6f64 696e 673e 5554 462d 383c 2f70  ncoding>UTF-8</p
-00000250: 726f 6a65 6374 2e62 7569 6c64 2e73 6f75  roject.build.sou
-00000260: 7263 6545 6e63 6f64 696e 673e 0d0a 2020  rceEncoding>..  
-00000270: 2020 3c2f 7072 6f70 6572 7469 6573 3e0d    </properties>.
-00000280: 0a0d 0a20 2020 203c 6465 7065 6e64 656e  ...    <dependen
-00000290: 6369 6573 3e0d 0a20 2020 2020 2020 203c  cies>..        <
-000002a0: 6465 7065 6e64 656e 6379 3e0d 0a20 2020  dependency>..   
-000002b0: 2020 2020 2020 2020 203c 6772 6f75 7049           <groupI
-000002c0: 643e 6172 6773 5b30 5d3c 2f67 726f 7570  d>args[0]</group
-000002d0: 4964 3e0d 0a20 2020 2020 2020 2020 2020  Id>..           
-000002e0: 203c 6172 7469 6661 6374 4964 3e61 7267   <artifactId>arg
-000002f0: 735b 315d 2d63 6f72 653c 2f61 7274 6966  s[1]-core</artif
-00000300: 6163 7449 643e 0d0a 2020 2020 2020 2020  actId>..        
-00000310: 2020 2020 3c76 6572 7369 6f6e 3e31 2e30      <version>1.0
-00000320: 2d53 4e41 5053 484f 543c 2f76 6572 7369  -SNAPSHOT</versi
-00000330: 6f6e 3e0d 0a20 2020 2020 2020 203c 2f64  on>..        </d
-00000340: 6570 656e 6465 6e63 793e 0d0a 2020 2020  ependency>..    
-00000350: 2020 2020 3c64 6570 656e 6465 6e63 793e      <dependency>
-00000360: 0d0a 2020 2020 2020 2020 2020 2020 3c67  ..            <g
-00000370: 726f 7570 4964 3e63 682e 716f 732e 6c6f  roupId>ch.qos.lo
-00000380: 6762 6163 6b3c 2f67 726f 7570 4964 3e0d  gback</groupId>.
-00000390: 0a20 2020 2020 2020 2020 2020 203c 6172  .            <ar
-000003a0: 7469 6661 6374 4964 3e6c 6f67 6261 636b  tifactId>logback
-000003b0: 2d63 6c61 7373 6963 3c2f 6172 7469 6661  -classic</artifa
-000003c0: 6374 4964 3e0d 0a20 2020 2020 2020 2020  ctId>..         
-000003d0: 2020 203c 7665 7273 696f 6e3e 312e 342e     <version>1.4.
-000003e0: 373c 2f76 6572 7369 6f6e 3e0d 0a20 2020  7</version>..   
-000003f0: 2020 2020 203c 2f64 6570 656e 6465 6e63       </dependenc
-00000400: 793e 0d0a 2020 2020 3c2f 6465 7065 6e64  y>..    </depend
-00000410: 656e 6369 6573 3e0d 0a0d 0a3c 2f70 726f  encies>....</pro
-00000420: 6a65 6374 3e                             ject>
+000000b0: 302e 7873 6422 3e0d 0a20 2020 203c 6d6f  0.xsd">..    <mo
+000000c0: 6465 6c56 6572 7369 6f6e 3e34 2e30 2e30  delVersion>4.0.0
+000000d0: 3c2f 6d6f 6465 6c56 6572 7369 6f6e 3e0d  </modelVersion>.
+000000e0: 0a0d 0a20 2020 203c 6772 6f75 7049 643e  ...    <groupId>
+000000f0: 6172 6773 5b30 5d3c 2f67 726f 7570 4964  args[0]</groupId
+00000100: 3e0d 0a20 2020 203c 6172 7469 6661 6374  >..    <artifact
+00000110: 4964 3e3c 7363 3e61 7267 735b 315d 6172  Id><sc>args[1]ar
+00000120: 6773 5b33 5d3c 7363 3e3c 2f61 7274 6966  gs[3]<sc></artif
+00000130: 6163 7449 643e 0d0a 2020 2020 3c70 6163  actId>..    <pac
+00000140: 6b61 6769 6e67 3e6a 6172 3c2f 7061 636b  kaging>jar</pack
+00000150: 6167 696e 673e 0d0a 2020 2020 3c76 6572  aging>..    <ver
+00000160: 7369 6f6e 3e31 2e30 2d53 4e41 5053 484f  sion>1.0-SNAPSHO
+00000170: 543c 2f76 6572 7369 6f6e 3e0d 0a20 2020  T</version>..   
+00000180: 203c 6e61 6d65 3e3c 7363 3e61 7267 735b   <name><sc>args[
+00000190: 315d 6172 6773 5b33 5d3c 7363 3e3c 2f6e  1]args[3]<sc></n
+000001a0: 616d 653e 0d0a 0d0a 2020 2020 3c75 726c  ame>....    <url
+000001b0: 3e68 7474 703a 2f2f 6d61 7665 6e2e 6170  >http://maven.ap
+000001c0: 6163 6865 2e6f 7267 3c2f 7572 6c3e 0d0a  ache.org</url>..
+000001d0: 0d0a 2020 2020 3c70 726f 7065 7274 6965  ..    <propertie
+000001e0: 733e 0d0a 2020 2020 2020 2020 3c6d 6176  s>..        <mav
+000001f0: 656e 2e63 6f6d 7069 6c65 722e 736f 7572  en.compiler.sour
+00000200: 6365 3e31 313c 2f6d 6176 656e 2e63 6f6d  ce>11</maven.com
+00000210: 7069 6c65 722e 736f 7572 6365 3e0d 0a20  piler.source>.. 
+00000220: 2020 2020 2020 203c 6d61 7665 6e2e 636f         <maven.co
+00000230: 6d70 696c 6572 2e74 6172 6765 743e 3131  mpiler.target>11
+00000240: 3c2f 6d61 7665 6e2e 636f 6d70 696c 6572  </maven.compiler
+00000250: 2e74 6172 6765 743e 0d0a 2020 2020 2020  .target>..      
+00000260: 2020 3c70 726f 6a65 6374 2e62 7569 6c64    <project.build
+00000270: 2e73 6f75 7263 6545 6e63 6f64 696e 673e  .sourceEncoding>
+00000280: 5554 462d 383c 2f70 726f 6a65 6374 2e62  UTF-8</project.b
+00000290: 7569 6c64 2e73 6f75 7263 6545 6e63 6f64  uild.sourceEncod
+000002a0: 696e 673e 0d0a 2020 2020 3c2f 7072 6f70  ing>..    </prop
+000002b0: 6572 7469 6573 3e0d 0a0d 0a20 2020 203c  erties>....    <
+000002c0: 6465 7065 6e64 656e 6369 6573 3e0d 0a20  dependencies>.. 
+000002d0: 2020 2020 2020 203c 6465 7065 6e64 656e         <dependen
+000002e0: 6379 3e0d 0a20 2020 2020 2020 2020 2020  cy>..           
+000002f0: 203c 6772 6f75 7049 643e 6f72 672e 6a75   <groupId>org.ju
+00000300: 6e69 742e 6a75 7069 7465 723c 2f67 726f  nit.jupiter</gro
+00000310: 7570 4964 3e0d 0a20 2020 2020 2020 2020  upId>..         
+00000320: 2020 203c 6172 7469 6661 6374 4964 3e6a     <artifactId>j
+00000330: 756e 6974 2d6a 7570 6974 6572 2d65 6e67  unit-jupiter-eng
+00000340: 696e 653c 2f61 7274 6966 6163 7449 643e  ine</artifactId>
+00000350: 0d0a 2020 2020 2020 2020 2020 2020 3c76  ..            <v
+00000360: 6572 7369 6f6e 3e35 2e39 2e30 3c2f 7665  ersion>5.9.0</ve
+00000370: 7273 696f 6e3e 0d0a 2020 2020 2020 2020  rsion>..        
+00000380: 2020 2020 3c73 636f 7065 3e74 6573 743c      <scope>test<
+00000390: 2f73 636f 7065 3e0d 0a20 2020 2020 2020  /scope>..       
+000003a0: 203c 2f64 6570 656e 6465 6e63 793e 0d0a   </dependency>..
+000003b0: 2020 2020 2020 2020 3c64 6570 656e 6465          <depende
+000003c0: 6e63 793e 0d0a 2020 2020 2020 2020 2020  ncy>..          
+000003d0: 2020 3c67 726f 7570 4964 3e6f 7267 2e6d    <groupId>org.m
+000003e0: 6f63 6b69 746f 3c2f 6772 6f75 7049 643e  ockito</groupId>
+000003f0: 0d0a 2020 2020 2020 2020 2020 2020 3c61  ..            <a
+00000400: 7274 6966 6163 7449 643e 6d6f 636b 6974  rtifactId>mockit
+00000410: 6f2d 636f 7265 3c2f 6172 7469 6661 6374  o-core</artifact
+00000420: 4964 3e0d 0a20 2020 2020 2020 2020 2020  Id>..           
+00000430: 203c 7665 7273 696f 6e3e 342e 382e 303c   <version>4.8.0<
+00000440: 2f76 6572 7369 6f6e 3e0d 0a20 2020 2020  /version>..     
+00000450: 2020 2020 2020 203c 7363 6f70 653e 7465         <scope>te
+00000460: 7374 3c2f 7363 6f70 653e 0d0a 2020 2020  st</scope>..    
+00000470: 2020 2020 3c2f 6465 7065 6e64 656e 6379      </dependency
+00000480: 3e0d 0a20 2020 2020 2020 203c 6465 7065  >..        <depe
+00000490: 6e64 656e 6379 3e0d 0a20 2020 2020 2020  ndency>..       
+000004a0: 2020 2020 203c 6772 6f75 7049 643e 6f72       <groupId>or
+000004b0: 672e 6d6f 636b 6974 6f3c 2f67 726f 7570  g.mockito</group
+000004c0: 4964 3e0d 0a20 2020 2020 2020 2020 2020  Id>..           
+000004d0: 203c 6172 7469 6661 6374 4964 3e6d 6f63   <artifactId>moc
+000004e0: 6b69 746f 2d6a 756e 6974 2d6a 7570 6974  kito-junit-jupit
+000004f0: 6572 3c2f 6172 7469 6661 6374 4964 3e0d  er</artifactId>.
+00000500: 0a20 2020 2020 2020 2020 2020 203c 7665  .            <ve
+00000510: 7273 696f 6e3e 342e 382e 303c 2f76 6572  rsion>4.8.0</ver
+00000520: 7369 6f6e 3e0d 0a20 2020 2020 2020 2020  sion>..         
+00000530: 2020 203c 7363 6f70 653e 7465 7374 3c2f     <scope>test</
+00000540: 7363 6f70 653e 0d0a 2020 2020 2020 2020  scope>..        
+00000550: 3c2f 6465 7065 6e64 656e 6379 3e0d 0a20  </dependency>.. 
+00000560: 2020 2020 2020 203c 6465 7065 6e64 656e         <dependen
+00000570: 6379 3e0d 0a20 2020 2020 2020 2020 2020  cy>..           
+00000580: 203c 6772 6f75 7049 643e 6a75 6e69 743c   <groupId>junit<
+00000590: 2f67 726f 7570 4964 3e0d 0a20 2020 2020  /groupId>..     
+000005a0: 2020 2020 2020 203c 6172 7469 6661 6374         <artifact
+000005b0: 4964 3e6a 756e 6974 3c2f 6172 7469 6661  Id>junit</artifa
+000005c0: 6374 4964 3e0d 0a20 2020 2020 2020 2020  ctId>..         
+000005d0: 2020 203c 7665 7273 696f 6e3e 332e 382e     <version>3.8.
+000005e0: 313c 2f76 6572 7369 6f6e 3e0d 0a20 2020  1</version>..   
+000005f0: 2020 2020 2020 2020 203c 7363 6f70 653e           <scope>
+00000600: 7465 7374 3c2f 7363 6f70 653e 0d0a 2020  test</scope>..  
+00000610: 2020 2020 2020 3c2f 6465 7065 6e64 656e        </dependen
+00000620: 6379 3e0d 0a20 2020 2020 2020 203c 6465  cy>..        <de
+00000630: 7065 6e64 656e 6379 3e0d 0a20 2020 2020  pendency>..     
+00000640: 2020 2020 2020 203c 6772 6f75 7049 643e         <groupId>
+00000650: 6172 6773 5b30 5d3c 2f67 726f 7570 4964  args[0]</groupId
+00000660: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00000670: 6172 7469 6661 6374 4964 3e61 7267 735b  artifactId>args[
+00000680: 315d 2d61 6461 7074 6572 733c 2f61 7274  1]-adapters</art
+00000690: 6966 6163 7449 643e 0d0a 2020 2020 2020  ifactId>..      
+000006a0: 2020 2020 2020 3c76 6572 7369 6f6e 3e31        <version>1
+000006b0: 2e30 2d53 4e41 5053 484f 543c 2f76 6572  .0-SNAPSHOT</ver
+000006c0: 7369 6f6e 3e0d 0a20 2020 2020 2020 203c  sion>..        <
+000006d0: 2f64 6570 656e 6465 6e63 793e 0d0a 2020  /dependency>..  
+000006e0: 2020 3c2f 6465 7065 6e64 656e 6369 6573    </dependencies
+000006f0: 3e0d 0a3c 2f70 726f 6a65 6374 3e         >..</project>
```

### Comparing `cae_cli-0.1.1/cae/templates/use_case.txt` & `cae_cli-0.1.2/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.1/cae/templates/use_case_factory.txt` & `cae_cli-0.1.2/cae/templates/use_case_factory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.1/cae/templates/use_case_implementation.txt` & `cae_cli-0.1.2/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.1/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.1.2/cae_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

