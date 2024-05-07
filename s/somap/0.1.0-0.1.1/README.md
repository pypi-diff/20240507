# Comparing `tmp/somap-0.1.0.tar.gz` & `tmp/somap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somap-0.1.0.tar", last modified: Thu Nov 23 22:23:04 2023, max compression
+gzip compressed data, was "somap-0.1.1.tar", last modified: Tue May  7 20:01:21 2024, max compression
```

## Comparing `somap-0.1.0.tar` & `somap-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-11-23 22:22:52.557231 somap-0.1.0/LICENSE
--rw-r--r--   0        0        0     2725 2023-11-23 22:22:52.557231 somap-0.1.0/README.md
--rw-r--r--   0        0        0     1366 2023-11-23 22:23:04.329293 somap-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1452 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/__init__.py
--rw-r--r--   0        0        0      454 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/config.py
--rw-r--r--   0        0        0     7376 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/core.py
--rw-r--r--   0        0        0      161 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/datasets/__init__.py
--rw-r--r--   0        0        0      254 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/datasets/base.py
--rw-r--r--   0        0        0     1152 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/datasets/mnist.py
--rw-r--r--   0        0        0     1328 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/datasets/utils.py
--rw-r--r--   0        0        0     2958 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/distance.py
--rw-r--r--   0        0        0     4002 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/grid.py
--rw-r--r--   0        0        0     1673 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/learning_rate.py
--rw-r--r--   0        0        0     2653 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/metrics.py
--rw-r--r--   0        0        0     3819 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/neighborhood.py
--rw-r--r--   0        0        0     1135 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/plot.py
--rw-r--r--   0        0        0     1396 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/plot_backends/__init__.py
--rw-r--r--   0        0        0     7081 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/plot_backends/altair.py
--rw-r--r--   0        0        0     2186 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/plot_backends/array2image.py
--rw-r--r--   0        0        0      898 2023-11-23 22:22:52.585231 somap-0.1.0/src/somap/plot_backends/base.py
--rw-r--r--   0        0        0   628032 2023-11-23 22:22:52.589231 somap-0.1.0/src/somap/plot_backends/resources/Carlito-Regular.ttf
--rw-r--r--   0        0        0      771 2023-11-23 22:22:52.589231 somap-0.1.0/src/somap/plot_backends/utils.py
--rw-r--r--   0        0        0      844 2023-11-23 22:22:52.589231 somap-0.1.0/src/somap/serialisation.py
--rw-r--r--   0        0        0     2986 2023-11-23 22:22:52.589231 somap-0.1.0/src/somap/som.py
--rw-r--r--   0        0        0       20 2023-11-23 22:22:52.589231 somap-0.1.0/src/somap/types.py
--rw-r--r--   0        0        0     1740 2023-11-23 22:22:52.589231 somap-0.1.0/src/somap/update.py
--rw-r--r--   0        0        0     2003 2023-11-23 22:22:52.589231 somap-0.1.0/src/somap/utils.py
--rw-r--r--   0        0        0     1831 2023-11-23 22:22:52.589231 somap-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1329 2023-11-23 22:22:52.589231 somap-0.1.0/tests/test_core.py
--rw-r--r--   0        0        0     2085 2023-11-23 22:22:52.589231 somap-0.1.0/tests/test_som.py
--rw-r--r--   0        0        0     3925 1970-01-01 00:00:00.000000 somap-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-07 20:01:10.189234 somap-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4435 2024-05-07 20:01:10.189234 somap-0.1.1/README.md
+-rw-r--r--   0        0        0     1396 2024-05-07 20:01:21.857276 somap-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1488 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/__init__.py
+-rw-r--r--   0        0        0      454 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/config.py
+-rw-r--r--   0        0        0     7376 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/core.py
+-rw-r--r--   0        0        0      161 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/datasets/__init__.py
+-rw-r--r--   0        0        0      254 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/datasets/base.py
+-rw-r--r--   0        0        0     1152 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/datasets/mnist.py
+-rw-r--r--   0        0        0     1328 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/datasets/utils.py
+-rw-r--r--   0        0        0     2958 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/distance.py
+-rw-r--r--   0        0        0     4002 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/grid.py
+-rw-r--r--   0        0        0     1673 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/learning_rate.py
+-rw-r--r--   0        0        0     4537 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/neighborhood.py
+-rw-r--r--   0        0        0     1135 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/plot.py
+-rw-r--r--   0        0        0     1396 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/plot_backends/__init__.py
+-rw-r--r--   0        0        0     7081 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/plot_backends/altair.py
+-rw-r--r--   0        0        0     2186 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/plot_backends/array2image.py
+-rw-r--r--   0        0        0      898 2024-05-07 20:01:10.221234 somap-0.1.1/src/somap/plot_backends/base.py
+-rw-r--r--   0        0        0   628032 2024-05-07 20:01:10.225234 somap-0.1.1/src/somap/plot_backends/resources/Carlito-Regular.ttf
+-rw-r--r--   0        0        0      771 2024-05-07 20:01:10.225234 somap-0.1.1/src/somap/plot_backends/utils.py
+-rw-r--r--   0        0        0      844 2024-05-07 20:01:10.225234 somap-0.1.1/src/somap/serialisation.py
+-rw-r--r--   0        0        0     2986 2024-05-07 20:01:10.225234 somap-0.1.1/src/somap/som.py
+-rw-r--r--   0        0        0     1776 2024-05-07 20:01:10.225234 somap-0.1.1/src/somap/update.py
+-rw-r--r--   0        0        0     2003 2024-05-07 20:01:10.225234 somap-0.1.1/src/somap/utils.py
+-rw-r--r--   0        0        0     1831 2024-05-07 20:01:10.225234 somap-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1329 2024-05-07 20:01:10.225234 somap-0.1.1/tests/test_core.py
+-rw-r--r--   0        0        0     2085 2024-05-07 20:01:10.225234 somap-0.1.1/tests/test_som.py
+-rw-r--r--   0        0        0     5690 1970-01-01 00:00:00.000000 somap-0.1.1/PKG-INFO
```

### Comparing `somap-0.1.0/LICENSE` & `somap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/README.md` & `somap-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -7,24 +7,24 @@
     &nbsp;&nbsp;&nbsp;&nbsp;
     <img src="docs/som_on_mnist_square.png">
 </p>
 
 # Why a new SOM library?
 
 There are already a few open-source libraries for Self-Organizing Maps in python, of which [MiniSom](https://github.com/JustGlowing/minisom) and [SOMPY](https://github.com/sevamoo/SOMPY) seem to be the most popular. I developped ***Somap*** to overcome what I believe to be two shortcomings of existing libraries for my research on bio-inspired AI: 
-- Ability to easily customize the SOM algorithm (e.g. distance, neighborhood, learning rate and update functions).
-- Capacity to vectorize the computations over many SOMs (e.g. for distributed learning over 2D maps of SOMs).
 
-Thanks to [JAX](https://github.com/google/jax)'s `jit` and `vmap` magic functions, it turned out that performance was also significantly better compared to other frameworks. More precisely, it relies indirectly on JAX via the [Equinox](https://github.com/patrick-kidger/equinox) library that offers an easy-to-use PyTorch-like syntax.
+* Ability to easily customize the SOM algorithm (e.g. distance, neighborhood, learning rate and update functions).
+* Capacity to vectorize the computations over many SOMs (e.g. for distributed learning over 2D maps of SOMs).
+
+Thanks to [JAX](https://github.com/google/jax)'s `jit` and `vmap` functions, it turned out that performance was also significantly better compared to other frameworks. Under the hood, it relies indirectly on JAX via the [Equinox](https://github.com/patrick-kidger/equinox) library that offers an easy-to-use PyTorch-like syntax.
 
 # Installation
 
 Requires Python 3.10+ and a working installation of JAX 0.4.20+. You can follow [these instructions](https://github.com/google/jax#installation) to install JAX with the relevant hardware acceleration support.
-
-Then:
+I am currently working on different ways to extend the basic SOM algorithm:
 
 ```bash
 pip install somap
 ```
 
 # Quick example
 
@@ -51,25 +51,60 @@
 smp.plot(model)
 
 # Retrieve the errors from all steps
 quantization_errors = aux["metrics"]["quantization_error"]
 topographic_errors = aux["metrics"]["topographic_error"]
 ```
 
+You can also define your custom SOM:
+```python
+import somap as smp
+from jaxtyping import Array, Float
+
+class MyCustomSomParams(smp.AbstractSomParams):
+    sigma: float | Float[Array, "..."]
+    alpha: float | Float[Array, "..."]
+
+class MyCustomSom(smp.AbstractSom):
+
+    @staticmethod
+    def generate_algo(p: MyCustomSomParams) -> smp.SomAlgo:
+        return smp.SomAlgo(
+            f_dist=smp.EuclidianDist(),
+            f_nbh=smp.GaussianNbh(sigma=p.sigma),
+            f_lr=smp.ConstantLr(alpha=p.alpha),
+            f_update=smp.SomUpdate(),
+        )
+```
+
+If you need custom distance, neighborhood, learning rate and update functions for your SOM, you can define them by inheriting from `smp.AbstractDist`, `smp.AbstractNbh`, `smp.AbstractLr` and `smp.AbstractUpdate`. See the library source code for how to do it.
+
+
 # Documentation
 
-* [Documentation website](https://mthiboust.github.io/somap/)
-* [Examples from notebooks](notebooks/)
+See: [https://mthiboust.github.io/somap/](https://mthiboust.github.io/somap/)
+
+
+# Next steps
+
+I am currently working on different ways to extend the basic SOM algorithm:
+
+* **Inputs**: In addition to classic bottom-up driving inputs, a SOM could also receive lateral contextual or top-down modulatory inputs.
+* **Weighted inputs**: Each data point from inputs can be weighted so that fuzzy data is weighted less for the winner selection.
+* **Dynamics**: When receiving continuous inputs in time, past activations can influence the computation of the next step.
+* **Supervised and self-supervised learning**: Top-down inputs and next inputs in time can act as teaching signal for supervised and self-supervised learning.
+* **Multi-agent system**: Each SOM is an agent of a mutli-agent system where thousands of SOMs interact with each other.
+
+Some of these features will land on an other library that depends on ***Somap***.
 
 # Citation
 
 If you found this library to be useful in academic work, then please cite:
 ```
 @misc{thiboust2023somap,
   title={Somap: a flexible, fast and scalable python library for Self-Organizing Maps.},
   author={Matthieu Thiboust},
   year={2023},
   url={https://github.com/mthiboust/somap/},
 }
 ```
 
-
```

### Comparing `somap-0.1.0/pyproject.toml` & `somap-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "somap"
-version = "0.1.0"
+version = "0.1.1"
 description = "Self-Organizing Maps in python"
 authors = [
     { name = "Matthieu Thiboust", email = "14574229+mthiboust@users.noreply.github.com" },
 ]
 dependencies = [
-    "jax==0.4.20",
+    "jax>=0.4.20",
     "equinox>=0.11.1",
     "jaxtyping>=0.2.23",
     "beartype>=0.16.4",
     "datasets>=2.14.6",
     "matplotlib>=3.8.0",
     "altair>=5.1.2",
     "vl-convert-python>=1.0.0",
@@ -37,14 +37,15 @@
     "pytest>=7.4.3",
     "ruff>=0.1.5",
 ]
 docs = [
     "mkdocs-material>=9.4.11",
     "mknotebooks>=0.8.0",
     "mkdocstrings[crystal,python]>=0.24.0",
+    "pytkdocs-tweaks>=0.0.7",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `somap-0.1.0/src/somap/__init__.py` & `somap-0.1.1/src/somap/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Classic imports
 from . import datasets
 from .core import AbstractSom, AbstractSomParams, make_step, make_steps, SomAlgo
 from .distance import EuclidianDist, wdist_l2
 from .grid import distance_map
 from .learning_rate import AbstractLr, ConstantLr, DsomLr, KsomLr
-from .neighborhood import AbstractNbh, DsomNbh, GaussianNbh, KsomNbh
+from .neighborhood import AbstractNbh, DsomNbh, GaussianNbh, KsomNbh, MexicanHatNbh
 from .plot import plot, save_plot
 from .plot_backends import set_plot_backend
 from .serialisation import load, save
 from .som import (
     Dsom,
     DsomParams,
     Ksom,
@@ -45,14 +45,15 @@
     "ConstantLr",
     "DsomLr",
     "KsomLr",
     "AbstractNbh",
     "DsomNbh",
     "GaussianNbh",
     "KsomNbh",
+    "MexicanHatNbh",
     "plot",
     "save_plot",
     "set_plot_backend",
     "load",
     "save",
     "Dsom",
     "DsomParams",
```

### Comparing `somap-0.1.0/src/somap/core.py` & `somap-0.1.1/src/somap/core.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/datasets/mnist.py` & `somap-0.1.1/src/somap/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/datasets/utils.py` & `somap-0.1.1/src/somap/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/distance.py` & `somap-0.1.1/src/somap/distance.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/grid.py` & `somap-0.1.1/src/somap/grid.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/learning_rate.py` & `somap-0.1.1/src/somap/learning_rate.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/neighborhood.py` & `somap-0.1.1/src/somap/neighborhood.py`

 * *Files 10% similar despite different names*

```diff
@@ -110,7 +110,29 @@
 
         Returns:
             The neighborhood distance, as calculated in the article.
         """
         return jnp.exp(
             -(distance_map**2) / (self.plasticity**2 * quantization_error**2)
         )
+
+
+class MexicanHatNbh(AbstractNbh):
+    """Mexican Hat neighborhood function."""
+
+    sigma: float | Float[Array, "..."] = 0.1
+
+    def __call__(self, distance_map: Float[Array, "x y"], _, __) -> Float[Array, "x y"]:
+        """Computes the Mexican Hat neighboring value of each grid element.
+
+        Args:
+            self:
+                self.sigma: Scale factor for the spread of the neighborhood.
+            distance_map: Distance of each element from the winner element.
+            _: Not used
+            __: Not used
+
+        Returns:
+            The Mexican Hat neighborhood distance.
+        """
+        r2_norm = distance_map**2 / self.sigma**2
+        return (1 - 0.5 * r2_norm) * jnp.exp(-r2_norm / 2)
```

### Comparing `somap-0.1.0/src/somap/plot.py` & `somap-0.1.1/src/somap/plot.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/plot_backends/__init__.py` & `somap-0.1.1/src/somap/plot_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/plot_backends/altair.py` & `somap-0.1.1/src/somap/plot_backends/altair.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/plot_backends/array2image.py` & `somap-0.1.1/src/somap/plot_backends/array2image.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/plot_backends/base.py` & `somap-0.1.1/src/somap/plot_backends/base.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/plot_backends/resources/Carlito-Regular.ttf` & `somap-0.1.1/src/somap/plot_backends/resources/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/plot_backends/utils.py` & `somap-0.1.1/src/somap/plot_backends/utils.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/serialisation.py` & `somap-0.1.1/src/somap/serialisation.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/som.py` & `somap-0.1.1/src/somap/som.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/src/somap/update.py` & `somap-0.1.1/src/somap/update.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,16 @@
         self,
         lr: Float[Array, "..."],
         nbh: Float[Array, "..."],
         input_bu: Float[Array, "..."],
         w_bu: Float[Array, "..."],
     ) -> Float[Array, "..."]:
         """Updates the prototype weights."""
-        return w_bu + (lr * nbh)[:, :, jnp.newaxis] * (input_bu - w_bu)
+        out = w_bu + (lr * nbh)[:, :, jnp.newaxis] * (input_bu - w_bu)
+        return jnp.clip(out, 0, 1.0)
 
 
 @experimental_warning
 class CyclicSomUpdate(AbstractUpdate):
     """Cyclic update functions."""
 
     def __call__(self, lr, nbh, input_bu, w_bu):
```

### Comparing `somap-0.1.0/src/somap/utils.py` & `somap-0.1.1/src/somap/utils.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/tests/__init__.py` & `somap-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/tests/test_core.py` & `somap-0.1.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/tests/test_som.py` & `somap-0.1.1/tests/test_som.py`

 * *Files identical despite different names*

### Comparing `somap-0.1.0/PKG-INFO` & `somap-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: somap
-Version: 0.1.0
+Version: 0.1.1
 Summary: Self-Organizing Maps in python
 Author-Email: Matthieu Thiboust <14574229+mthiboust@users.noreply.github.com>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/mthiboust/somap
 Project-URL: Documentation, https://mthiboust.github.io/somap/
 Requires-Python: <3.12,>=3.10
-Requires-Dist: jax==0.4.20
+Requires-Dist: jax>=0.4.20
 Requires-Dist: equinox>=0.11.1
 Requires-Dist: jaxtyping>=0.2.23
 Requires-Dist: beartype>=0.16.4
 Requires-Dist: datasets>=2.14.6
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: altair>=5.1.2
 Requires-Dist: vl-convert-python>=1.0.0
@@ -21,14 +21,15 @@
 Requires-Dist: ipywidgets>=8.1.1; extra == "notebook"
 Requires-Dist: python-dotenv>=1.0.0; extra == "notebook"
 Requires-Dist: pytest>=7.4.3; extra == "dev"
 Requires-Dist: ruff>=0.1.5; extra == "dev"
 Requires-Dist: mkdocs-material>=9.4.11; extra == "docs"
 Requires-Dist: mknotebooks>=0.8.0; extra == "docs"
 Requires-Dist: mkdocstrings[crystal,python]>=0.24.0; extra == "docs"
+Requires-Dist: pytkdocs-tweaks>=0.0.7; extra == "docs"
 Provides-Extra: notebook
 Provides-Extra: dev
 Provides-Extra: docs
 Description-Content-Type: text/markdown
 
 # Somap
 
@@ -39,24 +40,24 @@
     &nbsp;&nbsp;&nbsp;&nbsp;
     <img src="docs/som_on_mnist_square.png">
 </p>
 
 # Why a new SOM library?
 
 There are already a few open-source libraries for Self-Organizing Maps in python, of which [MiniSom](https://github.com/JustGlowing/minisom) and [SOMPY](https://github.com/sevamoo/SOMPY) seem to be the most popular. I developped ***Somap*** to overcome what I believe to be two shortcomings of existing libraries for my research on bio-inspired AI: 
-- Ability to easily customize the SOM algorithm (e.g. distance, neighborhood, learning rate and update functions).
-- Capacity to vectorize the computations over many SOMs (e.g. for distributed learning over 2D maps of SOMs).
 
-Thanks to [JAX](https://github.com/google/jax)'s `jit` and `vmap` magic functions, it turned out that performance was also significantly better compared to other frameworks. More precisely, it relies indirectly on JAX via the [Equinox](https://github.com/patrick-kidger/equinox) library that offers an easy-to-use PyTorch-like syntax.
+* Ability to easily customize the SOM algorithm (e.g. distance, neighborhood, learning rate and update functions).
+* Capacity to vectorize the computations over many SOMs (e.g. for distributed learning over 2D maps of SOMs).
+
+Thanks to [JAX](https://github.com/google/jax)'s `jit` and `vmap` functions, it turned out that performance was also significantly better compared to other frameworks. Under the hood, it relies indirectly on JAX via the [Equinox](https://github.com/patrick-kidger/equinox) library that offers an easy-to-use PyTorch-like syntax.
 
 # Installation
 
 Requires Python 3.10+ and a working installation of JAX 0.4.20+. You can follow [these instructions](https://github.com/google/jax#installation) to install JAX with the relevant hardware acceleration support.
-
-Then:
+I am currently working on different ways to extend the basic SOM algorithm:
 
 ```bash
 pip install somap
 ```
 
 # Quick example
 
@@ -83,25 +84,60 @@
 smp.plot(model)
 
 # Retrieve the errors from all steps
 quantization_errors = aux["metrics"]["quantization_error"]
 topographic_errors = aux["metrics"]["topographic_error"]
 ```
 
+You can also define your custom SOM:
+```python
+import somap as smp
+from jaxtyping import Array, Float
+
+class MyCustomSomParams(smp.AbstractSomParams):
+    sigma: float | Float[Array, "..."]
+    alpha: float | Float[Array, "..."]
+
+class MyCustomSom(smp.AbstractSom):
+
+    @staticmethod
+    def generate_algo(p: MyCustomSomParams) -> smp.SomAlgo:
+        return smp.SomAlgo(
+            f_dist=smp.EuclidianDist(),
+            f_nbh=smp.GaussianNbh(sigma=p.sigma),
+            f_lr=smp.ConstantLr(alpha=p.alpha),
+            f_update=smp.SomUpdate(),
+        )
+```
+
+If you need custom distance, neighborhood, learning rate and update functions for your SOM, you can define them by inheriting from `smp.AbstractDist`, `smp.AbstractNbh`, `smp.AbstractLr` and `smp.AbstractUpdate`. See the library source code for how to do it.
+
+
 # Documentation
 
-* [Documentation website](https://mthiboust.github.io/somap/)
-* [Examples from notebooks](notebooks/)
+See: [https://mthiboust.github.io/somap/](https://mthiboust.github.io/somap/)
+
+
+# Next steps
+
+I am currently working on different ways to extend the basic SOM algorithm:
+
+* **Inputs**: In addition to classic bottom-up driving inputs, a SOM could also receive lateral contextual or top-down modulatory inputs.
+* **Weighted inputs**: Each data point from inputs can be weighted so that fuzzy data is weighted less for the winner selection.
+* **Dynamics**: When receiving continuous inputs in time, past activations can influence the computation of the next step.
+* **Supervised and self-supervised learning**: Top-down inputs and next inputs in time can act as teaching signal for supervised and self-supervised learning.
+* **Multi-agent system**: Each SOM is an agent of a mutli-agent system where thousands of SOMs interact with each other.
+
+Some of these features will land on an other library that depends on ***Somap***.
 
 # Citation
 
 If you found this library to be useful in academic work, then please cite:
 ```
 @misc{thiboust2023somap,
   title={Somap: a flexible, fast and scalable python library for Self-Organizing Maps.},
   author={Matthieu Thiboust},
   year={2023},
   url={https://github.com/mthiboust/somap/},
 }
 ```
 
-
```

