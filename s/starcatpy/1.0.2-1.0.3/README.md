# Comparing `tmp/starcatpy-1.0.2.tar.gz` & `tmp/starcatpy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starcatpy-1.0.2.tar", last modified: Thu May  2 21:42:43 2024, max compression
+gzip compressed data, was "starcatpy-1.0.3.tar", last modified: Tue May  7 18:20:32 2024, max compression
```

## Comparing `starcatpy-1.0.2.tar` & `starcatpy-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-02 21:42:43.098060 starcatpy-1.0.2/
--rw-r--r--   0 dkotliar   (503) staff       (20)     1070 2024-05-02 20:08:01.000000 starcatpy-1.0.2/LICENSE
--rw-r--r--   0 dkotliar   (503) staff       (20)     3816 2024-05-02 21:42:43.097561 starcatpy-1.0.2/PKG-INFO
--rw-r--r--   0 dkotliar   (503) staff       (20)     2960 2024-05-02 21:00:49.000000 starcatpy-1.0.2/README.md
--rw-r--r--   0 dkotliar   (503) staff       (20)      103 2024-05-02 20:08:01.000000 starcatpy-1.0.2/pyproject.toml
--rw-r--r--   0 dkotliar   (503) staff       (20)       38 2024-05-02 21:42:43.098190 starcatpy-1.0.2/setup.cfg
--rw-r--r--   0 dkotliar   (503) staff       (20)     1191 2024-05-02 21:34:22.000000 starcatpy-1.0.2/setup.py
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-02 21:42:43.089421 starcatpy-1.0.2/src/
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-02 21:42:43.092904 starcatpy-1.0.2/src/starcat/
--rwxr-xr-x   0 dkotliar   (503) staff       (20)       35 2024-05-02 20:08:01.000000 starcatpy-1.0.2/src/starcat/__init__.py
--rwxr-xr-x   0 dkotliar   (503) staff       (20)    19188 2024-05-02 20:23:44.000000 starcatpy-1.0.2/src/starcat/starcat.py
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-02 21:42:43.096937 starcatpy-1.0.2/src/starcatpy.egg-info/
--rw-r--r--   0 dkotliar   (503) staff       (20)     3816 2024-05-02 21:42:43.000000 starcatpy-1.0.2/src/starcatpy.egg-info/PKG-INFO
--rw-r--r--   0 dkotliar   (503) staff       (20)      312 2024-05-02 21:42:43.000000 starcatpy-1.0.2/src/starcatpy.egg-info/SOURCES.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)        1 2024-05-02 21:42:43.000000 starcatpy-1.0.2/src/starcatpy.egg-info/dependency_links.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)       41 2024-05-02 21:42:43.000000 starcatpy-1.0.2/src/starcatpy.egg-info/entry_points.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)       90 2024-05-02 21:42:43.000000 starcatpy-1.0.2/src/starcatpy.egg-info/requires.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)        8 2024-05-02 21:42:43.000000 starcatpy-1.0.2/src/starcatpy.egg-info/top_level.txt
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-07 18:20:32.789781 starcatpy-1.0.3/
+-rw-r--r--   0 dkotliar   (503) staff       (20)     1070 2024-05-07 17:57:18.000000 starcatpy-1.0.3/LICENSE
+-rw-r--r--   0 dkotliar   (503) staff       (20)     3846 2024-05-07 18:20:32.789279 starcatpy-1.0.3/PKG-INFO
+-rw-r--r--   0 dkotliar   (503) staff       (20)     3001 2024-05-07 17:57:18.000000 starcatpy-1.0.3/README.md
+-rw-r--r--   0 dkotliar   (503) staff       (20)      103 2024-05-07 17:57:18.000000 starcatpy-1.0.3/pyproject.toml
+-rw-r--r--   0 dkotliar   (503) staff       (20)       38 2024-05-07 18:20:32.789929 starcatpy-1.0.3/setup.cfg
+-rw-r--r--   0 dkotliar   (503) staff       (20)     1180 2024-05-07 18:19:09.000000 starcatpy-1.0.3/setup.py
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-07 18:20:32.782842 starcatpy-1.0.3/src/
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-07 18:20:32.785362 starcatpy-1.0.3/src/starcat/
+-rwxr-xr-x   0 dkotliar   (503) staff       (20)       35 2024-05-07 17:57:18.000000 starcatpy-1.0.3/src/starcat/__init__.py
+-rwxr-xr-x   0 dkotliar   (503) staff       (20)    19404 2024-05-07 18:13:39.000000 starcatpy-1.0.3/src/starcat/starcat.py
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-07 18:20:32.788619 starcatpy-1.0.3/src/starcatpy.egg-info/
+-rw-r--r--   0 dkotliar   (503) staff       (20)     3846 2024-05-07 18:20:32.000000 starcatpy-1.0.3/src/starcatpy.egg-info/PKG-INFO
+-rw-r--r--   0 dkotliar   (503) staff       (20)      312 2024-05-07 18:20:32.000000 starcatpy-1.0.3/src/starcatpy.egg-info/SOURCES.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)        1 2024-05-07 18:20:32.000000 starcatpy-1.0.3/src/starcatpy.egg-info/dependency_links.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)       41 2024-05-07 18:20:32.000000 starcatpy-1.0.3/src/starcatpy.egg-info/entry_points.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)       90 2024-05-07 18:20:32.000000 starcatpy-1.0.3/src/starcatpy.egg-info/requires.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)        8 2024-05-07 18:20:32.000000 starcatpy-1.0.3/src/starcatpy.egg-info/top_level.txt
```

### Comparing `starcatpy-1.0.2/LICENSE` & `starcatpy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `starcatpy-1.0.2/PKG-INFO` & `starcatpy-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: starcatpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Implements *CellAnnotator (aka *CAT/starCAT), annotating scRNA-Seq with predefined gene expression programs
 Home-page: https://github.com/immunogenomics/starCAT
 Author: Dylan Kotliar, Michelle Curtis
-Author-email: dkotliar@broadinstitute.org, curtism@broadinstitute.org
+Author-email: dylkot@gmail.com, curtism@broadinstitute.org
 Project-URL: Bug Tracker, https://github.com/immunogenomics/starCAT/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn>=1.0
@@ -22,15 +22,15 @@
 Requires-Dist: pyyaml
 Requires-Dist: cnmf
 
 # starCAT
 Implements *CellAnnotator (aka *CAT/starCAT), annotating scRNA-Seq with predefined gene expression programs
 
 ## Citation
-If you use *CAT, please cite our [preprint]().
+If you use *CAT, please cite our [preprint](https://doi.org/10.1101/2024.05.03.592310).
 
 ## Installation
 
 You can install starCAT and its dependencies via the Python Package Index.
 ```bash
 pip install starcatpy
 ```
```

### Comparing `starcatpy-1.0.2/README.md` & `starcatpy-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # starCAT
 Implements *CellAnnotator (aka *CAT/starCAT), annotating scRNA-Seq with predefined gene expression programs
 
 ## Citation
-If you use *CAT, please cite our [preprint]().
+If you use *CAT, please cite our [preprint](https://doi.org/10.1101/2024.05.03.592310).
 
 ## Installation
 
 You can install starCAT and its dependencies via the Python Package Index.
 ```bash
 pip install starcatpy
 ```
```

### Comparing `starcatpy-1.0.2/setup.py` & `starcatpy-1.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="starcatpy",
-    version="1.0.2",
+    version="1.0.3",
     author="Dylan Kotliar, Michelle Curtis",
-    author_email="dkotliar@broadinstitute.org, curtism@broadinstitute.org",
+    author_email="dylkot@gmail.com, curtism@broadinstitute.org",
     description="Implements *CellAnnotator (aka *CAT/starCAT), annotating scRNA-Seq with predefined gene expression programs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/immunogenomics/starCAT",
     project_urls={
         "Bug Tracker": "https://github.com/immunogenomics/starCAT/issues",
     },
```

### Comparing `starcatpy-1.0.2/src/starcat/starcat.py` & `starcatpy-1.0.3/src/starcat/starcat.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,16 +281,15 @@
         ----------
         query : query AnnData object or pandas.DataFrame, cells X genes
         
         return_unnormalized : boolean, if True, return unnormalized usage. Default returns usages normalized to 1
 
         """
 
-        query = self.prepare_query(query)
-            
+        query = self.prepare_query(query)        
         self.usage = self.fit_query_usage(query)
         self.usage_norm = self.usage.div(self.usage.sum(axis=1), axis=0)
         
         if len(self.score_data) > 0:
             self.scores = self.compute_addon_scores()
         
         if return_unnormalized:
@@ -320,16 +319,20 @@
             warnings.warn("""WARNING!: query input is not an integer count matrix as expected.
             Please provide an integer count matrix unless you are sure you know what you are doing.""", UserWarning)
             
         overlap_genes = sorted(set(self.ref.columns).intersection(set(query.var.index)))
         print('%d out of %d genes in the reference overlap with the query' % (len(overlap_genes), self.ref.shape[1]))
         self.overlap_genes = overlap_genes
         query = query[:, self.overlap_genes].copy()
-
         sc.pp.scale(query, zero_center=False)
+
+        # In python 3.10, scale casts query as float64. Here just ensure its same dtype as reference
+        if query.X.dtype != self.ref.values.dtype:
+            query.X = query.X.astype(self.ref.values.dtype)
+        
         return query
          
         
     def fit_query_usage(self, query):
         rf_usages = self.refit_usage(query.X, self.ref[self.overlap_genes].values,
                          self._nmf_kwargs.copy())          
         rf_usages = pd.DataFrame(rf_usages, index=query.obs.index,
```

### Comparing `starcatpy-1.0.2/src/starcatpy.egg-info/PKG-INFO` & `starcatpy-1.0.3/src/starcatpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: starcatpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Implements *CellAnnotator (aka *CAT/starCAT), annotating scRNA-Seq with predefined gene expression programs
 Home-page: https://github.com/immunogenomics/starCAT
 Author: Dylan Kotliar, Michelle Curtis
-Author-email: dkotliar@broadinstitute.org, curtism@broadinstitute.org
+Author-email: dylkot@gmail.com, curtism@broadinstitute.org
 Project-URL: Bug Tracker, https://github.com/immunogenomics/starCAT/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn>=1.0
@@ -22,15 +22,15 @@
 Requires-Dist: pyyaml
 Requires-Dist: cnmf
 
 # starCAT
 Implements *CellAnnotator (aka *CAT/starCAT), annotating scRNA-Seq with predefined gene expression programs
 
 ## Citation
-If you use *CAT, please cite our [preprint]().
+If you use *CAT, please cite our [preprint](https://doi.org/10.1101/2024.05.03.592310).
 
 ## Installation
 
 You can install starCAT and its dependencies via the Python Package Index.
 ```bash
 pip install starcatpy
 ```
```

