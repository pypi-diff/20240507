# Comparing `tmp/PyPyNum-1.8.1.tar.gz` & `tmp/PyPyNum-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPyNum-1.8.1.tar", last modified: Wed Apr 24 12:33:16 2024, max compression
+gzip compressed data, was "PyPyNum-1.8.2.tar", last modified: Tue May  7 13:38:35 2024, max compression
```

## Comparing `PyPyNum-1.8.1.tar` & `PyPyNum-1.8.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 12:33:16.688000 PyPyNum-1.8.1/
--rw-rw-rw-   0        0        0    84338 2024-04-24 12:33:16.686999 PyPyNum-1.8.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 12:33:16.577000 PyPyNum-1.8.1/PyPyNum.egg-info/
--rw-rw-rw-   0        0        0    84338 2024-04-24 12:33:16.000000 PyPyNum-1.8.1/PyPyNum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2024-04-24 12:33:16.000000 PyPyNum-1.8.1/PyPyNum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 12:33:16.000000 PyPyNum-1.8.1/PyPyNum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 12:33:16.000000 PyPyNum-1.8.1/PyPyNum.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 12:33:16.682000 PyPyNum-1.8.1/pypynum/
--rw-rw-rw-   0        0        0     6632 2024-03-15 05:10:12.000000 PyPyNum-1.8.1/pypynum/Array.py
--rw-rw-rw-   0        0        0     1401 2024-01-30 11:14:26.000000 PyPyNum-1.8.1/pypynum/FourierT.py
--rw-rw-rw-   0        0        0    13982 2024-01-19 00:54:43.000000 PyPyNum-1.8.1/pypynum/Geometry.py
--rw-rw-rw-   0        0        0    10131 2024-03-31 04:23:02.000000 PyPyNum-1.8.1/pypynum/Graph.py
--rw-rw-rw-   0        0        0     2944 2024-01-19 05:30:50.000000 PyPyNum-1.8.1/pypynum/Group.py
--rw-rw-rw-   0        0        0    11000 2024-01-22 06:51:59.000000 PyPyNum-1.8.1/pypynum/Logic.py
--rw-rw-rw-   0        0        0    18050 2024-04-24 11:35:12.000000 PyPyNum-1.8.1/pypynum/Matrix.py
--rw-rw-rw-   0        0        0     3275 2024-03-09 09:24:21.000000 PyPyNum-1.8.1/pypynum/NeuralN.py
--rw-rw-rw-   0        0        0    11623 2024-01-11 12:35:25.000000 PyPyNum-1.8.1/pypynum/PyPyNum.png
--rw-rw-rw-   0        0        0     8007 2024-01-25 08:45:23.000000 PyPyNum-1.8.1/pypynum/Quaternion.py
--rw-rw-rw-   0        0        0    42891 2024-04-24 12:12:47.000000 PyPyNum-1.8.1/pypynum/README.md
--rw-rw-rw-   0        0        0     2898 2024-01-28 23:31:30.000000 PyPyNum-1.8.1/pypynum/Symbolics.py
--rw-rw-rw-   0        0        0     3801 2024-03-15 05:10:12.000000 PyPyNum-1.8.1/pypynum/Tensor.py
--rw-rw-rw-   0        0        0     2827 2024-03-30 08:22:31.000000 PyPyNum-1.8.1/pypynum/Tree.py
--rw-rw-rw-   0        0        0     3552 2024-03-15 05:10:12.000000 PyPyNum-1.8.1/pypynum/Vector.py
--rw-rw-rw-   0        0        0     1843 2024-04-22 14:16:33.000000 PyPyNum-1.8.1/pypynum/__init__.py
--rw-rw-rw-   0        0        0     1001 2024-03-03 12:14:46.000000 PyPyNum-1.8.1/pypynum/chars.py
--rw-rw-rw-   0        0        0     1002 2024-01-12 04:51:16.000000 PyPyNum-1.8.1/pypynum/cipher.py
--rw-rw-rw-   0        0        0      843 2024-03-02 07:05:21.000000 PyPyNum-1.8.1/pypynum/constants.py
--rw-rw-rw-   0        0        0      713 2024-04-24 11:23:59.000000 PyPyNum-1.8.1/pypynum/equations.py
--rw-rw-rw-   0        0        0      173 2024-01-10 02:34:45.000000 PyPyNum-1.8.1/pypynum/errors.py
--rw-rw-rw-   0        0        0     3188 2024-01-20 05:47:09.000000 PyPyNum-1.8.1/pypynum/file.py
--rw-rw-rw-   0        0        0    26637 2024-04-21 23:30:31.000000 PyPyNum-1.8.1/pypynum/maths.py
--rw-rw-rw-   0        0        0     6028 2024-03-03 04:29:29.000000 PyPyNum-1.8.1/pypynum/numbers.py
--rw-rw-rw-   0        0        0     8463 2024-04-24 12:20:39.000000 PyPyNum-1.8.1/pypynum/plotting.py
--rw-rw-rw-   0        0        0     5998 2024-04-12 11:56:56.000000 PyPyNum-1.8.1/pypynum/polynomial.py
--rw-rw-rw-   0        0        0     2130 2024-01-24 05:42:10.000000 PyPyNum-1.8.1/pypynum/probability.py
--rw-rw-rw-   0        0        0     4610 2024-01-19 00:54:43.000000 PyPyNum-1.8.1/pypynum/random.py
--rw-rw-rw-   0        0        0     2118 2024-01-30 23:32:31.000000 PyPyNum-1.8.1/pypynum/regression.py
--rw-rw-rw-   0        0        0     7194 2024-03-18 12:46:51.000000 PyPyNum-1.8.1/pypynum/sequence.py
--rw-rw-rw-   0        0        0     8428 2024-01-24 05:43:19.000000 PyPyNum-1.8.1/pypynum/test.py
--rw-rw-rw-   0        0        0     2129 2024-02-27 12:58:01.000000 PyPyNum-1.8.1/pypynum/this.py
--rw-rw-rw-   0        0        0    12697 2024-04-01 12:52:02.000000 PyPyNum-1.8.1/pypynum/tools.py
--rw-rw-rw-   0        0        0      181 2024-01-18 23:57:19.000000 PyPyNum-1.8.1/pypynum/types.py
--rw-rw-rw-   0        0        0     9881 2024-03-16 12:49:15.000000 PyPyNum-1.8.1/pypynum/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-24 12:33:16.689000 PyPyNum-1.8.1/setup.cfg
--rw-rw-rw-   0        0        0    36724 2024-04-24 12:31:55.000000 PyPyNum-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 13:38:35.459000 PyPyNum-1.8.2/
+-rw-rw-rw-   0        0        0    85030 2024-05-07 13:38:35.454000 PyPyNum-1.8.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 13:38:35.213000 PyPyNum-1.8.2/PyPyNum.egg-info/
+-rw-rw-rw-   0        0        0    85030 2024-05-07 13:38:35.000000 PyPyNum-1.8.2/PyPyNum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-05-07 13:38:35.000000 PyPyNum-1.8.2/PyPyNum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 13:38:35.000000 PyPyNum-1.8.2/PyPyNum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 13:38:35.000000 PyPyNum-1.8.2/PyPyNum.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 13:38:35.447000 PyPyNum-1.8.2/pypynum/
+-rw-rw-rw-   0        0        0     6739 2024-05-04 06:17:31.000000 PyPyNum-1.8.2/pypynum/Array.py
+-rw-rw-rw-   0        0        0     1401 2024-01-30 11:14:26.000000 PyPyNum-1.8.2/pypynum/FourierT.py
+-rw-rw-rw-   0        0        0    13982 2024-01-19 00:54:43.000000 PyPyNum-1.8.2/pypynum/Geometry.py
+-rw-rw-rw-   0        0        0    10131 2024-03-31 04:23:02.000000 PyPyNum-1.8.2/pypynum/Graph.py
+-rw-rw-rw-   0        0        0     2944 2024-01-19 05:30:50.000000 PyPyNum-1.8.2/pypynum/Group.py
+-rw-rw-rw-   0        0        0    11000 2024-01-22 06:51:59.000000 PyPyNum-1.8.2/pypynum/Logic.py
+-rw-rw-rw-   0        0        0    18050 2024-04-24 11:35:12.000000 PyPyNum-1.8.2/pypynum/Matrix.py
+-rw-rw-rw-   0        0        0     3275 2024-03-09 09:24:21.000000 PyPyNum-1.8.2/pypynum/NeuralN.py
+-rw-rw-rw-   0        0        0    11623 2024-01-11 12:35:25.000000 PyPyNum-1.8.2/pypynum/PyPyNum.png
+-rw-rw-rw-   0        0        0     8017 2024-05-04 10:25:35.000000 PyPyNum-1.8.2/pypynum/Quaternion.py
+-rw-rw-rw-   0        0        0    43586 2024-05-07 13:31:15.000000 PyPyNum-1.8.2/pypynum/README.md
+-rw-rw-rw-   0        0        0     2898 2024-01-28 23:31:30.000000 PyPyNum-1.8.2/pypynum/Symbolics.py
+-rw-rw-rw-   0        0        0     3801 2024-03-15 05:10:12.000000 PyPyNum-1.8.2/pypynum/Tensor.py
+-rw-rw-rw-   0        0        0     2827 2024-03-30 08:22:31.000000 PyPyNum-1.8.2/pypynum/Tree.py
+-rw-rw-rw-   0        0        0     3526 2024-05-04 06:34:57.000000 PyPyNum-1.8.2/pypynum/Vector.py
+-rw-rw-rw-   0        0        0     1905 2024-05-04 08:31:56.000000 PyPyNum-1.8.2/pypynum/__init__.py
+-rw-rw-rw-   0        0        0     1001 2024-03-03 12:14:46.000000 PyPyNum-1.8.2/pypynum/chars.py
+-rw-rw-rw-   0        0        0     1002 2024-01-12 04:51:16.000000 PyPyNum-1.8.2/pypynum/cipher.py
+-rw-rw-rw-   0        0        0      843 2024-03-02 07:05:21.000000 PyPyNum-1.8.2/pypynum/constants.py
+-rw-rw-rw-   0        0        0      713 2024-04-24 11:23:59.000000 PyPyNum-1.8.2/pypynum/equations.py
+-rw-rw-rw-   0        0        0      173 2024-01-10 02:34:45.000000 PyPyNum-1.8.2/pypynum/errors.py
+-rw-rw-rw-   0        0        0     3188 2024-01-20 05:47:09.000000 PyPyNum-1.8.2/pypynum/file.py
+-rw-rw-rw-   0        0        0    26719 2024-05-05 12:19:48.000000 PyPyNum-1.8.2/pypynum/maths.py
+-rw-rw-rw-   0        0        0     6028 2024-03-03 04:29:29.000000 PyPyNum-1.8.2/pypynum/numbers.py
+-rw-rw-rw-   0        0        0     8463 2024-04-24 12:20:39.000000 PyPyNum-1.8.2/pypynum/plotting.py
+-rw-rw-rw-   0        0        0     5998 2024-04-12 11:56:56.000000 PyPyNum-1.8.2/pypynum/polynomial.py
+-rw-rw-rw-   0        0        0     2130 2024-01-24 05:42:10.000000 PyPyNum-1.8.2/pypynum/probability.py
+-rw-rw-rw-   0        0        0     4610 2024-01-19 00:54:43.000000 PyPyNum-1.8.2/pypynum/random.py
+-rw-rw-rw-   0        0        0     2118 2024-01-30 23:32:31.000000 PyPyNum-1.8.2/pypynum/regression.py
+-rw-rw-rw-   0        0        0     7194 2024-03-18 12:46:51.000000 PyPyNum-1.8.2/pypynum/sequence.py
+-rw-rw-rw-   0        0        0     8461 2024-05-07 05:24:21.000000 PyPyNum-1.8.2/pypynum/test.py
+-rw-rw-rw-   0        0        0     2162 2024-05-07 05:23:26.000000 PyPyNum-1.8.2/pypynum/this.py
+-rw-rw-rw-   0        0        0    12697 2024-04-01 12:52:02.000000 PyPyNum-1.8.2/pypynum/tools.py
+-rw-rw-rw-   0        0        0      181 2024-01-18 23:57:19.000000 PyPyNum-1.8.2/pypynum/types.py
+-rw-rw-rw-   0        0        0     9881 2024-03-16 12:49:15.000000 PyPyNum-1.8.2/pypynum/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 13:38:35.462000 PyPyNum-1.8.2/setup.cfg
+-rw-rw-rw-   0        0        0    36721 2024-05-07 12:39:34.000000 PyPyNum-1.8.2/setup.py
```

### Comparing `PyPyNum-1.8.1/PKG-INFO` & `PyPyNum-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: PyPyNum
-Version: 1.8.1
-Summary: A multifunctional mathematical calculation package written in pure Python programming language [Python>=3.5]
-Home-page: https://www.gitee.com/PythonSJL/PyPyNum
+Version: 1.8.2
+Summary: A multifunctional mathematical calculation package written in pure Python programming language [Python>=3.4]
+Home-page: https://github.com/PythonSJL/PyPyNum
 Author: Shen Jiayi
 Author-email: 2261748025@qq.com
 License: 
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -665,21 +665,21 @@
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <http://www.gnu.org/licenses/>.
         
 Keywords: math,数学,mathematics,数学计算,numerical,数值,computation,计算,scientific,科学,algebra,代数,calculus,微积分,statistics,统计,linear-algebra,线性代数,optimization,优化,numerical-analysis,数值分析,matrix,矩阵,vector,向量,tensor,张量,numerics,数值计算,library,库,tools,工具,utils,实用程序,algorithms,算法,software,软件,package,包,methods,方法,data-science,数据科学,machine-learning,机器学习,computational,计算的,operations,操作,functions,函数,processing,处理,programming,编程,simulation,仿真,visualization,可视化,physics,物理
-Requires-Python: >=3.5
+Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 
 ﻿# <font color = blue>PyPyNum</font>
 
 <font color = gree>A multifunctional mathematical calculation package written in pure Python programming language
-</font><font color = red>[Python>=3.5]</font>
+</font><font color = red>[Python>=3.4]</font>
 
 ```
  ________   ___    ___  ________   ___    ___  ________    ___  ___   _____ ______
 |\   __  \ |\  \  /  /||\   __  \ |\  \  /  /||\   ___  \ |\  \|\  \ |\   _ \  _   \
 \ \  \|\  \\ \  \/  / /\ \  \|\  \\ \  \/  / /\ \  \\ \  \\ \  \\\  \\ \  \\\__\ \  \
  \ \   ____\\ \    / /  \ \   ____\\ \    / /  \ \  \\ \  \\ \  \\\  \\ \  \\|__| \  \
   \ \  \___| \/  /  /    \ \  \___| \/  /  /    \ \  \\ \  \\ \  \\\  \\ \  \    \ \  \
@@ -688,28 +688,29 @@
           \|___|/                \|___|/
 ```
 
 [![Downloads](https://static.pepy.tech/badge/pypynum)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/month)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/week)](https://pepy.tech/project/pypynum)
 
-## Version -> 1.8.1 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum
+## Version -> 1.8.2 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum | GitHub -> https://github.com/PythonSJL/PyPyNum
 
 ![LOGO](PyPyNum.png)
 
 PyPI上无法显示logo，可以在Gitee中查看。
 
 The logo cannot be displayed on PyPI, it can be viewed in Gitee.
 
 ### 介绍
 
 #### Introduction
 
-+ DIY数学库，类似于numpy、scipy等，专为PyPy解释器制作
-+ DIY math library, similar to numpy, scipy, etc., specifically designed for PyPy interpreters
++ 多功能数学库，类似于numpy、scipy等，专为PyPy解释器制作，亦支持其他类型的Python解释器
++ Multi functional math library, similar to numpy, scipy, etc., designed specifically for PyPy interpreters and also
+  supports other types of Python interpreters
 + 不定期更新版本，增加更多实用功能
 + Update versions periodically to add more practical features
 + 如需联系，QQ 2261748025 （Py𝙿𝚢𝚝𝚑𝚘𝚗-水晶兰）
 + If you need to contact, QQ 2261748025 (Py𝙿𝚢𝚝𝚑𝚘𝚗-水晶兰)
 
 ### PyPyNum的Zen（预览）
 
@@ -737,34 +738,57 @@
 ### 与上一个版本相比新增功能
 
 #### New features compared to the previous version
 
 ```
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-eig函数修复了计算错误并改名为eigen
+已确认此库能够向下兼容Python 3.4版本
+以此支持IronPython解释器。
 
-The eig function fixed
-calculation errors and changed
-its name to eigen
+It has been confirmed that this
+library is backward compatible
+with Python version 3.4 to
+support the IronPython
+interpreter.
 
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-<<<以下结构中的省略号表示原有的部分>>>
+修改并优化了部分功能。
 
-<<<The ellipsis in the following structure represents the original part>>>
+Modified and optimized some
+features.
 
-PyPyNum
-    ★ Matrix [Matrix calculation]
-        FUNCTIONS
-            ...
-            rotate90(matrix: pypynum.Matrix.Matrix, times: int) -> pypynum.Matrix.Matrix
-            hessenberg(matrix: pypynum.Matrix.Matrix) -> tuple
-            eigen(matrix: pypynum.Matrix.Matrix) -> tuple
-            ...
+!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
+
+修改了fill函数，该函数将一维值序列填充
+到指定形状的数组中。如果未指定列表，则默
+认为从零开始递增的序列。此函数默认为循环
+填充，否则使用零填充来填充剩余位置。
+
+Modified the fill function,
+which fills a one-dimensional
+value sequence into an array of
+specified shapes. If no list is
+specified, it defaults to a
+sequence that increments from
+zero. This function defaults to
+loop padding, otherwise zero
+padding is used to fill the
+remaining positions.
+
+!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
+
+使用辛普森公式提高定积分的计算精度。
+
+Use Simpson's formula to improve
+the calculation accuracy of
+definite integrals.
+
+!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 ```
 
 ### 运行用时测试
 
 #### Run Time Test
 
 |                     矩阵用时测试<br>Matrix Time Test                     |                                                                            NumPy﻿+﻿CPython﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                             PyPyNum﻿+﻿PyPy﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                           Mpmath﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                           | 排名<br>Ranking |                                                                                                     SymPy﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                                                     | 排名<br>Ranking |
@@ -807,15 +831,15 @@
             num = typing.Union[int, float, complex]
             real = typing.Union[int, float]
     ★ Array [N-dimensional array]
         CLASSES
             Array
         FUNCTIONS
             array(data=None)
-            fill(shape, sequence=None)
+            fill(shape, sequence=None, repeat=True)
             function(_array, _function, args=None)
             get_shape(data)
             is_valid_array(_array, _shape)
             zeros(shape)
             zeros_like(_nested_list)
     ★ FourierT [Fourier transform and inverse Fourier transform]
         CLASSES
```

### Comparing `PyPyNum-1.8.1/PyPyNum.egg-info/PKG-INFO` & `PyPyNum-1.8.2/PyPyNum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: PyPyNum
-Version: 1.8.1
-Summary: A multifunctional mathematical calculation package written in pure Python programming language [Python>=3.5]
-Home-page: https://www.gitee.com/PythonSJL/PyPyNum
+Version: 1.8.2
+Summary: A multifunctional mathematical calculation package written in pure Python programming language [Python>=3.4]
+Home-page: https://github.com/PythonSJL/PyPyNum
 Author: Shen Jiayi
 Author-email: 2261748025@qq.com
 License: 
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -665,21 +665,21 @@
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <http://www.gnu.org/licenses/>.
         
 Keywords: math,数学,mathematics,数学计算,numerical,数值,computation,计算,scientific,科学,algebra,代数,calculus,微积分,statistics,统计,linear-algebra,线性代数,optimization,优化,numerical-analysis,数值分析,matrix,矩阵,vector,向量,tensor,张量,numerics,数值计算,library,库,tools,工具,utils,实用程序,algorithms,算法,software,软件,package,包,methods,方法,data-science,数据科学,machine-learning,机器学习,computational,计算的,operations,操作,functions,函数,processing,处理,programming,编程,simulation,仿真,visualization,可视化,physics,物理
-Requires-Python: >=3.5
+Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 
 ﻿# <font color = blue>PyPyNum</font>
 
 <font color = gree>A multifunctional mathematical calculation package written in pure Python programming language
-</font><font color = red>[Python>=3.5]</font>
+</font><font color = red>[Python>=3.4]</font>
 
 ```
  ________   ___    ___  ________   ___    ___  ________    ___  ___   _____ ______
 |\   __  \ |\  \  /  /||\   __  \ |\  \  /  /||\   ___  \ |\  \|\  \ |\   _ \  _   \
 \ \  \|\  \\ \  \/  / /\ \  \|\  \\ \  \/  / /\ \  \\ \  \\ \  \\\  \\ \  \\\__\ \  \
  \ \   ____\\ \    / /  \ \   ____\\ \    / /  \ \  \\ \  \\ \  \\\  \\ \  \\|__| \  \
   \ \  \___| \/  /  /    \ \  \___| \/  /  /    \ \  \\ \  \\ \  \\\  \\ \  \    \ \  \
@@ -688,28 +688,29 @@
           \|___|/                \|___|/
 ```
 
 [![Downloads](https://static.pepy.tech/badge/pypynum)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/month)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/week)](https://pepy.tech/project/pypynum)
 
-## Version -> 1.8.1 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum
+## Version -> 1.8.2 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum | GitHub -> https://github.com/PythonSJL/PyPyNum
 
 ![LOGO](PyPyNum.png)
 
 PyPI上无法显示logo，可以在Gitee中查看。
 
 The logo cannot be displayed on PyPI, it can be viewed in Gitee.
 
 ### 介绍
 
 #### Introduction
 
-+ DIY数学库，类似于numpy、scipy等，专为PyPy解释器制作
-+ DIY math library, similar to numpy, scipy, etc., specifically designed for PyPy interpreters
++ 多功能数学库，类似于numpy、scipy等，专为PyPy解释器制作，亦支持其他类型的Python解释器
++ Multi functional math library, similar to numpy, scipy, etc., designed specifically for PyPy interpreters and also
+  supports other types of Python interpreters
 + 不定期更新版本，增加更多实用功能
 + Update versions periodically to add more practical features
 + 如需联系，QQ 2261748025 （Py𝙿𝚢𝚝𝚑𝚘𝚗-水晶兰）
 + If you need to contact, QQ 2261748025 (Py𝙿𝚢𝚝𝚑𝚘𝚗-水晶兰)
 
 ### PyPyNum的Zen（预览）
 
@@ -737,34 +738,57 @@
 ### 与上一个版本相比新增功能
 
 #### New features compared to the previous version
 
 ```
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-eig函数修复了计算错误并改名为eigen
+已确认此库能够向下兼容Python 3.4版本
+以此支持IronPython解释器。
 
-The eig function fixed
-calculation errors and changed
-its name to eigen
+It has been confirmed that this
+library is backward compatible
+with Python version 3.4 to
+support the IronPython
+interpreter.
 
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-<<<以下结构中的省略号表示原有的部分>>>
+修改并优化了部分功能。
 
-<<<The ellipsis in the following structure represents the original part>>>
+Modified and optimized some
+features.
 
-PyPyNum
-    ★ Matrix [Matrix calculation]
-        FUNCTIONS
-            ...
-            rotate90(matrix: pypynum.Matrix.Matrix, times: int) -> pypynum.Matrix.Matrix
-            hessenberg(matrix: pypynum.Matrix.Matrix) -> tuple
-            eigen(matrix: pypynum.Matrix.Matrix) -> tuple
-            ...
+!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
+
+修改了fill函数，该函数将一维值序列填充
+到指定形状的数组中。如果未指定列表，则默
+认为从零开始递增的序列。此函数默认为循环
+填充，否则使用零填充来填充剩余位置。
+
+Modified the fill function,
+which fills a one-dimensional
+value sequence into an array of
+specified shapes. If no list is
+specified, it defaults to a
+sequence that increments from
+zero. This function defaults to
+loop padding, otherwise zero
+padding is used to fill the
+remaining positions.
+
+!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
+
+使用辛普森公式提高定积分的计算精度。
+
+Use Simpson's formula to improve
+the calculation accuracy of
+definite integrals.
+
+!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 ```
 
 ### 运行用时测试
 
 #### Run Time Test
 
 |                     矩阵用时测试<br>Matrix Time Test                     |                                                                            NumPy﻿+﻿CPython﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                             PyPyNum﻿+﻿PyPy﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                           Mpmath﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                           | 排名<br>Ranking |                                                                                                     SymPy﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                                                     | 排名<br>Ranking |
@@ -807,15 +831,15 @@
             num = typing.Union[int, float, complex]
             real = typing.Union[int, float]
     ★ Array [N-dimensional array]
         CLASSES
             Array
         FUNCTIONS
             array(data=None)
-            fill(shape, sequence=None)
+            fill(shape, sequence=None, repeat=True)
             function(_array, _function, args=None)
             get_shape(data)
             is_valid_array(_array, _shape)
             zeros(shape)
             zeros_like(_nested_list)
     ★ FourierT [Fourier transform and inverse Fourier transform]
         CLASSES
```

### Comparing `PyPyNum-1.8.1/PyPyNum.egg-info/SOURCES.txt` & `PyPyNum-1.8.2/PyPyNum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/Array.py` & `PyPyNum-1.8.2/pypynum/Array.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,27 +179,30 @@
         for item in _nested_list:
             _copy.append(zeros_like(item))
         return _copy
     else:
         return 0
 
 
-def fill(shape, sequence=None):
+def fill(shape, sequence=None, repeat=True):
     pointer = -1
     length = 1
     for item in shape:
         length *= item
     if sequence is None:
         sequence = list(range(length))
+    total = len(sequence)
 
     def inner(_shape):
         nonlocal pointer
         if len(_shape) == 0:
+            if pointer == total and not repeat:
+                return 0
             pointer += 1
-            return sequence[pointer % len(sequence)]
+            return sequence[pointer % total]
         else:
             _array = []
             for i in range(_shape[0]):
                 _row = inner(_shape[1:])
                 _array.append(_row)
             return _array
```

### Comparing `PyPyNum-1.8.1/pypynum/FourierT.py` & `PyPyNum-1.8.2/pypynum/FourierT.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/Geometry.py` & `PyPyNum-1.8.2/pypynum/Geometry.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/Graph.py` & `PyPyNum-1.8.2/pypynum/Graph.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/Group.py` & `PyPyNum-1.8.2/pypynum/Group.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/Logic.py` & `PyPyNum-1.8.2/pypynum/Logic.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/Matrix.py` & `PyPyNum-1.8.2/pypynum/Matrix.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/NeuralN.py` & `PyPyNum-1.8.2/pypynum/NeuralN.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/PyPyNum.png` & `PyPyNum-1.8.2/pypynum/PyPyNum.png`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/Quaternion.py` & `PyPyNum-1.8.2/pypynum/Quaternion.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,8 +199,8 @@
             t2 = 2.0 * (w * y - z * x)
             pitch = asin(t2)
             t3 = 2.0 * (w * z + x * y)
             t4 = 1.0 - 2.0 * (y * y + z * z)
             roll = atan2(t3, t4)
             return Euler(yaw, pitch, roll)
     else:
-        raise TypeError("Data can only be Euler or Quaternion")
+        raise TypeError("Data can only be Euler or Matrix or Quaternion")
```

### Comparing `PyPyNum-1.8.1/pypynum/README.md` & `PyPyNum-1.8.2/pypynum/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ﻿# <font color = blue>PyPyNum</font>
 
 <font color = gree>A multifunctional mathematical calculation package written in pure Python programming language
-</font><font color = red>[Python>=3.5]</font>
+</font><font color = red>[Python>=3.4]</font>
 
 ```
  ________   ___    ___  ________   ___    ___  ________    ___  ___   _____ ______
 |\   __  \ |\  \  /  /||\   __  \ |\  \  /  /||\   ___  \ |\  \|\  \ |\   _ \  _   \
 \ \  \|\  \\ \  \/  / /\ \  \|\  \\ \  \/  / /\ \  \\ \  \\ \  \\\  \\ \  \\\__\ \  \
  \ \   ____\\ \    / /  \ \   ____\\ \    / /  \ \  \\ \  \\ \  \\\  \\ \  \\|__| \  \
   \ \  \___| \/  /  /    \ \  \___| \/  /  /    \ \  \\ \  \\ \  \\\  \\ \  \    \ \  \
@@ -14,28 +14,29 @@
           \|___|/                \|___|/
 ```
 
 [![Downloads](https://static.pepy.tech/badge/pypynum)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/month)](https://pepy.tech/project/pypynum)
 [![Downloads](https://static.pepy.tech/badge/pypynum/week)](https://pepy.tech/project/pypynum)
 
-## Version -> 1.8.1 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum
+## Version -> 1.8.2 | PyPI -> https://pypi.org/project/PyPyNum/ | Gitee -> https://www.gitee.com/PythonSJL/PyPyNum | GitHub -> https://github.com/PythonSJL/PyPyNum
 
 ![LOGO](PyPyNum.png)
 
 PyPI上无法显示logo，可以在Gitee中查看。
 
 The logo cannot be displayed on PyPI, it can be viewed in Gitee.
 
 ### 介绍
 
 #### Introduction
 
-+ DIY数学库，类似于numpy、scipy等，专为PyPy解释器制作
-+ DIY math library, similar to numpy, scipy, etc., specifically designed for PyPy interpreters
++ 多功能数学库，类似于numpy、scipy等，专为PyPy解释器制作，亦支持其他类型的Python解释器
++ Multi functional math library, similar to numpy, scipy, etc., designed specifically for PyPy interpreters and also
+  supports other types of Python interpreters
 + 不定期更新版本，增加更多实用功能
 + Update versions periodically to add more practical features
 + 如需联系，QQ 2261748025 （Py𝙿𝚢𝚝𝚑𝚘𝚗-水晶兰）
 + If you need to contact, QQ 2261748025 (Py𝙿𝚢𝚝𝚑𝚘𝚗-水晶兰)
 
 ### PyPyNum的Zen（预览）
 
@@ -63,34 +64,57 @@
 ### 与上一个版本相比新增功能
 
 #### New features compared to the previous version
 
 ```
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-eig函数修复了计算错误并改名为eigen
+已确认此库能够向下兼容Python 3.4版本
+以此支持IronPython解释器。
 
-The eig function fixed
-calculation errors and changed
-its name to eigen
+It has been confirmed that this
+library is backward compatible
+with Python version 3.4 to
+support the IronPython
+interpreter.
 
 !=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 
-<<<以下结构中的省略号表示原有的部分>>>
+修改并优化了部分功能。
 
-<<<The ellipsis in the following structure represents the original part>>>
+Modified and optimized some
+features.
 
-PyPyNum
-    ★ Matrix [Matrix calculation]
-        FUNCTIONS
-            ...
-            rotate90(matrix: pypynum.Matrix.Matrix, times: int) -> pypynum.Matrix.Matrix
-            hessenberg(matrix: pypynum.Matrix.Matrix) -> tuple
-            eigen(matrix: pypynum.Matrix.Matrix) -> tuple
-            ...
+!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
+
+修改了fill函数，该函数将一维值序列填充
+到指定形状的数组中。如果未指定列表，则默
+认为从零开始递增的序列。此函数默认为循环
+填充，否则使用零填充来填充剩余位置。
+
+Modified the fill function,
+which fills a one-dimensional
+value sequence into an array of
+specified shapes. If no list is
+specified, it defaults to a
+sequence that increments from
+zero. This function defaults to
+loop padding, otherwise zero
+padding is used to fill the
+remaining positions.
+
+!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
+
+使用辛普森公式提高定积分的计算精度。
+
+Use Simpson's formula to improve
+the calculation accuracy of
+definite integrals.
+
+!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=!=
 ```
 
 ### 运行用时测试
 
 #### Run Time Test
 
 |                     矩阵用时测试<br>Matrix Time Test                     |                                                                            NumPy﻿+﻿CPython﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                             PyPyNum﻿+﻿PyPy﻿（﻿seconds﻿）                                                                             | 排名<br>Ranking |                                                                           Mpmath﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                           | 排名<br>Ranking |                                                                                                     SymPy﻿_﻿+﻿_﻿PyPy﻿_﻿（﻿_﻿seconds﻿_﻿）                                                                                                     | 排名<br>Ranking |
@@ -133,15 +157,15 @@
             num = typing.Union[int, float, complex]
             real = typing.Union[int, float]
     ★ Array [N-dimensional array]
         CLASSES
             Array
         FUNCTIONS
             array(data=None)
-            fill(shape, sequence=None)
+            fill(shape, sequence=None, repeat=True)
             function(_array, _function, args=None)
             get_shape(data)
             is_valid_array(_array, _shape)
             zeros(shape)
             zeros_like(_nested_list)
     ★ FourierT [Fourier transform and inverse Fourier transform]
         CLASSES
```

### Comparing `PyPyNum-1.8.1/pypynum/Symbolics.py` & `PyPyNum-1.8.2/pypynum/Symbolics.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/Tensor.py` & `PyPyNum-1.8.2/pypynum/Tensor.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/Tree.py` & `PyPyNum-1.8.2/pypynum/Tree.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/Vector.py` & `PyPyNum-1.8.2/pypynum/Vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             raise MatchError
         return sum([self.data[i] * other.data[i] for i in range(self.len)])
 
     def __abs__(self):
         return self.norm()
 
     def __pos__(self):
-        return Vector([abs(item) for item in self.data])
+        return Vector([item for item in self.data])
 
     def __neg__(self):
         return Vector([-item for item in self.data])
 
     def norm(self, p=2):
         if p == 0:
             return len([item for item in self.data if item != 0])
@@ -69,15 +69,15 @@
     def angles(self, axes=None):
         from math import acos
         if axes is None or axes == [] or axes == ():
             result = []
             for a in range(self.len):
                 axis = Vector([1 if p == a else 0 for p in range(self.len)])
                 result.append(acos(self @ axis / (self.norm() * axis.norm())))
-        elif isinstance(axes, int) and abs(axes) == axes:
+        elif int(abs(axes)) == axes:
             axis = Vector([1 if p == axes else 0 for p in range(self.len)])
             result = acos(self @ axis / (self.norm() * axis.norm()))
         elif isinstance(axes, (list, tuple)):
             result = []
             for a in axes:
                 axis = Vector([1 if p == a else 0 for p in range(self.len)])
                 result.append(acos(self @ axis / (self.norm() * axis.norm())))
```

### Comparing `PyPyNum-1.8.1/pypynum/__init__.py` & `PyPyNum-1.8.2/pypynum/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .file import read, write
 from .FourierT import *
 from .Geometry import *
 from .Graph import *
 from .Group import group
 from .Logic import *
 from .maths import *
-from .Matrix import mat, identity, rotate90, lu, qr, eigen, svd
+from .Matrix import mat, identity, rotate90, lu, qr, hessenberg, eigen, svd
 from .NeuralN import *
 from .numbers import *
 from .plotting import unary, binary, c_unary, color
 from .polynomial import *
 from .probability import *
 from .Quaternion import quat, euler
 from .random import *
@@ -35,11 +35,11 @@
 from .Tensor import ten, tensorproduct
 from .tools import *
 from .Tree import *
 from . import types
 from .utils import OrderedSet, InfIterator
 from .Vector import vec
 
-__version__ = "1.8.1"
+__version__ = "1.8.2"
 print("PyPyNum", "Version -> " + __version__, "PyPI -> https://pypi.org/project/PyPyNum/",
-      "Gitee -> https://www.gitee.com/PythonSJL/PyPyNum", sep=" | ")
+      "Gitee -> https://www.gitee.com/PythonSJL/PyPyNum", "GitHub -> https://github.com/PythonSJL/PyPyNum", sep=" | ")
 del math, arr, ite, num, real, geom, ContentError, RandomError, LogicError, InputError, FullError, Union
```

### Comparing `PyPyNum-1.8.1/pypynum/chars.py` & `PyPyNum-1.8.2/pypynum/chars.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/cipher.py` & `PyPyNum-1.8.2/pypynum/cipher.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/constants.py` & `PyPyNum-1.8.2/pypynum/constants.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/equations.py` & `PyPyNum-1.8.2/pypynum/equations.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/file.py` & `PyPyNum-1.8.2/pypynum/file.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/maths.py` & `PyPyNum-1.8.2/pypynum/maths.py`

 * *Files 2% similar despite different names*

```diff
@@ -746,56 +746,56 @@
     :param n: integer
     :param f: function
     :return:
     """
     return product(list(map(f, range(i, n + 1))))
 
 
-def derivative(f, x: real, h: real = 1e-7) -> float:
+def derivative(f, x: real, h: real = 1e-6) -> float:
     """
     introduction
     ==========
     Derivative calculation
 
     example
     ==========
     >>> derivative(lambda a: a ** 2, 2)
-    3.9999999956741306
+    4.000000000115023
     >>>
     :param f: function
     :param x: integer | float
     :param h: integer | float
     :return:
     """
+    h = h / 2
     return (f(x + h) - f(x - h)) / (2 * h)
 
 
-def definite_integral(f, x_start: real, x_end: real, n: int = 10000000) -> float:
+def definite_integral(f, x_start: real, x_end: real, n: int = 1000000) -> float:
     """
     introduction
     ==========
     Definite integral calculation
 
     example
     ==========
     >>> definite_integral(lambda a: a ** 2, 0, 2)
-    2.6666666666664036
+    2.666666666666616
     >>>
     :param f: function
     :param x_start: integer | float
     :param x_end: integer | float
     :param n: integer | float
     :return:
     """
     h = (x_end - x_start) / n
-    _sum = 0
-    for i in range(n):
-        x = x_start + i * h
-        _sum += f(x + h) + f(x)
-    return _sum * h / 2
+    s = f(x_start) + f(x_end)
+    s += sum(map(lambda i: 4 * f(x_start + i * h), range(1, n, 2)))
+    s += sum(map(lambda i: 2 * f(x_start + i * h), range(2, n - 1, 2)))
+    return s * h / 3
 
 
 def beta(p: real, q: real) -> real:
     """
     introduction
     ==========
     Beta function calculation \n
```

### Comparing `PyPyNum-1.8.1/pypynum/numbers.py` & `PyPyNum-1.8.2/pypynum/numbers.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/plotting.py` & `PyPyNum-1.8.2/pypynum/plotting.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/polynomial.py` & `PyPyNum-1.8.2/pypynum/polynomial.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/probability.py` & `PyPyNum-1.8.2/pypynum/probability.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/random.py` & `PyPyNum-1.8.2/pypynum/random.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/regression.py` & `PyPyNum-1.8.2/pypynum/regression.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/sequence.py` & `PyPyNum-1.8.2/pypynum/sequence.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/test.py` & `PyPyNum-1.8.2/pypynum/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,16 @@
 \033[m""")
 print(tools.classify([1, 2.3, 4 + 5j, "string", list, True, 3.14, False, tuple, tools]))
 print(tools.deduplicate(["Python", 6, "NumPy", int, "PyPyNum", 9, "pypynum", "NumPy", 6, True]))
 print(tools.frange(0, 3, 0.4))
 print(tools.linspace(0, 2.8, 8))
 
 for _ in list(globals().keys()):
-    del globals()[_]
+    if _ != "__builtins__":
+        del globals()[_]
 del _
 
 print("""\033[91m
 提示：
 
 测试已成功通过并结束。
```

### Comparing `PyPyNum-1.8.1/pypynum/this.py` & `PyPyNum-1.8.2/pypynum/this.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 The Zen of PyPyNum
 """
 
 Zen = "\x9a¤¢\xa0¢°¼§¢°éâñåâòõÖ°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°°\x9a\x9a±äù°õóñâòýõ°ã·äõü½äàõóþÿó°äåÿôþñäã°ñ°ãù°þ÷ùãõô°âñüåôÿÝ\x9a¾÷þùãùýÿâà°õò°äø÷ùý°äù°¼ôâñçâÿöäø÷ùñâäã°ãù°þÿùäñäþõýõüàýù°õøä°öÙ\x9a¾äù°âõôùãþÿóõâ°¼ôþõøõâàýÿó°ÿä°÷þù÷þõüüñøó°ãù°þÿùäñäþõýõüàýù°õøä°öÙ\x9a¾÷þùøãåâ°ÿä°âÿùâõàåã°ãù°÷þùäùñç°ãõýùäõýÿã°¼âõæõçÿØ\x9a¾þÿùäñþùäãñâóÿâà°þñøä°âõääõò°ãù°éüäàýÿâà°÷þùäóÑ\x9a¾øóñÿâààñ°ãåÿùæòÿ½õþÿ°éüþÿ°õøä°¼éüüñõôù½õþÿ°õò°äãåý°õâõøÄ\x9a¾õäñüåóõàã°ÿä°õ÷âå°õøä°äãùãõâ°¼ããõþõå÷ñæ°öÿ°õóþõãõâà°õøä°þÙ\x9a¾ôõäåý°éüäùóùüàèõ°ããõüþÅ\x9a¾ôõóþõüùã°äÿþ°¼þõûÿàã°õò°äãåý°ãâÿââÕ\x9a¾éäùâåà°âõæÿ°ãøàýåùâä°þõäöÿ°éäùüñóùäóñâÀ\x9a¾ãýâÿþ°õøä°õôùââõæÿ°äÿþ°ôüåÿøã°ãõãñó°üñùóõàÃ\x9a¾äþåÿýñâñà°ãù°éäùüùòñôñõÂ\x9a¾ãõþÿ°ôõäñÿüò°âõæÿ°ãþùç°õôÿó°õãâñàÃ\x9a¾ãõùøóâñâõùø°ôõäãõþ°ãäñõò°õâåäóåâäã°äñüÖ\x9a¾ôõäñóùüàýÿóâõæÿ°þñøä°âõääõò°ãù°ôõäñóùäãùøàÿÃ\x9a¾þÿùäåüÿæþÿó°âõæÿ°ôõââõöõâà°ãù°ããõþôâñçâÿöäø÷ùñâäÃ\x9a¾éäùâåóãòÿ°ãàýåâä°éäùâñüÓ\x9a¾éûþåüó°ÿä°âÿùâõàåã°ãù°äþñ÷õüÕ\x9a\x9a¾þÿøäéÀ°þù°éüõâåà°þõääùâç°õ÷ñûóñà°øäñý°ñ°ãù°ãùøÄ\x9a\x9aùéñùÚ°þõøÃ°éò°¼ýåÞéÀéÀ°öÿ°þõÊ°õøÄ°°°°\x9a"
 print("".join([chr(ord(_) ^ 144) for _ in Zen[::-1]]))
 for _ in list(globals().keys()):
-    del globals()[_]
+    if _ != "__builtins__":
+        del globals()[_]
 del _
```

### Comparing `PyPyNum-1.8.1/pypynum/tools.py` & `PyPyNum-1.8.2/pypynum/tools.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/pypynum/utils.py` & `PyPyNum-1.8.2/pypynum/utils.py`

 * *Files identical despite different names*

### Comparing `PyPyNum-1.8.1/setup.py` & `PyPyNum-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,22 +676,22 @@
 if any, to sign a "copyright disclaimer" for the program, if necessary.
 For more information on this, and how to apply and follow the GNU AGPL, see
 <http://www.gnu.org/licenses/>.
 """
 
 setup(
     name="PyPyNum",
-    version="1.8.1",
+    version="1.8.2",
     packages=find_packages(),
-    url="https://www.gitee.com/PythonSJL/PyPyNum",
+    url="https://github.com/PythonSJL/PyPyNum",
     license=LICENSE,
     author="Shen Jiayi",
     author_email="2261748025@qq.com",
     description="""
-    A multifunctional mathematical calculation package written in pure Python programming language [Python>=3.5]
+    A multifunctional mathematical calculation package written in pure Python programming language [Python>=3.4]
     """,
-    python_requires=">=3.5",
+    python_requires=">=3.4",
     package_data={"pypynum": ["*"]},
     long_description=md,
     long_description_content_type="text/markdown",
     keywords=keywords
 )
```

