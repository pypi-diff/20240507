# Comparing `tmp/speakleash-0.3.4.tar.gz` & `tmp/speakleash-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakleash-0.3.4.tar", last modified: Sun Oct 15 20:19:23 2023, max compression
+gzip compressed data, was "speakleash-0.3.5.tar", last modified: Sun May  5 22:16:40 2024, max compression
```

## Comparing `speakleash-0.3.4.tar` & `speakleash-0.3.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-10-15 20:19:23.507026 speakleash-0.3.4/
--rw-rw-rw-   0        0        0     1082 2023-09-14 13:15:39.000000 speakleash-0.3.4/LICENSE
--rw-rw-rw-   0        0        0     4016 2023-10-15 20:19:23.506428 speakleash-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     3509 2023-09-27 11:44:24.000000 speakleash-0.3.4/README.md
--rw-rw-rw-   0        0        0       42 2023-10-15 20:19:23.507026 speakleash-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-10-15 20:10:07.000000 speakleash-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-15 20:19:23.420143 speakleash-0.3.4/speakleash/
--rw-rw-rw-   0        0        0      526 2023-09-14 13:15:39.000000 speakleash-0.3.4/speakleash/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-15 20:19:23.461408 speakleash-0.3.4/speakleash/category_manager/
--rw-rw-rw-   0        0        0      183 2023-09-14 13:15:39.000000 speakleash-0.3.4/speakleash/category_manager/__init__.py
--rw-rw-rw-   0        0        0     6769 2023-09-14 13:15:39.000000 speakleash-0.3.4/speakleash/category_manager/category_manager.py
--rw-rw-rw-   0        0        0      314 2023-09-14 13:15:39.000000 speakleash-0.3.4/speakleash/config.json
--rw-rw-rw-   0        0        0      930 2023-09-14 13:15:39.000000 speakleash-0.3.4/speakleash/config_loader.py
--rw-rw-rw-   0        0        0     1869 2023-09-14 13:15:39.000000 speakleash-0.3.4/speakleash/contrib.py
-drwxrwxrwx   0        0        0        0 2023-10-15 20:19:23.469748 speakleash-0.3.4/speakleash/core/
--rw-rw-rw-   0        0        0      151 2023-09-14 13:15:39.000000 speakleash-0.3.4/speakleash/core/__init__.py
--rw-rw-rw-   0        0        0     3320 2023-10-15 18:58:16.000000 speakleash-0.3.4/speakleash/core/core.py
-drwxrwxrwx   0        0        0        0 2023-10-15 20:19:23.487392 speakleash-0.3.4/speakleash/dataset/
--rw-rw-rw-   0        0        0      167 2023-09-14 13:15:39.000000 speakleash-0.3.4/speakleash/dataset/__init__.py
--rw-rw-rw-   0        0        0    12869 2023-09-14 13:15:39.000000 speakleash-0.3.4/speakleash/dataset/dataset.py
-drwxrwxrwx   0        0        0        0 2023-10-15 20:19:23.504503 speakleash-0.3.4/speakleash/downloader/
--rw-rw-rw-   0        0        0      210 2023-09-14 13:15:39.000000 speakleash-0.3.4/speakleash/downloader/__init__.py
--rw-rw-rw-   0        0        0     4560 2023-09-14 13:15:39.000000 speakleash-0.3.4/speakleash/downloader/structure_downloader.py
-drwxrwxrwx   0        0        0        0 2023-10-15 20:19:23.446267 speakleash-0.3.4/speakleash.egg-info/
--rw-rw-rw-   0        0        0     4016 2023-10-15 20:19:23.000000 speakleash-0.3.4/speakleash.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      572 2023-10-15 20:19:23.000000 speakleash-0.3.4/speakleash.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-15 20:19:23.000000 speakleash-0.3.4/speakleash.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-10-15 20:19:23.000000 speakleash-0.3.4/speakleash.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-10-15 20:19:23.000000 speakleash-0.3.4/speakleash.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.274949 speakleash-0.3.5/
+-rw-rw-rw-   0        0        0     1082 2024-05-05 21:15:03.000000 speakleash-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0     3461 2024-05-05 22:16:40.272849 speakleash-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2983 2024-05-05 21:15:03.000000 speakleash-0.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 22:16:40.274949 speakleash-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      669 2024-05-05 21:15:03.000000 speakleash-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.191643 speakleash-0.3.5/speakleash/
+-rw-rw-rw-   0        0        0      573 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.223173 speakleash-0.3.5/speakleash/category_manager/
+-rw-rw-rw-   0        0        0      183 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/category_manager/__init__.py
+-rw-rw-rw-   0        0        0     6769 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/category_manager/category_manager.py
+-rw-rw-rw-   0        0        0      298 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/config.json
+-rw-rw-rw-   0        0        0      930 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/config_loader.py
+-rw-rw-rw-   0        0        0     1869 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/contrib.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.237879 speakleash-0.3.5/speakleash/core/
+-rw-rw-rw-   0        0        0      151 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/core/__init__.py
+-rw-rw-rw-   0        0        0     3924 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/core/core.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.255653 speakleash-0.3.5/speakleash/dataset/
+-rw-rw-rw-   0        0        0      167 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/dataset/__init__.py
+-rw-rw-rw-   0        0        0    12921 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/dataset/dataset.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.270841 speakleash-0.3.5/speakleash/downloader/
+-rw-rw-rw-   0        0        0      210 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/downloader/__init__.py
+-rw-rw-rw-   0        0        0     4560 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/downloader/structure_downloader.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.271848 speakleash-0.3.5/speakleash.egg-info/
+-rw-rw-rw-   0        0        0     3461 2024-05-05 22:16:40.000000 speakleash-0.3.5/speakleash.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2024-05-05 22:16:40.000000 speakleash-0.3.5/speakleash.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 22:16:40.000000 speakleash-0.3.5/speakleash.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-05 22:16:40.000000 speakleash-0.3.5/speakleash.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-05 22:16:40.000000 speakleash-0.3.5/speakleash.egg-info/top_level.txt
```

### Comparing `speakleash-0.3.4/LICENSE` & `speakleash-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `speakleash-0.3.4/README.md` & `speakleash-0.3.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 <h1 align="center">
 <img src="https://raw.githubusercontent.com/speakleash/speakleash/main/branding/logo/speakleash_logo.png" width="300">
 </h1><br>
 
 <p align="center">
-    <a href="https://pypi.org/project/speakleash">
-        <img src="https://badge.fury.io/py/speakleash.svg">
-    </a>
-    <a href="https://speakleash.org/">
-        <img src="https://img.shields.io/badge/organisation-Speakleash-orange">
-    </a>
-    <a href="https://pypi.org/project/speakleash">
-        <img src="https://img.shields.io/badge/python-_>=_3.6-blue">
-    </a>
-    <a href="https://speakleash.org/dashboard/">
-        <img src="https://img.shields.io/badge/dynamic/json?url=https://cutt.ly/ywcfnFY7&query=datasetsGB&suffix=%20GB&label=datasets&color=brightgreen">
-    </a>
-    <a href="https://speakleash.org/spolecznosc-i-kontakt/">
-        <img src="https://img.shields.io/discord/1043112910278381619?logo=discord&label=discord&color=%23603FEF">
-    </a>
+    <a href="https://pypi.org/project/speakleash"><img src="https://badge.fury.io/py/speakleash.svg"></a>
+    <a href="https://speakleash.org/"><img src="https://img.shields.io/badge/organisation-Speakleash-orange"></a>
+    <a href="https://pypi.org/project/speakleash"><img src="https://img.shields.io/badge/python-_>=_3.6-blue"></a>
+    <a href="https://speakleash.org/dashboard/"><img src="https://img.shields.io/badge/dynamic/json?url=https://cutt.ly/ywcfnFY7&query=datasetsGB&suffix=%20GB&label=datasets&color=brightgreen"></a>
+    <a href="https://speakleash.org/spolecznosc-i-kontakt/"><img src="https://img.shields.io/discord/1043112910278381619?logo=discord&label=discord&color=%23603FEF"></a>
 </p>
 
+### UPDATE 05.05.2024: 
+Due to the changes related with the hosting, it is recommended to update the version of the package to the newest one, using command:
+```python
+pip install --upgrade speakleash
+```
+
 [SpeakLeash](href="https://pypi.org/project/speakleash) is a lightweight library providing datasets for the Polish language
 and tools to make them useful.
 
 - **Website:** https://speakleash.org/
 - **Datasets:** https://speakleash.org/dashboard/
 - **Source code:** https://github.com/speakleash/speakleash
 - **Data in action:** https://github.com/speakleash/speakleash-examples
@@ -46,18 +42,16 @@
 
 base_dir = os.path.join(os.path.dirname(__file__))
 replicate_to = os.path.join(base_dir, "datasets")
 
 sl = Speakleash(replicate_to)
 
 for d in sl.datasets:
-    print(d.name)
-    for doc in d.data:
-        size_mb = round(d.characters/1024/1024)
-        print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format(d.name, size_mb, d.characters, d.documents))
+    size_mb = round(d.characters/1024/1024)
+    print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format(d.name, size_mb, d.characters, d.documents))
 ```
 
 You can use individual properties (e.g.:***characters***, ***documents***), but you can display the entire manifest
 ```python
 sl = Speakleash(replicate_to)
 print(sl.get("plwiki").manifest)
 ```
@@ -93,29 +87,7 @@
 * length
 * sentences
 * words
 * verbs
 * nouns
 * symbols
 * punctuations
-
-
-## Supported languages
-
-On June 9, 2023, Croatia joined our projects. If you want to use Croatian language datasets just add lang parameter when creating Speakleash object.
-
-```python
-from speakleash import Speakleash
-import os
-
-base_dir = os.path.join(os.path.dirname(__file__))
-replicate_to = os.path.join(base_dir, "datasets")
-
-sl = Speakleash(replicate_to, "hr")
-
-for d in sl.datasets:
-    print(d.name)
-    for doc in d.data:
-        size_mb = round(d.characters/1024/1024)
-        print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format(d.name, size_mb, d.characters, d.documents))
-
-```
```

#### html2text {}

```diff
@@ -3,40 +3,34 @@
 
     _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_s_p_e_a_k_l_e_a_s_h_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
  _o_r_g_a_n_i_s_a_t_i_o_n_-_S_p_e_a_k_l_e_a_s_h_-_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-___>_=___3_._6_-
      _b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_d_y_n_a_m_i_c_/_j_s_o_n_?_u_r_l_=_h_t_t_p_s_:_/_/_c_u_t_t_._l_y_/
 _y_w_c_f_n_F_Y_7_&_q_u_e_r_y_=_d_a_t_a_s_e_t_s_G_B_&_s_u_f_f_i_x_=_%_2_0_G_B_&_l_a_b_e_l_=_d_a_t_a_s_e_t_s_&_c_o_l_o_r_=_b_r_i_g_h_t_g_r_e_e_n_]_[_h_t_t_p_s_:
                            _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
         _1_0_4_3_1_1_2_9_1_0_2_7_8_3_8_1_6_1_9_?_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_=_d_i_s_c_o_r_d_&_c_o_l_o_r_=_%_2_3_6_0_3_F_E_F_]
-[SpeakLeash](href="https://pypi.org/project/speakleash) is a lightweight
-library providing datasets for the Polish language and tools to make them
-useful. - **Website:** https://speakleash.org/ - **Datasets:** https://
-speakleash.org/dashboard/ - **Source code:** https://github.com/speakleash/
-speakleash - **Data in action:** https://github.com/speakleash/speakleash-
-examples - **Bug reports:** https://github.com/speakleash/speakleash/issues ##
-Installation Speakleash package can be installed from PyPi and has to be
-installed in a virtual environment: ```python pip install speakleash ``` ##
-Basic Usage If you just want to see the details of the datasets ```python from
-speakleash import Speakleash import os base_dir = os.path.join(os.path.dirname
-(__file__)) replicate_to = os.path.join(base_dir, "datasets") sl = Speakleash
-(replicate_to) for d in sl.datasets: print(d.name) for doc in d.data: size_mb =
-round(d.characters/1024/1024) print("Dataset: {0}, size: {1} MB, characters:
-{2}, documents: {3}".format(d.name, size_mb, d.characters, d.documents)) ```
-You can use individual properties (e.g.:***characters***, ***documents***), but
-you can display the entire manifest ```python sl = Speakleash(replicate_to)
-print(sl.get("plwiki").manifest) ``` If you chose one of them (***.get(name of
-dataset)***) then you will get a lot of text data ;-) ```python from speakleash
-import Speakleash import os base_dir = os.path.join(os.path.dirname(__file__))
-replicate_to = os.path.join(base_dir, "datasets") sl = Speakleash(replicate_to)
-wiki = sl.get("plwiki").data for doc in wiki: print(doc[:40]) ``` If you also
-need meta data then use the ***ext_data*** property ```python ds = sl.get
-("plwiki").ext_data for doc in ds: print(doc) txt, meta = doc print(meta.get
-("title")) print(txt) ``` Popular meta data: * title * length * sentences *
-words * verbs * nouns * symbols * punctuations ## Supported languages On June
-9, 2023, Croatia joined our projects. If you want to use Croatian language
-datasets just add lang parameter when creating Speakleash object. ```python
-from speakleash import Speakleash import os base_dir = os.path.join
+### UPDATE 05.05.2024: Due to the changes related with the hosting, it is
+recommended to update the version of the package to the newest one, using
+command: ```python pip install --upgrade speakleash ``` [SpeakLeash]
+(href="https://pypi.org/project/speakleash) is a lightweight library providing
+datasets for the Polish language and tools to make them useful. - **Website:**
+https://speakleash.org/ - **Datasets:** https://speakleash.org/dashboard/ -
+**Source code:** https://github.com/speakleash/speakleash - **Data in action:**
+https://github.com/speakleash/speakleash-examples - **Bug reports:** https://
+github.com/speakleash/speakleash/issues ## Installation Speakleash package can
+be installed from PyPi and has to be installed in a virtual environment:
+```python pip install speakleash ``` ## Basic Usage If you just want to see the
+details of the datasets ```python from speakleash import Speakleash import os
+base_dir = os.path.join(os.path.dirname(__file__)) replicate_to = os.path.join
+(base_dir, "datasets") sl = Speakleash(replicate_to) for d in sl.datasets:
+size_mb = round(d.characters/1024/1024) print("Dataset: {0}, size: {1} MB,
+characters: {2}, documents: {3}".format(d.name, size_mb, d.characters,
+d.documents)) ``` You can use individual properties (e.g.:***characters***,
+***documents***), but you can display the entire manifest ```python sl =
+Speakleash(replicate_to) print(sl.get("plwiki").manifest) ``` If you chose one
+of them (***.get(name of dataset)***) then you will get a lot of text data ;-
+) ```python from speakleash import Speakleash import os base_dir = os.path.join
 (os.path.dirname(__file__)) replicate_to = os.path.join(base_dir, "datasets")
-sl = Speakleash(replicate_to, "hr") for d in sl.datasets: print(d.name) for doc
-in d.data: size_mb = round(d.characters/1024/1024) print("Dataset: {0}, size:
-{1} MB, characters: {2}, documents: {3}".format(d.name, size_mb, d.characters,
-d.documents)) ```
+sl = Speakleash(replicate_to) wiki = sl.get("plwiki").data for doc in wiki:
+print(doc[:40]) ``` If you also need meta data then use the ***ext_data***
+property ```python ds = sl.get("plwiki").ext_data for doc in ds: print(doc)
+txt, meta = doc print(meta.get("title")) print(txt) ``` Popular meta data: *
+title * length * sentences * words * verbs * nouns * symbols * punctuations
```

### Comparing `speakleash-0.3.4/setup.py` & `speakleash-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="speakleash",
-    version="0.3.4",
+    version="0.3.5",
     author="SpeakLeash Team",
     author_email="team@speakleash.org",
     description="SpeakLeash agnostic dataset for Polish",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/speakleash/speakleash",
     packages=find_packages(),
```

### Comparing `speakleash-0.3.4/speakleash/__init__.py` & `speakleash-0.3.5/speakleash/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,8 +5,9 @@
 
 Modules:
 - core: Provides the Speakleash class for managing and accessing datasets.
 - category_manager: Provides the CategoryManager class for managing categories in Speakleash.
 - dataset: Provides the SpeakleashDataset class for handling datasets in Speakleash.
 - structure_downloader: Provides the StructureDownloader class for downloading dataset structures in Speakleash.
 """
-from .core import Speakleash
+from .core import Speakleash
+from .category_manager import CategoryManager
```

### Comparing `speakleash-0.3.4/speakleash/category_manager/category_manager.py` & `speakleash-0.3.5/speakleash/category_manager/category_manager.py`

 * *Files identical despite different names*

### Comparing `speakleash-0.3.4/speakleash/config_loader.py` & `speakleash-0.3.5/speakleash/config_loader.py`

 * *Files identical despite different names*

### Comparing `speakleash-0.3.4/speakleash/contrib.py` & `speakleash-0.3.5/speakleash/contrib.py`

 * *Files identical despite different names*

### Comparing `speakleash-0.3.4/speakleash/dataset/dataset.py` & `speakleash-0.3.5/speakleash/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 - lm_dataformat: Provides a reader for the data format.
 - requests: Allows sending HTTP requests.
 - tqdm: Instantly makes loops show a smart progress meter.
 - typing: Provides the Dict, Tuple, List and Union types for type hinting.
 - speakleash.downloader: Provides the StructureDownloader class for downloading dataset structures.
 """
 import os
-from typing import Dict, Tuple, List, Union, Any
+from typing import Any, Dict, Generator, List, Optional, Tuple
 
 from lm_dataformat import Reader
 import requests
 from tqdm import tqdm
 
 from speakleash.downloader import StructureDownloader
 
@@ -56,15 +56,15 @@
 
         :param file_name: The name of the file to download.
         :return: True if download is successful, False otherwise.
         """
         url = f"{self.url}{self.name}.jsonl.zst"
         file_path = os.path.join(self.replicate_dir, file_name)
         response = requests.get(url, stream=True)
-        total_size_in_bytes = int(response.headers.get('content-length', 0))
+        total_size_in_bytes = int(response.headers.get('Content-Length', 0))
 
         with open(file_path, 'wb') as file:
             progress_bar = self.display_progress_bar(response, file, total_size_in_bytes)
 
         return self._download_complete(total_size_in_bytes, progress_bar.n)
 
     @staticmethod
@@ -327,33 +327,33 @@
 
         :return: A list of samples from the dataset.
         """
         sample_url = f"{self.url}{self.name}.sample"
         return StructureDownloader(self.replicate_dir).get_structure(sample_url, False) or []
 
     @property
-    def ext_data(self) -> Union[None, List[str]]:
+    def ext_data(self) -> Optional[Generator[str, None, None]]:
         """
         Extracts extended data from the dataset file.
 
-        :return: A list containing the streamed data with metadata, or None if the file check fails.
+        :return: A generator containing the streamed data with metadata, or None if the file check fails.
         """
         file_valid, file_path_json_zst = self.check_file()
 
         if not file_valid:
             return None
 
         return Reader(file_path_json_zst).stream_data(get_meta=True)
 
     @property
-    def data(self) -> Union[None, List[str]]:
+    def data(self) -> Optional[Generator[str, None, None]]:
         """
         Extracts data from the dataset file.
 
-        :return: A list containing the streamed data, or None if the file check fails.
+        :return: A generator containing the streamed data, or None if the file check fails.
         """
         file_valid, file_path_json_zst = self.check_file()
 
         if not file_valid:
             return None
 
         return Reader(file_path_json_zst).stream_data()
```

### Comparing `speakleash-0.3.4/speakleash/downloader/structure_downloader.py` & `speakleash-0.3.5/speakleash/downloader/structure_downloader.py`

 * *Files identical despite different names*

### Comparing `speakleash-0.3.4/speakleash.egg-info/SOURCES.txt` & `speakleash-0.3.5/speakleash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

