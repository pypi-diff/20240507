# Comparing `tmp/circadipy-0.1.8.tar.gz` & `tmp/circadipy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circadipy-0.1.8.tar", last modified: Mon Apr 29 22:30:30 2024, max compression
+gzip compressed data, was "circadipy-0.1.9.tar", last modified: Tue May  7 14:14:50 2024, max compression
```

## Comparing `circadipy-0.1.8.tar` & `circadipy-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 22:30:30.375301 circadipy-0.1.8/
--rw-rw-rw-   0        0        0    35823 2024-04-29 18:19:55.000000 circadipy-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       45 2024-04-29 22:30:26.000000 circadipy-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2773 2024-04-29 22:30:30.375301 circadipy-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1930 2024-04-29 18:19:55.000000 circadipy-0.1.8/README.md
--rw-rw-rw-   0        0        0       82 2024-04-29 18:19:55.000000 circadipy-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      851 2024-04-29 22:30:30.376300 circadipy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-29 18:19:55.000000 circadipy-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:30:30.360038 circadipy-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 22:30:30.367302 circadipy-0.1.8/src/circadipy/
--rw-rw-rw-   0        0        0        0 2024-04-29 18:19:55.000000 circadipy-0.1.8/src/circadipy/__init__.py
--rw-rw-rw-   0        0        0    76597 2024-04-29 18:20:00.000000 circadipy-0.1.8/src/circadipy/chrono_plotter.py
--rw-rw-rw-   0        0        0    65011 2024-04-29 18:20:00.000000 circadipy-0.1.8/src/circadipy/chrono_reader.py
--rw-rw-rw-   0        0        0    23915 2024-04-29 18:20:00.000000 circadipy-0.1.8/src/circadipy/chrono_rhythm.py
--rw-rw-rw-   0        0        0    16070 2024-04-29 18:20:00.000000 circadipy-0.1.8/src/circadipy/chrono_simulation.py
--rw-rw-rw-   0        0        0    42182 2024-04-29 21:26:25.000000 circadipy-0.1.8/src/circadipy/tutorial_pipeline.ipynb
-drwxrwxrwx   0        0        0        0 2024-04-29 22:30:30.374301 circadipy-0.1.8/src/circadipy.egg-info/
--rw-rw-rw-   0        0        0     2773 2024-04-29 22:30:30.000000 circadipy-0.1.8/src/circadipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2024-04-29 22:30:30.000000 circadipy-0.1.8/src/circadipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 22:30:30.000000 circadipy-0.1.8/src/circadipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      253 2024-04-29 22:30:30.000000 circadipy-0.1.8/src/circadipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-29 22:30:30.000000 circadipy-0.1.8/src/circadipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-29 19:15:32.000000 circadipy-0.1.8/src/circadipy.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-05-07 14:14:50.439068 circadipy-0.1.9/
+-rw-rw-rw-   0        0        0    35823 2024-04-29 18:19:55.000000 circadipy-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-04-29 22:30:26.000000 circadipy-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2773 2024-05-07 14:14:50.439068 circadipy-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1930 2024-04-29 18:19:55.000000 circadipy-0.1.9/README.md
+-rw-rw-rw-   0        0        0       82 2024-04-29 18:19:55.000000 circadipy-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      851 2024-05-07 14:14:50.440069 circadipy-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-29 18:19:55.000000 circadipy-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:14:50.367989 circadipy-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 14:14:50.428066 circadipy-0.1.9/src/circadipy/
+-rw-rw-rw-   0        0        0        0 2024-04-29 18:19:55.000000 circadipy-0.1.9/src/circadipy/__init__.py
+-rw-rw-rw-   0        0        0    76597 2024-04-29 18:20:00.000000 circadipy-0.1.9/src/circadipy/chrono_plotter.py
+-rw-rw-rw-   0        0        0    65011 2024-04-29 18:20:00.000000 circadipy-0.1.9/src/circadipy/chrono_reader.py
+-rw-rw-rw-   0        0        0    23915 2024-04-29 18:20:00.000000 circadipy-0.1.9/src/circadipy/chrono_rhythm.py
+-rw-rw-rw-   0        0        0    16070 2024-04-29 18:20:00.000000 circadipy-0.1.9/src/circadipy/chrono_simulation.py
+-rw-rw-rw-   0        0        0    42159 2024-05-03 12:14:52.000000 circadipy-0.1.9/src/circadipy/tutorial_pipeline.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-07 14:14:50.438068 circadipy-0.1.9/src/circadipy.egg-info/
+-rw-rw-rw-   0        0        0     2773 2024-05-07 14:14:50.000000 circadipy-0.1.9/src/circadipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2024-05-07 14:14:50.000000 circadipy-0.1.9/src/circadipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:14:50.000000 circadipy-0.1.9/src/circadipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      253 2024-05-07 14:14:50.000000 circadipy-0.1.9/src/circadipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-07 14:14:50.000000 circadipy-0.1.9/src/circadipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-29 19:15:32.000000 circadipy-0.1.9/src/circadipy.egg-info/zip-safe
```

### Comparing `circadipy-0.1.8/LICENSE` & `circadipy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `circadipy-0.1.8/PKG-INFO` & `circadipy-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circadipy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tool for analyzing and visualizing circadian cycle data
 Home-page: https://github.com/mcjpedro/circadipy
 Author: João Pedro Carvalho Moreira
 Author-email: mcjpedro@gmail.com
 Keywords: circadian,chronobiology,data
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `circadipy-0.1.8/README.md` & `circadipy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `circadipy-0.1.8/setup.cfg` & `circadipy-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6972 6361 6469 7079 0d0a 7665   = circadipy..ve
-00000020: 7273 696f 6e20 3d20 302e 312e 380d 0a61  rsion = 0.1.8..a
+00000020: 7273 696f 6e20 3d20 302e 312e 390d 0a61  rsion = 0.1.9..a
 00000030: 7574 686f 7220 3d20 4a6f c3a3 6f20 5065  uthor = Jo..o Pe
 00000040: 6472 6f20 4361 7276 616c 686f 204d 6f72  dro Carvalho Mor
 00000050: 6569 7261 0d0a 6175 7468 6f72 5f65 6d61  eira..author_ema
 00000060: 696c 203d 206d 636a 7065 6472 6f40 676d  il = mcjpedro@gm
 00000070: 6169 6c2e 636f 6d0d 0a75 726c 203d 2068  ail.com..url = h
 00000080: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 00000090: 6d2f 6d63 6a70 6564 726f 2f63 6972 6361  m/mcjpedro/circa
```

### Comparing `circadipy-0.1.8/src/circadipy/chrono_plotter.py` & `circadipy-0.1.9/src/circadipy/chrono_plotter.py`

 * *Files identical despite different names*

### Comparing `circadipy-0.1.8/src/circadipy/chrono_reader.py` & `circadipy-0.1.9/src/circadipy/chrono_reader.py`

 * *Files identical despite different names*

### Comparing `circadipy-0.1.8/src/circadipy/chrono_rhythm.py` & `circadipy-0.1.9/src/circadipy/chrono_rhythm.py`

 * *Files identical despite different names*

### Comparing `circadipy-0.1.8/src/circadipy/chrono_simulation.py` & `circadipy-0.1.9/src/circadipy/chrono_simulation.py`

 * *Files identical despite different names*

### Comparing `circadipy-0.1.8/src/circadipy/tutorial_pipeline.ipynb` & `circadipy-0.1.9/src/circadipy/tutorial_pipeline.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.8.19'}}"}*

```diff
@@ -804,15 +804,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "undefined.undefined.undefined"
+            "version": "3.8.19"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2939af26a36fc942e0c066bfc7148c204547295e343f43ef46c39eb3082d0963"
             }
         }
     },
```

### Comparing `circadipy-0.1.8/src/circadipy.egg-info/PKG-INFO` & `circadipy-0.1.9/src/circadipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circadipy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tool for analyzing and visualizing circadian cycle data
 Home-page: https://github.com/mcjpedro/circadipy
 Author: João Pedro Carvalho Moreira
 Author-email: mcjpedro@gmail.com
 Keywords: circadian,chronobiology,data
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

