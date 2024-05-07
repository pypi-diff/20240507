# Comparing `tmp/porgo-1.0.1-py3-none-any.whl.zip` & `tmp/porgo-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5512 bytes, number of entries: 9
+Zip file size: 5585 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      225 b- defN 24-Mar-23 13:55 porgo/__init__.py
 -rw-rw-rw-  2.0 fat      157 b- defN 24-Mar-21 07:37 porgo/_typing.py
--rw-rw-rw-  2.0 fat       57 b- defN 24-Apr-09 10:19 porgo/_version.py
--rw-rw-rw-  2.0 fat     4193 b- defN 24-Apr-09 10:35 porgo/runtime.py
--rw-rw-rw-  2.0 fat     1089 b- defN 24-Apr-09 10:39 porgo-1.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3285 b- defN 24-Apr-09 10:39 porgo-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-09 10:39 porgo-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-09 10:39 porgo-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      665 b- defN 24-Apr-09 10:39 porgo-1.0.1.dist-info/RECORD
-9 files, 9769 bytes uncompressed, 4376 bytes compressed:  55.2%
+-rw-rw-rw-  2.0 fat       57 b- defN 24-May-07 12:29 porgo/_version.py
+-rw-rw-rw-  2.0 fat     4292 b- defN 24-May-07 12:58 porgo/runtime.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 24-May-07 13:08 porgo-1.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3400 b- defN 24-May-07 13:08 porgo-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 13:08 porgo-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-07 13:08 porgo-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      665 b- defN 24-May-07 13:08 porgo-1.1.0.dist-info/RECORD
+9 files, 9983 bytes uncompressed, 4449 bytes compressed:  55.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: porgo/_version.py
 Comment: 
 
 Filename: porgo/runtime.py
 Comment: 
 
-Filename: porgo-1.0.1.dist-info/LICENSE
+Filename: porgo-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: porgo-1.0.1.dist-info/METADATA
+Filename: porgo-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: porgo-1.0.1.dist-info/WHEEL
+Filename: porgo-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: porgo-1.0.1.dist-info/top_level.txt
+Filename: porgo-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: porgo-1.0.1.dist-info/RECORD
+Filename: porgo-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## porgo/_version.py

```diff
@@ -1,3 +1,3 @@
 # Copyright (c) 2024 linjing-lab
 
-__version__ = '1.0.1'
+__version__ = '1.1.0'
```

## porgo/runtime.py

```diff
@@ -74,17 +74,17 @@
         '''
         assert cycles > 0
         for _ in range(cycles): 
             self._evo_pop()
 
     def result(self, verbose: bool=False) -> None:
         '''
-        Find the best converged result or output console information with `verbose=True`.
+        Find the top 3 updated results or output console information with `verbose=True`.
         :param verbose: bool. whether to output console information with 'index point value'. default: False.
         '''
         if not verbose:
-            best_index = numpy.argmin([self.obj(updated) for updated in self.uniform])
-            self.best = self.uniform[best_index]
-            self.best_fit = self.obj(self.best)
+            top3_index = numpy.argsort([self.obj(updated) for updated in self.uniform])[:3]
+            self.mini, self.medi, self.maxi = self.uniform[top3_index]
+            self.fit_mini, self.fit_medi, self.fit_maxi = self.obj(self.mini), self.obj(self.medi), self.obj(self.maxi)
         else:
             for i, updated in enumerate(self.uniform):
                 print('{}\t{}\t{}'.format(i, updated, self.obj(updated)))
```

## Comparing `porgo-1.0.1.dist-info/LICENSE` & `porgo-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `porgo-1.0.1.dist-info/METADATA` & `porgo-1.1.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porgo
-Version: 1.0.1
+Version: 1.1.0
 Summary: The portable universal library in global optimization.
 Home-page: https://github.com/linjing-lab/porgo
 Download-URL: https://github.com/linjing-lab/porgo/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MIT
 Project-URL: Source, https://github.com/linjing-lab/porgo/tree/master/porgo/
@@ -43,27 +43,27 @@
 
 ## glos
 
 glos is the main runtime to serve as a global search class, users can run train_gen module with given cycles at any times until the function searching process converged.
 
 init:
 - objective_function: *Callable*, a high-dimensional function with convex, non-convex, and many local minima.
-- bounds: *List[List[float]] | List[Tuple[float]]*, changes this value makes a significant influence of best and best_fit.
+- bounds: *List[List[float]] | List[Tuple[float]]*, changes this value makes a significant influence of mini and fit_mini.
 - mutation: *float=0.5*, increase this value makes the search radius larger.
 - recombination: *float=0.9*, increase this value allows larger number of mutation.
 
 rand_pop:
 - population_size: *int=50*, randomly init the population (or called initial points) with shape at (population, dimension).
 - verbose: *bool=False*, whether to output initial population when manually replace the random generated rule.
 
 train_gen:
 - cycles: *int=1000*, try to run several times (until converged) when give a smaller cycle number if search bounds is in large space.
 
 result:
-- verbose: *bool=False*, whether to output console information after search populations were updated (check self.best and self.best_fit).
+- verbose: *bool=False*, whether to output console information after search populations were updated (check self.mini and self.fit_mini, the top3 updated results are (self.mini, self.fit_mini) < (self.medi, self.fit_medi) < (self.maxi, self.fit_maxi)).
 
 ## reference
 
 Storn, R and Price, K, Differential Evolution - a Simple and Efficient Heuristic for Global Optimization over Continuous Spaces, Journal of Global Optimization, 1997, 11, 341 - 359.
 
 ## LICENSE
```

## Comparing `porgo-1.0.1.dist-info/RECORD` & `porgo-1.1.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 porgo/__init__.py,sha256=38xCrK8ms2668EMOzga_pryhdruIgnMdKXzskCKP3mg,225
 porgo/_typing.py,sha256=mGwg2-1CTe39GGslsJr4VTHcK0FQbECOh5Bx2JBwWgA,157
-porgo/_version.py,sha256=TJ5JaRCRguW7179mPLN9aTCOeZZJ6_tzBhnYU6SVlbY,57
-porgo/runtime.py,sha256=ZH2Yb365ikIkPO0uxhe4rgEjVZecj5naMa6bEkwDz84,4193
-porgo-1.0.1.dist-info/LICENSE,sha256=6tZMvmRANwvfuPHCTWM4gS9MHtQFReXNH_yqQFVRqlw,1089
-porgo-1.0.1.dist-info/METADATA,sha256=zj5EieBZ6jhjqNnS68IbIjnd6P7Ob0D26-RAbvOyja8,3285
-porgo-1.0.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-porgo-1.0.1.dist-info/top_level.txt,sha256=rE9a1sFwUTPF1rtbHkyRSdCEK2q_yytJfKybWP8tMRo,6
-porgo-1.0.1.dist-info/RECORD,,
+porgo/_version.py,sha256=r7egOSFd6l3bZ1wur-g3ZxxOMx989V7Ai7WBpMRTjak,57
+porgo/runtime.py,sha256=zdaYAwhzNqTxMXhnn0-1CzNcG71dg2vdFYAL5MtNLxg,4292
+porgo-1.1.0.dist-info/LICENSE,sha256=6tZMvmRANwvfuPHCTWM4gS9MHtQFReXNH_yqQFVRqlw,1089
+porgo-1.1.0.dist-info/METADATA,sha256=3Fq4V9pj-fX_jEuu9QIiaJFhextJXkZyfPfOe6-_Vo4,3400
+porgo-1.1.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+porgo-1.1.0.dist-info/top_level.txt,sha256=rE9a1sFwUTPF1rtbHkyRSdCEK2q_yytJfKybWP8tMRo,6
+porgo-1.1.0.dist-info/RECORD,,
```

