# Comparing `tmp/contextplus-0.1.0.tar.gz` & `tmp/contextplus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contextplus-0.1.0.tar", max compression
+gzip compressed data, was "contextplus-0.1.1.tar", max compression
```

## Comparing `contextplus-0.1.0.tar` & `contextplus-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1000 2024-05-07 12:31:18.092581 contextplus-0.1.0/README.md
--rw-r--r--   0        0        0       36 2024-05-07 12:31:18.092581 contextplus-0.1.0/contextplus/__init__.py
--rw-r--r--   0        0        0     3369 2024-05-07 12:31:18.092581 contextplus-0.1.0/contextplus/main.py
--rw-r--r--   0        0        0     3913 2024-05-07 12:31:18.092581 contextplus-0.1.0/contextplus/model.py
--rw-r--r--   0        0        0     4090 2024-05-07 12:31:18.092581 contextplus-0.1.0/contextplus/wiki.py
--rw-r--r--   0        0        0      334 2024-05-07 12:31:18.096581 contextplus-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 contextplus-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1737 2024-05-07 14:02:33.979872 contextplus-0.1.1/README.md
+-rw-r--r--   0        0        0       36 2024-05-07 14:02:33.979872 contextplus-0.1.1/contextplus/__init__.py
+-rw-r--r--   0        0        0     3369 2024-05-07 14:02:33.979872 contextplus-0.1.1/contextplus/main.py
+-rw-r--r--   0        0        0     3913 2024-05-07 14:02:33.979872 contextplus-0.1.1/contextplus/model.py
+-rw-r--r--   0        0        0     4090 2024-05-07 14:02:33.979872 contextplus-0.1.1/contextplus/wiki.py
+-rw-r--r--   0        0        0      705 2024-05-07 14:02:38.315871 contextplus-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 contextplus-0.1.1/PKG-INFO
```

### Comparing `contextplus-0.1.0/contextplus/main.py` & `contextplus-0.1.1/contextplus/main.py`

 * *Files identical despite different names*

### Comparing `contextplus-0.1.0/contextplus/model.py` & `contextplus-0.1.1/contextplus/model.py`

 * *Files identical despite different names*

### Comparing `contextplus-0.1.0/contextplus/wiki.py` & `contextplus-0.1.1/contextplus/wiki.py`

 * *Files identical despite different names*

### Comparing `contextplus-0.1.0/PKG-INFO` & `contextplus-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,10 @@
-Metadata-Version: 2.1
-Name: contextplus
-Version: 0.1.0
-Summary: 
-Author: Florian Wunderlich
-Requires-Python: >=3.11,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: sentence-transformers (>=2.7.0,<3.0.0)
-Requires-Dist: transformers (>=4.40.2,<5.0.0)
-Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
-Description-Content-Type: text/markdown
-
 <br />
 <p align="center">
-<a><img src="image/contextplus-circle.png" alt="ContextPlus" width="128" height="128" title="FawnRescue"></a>
+<a><img src="https://raw.githubusercontent.com/Multi-Agent-LLMs/context-plus/main/image/contextplus-circle.png" alt="ContextPlus" width="128" height="128" title="FawnRescue"></a>
   <h3 align="center">ContextPlus</h3>
   <p align="center">
     Empowering Conversations with Real-Time Facts<br />
     <p align="center">
   <a href="https://github.com/Multi-Agent-LLMs/ContextPlus/blob/main/LICENSE"><img src="https://img.shields.io/github/license/FawnRescue/drone" alt="License"></a>
   <a href="https://github.com/Multi-Agent-LLMs/ContextPlus/network/members"><img src="https://img.shields.io/github/forks/FawnRescue/drone?style=social" alt="GitHub forks"></a>
   <a href="https://github.com/Multi-Agent-LLMs/ContextPlus/stargazers"><img src="https://img.shields.io/github/stars/FawnRescue/drone?style=social" alt="GitHub stars"></a>
@@ -27,7 +13,29 @@
     <a href="https://github.com/Multi-Agent-LLMs/ContextPlus/issues">Report Bug</a>
     ·
     <a href="https://github.com/Multi-Agent-LLMs/ContextPlus/issues">Request Feature</a>
     </p>
   </p>
 </p>
 
+## Overview
+**ContextPlus** is a Python library designed to enhance conversations by providing real-time facts and information using large language models (LLMs). It operates completely on the CPU, making it accessible for integration into various applications without the need for specialized hardware.
+
+## Installation
+
+To install ContextPlus, use the following pip command:
+
+```bash
+pip install contextplus
+```
+
+## Usage
+
+Import and use the `context` function from the `contextplus` library to integrate real-time factual data into your projects:
+
+```python
+from contextplus import context
+
+# Example usage
+response = context("What is a LLM?")
+print(response)
+```
```

#### html2text {}

```diff
@@ -1,11 +1,15 @@
-Metadata-Version: 2.1 Name: contextplus Version: 0.1.0 Summary: Author: Florian
-Wunderlich Requires-Python: >=3.11,<4.0 Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Requires-Dist: sentence-transformers
-(>=2.7.0,<3.0.0) Requires-Dist: transformers (>=4.40.2,<5.0.0) Requires-Dist:
-wikipedia (>=1.4.0,<2.0.0) Description-Content-Type: text/markdown
+
                                  [ContextPlus]
                              ******** CCoonntteexxttPPlluuss ********
                  Empowering Conversations with Real-Time Facts
                      _[_L_i_c_e_n_s_e_]_[_G_i_t_H_u_b_ _f_o_r_k_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]
 _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
+## Overview **ContextPlus** is a Python library designed to enhance
+conversations by providing real-time facts and information using large language
+models (LLMs). It operates completely on the CPU, making it accessible for
+integration into various applications without the need for specialized
+hardware. ## Installation To install ContextPlus, use the following pip
+command: ```bash pip install contextplus ``` ## Usage Import and use the
+`context` function from the `contextplus` library to integrate real-time
+factual data into your projects: ```python from contextplus import context #
+Example usage response = context("What is a LLM?") print(response) ```
```

