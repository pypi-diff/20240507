# Comparing `tmp/kasa_crypt-0.4.1.tar.gz` & `tmp/kasa_crypt-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kasa_crypt-0.4.1.tar", max compression
+gzip compressed data, was "kasa_crypt-0.4.2.tar", max compression
```

## Comparing `kasa_crypt-0.4.1.tar` & `kasa_crypt-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11345 2024-01-10 03:10:27.825639 kasa_crypt-0.4.1/LICENSE
--rw-r--r--   0        0        0     3455 2024-01-10 03:10:27.825639 kasa_crypt-0.4.1/README.md
--rw-r--r--   0        0        0     1303 2024-01-10 03:10:27.825639 kasa_crypt-0.4.1/build_ext.py
--rw-r--r--   0        0        0     2046 2024-01-10 03:10:28.533641 kasa_crypt-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      502 2024-01-10 03:10:28.505641 kasa_crypt-0.4.1/src/kasa_crypt/__init__.py
--rw-r--r--   0        0        0     1329 2024-01-10 03:10:27.825639 kasa_crypt-0.4.1/src/kasa_crypt/_crypt_impl.pyx
--rw-r--r--   0        0        0      743 2024-01-10 03:10:27.825639 kasa_crypt-0.4.1/src/kasa_crypt/crypt_wrapper.h
--rw-r--r--   0        0        0        0 2024-01-10 03:10:27.825639 kasa_crypt-0.4.1/src/kasa_crypt/py.typed
--rw-r--r--   0        0        0      557 2024-01-10 03:10:27.825639 kasa_crypt-0.4.1/src/kasa_crypt/python_impl.py
--rw-r--r--   0        0        0     4176 1970-01-01 00:00:00.000000 kasa_crypt-0.4.1/setup.py
--rw-r--r--   0        0        0     4592 1970-01-01 00:00:00.000000 kasa_crypt-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-05-07 18:53:53.330445 kasa_crypt-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3455 2024-05-07 18:53:53.330445 kasa_crypt-0.4.2/README.md
+-rw-r--r--   0        0        0     1303 2024-05-07 18:53:53.330445 kasa_crypt-0.4.2/build_ext.py
+-rw-r--r--   0        0        0     2029 2024-05-07 18:53:53.994447 kasa_crypt-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      502 2024-05-07 18:53:53.974447 kasa_crypt-0.4.2/src/kasa_crypt/__init__.py
+-rw-r--r--   0        0        0     1329 2024-05-07 18:53:53.330445 kasa_crypt-0.4.2/src/kasa_crypt/_crypt_impl.pyx
+-rw-r--r--   0        0        0      743 2024-05-07 18:53:53.330445 kasa_crypt-0.4.2/src/kasa_crypt/crypt_wrapper.h
+-rw-r--r--   0        0        0        0 2024-05-07 18:53:53.330445 kasa_crypt-0.4.2/src/kasa_crypt/py.typed
+-rw-r--r--   0        0        0      557 2024-05-07 18:53:53.330445 kasa_crypt-0.4.2/src/kasa_crypt/python_impl.py
+-rw-r--r--   0        0        0     4176 1970-01-01 00:00:00.000000 kasa_crypt-0.4.2/setup.py
+-rw-r--r--   0        0        0     4589 1970-01-01 00:00:00.000000 kasa_crypt-0.4.2/PKG-INFO
```

### Comparing `kasa_crypt-0.4.1/LICENSE` & `kasa_crypt-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kasa_crypt-0.4.1/README.md` & `kasa_crypt-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `kasa_crypt-0.4.1/build_ext.py` & `kasa_crypt-0.4.2/build_ext.py`

 * *Files identical despite different names*

### Comparing `kasa_crypt-0.4.1/pyproject.toml` & `kasa_crypt-0.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "kasa-crypt"
-version = "0.4.1"
+version = "0.4.2"
 description = "Fast kasa crypt"
 authors = ["J. Nick Koston <nick@koston.org>"]
-license = "Apache Software License 2.0"
+license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/kasa-crypt"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
```

### Comparing `kasa_crypt-0.4.1/src/kasa_crypt/_crypt_impl.pyx` & `kasa_crypt-0.4.2/src/kasa_crypt/_crypt_impl.pyx`

 * *Files identical despite different names*

### Comparing `kasa_crypt-0.4.1/src/kasa_crypt/crypt_wrapper.h` & `kasa_crypt-0.4.2/src/kasa_crypt/crypt_wrapper.h`

 * *Files identical despite different names*

### Comparing `kasa_crypt-0.4.1/src/kasa_crypt/python_impl.py` & `kasa_crypt-0.4.2/src/kasa_crypt/python_impl.py`

 * *Files identical despite different names*

### Comparing `kasa_crypt-0.4.1/setup.py` & `kasa_crypt-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['kasa_crypt']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'kasa-crypt',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'Fast kasa crypt',
     'long_description': '# kasa-crypt\n\n<p align="center">\n  <a href="https://github.com/bdraco/kasa-crypt/actions/workflows/ci.yml?query=branch%3Amain">\n    <img src="https://img.shields.io/github/actions/workflow/status/bdraco/kasa-crypt/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://codecov.io/gh/bdraco/kasa-crypt">\n    <img src="https://img.shields.io/codecov/c/github/bdraco/kasa-crypt.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/kasa-crypt/">\n    <img src="https://img.shields.io/pypi/v/kasa-crypt.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/kasa-crypt.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/kasa-crypt.svg?style=flat-square" alt="License">\n</p>\n\nFast kasa crypt\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install kasa-crypt`\n\n## Example usage\n\n```python\nfrom kasa_crypt import encrypt, decrypt\n\nencrypted = encrypt(\'{"hello":"world"}\')\ndecrypted = decrypt(encrypted[4:])  # Always a 4 byte header\nprint (decrypted)\n```\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'nick@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bdraco/kasa-crypt',
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['kasa_crypt'] package_data = \ {'': ['*']} setup_kwargs =
-{ 'name': 'kasa-crypt', 'version': '0.4.1', 'description': 'Fast kasa crypt',
+{ 'name': 'kasa-crypt', 'version': '0.4.2', 'description': 'Fast kasa crypt',
 'long_description': '# kasa-crypt\n\n
            \n _\_n_ _[_C_I_ _S_t_a_t_u_s_]_\_n_ \n _\_n_ _[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]_\_n_ \n
 \n
            \n _\_n_ _[_P_o_e_t_r_y_]_\_n_ \n _\_n_ _[_b_l_a_c_k_]_\_n_ \n _\_n_ _[_p_r_e_-_c_o_m_m_i_t_]_\_n_ \n
 \n
       \n _\_n_ _[_P_y_P_I_ _V_e_r_s_i_o_n_]_\_n_ \n [Supported Python versions]\n [License]\n
 \n\nFast kasa crypt\n\n## Installation\n\nInstall this via pip (or your
```

### Comparing `kasa_crypt-0.4.1/PKG-INFO` & `kasa_crypt-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: kasa-crypt
-Version: 0.4.1
+Version: 0.4.2
 Summary: Fast kasa crypt
 Home-page: https://github.com/bdraco/kasa-crypt
-License: Apache Software License 2.0
+License: Apache-2.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: kasa-crypt Version: 0.4.1 Summary: Fast kasa crypt
-Home-page: https://github.com/bdraco/kasa-crypt License: Apache Software
-License 2.0 Author: J. Nick Koston Author-email: nick@koston.org Requires-
-Python: >=3.7,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
-Intended Audience :: Developers Classifier: License :: Other/Proprietary
-License Classifier: Natural Language :: English Classifier: Operating System ::
-OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Metadata-Version: 2.1 Name: kasa-crypt Version: 0.4.2 Summary: Fast kasa crypt
+Home-page: https://github.com/bdraco/kasa-crypt License: Apache-2.0 Author: J.
+Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
+:: Developers Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Project-URL: Bug Tracker, https://
 github.com/bdraco/kasa-crypt/issues Project-URL: Changelog, https://github.com/
 bdraco/kasa-crypt/blob/main/CHANGELOG.md Project-URL: Repository, https://
```

