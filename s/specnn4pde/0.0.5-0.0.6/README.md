# Comparing `tmp/specnn4pde-0.0.5.tar.gz` & `tmp/specnn4pde-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specnn4pde-0.0.5.tar", last modified: Sun Apr  7 02:59:07 2024, max compression
+gzip compressed data, was "specnn4pde-0.0.6.tar", last modified: Tue May  7 05:53:38 2024, max compression
```

## Comparing `specnn4pde-0.0.5.tar` & `specnn4pde-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 02:59:07.195542 specnn4pde-0.0.5/
--rw-rw-rw-   0        0        0     1091 2024-04-03 06:49:12.000000 specnn4pde-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2716 2024-04-07 02:59:07.193467 specnn4pde-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1654 2024-04-05 03:16:54.000000 specnn4pde-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 02:59:07.195542 specnn4pde-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1709 2024-04-07 02:58:57.000000 specnn4pde-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 02:59:07.183115 specnn4pde-0.0.5/specnn4pde/
--rw-rw-rw-   0        0        0       37 2024-04-05 03:16:25.000000 specnn4pde-0.0.5/specnn4pde/__init__.py
--rw-rw-rw-   0        0        0     1755 2024-03-15 09:39:53.000000 specnn4pde-0.0.5/specnn4pde/linalg.py
--rw-rw-rw-   0        0        0     9192 2024-04-06 15:04:07.000000 specnn4pde-0.0.5/specnn4pde/nn.py
--rw-rw-rw-   0        0        0    12153 2024-04-07 02:55:20.000000 specnn4pde-0.0.5/specnn4pde/npde.py
--rw-rw-rw-   0        0        0    16238 2024-04-04 03:16:10.000000 specnn4pde-0.0.5/specnn4pde/spectral.py
--rw-rw-rw-   0        0        0     6621 2024-03-20 02:37:42.000000 specnn4pde-0.0.5/specnn4pde/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-07 02:59:07.193467 specnn4pde-0.0.5/specnn4pde.egg-info/
--rw-rw-rw-   0        0        0     2716 2024-04-07 02:59:07.000000 specnn4pde-0.0.5/specnn4pde.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-04-07 02:59:07.000000 specnn4pde-0.0.5/specnn4pde.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 02:59:07.000000 specnn4pde-0.0.5/specnn4pde.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-07 02:59:07.000000 specnn4pde-0.0.5/specnn4pde.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 02:59:07.000000 specnn4pde-0.0.5/specnn4pde.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 05:53:38.185854 specnn4pde-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2024-04-03 06:49:12.000000 specnn4pde-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3073 2024-05-07 05:53:38.185854 specnn4pde-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2011 2024-04-22 13:43:46.000000 specnn4pde-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 05:53:38.186856 specnn4pde-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1709 2024-05-07 05:53:09.000000 specnn4pde-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:53:38.170852 specnn4pde-0.0.6/specnn4pde/
+-rw-rw-rw-   0        0        0       37 2024-04-05 03:16:25.000000 specnn4pde-0.0.6/specnn4pde/__init__.py
+-rw-rw-rw-   0        0        0     1844 2024-04-12 02:29:21.000000 specnn4pde-0.0.6/specnn4pde/linalg.py
+-rw-rw-rw-   0        0        0     9192 2024-04-06 15:04:07.000000 specnn4pde-0.0.6/specnn4pde/nn.py
+-rw-rw-rw-   0        0        0    12447 2024-05-07 05:52:11.000000 specnn4pde-0.0.6/specnn4pde/npde.py
+-rw-rw-rw-   0        0        0    16373 2024-05-02 03:47:36.000000 specnn4pde-0.0.6/specnn4pde/spectral.py
+-rw-rw-rw-   0        0        0     7792 2024-04-25 14:36:20.000000 specnn4pde-0.0.6/specnn4pde/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 05:53:38.184853 specnn4pde-0.0.6/specnn4pde.egg-info/
+-rw-rw-rw-   0        0        0     3073 2024-05-07 05:53:38.000000 specnn4pde-0.0.6/specnn4pde.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-07 05:53:38.000000 specnn4pde-0.0.6/specnn4pde.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 05:53:38.000000 specnn4pde-0.0.6/specnn4pde.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-07 05:53:38.000000 specnn4pde-0.0.6/specnn4pde.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-07 05:53:38.000000 specnn4pde-0.0.6/specnn4pde.egg-info/top_level.txt
```

### Comparing `specnn4pde-0.0.5/LICENSE` & `specnn4pde-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `specnn4pde-0.0.5/PKG-INFO` & `specnn4pde-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specnn4pde
-Version: 0.0.5
+Version: 0.0.6
 Summary: Solving partial differential equations using spectral methods and neural networks.
 Home-page: https://github.com/mxweng/specnn4pde
 Author: MXWeng
 Author-email: 2431141461@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,27 +27,29 @@
 Requires-Dist: scipy
 Requires-Dist: sympy
 
 # SpecNN4PDE
 SpecNN4PDE is an under development Python library for solving partial differential equations using spectral methods and neural networks. It consists of the following modules:
 
 - `spectral`: Provides functions for working with spectral methods as described in the book [Spectral Methods: Algorithms, Analysis and Applications](https://link.springer.com/book/10.1007/978-3-540-71041-7) by Shen, Tang, and Wang.
+- `nn`: Contains classes for building neural networks, including [random feature method (RFM)](https://global-sci.org/intro/article_detail/jml/21029.html) neural networks, etc.
+- `sav`: The [Scalar auxiliary variable (SAV)](https://www.sciencedirect.com/science/article/pii/S002199911730774X) optimizer and its variants.
+- `npde`: Functions for solving partial differential equations, e.g., calculating the multivariate derivatives.
 - `linalg`: This module primarily focuses on numerical algebra methods.
 - `utils`: A collection of utility functions for system and package information retrieval, time measurement, etc.
-- `npde`: Functions for solving partial differential equations, e.g., calculating the multivariate derivatives.
 
 This project is still in the early stages of development, and the API is subject to change. The library is designed to be used in research and educational settings.
 
 ## Dependencies
 
-When you install this library using pip, most dependencies will be automatically handled. However, please note that the `npde` module requires PyTorch, which needs to be installed separately.
+When you install this library using pip, most dependencies will be automatically handled. However, please note that the `nn`, `sav`, and `npde` module requires PyTorch, which needs to be installed separately.
 
 You can install PyTorch by following the instructions on the [official PyTorch website](https://pytorch.org/get-started/locally/). Please ensure that you select the correct installation command based on your operating system, package manager, Python version, and the specifications of your CUDA toolkit if you are planning to use PyTorch with GPU support.
 
-If you are not planning to use the `npde` module, you do not need to install PyTorch.
+If you are not planning to use the `nn`, `sav`, and `npde` module, you do not need to install PyTorch.
 
 ## Installation
 
 To install this library, you can use pip:
 
 ```bash
 pip install specnn4pde
```

### Comparing `specnn4pde-0.0.5/README.md` & `specnn4pde-0.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # SpecNN4PDE
 SpecNN4PDE is an under development Python library for solving partial differential equations using spectral methods and neural networks. It consists of the following modules:
 
 - `spectral`: Provides functions for working with spectral methods as described in the book [Spectral Methods: Algorithms, Analysis and Applications](https://link.springer.com/book/10.1007/978-3-540-71041-7) by Shen, Tang, and Wang.
+- `nn`: Contains classes for building neural networks, including [random feature method (RFM)](https://global-sci.org/intro/article_detail/jml/21029.html) neural networks, etc.
+- `sav`: The [Scalar auxiliary variable (SAV)](https://www.sciencedirect.com/science/article/pii/S002199911730774X) optimizer and its variants.
+- `npde`: Functions for solving partial differential equations, e.g., calculating the multivariate derivatives.
 - `linalg`: This module primarily focuses on numerical algebra methods.
 - `utils`: A collection of utility functions for system and package information retrieval, time measurement, etc.
-- `npde`: Functions for solving partial differential equations, e.g., calculating the multivariate derivatives.
 
 This project is still in the early stages of development, and the API is subject to change. The library is designed to be used in research and educational settings.
 
 ## Dependencies
 
-When you install this library using pip, most dependencies will be automatically handled. However, please note that the `npde` module requires PyTorch, which needs to be installed separately.
+When you install this library using pip, most dependencies will be automatically handled. However, please note that the `nn`, `sav`, and `npde` module requires PyTorch, which needs to be installed separately.
 
 You can install PyTorch by following the instructions on the [official PyTorch website](https://pytorch.org/get-started/locally/). Please ensure that you select the correct installation command based on your operating system, package manager, Python version, and the specifications of your CUDA toolkit if you are planning to use PyTorch with GPU support.
 
-If you are not planning to use the `npde` module, you do not need to install PyTorch.
+If you are not planning to use the `nn`, `sav`, and `npde` module, you do not need to install PyTorch.
 
 ## Installation
 
 To install this library, you can use pip:
 
 ```bash
 pip install specnn4pde
```

### Comparing `specnn4pde-0.0.5/setup.py` & `specnn4pde-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.command import install_data
 from setuptools import setup, find_packages
 
 setup(
     name='specnn4pde',  # package name
-    version='0.0.5',  # version
+    version='0.0.6',  # version
     author='MXWeng',  # author name
     author_email='2431141461@qq.com',  # author email
     description='Solving partial differential equations using spectral methods and neural networks.',  # short description
     long_description=open('README.md').read(),  # long description, usually your README
     long_description_content_type='text/markdown',  # format of the long description, 'text/markdown' if it's Markdown
     url='https://github.com/mxweng/specnn4pde',  # project homepage
     packages=find_packages(),  # automatically discover all packages
```

### Comparing `specnn4pde-0.0.5/specnn4pde/linalg.py` & `specnn4pde-0.0.6/specnn4pde/linalg.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
            ]
 
 import numpy as np
 
 def ROU_cholesky(L, v, alpha=1, beta=1):
     """
     Perform a rank-one update of the Cholesky decomposition of a matrix.
+    The complexity of the rank-one update is O(n^2), where n is the size of the matrix.
 
     Parameters
     ----------
     L : ndarray
         The lower triangular Cholesky factor of the matrix A.
     alpha : float
         The scalar multiplier for the matrix. Must be non-negative.
```

### Comparing `specnn4pde-0.0.5/specnn4pde/nn.py` & `specnn4pde-0.0.6/specnn4pde/nn.py`

 * *Files identical despite different names*

### Comparing `specnn4pde-0.0.5/specnn4pde/npde.py` & `specnn4pde-0.0.6/specnn4pde/npde.py`

 * *Files 4% similar despite different names*

```diff
@@ -236,15 +236,16 @@
             [2.0000, 5.0000]])
     """
 
     Co = torch.meshgrid(*inputs, indexing=indexing)
     return torch.cat([c.reshape(-1,1) for c in Co], dim=1)
 
 
-def gen_collo(Domain = [], grids = [], temporal = False, corner = True, G = None):
+def gen_collo(Domain = [], grids = [], temporal = False, corner = True, G = None,
+              dtype = torch.float32, device = 'cpu'):
     """
     Generate the collocation points for the PDE problem on regular domain.
     If Domain and grids are provided, the uniform grids will be generated automatically as G.
     If Domain and grids are not provided, G should be provided.
 
     Parameters
     ----------
@@ -255,14 +256,18 @@
     temporal : bool, optional
         If the problem is temporal. The default is False.
     corner : bool, optional
         If the collocation points include the corner points. The default is True.
     G : list of tensor, optional
         The tensors in the list are the collocation points in each dimension.
         If Domain and grids are not provided, G should be provided.
+    dtype : torch.dtype, optional
+        The data type of the collocation points. The default is torch.float32.
+    device : str, optional
+        The device of the collocation points. The default is 'cpu'.
     
     Returns
     -------
     collo_rs : tensor
         The collocation points in the interior of the domain.
     collo_ic : tensor, optional
         If temporal is set as True. The collocation points on the initial condition.
@@ -296,15 +301,15 @@
         dim = len(Domain[0])
         if len(grids) != dim:
             if len(grids) == 1:
                 Warning("The number of grids is set as the same for all dimensions.")
                 grids = grids * dim
             else:
                 raise ValueError("The length of grids should be equal to the dimension of the domain.")
-        G = [torch.linspace(l, r, n) for l, r, n in zip(*(Domain + [grids]))]
+        G = [torch.linspace(l, r, n, dtype=dtype, device=device) for l, r, n in zip(*(Domain + [grids]))]
     dim = len(G)
     if temporal:
         G_rs = [G[0][1:]] + [G[i][1:-1] for i in range(1, dim)]
         G_ic = [G[0][0]] + G[1:]
         collo_rs = meshgrid_to_matrix(G_rs)
         collo_ic = meshgrid_to_matrix(G_ic)
         collo_bc = []
```

### Comparing `specnn4pde-0.0.5/specnn4pde/spectral.py` & `specnn4pde-0.0.6/specnn4pde/spectral.py`

 * *Files 3% similar despite different names*

```diff
@@ -357,31 +357,31 @@
     1. Spectral Method P280, P286
     """
 
     y, s = symbols('y s')
 
     if mapping == 'alg':
         map_expr = s * y / sqrt(1 - y**2)
-        diff_map_expr = diff(map_expr, y)
     elif mapping == 'log':
         map_expr = s * atanh(y)
-        diff_map_expr = diff(map_expr, y)
     elif mapping == 'exp':
         map_expr = sinh(s * y)
-        diff_map_expr = diff(map_expr, y)
     else:
         raise ValueError("Invalid mapping function. Please choose from 'alg', 'log' and 'exp'.")
-
-    map = lambdify((y, s), map_expr, "numpy")
+    
+    diff_map_expr = diff(map_expr, y)
+    Map = lambdify((y, s), map_expr, "numpy")
     diff_map = lambdify((y, s), diff_map_expr, "numpy")
 
     D, r, w = Jacobi_Gauss(alpha, beta, N)
     omega = (1 - r)**alpha * (1 + r)**beta
     diff_g = diff_map(r, sf)
-    D, r, w = D / diff_g[:, None], map(r, sf), w / omega * diff_g
+    # here we use the chain rule to compute the derivative of the mapped Jacobi-Gauss quadrature
+    # if the weight function is known, we can directly compute the derivative of the weight function (cf. P261 equ(7.93))
+    D, r, w = D / diff_g[:, None], Map(r, sf), w / omega * diff_g
     return D, r, w
 
 
 
 
 def glue1D(interval, Ncell, D, r, w, end_pts = False):
     """
```

### Comparing `specnn4pde-0.0.5/specnn4pde/utils.py` & `specnn4pde-0.0.6/specnn4pde/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-__all__ = ['pkg_system_info', 'func_timer', 'timer',
+__all__ = ['pkg_system_info', 'svg2pdf', 'func_timer', 'timer',
            ]
 
+import os
 import platform
 import psutil
 import pandas as pd
 from datetime import datetime
 from IPython.display import display, HTML
 import GPUtil
 import importlib
@@ -106,15 +107,41 @@
             architecture, cpu_info = get_cpu_info()
             system_info['CPU Version'] = f"{architecture} Family {cpu_info['CPU family']} Model {cpu_info['Model']} Stepping {cpu_info['Stepping']}, {cpu_info['Vendor ID']}"
 
         system_info_df = pd.DataFrame(list(system_info.items()), columns=['System Information', 'Details'])
         display(HTML(system_info_df.to_html(index=False)))
 
 
+def svg2pdf(directory, inkscape_path=None):
+    """
+    Convert all SVG files in a directory to PDF using Inkscape.
+
+    This function is only tested on Windows and it requires 
+    Inkscape to be installed on your system. 
+    You can download it from https://inkscape.org/release/ and install it.
+
+    Parameters:
+    ----------
+    directory (str): The directory that contains the SVG files.
+    inkscape_path (str, optional): The path to the Inkscape executable. 
+        If not provided, the function will use "inkscape" as the default value, 
+        assuming that Inkscape is in the system's PATH.
 
+    Example:
+    ----------
+    >>> convert_svg_to_pdf(r'D:/path/to/your/directory')
+    """
+    if inkscape_path is None:
+        inkscape_path = "inkscape"
+    for filename in os.listdir(directory):
+        if filename.endswith(".svg"):
+            svg_file = os.path.join(directory, filename)
+            pdf_file = os.path.join(directory, os.path.splitext(filename)[0] + ".pdf")
+            command = f'"{inkscape_path}" "{svg_file}" --export-filename="{pdf_file}"'
+            subprocess.run(command, shell=True)
 
 def func_timer(function):
     """
     This is a timer decorator. It calculates the execution time of the function.
     
     Args
     ----------
```

### Comparing `specnn4pde-0.0.5/specnn4pde.egg-info/PKG-INFO` & `specnn4pde-0.0.6/specnn4pde.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specnn4pde
-Version: 0.0.5
+Version: 0.0.6
 Summary: Solving partial differential equations using spectral methods and neural networks.
 Home-page: https://github.com/mxweng/specnn4pde
 Author: MXWeng
 Author-email: 2431141461@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,27 +27,29 @@
 Requires-Dist: scipy
 Requires-Dist: sympy
 
 # SpecNN4PDE
 SpecNN4PDE is an under development Python library for solving partial differential equations using spectral methods and neural networks. It consists of the following modules:
 
 - `spectral`: Provides functions for working with spectral methods as described in the book [Spectral Methods: Algorithms, Analysis and Applications](https://link.springer.com/book/10.1007/978-3-540-71041-7) by Shen, Tang, and Wang.
+- `nn`: Contains classes for building neural networks, including [random feature method (RFM)](https://global-sci.org/intro/article_detail/jml/21029.html) neural networks, etc.
+- `sav`: The [Scalar auxiliary variable (SAV)](https://www.sciencedirect.com/science/article/pii/S002199911730774X) optimizer and its variants.
+- `npde`: Functions for solving partial differential equations, e.g., calculating the multivariate derivatives.
 - `linalg`: This module primarily focuses on numerical algebra methods.
 - `utils`: A collection of utility functions for system and package information retrieval, time measurement, etc.
-- `npde`: Functions for solving partial differential equations, e.g., calculating the multivariate derivatives.
 
 This project is still in the early stages of development, and the API is subject to change. The library is designed to be used in research and educational settings.
 
 ## Dependencies
 
-When you install this library using pip, most dependencies will be automatically handled. However, please note that the `npde` module requires PyTorch, which needs to be installed separately.
+When you install this library using pip, most dependencies will be automatically handled. However, please note that the `nn`, `sav`, and `npde` module requires PyTorch, which needs to be installed separately.
 
 You can install PyTorch by following the instructions on the [official PyTorch website](https://pytorch.org/get-started/locally/). Please ensure that you select the correct installation command based on your operating system, package manager, Python version, and the specifications of your CUDA toolkit if you are planning to use PyTorch with GPU support.
 
-If you are not planning to use the `npde` module, you do not need to install PyTorch.
+If you are not planning to use the `nn`, `sav`, and `npde` module, you do not need to install PyTorch.
 
 ## Installation
 
 To install this library, you can use pip:
 
 ```bash
 pip install specnn4pde
```

