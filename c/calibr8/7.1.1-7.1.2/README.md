# Comparing `tmp/calibr8-7.1.1.tar.gz` & `tmp/calibr8-7.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calibr8-7.1.1.tar", last modified: Tue Feb 13 17:24:48 2024, max compression
+gzip compressed data, was "calibr8-7.1.2.tar", last modified: Tue May  7 08:12:17 2024, max compression
```

## Comparing `calibr8-7.1.1.tar` & `calibr8-7.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:24:48.245653 calibr8-7.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-02-13 17:16:50.000000 calibr8-7.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-02-13 17:24:48.245653 calibr8-7.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-02-13 17:16:50.000000 calibr8-7.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:24:48.241653 calibr8-7.1.1/calibr8/
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-02-13 17:16:50.000000 calibr8-7.1.1/calibr8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:24:48.241653 calibr8-7.1.1/calibr8/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-02-13 17:17:10.000000 calibr8-7.1.1/calibr8/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)    40093 2024-02-13 17:17:10.000000 calibr8-7.1.1/calibr8/__pycache__/core.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-02-13 17:17:11.000000 calibr8-7.1.1/calibr8/__pycache__/optimization.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)   106412 2024-02-13 17:17:11.000000 calibr8-7.1.1/calibr8/__pycache__/test_all.cpython-39-pytest-8.0.0.pyc
--rw-r--r--   0 runner    (1001) docker     (127)    13913 2024-02-13 17:17:10.000000 calibr8-7.1.1/calibr8/__pycache__/utils.cpython-39.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:24:48.241653 calibr8-7.1.1/calibr8/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 17:16:50.000000 calibr8-7.1.1/calibr8/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:24:48.245653 calibr8-7.1.1/calibr8/contrib/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-13 17:17:10.000000 calibr8-7.1.1/calibr8/contrib/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-02-13 17:17:10.000000 calibr8-7.1.1/calibr8/contrib/__pycache__/noise.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-02-13 17:17:11.000000 calibr8-7.1.1/calibr8/contrib/__pycache__/normal.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)    15038 2024-02-13 17:17:11.000000 calibr8-7.1.1/calibr8/contrib/__pycache__/studentt.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-02-13 17:16:50.000000 calibr8-7.1.1/calibr8/contrib/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    13773 2024-02-13 17:16:50.000000 calibr8-7.1.1/calibr8/contrib/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)    15471 2024-02-13 17:16:50.000000 calibr8-7.1.1/calibr8/contrib/studentt.py
--rw-r--r--   0 runner    (1001) docker     (127)    42854 2024-02-13 17:16:50.000000 calibr8-7.1.1/calibr8/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-02-13 17:16:50.000000 calibr8-7.1.1/calibr8/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 17:24:48.000000 calibr8-7.1.1/calibr8/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    65574 2024-02-13 17:16:50.000000 calibr8-7.1.1/calibr8/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)    16710 2024-02-13 17:16:50.000000 calibr8-7.1.1/calibr8/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:24:48.245653 calibr8-7.1.1/calibr8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-02-13 17:24:48.000000 calibr8-7.1.1/calibr8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-02-13 17:24:48.000000 calibr8-7.1.1/calibr8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 17:24:48.000000 calibr8-7.1.1/calibr8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-13 17:24:48.000000 calibr8-7.1.1/calibr8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-13 17:24:48.000000 calibr8-7.1.1/calibr8.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-13 17:16:50.000000 calibr8-7.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 17:24:48.245653 calibr8-7.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-02-13 17:16:50.000000 calibr8-7.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:12:17.048143 calibr8-7.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-05-07 08:04:17.000000 calibr8-7.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-07 08:12:17.048143 calibr8-7.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-07 08:04:17.000000 calibr8-7.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:12:17.044142 calibr8-7.1.2/calibr8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-07 08:04:17.000000 calibr8-7.1.2/calibr8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:12:17.048143 calibr8-7.1.2/calibr8/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-07 08:04:36.000000 calibr8-7.1.2/calibr8/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    58231 2024-05-07 08:04:37.000000 calibr8-7.1.2/calibr8/__pycache__/core.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    11165 2024-05-07 08:04:38.000000 calibr8-7.1.2/calibr8/__pycache__/optimization.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)   288757 2024-05-07 08:04:38.000000 calibr8-7.1.2/calibr8/__pycache__/test_all.cpython-311-pytest-8.2.0.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    22666 2024-05-07 08:04:37.000000 calibr8-7.1.2/calibr8/__pycache__/utils.cpython-311.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:12:17.048143 calibr8-7.1.2/calibr8/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 08:04:17.000000 calibr8-7.1.2/calibr8/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:12:17.048143 calibr8-7.1.2/calibr8/contrib/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 08:04:36.000000 calibr8-7.1.2/calibr8/contrib/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-07 08:04:36.000000 calibr8-7.1.2/calibr8/contrib/__pycache__/noise.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    18022 2024-05-07 08:04:38.000000 calibr8-7.1.2/calibr8/contrib/__pycache__/normal.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    19906 2024-05-07 08:04:38.000000 calibr8-7.1.2/calibr8/contrib/__pycache__/studentt.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-07 08:04:17.000000 calibr8-7.1.2/calibr8/contrib/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13773 2024-05-07 08:04:17.000000 calibr8-7.1.2/calibr8/contrib/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15471 2024-05-07 08:04:17.000000 calibr8-7.1.2/calibr8/contrib/studentt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42827 2024-05-07 08:04:17.000000 calibr8-7.1.2/calibr8/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-05-07 08:04:17.000000 calibr8-7.1.2/calibr8/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 08:12:16.000000 calibr8-7.1.2/calibr8/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    65574 2024-05-07 08:04:17.000000 calibr8-7.1.2/calibr8/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16860 2024-05-07 08:04:17.000000 calibr8-7.1.2/calibr8/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:12:17.048143 calibr8-7.1.2/calibr8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-07 08:12:17.000000 calibr8-7.1.2/calibr8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-07 08:12:17.000000 calibr8-7.1.2/calibr8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:12:17.000000 calibr8-7.1.2/calibr8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 08:12:17.000000 calibr8-7.1.2/calibr8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 08:12:17.000000 calibr8-7.1.2/calibr8.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-07 08:04:17.000000 calibr8-7.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:12:17.048143 calibr8-7.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-07 08:04:17.000000 calibr8-7.1.2/setup.py
```

### Comparing `calibr8-7.1.1/LICENSE` & `calibr8-7.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calibr8-7.1.1/PKG-INFO` & `calibr8-7.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibr8
-Version: 7.1.1
+Version: 7.1.2
 Summary: Toolbox for non-linear calibration modeling.
 Home-page: https://github.com/JuBiotech/calibr8
 Author: Laura Marie Helleckes, Michael Osthege
 Author-email: l.helleckes@fz-juelich.de, m.osthege@fz-juelich.de
 License: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
@@ -14,18 +14,14 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: scipy>1.6.0
-Requires-Dist: typing_extensions
 
 [![PyPI version](https://img.shields.io/pypi/v/calibr8)](https://pypi.org/project/calibr8)
 [![pipeline](https://github.com/jubiotech/calibr8/workflows/pipeline/badge.svg)](https://github.com/jubiotech/calibr8/actions)
 [![coverage](https://codecov.io/gh/jubiotech/calibr8/branch/master/graph/badge.svg)](https://codecov.io/gh/jubiotech/calibr8)
 [![documentation](https://readthedocs.org/projects/calibr8/badge/?version=latest)](https://calibr8.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/306862348.svg)](https://zenodo.org/badge/latestdoi/306862348)
```

### Comparing `calibr8-7.1.1/README.md` & `calibr8-7.1.2/README.md`

 * *Files identical despite different names*

### Comparing `calibr8-7.1.1/calibr8/__init__.py` & `calibr8-7.1.2/calibr8/__init__.py`

 * *Files identical despite different names*

### Comparing `calibr8-7.1.1/calibr8/contrib/__pycache__/studentt.cpython-39.pyc` & `calibr8-7.1.2/calibr8/contrib/__pycache__/normal.cpython-311.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Feb 13 17:16:50 2024 UTC, .py size: 15471 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,940 +1,1127 @@
-00000000: 610d 0d0a 0000 0000 02a4 cb65 6f3c 0000  a..........eo<..
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
-00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 5a02 6401 6403 6c01 6d03 5a03 6d04 5a04  Z.d.d.l.m.Z.m.Z.
-00000050: 6d05 5a05 0100 6404 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 6d08 5a08 0100 6406 6407 6c06 6d09 5a09  m.Z...d.d.l.m.Z.
-00000070: 0100 4700 6408 6409 8400 6409 6507 6a0a  ..G.d.d...d.e.j.
-00000080: 6509 6a0b 8304 5a0c 4700 640a 640b 8400  e.j...Z.G.d.d...
-00000090: 640b 6507 6a0a 6509 6a0b 8304 5a0d 4700  d.e.j.e.j...Z.G.
-000000a0: 640c 640d 8400 640d 6507 6a0a 6509 6a0b  d.d...d.e.j.e.j.
-000000b0: 8304 5a0e 4700 640e 640f 8400 640f 6507  ..Z.G.d.d...d.e.
-000000c0: 6a0a 6509 6a0b 8304 5a0f 4700 6410 6411  j.e.j...Z.G.d.d.
-000000d0: 8400 6411 6507 6a0a 6509 6a0b 8304 5a10  ..d.e.j.e.j...Z.
-000000e0: 6402 5300 2912 7a6e 0a54 6869 7320 6d6f  d.S.).zn.This mo
-000000f0: 6475 6c65 2069 6d70 6c65 6d65 6e74 7320  dule implements 
-00000100: 7265 7573 6162 6c65 2063 616c 6962 7261  reusable calibra
-00000110: 7469 6f6e 206d 6f64 656c 730a 7769 7468  tion models.with
-00000120: 2053 7475 6465 6e74 732d 7420 6469 7374   Students-t dist
-00000130: 7269 6275 7469 6f6e 7320 666f 7220 7468  ributions for th
-00000140: 6520 6465 7065 6e64 656e 7420 7661 7269  e dependent vari
-00000150: 6162 6c65 2e0a e900 0000 004e 2903 da08  able.......N)...
-00000160: 4f70 7469 6f6e 616c da08 5365 7175 656e  Optional..Sequen
-00000170: 6365 da05 5475 706c 65e9 0200 0000 2902  ce..Tuple.....).
-00000180: da04 636f 7265 da05 7574 696c 73e9 0100  ..core..utils...
-00000190: 0000 2901 da05 6e6f 6973 6563 0000 0000  ..)...noisec....
-000001a0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-000001b0: 0000 0000 732c 0000 0065 005a 0164 005a  ....s,...e.Z.d.Z
-000001c0: 0265 0365 0365 046a 0565 0319 0064 019c  .e.e.e.j.e...d..
-000001d0: 0387 0066 0164 0264 0384 0c5a 0687 0004  ...f.d.d...Z....
-000001e0: 005a 0753 0029 04da 0a42 6173 654d 6f64  .Z.S.)...BaseMod
-000001f0: 656c 54a9 03da 0f69 6e64 6570 656e 6465  elT....independe
-00000200: 6e74 5f6b 6579 da0d 6465 7065 6e64 656e  nt_key..dependen
-00000210: 745f 6b65 79da 0b74 6865 7461 5f6e 616d  t_key..theta_nam
-00000220: 6573 6303 0000 0000 0000 0001 0000 0004  esc.............
-00000230: 0000 0005 0000 0003 0000 0073 2200 0000  ...........s"...
-00000240: 7400 a001 6401 7402 a102 0100 7403 8300  t...d.t.....t...
-00000250: 6a04 7c01 7c02 7c03 6402 8d03 0100 6400  j.|.|.|.d.....d.
-00000260: 5300 2903 4e7a 6c54 6865 6042 6173 654d  S.).NzlThe`BaseM
-00000270: 6f64 656c 5460 2063 6c61 7373 2069 7320  odelT` class is 
-00000280: 6465 7072 6563 6174 6564 2e20 496e 6865  deprecated. Inhe
-00000290: 7269 7420 6063 6f72 652e 436f 6e74 696e  rit `core.Contin
-000002a0: 756f 7573 556e 6976 6172 6961 7465 4d6f  uousUnivariateMo
-000002b0: 6465 6c2c 206e 6f69 7365 2e53 7475 6465  del, noise.Stude
-000002c0: 6e74 544e 6f69 7365 6020 6469 7265 6374  ntTNoise` direct
-000002d0: 6c79 2e72 0b00 0000 2905 da08 7761 726e  ly.r....)...warn
-000002e0: 696e 6773 da04 7761 726e da0d 4675 7475  ings..warn..Futu
-000002f0: 7265 5761 726e 696e 67da 0573 7570 6572  reWarning..super
-00000300: da08 5f5f 696e 6974 5f5f 2904 da04 7365  ..__init__)...se
-00000310: 6c66 720c 0000 0072 0d00 0000 720e 0000  lfr....r....r...
-00000320: 00a9 01da 095f 5f63 6c61 7373 5f5f a900  .....__class__..
-00000330: fa3d 2f68 6f6d 652f 7275 6e6e 6572 2f77  .=/home/runner/w
-00000340: 6f72 6b2f 6361 6c69 6272 382f 6361 6c69  ork/calibr8/cali
-00000350: 6272 382f 6361 6c69 6272 382f 636f 6e74  br8/calibr8/cont
-00000360: 7269 622f 7374 7564 656e 7474 2e70 7972  rib/studentt.pyr
-00000370: 1300 0000 0e00 0000 730e 0000 0000 0104  ........s.......
-00000380: 0102 0202 fd04 0506 0106 ff7a 1342 6173  ...........z.Bas
-00000390: 654d 6f64 656c 542e 5f5f 696e 6974 5f5f  eModelT.__init__
-000003a0: 2908 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000003b0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000003c0: 6e61 6d65 5f5f da03 7374 72da 0674 7970  name__..str..typ
-000003d0: 696e 6772 0400 0000 7213 0000 00da 0d5f  ingr....r......_
-000003e0: 5f63 6c61 7373 6365 6c6c 5f5f 7217 0000  _classcell__r...
-000003f0: 0072 1700 0000 7215 0000 0072 1800 0000  .r....r....r....
-00000400: 720a 0000 000d 0000 0073 0200 0000 0801  r........s......
-00000410: 720a 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000420: 0000 0000 0000 0800 0000 0000 0000 7356  ..............sV
-00000430: 0000 0065 005a 0164 005a 0264 0164 0264  ...e.Z.d.Z.d.d.d
-00000440: 039c 0265 0365 0365 0465 0465 0565 0665  ...e.e.e.e.e.e.e
-00000450: 0319 0019 0064 049c 0587 0066 0164 0564  .....d.....f.d.d
-00000460: 0684 0e5a 0764 0264 079c 0164 0864 0984  ...Z.d.d...d.d..
-00000470: 025a 0864 0264 079c 0164 0a64 0b84 025a  .Z.d.d...d.d...Z
-00000480: 0987 0004 005a 0a53 0029 0cda 1442 6173  .....Z.S.)...Bas
-00000490: 6550 6f6c 796e 6f6d 6961 6c4d 6f64 656c  ePolynomialModel
-000004a0: 5472 0100 0000 4ea9 02da 0c73 6361 6c65  Tr....N....scale
-000004b0: 5f64 6567 7265 6572 0e00 0000 2905 720c  _degreer....).r.
-000004c0: 0000 0072 0d00 0000 da09 6d75 5f64 6567  ...r......mu_deg
-000004d0: 7265 6572 2100 0000 720e 0000 0063 0100  reer!...r....c..
-000004e0: 0000 0000 0000 0500 0000 0600 0000 0600  ................
-000004f0: 0000 0300 0000 7378 0000 007c 0364 016b  ......sx...|.d.k
-00000500: 0272 1074 0064 0283 0182 017c 037c 005f  .r.t.d.....|.|._
-00000510: 0174 02a0 037c 04a1 017c 005f 047c 0564  .t...|...|._.|.d
-00000520: 0375 0072 6274 0564 0464 0584 0074 067c  .u.rbt.d.d...t.|
-00000530: 0364 0617 0083 0144 0083 0183 0174 0564  .d.....D.....t.d
-00000540: 0764 0584 0074 067c 0464 0617 0083 0144  .d...t.|.d.....D
-00000550: 0083 0183 0117 0064 0817 007d 0574 0783  .......d...}.t..
-00000560: 006a 087c 017c 027c 0564 098d 0301 0064  .j.|.|.|.d.....d
-00000570: 0353 0029 0a61 8d02 0000 5465 6d70 6c61  .S.).a....Templa
-00000580: 7465 2066 6f72 2061 206d 6f64 656c 2077  te for a model w
-00000590: 6974 6820 706f 6c79 6e6f 6d69 616c 2074  ith polynomial t
-000005a0: 7265 6e64 2028 6d75 2920 616e 6420 7363  rend (mu) and sc
-000005b0: 616c 6520 2861 7320 6120 6675 6e63 7469  ale (as a functi
-000005c0: 6f6e 206f 6620 6d75 290a 2020 2020 2020  on of mu).      
-000005d0: 2020 7769 7468 2061 2053 7475 6465 6e74    with a Student
-000005e0: 2d74 2064 6973 7472 6962 7574 6564 206f  -t distributed o
-000005f0: 6273 6572 7661 7469 6f6e 206e 6f69 7365  bservation noise
-00000600: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00000610: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00000620: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00000630: 2069 6e64 6570 656e 6465 6e74 5f6b 6579   independent_key
-00000640: 203a 2073 7472 0a20 2020 2020 2020 2020   : str.         
-00000650: 2020 206e 616d 6520 6f66 2074 6865 2069     name of the i
-00000660: 6e64 6570 656e 6465 6e74 2076 6172 6961  ndependent varia
-00000670: 626c 650a 2020 2020 2020 2020 6465 7065  ble.        depe
-00000680: 6e64 656e 745f 6b65 7920 3a20 7374 720a  ndent_key : str.
-00000690: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-000006a0: 206f 6620 7468 6520 6465 7065 6e64 656e   of the dependen
-000006b0: 7420 7661 7269 6162 6c65 0a20 2020 2020  t variable.     
-000006c0: 2020 206d 755f 6465 6772 6565 203a 2069     mu_degree : i
-000006d0: 6e74 0a20 2020 2020 2020 2020 2020 2064  nt.            d
-000006e0: 6567 7265 6520 6f66 2074 6865 2070 6f6c  egree of the pol
-000006f0: 796e 6f6d 6961 6c20 6d6f 6465 6c20 6465  ynomial model de
-00000700: 7363 7269 6269 6e67 2074 6865 2074 7265  scribing the tre
-00000710: 6e64 2028 6d75 290a 2020 2020 2020 2020  nd (mu).        
-00000720: 7363 616c 655f 6465 6772 6565 203a 206f  scale_degree : o
-00000730: 7074 696f 6e61 6c2c 2069 6e74 0a20 2020  ptional, int.   
-00000740: 2020 2020 2020 2020 2064 6567 7265 6520           degree 
-00000750: 6f66 2074 6865 2070 6f6c 796e 6f6d 6961  of the polynomia
-00000760: 6c20 6d6f 6465 6c20 6465 7363 7269 6269  l model describi
-00000770: 6e67 2074 6865 2073 6361 6c65 2061 7320  ng the scale as 
-00000780: 6120 6675 6e63 7469 6f6e 206f 6620 6d75  a function of mu
-00000790: 0a20 2020 2020 2020 2074 6865 7461 5f6e  .        theta_n
-000007a0: 616d 6573 203a 206f 7074 696f 6e61 6c2c  ames : optional,
-000007b0: 2074 7570 6c65 206f 6620 7374 720a 2020   tuple of str.  
-000007c0: 2020 2020 2020 2020 2020 6d61 7920 6265            may be
-000007d0: 2075 7365 6420 746f 2073 6574 2074 6865   used to set the
-000007e0: 206e 616d 6573 206f 6620 7468 6520 6d6f   names of the mo
-000007f0: 6465 6c20 7061 7261 6d65 7465 7273 0a20  del parameters. 
-00000800: 2020 2020 2020 2072 0100 0000 7a36 302d         r....z60-
-00000810: 6465 6772 6565 2028 636f 6e73 7461 6e74  degree (constant
-00000820: 2920 6d75 2063 616c 6962 7261 7469 6f6e  ) mu calibration
-00000830: 206d 6f64 656c 7320 6172 6520 7573 656c   models are usel
-00000840: 6573 732e 4e63 0100 0000 0000 0000 0000  ess.Nc..........
-00000850: 0000 0200 0000 0300 0000 7300 0000 7318  ..........s...s.
-00000860: 0000 007c 005d 107d 0164 007c 019b 009d  ...|.].}.d.|....
-00000870: 0256 0001 0071 0264 0153 0029 02da 036d  .V...q.d.S.)...m
-00000880: 755f 4e72 1700 0000 a902 da02 2e30 da01  u_Nr.........0..
-00000890: 6472 1700 0000 7217 0000 0072 1800 0000  dr....r....r....
-000008a0: da09 3c67 656e 6578 7072 3e39 0000 00f3  ..<genexpr>9....
-000008b0: 0000 0000 7a30 4261 7365 506f 6c79 6e6f  ....z0BasePolyno
-000008c0: 6d69 616c 4d6f 6465 6c54 2e5f 5f69 6e69  mialModelT.__ini
-000008d0: 745f 5f2e 3c6c 6f63 616c 733e 2e3c 6765  t__.<locals>.<ge
-000008e0: 6e65 7870 723e 7208 0000 0063 0100 0000  nexpr>r....c....
-000008f0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000900: 7300 0000 7318 0000 007c 005d 107d 0164  s...s....|.].}.d
-00000910: 007c 019b 009d 0256 0001 0071 0264 0153  .|.....V...q.d.S
-00000920: 00a9 025a 0673 6361 6c65 5f4e 7217 0000  ...Z.scale_Nr...
-00000930: 0072 2400 0000 7217 0000 0072 1700 0000  .r$...r....r....
-00000940: 7218 0000 0072 2700 0000 3a00 0000 7228  r....r'...:...r(
-00000950: 0000 00a9 01da 0264 6672 0b00 0000 2909  .......dfr....).
-00000960: da0a 5661 6c75 6545 7272 6f72 7222 0000  ..ValueErrorr"..
-00000970: 0072 0700 0000 da12 6368 6563 6b5f 7363  .r......check_sc
-00000980: 616c 655f 6465 6772 6565 7221 0000 00da  ale_degreer!....
-00000990: 0574 7570 6c65 da05 7261 6e67 6572 1200  .tuple..ranger..
-000009a0: 0000 7213 0000 0029 0672 1400 0000 720c  ..r....).r....r.
-000009b0: 0000 0072 0d00 0000 7222 0000 0072 2100  ...r....r"...r!.
-000009c0: 0000 720e 0000 0072 1500 0000 7217 0000  ..r....r....r...
-000009d0: 0072 1800 0000 7213 0000 001a 0000 0073  .r....r........s
-000009e0: 1c00 0000 0019 0801 0801 0601 0c01 0802  ................
-000009f0: 1801 18ff 0202 02fe 02ff 0205 0601 06ff  ................
-00000a00: 7a1d 4261 7365 506f 6c79 6e6f 6d69 616c  z.BasePolynomial
-00000a10: 4d6f 6465 6c54 2e5f 5f69 6e69 745f 5fa9  ModelT.__init__.
-00000a20: 01da 0574 6865 7461 6302 0000 0000 0000  ...thetac.......
-00000a30: 0001 0000 0006 0000 0006 0000 0043 0000  .............C..
-00000a40: 0073 7c00 0000 7c02 6401 7500 720e 7c00  .s|...|.d.u.r.|.
-00000a50: 6a00 7d02 7401 6a02 7c01 7c02 6401 7c00  j.}.t.j.|.|.d.|.
-00000a60: 6a03 6402 1700 8502 1900 6403 8d02 7d03  j.d.......d...}.
-00000a70: 7c00 6a04 6404 6b02 723e 7c02 6405 1900  |.j.d.k.r>|.d...
-00000a80: 7d04 6e2c 7401 6a02 7c03 7c02 7c00 6a03  }.n,t.j.|.|.|.j.
-00000a90: 6402 1700 7c00 6a03 6402 1700 7c00 6a04  d...|.j.d...|.j.
-00000aa0: 1700 6402 1700 8502 1900 6403 8d02 7d04  ..d.......d...}.
-00000ab0: 7c02 6406 1900 7d05 7c03 7c04 7c05 6603  |.d...}.|.|.|.f.
-00000ac0: 5300 2907 61a6 0300 0050 7265 6469 6374  S.).a....Predict
-00000ad0: 7320 7468 6520 7061 7261 6d65 7465 7273  s the parameters
-00000ae0: 206d 7520 616e 6420 7363 616c 6520 6f66   mu and scale of
-00000af0: 2061 2053 7475 6465 6e74 2d74 2064 6973   a Student-t dis
-00000b00: 7472 6962 7574 696f 6e20 7768 6963 680a  tribution which.
-00000b10: 2020 2020 2020 2020 6368 6172 6163 7465          characte
-00000b20: 7269 7a65 7320 7468 6520 6465 7065 6e64  rizes the depend
-00000b30: 656e 7420 7661 7269 6162 6c65 2067 6976  ent variable giv
-00000b40: 656e 2076 616c 7565 7320 6f66 2074 6865  en values of the
-00000b50: 2069 6e64 6570 656e 6465 6e74 2076 6172   independent var
-00000b60: 6961 626c 652e 0a0a 2020 2020 2020 2020  iable...        
-00000b70: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00000b80: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00000b90: 2020 2020 2020 7820 3a20 6172 7261 792d        x : array-
-00000ba0: 6c69 6b65 0a20 2020 2020 2020 2020 2020  like.           
-00000bb0: 2076 616c 7565 7320 6f66 2074 6865 2069   values of the i
-00000bc0: 6e64 6570 656e 6465 6e74 2076 6172 6961  ndependent varia
-00000bd0: 626c 650a 2020 2020 2020 2020 7468 6574  ble.        thet
-00000be0: 6120 3a20 6f70 7469 6f6e 616c 2c20 6172  a : optional, ar
-00000bf0: 7261 792d 6c69 6b65 0a20 2020 2020 2020  ray-like.       
-00000c00: 2020 2020 2070 6172 616d 6574 6572 2076       parameter v
-00000c10: 6563 746f 7220 6f66 2074 6865 2063 616c  ector of the cal
-00000c20: 6962 7261 7469 6f6e 206d 6f64 656c 3a0a  ibration model:.
-00000c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c40: 5b6d 755f 6465 6772 6565 5d20 7061 7261  [mu_degree] para
-00000c50: 6d65 7465 7273 2066 6f72 206d 7520 286c  meters for mu (l
-00000c60: 6f77 6573 7420 6465 6772 6565 2066 6972  owest degree fir
-00000c70: 7374 290a 2020 2020 2020 2020 2020 2020  st).            
-00000c80: 2020 2020 5b73 6361 6c65 5f64 6567 7265      [scale_degre
-00000c90: 655d 2070 6172 616d 6574 6572 7320 666f  e] parameters fo
-00000ca0: 7220 7363 616c 6520 286c 6f77 6573 7420  r scale (lowest 
-00000cb0: 6465 6772 6565 2066 6972 7374 290a 2020  degree first).  
-00000cc0: 2020 2020 2020 2020 2020 2020 2020 3120                1 
-00000cd0: 7061 7261 6d65 7465 7220 666f 7220 6465  parameter for de
-00000ce0: 6772 6565 206f 6620 6672 6565 646f 6d0a  gree of freedom.
-00000cf0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00000d00: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00000d10: 0a20 2020 2020 2020 206d 7520 3a20 6172  .        mu : ar
-00000d20: 7261 792d 6c69 6b65 0a20 2020 2020 2020  ray-like.       
-00000d30: 2020 2020 2076 616c 7565 7320 666f 7220       values for 
-00000d40: 7468 6520 6d75 2070 6172 616d 6574 6572  the mu parameter
-00000d50: 206f 6620 6120 5374 7564 656e 742d 7420   of a Student-t 
-00000d60: 6469 7374 7269 6275 7469 6f6e 2064 6573  distribution des
-00000d70: 6372 6962 696e 6720 7468 6520 6465 7065  cribing the depe
-00000d80: 6e64 656e 7420 7661 7269 6162 6c65 0a20  ndent variable. 
-00000d90: 2020 2020 2020 2073 6361 6c65 203a 2061         scale : a
-00000da0: 7272 6179 2d6c 696b 6520 6f72 2066 6c6f  rray-like or flo
-00000db0: 6174 0a20 2020 2020 2020 2020 2020 2076  at.            v
-00000dc0: 616c 7565 7320 666f 7220 7468 6520 7363  alues for the sc
-00000dd0: 616c 6520 7061 7261 6d65 7465 7220 6f66  ale parameter of
-00000de0: 2061 2053 7475 6465 6e74 2d74 2064 6973   a Student-t dis
-00000df0: 7472 6962 7574 696f 6e20 6465 7363 7269  tribution descri
-00000e00: 6269 6e67 2074 6865 2064 6570 656e 6465  bing the depende
-00000e10: 6e74 2076 6172 6961 626c 650a 2020 2020  nt variable.    
-00000e20: 2020 2020 6466 203a 2066 6c6f 6174 0a20      df : float. 
-00000e30: 2020 2020 2020 2020 2020 2064 6567 7265             degre
-00000e40: 6520 6f66 2066 7265 6564 6f6d 206f 6620  e of freedom of 
-00000e50: 5374 7564 656e 742d 7420 6469 7374 7269  Student-t distri
-00000e60: 6275 7469 6f6e 0a20 2020 2020 2020 204e  bution.        N
-00000e70: 7208 0000 0072 3000 0000 7201 0000 00e9  r....r0...r.....
-00000e80: feff ffff e9ff ffff ff29 05da 0c74 6865  .........)...the
-00000e90: 7461 5f66 6974 7465 6472 0600 0000 da0a  ta_fittedr......
-00000ea0: 706f 6c79 6e6f 6d69 616c 7222 0000 0072  polynomialr"...r
-00000eb0: 2100 0000 a906 7214 0000 00da 0178 7231  !.....r......xr1
-00000ec0: 0000 00da 026d 75da 0573 6361 6c65 722b  .....mu..scaler+
-00000ed0: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
-00000ee0: 0000 da11 7072 6564 6963 745f 6465 7065  ....predict_depe
-00000ef0: 6e64 656e 7441 0000 0073 1400 0000 0017  ndentA...s......
-00000f00: 0801 0601 1c01 0a01 0a02 0401 22ff 0603  ............"...
-00000f10: 0801 7a26 4261 7365 506f 6c79 6e6f 6d69  ..z&BasePolynomi
-00000f20: 616c 4d6f 6465 6c54 2e70 7265 6469 6374  alModelT.predict
-00000f30: 5f64 6570 656e 6465 6e74 6302 0000 0000  _dependentc.....
-00000f40: 0000 0001 0000 0005 0000 0003 0000 0043  ...............C
-00000f50: 0000 0073 3c00 0000 7c02 6401 7500 720e  ...s<...|.d.u.r.
-00000f60: 7c00 6a00 7d02 7c00 6a01 6402 6b04 7220  |.j.}.|.j.d.k.r 
-00000f70: 7402 6403 8301 8201 7c02 6401 6404 8502  t.d.....|.d.d...
-00000f80: 1900 5c02 7d03 7d04 7c01 7c03 1800 7c04  ..\.}.}.|.|...|.
-00000f90: 1b00 5300 2905 6133 0200 0050 7265 6469  ..S.).a3...Predi
-00000fa0: 6374 2074 6865 2069 6e64 6570 656e 6465  ct the independe
-00000fb0: 6e74 2076 6172 6961 626c 6520 7573 696e  nt variable usin
-00000fc0: 6720 7468 6520 696e 7665 7273 6520 7472  g the inverse tr
-00000fd0: 656e 6420 6d6f 6465 6c2e 0a0a 2020 2020  end model...    
-00000fe0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00000ff0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00001000: 2d0a 2020 2020 2020 2020 7920 3a20 6172  -.        y : ar
-00001010: 7261 792d 6c69 6b65 0a20 2020 2020 2020  ray-like.       
-00001020: 2020 2020 206f 6273 6572 7661 7469 6f6e       observation
-00001030: 730a 2020 2020 2020 2020 7468 6574 6120  s.        theta 
-00001040: 3a20 6f70 7469 6f6e 616c 2c20 6172 7261  : optional, arra
-00001050: 792d 6c69 6b65 0a20 2020 2020 2020 2020  y-like.         
-00001060: 2020 2070 6172 616d 6574 6572 2076 6563     parameter vec
-00001070: 746f 7220 6f66 2074 6865 2063 616c 6962  tor of the calib
-00001080: 7261 7469 6f6e 206d 6f64 656c 3a0a 2020  ration model:.  
-00001090: 2020 2020 2020 2020 2020 2020 2020 5b6d                [m
-000010a0: 755f 6465 6772 6565 5d20 7061 7261 6d65  u_degree] parame
-000010b0: 7465 7273 2066 6f72 206d 7520 286c 6f77  ters for mu (low
-000010c0: 6573 7420 6465 6772 6565 2066 6972 7374  est degree first
-000010d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000010e0: 2020 5b73 6361 6c65 5f64 6567 7265 655d    [scale_degree]
-000010f0: 2070 6172 616d 6574 6572 7320 666f 7220   parameters for 
-00001100: 7363 616c 6520 286c 6f77 6573 7420 6465  scale (lowest de
-00001110: 6772 6565 2066 6972 7374 290a 2020 2020  gree first).    
-00001120: 2020 2020 2020 2020 2020 2020 3120 7061              1 pa
-00001130: 7261 6d65 7465 7220 666f 7220 6465 6772  rameter for degr
-00001140: 6565 206f 6620 6672 6565 646f 6d0a 0a20  ee of freedom.. 
-00001150: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-00001160: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00001170: 2020 2020 2020 2078 203a 2061 7272 6179         x : array
-00001180: 2d6c 696b 650a 2020 2020 2020 2020 2020  -like.          
-00001190: 2020 7072 6564 6963 7465 6420 696e 6465    predicted inde
-000011a0: 7065 6e64 656e 7420 7661 6c75 6573 2067  pendent values g
-000011b0: 6976 656e 2074 6865 206f 6273 6572 7661  iven the observa
-000011c0: 7469 6f6e 730a 2020 2020 2020 2020 4e72  tions.        Nr
-000011d0: 0800 0000 7a43 496e 7665 7273 6520 7072  ....zCInverse pr
-000011e0: 6564 6963 7469 6f6e 206f 6620 6869 6768  ediction of high
-000011f0: 6572 206f 7264 6572 2070 6f6c 796e 6f6d  er order polynom
-00001200: 6961 6c73 2061 7265 206e 6f74 2069 6d70  ials are not imp
-00001210: 6c65 6d65 6e74 6564 2e72 0500 0000 2903  lemented.r....).
-00001220: 7234 0000 0072 2200 0000 da13 4e6f 7449  r4...r".....NotI
-00001230: 6d70 6c65 6d65 6e74 6564 4572 726f 7229  mplementedError)
-00001240: 0572 1400 0000 da01 7972 3100 0000 da01  .r......yr1.....
-00001250: 61da 0162 7217 0000 0072 1700 0000 7218  a..br....r....r.
-00001260: 0000 00da 1370 7265 6469 6374 5f69 6e64  .....predict_ind
-00001270: 6570 656e 6465 6e74 6400 0000 730c 0000  ependentd...s...
-00001280: 0000 1208 0106 010a 0108 0110 017a 2842  .............z(B
-00001290: 6173 6550 6f6c 796e 6f6d 6961 6c4d 6f64  asePolynomialMod
-000012a0: 656c 542e 7072 6564 6963 745f 696e 6465  elT.predict_inde
-000012b0: 7065 6e64 656e 74a9 0b72 1900 0000 721a  pendent..r....r.
-000012c0: 0000 0072 1b00 0000 721c 0000 00da 0369  ...r....r......i
-000012d0: 6e74 7202 0000 0072 0300 0000 7213 0000  ntr....r....r...
-000012e0: 0072 3a00 0000 723f 0000 0072 1e00 0000  .r:...r?...r....
-000012f0: 7217 0000 0072 1700 0000 7215 0000 0072  r....r....r....r
-00001300: 1800 0000 721f 0000 0019 0000 0073 1600  ....r........s..
-00001310: 0000 0807 0201 02f9 0403 0201 0201 0201  ................
-00001320: 0201 0af9 1027 0e23 721f 0000 0063 0000  .....'.#r....c..
-00001330: 0000 0000 0000 0000 0000 0000 0000 0700  ................
-00001340: 0000 0000 0000 7354 0000 0065 005a 0164  ......sT...e.Z.d
-00001350: 005a 0264 0164 0264 039c 0265 0365 0365  .Z.d.d.d...e.e.e
-00001360: 0465 0565 0665 0319 0019 0064 049c 0487  .e.e.e.....d....
-00001370: 0066 0164 0564 0684 0e5a 0764 0264 079c  .f.d.d...Z.d.d..
-00001380: 0164 0864 0984 025a 0864 0264 079c 0164  .d.d...Z.d.d...d
-00001390: 0a64 0b84 025a 0987 0004 005a 0a53 0029  .d...Z.....Z.S.)
-000013a0: 0cda 1742 6173 6541 7379 6d6d 6574 7269  ...BaseAsymmetri
-000013b0: 634c 6f67 6973 7469 6354 7201 0000 004e  cLogisticTr....N
-000013c0: 7220 0000 00a9 0472 0c00 0000 720d 0000  r .....r....r...
-000013d0: 0072 2100 0000 720e 0000 0063 0100 0000  .r!...r....c....
-000013e0: 0000 0000 0400 0000 0500 0000 0600 0000  ................
-000013f0: 0300 0000 7356 0000 0074 00a0 017c 03a1  ....sV...t...|..
-00001400: 017c 005f 027c 0464 0175 0072 4074 0364  .|._.|.d.u.r@t.d
-00001410: 02a0 0464 03a1 0183 0174 0364 0464 0584  ...d.....t.d.d..
-00001420: 0074 057c 0364 0617 0083 0144 0083 0183  .t.|.d.....D....
-00001430: 0117 0064 0717 007d 0474 0683 006a 077c  ...d...}.t...j.|
-00001440: 017c 027c 0464 088d 0301 0064 0153 0029  .|.|.d.....d.S.)
-00001450: 09e1 0d02 0000 5465 6d70 6c61 7465 2066  ......Template f
-00001460: 6f72 2061 206d 6f64 656c 2077 6974 6820  or a model with 
-00001470: 6173 796d 6d65 7472 6963 206c 6f67 6973  asymmetric logis
-00001480: 7469 6320 7472 656e 6420 286d 7529 2061  tic trend (mu) a
-00001490: 6e64 2070 6f6c 796e 6f6d 6961 6c20 7363  nd polynomial sc
-000014a0: 616c 6520 2861 7320 6120 6675 6e63 7469  ale (as a functi
-000014b0: 6f6e 206f 6620 6d75 292e 0a0a 2020 2020  on of mu)...    
-000014c0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-000014d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-000014e0: 2d0a 2020 2020 2020 2020 696e 6465 7065  -.        indepe
-000014f0: 6e64 656e 745f 6b65 7920 3a20 7374 720a  ndent_key : str.
-00001500: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00001510: 206f 6620 7468 6520 696e 6465 7065 6e64   of the independ
-00001520: 656e 7420 7661 7269 6162 6c65 0a20 2020  ent variable.   
-00001530: 2020 2020 2064 6570 656e 6465 6e74 5f6b       dependent_k
-00001540: 6579 203a 2073 7472 0a20 2020 2020 2020  ey : str.       
-00001550: 2020 2020 206e 616d 6520 6f66 2074 6865       name of the
-00001560: 2064 6570 656e 6465 6e74 2076 6172 6961   dependent varia
-00001570: 626c 650a 2020 2020 2020 2020 7363 616c  ble.        scal
-00001580: 655f 6465 6772 6565 203a 206f 7074 696f  e_degree : optio
-00001590: 6e61 6c2c 2069 6e74 0a20 2020 2020 2020  nal, int.       
-000015a0: 2020 2020 2064 6567 7265 6520 6f66 2074       degree of t
-000015b0: 6865 2070 6f6c 796e 6f6d 6961 6c20 6d6f  he polynomial mo
-000015c0: 6465 6c20 6465 7363 7269 6269 6e67 2074  del describing t
-000015d0: 6865 2073 6361 6c65 2061 7320 6120 6675  he scale as a fu
-000015e0: 6e63 7469 6f6e 206f 6620 6d75 0a20 2020  nction of mu.   
-000015f0: 2020 2020 2074 6865 7461 5f6e 616d 6573       theta_names
-00001600: 203a 206f 7074 696f 6e61 6c2c 2074 7570   : optional, tup
-00001610: 6c65 206f 6620 7374 720a 2020 2020 2020  le of str.      
-00001620: 2020 2020 2020 6d61 7920 6265 2075 7365        may be use
-00001630: 6420 746f 2073 6574 2074 6865 206e 616d  d to set the nam
-00001640: 6573 206f 6620 7468 6520 6d6f 6465 6c20  es of the model 
-00001650: 7061 7261 6d65 7465 7273 0a20 2020 2020  parameters.     
-00001660: 2020 204e 7a0f 4c5f 4c2c 4c5f 552c 495f     Nz.L_L,L_U,I_
-00001670: 782c 532c 63fa 012c 6301 0000 0000 0000  x,S,c..,c.......
-00001680: 0000 0000 0002 0000 0003 0000 0073 0000  .............s..
-00001690: 0073 1800 0000 7c00 5d10 7d01 6400 7c01  .s....|.].}.d.|.
-000016a0: 9b00 9d02 5600 0100 7102 6401 5300 7229  ....V...q.d.S.r)
-000016b0: 0000 0072 1700 0000 7224 0000 0072 1700  ...r....r$...r..
-000016c0: 0000 7217 0000 0072 1800 0000 7227 0000  ..r....r....r'..
-000016d0: 0098 0000 0072 2800 0000 7a33 4261 7365  .....r(...z3Base
-000016e0: 4173 796d 6d65 7472 6963 4c6f 6769 7374  AsymmetricLogist
-000016f0: 6963 542e 5f5f 696e 6974 5f5f 2e3c 6c6f  icT.__init__.<lo
-00001700: 6361 6c73 3e2e 3c67 656e 6578 7072 3e72  cals>.<genexpr>r
-00001710: 0800 0000 722a 0000 00a9 0172 0e00 0000  ....r*.....r....
-00001720: a908 7207 0000 0072 2d00 0000 7221 0000  ..r....r-...r!..
-00001730: 0072 2e00 0000 da05 7370 6c69 7472 2f00  .r......splitr/.
-00001740: 0000 7212 0000 0072 1300 0000 a905 7214  ..r....r......r.
-00001750: 0000 0072 0c00 0000 720d 0000 0072 2100  ...r....r....r!.
-00001760: 0000 720e 0000 0072 1500 0000 7217 0000  ..r....r....r...
-00001770: 0072 1800 0000 7213 0000 007f 0000 0073  .r....r........s
-00001780: 1200 0000 0015 0c01 0802 0c01 18ff 0202  ................
-00001790: 02fe 02ff 0205 7a20 4261 7365 4173 796d  ......z BaseAsym
-000017a0: 6d65 7472 6963 4c6f 6769 7374 6963 542e  metricLogisticT.
-000017b0: 5f5f 696e 6974 5f5f 7230 0000 0063 0200  __init__r0...c..
-000017c0: 0000 0000 0000 0100 0000 0600 0000 0600  ................
-000017d0: 0000 4300 0000 735c 0000 007c 0264 0175  ..C...s\...|.d.u
-000017e0: 0072 0e7c 006a 007d 0274 01a0 027c 017c  .r.|.j.}.t...|.|
-000017f0: 0264 0164 0285 0219 00a1 027d 037c 006a  .d.d.......}.|.j
-00001800: 0364 036b 0272 367c 0264 0419 007d 046e  .d.k.r6|.d...}.n
-00001810: 1474 01a0 047c 037c 0264 0264 0585 0219  .t...|.|.d.d....
-00001820: 00a1 027d 047c 0264 0519 007d 057c 037c  ...}.|.d...}.|.|
-00001830: 047c 0566 0353 0029 0661 a303 0000 5072  .|.f.S.).a....Pr
-00001840: 6564 6963 7473 2074 6865 2070 6172 616d  edicts the param
-00001850: 6574 6572 7320 6d75 2061 6e64 2073 6361  eters mu and sca
-00001860: 6c65 206f 6620 6120 5374 7564 656e 742d  le of a Student-
-00001870: 7420 6469 7374 7269 6275 7469 6f6e 2077  t distribution w
-00001880: 6869 6368 0a20 2020 2020 2020 2063 6861  hich.        cha
-00001890: 7261 6374 6572 697a 6573 2074 6865 2064  racterizes the d
-000018a0: 6570 656e 6465 6e74 2076 6172 6961 626c  ependent variabl
-000018b0: 6520 6769 7665 6e20 7661 6c75 6573 206f  e given values o
-000018c0: 6620 7468 6520 696e 6465 7065 6e64 656e  f the independen
-000018d0: 7420 7661 7269 6162 6c65 2e0a 0a20 2020  t variable...   
-000018e0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-000018f0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00001900: 2d2d 0a20 2020 2020 2020 2078 203a 2061  --.        x : a
-00001910: 7272 6179 2d6c 696b 650a 2020 2020 2020  rray-like.      
-00001920: 2020 2020 2020 7661 6c75 6573 206f 6620        values of 
-00001930: 7468 6520 696e 6465 7065 6e64 656e 7420  the independent 
-00001940: 7661 7269 6162 6c65 0a20 2020 2020 2020  variable.       
-00001950: 2074 6865 7461 203a 206f 7074 696f 6e61   theta : optiona
-00001960: 6c2c 2061 7272 6179 2d6c 696b 650a 2020  l, array-like.  
-00001970: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
-00001980: 7465 7220 7665 6374 6f72 206f 6620 7468  ter vector of th
-00001990: 6520 6361 6c69 6272 6174 696f 6e20 6d6f  e calibration mo
-000019a0: 6465 6c3a 0a20 2020 2020 2020 2020 2020  del:.           
-000019b0: 2020 2020 2035 2070 6172 616d 6574 6572       5 parameter
-000019c0: 7320 6f66 2061 7379 6d6d 6574 7269 6320  s of asymmetric 
-000019d0: 6c6f 6769 7374 6963 206d 6f64 656c 2066  logistic model f
-000019e0: 6f72 206d 750a 2020 2020 2020 2020 2020  or mu.          
-000019f0: 2020 2020 2020 5b73 6361 6c65 5f64 6567        [scale_deg
-00001a00: 7265 655d 2070 6172 616d 6574 6572 7320  ree] parameters 
-00001a10: 666f 7220 7363 616c 6520 286c 6f77 6573  for scale (lowes
-00001a20: 7420 6465 6772 6565 2066 6972 7374 290a  t degree first).
-00001a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a40: 3120 7061 7261 6d65 7465 7220 666f 7220  1 parameter for 
-00001a50: 6465 6772 6565 206f 6620 6672 6565 646f  degree of freedo
-00001a60: 6d0a 0a20 2020 2020 2020 2052 6574 7572  m..        Retur
-00001a70: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00001a80: 2d2d 0a20 2020 2020 2020 206d 7520 3a20  --.        mu : 
-00001a90: 6172 7261 792d 6c69 6b65 0a20 2020 2020  array-like.     
-00001aa0: 2020 2020 2020 2076 616c 7565 7320 666f         values fo
-00001ab0: 7220 7468 6520 6d75 2070 6172 616d 6574  r the mu paramet
-00001ac0: 6572 206f 6620 6120 5374 7564 656e 742d  er of a Student-
-00001ad0: 7420 6469 7374 7269 6275 7469 6f6e 2064  t distribution d
-00001ae0: 6573 6372 6962 696e 6720 7468 6520 6465  escribing the de
-00001af0: 7065 6e64 656e 7420 7661 7269 6162 6c65  pendent variable
-00001b00: 0a20 2020 2020 2020 2073 6361 6c65 203a  .        scale :
-00001b10: 2061 7272 6179 2d6c 696b 6520 6f72 2066   array-like or f
-00001b20: 6c6f 6174 0a20 2020 2020 2020 2020 2020  loat.           
-00001b30: 2076 616c 7565 7320 666f 7220 7468 6520   values for the 
-00001b40: 7363 616c 6520 7061 7261 6d65 7465 7220  scale parameter 
-00001b50: 6f66 2061 2053 7475 6465 6e74 2d74 2064  of a Student-t d
-00001b60: 6973 7472 6962 7574 696f 6e20 6465 7363  istribution desc
-00001b70: 7269 6269 6e67 2074 6865 2064 6570 656e  ribing the depen
-00001b80: 6465 6e74 2076 6172 6961 626c 650a 2020  dent variable.  
-00001b90: 2020 2020 2020 6466 203a 2066 6c6f 6174        df : float
-00001ba0: 0a20 2020 2020 2020 2020 2020 2064 6567  .            deg
-00001bb0: 7265 6520 6f66 2066 7265 6564 6f6d 206f  ree of freedom o
-00001bc0: 6620 5374 7564 656e 742d 7420 6469 7374  f Student-t dist
-00001bd0: 7269 6275 7469 6f6e 0a20 2020 2020 2020  ribution.       
-00001be0: 204e e905 0000 0072 0100 0000 7232 0000   N.....r....r2..
-00001bf0: 0072 3300 0000 2905 7234 0000 0072 0600  .r3...).r4...r..
-00001c00: 0000 da13 6173 796d 6d65 7472 6963 5f6c  ....asymmetric_l
-00001c10: 6f67 6973 7469 6372 2100 0000 7235 0000  ogisticr!...r5..
-00001c20: 0072 3600 0000 7217 0000 0072 1700 0000  .r6...r....r....
-00001c30: 7218 0000 0072 3a00 0000 9d00 0000 7310  r....r:.......s.
-00001c40: 0000 0000 1708 0106 0114 010a 010a 0214  ................
-00001c50: 0108 017a 2942 6173 6541 7379 6d6d 6574  ...z)BaseAsymmet
-00001c60: 7269 634c 6f67 6973 7469 6354 2e70 7265  ricLogisticT.pre
-00001c70: 6469 6374 5f64 6570 656e 6465 6e74 6302  dict_dependentc.
-00001c80: 0000 0000 0000 0001 0000 0003 0000 0006  ................
-00001c90: 0000 0043 0000 0073 2200 0000 7c02 6401  ...C...s"...|.d.
-00001ca0: 7500 720e 7c00 6a00 7d02 7401 a002 7c01  u.r.|.j.}.t...|.
-00001cb0: 7c02 6401 6402 8502 1900 a102 5300 2903  |.d.d.......S.).
-00001cc0: 6131 0200 0050 7265 6469 6374 2074 6865  a1...Predict the
-00001cd0: 2069 6e64 6570 656e 6465 6e74 2076 6172   independent var
-00001ce0: 6961 626c 6520 7573 696e 6720 7468 6520  iable using the 
-00001cf0: 696e 7665 7273 6520 7472 656e 6420 6d6f  inverse trend mo
-00001d00: 6465 6c2e 0a0a 2020 2020 2020 2020 5061  del...        Pa
-00001d10: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00001d20: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00001d30: 2020 2020 7920 3a20 6172 7261 792d 6c69      y : array-li
-00001d40: 6b65 0a20 2020 2020 2020 2020 2020 206f  ke.            o
-00001d50: 6273 6572 7661 7469 6f6e 730a 2020 2020  bservations.    
-00001d60: 2020 2020 2074 6865 7461 203a 206f 7074       theta : opt
-00001d70: 696f 6e61 6c2c 2061 7272 6179 2d6c 696b  ional, array-lik
-00001d80: 650a 2020 2020 2020 2020 2020 2020 7061  e.            pa
-00001d90: 7261 6d65 7465 7220 7665 6374 6f72 206f  rameter vector o
-00001da0: 6620 7468 6520 6361 6c69 6272 6174 696f  f the calibratio
-00001db0: 6e20 6d6f 6465 6c3a 0a20 2020 2020 2020  n model:.       
-00001dc0: 2020 2020 2020 2020 2035 2070 6172 616d           5 param
-00001dd0: 6574 6572 7320 6f66 2061 7379 6d6d 6574  eters of asymmet
-00001de0: 7269 6320 6c6f 6769 7374 6963 206d 6f64  ric logistic mod
-00001df0: 656c 2066 6f72 206d 750a 2020 2020 2020  el for mu.      
-00001e00: 2020 2020 2020 2020 2020 5b73 6361 6c65            [scale
-00001e10: 5f64 6567 7265 655d 2070 6172 616d 6574  _degree] paramet
-00001e20: 6572 7320 666f 7220 7363 616c 6520 286c  ers for scale (l
-00001e30: 6f77 6573 7420 6465 6772 6565 2066 6972  owest degree fir
-00001e40: 7374 290a 2020 2020 2020 2020 2020 2020  st).            
-00001e50: 2020 2020 3120 7061 7261 6d65 7465 7220      1 parameter 
-00001e60: 666f 7220 6465 6772 6565 206f 6620 6672  for degree of fr
-00001e70: 6565 646f 6d0a 0a20 2020 2020 2020 2052  eedom..        R
-00001e80: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00001e90: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
-00001ea0: 203a 2061 7272 6179 2d6c 696b 650a 2020   : array-like.  
-00001eb0: 2020 2020 2020 2020 2020 7072 6564 6963            predic
-00001ec0: 7465 6420 696e 6465 7065 6e64 656e 7420  ted independent 
-00001ed0: 7661 6c75 6573 2067 6976 656e 2074 6865  values given the
-00001ee0: 206f 6273 6572 7661 7469 6f6e 730a 2020   observations.  
-00001ef0: 2020 2020 2020 4e72 4a00 0000 2903 7234        NrJ...).r4
-00001f00: 0000 0072 0600 0000 da1b 696e 7665 7273  ...r......invers
-00001f10: 655f 6173 796d 6d65 7472 6963 5f6c 6f67  e_asymmetric_log
-00001f20: 6973 7469 63a9 0372 1400 0000 723c 0000  istic..r....r<..
-00001f30: 0072 3100 0000 7217 0000 0072 1700 0000  .r1...r....r....
-00001f40: 7218 0000 0072 3f00 0000 be00 0000 7306  r....r?.......s.
-00001f50: 0000 0000 1208 0106 017a 2b42 6173 6541  .........z+BaseA
-00001f60: 7379 6d6d 6574 7269 634c 6f67 6973 7469  symmetricLogisti
-00001f70: 6354 2e70 7265 6469 6374 5f69 6e64 6570  cT.predict_indep
-00001f80: 656e 6465 6e74 7240 0000 0072 1700 0000  endentr@...r....
-00001f90: 7217 0000 0072 1500 0000 7218 0000 0072  r....r....r....r
-00001fa0: 4200 0000 7e00 0000 7314 0000 0008 0602  B...~...s.......
-00001fb0: 0102 fa04 0302 0102 0102 010a fa10 1e0e  ................
-00001fc0: 2172 4200 0000 6300 0000 0000 0000 0000  !rB...c.........
-00001fd0: 0000 0000 0000 0007 0000 0000 0000 0073  ...............s
-00001fe0: 5400 0000 6500 5a01 6400 5a02 6401 6402  T...e.Z.d.Z.d.d.
-00001ff0: 6403 9c02 6503 6503 6504 6505 6506 6503  d...e.e.e.e.e.e.
-00002000: 1900 1900 6404 9c04 8700 6601 6405 6406  ....d.....f.d.d.
-00002010: 840e 5a07 6402 6407 9c01 6408 6409 8402  ..Z.d.d...d.d...
-00002020: 5a08 6402 6407 9c01 640a 640b 8402 5a09  Z.d.d...d.d...Z.
-00002030: 8700 0400 5a0a 5300 290c da25 4261 7365  ....Z.S.)..%Base
-00002040: 4c6f 6749 6e64 6570 656e 6465 6e74 4173  LogIndependentAs
-00002050: 796d 6d65 7472 6963 4c6f 6769 7374 6963  ymmetricLogistic
-00002060: 5472 0100 0000 4e72 2000 0000 7243 0000  Tr....Nr ...rC..
-00002070: 0063 0100 0000 0000 0000 0400 0000 0500  .c..............
-00002080: 0000 0600 0000 0300 0000 7356 0000 0074  ..........sV...t
-00002090: 00a0 017c 03a1 017c 005f 027c 0464 0175  ...|...|._.|.d.u
-000020a0: 0072 4074 0364 02a0 0464 03a1 0183 0174  .r@t.d...d.....t
-000020b0: 0364 0464 0584 0074 057c 0364 0617 0083  .d.d...t.|.d....
-000020c0: 0144 0083 0183 0117 0064 0717 007d 0474  .D.......d...}.t
-000020d0: 0683 006a 077c 017c 027c 0464 088d 0301  ...j.|.|.|.d....
-000020e0: 0064 0153 0029 0972 4400 0000 4e7a 134c  .d.S.).rD...Nz.L
-000020f0: 5f4c 2c4c 5f55 2c6c 6f67 5f49 5f78 2c53  _L,L_U,log_I_x,S
-00002100: 2c63 7245 0000 0063 0100 0000 0000 0000  ,crE...c........
-00002110: 0000 0000 0200 0000 0300 0000 7300 0000  ............s...
-00002120: 7318 0000 007c 005d 107d 0164 007c 019b  s....|.].}.d.|..
-00002130: 009d 0256 0001 0071 0264 0153 0072 2900  ...V...q.d.S.r).
-00002140: 0000 7217 0000 0072 2400 0000 7217 0000  ..r....r$...r...
-00002150: 0072 1700 0000 7218 0000 0072 2700 0000  .r....r....r'...
-00002160: ef00 0000 7228 0000 007a 4142 6173 654c  ....r(...zABaseL
-00002170: 6f67 496e 6465 7065 6e64 656e 7441 7379  ogIndependentAsy
-00002180: 6d6d 6574 7269 634c 6f67 6973 7469 6354  mmetricLogisticT
-00002190: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
-000021a0: 733e 2e3c 6765 6e65 7870 723e 7208 0000  s>.<genexpr>r...
-000021b0: 0072 2a00 0000 7246 0000 0072 4700 0000  .r*...rF...rG...
-000021c0: 7249 0000 0072 1500 0000 7217 0000 0072  rI...r....r....r
-000021d0: 1800 0000 7213 0000 00d6 0000 0073 1200  ....r........s..
-000021e0: 0000 0015 0c01 0802 0c01 18ff 0202 02fe  ................
-000021f0: 02ff 0205 7a2e 4261 7365 4c6f 6749 6e64  ....z.BaseLogInd
-00002200: 6570 656e 6465 6e74 4173 796d 6d65 7472  ependentAsymmetr
-00002210: 6963 4c6f 6769 7374 6963 542e 5f5f 696e  icLogisticT.__in
-00002220: 6974 5f5f 7230 0000 0063 0200 0000 0000  it__r0...c......
-00002230: 0000 0100 0000 0600 0000 0600 0000 4300  ..............C.
-00002240: 0000 735c 0000 007c 0264 0175 0072 0e7c  ..s\...|.d.u.r.|
-00002250: 006a 007d 0274 01a0 027c 017c 0264 0164  .j.}.t...|.|.d.d
-00002260: 0285 0219 00a1 027d 037c 006a 0364 036b  .......}.|.j.d.k
-00002270: 0272 367c 0264 0419 007d 046e 1474 01a0  .r6|.d...}.n.t..
-00002280: 047c 037c 0264 0264 0585 0219 00a1 027d  .|.|.d.d.......}
-00002290: 047c 0264 0519 007d 057c 037c 047c 0566  .|.d...}.|.|.|.f
-000022a0: 0353 0029 0661 b303 0000 5072 6564 6963  .S.).a....Predic
-000022b0: 7473 2074 6865 2070 6172 616d 6574 6572  ts the parameter
-000022c0: 7320 6d75 2061 6e64 2073 6361 6c65 206f  s mu and scale o
-000022d0: 6620 6120 5374 7564 656e 742d 7420 6469  f a Student-t di
-000022e0: 7374 7269 6275 7469 6f6e 2077 6869 6368  stribution which
-000022f0: 0a20 2020 2020 2020 2063 6861 7261 6374  .        charact
-00002300: 6572 697a 6573 2074 6865 2064 6570 656e  erizes the depen
-00002310: 6465 6e74 2076 6172 6961 626c 6520 6769  dent variable gi
-00002320: 7665 6e20 7661 6c75 6573 206f 6620 7468  ven values of th
-00002330: 6520 696e 6465 7065 6e64 656e 7420 7661  e independent va
-00002340: 7269 6162 6c65 2e0a 0a20 2020 2020 2020  riable...       
-00002350: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00002360: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00002370: 2020 2020 2020 2078 203a 2061 7272 6179         x : array
-00002380: 2d6c 696b 650a 2020 2020 2020 2020 2020  -like.          
-00002390: 2020 7661 6c75 6573 206f 6620 7468 6520    values of the 
-000023a0: 696e 6465 7065 6e64 656e 7420 7661 7269  independent vari
-000023b0: 6162 6c65 0a20 2020 2020 2020 2074 6865  able.        the
-000023c0: 7461 203a 206f 7074 696f 6e61 6c2c 2061  ta : optional, a
-000023d0: 7272 6179 2d6c 696b 650a 2020 2020 2020  rray-like.      
-000023e0: 2020 2020 2020 7061 7261 6d65 7465 7220        parameter 
-000023f0: 7665 6374 6f72 206f 6620 7468 6520 6361  vector of the ca
-00002400: 6c69 6272 6174 696f 6e20 6d6f 6465 6c3a  libration model:
-00002410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002420: 2035 2070 6172 616d 6574 6572 7320 6f66   5 parameters of
-00002430: 206c 6f67 2d69 6e64 6570 656e 6465 6e74   log-independent
-00002440: 2061 7379 6d6d 6574 7269 6320 6c6f 6769   asymmetric logi
-00002450: 7374 6963 206d 6f64 656c 2066 6f72 206d  stic model for m
-00002460: 750a 2020 2020 2020 2020 2020 2020 2020  u.              
-00002470: 2020 5b73 6361 6c65 5f64 6567 7265 655d    [scale_degree]
-00002480: 2070 6172 616d 6574 6572 7320 666f 7220   parameters for 
-00002490: 7363 616c 6520 286c 6f77 6573 7420 6465  scale (lowest de
-000024a0: 6772 6565 2066 6972 7374 290a 2020 2020  gree first).    
-000024b0: 2020 2020 2020 2020 2020 2020 3120 7061              1 pa
-000024c0: 7261 6d65 7465 7220 666f 7220 6465 6772  rameter for degr
-000024d0: 6565 206f 6620 6672 6565 646f 6d0a 0a20  ee of freedom.. 
-000024e0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-000024f0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00002500: 2020 2020 2020 206d 7520 3a20 6172 7261         mu : arra
-00002510: 792d 6c69 6b65 0a20 2020 2020 2020 2020  y-like.         
-00002520: 2020 2076 616c 7565 7320 666f 7220 7468     values for th
-00002530: 6520 6d75 2070 6172 616d 6574 6572 206f  e mu parameter o
-00002540: 6620 6120 5374 7564 656e 742d 7420 6469  f a Student-t di
-00002550: 7374 7269 6275 7469 6f6e 2064 6573 6372  stribution descr
-00002560: 6962 696e 6720 7468 6520 6465 7065 6e64  ibing the depend
-00002570: 656e 7420 7661 7269 6162 6c65 0a20 2020  ent variable.   
-00002580: 2020 2020 2073 6361 6c65 203a 2061 7272       scale : arr
-00002590: 6179 2d6c 696b 6520 6f72 2066 6c6f 6174  ay-like or float
-000025a0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-000025b0: 7565 7320 666f 7220 7468 6520 7363 616c  ues for the scal
-000025c0: 6520 7061 7261 6d65 7465 7220 6f66 2061  e parameter of a
-000025d0: 2053 7475 6465 6e74 2d74 2064 6973 7472   Student-t distr
-000025e0: 6962 7574 696f 6e20 6465 7363 7269 6269  ibution describi
-000025f0: 6e67 2074 6865 2064 6570 656e 6465 6e74  ng the dependent
-00002600: 2076 6172 6961 626c 650a 2020 2020 2020   variable.      
-00002610: 2020 6466 203a 2066 6c6f 6174 0a20 2020    df : float.   
-00002620: 2020 2020 2020 2020 2064 6567 7265 6520           degree 
-00002630: 6f66 2066 7265 6564 6f6d 206f 6620 5374  of freedom of St
-00002640: 7564 656e 742d 7420 6469 7374 7269 6275  udent-t distribu
-00002650: 7469 6f6e 0a20 2020 2020 2020 204e 724a  tion.        NrJ
-00002660: 0000 0072 0100 0000 7232 0000 0072 3300  ...r....r2...r3.
-00002670: 0000 2905 7234 0000 0072 0600 0000 da18  ..).r4...r......
-00002680: 786c 6f67 5f61 7379 6d6d 6574 7269 635f  xlog_asymmetric_
-00002690: 6c6f 6769 7374 6963 7221 0000 0072 3500  logisticr!...r5.
-000026a0: 0000 7236 0000 0072 1700 0000 7217 0000  ..r6...r....r...
-000026b0: 0072 1800 0000 723a 0000 00f4 0000 0073  .r....r:.......s
-000026c0: 1000 0000 0017 0801 0601 1401 0a01 0a02  ................
-000026d0: 1401 0801 7a37 4261 7365 4c6f 6749 6e64  ....z7BaseLogInd
-000026e0: 6570 656e 6465 6e74 4173 796d 6d65 7472  ependentAsymmetr
-000026f0: 6963 4c6f 6769 7374 6963 542e 7072 6564  icLogisticT.pred
-00002700: 6963 745f 6465 7065 6e64 656e 7463 0200  ict_dependentc..
-00002710: 0000 0000 0000 0100 0000 0300 0000 0600  ................
-00002720: 0000 4300 0000 7322 0000 007c 0264 0175  ..C...s"...|.d.u
-00002730: 0072 0e7c 006a 007d 0274 01a0 027c 017c  .r.|.j.}.t...|.|
-00002740: 0264 0164 0285 0219 00a1 0253 0029 0361  .d.d.......S.).a
-00002750: 4002 0000 5072 6564 6963 7420 7468 6520  @...Predict the 
-00002760: 696e 6465 7065 6e64 656e 7420 7661 7269  independent vari
-00002770: 6162 6c65 2075 7369 6e67 2074 6865 2069  able using the i
-00002780: 6e76 6572 7365 2074 7265 6e64 206d 6f64  nverse trend mod
-00002790: 656c 2e0a 0a20 2020 2020 2020 2050 6172  el...        Par
-000027a0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-000027b0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-000027c0: 2020 2079 203a 2061 7272 6179 2d6c 696b     y : array-lik
-000027d0: 650a 2020 2020 2020 2020 2020 2020 6f62  e.            ob
-000027e0: 7365 7276 6174 696f 6e73 0a20 2020 2020  servations.     
-000027f0: 2020 2074 6865 7461 203a 206f 7074 696f     theta : optio
-00002800: 6e61 6c2c 2061 7272 6179 2d6c 696b 650a  nal, array-like.
-00002810: 2020 2020 2020 2020 2020 2020 7061 7261              para
-00002820: 6d65 7465 7220 7665 6374 6f72 206f 6620  meter vector of 
-00002830: 7468 6520 6361 6c69 6272 6174 696f 6e20  the calibration 
-00002840: 6d6f 6465 6c3a 0a20 2020 2020 2020 2020  model:.         
-00002850: 2020 2020 2020 2035 2070 6172 616d 6574         5 paramet
-00002860: 6572 7320 6f66 206c 6f67 2d69 6e64 6570  ers of log-indep
-00002870: 656e 6465 6e74 2061 7379 6d6d 6574 7269  endent asymmetri
-00002880: 6320 6c6f 6769 7374 6963 206d 6f64 656c  c logistic model
-00002890: 2066 6f72 206d 750a 2020 2020 2020 2020   for mu.        
-000028a0: 2020 2020 2020 2020 5b73 6361 6c65 5f64          [scale_d
-000028b0: 6567 7265 655d 2070 6172 616d 6574 6572  egree] parameter
-000028c0: 7320 666f 7220 7363 616c 6520 286c 6f77  s for scale (low
-000028d0: 6573 7420 6465 6772 6565 2066 6972 7374  est degree first
-000028e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000028f0: 2020 3120 7061 7261 6d65 7465 7220 666f    1 parameter fo
-00002900: 7220 6465 6772 6565 206f 6620 6672 6565  r degree of free
-00002910: 646f 6d0a 0a20 2020 2020 2020 2052 6574  dom..        Ret
-00002920: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00002930: 2d2d 2d2d 0a20 2020 2020 2020 2078 203a  ----.        x :
-00002940: 2061 7272 6179 2d6c 696b 650a 2020 2020   array-like.    
-00002950: 2020 2020 2020 2020 7072 6564 6963 7465          predicte
-00002960: 6420 696e 6465 7065 6e64 656e 7420 7661  d independent va
-00002970: 6c75 6573 2067 6976 656e 2074 6865 206f  lues given the o
-00002980: 6273 6572 7661 7469 6f6e 730a 2020 2020  bservations.    
-00002990: 2020 2020 4e72 4a00 0000 2903 7234 0000      NrJ...).r4..
-000029a0: 0072 0600 0000 da20 696e 7665 7273 655f  .r..... inverse_
-000029b0: 786c 6f67 5f61 7379 6d6d 6574 7269 635f  xlog_asymmetric_
-000029c0: 6c6f 6769 7374 6963 724d 0000 0072 1700  logisticrM...r..
-000029d0: 0000 7217 0000 0072 1800 0000 723f 0000  ..r....r....r?..
-000029e0: 0015 0100 0073 0600 0000 0012 0801 0601  .....s..........
-000029f0: 7a39 4261 7365 4c6f 6749 6e64 6570 656e  z9BaseLogIndepen
-00002a00: 6465 6e74 4173 796d 6d65 7472 6963 4c6f  dentAsymmetricLo
-00002a10: 6769 7374 6963 542e 7072 6564 6963 745f  gisticT.predict_
-00002a20: 696e 6465 7065 6e64 656e 7472 4000 0000  independentr@...
-00002a30: 7217 0000 0072 1700 0000 7215 0000 0072  r....r....r....r
-00002a40: 1800 0000 724e 0000 00d5 0000 0073 1400  ....rN.......s..
-00002a50: 0000 0806 0201 02fa 0403 0201 0201 0201  ................
-00002a60: 0afa 101e 0e21 724e 0000 0063 0000 0000  .....!rN...c....
-00002a70: 0000 0000 0000 0000 0000 0000 0800 0000  ................
-00002a80: 0000 0000 735c 0000 0065 005a 0164 005a  ....s\...e.Z.d.Z
-00002a90: 0264 0164 0264 0264 039c 0365 0365 0365  .d.d.d.d...e.e.e
-00002aa0: 0465 0565 0619 0065 0565 0765 0319 0019  .e.e...e.e.e....
-00002ab0: 0064 049c 0587 0066 0164 0564 0684 0e5a  .d.....f.d.d...Z
-00002ac0: 0864 0264 079c 0164 0864 0984 025a 0964  .d.d...d.d...Z.d
-00002ad0: 0264 079c 0164 0a64 0b84 025a 0a87 0004  .d...d.d...Z....
-00002ae0: 005a 0b53 0029 0cda 1542 6173 6545 7870  .Z.S.)...BaseExp
-00002af0: 6f6e 656e 7469 616c 4d6f 6465 6c54 7201  onentialModelTr.
-00002b00: 0000 004e 2903 7221 0000 00da 0f66 6978  ...N).r!.....fix
-00002b10: 6564 5f69 6e74 6572 6365 7074 720e 0000  ed_interceptr...
-00002b20: 0029 0572 0c00 0000 720d 0000 0072 2100  .).r....r....r!.
-00002b30: 0000 7252 0000 0072 0e00 0000 6301 0000  ..rR...r....c...
-00002b40: 0000 0000 0005 0000 0007 0000 0006 0000  ................
-00002b50: 0003 0000 0073 6400 0000 7400 a001 7c03  .....sd...t...|.
-00002b60: a101 7c00 5f02 7c04 7c00 5f03 7c05 6401  ..|._.|.|._.|.d.
-00002b70: 7500 724e 7c04 6401 7501 7228 6402 7d06  u.rN|.d.u.r(d.}.
-00002b80: 6e04 6403 7d06 7c06 7404 6404 6405 8400  n.d.}.|.t.d.d...
-00002b90: 7405 7c03 6406 1700 8301 4400 8301 8301  t.|.d.....D.....
-00002ba0: 1700 6407 1700 7d05 7406 8300 6a07 7c01  ..d...}.t...j.|.
-00002bb0: 7c02 7c05 6408 8d03 0100 6401 5300 2909  |.|.d.....d.S.).
-00002bc0: 750e 0300 0054 656d 706c 6174 6520 666f  u....Template fo
-00002bd0: 7220 6120 6d6f 6465 6c20 7769 7468 2065  r a model with e
-00002be0: 7870 6f6e 656e 7469 616c 2074 7265 6e64  xponential trend
-00002bf0: 2028 6d75 2920 616e 6420 706f 6c79 6e6f   (mu) and polyno
-00002c00: 6d69 616c 2073 6361 6c65 2028 6173 2061  mial scale (as a
-00002c10: 2066 756e 6374 696f 6e20 6f66 206d 7529   function of mu)
-00002c20: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00002c30: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00002c40: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00002c50: 2069 6e64 6570 656e 6465 6e74 5f6b 6579   independent_key
-00002c60: 203a 2073 7472 0a20 2020 2020 2020 2020   : str.         
-00002c70: 2020 204e 616d 6520 6f66 2074 6865 2069     Name of the i
-00002c80: 6e64 6570 656e 6465 6e74 2076 6172 6961  ndependent varia
-00002c90: 626c 652e 0a20 2020 2020 2020 2064 6570  ble..        dep
-00002ca0: 656e 6465 6e74 5f6b 6579 203a 2073 7472  endent_key : str
-00002cb0: 0a20 2020 2020 2020 2020 2020 204e 616d  .            Nam
-00002cc0: 6520 6f66 2074 6865 2064 6570 656e 6465  e of the depende
-00002cd0: 6e74 2076 6172 6961 626c 652e 0a20 2020  nt variable..   
-00002ce0: 2020 2020 2073 6361 6c65 5f64 6567 7265       scale_degre
-00002cf0: 6520 3a20 6f70 7469 6f6e 616c 2c20 696e  e : optional, in
-00002d00: 740a 2020 2020 2020 2020 2020 2020 4465  t.            De
-00002d10: 6772 6565 206f 6620 7468 6520 706f 6c79  gree of the poly
-00002d20: 6e6f 6d69 616c 206d 6f64 656c 2064 6573  nomial model des
-00002d30: 6372 6962 696e 6720 7468 6520 7363 616c  cribing the scal
-00002d40: 6520 6173 2061 2066 756e 6374 696f 6e20  e as a function 
-00002d50: 6f66 206d 752e 0a20 2020 2020 2020 2020  of mu..         
-00002d60: 2020 20e2 9aa0 2041 7474 656e 7469 6f6e     ... Attention
-00002d70: 3a20 666f 7220 7363 616c 655f 6465 6772  : for scale_degr
-00002d80: 6565 203e 2030 2c20 656e 7375 7265 2074  ee > 0, ensure t
-00002d90: 6861 7420 7363 616c 6520 6973 2061 6c77  hat scale is alw
-00002da0: 6179 7320 706f 7369 7469 7665 210a 2020  ays positive!.  
-00002db0: 2020 2020 2020 6669 7865 645f 696e 7465        fixed_inte
-00002dc0: 7263 6570 7420 3a20 6f70 7469 6f6e 616c  rcept : optional
-00002dd0: 2c20 666c 6f61 740a 2020 2020 2020 2020  , float.        
-00002de0: 2020 2020 4966 2073 6574 2c20 7468 6520      If set, the 
-00002df0: 792d 6178 6973 2069 6e74 6572 6365 7074  y-axis intercept
-00002e00: 2077 696c 6c20 6265 2066 6978 6564 2074   will be fixed t
-00002e10: 6f20 7468 6973 2076 616c 7565 2e0a 2020  o this value..  
-00002e20: 2020 2020 2020 2020 2020 4f74 6865 7277            Otherw
-00002e30: 6973 6520 7468 6520 696e 7465 7263 6570  ise the intercep
-00002e40: 7420 6265 636f 6d65 7320 6120 6672 6565  t becomes a free
-00002e50: 2070 6172 616d 6574 6572 2e0a 2020 2020   parameter..    
-00002e60: 2020 2020 7468 6574 615f 6e61 6d65 7320      theta_names 
-00002e70: 3a20 6f70 7469 6f6e 616c 2c20 7475 706c  : optional, tupl
-00002e80: 6520 6f66 2073 7472 0a20 2020 2020 2020  e of str.       
-00002e90: 2020 2020 204d 6179 2062 6520 7573 6564       May be used
-00002ea0: 2074 6f20 7365 7420 7468 6520 6e61 6d65   to set the name
-00002eb0: 7320 6f66 2074 6865 206d 6f64 656c 2070  s of the model p
-00002ec0: 6172 616d 6574 6572 732e 0a20 2020 2020  arameters..     
-00002ed0: 2020 204e 2902 da01 4cda 016b 2903 da01     N)...L..k)...
-00002ee0: 4972 5300 0000 7254 0000 0063 0100 0000  IrS...rT...c....
-00002ef0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00002f00: 7300 0000 7318 0000 007c 005d 107d 0164  s...s....|.].}.d
-00002f10: 007c 019b 009d 0256 0001 0071 0264 0153  .|.....V...q.d.S
-00002f20: 0072 2900 0000 7217 0000 0072 2400 0000  .r)...r....r$...
-00002f30: 7217 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-00002f40: 2700 0000 4f01 0000 7228 0000 007a 3142  '...O...r(...z1B
-00002f50: 6173 6545 7870 6f6e 656e 7469 616c 4d6f  aseExponentialMo
-00002f60: 6465 6c54 2e5f 5f69 6e69 745f 5f2e 3c6c  delT.__init__.<l
-00002f70: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
-00002f80: 7208 0000 0072 2a00 0000 7246 0000 0029  r....r*...rF...)
-00002f90: 0872 0700 0000 722d 0000 0072 2100 0000  .r....r-...r!...
-00002fa0: 7252 0000 0072 2e00 0000 722f 0000 0072  rR...r....r/...r
-00002fb0: 1200 0000 7213 0000 0029 0772 1400 0000  ....r....).r....
-00002fc0: 720c 0000 0072 0d00 0000 7221 0000 0072  r....r....r!...r
-00002fd0: 5200 0000 720e 0000 00da 0674 6e61 6d65  R...r......tname
-00002fe0: 7372 1500 0000 7217 0000 0072 1800 0000  sr....r....r....
-00002ff0: 7213 0000 002d 0100 0073 1000 0000 001a  r....-...s......
-00003000: 0c01 0601 0802 0801 0602 0401 2201 7a1e  ............".z.
-00003010: 4261 7365 4578 706f 6e65 6e74 6961 6c4d  BaseExponentialM
-00003020: 6f64 656c 542e 5f5f 696e 6974 5f5f 7230  odelT.__init__r0
-00003030: 0000 0063 0200 0000 0000 0000 0100 0000  ...c............
-00003040: 0800 0000 0400 0000 4300 0000 73b0 0000  ........C...s...
-00003050: 007c 0264 0175 0072 0e7c 006a 007d 027c  .|.d.u.r.|.j.}.|
-00003060: 006a 0164 0175 0072 3c7c 0264 0219 007c  .j.d.u.r<|.d...|
-00003070: 0264 0319 007c 0264 0419 0066 037d 037c  .d...|.d...f.}.|
-00003080: 0264 0564 0685 0219 007d 046e 207c 006a  .d.d.....}.n |.j
-00003090: 017c 0264 0219 007c 0264 0319 0066 037d  .|.d...|.d...f.}
-000030a0: 037c 0264 0464 0685 0219 007d 0474 027c  .|.d.d.....}.t.|
-000030b0: 0483 017c 006a 0364 0317 006b 0273 724a  ...|.j.d...k.srJ
-000030c0: 0082 0174 04a0 057c 017c 03a1 027d 057c  ...t...|.|...}.|
-000030d0: 006a 0364 026b 0272 927c 0264 0719 007d  .j.d.k.r.|.d...}
-000030e0: 066e 0c74 04a0 067c 057c 04a1 027d 067c  .n.t...|.|...}.|
-000030f0: 0264 0619 007d 077c 057c 067c 0766 0353  .d...}.|.|.|.f.S
-00003100: 0029 0861 0004 0000 5072 6564 6963 7473  .).a....Predicts
-00003110: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
-00003120: 6d75 2061 6e64 2073 6361 6c65 206f 6620  mu and scale of 
-00003130: 6120 5374 7564 656e 742d 7420 6469 7374  a Student-t dist
-00003140: 7269 6275 7469 6f6e 2077 6869 6368 0a20  ribution which. 
-00003150: 2020 2020 2020 2063 6861 7261 6374 6572         character
-00003160: 697a 6573 2074 6865 2064 6570 656e 6465  izes the depende
-00003170: 6e74 2076 6172 6961 626c 6520 6769 7665  nt variable give
-00003180: 6e20 7661 6c75 6573 206f 6620 7468 6520  n values of the 
-00003190: 696e 6465 7065 6e64 656e 7420 7661 7269  independent vari
-000031a0: 6162 6c65 2e0a 0a20 2020 2020 2020 2050  able...        P
-000031b0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-000031c0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-000031d0: 2020 2020 2078 203a 2061 7272 6179 2d6c       x : array-l
-000031e0: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
-000031f0: 5661 6c75 6573 206f 6620 7468 6520 696e  Values of the in
-00003200: 6465 7065 6e64 656e 7420 7661 7269 6162  dependent variab
-00003210: 6c65 2e0a 2020 2020 2020 2020 7468 6574  le..        thet
-00003220: 6120 3a20 6f70 7469 6f6e 616c 2c20 6172  a : optional, ar
-00003230: 7261 792d 6c69 6b65 0a20 2020 2020 2020  ray-like.       
-00003240: 2020 2020 2050 6172 616d 6574 6572 2076       Parameter v
-00003250: 6563 746f 7220 6f66 2074 6865 2063 616c  ector of the cal
-00003260: 6962 7261 7469 6f6e 206d 6f64 656c 2e0a  ibration model..
-00003270: 2020 2020 2020 2020 2020 2020 4465 7065              Depe
-00003280: 6e64 696e 6720 6f6e 2074 6865 2060 6066  nding on the ``f
-00003290: 6978 6564 5f69 6e74 6572 6365 7074 6060  ixed_intercept``
-000032a0: 2073 6574 7469 6e67 2074 6865 7365 2061   setting these a
-000032b0: 7265 0a20 2020 2020 2020 2020 2020 205b  re.            [
-000032c0: 492c 204c 2c20 6b5d 206f 7220 5b4c 2c20  I, L, k] or [L, 
-000032d0: 6b5d 2070 6172 616d 6574 6572 7320 6f66  k] parameters of
-000032e0: 2065 7870 6f6e 656e 7469 616c 206d 6f64   exponential mod
-000032f0: 656c 2066 6f72 206d 752e 0a20 2020 2020  el for mu..     
-00003300: 2020 2020 2020 2046 6f6c 6c6f 7765 6420         Followed 
-00003310: 6279 2070 6172 616d 6574 6572 7320 666f  by parameters fo
-00003320: 7220 7468 6520 6d6f 6465 6c20 666f 7220  r the model for 
-00003330: 7363 616c 6520 286c 6f77 6573 7420 6465  scale (lowest de
-00003340: 6772 6565 2066 6972 7374 292e 0a20 2020  gree first)..   
-00003350: 2020 2020 2020 2020 2046 6f6c 6c6f 7765           Followe
-00003360: 6420 6279 2074 6865 2064 6567 7265 6520  d by the degree 
-00003370: 6f66 2066 7265 6564 6f6d 2070 6172 616d  of freedom param
-00003380: 6574 6572 2e0a 0a20 2020 2020 2020 2052  eter...        R
-00003390: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-000033a0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 206d  ------.        m
-000033b0: 7520 3a20 6172 7261 792d 6c69 6b65 0a20  u : array-like. 
-000033c0: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-000033d0: 7320 666f 7220 7468 6520 6d75 2070 6172  s for the mu par
-000033e0: 616d 6574 6572 206f 6620 6120 5374 7564  ameter of a Stud
-000033f0: 656e 742d 7420 6469 7374 7269 6275 7469  ent-t distributi
-00003400: 6f6e 2064 6573 6372 6962 696e 6720 7468  on describing th
-00003410: 6520 6465 7065 6e64 656e 7420 7661 7269  e dependent vari
-00003420: 6162 6c65 2e0a 2020 2020 2020 2020 7363  able..        sc
-00003430: 616c 6520 3a20 6172 7261 792d 6c69 6b65  ale : array-like
-00003440: 206f 7220 666c 6f61 740a 2020 2020 2020   or float.      
-00003450: 2020 2020 2020 5661 6c75 6573 2066 6f72        Values for
-00003460: 2074 6865 2073 6361 6c65 2070 6172 616d   the scale param
-00003470: 6574 6572 206f 6620 6120 5374 7564 656e  eter of a Studen
-00003480: 742d 7420 6469 7374 7269 6275 7469 6f6e  t-t distribution
-00003490: 2064 6573 6372 6962 696e 6720 7468 6520   describing the 
-000034a0: 6465 7065 6e64 656e 7420 7661 7269 6162  dependent variab
-000034b0: 6c65 2e0a 2020 2020 2020 2020 6466 203a  le..        df :
-000034c0: 2066 6c6f 6174 0a20 2020 2020 2020 2020   float.         
-000034d0: 2020 2044 6567 7265 6520 6f66 2066 7265     Degree of fre
-000034e0: 6564 6f6d 206f 6620 5374 7564 656e 742d  edom of Student-
-000034f0: 7420 6469 7374 7269 6275 7469 6f6e 2e0a  t distribution..
-00003500: 2020 2020 2020 2020 4e72 0100 0000 7208          Nr....r.
-00003510: 0000 0072 0500 0000 e903 0000 0072 3300  ...r.........r3.
-00003520: 0000 7232 0000 0029 0772 3400 0000 7252  ..r2...).r4...rR
-00003530: 0000 00da 036c 656e 7221 0000 0072 0600  .....lenr!...r..
-00003540: 0000 da0b 6578 706f 6e65 6e74 6961 6c72  ....exponentialr
-00003550: 3500 0000 2908 7214 0000 0072 3700 0000  5...).r....r7...
-00003560: 7231 0000 00da 0874 6865 7461 5f6d 755a  r1.....theta_muZ
-00003570: 0b74 6865 7461 5f73 6361 6c65 7238 0000  .theta_scaler8..
-00003580: 0072 3900 0000 722b 0000 0072 1700 0000  .r9...r+...r....
-00003590: 7217 0000 0072 1800 0000 723a 0000 0052  r....r....r:...R
-000035a0: 0100 0073 1c00 0000 0018 0801 0602 0a01  ...s............
-000035b0: 1601 0e02 1401 0c01 1601 0c01 0a01 0a02  ................
-000035c0: 0c01 0801 7a27 4261 7365 4578 706f 6e65  ....z'BaseExpone
-000035d0: 6e74 6961 6c4d 6f64 656c 542e 7072 6564  ntialModelT.pred
-000035e0: 6963 745f 6465 7065 6e64 656e 7463 0200  ict_dependentc..
-000035f0: 0000 0000 0000 0100 0000 0400 0000 0400  ................
-00003600: 0000 4300 0000 7350 0000 007c 0264 0175  ..C...sP...|.d.u
-00003610: 0072 0e7c 006a 007d 027c 006a 0164 0175  .r.|.j.}.|.j.d.u
-00003620: 0072 307c 0264 0219 007c 0264 0319 007c  .r0|.d...|.d...|
-00003630: 0264 0419 0066 037d 036e 147c 006a 017c  .d...f.}.n.|.j.|
-00003640: 0264 0219 007c 0264 0319 0066 037d 0374  .d...|.d...f.}.t
-00003650: 02a0 037c 017c 03a1 0253 0029 0561 8a02  ...|.|...S.).a..
-00003660: 0000 5072 6564 6963 7420 7468 6520 696e  ..Predict the in
-00003670: 6465 7065 6e64 656e 7420 7661 7269 6162  dependent variab
-00003680: 6c65 2075 7369 6e67 2074 6865 2069 6e76  le using the inv
-00003690: 6572 7365 2074 7265 6e64 206d 6f64 656c  erse trend model
-000036a0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-000036b0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-000036c0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-000036d0: 2079 203a 2061 7272 6179 2d6c 696b 650a   y : array-like.
-000036e0: 2020 2020 2020 2020 2020 2020 4f62 7365              Obse
-000036f0: 7276 6174 696f 6e73 0a20 2020 2020 2020  rvations.       
-00003700: 2074 6865 7461 203a 206f 7074 696f 6e61   theta : optiona
-00003710: 6c2c 2061 7272 6179 2d6c 696b 650a 2020  l, array-like.  
-00003720: 2020 2020 2020 2020 2020 5061 7261 6d65            Parame
-00003730: 7465 7220 7665 6374 6f72 206f 6620 7468  ter vector of th
-00003740: 6520 6361 6c69 6272 6174 696f 6e20 6d6f  e calibration mo
-00003750: 6465 6c2e 0a20 2020 2020 2020 2020 2020  del..           
-00003760: 2044 6570 656e 6469 6e67 206f 6e20 7468   Depending on th
-00003770: 6520 6060 6669 7865 645f 696e 7465 7263  e ``fixed_interc
-00003780: 6570 7460 6020 7365 7474 696e 6720 7468  ept`` setting th
-00003790: 6573 6520 6172 650a 2020 2020 2020 2020  ese are.        
-000037a0: 2020 2020 5b49 2c20 4c2c 206b 5d20 6f72      [I, L, k] or
-000037b0: 205b 4c2c 206b 5d20 7061 7261 6d65 7465   [L, k] paramete
-000037c0: 7273 206f 6620 6578 706f 6e65 6e74 6961  rs of exponentia
-000037d0: 6c20 6d6f 6465 6c20 666f 7220 6d75 2e0a  l model for mu..
-000037e0: 2020 2020 2020 2020 2020 2020 466f 6c6c              Foll
-000037f0: 6f77 6564 2062 7920 7061 7261 6d65 7465  owed by paramete
-00003800: 7273 2066 6f72 2074 6865 206d 6f64 656c  rs for the model
-00003810: 2066 6f72 2073 6361 6c65 2028 6c6f 7765   for scale (lowe
-00003820: 7374 2064 6567 7265 6520 6669 7273 7429  st degree first)
-00003830: 2e0a 2020 2020 2020 2020 2020 2020 466f  ..            Fo
-00003840: 6c6c 6f77 6564 2062 7920 7468 6520 6465  llowed by the de
-00003850: 6772 6565 206f 6620 6672 6565 646f 6d20  gree of freedom 
-00003860: 7061 7261 6d65 7465 722e 0a0a 2020 2020  parameter...    
-00003870: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00003880: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00003890: 2020 2020 7820 3a20 6172 7261 792d 6c69      x : array-li
-000038a0: 6b65 0a20 2020 2020 2020 2020 2020 2050  ke.            P
-000038b0: 7265 6469 6374 6564 2069 6e64 6570 656e  redicted indepen
-000038c0: 6465 6e74 2076 616c 7565 7320 6769 7665  dent values give
-000038d0: 6e20 7468 6520 6f62 7365 7276 6174 696f  n the observatio
-000038e0: 6e73 2e0a 2020 2020 2020 2020 4e72 0100  ns..        Nr..
-000038f0: 0000 7208 0000 0072 0500 0000 2904 7234  ..r....r....).r4
-00003900: 0000 0072 5200 0000 7206 0000 00da 1369  ...rR...r......i
-00003910: 6e76 6572 7365 5f65 7870 6f6e 656e 7469  nverse_exponenti
-00003920: 616c 2904 7214 0000 0072 3c00 0000 7231  al).r....r<...r1
-00003930: 0000 0072 5a00 0000 7217 0000 0072 1700  ...rZ...r....r..
-00003940: 0000 7218 0000 0072 3f00 0000 7c01 0000  ..r....r?...|...
-00003950: 730c 0000 0000 1308 0106 020a 0118 0214  s...............
-00003960: 027a 2942 6173 6545 7870 6f6e 656e 7469  .z)BaseExponenti
-00003970: 616c 4d6f 6465 6c54 2e70 7265 6469 6374  alModelT.predict
-00003980: 5f69 6e64 6570 656e 6465 6e74 290c 7219  _independent).r.
-00003990: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
-000039a0: 0000 7241 0000 0072 0200 0000 da05 666c  ..rA...r......fl
-000039b0: 6f61 7472 0300 0000 7213 0000 0072 3a00  oatr....r....r:.
-000039c0: 0000 723f 0000 0072 1e00 0000 7217 0000  ..r?...r....r...
-000039d0: 0072 1700 0000 7215 0000 0072 1800 0000  .r....r....r....
-000039e0: 7251 0000 002c 0100 0073 1800 0000 0806  rQ...,...s......
-000039f0: 0201 0201 02f9 0403 0201 0201 0201 0601  ................
-00003a00: 0af9 1025 0e2a 7251 0000 0029 11da 075f  ...%.*rQ...)..._
-00003a10: 5f64 6f63 5f5f 721d 0000 0072 0f00 0000  _doc__r....r....
-00003a20: 7202 0000 0072 0300 0000 7204 0000 00da  r....r....r.....
-00003a30: 0072 0600 0000 7207 0000 0072 0900 0000  .r....r....r....
-00003a40: da19 436f 6e74 696e 756f 7573 556e 6976  ..ContinuousUniv
-00003a50: 6172 6961 7465 4d6f 6465 6cda 0d53 7475  ariateModel..Stu
-00003a60: 6465 6e74 544e 6f69 7365 720a 0000 0072  dentTNoiser....r
-00003a70: 1f00 0000 7242 0000 0072 4e00 0000 7251  ....rB...rN...rQ
-00003a80: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
-00003a90: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00003aa0: 3e01 0000 0073 1400 0000 0404 0801 0801  >....s..........
-00003ab0: 1402 1001 0c03 160c 1665 1657 1657       .........e.W.W
+00000000: a70d 0d0a 0000 0000 81e0 3966 cd35 0000  ..........9f.5..
+00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
+00000020: 0000 0000 00f3 0201 0000 9700 6400 5a00  ............d.Z.
+00000030: 6401 6402 6c01 6d02 5a02 6d03 5a03 6d04  d.d.l.m.Z.m.Z.m.
+00000040: 5a04 0100 6403 6404 6c05 6d06 5a06 6d07  Z...d.d.l.m.Z.m.
+00000050: 5a07 0100 6405 6406 6c05 6d08 5a08 0100  Z...d.d.l.m.Z...
+00000060: 0200 4700 6407 8400 6408 6506 6a09 0000  ..G.d...d.e.j...
+00000070: 0000 0000 0000 6508 6a0a 0000 0000 0000  ......e.j.......
+00000080: 0000 a604 0000 ab04 0000 0000 0000 0000  ................
+00000090: 5a0b 0200 4700 6409 8400 640a 6506 6a09  Z...G.d...d.e.j.
+000000a0: 0000 0000 0000 0000 6508 6a0a 0000 0000  ........e.j.....
+000000b0: 0000 0000 a604 0000 ab04 0000 0000 0000  ................
+000000c0: 0000 5a0c 0200 4700 640b 8400 640c 6506  ..Z...G.d...d.e.
+000000d0: 6a09 0000 0000 0000 0000 6508 6a0a 0000  j.........e.j...
+000000e0: 0000 0000 0000 a604 0000 ab04 0000 0000  ................
+000000f0: 0000 0000 5a0d 0200 4700 640d 8400 640e  ....Z...G.d...d.
+00000100: 6506 6a09 0000 0000 0000 0000 6508 6a0a  e.j.........e.j.
+00000110: 0000 0000 0000 0000 a604 0000 ab04 0000  ................
+00000120: 0000 0000 0000 5a0e 640f 5300 2910 7a6a  ......Z.d.S.).zj
+00000130: 0a54 6869 7320 6d6f 6475 6c65 2069 6d70  .This module imp
+00000140: 6c65 6d65 6e74 7320 7265 7573 6162 6c65  lements reusable
+00000150: 2063 616c 6962 7261 7469 6f6e 206d 6f64   calibration mod
+00000160: 656c 730a 7769 7468 204e 6f72 6d61 6c20  els.with Normal 
+00000170: 6469 7374 7269 6275 7469 6f6e 7320 666f  distributions fo
+00000180: 7220 7468 6520 6465 7065 6e64 656e 7420  r the dependent 
+00000190: 7661 7269 6162 6c65 2e0a e900 0000 0029  variable.......)
+000001a0: 03da 084f 7074 696f 6e61 6cda 0853 6571  ...Optional..Seq
+000001b0: 7565 6e63 65da 0554 7570 6c65 e902 0000  uence..Tuple....
+000001c0: 0029 02da 0463 6f72 65da 0575 7469 6c73  .)...core..utils
+000001d0: e901 0000 0029 01da 056e 6f69 7365 6300  .....)...noisec.
+000001e0: 0000 0000 0000 0000 0000 000d 0000 0000  ................
+000001f0: 0000 00f3 6c00 0000 8700 9700 6500 5a01  ....l.......e.Z.
+00000200: 6400 5a02 6401 6402 6403 9c02 6404 6503  d.Z.d.d.d...d.e.
+00000210: 6405 6503 6406 6504 6407 6504 6408 6505  d.e.d.e.d.e.d.e.
+00000220: 6506 6503 1900 0000 0000 0000 0000 1900  e.e.............
+00000230: 0000 0000 0000 0000 660a 8800 6601 6409  ........f...f.d.
+00000240: 840e 5a07 6402 640a 9c01 640b 8402 5a08  ..Z.d.d...d...Z.
+00000250: 6402 640a 9c01 640c 8402 5a09 8800 7801  d.d...d...Z...x.
+00000260: 5a0a 5300 290d da14 4261 7365 506f 6c79  Z.S.)...BasePoly
+00000270: 6e6f 6d69 616c 4d6f 6465 6c4e 7202 0000  nomialModelNr...
+00000280: 004e a902 da0c 7369 676d 615f 6465 6772  .N....sigma_degr
+00000290: 6565 da0b 7468 6574 615f 6e61 6d65 73da  ee..theta_names.
+000002a0: 0f69 6e64 6570 656e 6465 6e74 5f6b 6579  .independent_key
+000002b0: da0d 6465 7065 6e64 656e 745f 6b65 79da  ..dependent_key.
+000002c0: 096d 755f 6465 6772 6565 720e 0000 0072  .mu_degreer....r
+000002d0: 0f00 0000 6301 0000 0000 0000 0005 0000  ....c...........
+000002e0: 0008 0000 0003 0000 00f3 6401 0000 9501  ..........d.....
+000002f0: 9700 7c03 6401 6b02 0000 0000 720f 7401  ..|.d.k.....r.t.
+00000300: 0000 0000 0000 0000 0000 6402 a601 0000  ..........d.....
+00000310: ab01 0000 0000 0000 0000 8201 7c03 7c00  ............|.|.
+00000320: 5f01 0000 0000 0000 0000 7405 0000 0000  _.........t.....
+00000330: 0000 0000 0000 6a03 0000 0000 0000 0000  ......j.........
+00000340: 7c04 a601 0000 ab01 0000 0000 0000 0000  |...............
+00000350: 7c00 5f04 0000 0000 0000 0000 7c05 8053  |._.........|..S
+00000360: 740b 0000 0000 0000 0000 0000 6404 8400  t...........d...
+00000370: 740d 0000 0000 0000 0000 0000 7c03 6405  t...........|.d.
+00000380: 7a00 0000 a601 0000 ab01 0000 0000 0000  z...............
+00000390: 0000 4400 a600 0000 ab00 0000 0000 0000  ..D.............
+000003a0: 0000 a601 0000 ab01 0000 0000 0000 0000  ................
+000003b0: 740b 0000 0000 0000 0000 0000 6406 8400  t...........d...
+000003c0: 740d 0000 0000 0000 0000 0000 7c04 6405  t...........|.d.
+000003d0: 7a00 0000 a601 0000 ab01 0000 0000 0000  z...............
+000003e0: 0000 4400 a600 0000 ab00 0000 0000 0000  ..D.............
+000003f0: 0000 a601 0000 ab01 0000 0000 0000 0000  ................
+00000400: 7a00 0000 7d05 740f 0000 0000 0000 0000  z...}.t.........
+00000410: 0000 a600 0000 ab00 0000 0000 0000 0000  ................
+00000420: a008 0000 0000 0000 0000 0000 0000 0000  ................
+00000430: 0000 0000 0000 7c01 7c02 7c05 ac07 a603  ......|.|.|.....
+00000440: 0000 ab03 0000 0000 0000 0000 0100 6403  ..............d.
+00000450: 5300 2908 618c 0200 0054 656d 706c 6174  S.).a....Templat
+00000460: 6520 666f 7220 6120 6d6f 6465 6c20 7769  e for a model wi
+00000470: 7468 2070 6f6c 796e 6f6d 6961 6c20 7472  th polynomial tr
+00000480: 656e 6420 286d 7529 2061 6e64 2073 6967  end (mu) and sig
+00000490: 6d61 2028 6173 2061 2066 756e 6374 696f  ma (as a functio
+000004a0: 6e20 6f66 206d 7529 0a20 2020 2020 2020  n of mu).       
+000004b0: 2077 6974 6820 6120 6e6f 726d 616c 6c79   with a normally
+000004c0: 2064 6973 7472 6962 7574 6564 206f 6273   distributed obs
+000004d0: 6572 7661 7469 6f6e 206e 6f69 7365 2e0a  ervation noise..
+000004e0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+000004f0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00000500: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2069  ------.        i
+00000510: 6e64 6570 656e 6465 6e74 5f6b 6579 203a  ndependent_key :
+00000520: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+00000530: 206e 616d 6520 6f66 2074 6865 2069 6e64   name of the ind
+00000540: 6570 656e 6465 6e74 2076 6172 6961 626c  ependent variabl
+00000550: 650a 2020 2020 2020 2020 6465 7065 6e64  e.        depend
+00000560: 656e 745f 6b65 7920 3a20 7374 720a 2020  ent_key : str.  
+00000570: 2020 2020 2020 2020 2020 6e61 6d65 206f            name o
+00000580: 6620 7468 6520 6465 7065 6e64 656e 7420  f the dependent 
+00000590: 7661 7269 6162 6c65 0a20 2020 2020 2020  variable.       
+000005a0: 206d 755f 6465 6772 6565 203a 2069 6e74   mu_degree : int
+000005b0: 0a20 2020 2020 2020 2020 2020 2064 6567  .            deg
+000005c0: 7265 6520 6f66 2074 6865 2070 6f6c 796e  ree of the polyn
+000005d0: 6f6d 6961 6c20 6d6f 6465 6c20 6465 7363  omial model desc
+000005e0: 7269 6269 6e67 2074 6865 2074 7265 6e64  ribing the trend
+000005f0: 2028 6d75 290a 2020 2020 2020 2020 7369   (mu).        si
+00000600: 676d 615f 6465 6772 6565 203a 206f 7074  gma_degree : opt
+00000610: 696f 6e61 6c2c 2069 6e74 0a20 2020 2020  ional, int.     
+00000620: 2020 2020 2020 2064 6567 7265 6520 6f66         degree of
+00000630: 2074 6865 2070 6f6c 796e 6f6d 6961 6c20   the polynomial 
+00000640: 6d6f 6465 6c20 6465 7363 7269 6269 6e67  model describing
+00000650: 2074 6865 2073 6967 6d61 2061 7320 6120   the sigma as a 
+00000660: 6675 6e63 7469 6f6e 206f 6620 6d75 0a20  function of mu. 
+00000670: 2020 2020 2020 2074 6865 7461 5f6e 616d         theta_nam
+00000680: 6573 203a 206f 7074 696f 6e61 6c2c 2074  es : optional, t
+00000690: 7570 6c65 206f 6620 7374 720a 2020 2020  uple of str.    
+000006a0: 2020 2020 2020 2020 6d61 7920 6265 2075          may be u
+000006b0: 7365 6420 746f 2073 6574 2074 6865 206e  sed to set the n
+000006c0: 616d 6573 206f 6620 7468 6520 6d6f 6465  ames of the mode
+000006d0: 6c20 7061 7261 6d65 7465 7273 0a20 2020  l parameters.   
+000006e0: 2020 2020 2072 0200 0000 7a36 302d 6465       r....z60-de
+000006f0: 6772 6565 2028 636f 6e73 7461 6e74 2920  gree (constant) 
+00000700: 6d75 2063 616c 6962 7261 7469 6f6e 206d  mu calibration m
+00000710: 6f64 656c 7320 6172 6520 7573 656c 6573  odels are useles
+00000720: 732e 4e63 0100 0000 0000 0000 0000 0000  s.Nc............
+00000730: 0300 0000 3300 0000 f320 0000 004b 0001  ....3.... ...K..
+00000740: 0097 007c 005d 097d 0164 007c 019b 009d  ...|.].}.d.|....
+00000750: 0256 0097 0101 008c 0a64 0153 0029 02da  .V.......d.S.)..
+00000760: 036d 755f 4ea9 00a9 02da 022e 30da 0164  .mu_N.......0..d
+00000770: 7302 0000 0020 20fa 3b2f 686f 6d65 2f72  s....  .;/home/r
+00000780: 756e 6e65 722f 776f 726b 2f63 616c 6962  unner/work/calib
+00000790: 7238 2f63 616c 6962 7238 2f63 616c 6962  r8/calibr8/calib
+000007a0: 7238 2f63 6f6e 7472 6962 2f6e 6f72 6d61  r8/contrib/norma
+000007b0: 6c2e 7079 fa09 3c67 656e 6578 7072 3e7a  l.py..<genexpr>z
+000007c0: 3042 6173 6550 6f6c 796e 6f6d 6961 6c4d  0BasePolynomialM
+000007d0: 6f64 656c 4e2e 5f5f 696e 6974 5f5f 2e3c  odelN.__init__.<
+000007e0: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
+000007f0: 3e2a 0000 0073 2800 0000 e800 e800 8000  >*...s(.........
+00000800: d01f 48d0 1f48 a861 a009 a061 a009 a009  ..H..H.a...a....
+00000810: d01f 48d0 1f48 d01f 48d0 1f48 d01f 48d0  ..H..H..H..H..H.
+00000820: 1f48 f300 0000 0072 0900 0000 6301 0000  .H.....r....c...
+00000830: 0000 0000 0000 0000 0003 0000 0033 0000  .............3..
+00000840: 00f3 2000 0000 4b00 0100 9700 7c00 5d09  .. ...K.....|.].
+00000850: 7d01 6400 7c01 9b00 9d02 5600 9701 0100  }.d.|.....V.....
+00000860: 8c0a 6401 5300 a902 da06 7369 676d 615f  ..d.S.....sigma_
+00000870: 4e72 1600 0000 7217 0000 0073 0200 0000  Nr....r....s....
+00000880: 2020 721a 0000 0072 1b00 0000 7a30 4261    r....r....z0Ba
+00000890: 7365 506f 6c79 6e6f 6d69 616c 4d6f 6465  sePolynomialMode
+000008a0: 6c4e 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  lN.__init__.<loc
+000008b0: 616c 733e 2e3c 6765 6e65 7870 723e 2a00  als>.<genexpr>*.
+000008c0: 0000 7341 0000 00e8 00e8 0080 00f0 0002  ..sA............
+000008d0: 5101 0ef0 0002 5101 0ed8 2122 900c 9811  Q.....Q...!"....
+000008e0: 900c 900c f003 0251 010e f000 0251 010e  .......Q.....Q..
+000008f0: f000 0251 010e f000 0251 010e f000 0251  ...Q.....Q.....Q
+00000900: 010e f000 0251 010e 721c 0000 0029 0372  .....Q..r....).r
+00000910: 1000 0000 7211 0000 0072 0f00 0000 2909  ....r....r....).
+00000920: da0a 5661 6c75 6545 7272 6f72 7212 0000  ..ValueErrorr...
+00000930: 0072 0800 0000 da12 6368 6563 6b5f 7363  .r......check_sc
+00000940: 616c 655f 6465 6772 6565 720e 0000 00da  ale_degreer.....
+00000950: 0574 7570 6c65 da05 7261 6e67 65da 0573  .tuple..range..s
+00000960: 7570 6572 da08 5f5f 696e 6974 5f5f 2907  uper..__init__).
+00000970: da04 7365 6c66 7210 0000 0072 1100 0000  ..selfr....r....
+00000980: 7212 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
+00000990: 095f 5f63 6c61 7373 5f5f 7307 0000 0020  .__class__s.... 
+000009a0: 2020 2020 2080 721a 0000 0072 2500 0000       .r....r%...
+000009b0: 7a1d 4261 7365 506f 6c79 6e6f 6d69 616c  z.BasePolynomial
+000009c0: 4d6f 6465 6c4e 2e5f 5f69 6e69 745f 5f0c  ModelN.__init__.
+000009d0: 0000 0073 db00 0000 f880 00f0 3200 0c15  ...s........2...
+000009e0: 9801 8a3e 883e dd12 1cd0 1d55 d112 56d4  ...>.>.....U..V.
+000009f0: 1256 d00c 56d8 1922 8804 8c0e dd1c 21d4  .V..V.."......!.
+00000a00: 1c34 b05c d11c 42d4 1c42 8804 d408 19d8  .4.\..B..B......
+00000a10: 0b16 d00b 1edd 1a1f d01f 48d0 1f48 b535  ..........H..H.5
+00000a20: b819 c051 b91d d133 47d4 3347 d01f 48d1  ...Q...3G.3G..H.
+00000a30: 1f48 d41f 48d1 1a48 d41a 48cd 35f0 0002  .H..H..H..H.5...
+00000a40: 5101 0ef0 0002 5101 0edd 262b a84c b831  Q.....Q...&+.L.1
+00000a50: d12c 3cd1 263d d426 3df0 0302 5101 0ef1  .,<.&=.&=...Q...
+00000a60: 0002 5101 0ef4 0002 5101 0ef1 0002 4c01  ..Q.....Q.....L.
+00000a70: 0ef4 0002 4c01 0ef1 0002 1b0e 884b f506  ....L........K..
+00000a80: 0009 0e89 078c 07d7 0818 d208 18d8 1c2b  ...............+
+00000a90: b83d d056 61f0 0300 0919 f100 0209 0af4  .=.Va...........
+00000aa0: 0002 090a f000 0209 0af0 0002 090a f000  ................
+00000ab0: 0209 0a72 1c00 0000 a901 da05 7468 6574  ...r........thet
+00000ac0: 6163 0200 0000 0000 0000 0100 0000 0700  ac..............
+00000ad0: 0000 0300 0000 f3dc 0000 0097 007c 0280  .............|..
+00000ae0: 077c 006a 0000 0000 0000 0000 007d 0274  .|.j.........}.t
+00000af0: 0300 0000 0000 0000 0000 006a 0200 0000  ...........j....
+00000b00: 0000 0000 007c 017c 0264 017c 006a 0300  .....|.|.d.|.j..
+00000b10: 0000 0000 0000 0064 027a 0000 0085 0219  .......d.z......
+00000b20: 0000 0000 0000 0000 00ac 03a6 0200 00ab  ................
+00000b30: 0200 0000 0000 0000 007d 037c 006a 0400  .........}.|.j..
+00000b40: 0000 0000 0000 0064 046b 0200 0000 0072  .......d.k.....r
+00000b50: 097c 0264 0519 0000 0000 0000 0000 007d  .|.d...........}
+00000b60: 046e 2674 0300 0000 0000 0000 0000 006a  .n&t...........j
+00000b70: 0200 0000 0000 0000 007c 037c 027c 006a  .........|.|.|.j
+00000b80: 0300 0000 0000 0000 0064 027a 0000 0064  .........d.z...d
+00000b90: 0185 0219 0000 0000 0000 0000 00ac 03a6  ................
+00000ba0: 0200 00ab 0200 0000 0000 0000 007d 047c  .............}.|
+00000bb0: 037c 0466 0253 0029 0661 2003 0000 5072  .|.f.S.).a ...Pr
+00000bc0: 6564 6963 7473 2074 6865 2070 6172 616d  edicts the param
+00000bd0: 6574 6572 7320 6d75 2061 6e64 2073 6967  eters mu and sig
+00000be0: 6d61 206f 6620 6120 6e6f 726d 616c 2064  ma of a normal d
+00000bf0: 6973 7472 6962 7574 696f 6e20 7768 6963  istribution whic
+00000c00: 680a 2020 2020 2020 2020 6368 6172 6163  h.        charac
+00000c10: 7465 7269 7a65 7320 7468 6520 6465 7065  terizes the depe
+00000c20: 6e64 656e 7420 7661 7269 6162 6c65 2067  ndent variable g
+00000c30: 6976 656e 2076 616c 7565 7320 6f66 2074  iven values of t
+00000c40: 6865 2069 6e64 6570 656e 6465 6e74 2076  he independent v
+00000c50: 6172 6961 626c 652e 0a0a 2020 2020 2020  ariable...      
+00000c60: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00000c70: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00000c80: 2020 2020 2020 2020 7820 3a20 6172 7261          x : arra
+00000c90: 792d 6c69 6b65 0a20 2020 2020 2020 2020  y-like.         
+00000ca0: 2020 2076 616c 7565 7320 6f66 2074 6865     values of the
+00000cb0: 2069 6e64 6570 656e 6465 6e74 2076 6172   independent var
+00000cc0: 6961 626c 650a 2020 2020 2020 2020 7468  iable.        th
+00000cd0: 6574 6120 3a20 6f70 7469 6f6e 616c 2c20  eta : optional, 
+00000ce0: 6172 7261 792d 6c69 6b65 0a20 2020 2020  array-like.     
+00000cf0: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
+00000d00: 2076 6563 746f 7220 6f66 2074 6865 2063   vector of the c
+00000d10: 616c 6962 7261 7469 6f6e 206d 6f64 656c  alibration model
+00000d20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000d30: 2020 5b6d 755f 6465 6772 6565 5d20 7061    [mu_degree] pa
+00000d40: 7261 6d65 7465 7273 2066 6f72 206d 7520  rameters for mu 
+00000d50: 286c 6f77 6573 7420 6465 6772 6565 2066  (lowest degree f
+00000d60: 6972 7374 290a 2020 2020 2020 2020 2020  irst).          
+00000d70: 2020 2020 2020 5b73 6967 6d61 5f64 6567        [sigma_deg
+00000d80: 7265 655d 2070 6172 616d 6574 6572 7320  ree] parameters 
+00000d90: 666f 7220 7369 676d 6120 286c 6f77 6573  for sigma (lowes
+00000da0: 7420 6465 6772 6565 2066 6972 7374 290a  t degree first).
+00000db0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00000dc0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00000dd0: 0a20 2020 2020 2020 206d 7520 3a20 6172  .        mu : ar
+00000de0: 7261 792d 6c69 6b65 0a20 2020 2020 2020  ray-like.       
+00000df0: 2020 2020 2076 616c 7565 7320 666f 7220       values for 
+00000e00: 7468 6520 6d75 2070 6172 616d 6574 6572  the mu parameter
+00000e10: 206f 6620 6120 6e6f 726d 616c 2064 6973   of a normal dis
+00000e20: 7472 6962 7574 696f 6e20 6465 7363 7269  tribution descri
+00000e30: 6269 6e67 2074 6865 2064 6570 656e 6465  bing the depende
+00000e40: 6e74 2076 6172 6961 626c 650a 2020 2020  nt variable.    
+00000e50: 2020 2020 7369 676d 6120 3a20 6172 7261      sigma : arra
+00000e60: 792d 6c69 6b65 206f 7220 666c 6f61 740a  y-like or float.
+00000e70: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00000e80: 6573 2066 6f72 2074 6865 2073 6967 6d61  es for the sigma
+00000e90: 2070 6172 616d 6574 6572 206f 6620 6120   parameter of a 
+00000ea0: 6e6f 726d 616c 2064 6973 7472 6962 7574  normal distribut
+00000eb0: 696f 6e20 6465 7363 7269 6269 6e67 2074  ion describing t
+00000ec0: 6865 2064 6570 656e 6465 6e74 2076 6172  he dependent var
+00000ed0: 6961 626c 650a 2020 2020 2020 2020 4e72  iable.        Nr
+00000ee0: 0900 0000 7228 0000 0072 0200 0000 e9ff  ....r(...r......
+00000ef0: ffff ff29 05da 0c74 6865 7461 5f66 6974  ...)...theta_fit
+00000f00: 7465 6472 0700 0000 da0a 706f 6c79 6e6f  tedr......polyno
+00000f10: 6d69 616c 7212 0000 0072 0e00 0000 a905  mialr....r......
+00000f20: 7226 0000 00da 0178 7229 0000 00da 026d  r&.....xr).....m
+00000f30: 75da 0573 6967 6d61 7305 0000 0020 2020  u..sigmas....   
+00000f40: 2020 721a 0000 00da 1170 7265 6469 6374    r......predict
+00000f50: 5f64 6570 656e 6465 6e74 7a26 4261 7365  _dependentz&Base
+00000f60: 506f 6c79 6e6f 6d69 616c 4d6f 6465 6c4e  PolynomialModelN
+00000f70: 2e70 7265 6469 6374 5f64 6570 656e 6465  .predict_depende
+00000f80: 6e74 3100 0000 7380 0000 0080 00f0 2800  nt1...s.......(.
+00000f90: 0c11 883d d814 18d4 1425 8845 dd0d 118c  ...=.....%.E....
+00000fa0: 5f98 51a0 65d0 2c40 a864 ac6e b871 d12e  _.Q.e.,@.d.n.q..
+00000fb0: 40d0 2c40 d426 41d0 0d42 d10d 42d4 0d42  @.,@.&A..B..B..B
+00000fc0: 8802 d80b 0fd4 0b1c a001 d20b 21d0 0b21  ............!..!
+00000fd0: d814 1998 2294 4988 4588 45e5 1418 944f  ....".I.E.E....O
+00000fe0: a042 a865 b044 b44e c051 d134 46d0 3448  .B.e.D.N.Q.4F.4H
+00000ff0: d034 48d4 2e49 d014 4ad1 144a d414 4a88  .4H..I..J..J..J.
+00001000: 45d8 0f11 9035 8879 d008 1872 1c00 0000  E....5.y...r....
+00001010: 6302 0000 0000 0000 0001 0000 0003 0000  c...............
+00001020: 0003 0000 00f3 7200 0000 9700 7c02 8007  ......r.....|...
+00001030: 7c00 6a00 0000 0000 0000 0000 7d02 7c00  |.j.........}.|.
+00001040: 6a01 0000 0000 0000 0000 6402 6b04 0000  j.........d.k...
+00001050: 0000 720f 7405 0000 0000 0000 0000 0000  ..r.t...........
+00001060: 6403 a601 0000 ab01 0000 0000 0000 0000  d...............
+00001070: 8201 7c02 6401 6404 8502 1900 0000 0000  ..|.d.d.........
+00001080: 0000 0000 5c02 0000 7d03 7d04 7c01 7c03  ....\...}.}.|.|.
+00001090: 7a0a 0000 7c04 7a0b 0000 5300 2905 6101  z...|.z...S.).a.
+000010a0: 0200 0050 7265 6469 6374 2074 6865 2069  ...Predict the i
+000010b0: 6e64 6570 656e 6465 6e74 2076 6172 6961  ndependent varia
+000010c0: 626c 6520 7573 696e 6720 7468 6520 696e  ble using the in
+000010d0: 7665 7273 6520 7472 656e 6420 6d6f 6465  verse trend mode
+000010e0: 6c2e 0a0a 2020 2020 2020 2020 5061 7261  l...        Para
+000010f0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+00001100: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00001110: 2020 7920 3a20 6172 7261 792d 6c69 6b65    y : array-like
+00001120: 0a20 2020 2020 2020 2020 2020 206f 6273  .            obs
+00001130: 6572 7661 7469 6f6e 730a 2020 2020 2020  ervations.      
+00001140: 2020 7468 6574 6120 3a20 6f70 7469 6f6e    theta : option
+00001150: 616c 2c20 6172 7261 792d 6c69 6b65 0a20  al, array-like. 
+00001160: 2020 2020 2020 2020 2020 2070 6172 616d             param
+00001170: 6574 6572 2076 6563 746f 7220 6f66 2074  eter vector of t
+00001180: 6865 2063 616c 6962 7261 7469 6f6e 206d  he calibration m
+00001190: 6f64 656c 3a0a 2020 2020 2020 2020 2020  odel:.          
+000011a0: 2020 2020 2020 5b6d 755f 6465 6772 6565        [mu_degree
+000011b0: 5d20 7061 7261 6d65 7465 7273 2066 6f72  ] parameters for
+000011c0: 206d 7520 286c 6f77 6573 7420 6465 6772   mu (lowest degr
+000011d0: 6565 2066 6972 7374 290a 2020 2020 2020  ee first).      
+000011e0: 2020 2020 2020 2020 2020 5b73 6967 6d61            [sigma
+000011f0: 5f64 6567 7265 655d 2070 6172 616d 6574  _degree] paramet
+00001200: 6572 7320 666f 7220 7369 676d 6120 286c  ers for sigma (l
+00001210: 6f77 6573 7420 6465 6772 6565 2066 6972  owest degree fir
+00001220: 7374 290a 0a20 2020 2020 2020 2052 6574  st)..        Ret
+00001230: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00001240: 2d2d 2d2d 0a20 2020 2020 2020 2078 203a  ----.        x :
+00001250: 2061 7272 6179 2d6c 696b 650a 2020 2020   array-like.    
+00001260: 2020 2020 2020 2020 7072 6564 6963 7465          predicte
+00001270: 6420 696e 6465 7065 6e64 656e 7420 7661  d independent va
+00001280: 6c75 6573 2067 6976 656e 2074 6865 206f  lues given the o
+00001290: 6273 6572 7661 7469 6f6e 730a 2020 2020  bservations.    
+000012a0: 2020 2020 4e72 0900 0000 7a43 496e 7665      Nr....zCInve
+000012b0: 7273 6520 7072 6564 6963 7469 6f6e 206f  rse prediction o
+000012c0: 6620 6869 6768 6572 206f 7264 6572 2070  f higher order p
+000012d0: 6f6c 796e 6f6d 6961 6c73 2061 7265 206e  olynomials are n
+000012e0: 6f74 2069 6d70 6c65 6d65 6e74 6564 2e72  ot implemented.r
+000012f0: 0600 0000 2903 722c 0000 0072 1200 0000  ....).r,...r....
+00001300: da13 4e6f 7449 6d70 6c65 6d65 6e74 6564  ..NotImplemented
+00001310: 4572 726f 7229 0572 2600 0000 da01 7972  Error).r&.....yr
+00001320: 2900 0000 da01 61da 0162 7305 0000 0020  ).....a..bs.... 
+00001330: 2020 2020 721a 0000 00da 1370 7265 6469      r......predi
+00001340: 6374 5f69 6e64 6570 656e 6465 6e74 7a28  ct_independentz(
+00001350: 4261 7365 506f 6c79 6e6f 6d69 616c 4d6f  BasePolynomialMo
+00001360: 6465 6c4e 2e70 7265 6469 6374 5f69 6e64  delN.predict_ind
+00001370: 6570 656e 6465 6e74 4e00 0000 734c 0000  ependentN...sL..
+00001380: 0080 00f0 2200 0c11 883d d814 18d4 1425  ...."....=.....%
+00001390: 8845 d80b 0f8c 3e98 41d2 0b1d d00b 1ddd  .E....>.A.......
+000013a0: 1225 d026 6bd1 126c d412 6cd0 0c6c d80f  .%.&k..l..l..l..
+000013b0: 1490 5290 6190 528c 7989 0488 0188 31d8  ..R.a.R.y.....1.
+000013c0: 1011 9041 9105 9811 897b d008 1a72 1c00  ...A.....{...r..
+000013d0: 0000 a90b da08 5f5f 6e61 6d65 5f5f da0a  ......__name__..
+000013e0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000013f0: 616c 6e61 6d65 5f5f da03 7374 72da 0369  alname__..str..i
+00001400: 6e74 7203 0000 0072 0400 0000 7225 0000  ntr....r....r%..
+00001410: 0072 3200 0000 7238 0000 00da 0d5f 5f63  .r2...r8.....__c
+00001420: 6c61 7373 6365 6c6c 5f5f a901 7227 0000  lasscell__..r'..
+00001430: 0073 0100 0000 4072 1a00 0000 720c 0000  .s....@r....r...
+00001440: 0072 0c00 0000 0b00 0000 73c7 0000 00f8  .r........s.....
+00001450: 8000 8000 8000 8000 8000 f00e 001d 1ed8  ................
+00001460: 2f33 f00f 2305 0af0 0023 050a f000 2305  /3..#....#....#.
+00001470: 0af0 0600 1a1d f007 2305 0af0 0800 181b  ........#.......
+00001480: f009 2305 0af0 0a00 1417 f00b 2305 0af0  ..#.........#...
+00001490: 0c00 171a f00d 2305 0af0 0e00 161e 9868  ......#........h
+000014a0: a073 9c6d d415 2cf0 0f23 050a f000 2305  .s.m..,..#....#.
+000014b0: 0af0 0023 050a f000 2305 0af0 0023 050a  ...#....#....#..
+000014c0: f000 2305 0af0 4a01 002d 31f0 001b 0519  ..#...J..-1.....
+000014d0: f000 1b05 19f0 001b 0519 f000 1b05 19f0  ................
+000014e0: 001b 0519 f03a 002f 33f0 0016 051b f000  .....:./3.......
+000014f0: 1605 1bf0 0016 051b f000 1605 1bf0 0016  ................
+00001500: 051b f000 1605 1bf0 0016 051b f000 1605  ................
+00001510: 1bf0 0016 051b 721c 0000 0072 0c00 0000  ......r....r....
+00001520: 6300 0000 0000 0000 0000 0000 000b 0000  c...............
+00001530: 0000 0000 00f3 6800 0000 8700 9700 6500  ......h.......e.
+00001540: 5a01 6400 5a02 6401 6402 6403 9c02 6404  Z.d.Z.d.d.d...d.
+00001550: 6503 6405 6503 6406 6504 6407 6505 6506  e.d.e.d.e.d.e.e.
+00001560: 6503 1900 0000 0000 0000 0000 1900 0000  e...............
+00001570: 0000 0000 0000 6608 8800 6601 6408 840e  ......f...f.d...
+00001580: 5a07 6402 6409 9c01 640a 8402 5a08 6402  Z.d.d...d...Z.d.
+00001590: 6409 9c01 640b 8402 5a09 8800 7801 5a0a  d...d...Z...x.Z.
+000015a0: 5300 290c da17 4261 7365 4173 796d 6d65  S.)...BaseAsymme
+000015b0: 7472 6963 4c6f 6769 7374 6963 4e72 0200  tricLogisticNr..
+000015c0: 0000 4e72 0d00 0000 7210 0000 0072 1100  ..Nr....r....r..
+000015d0: 0000 720e 0000 0072 0f00 0000 6301 0000  ..r....r....c...
+000015e0: 0000 0000 0004 0000 0008 0000 0003 0000  ................
+000015f0: 00f3 1e01 0000 9501 9700 7401 0000 0000  ..........t.....
+00001600: 0000 0000 0000 6a01 0000 0000 0000 0000  ......j.........
+00001610: 7c03 a601 0000 ab01 0000 0000 0000 0000  |...............
+00001620: 7c00 5f02 0000 0000 0000 0000 7c04 804c  |._.........|..L
+00001630: 7407 0000 0000 0000 0000 0000 6402 a004  t...........d...
+00001640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001650: 0000 0000 6403 a601 0000 ab01 0000 0000  ....d...........
+00001660: 0000 0000 a601 0000 ab01 0000 0000 0000  ................
+00001670: 0000 7407 0000 0000 0000 0000 0000 6404  ..t...........d.
+00001680: 8400 740b 0000 0000 0000 0000 0000 7c03  ..t...........|.
+00001690: 6405 7a00 0000 a601 0000 ab01 0000 0000  d.z.............
+000016a0: 0000 0000 4400 a600 0000 ab00 0000 0000  ....D...........
+000016b0: 0000 0000 a601 0000 ab01 0000 0000 0000  ................
+000016c0: 0000 7a00 0000 7d04 740d 0000 0000 0000  ..z...}.t.......
+000016d0: 0000 0000 a600 0000 ab00 0000 0000 0000  ................
+000016e0: 0000 a007 0000 0000 0000 0000 0000 0000  ................
+000016f0: 0000 0000 0000 0000 7c01 7c02 7c04 ac06  ........|.|.|...
+00001700: a603 0000 ab03 0000 0000 0000 0000 0100  ................
+00001710: 6401 5300 2907 e10d 0200 0054 656d 706c  d.S.)......Templ
+00001720: 6174 6520 666f 7220 6120 6d6f 6465 6c20  ate for a model 
+00001730: 7769 7468 2061 7379 6d6d 6574 7269 6320  with asymmetric 
+00001740: 6c6f 6769 7374 6963 2074 7265 6e64 2028  logistic trend (
+00001750: 6d75 2920 616e 6420 706f 6c79 6e6f 6d69  mu) and polynomi
+00001760: 616c 2073 6967 6d61 2028 6173 2061 2066  al sigma (as a f
+00001770: 756e 6374 696f 6e20 6f66 206d 7529 2e0a  unction of mu)..
+00001780: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00001790: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+000017a0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2069  ------.        i
+000017b0: 6e64 6570 656e 6465 6e74 5f6b 6579 203a  ndependent_key :
+000017c0: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+000017d0: 206e 616d 6520 6f66 2074 6865 2069 6e64   name of the ind
+000017e0: 6570 656e 6465 6e74 2076 6172 6961 626c  ependent variabl
+000017f0: 650a 2020 2020 2020 2020 6465 7065 6e64  e.        depend
+00001800: 656e 745f 6b65 7920 3a20 7374 720a 2020  ent_key : str.  
+00001810: 2020 2020 2020 2020 2020 6e61 6d65 206f            name o
+00001820: 6620 7468 6520 6465 7065 6e64 656e 7420  f the dependent 
+00001830: 7661 7269 6162 6c65 0a20 2020 2020 2020  variable.       
+00001840: 2073 6967 6d61 5f64 6567 7265 6520 3a20   sigma_degree : 
+00001850: 6f70 7469 6f6e 616c 2c20 696e 740a 2020  optional, int.  
+00001860: 2020 2020 2020 2020 2020 6465 6772 6565            degree
+00001870: 206f 6620 7468 6520 706f 6c79 6e6f 6d69   of the polynomi
+00001880: 616c 206d 6f64 656c 2064 6573 6372 6962  al model describ
+00001890: 696e 6720 7468 6520 7369 676d 6120 6173  ing the sigma as
+000018a0: 2061 2066 756e 6374 696f 6e20 6f66 206d   a function of m
+000018b0: 750a 2020 2020 2020 2020 7468 6574 615f  u.        theta_
+000018c0: 6e61 6d65 7320 3a20 6f70 7469 6f6e 616c  names : optional
+000018d0: 2c20 7475 706c 6520 6f66 2073 7472 0a20  , tuple of str. 
+000018e0: 2020 2020 2020 2020 2020 206d 6179 2062             may b
+000018f0: 6520 7573 6564 2074 6f20 7365 7420 7468  e used to set th
+00001900: 6520 6e61 6d65 7320 6f66 2074 6865 206d  e names of the m
+00001910: 6f64 656c 2070 6172 616d 6574 6572 730a  odel parameters.
+00001920: 2020 2020 2020 2020 4e7a 0f4c 5f4c 2c4c          Nz.L_L,L
+00001930: 5f55 2c49 5f78 2c53 2c63 fa01 2c63 0100  _U,I_x,S,c..,c..
+00001940: 0000 0000 0000 0000 0000 0300 0000 3300  ..............3.
+00001950: 0000 f320 0000 004b 0001 0097 007c 005d  ... ...K.....|.]
+00001960: 097d 0164 007c 019b 009d 0256 0097 0101  .}.d.|.....V....
+00001970: 008c 0a64 0153 0072 1e00 0000 7216 0000  ...d.S.r....r...
+00001980: 0072 1700 0000 7302 0000 0020 2072 1a00  .r....s....  r..
+00001990: 0000 721b 0000 007a 3342 6173 6541 7379  ..r....z3BaseAsy
+000019a0: 6d6d 6574 7269 634c 6f67 6973 7469 634e  mmetricLogisticN
+000019b0: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
+000019c0: 733e 2e3c 6765 6e65 7870 723e 7f00 0000  s>.<genexpr>....
+000019d0: 7341 0000 00e8 00e8 0080 00f0 0002 4601  sA............F.
+000019e0: 0ef0 0002 4601 0ed8 2122 900c 9811 900c  ....F...!"......
+000019f0: 900c f003 0246 010e f000 0246 010e f000  .....F.....F....
+00001a00: 0246 010e f000 0246 010e f000 0246 010e  .F.....F.....F..
+00001a10: f000 0246 010e 721c 0000 0072 0900 0000  ...F..r....r....
+00001a20: a901 720f 0000 00a9 0872 0800 0000 7221  ..r......r....r!
+00001a30: 0000 0072 0e00 0000 7222 0000 00da 0573  ...r....r".....s
+00001a40: 706c 6974 7223 0000 0072 2400 0000 7225  plitr#...r$...r%
+00001a50: 0000 00a9 0672 2600 0000 7210 0000 0072  .....r&...r....r
+00001a60: 1100 0000 720e 0000 0072 0f00 0000 7227  ....r....r....r'
+00001a70: 0000 0073 0600 0000 2020 2020 2080 721a  ...s....     .r.
+00001a80: 0000 0072 2500 0000 7a20 4261 7365 4173  ...r%...z BaseAs
+00001a90: 796d 6d65 7472 6963 4c6f 6769 7374 6963  ymmetricLogistic
+00001aa0: 4e2e 5f5f 696e 6974 5f5f 6800 0000 73a2  N.__init__h...s.
+00001ab0: 0000 00f8 8000 f52a 001d 22d4 1c34 b05c  .......*.."..4.\
+00001ac0: d11c 42d4 1c42 8804 d408 19d8 0b16 d00b  ..B..B..........
+00001ad0: 1edd 1a1f d020 31d7 2037 d220 37b8 03d1  ..... 1. 7. 7...
+00001ae0: 203c d420 3cd1 1a3d d41a 3dc5 05f0 0002   <. <..=..=.....
+00001af0: 4601 0ef0 0002 4601 0edd 262b a84c b831  F.....F...&+.L.1
+00001b00: d12c 3cd1 263d d426 3df0 0302 4601 0ef1  .,<.&=.&=...F...
+00001b10: 0002 4601 0ef4 0002 4601 0ef1 0002 4101  ..F.....F.....A.
+00001b20: 0ef4 0002 4101 0ef1 0002 1b0e 884b f506  ....A........K..
+00001b30: 0009 0e89 078c 07d7 0818 d208 1898 1fa8  ................
+00001b40: 2dc0 5bd0 0818 d108 51d4 0851 d008 51d0  -.[.....Q..Q..Q.
+00001b50: 0851 d008 5172 1c00 0000 7228 0000 0063  .Q..Qr....r(...c
+00001b60: 0200 0000 0000 0000 0100 0000 0600 0000  ................
+00001b70: 0300 0000 f3b8 0000 0097 007c 0280 077c  ...........|...|
+00001b80: 006a 0000 0000 0000 0000 007d 0274 0300  .j.........}.t..
+00001b90: 0000 0000 0000 0000 006a 0200 0000 0000  .........j......
+00001ba0: 0000 007c 017c 0264 0164 0285 0219 0000  ...|.|.d.d......
+00001bb0: 0000 0000 0000 00a6 0200 00ab 0200 0000  ................
+00001bc0: 0000 0000 007d 037c 006a 0300 0000 0000  .....}.|.j......
+00001bd0: 0000 0064 036b 0200 0000 0072 097c 0264  ...d.k.....r.|.d
+00001be0: 0419 0000 0000 0000 0000 007d 046e 1d74  ...........}.n.t
+00001bf0: 0300 0000 0000 0000 0000 006a 0400 0000  ...........j....
+00001c00: 0000 0000 007c 037c 0264 0264 0185 0219  .....|.|.d.d....
+00001c10: 0000 0000 0000 0000 00a6 0200 00ab 0200  ................
+00001c20: 0000 0000 0000 007d 047c 037c 0466 0253  .......}.|.|.f.S
+00001c30: 0029 0561 1d03 0000 5072 6564 6963 7473  .).a....Predicts
+00001c40: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
+00001c50: 6d75 2061 6e64 2073 6967 6d61 206f 6620  mu and sigma of 
+00001c60: 6120 6e6f 726d 616c 2064 6973 7472 6962  a normal distrib
+00001c70: 7574 696f 6e20 7768 6963 680a 2020 2020  ution which.    
+00001c80: 2020 2020 6368 6172 6163 7465 7269 7a65      characterize
+00001c90: 7320 7468 6520 6465 7065 6e64 656e 7420  s the dependent 
+00001ca0: 7661 7269 6162 6c65 2067 6976 656e 2076  variable given v
+00001cb0: 616c 7565 7320 6f66 2074 6865 2069 6e64  alues of the ind
+00001cc0: 6570 656e 6465 6e74 2076 6172 6961 626c  ependent variabl
+00001cd0: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
+00001ce0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+00001cf0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00001d00: 2020 7820 3a20 6172 7261 792d 6c69 6b65    x : array-like
+00001d10: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00001d20: 7565 7320 6f66 2074 6865 2069 6e64 6570  ues of the indep
+00001d30: 656e 6465 6e74 2076 6172 6961 626c 650a  endent variable.
+00001d40: 2020 2020 2020 2020 7468 6574 6120 3a20          theta : 
+00001d50: 6f70 7469 6f6e 616c 2c20 6172 7261 792d  optional, array-
+00001d60: 6c69 6b65 0a20 2020 2020 2020 2020 2020  like.           
+00001d70: 2070 6172 616d 6574 6572 2076 6563 746f   parameter vecto
+00001d80: 7220 6f66 2074 6865 2063 616c 6962 7261  r of the calibra
+00001d90: 7469 6f6e 206d 6f64 656c 3a0a 2020 2020  tion model:.    
+00001da0: 2020 2020 2020 2020 2020 2020 3520 7061              5 pa
+00001db0: 7261 6d65 7465 7273 206f 6620 6173 796d  rameters of asym
+00001dc0: 6d65 7472 6963 206c 6f67 6973 7469 6320  metric logistic 
+00001dd0: 6d6f 6465 6c20 666f 7220 6d75 0a20 2020  model for mu.   
+00001de0: 2020 2020 2020 2020 2020 2020 205b 7369               [si
+00001df0: 676d 615f 6465 6772 6565 5d20 7061 7261  gma_degree] para
+00001e00: 6d65 7465 7273 2066 6f72 2073 6967 6d61  meters for sigma
+00001e10: 2028 6c6f 7765 7374 2064 6567 7265 6520   (lowest degree 
+00001e20: 6669 7273 7429 0a0a 2020 2020 2020 2020  first)..        
+00001e30: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00001e40: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00001e50: 6d75 203a 2061 7272 6179 2d6c 696b 650a  mu : array-like.
+00001e60: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00001e70: 6573 2066 6f72 2074 6865 206d 7520 7061  es for the mu pa
+00001e80: 7261 6d65 7465 7220 6f66 2061 206e 6f72  rameter of a nor
+00001e90: 6d61 6c20 6469 7374 7269 6275 7469 6f6e  mal distribution
+00001ea0: 2064 6573 6372 6962 696e 6720 7468 6520   describing the 
+00001eb0: 6465 7065 6e64 656e 7420 7661 7269 6162  dependent variab
+00001ec0: 6c65 0a20 2020 2020 2020 2073 6967 6d61  le.        sigma
+00001ed0: 203a 2061 7272 6179 2d6c 696b 6520 6f72   : array-like or
+00001ee0: 2066 6c6f 6174 0a20 2020 2020 2020 2020   float.         
+00001ef0: 2020 2076 616c 7565 7320 666f 7220 7468     values for th
+00001f00: 6520 7369 676d 6120 7061 7261 6d65 7465  e sigma paramete
+00001f10: 7220 6f66 2061 206e 6f72 6d61 6c20 6469  r of a normal di
+00001f20: 7374 7269 6275 7469 6f6e 2064 6573 6372  stribution descr
+00001f30: 6962 696e 6720 7468 6520 6465 7065 6e64  ibing the depend
+00001f40: 656e 7420 7661 7269 6162 6c65 0a20 2020  ent variable.   
+00001f50: 2020 2020 204e e905 0000 0072 0200 0000       N.....r....
+00001f60: 722b 0000 0029 0572 2c00 0000 7207 0000  r+...).r,...r...
+00001f70: 00da 1361 7379 6d6d 6574 7269 635f 6c6f  ...asymmetric_lo
+00001f80: 6769 7374 6963 720e 0000 0072 2d00 0000  gisticr....r-...
+00001f90: 722e 0000 0073 0500 0000 2020 2020 2072  r....s....     r
+00001fa0: 1a00 0000 7232 0000 007a 2942 6173 6541  ....r2...z)BaseA
+00001fb0: 7379 6d6d 6574 7269 634c 6f67 6973 7469  symmetricLogisti
+00001fc0: 634e 2e70 7265 6469 6374 5f64 6570 656e  cN.predict_depen
+00001fd0: 6465 6e74 8400 0000 7367 0000 0080 00f0  dent....sg......
+00001fe0: 2800 0c11 883d d814 18d4 1425 8845 dd0d  (....=.....%.E..
+00001ff0: 11d4 0d25 a061 a815 a872 b001 a872 ac19  ...%.a...r...r..
+00002000: d10d 33d4 0d33 8802 d80b 0fd4 0b1c a001  ..3..3..........
+00002010: d20b 21d0 0b21 d814 1998 2294 4988 4588  ..!..!....".I.E.
+00002020: 45e5 1418 944f a042 a805 a861 a862 a862  E....O.B...a.b.b
+00002030: ac09 d114 32d4 1432 8845 d80f 1190 3588  ....2..2.E....5.
+00002040: 79d0 0818 721c 0000 0063 0200 0000 0000  y...r....c......
+00002050: 0000 0100 0000 0600 0000 0300 0000 f34e  ...............N
+00002060: 0000 0097 007c 0280 077c 006a 0000 0000  .....|...|.j....
+00002070: 0000 0000 007d 0274 0300 0000 0000 0000  .....}.t........
+00002080: 0000 006a 0200 0000 0000 0000 007c 017c  ...j.........|.|
+00002090: 0264 0164 0285 0219 0000 0000 0000 0000  .d.d............
+000020a0: 00a6 0200 00ab 0200 0000 0000 0000 0053  ...............S
+000020b0: 0029 0361 fe01 0000 5072 6564 6963 7420  .).a....Predict 
+000020c0: 7468 6520 696e 6465 7065 6e64 656e 7420  the independent 
+000020d0: 7661 7269 6162 6c65 2075 7369 6e67 2074  variable using t
+000020e0: 6865 2069 6e76 6572 7365 2074 7265 6e64  he inverse trend
+000020f0: 206d 6f64 656c 2e0a 0a20 2020 2020 2020   model...       
+00002100: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00002110: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00002120: 2020 2020 2020 2079 203a 2061 7272 6179         y : array
+00002130: 2d6c 696b 650a 2020 2020 2020 2020 2020  -like.          
+00002140: 2020 6f62 7365 7276 6174 696f 6e73 0a20    observations. 
+00002150: 2020 2020 2020 2074 6865 7461 203a 206f         theta : o
+00002160: 7074 696f 6e61 6c2c 2061 7272 6179 2d6c  ptional, array-l
+00002170: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
+00002180: 7061 7261 6d65 7465 7220 7665 6374 6f72  parameter vector
+00002190: 206f 6620 7468 6520 6361 6c69 6272 6174   of the calibrat
+000021a0: 696f 6e20 6d6f 6465 6c3a 0a20 2020 2020  ion model:.     
+000021b0: 2020 2020 2020 2020 2020 2035 2070 6172             5 par
+000021c0: 616d 6574 6572 7320 6f66 2061 7379 6d6d  ameters of asymm
+000021d0: 6574 7269 6320 6c6f 6769 7374 6963 206d  etric logistic m
+000021e0: 6f64 656c 2066 6f72 206d 750a 2020 2020  odel for mu.    
+000021f0: 2020 2020 2020 2020 2020 2020 5b73 6967              [sig
+00002200: 6d61 5f64 6567 7265 655d 2070 6172 616d  ma_degree] param
+00002210: 6574 6572 7320 666f 7220 7369 676d 6120  eters for sigma 
+00002220: 286c 6f77 6573 7420 6465 6772 6565 2066  (lowest degree f
+00002230: 6972 7374 290a 0a20 2020 2020 2020 2052  irst)..        R
+00002240: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00002250: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
+00002260: 203a 2061 7272 6179 2d6c 696b 650a 2020   : array-like.  
+00002270: 2020 2020 2020 2020 2020 7072 6564 6963            predic
+00002280: 7465 6420 696e 6465 7065 6e64 656e 7420  ted independent 
+00002290: 7661 6c75 6573 2067 6976 656e 2074 6865  values given the
+000022a0: 206f 6273 6572 7661 7469 6f6e 730a 2020   observations.  
+000022b0: 2020 2020 2020 4e72 4c00 0000 2903 722c        NrL...).r,
+000022c0: 0000 0072 0700 0000 da1b 696e 7665 7273  ...r......invers
+000022d0: 655f 6173 796d 6d65 7472 6963 5f6c 6f67  e_asymmetric_log
+000022e0: 6973 7469 63a9 0372 2600 0000 7235 0000  istic..r&...r5..
+000022f0: 0072 2900 0000 7303 0000 0020 2020 721a  .r)...s....   r.
+00002300: 0000 0072 3800 0000 7a2b 4261 7365 4173  ...r8...z+BaseAs
+00002310: 796d 6d65 7472 6963 4c6f 6769 7374 6963  ymmetricLogistic
+00002320: 4e2e 7072 6564 6963 745f 696e 6465 7065  N.predict_indepe
+00002330: 6e64 656e 74a1 0000 0073 2c00 0000 8000  ndent....s,.....
+00002340: f022 000c 1188 3dd8 1418 d414 2588 45dd  ."....=.....%.E.
+00002350: 0f13 d40f 2fb0 01b0 35b8 12b8 21b8 12b4  ..../...5...!...
+00002360: 39d1 0f3d d40f 3dd0 083d 721c 0000 0072  9..=..=..=r....r
+00002370: 3900 0000 7240 0000 0073 0100 0000 4072  9...r@...s....@r
+00002380: 1a00 0000 7242 0000 0072 4200 0000 6700  ....rB...rB...g.
+00002390: 0000 73c8 0000 00f8 8000 8000 8000 8000  ..s.............
+000023a0: 8000 f00c 001d 1ed8 2f33 f00d 1a05 5201  ......../3....R.
+000023b0: f000 1a05 5201 f000 1a05 5201 f006 001a  ....R.....R.....
+000023c0: 1df0 071a 0552 01f0 0800 181b f009 1a05  .....R..........
+000023d0: 5201 f00a 0017 1af0 0b1a 0552 01f0 0c00  R..........R....
+000023e0: 161e 9868 a073 9c6d d415 2cf0 0d1a 0552  ...h.s.m..,....R
+000023f0: 01f0 001a 0552 01f0 001a 0552 01f0 001a  .....R.....R....
+00002400: 0552 01f0 001a 0552 01f0 001a 0552 01f0  .R.....R.....R..
+00002410: 3800 2d31 f000 1b05 19f0 001b 0519 f000  8.-1............
+00002420: 1b05 19f0 001b 0519 f000 1b05 19f0 3a00  ..............:.
+00002430: 2f33 f000 1305 3ef0 0013 053e f000 1305  /3....>....>....
+00002440: 3ef0 0013 053e f000 1305 3ef0 0013 053e  >....>....>....>
+00002450: f000 1305 3ef0 0013 053e f000 1305 3e72  ....>....>....>r
+00002460: 1c00 0000 7242 0000 0063 0000 0000 0000  ....rB...c......
+00002470: 0000 0000 0000 0b00 0000 0000 0000 f368  ...............h
+00002480: 0000 0087 0097 0065 005a 0164 005a 0264  .......e.Z.d.Z.d
+00002490: 0164 0264 039c 0264 0465 0364 0565 0364  .d.d...d.e.d.e.d
+000024a0: 0665 0464 0765 0565 0665 0319 0000 0000  .e.d.e.e.e......
+000024b0: 0000 0000 0019 0000 0000 0000 0000 0066  ...............f
+000024c0: 0888 0066 0164 0884 0e5a 0764 0264 099c  ...f.d...Z.d.d..
+000024d0: 0164 0a84 025a 0864 0264 099c 0164 0b84  .d...Z.d.d...d..
+000024e0: 025a 0988 0078 015a 0a53 0029 0cda 2542  .Z...x.Z.S.)..%B
+000024f0: 6173 654c 6f67 496e 6465 7065 6e64 656e  aseLogIndependen
+00002500: 7441 7379 6d6d 6574 7269 634c 6f67 6973  tAsymmetricLogis
+00002510: 7469 634e 7202 0000 004e 720d 0000 0072  ticNr....Nr....r
+00002520: 1000 0000 7211 0000 0072 0e00 0000 720f  ....r....r....r.
+00002530: 0000 0063 0100 0000 0000 0000 0400 0000  ...c............
+00002540: 0800 0000 0300 0000 f31e 0100 0095 0197  ................
+00002550: 0074 0100 0000 0000 0000 0000 006a 0100  .t...........j..
+00002560: 0000 0000 0000 007c 03a6 0100 00ab 0100  .......|........
+00002570: 0000 0000 0000 007c 005f 0200 0000 0000  .......|._......
+00002580: 0000 007c 0480 4c74 0700 0000 0000 0000  ...|..Lt........
+00002590: 0000 0064 02a0 0400 0000 0000 0000 0000  ...d............
+000025a0: 0000 0000 0000 0000 0000 0064 03a6 0100  ...........d....
+000025b0: 00ab 0100 0000 0000 0000 00a6 0100 00ab  ................
+000025c0: 0100 0000 0000 0000 0074 0700 0000 0000  .........t......
+000025d0: 0000 0000 0064 0484 0074 0b00 0000 0000  .....d...t......
+000025e0: 0000 0000 007c 0364 057a 0000 00a6 0100  .....|.d.z......
+000025f0: 00ab 0100 0000 0000 0000 0044 00a6 0000  ...........D....
+00002600: 00ab 0000 0000 0000 0000 00a6 0100 00ab  ................
+00002610: 0100 0000 0000 0000 007a 0000 007d 0474  .........z...}.t
+00002620: 0d00 0000 0000 0000 0000 00a6 0000 00ab  ................
+00002630: 0000 0000 0000 0000 00a0 0700 0000 0000  ................
+00002640: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
+00002650: 017c 027c 04ac 06a6 0300 00ab 0300 0000  .|.|............
+00002660: 0000 0000 0001 0064 0153 0029 0772 4400  .......d.S.).rD.
+00002670: 0000 4e7a 134c 5f4c 2c4c 5f55 2c6c 6f67  ..Nz.L_L,L_U,log
+00002680: 5f49 5f78 2c53 2c63 7245 0000 0063 0100  _I_x,S,crE...c..
+00002690: 0000 0000 0000 0000 0000 0300 0000 3300  ..............3.
+000026a0: 0000 f320 0000 004b 0001 0097 007c 005d  ... ...K.....|.]
+000026b0: 097d 0164 007c 019b 009d 0256 0097 0101  .}.d.|.....V....
+000026c0: 008c 0a64 0153 0072 1e00 0000 7216 0000  ...d.S.r....r...
+000026d0: 0072 1700 0000 7302 0000 0020 2072 1a00  .r....s....  r..
+000026e0: 0000 721b 0000 007a 4142 6173 654c 6f67  ..r....zABaseLog
+000026f0: 496e 6465 7065 6e64 656e 7441 7379 6d6d  IndependentAsymm
+00002700: 6574 7269 634c 6f67 6973 7469 634e 2e5f  etricLogisticN._
+00002710: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
+00002720: 2e3c 6765 6e65 7870 723e cf00 0000 7341  .<genexpr>....sA
+00002730: 0000 00e8 00e8 0080 00f0 0002 4a01 0ef0  ............J...
+00002740: 0002 4a01 0ed8 2122 900c 9811 900c 900c  ..J...!"........
+00002750: f003 024a 010e f000 024a 010e f000 024a  ...J.....J.....J
+00002760: 010e f000 024a 010e f000 024a 010e f000  .....J.....J....
+00002770: 024a 010e 721c 0000 0072 0900 0000 7247  .J..r....r....rG
+00002780: 0000 0072 4800 0000 724a 0000 0073 0600  ...rH...rJ...s..
+00002790: 0000 2020 2020 2080 721a 0000 0072 2500  ..     .r....r%.
+000027a0: 0000 7a2e 4261 7365 4c6f 6749 6e64 6570  ..z.BaseLogIndep
+000027b0: 656e 6465 6e74 4173 796d 6d65 7472 6963  endentAsymmetric
+000027c0: 4c6f 6769 7374 6963 4e2e 5f5f 696e 6974  LogisticN.__init
+000027d0: 5f5f b800 0000 73a2 0000 00f8 8000 f52a  __....s........*
+000027e0: 001d 22d4 1c34 b05c d11c 42d4 1c42 8804  .."..4.\..B..B..
+000027f0: d408 19d8 0b16 d00b 1edd 1a1f d020 35d7  ............. 5.
+00002800: 203b d220 3bb8 43d1 2040 d420 40d1 1a41   ;. ;.C. @. @..A
+00002810: d41a 41c5 45f0 0002 4a01 0ef0 0002 4a01  ..A.E...J.....J.
+00002820: 0edd 262b a84c b831 d12c 3cd1 263d d426  ..&+.L.1.,<.&=.&
+00002830: 3df0 0302 4a01 0ef1 0002 4a01 0ef4 0002  =...J.....J.....
+00002840: 4a01 0ef1 0002 4501 0ef4 0002 4501 0ef1  J.....E.....E...
+00002850: 0002 1b0e 884b f506 0009 0e89 078c 07d7  .....K..........
+00002860: 0818 d208 1898 1fa8 2dc0 5bd0 0818 d108  ........-.[.....
+00002870: 51d4 0851 d008 51d0 0851 d008 5172 1c00  Q..Q..Q..Q..Qr..
+00002880: 0000 7228 0000 0063 0200 0000 0000 0000  ..r(...c........
+00002890: 0100 0000 0600 0000 0300 0000 f3b8 0000  ................
+000028a0: 0097 007c 0280 077c 006a 0000 0000 0000  ...|...|.j......
+000028b0: 0000 007d 0274 0300 0000 0000 0000 0000  ...}.t..........
+000028c0: 006a 0200 0000 0000 0000 007c 017c 0264  .j.........|.|.d
+000028d0: 0164 0285 0219 0000 0000 0000 0000 00a6  .d..............
+000028e0: 0200 00ab 0200 0000 0000 0000 007d 037c  .............}.|
+000028f0: 006a 0300 0000 0000 0000 0064 036b 0200  .j.........d.k..
+00002900: 0000 0072 097c 0264 0419 0000 0000 0000  ...r.|.d........
+00002910: 0000 007d 046e 1d74 0300 0000 0000 0000  ...}.n.t........
+00002920: 0000 006a 0400 0000 0000 0000 007c 037c  ...j.........|.|
+00002930: 0264 0264 0185 0219 0000 0000 0000 0000  .d.d............
+00002940: 00a6 0200 00ab 0200 0000 0000 0000 007d  ...............}
+00002950: 047c 037c 0466 0253 0029 0561 2d03 0000  .|.|.f.S.).a-...
+00002960: 5072 6564 6963 7473 2074 6865 2070 6172  Predicts the par
+00002970: 616d 6574 6572 7320 6d75 2061 6e64 2073  ameters mu and s
+00002980: 6967 6d61 206f 6620 6120 6e6f 726d 616c  igma of a normal
+00002990: 2064 6973 7472 6962 7574 696f 6e20 7768   distribution wh
+000029a0: 6963 680a 2020 2020 2020 2020 6368 6172  ich.        char
+000029b0: 6163 7465 7269 7a65 7320 7468 6520 6465  acterizes the de
+000029c0: 7065 6e64 656e 7420 7661 7269 6162 6c65  pendent variable
+000029d0: 2067 6976 656e 2076 616c 7565 7320 6f66   given values of
+000029e0: 2074 6865 2069 6e64 6570 656e 6465 6e74   the independent
+000029f0: 2076 6172 6961 626c 652e 0a0a 2020 2020   variable...    
+00002a00: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00002a10: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00002a20: 2d0a 2020 2020 2020 2020 7820 3a20 6172  -.        x : ar
+00002a30: 7261 792d 6c69 6b65 0a20 2020 2020 2020  ray-like.       
+00002a40: 2020 2020 2076 616c 7565 7320 6f66 2074       values of t
+00002a50: 6865 2069 6e64 6570 656e 6465 6e74 2076  he independent v
+00002a60: 6172 6961 626c 650a 2020 2020 2020 2020  ariable.        
+00002a70: 7468 6574 6120 3a20 6f70 7469 6f6e 616c  theta : optional
+00002a80: 2c20 6172 7261 792d 6c69 6b65 0a20 2020  , array-like.   
+00002a90: 2020 2020 2020 2020 2070 6172 616d 6574           paramet
+00002aa0: 6572 2076 6563 746f 7220 6f66 2074 6865  er vector of the
+00002ab0: 2063 616c 6962 7261 7469 6f6e 206d 6f64   calibration mod
+00002ac0: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
+00002ad0: 2020 2020 3520 7061 7261 6d65 7465 7273      5 parameters
+00002ae0: 206f 6620 6c6f 672d 696e 6465 7065 6e64   of log-independ
+00002af0: 656e 7420 6173 796d 6d65 7472 6963 206c  ent asymmetric l
+00002b00: 6f67 6973 7469 6320 6d6f 6465 6c20 666f  ogistic model fo
+00002b10: 7220 6d75 0a20 2020 2020 2020 2020 2020  r mu.           
+00002b20: 2020 2020 205b 7369 676d 615f 6465 6772       [sigma_degr
+00002b30: 6565 5d20 7061 7261 6d65 7465 7273 2066  ee] parameters f
+00002b40: 6f72 2073 6967 6d61 2028 6c6f 7765 7374  or sigma (lowest
+00002b50: 2064 6567 7265 6520 6669 7273 7429 0a0a   degree first)..
+00002b60: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00002b70: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00002b80: 2020 2020 2020 2020 6d75 203a 2061 7272          mu : arr
+00002b90: 6179 2d6c 696b 650a 2020 2020 2020 2020  ay-like.        
+00002ba0: 2020 2020 7661 6c75 6573 2066 6f72 2074      values for t
+00002bb0: 6865 206d 7520 7061 7261 6d65 7465 7220  he mu parameter 
+00002bc0: 6f66 2061 206e 6f72 6d61 6c20 6469 7374  of a normal dist
+00002bd0: 7269 6275 7469 6f6e 2064 6573 6372 6962  ribution describ
+00002be0: 696e 6720 7468 6520 6465 7065 6e64 656e  ing the dependen
+00002bf0: 7420 7661 7269 6162 6c65 0a20 2020 2020  t variable.     
+00002c00: 2020 2073 6967 6d61 203a 2061 7272 6179     sigma : array
+00002c10: 2d6c 696b 6520 6f72 2066 6c6f 6174 0a20  -like or float. 
+00002c20: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00002c30: 7320 666f 7220 7468 6520 7369 676d 6120  s for the sigma 
+00002c40: 7061 7261 6d65 7465 7220 6f66 2061 206e  parameter of a n
+00002c50: 6f72 6d61 6c20 6469 7374 7269 6275 7469  ormal distributi
+00002c60: 6f6e 2064 6573 6372 6962 696e 6720 7468  on describing th
+00002c70: 6520 6465 7065 6e64 656e 7420 7661 7269  e dependent vari
+00002c80: 6162 6c65 0a20 2020 2020 2020 204e 724c  able.        NrL
+00002c90: 0000 0072 0200 0000 722b 0000 0029 0572  ...r....r+...).r
+00002ca0: 2c00 0000 7207 0000 00da 1878 6c6f 675f  ,...r......xlog_
+00002cb0: 6173 796d 6d65 7472 6963 5f6c 6f67 6973  asymmetric_logis
+00002cc0: 7469 6372 0e00 0000 722d 0000 0072 2e00  ticr....r-...r..
+00002cd0: 0000 7305 0000 0020 2020 2020 721a 0000  ..s....     r...
+00002ce0: 0072 3200 0000 7a37 4261 7365 4c6f 6749  .r2...z7BaseLogI
+00002cf0: 6e64 6570 656e 6465 6e74 4173 796d 6d65  ndependentAsymme
+00002d00: 7472 6963 4c6f 6769 7374 6963 4e2e 7072  tricLogisticN.pr
+00002d10: 6564 6963 745f 6465 7065 6e64 656e 74d4  edict_dependent.
+00002d20: 0000 0073 6700 0000 8000 f028 000c 1188  ...sg......(....
+00002d30: 3dd8 1418 d414 2588 45dd 0d11 d40d 2aa8  =.....%.E.....*.
+00002d40: 31a8 65b0 42b0 51b0 42ac 69d1 0d38 d40d  1.e.B.Q.B.i..8..
+00002d50: 3888 02d8 0b0f d40b 1ca0 01d2 0b21 d00b  8............!..
+00002d60: 21d8 1419 9822 9449 8845 8845 e514 1894  !....".I.E.E....
+00002d70: 4fa0 42a8 05a8 61a8 62a8 62ac 09d1 1432  O.B...a.b.b....2
+00002d80: d414 3288 45d8 0f11 9035 8879 d008 1872  ..2.E....5.y...r
+00002d90: 1c00 0000 6302 0000 0000 0000 0001 0000  ....c...........
+00002da0: 0006 0000 0003 0000 00f3 4e00 0000 9700  ..........N.....
+00002db0: 7c02 8007 7c00 6a00 0000 0000 0000 0000  |...|.j.........
+00002dc0: 7d02 7403 0000 0000 0000 0000 0000 6a02  }.t...........j.
+00002dd0: 0000 0000 0000 0000 7c01 7c02 6401 6402  ........|.|.d.d.
+00002de0: 8502 1900 0000 0000 0000 0000 a602 0000  ................
+00002df0: ab02 0000 0000 0000 0000 5300 2903 610e  ..........S.).a.
+00002e00: 0200 0050 7265 6469 6374 2074 6865 2069  ...Predict the i
+00002e10: 6e64 6570 656e 6465 6e74 2076 6172 6961  ndependent varia
+00002e20: 626c 6520 7573 696e 6720 7468 6520 696e  ble using the in
+00002e30: 7665 7273 6520 7472 656e 6420 6d6f 6465  verse trend mode
+00002e40: 6c2e 0a0a 2020 2020 2020 2020 5061 7261  l...        Para
+00002e50: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+00002e60: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00002e70: 2020 7920 3a20 6172 7261 792d 6c69 6b65    y : array-like
+00002e80: 0a20 2020 2020 2020 2020 2020 206f 6273  .            obs
+00002e90: 6572 7661 7469 6f6e 730a 2020 2020 2020  ervations.      
+00002ea0: 2020 7468 6574 6120 3a20 6f70 7469 6f6e    theta : option
+00002eb0: 616c 2c20 6172 7261 792d 6c69 6b65 0a20  al, array-like. 
+00002ec0: 2020 2020 2020 2020 2020 2070 6172 616d             param
+00002ed0: 6574 6572 2076 6563 746f 7220 6f66 2074  eter vector of t
+00002ee0: 6865 2063 616c 6962 7261 7469 6f6e 206d  he calibration m
+00002ef0: 6f64 656c 3a0a 2020 2020 2020 2020 2020  odel:.          
+00002f00: 2020 2020 2020 3520 7061 7261 6d65 7465        5 paramete
+00002f10: 7273 206f 6620 6c6f 672d 696e 6465 7065  rs of log-indepe
+00002f20: 6e64 656e 7420 6173 796d 6d65 7472 6963  ndent asymmetric
+00002f30: 206c 6f67 6973 7469 6320 6d6f 6465 6c20   logistic model 
+00002f40: 666f 7220 6d75 0a20 2020 2020 2020 2020  for mu.         
+00002f50: 2020 2020 2020 205b 7369 676d 615f 6465         [sigma_de
+00002f60: 6772 6565 5d20 7061 7261 6d65 7465 7273  gree] parameters
+00002f70: 2066 6f72 2073 6967 6d61 2028 6c6f 7765   for sigma (lowe
+00002f80: 7374 2064 6567 7265 6520 6669 7273 7429  st degree first)
+00002f90: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00002fa0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00002fb0: 2d0a 2020 2020 2020 2020 7820 3a20 6172  -.        x : ar
+00002fc0: 7261 792d 6c69 6b65 0a20 2020 2020 2020  ray-like.       
+00002fd0: 2020 2020 2070 7265 6469 6374 6564 2069       predicted i
+00002fe0: 6e64 6570 656e 6465 6e74 2076 616c 7565  ndependent value
+00002ff0: 7320 6769 7665 6e20 7468 6520 6f62 7365  s given the obse
+00003000: 7276 6174 696f 6e73 0a20 2020 2020 2020  rvations.       
+00003010: 204e 724c 0000 0029 0372 2c00 0000 7207   NrL...).r,...r.
+00003020: 0000 00da 2069 6e76 6572 7365 5f78 6c6f  .... inverse_xlo
+00003030: 675f 6173 796d 6d65 7472 6963 5f6c 6f67  g_asymmetric_log
+00003040: 6973 7469 6372 5000 0000 7303 0000 0020  isticrP...s.... 
+00003050: 2020 721a 0000 0072 3800 0000 7a39 4261    r....r8...z9Ba
+00003060: 7365 4c6f 6749 6e64 6570 656e 6465 6e74  seLogIndependent
+00003070: 4173 796d 6d65 7472 6963 4c6f 6769 7374  AsymmetricLogist
+00003080: 6963 4e2e 7072 6564 6963 745f 696e 6465  icN.predict_inde
+00003090: 7065 6e64 656e 74f1 0000 0073 2c00 0000  pendent....s,...
+000030a0: 8000 f022 000c 1188 3dd8 1418 d414 2588  ..."....=.....%.
+000030b0: 45dd 0f13 d40f 34b0 51b8 05b8 62b8 71b8  E.....4.Q...b.q.
+000030c0: 62bc 09d1 0f42 d40f 42d0 0842 721c 0000  b....B..B..Br...
+000030d0: 0072 3900 0000 7240 0000 0073 0100 0000  .r9...r@...s....
+000030e0: 4072 1a00 0000 7252 0000 0072 5200 0000  @r....rR...rR...
+000030f0: b700 0000 73d1 0000 00f8 8000 8000 8000  ....s...........
+00003100: 8000 8000 f00c 001d 1ed8 2f33 f00d 1a05  ........../3....
+00003110: 5201 f000 1a05 5201 f000 1a05 5201 f006  R.....R.....R...
+00003120: 001a 1df0 071a 0552 01f0 0800 181b f009  .......R........
+00003130: 1a05 5201 f00a 0017 1af0 0b1a 0552 01f0  ..R..........R..
+00003140: 0c00 161e 9868 a073 9c6d d415 2cf0 0d1a  .....h.s.m..,...
+00003150: 0552 01f0 001a 0552 01f0 001a 0552 01f0  .R.....R.....R..
+00003160: 001a 0552 01f0 001a 0552 01f0 001a 0552  ...R.....R.....R
+00003170: 01f0 3800 2d31 f000 1b05 19f0 001b 0519  ..8.-1..........
+00003180: f000 1b05 19f0 001b 0519 f000 1b05 19f0  ................
+00003190: 3a00 2f33 f000 1305 4301 f000 1305 4301  :./3....C.....C.
+000031a0: f000 1305 4301 f000 1305 4301 f000 1305  ....C.....C.....
+000031b0: 4301 f000 1305 4301 f000 1305 4301 f000  C.....C.....C...
+000031c0: 1305 4301 f000 1305 4301 721c 0000 0072  ..C.....C.r....r
+000031d0: 5200 0000 6300 0000 0000 0000 0000 0000  R...c...........
+000031e0: 000d 0000 0000 0000 00f3 7a00 0000 8700  ..........z.....
+000031f0: 9700 6500 5a01 6400 5a02 6401 6402 6402  ..e.Z.d.Z.d.d.d.
+00003200: 6403 9c03 6404 6503 6405 6503 6406 6504  d...d.e.d.e.d.e.
+00003210: 6407 6505 6506 1900 0000 0000 0000 0000  d.e.e...........
+00003220: 6408 6505 6507 6503 1900 0000 0000 0000  d.e.e.e.........
+00003230: 0000 1900 0000 0000 0000 0000 660a 8800  ............f...
+00003240: 6601 6409 840e 5a08 6402 640a 9c01 640b  f.d...Z.d.d...d.
+00003250: 8402 5a09 6402 640a 9c01 640c 8402 5a0a  ..Z.d.d...d...Z.
+00003260: 8800 7801 5a0b 5300 290d da15 4261 7365  ..x.Z.S.)...Base
+00003270: 4578 706f 6e65 6e74 6961 6c4d 6f64 656c  ExponentialModel
+00003280: 4e72 0200 0000 4e29 0372 0e00 0000 da0f  Nr....N).r......
+00003290: 6669 7865 645f 696e 7465 7263 6570 7472  fixed_interceptr
+000032a0: 0f00 0000 7210 0000 0072 1100 0000 720e  ....r....r....r.
+000032b0: 0000 0072 5b00 0000 720f 0000 0063 0100  ...r[...r....c..
+000032c0: 0000 0000 0000 0500 0000 0800 0000 0300  ................
+000032d0: 0000 f3fa 0000 0095 0197 0074 0100 0000  ...........t....
+000032e0: 0000 0000 0000 006a 0100 0000 0000 0000  .......j........
+000032f0: 007c 03a6 0100 00ab 0100 0000 0000 0000  .|..............
+00003300: 007c 005f 0200 0000 0000 0000 007c 047c  .|._.........|.|
+00003310: 005f 0300 0000 0000 0000 007c 0580 337c  ._.........|..3|
+00003320: 0481 0364 027d 066e 0264 037d 067c 0674  ...d.}.n.d.}.|.t
+00003330: 0900 0000 0000 0000 0000 0064 0484 0074  ...........d...t
+00003340: 0b00 0000 0000 0000 0000 007c 0364 057a  ...........|.d.z
+00003350: 0000 00a6 0100 00ab 0100 0000 0000 0000  ................
+00003360: 0044 00a6 0000 00ab 0000 0000 0000 0000  .D..............
+00003370: 00a6 0100 00ab 0100 0000 0000 0000 007a  ...............z
+00003380: 0000 007d 0574 0d00 0000 0000 0000 0000  ...}.t..........
+00003390: 00a6 0000 00ab 0000 0000 0000 0000 00a0  ................
+000033a0: 0700 0000 0000 0000 0000 0000 0000 0000  ................
+000033b0: 0000 0000 007c 017c 027c 05ac 06a6 0300  .....|.|.|......
+000033c0: 00ab 0300 0000 0000 0000 0001 0064 0153  .............d.S
+000033d0: 0029 0775 0a03 0000 5465 6d70 6c61 7465  .).u....Template
+000033e0: 2066 6f72 2061 206d 6f64 656c 2077 6974   for a model wit
+000033f0: 6820 6578 706f 6e65 6e74 6961 6c20 7472  h exponential tr
+00003400: 656e 6420 286d 7529 2061 6e64 2070 6f6c  end (mu) and pol
+00003410: 796e 6f6d 6961 6c20 7369 676d 6120 2861  ynomial sigma (a
+00003420: 7320 6120 6675 6e63 7469 6f6e 206f 6620  s a function of 
+00003430: 6d75 292e 0a0a 2020 2020 2020 2020 5061  mu)...        Pa
+00003440: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00003450: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00003460: 2020 2020 696e 6465 7065 6e64 656e 745f      independent_
+00003470: 6b65 7920 3a20 7374 720a 2020 2020 2020  key : str.      
+00003480: 2020 2020 2020 6e61 6d65 206f 6620 7468        name of th
+00003490: 6520 696e 6465 7065 6e64 656e 7420 7661  e independent va
+000034a0: 7269 6162 6c65 0a20 2020 2020 2020 2064  riable.        d
+000034b0: 6570 656e 6465 6e74 5f6b 6579 203a 2073  ependent_key : s
+000034c0: 7472 0a20 2020 2020 2020 2020 2020 206e  tr.            n
+000034d0: 616d 6520 6f66 2074 6865 2064 6570 656e  ame of the depen
+000034e0: 6465 6e74 2076 6172 6961 626c 650a 2020  dent variable.  
+000034f0: 2020 2020 2020 7369 676d 615f 6465 6772        sigma_degr
+00003500: 6565 203a 206f 7074 696f 6e61 6c2c 2069  ee : optional, i
+00003510: 6e74 0a20 2020 2020 2020 2020 2020 2064  nt.            d
+00003520: 6567 7265 6520 6f66 2074 6865 2070 6f6c  egree of the pol
+00003530: 796e 6f6d 6961 6c20 6d6f 6465 6c20 6465  ynomial model de
+00003540: 7363 7269 6269 6e67 2074 6865 2073 6967  scribing the sig
+00003550: 6d61 2061 7320 6120 6675 6e63 7469 6f6e  ma as a function
+00003560: 206f 6620 6d75 0a20 2020 2020 2020 2020   of mu.         
+00003570: 2020 20e2 9aa0 2041 7474 656e 7469 6f6e     ... Attention
+00003580: 3a20 666f 7220 7369 676d 615f 6465 6772  : for sigma_degr
+00003590: 6565 203e 2030 2c20 656e 7375 7265 2074  ee > 0, ensure t
+000035a0: 6861 7420 7369 676d 6120 6973 2061 6c77  hat sigma is alw
+000035b0: 6179 7320 706f 7369 7469 7665 210a 2020  ays positive!.  
+000035c0: 2020 2020 2020 6669 7865 645f 696e 7465        fixed_inte
+000035d0: 7263 6570 7420 3a20 6f70 7469 6f6e 616c  rcept : optional
+000035e0: 2c20 666c 6f61 740a 2020 2020 2020 2020  , float.        
+000035f0: 2020 2020 4966 2073 6574 2c20 7468 6520      If set, the 
+00003600: 792d 6178 6973 2069 6e74 6572 6365 7074  y-axis intercept
+00003610: 2077 696c 6c20 6265 2066 6978 6564 2074   will be fixed t
+00003620: 6f20 7468 6973 2076 616c 7565 2e0a 2020  o this value..  
+00003630: 2020 2020 2020 2020 2020 4f74 6865 7277            Otherw
+00003640: 6973 6520 7468 6520 696e 7465 7263 6570  ise the intercep
+00003650: 7420 6265 636f 6d65 7320 6120 6672 6565  t becomes a free
+00003660: 2070 6172 616d 6574 6572 2e0a 2020 2020   parameter..    
+00003670: 2020 2020 7468 6574 615f 6e61 6d65 7320      theta_names 
+00003680: 3a20 6f70 7469 6f6e 616c 2c20 7475 706c  : optional, tupl
+00003690: 6520 6f66 2073 7472 0a20 2020 2020 2020  e of str.       
+000036a0: 2020 2020 206d 6179 2062 6520 7573 6564       may be used
+000036b0: 2074 6f20 7365 7420 7468 6520 6e61 6d65   to set the name
+000036c0: 7320 6f66 2074 6865 206d 6f64 656c 2070  s of the model p
+000036d0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+000036e0: 2020 4e29 02da 014c da01 6b29 03da 0149    N)...L..k)...I
+000036f0: 725d 0000 0072 5e00 0000 6301 0000 0000  r]...r^...c.....
+00003700: 0000 0000 0000 0003 0000 0033 0000 00f3  ...........3....
+00003710: 2000 0000 4b00 0100 9700 7c00 5d09 7d01   ...K.....|.].}.
+00003720: 6400 7c01 9b00 9d02 5600 9701 0100 8c0a  d.|.....V.......
+00003730: 6401 5300 721e 0000 0072 1600 0000 7217  d.S.r....r....r.
+00003740: 0000 0073 0200 0000 2020 721a 0000 0072  ...s....  r....r
+00003750: 1b00 0000 7a31 4261 7365 4578 706f 6e65  ....z1BaseExpone
+00003760: 6e74 6961 6c4d 6f64 656c 4e2e 5f5f 696e  ntialModelN.__in
+00003770: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c67  it__.<locals>.<g
+00003780: 656e 6578 7072 3e2a 0100 0073 2800 0000  enexpr>*...s(...
+00003790: e800 e800 8000 d028 57d0 2857 b821 a81c  .......(W.(W.!..
+000037a0: b021 a81c a81c d028 57d0 2857 d028 57d0  .!.....(W.(W.(W.
+000037b0: 2857 d028 57d0 2857 721c 0000 0072 0900  (W.(W.(Wr....r..
+000037c0: 0000 7247 0000 0029 0872 0800 0000 7221  ..rG...).r....r!
+000037d0: 0000 0072 0e00 0000 725b 0000 0072 2200  ...r....r[...r".
+000037e0: 0000 7223 0000 0072 2400 0000 7225 0000  ..r#...r$...r%..
+000037f0: 0029 0872 2600 0000 7210 0000 0072 1100  .).r&...r....r..
+00003800: 0000 720e 0000 0072 5b00 0000 720f 0000  ..r....r[...r...
+00003810: 00da 0674 6e61 6d65 7372 2700 0000 7308  ...tnamesr'...s.
+00003820: 0000 0020 2020 2020 2020 8072 1a00 0000  ...       .r....
+00003830: 7225 0000 007a 1e42 6173 6545 7870 6f6e  r%...z.BaseExpon
+00003840: 656e 7469 616c 4d6f 6465 6c4e 2e5f 5f69  entialModelN.__i
+00003850: 6e69 745f 5f08 0100 0073 8c00 0000 f880  nit__....s......
+00003860: 00f5 3400 1d22 d41c 34b0 5cd1 1c42 d41c  ..4.."..4.\..B..
+00003870: 4288 04d4 0819 d81f 2e88 04d4 081c d80b  B...............
+00003880: 16d0 0b1e e00f 1ed0 0f2a d819 2390 0690  .........*..#...
+00003890: 06e0 1928 9006 d81a 20a5 35d0 2857 d028  ...(.... .5.(W.(
+000038a0: 57bd 75c0 5cd0 5455 d145 55d1 3f56 d43f  W.u.\.TU.EU.?V.?
+000038b0: 56d0 2857 d128 57d4 2857 d123 57d4 2357  V.(W.(W.(W.#W.#W
+000038c0: d11a 5788 4bdd 080d 8907 8c07 d708 18d2  ..W.K...........
+000038d0: 0818 981f a82d c05b d008 18d1 0851 d408  .....-.[.....Q..
+000038e0: 51d0 0851 d008 51d0 0851 721c 0000 0072  Q..Q..Q..Qr....r
+000038f0: 2800 0000 6302 0000 0000 0000 0001 0000  (...c...........
+00003900: 0004 0000 0003 0000 00f3 2a01 0000 9700  ..........*.....
+00003910: 7c02 8007 7c00 6a00 0000 0000 0000 0000  |...|.j.........
+00003920: 7d02 7c00 6a01 0000 0000 0000 0000 8022  }.|.j.........."
+00003930: 7c02 6402 1900 0000 0000 0000 0000 7c02  |.d...........|.
+00003940: 6403 1900 0000 0000 0000 0000 7c02 6404  d...........|.d.
+00003950: 1900 0000 0000 0000 0000 6603 7d03 7c02  ..........f.}.|.
+00003960: 6405 6401 8502 1900 0000 0000 0000 0000  d.d.............
+00003970: 7d04 6e20 7c00 6a01 0000 0000 0000 0000  }.n |.j.........
+00003980: 7c02 6402 1900 0000 0000 0000 0000 7c02  |.d...........|.
+00003990: 6403 1900 0000 0000 0000 0000 6603 7d03  d...........f.}.
+000039a0: 7c02 6404 6401 8502 1900 0000 0000 0000  |.d.d...........
+000039b0: 0000 7d04 7405 0000 0000 0000 0000 0000  ..}.t...........
+000039c0: 6a03 0000 0000 0000 0000 7c01 7c03 a602  j.........|.|...
+000039d0: 0000 ab02 0000 0000 0000 0000 7d05 7c00  ............}.|.
+000039e0: 6a04 0000 0000 0000 0000 6402 6b02 0000  j.........d.k...
+000039f0: 0000 7209 7c02 6406 1900 0000 0000 0000  ..r.|.d.........
+00003a00: 0000 7d06 6e15 7405 0000 0000 0000 0000  ..}.n.t.........
+00003a10: 0000 6a05 0000 0000 0000 0000 7c05 7c04  ..j.........|.|.
+00003a20: a602 0000 ab02 0000 0000 0000 0000 7d06  ..............}.
+00003a30: 7c05 7c06 6602 5300 2907 616f 0300 0050  |.|.f.S.).ao...P
+00003a40: 7265 6469 6374 7320 7468 6520 7061 7261  redicts the para
+00003a50: 6d65 7465 7273 206d 7520 616e 6420 7369  meters mu and si
+00003a60: 676d 6120 6f66 2061 206e 6f72 6d61 6c20  gma of a normal 
+00003a70: 6469 7374 7269 6275 7469 6f6e 2077 6869  distribution whi
+00003a80: 6368 0a20 2020 2020 2020 2063 6861 7261  ch.        chara
+00003a90: 6374 6572 697a 6573 2074 6865 2064 6570  cterizes the dep
+00003aa0: 656e 6465 6e74 2076 6172 6961 626c 6520  endent variable 
+00003ab0: 6769 7665 6e20 7661 6c75 6573 206f 6620  given values of 
+00003ac0: 7468 6520 696e 6465 7065 6e64 656e 7420  the independent 
+00003ad0: 7661 7269 6162 6c65 2e0a 0a20 2020 2020  variable...     
+00003ae0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00003af0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00003b00: 0a20 2020 2020 2020 2078 203a 2061 7272  .        x : arr
+00003b10: 6179 2d6c 696b 650a 2020 2020 2020 2020  ay-like.        
+00003b20: 2020 2020 7661 6c75 6573 206f 6620 7468      values of th
+00003b30: 6520 696e 6465 7065 6e64 656e 7420 7661  e independent va
+00003b40: 7269 6162 6c65 0a20 2020 2020 2020 2074  riable.        t
+00003b50: 6865 7461 203a 206f 7074 696f 6e61 6c2c  heta : optional,
+00003b60: 2061 7272 6179 2d6c 696b 650a 2020 2020   array-like.    
+00003b70: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00003b80: 7220 7665 6374 6f72 206f 6620 7468 6520  r vector of the 
+00003b90: 6361 6c69 6272 6174 696f 6e20 6d6f 6465  calibration mode
+00003ba0: 6c2e 0a20 2020 2020 2020 2020 2020 2044  l..            D
+00003bb0: 6570 656e 6469 6e67 206f 6e20 7468 6520  epending on the 
+00003bc0: 6060 6669 7865 645f 696e 7465 7263 6570  ``fixed_intercep
+00003bd0: 7460 6020 7365 7474 696e 6720 7468 6573  t`` setting thes
+00003be0: 6520 6172 650a 2020 2020 2020 2020 2020  e are.          
+00003bf0: 2020 5b49 2c20 4c2c 206b 5d20 6f72 205b    [I, L, k] or [
+00003c00: 4c2c 206b 5d20 7061 7261 6d65 7465 7273  L, k] parameters
+00003c10: 206f 6620 6578 706f 6e65 6e74 6961 6c20   of exponential 
+00003c20: 6d6f 6465 6c20 666f 7220 6d75 2e0a 2020  model for mu..  
+00003c30: 2020 2020 2020 2020 2020 466f 6c6c 6f77            Follow
+00003c40: 6564 2062 7920 7061 7261 6d65 7465 7273  ed by parameters
+00003c50: 2066 6f72 2074 6865 206d 6f64 656c 2066   for the model f
+00003c60: 6f72 2073 6967 6d61 2028 6c6f 7765 7374  or sigma (lowest
+00003c70: 2064 6567 7265 6520 6669 7273 7429 2e0a   degree first)..
+00003c80: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00003c90: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00003ca0: 0a20 2020 2020 2020 206d 7520 3a20 6172  .        mu : ar
+00003cb0: 7261 792d 6c69 6b65 0a20 2020 2020 2020  ray-like.       
+00003cc0: 2020 2020 2076 616c 7565 7320 666f 7220       values for 
+00003cd0: 7468 6520 6d75 2070 6172 616d 6574 6572  the mu parameter
+00003ce0: 206f 6620 6120 6e6f 726d 616c 2064 6973   of a normal dis
+00003cf0: 7472 6962 7574 696f 6e20 6465 7363 7269  tribution descri
+00003d00: 6269 6e67 2074 6865 2064 6570 656e 6465  bing the depende
+00003d10: 6e74 2076 6172 6961 626c 650a 2020 2020  nt variable.    
+00003d20: 2020 2020 7369 676d 6120 3a20 6172 7261      sigma : arra
+00003d30: 792d 6c69 6b65 206f 7220 666c 6f61 740a  y-like or float.
+00003d40: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00003d50: 6573 2066 6f72 2074 6865 2073 6967 6d61  es for the sigma
+00003d60: 2070 6172 616d 6574 6572 206f 6620 6120   parameter of a 
+00003d70: 6e6f 726d 616c 2064 6973 7472 6962 7574  normal distribut
+00003d80: 696f 6e20 6465 7363 7269 6269 6e67 2074  ion describing t
+00003d90: 6865 2064 6570 656e 6465 6e74 2076 6172  he dependent var
+00003da0: 6961 626c 650a 2020 2020 2020 2020 4e72  iable.        Nr
+00003db0: 0200 0000 7209 0000 0072 0600 0000 e903  ....r....r......
+00003dc0: 0000 0072 2b00 0000 2906 722c 0000 0072  ...r+...).r,...r
+00003dd0: 5b00 0000 7207 0000 00da 0b65 7870 6f6e  [...r......expon
+00003de0: 656e 7469 616c 720e 0000 0072 2d00 0000  entialr....r-...
+00003df0: 2907 7226 0000 0072 2f00 0000 7229 0000  ).r&...r/...r)..
+00003e00: 00da 0874 6865 7461 5f6d 75da 0b74 6865  ...theta_mu..the
+00003e10: 7461 5f73 6967 6d61 7230 0000 0072 3100  ta_sigmar0...r1.
+00003e20: 0000 7307 0000 0020 2020 2020 2020 721a  ..s....       r.
+00003e30: 0000 0072 3200 0000 7a27 4261 7365 4578  ...r2...z'BaseEx
+00003e40: 706f 6e65 6e74 6961 6c4d 6f64 656c 4e2e  ponentialModelN.
+00003e50: 7072 6564 6963 745f 6465 7065 6e64 656e  predict_dependen
+00003e60: 742d 0100 0073 ab00 0000 8000 f02a 000c  t-...s.......*..
+00003e70: 1188 3dd8 1418 d414 2588 45e0 0b0f d40b  ..=.....%.E.....
+00003e80: 1fd0 0b27 d818 1d98 619c 08a0 25a8 01a4  ...'....a...%...
+00003e90: 28a8 45b0 21ac 48d0 1735 8848 d81a 1fa0  (.E.!.H..5.H....
+00003ea0: 01a0 02a0 029c 2988 4b88 4be0 181c d418  ......).K.K.....
+00003eb0: 2ca8 65b0 41ac 68b8 05b8 61bc 08d0 1741  ,.e.A.h...a....A
+00003ec0: 8848 d81a 1fa0 01a0 02a0 029c 2988 4be5  .H..........).K.
+00003ed0: 0d11 d40d 1d98 61a0 18d1 0d2a d40d 2a88  ......a....*..*.
+00003ee0: 02d8 0b0f d40b 1ca0 01d2 0b21 d00b 21d8  ...........!..!.
+00003ef0: 1419 9822 9449 8845 8845 e514 1894 4fa0  ...".I.E.E....O.
+00003f00: 42a8 0bd1 1434 d414 3488 45d8 0f11 9035  B....4..4.E....5
+00003f10: 8879 d008 1872 1c00 0000 6302 0000 0000  .y...r....c.....
+00003f20: 0000 0001 0000 0004 0000 0003 0000 00f3  ................
+00003f30: a800 0000 9700 7c02 8007 7c00 6a00 0000  ......|...|.j...
+00003f40: 0000 0000 0000 7d02 7c00 6a01 0000 0000  ......}.|.j.....
+00003f50: 0000 0000 8018 7c02 6402 1900 0000 0000  ......|.d.......
+00003f60: 0000 0000 7c02 6403 1900 0000 0000 0000  ....|.d.........
+00003f70: 0000 7c02 6404 1900 0000 0000 0000 0000  ..|.d...........
+00003f80: 6603 7d03 6e16 7c00 6a01 0000 0000 0000  f.}.n.|.j.......
+00003f90: 0000 7c02 6402 1900 0000 0000 0000 0000  ..|.d...........
+00003fa0: 7c02 6403 1900 0000 0000 0000 0000 6603  |.d...........f.
+00003fb0: 7d03 7405 0000 0000 0000 0000 0000 6a03  }.t...........j.
+00003fc0: 0000 0000 0000 0000 7c01 7c03 a602 0000  ........|.|.....
+00003fd0: ab02 0000 0000 0000 0000 5300 2905 6150  ..........S.).aP
+00003fe0: 0200 0050 7265 6469 6374 2074 6865 2069  ...Predict the i
+00003ff0: 6e64 6570 656e 6465 6e74 2076 6172 6961  ndependent varia
+00004000: 626c 6520 7573 696e 6720 7468 6520 696e  ble using the in
+00004010: 7665 7273 6520 7472 656e 6420 6d6f 6465  verse trend mode
+00004020: 6c2e 0a0a 2020 2020 2020 2020 5061 7261  l...        Para
+00004030: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+00004040: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00004050: 2020 7920 3a20 6172 7261 792d 6c69 6b65    y : array-like
+00004060: 0a20 2020 2020 2020 2020 2020 206f 6273  .            obs
+00004070: 6572 7661 7469 6f6e 730a 2020 2020 2020  ervations.      
+00004080: 2020 7468 6574 6120 3a20 6f70 7469 6f6e    theta : option
+00004090: 616c 2c20 6172 7261 792d 6c69 6b65 0a20  al, array-like. 
+000040a0: 2020 2020 2020 2020 2020 2050 6172 616d             Param
+000040b0: 6574 6572 2076 6563 746f 7220 6f66 2074  eter vector of t
+000040c0: 6865 2063 616c 6962 7261 7469 6f6e 206d  he calibration m
+000040d0: 6f64 656c 2e0a 2020 2020 2020 2020 2020  odel..          
+000040e0: 2020 4465 7065 6e64 696e 6720 6f6e 2074    Depending on t
+000040f0: 6865 2060 6066 6978 6564 5f69 6e74 6572  he ``fixed_inter
+00004100: 6365 7074 6060 2073 6574 7469 6e67 2074  cept`` setting t
+00004110: 6865 7365 2061 7265 0a20 2020 2020 2020  hese are.       
+00004120: 2020 2020 205b 492c 204c 2c20 6b5d 206f       [I, L, k] o
+00004130: 7220 5b4c 2c20 6b5d 2070 6172 616d 6574  r [L, k] paramet
+00004140: 6572 7320 6f66 2065 7870 6f6e 656e 7469  ers of exponenti
+00004150: 616c 206d 6f64 656c 2066 6f72 206d 752e  al model for mu.
+00004160: 0a20 2020 2020 2020 2020 2020 2046 6f6c  .            Fol
+00004170: 6c6f 7765 6420 6279 2070 6172 616d 6574  lowed by paramet
+00004180: 6572 7320 666f 7220 7468 6520 6d6f 6465  ers for the mode
+00004190: 6c20 666f 7220 7369 676d 6120 286c 6f77  l for sigma (low
+000041a0: 6573 7420 6465 6772 6565 2066 6972 7374  est degree first
+000041b0: 292e 0a0a 2020 2020 2020 2020 5265 7475  )...        Retu
+000041c0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+000041d0: 2d2d 2d0a 2020 2020 2020 2020 7820 3a20  ---.        x : 
+000041e0: 6172 7261 792d 6c69 6b65 0a20 2020 2020  array-like.     
+000041f0: 2020 2020 2020 2070 7265 6469 6374 6564         predicted
+00004200: 2069 6e64 6570 656e 6465 6e74 2076 616c   independent val
+00004210: 7565 7320 6769 7665 6e20 7468 6520 6f62  ues given the ob
+00004220: 7365 7276 6174 696f 6e73 0a20 2020 2020  servations.     
+00004230: 2020 204e 7202 0000 0072 0900 0000 7206     Nr....r....r.
+00004240: 0000 0029 0472 2c00 0000 725b 0000 0072  ...).r,...r[...r
+00004250: 0700 0000 da13 696e 7665 7273 655f 6578  ......inverse_ex
+00004260: 706f 6e65 6e74 6961 6c29 0472 2600 0000  ponential).r&...
+00004270: 7235 0000 0072 2900 0000 7265 0000 0073  r5...r)...re...s
+00004280: 0400 0000 2020 2020 721a 0000 0072 3800  ....    r....r8.
+00004290: 0000 7a29 4261 7365 4578 706f 6e65 6e74  ..z)BaseExponent
+000042a0: 6961 6c4d 6f64 656c 4e2e 7072 6564 6963  ialModelN.predic
+000042b0: 745f 696e 6465 7065 6e64 656e 7453 0100  t_independentS..
+000042c0: 0073 5e00 0000 8000 f024 000c 1188 3dd8  .s^......$....=.
+000042d0: 1418 d414 2588 45e0 0b0f d40b 1fd0 0b27  ....%.E........'
+000042e0: d818 1d98 619c 08a0 25a8 01a4 28a8 45b0  ....a...%...(.E.
+000042f0: 21ac 48d0 1735 8848 8848 e018 1cd4 182c  !.H..5.H.H.....,
+00004300: a865 b041 ac68 b805 b861 bc08 d017 4188  .e.A.h...a....A.
+00004310: 48dd 0f13 d40f 27a8 01a8 38d1 0f34 d40f  H.....'...8..4..
+00004320: 34d0 0834 721c 0000 0029 0c72 3a00 0000  4..4r....).r:...
+00004330: 723b 0000 0072 3c00 0000 723d 0000 0072  r;...r<...r=...r
+00004340: 3e00 0000 7203 0000 00da 0566 6c6f 6174  >...r......float
+00004350: 7204 0000 0072 2500 0000 7232 0000 0072  r....r%...r2...r
+00004360: 3800 0000 723f 0000 0072 4000 0000 7301  8...r?...r@...s.
+00004370: 0000 0040 721a 0000 0072 5a00 0000 725a  ...@r....rZ...rZ
+00004380: 0000 0007 0100 0073 dc00 0000 f880 0080  .......s........
+00004390: 0080 0080 0080 00f0 0c00 1d1e d82b 2fd8  .............+/.
+000043a0: 2f33 f00f 2305 5201 f000 2305 5201 f000  /3..#.R...#.R...
+000043b0: 2305 5201 f006 001a 1df0 0723 0552 01f0  #.R........#.R..
+000043c0: 0800 181b f009 2305 5201 f00a 0017 1af0  ......#.R.......
+000043d0: 0b23 0552 01f0 0c00 1a22 a025 9c1f f00d  .#.R.....".%....
+000043e0: 2305 5201 f00e 0016 1e98 68a0 739c 6dd4  #.R.......h.s.m.
+000043f0: 152c f00f 2305 5201 f000 2305 5201 f000  .,..#.R...#.R...
+00004400: 2305 5201 f000 2305 5201 f000 2305 5201  #.R...#.R...#.R.
+00004410: f000 2305 5201 f04a 0100 2d31 f000 2405  ..#.R..J..-1..$.
+00004420: 19f0 0024 0519 f000 2405 19f0 0024 0519  ...$....$....$..
+00004430: f000 2405 19f0 4c01 002f 33f0 0019 0535  ..$...L../3....5
+00004440: f000 1905 35f0 0019 0535 f000 1905 35f0  ....5....5....5.
+00004450: 0019 0535 f000 1905 35f0 0019 0535 f000  ...5....5....5..
+00004460: 1905 35f0 0019 0535 721c 0000 0072 5a00  ..5....5r....rZ.
+00004470: 0000 4e29 0fda 075f 5f64 6f63 5f5f da06  ..N)...__doc__..
+00004480: 7479 7069 6e67 7203 0000 0072 0400 0000  typingr....r....
+00004490: 7205 0000 00da 0072 0700 0000 7208 0000  r......r....r...
+000044a0: 0072 0a00 0000 da19 436f 6e74 696e 756f  .r......Continuo
+000044b0: 7573 556e 6976 6172 6961 7465 4d6f 6465  usUnivariateMode
+000044c0: 6cda 0b4e 6f72 6d61 6c4e 6f69 7365 720c  l..NormalNoiser.
+000044d0: 0000 0072 4200 0000 7252 0000 0072 5a00  ...rB...rR...rZ.
+000044e0: 0000 7216 0000 0072 1c00 0000 721a 0000  ..r....r....r...
+000044f0: 00fa 083c 6d6f 6475 6c65 3e72 6f00 0000  ...<module>ro...
+00004500: 0100 0000 7358 0100 00f0 0301 0101 f002  ....sX..........
+00004510: 0301 04f0 0003 0104 f008 0001 2dd0 002c  ............-..,
+00004520: d000 2cd0 002c d000 2cd0 002c d000 2cd0  ..,..,..,..,..,.
+00004530: 002c d000 2cd0 002c e000 1ad0 001a d000  .,..,..,........
+00004540: 1ad0 001a d000 1ad0 001a d000 1ad0 001a  ................
+00004550: d800 13d0 0013 d000 13d0 0013 d000 13d0  ................
+00004560: 0013 f006 5901 011b f000 5901 011b f000  ....Y.....Y.....
+00004570: 5901 011b f000 5901 011b f000 5901 011b  Y.....Y.....Y...
+00004580: 9834 d41b 39b8 35d4 3b4c f100 5901 011b  .4..9.5.;L..Y...
+00004590: f400 5901 011b f000 5901 011b f078 024d  ..Y.....Y....x.M
+000045a0: 0101 3ef0 004d 0101 3ef0 004d 0101 3ef0  ..>..M..>..M..>.
+000045b0: 004d 0101 3ef0 004d 0101 3e98 64d4 1e3c  .M..>..M..>.d..<
+000045c0: b865 d43e 4ff1 004d 0101 3ef4 004d 0101  .e.>O..M..>..M..
+000045d0: 3ef0 004d 0101 3ef0 6002 4d01 0143 01f0  >..M..>.`.M..C..
+000045e0: 004d 0101 4301 f000 4d01 0143 01f0 004d  .M..C...M..C...M
+000045f0: 0101 4301 f000 4d01 0143 01a8 44d4 2c4a  ..C...M..C..D.,J
+00004600: c845 d44c 5df1 004d 0101 4301 f400 4d01  .E.L]..M..C...M.
+00004610: 0143 01f0 004d 0101 4301 f060 0265 0101  .C...M..C..`.e..
+00004620: 35f0 0065 0101 35f0 0065 0101 35f0 0065  5..e..5..e..5..e
+00004630: 0101 35f0 0065 0101 3598 44d4 1c3a b845  ..5..e..5.D..:.E
+00004640: d43c 4df1 0065 0101 35f4 0065 0101 35f0  .<M..e..5..e..5.
+00004650: 0065 0101 35f0 0065 0101 35f0 0065 0101  .e..5..e..5..e..
+00004660: 3572 1c00 0000                           5r....
```

### Comparing `calibr8-7.1.1/calibr8/contrib/noise.py` & `calibr8-7.1.2/calibr8/contrib/noise.py`

 * *Files identical despite different names*

### Comparing `calibr8-7.1.1/calibr8/contrib/normal.py` & `calibr8-7.1.2/calibr8/contrib/normal.py`

 * *Files identical despite different names*

### Comparing `calibr8-7.1.1/calibr8/contrib/studentt.py` & `calibr8-7.1.2/calibr8/contrib/studentt.py`

 * *Files identical despite different names*

### Comparing `calibr8-7.1.1/calibr8/core.py` & `calibr8-7.1.2/calibr8/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 or (asymmetric) logistic functions and their corresponding inverse functions.
 """
 import datetime
 import inspect
 import json
 import logging
 import os
-import typing
 import warnings
 from pathlib import Path
-from typing import Callable, Optional, Sequence, Tuple, Union
+from typing import Callable, DefaultDict, List, Optional, Sequence, Tuple, Union
 
 import numpy
 import scipy
 
 from . import utils
 from .utils import DistributionType, pm
 
-__version__ = "7.1.1"
+__version__ = "7.1.2"
 _log = logging.getLogger("calibr8")
 
 
 class InferenceResult:
     """Generic base type of independent value inference results."""
 
 
@@ -166,15 +165,15 @@
 def _interval_prob(x_cdf: numpy.ndarray, cdf: numpy.ndarray, a: float, b: float):
     """Calculates the probability in the interval [a, b]."""
     ia = numpy.argmin(numpy.abs(x_cdf - a))
     ib = numpy.argmin(numpy.abs(x_cdf - b))
     return cdf[ib] - cdf[ia]
 
 
-def _get_eti(x_cdf: numpy.ndarray, cdf: numpy.ndarray, ci_prob: float) -> typing.Tuple[float, float]:
+def _get_eti(x_cdf: numpy.ndarray, cdf: numpy.ndarray, ci_prob: float) -> Tuple[float, float]:
     """Find the equal tailed interval (ETI) corresponding to a certain credible interval probability level.
 
     Parameters
     ----------
     x_cdf : numpy.ndarray
         Coordinates where the cumulative density function was evaluated
     cdf : numpy.ndarray
@@ -199,16 +198,16 @@
 def _get_hdi(
     x_cdf: numpy.ndarray,
     cdf: numpy.ndarray,
     ci_prob: float,
     guess_lower: float,
     guess_upper: float,
     *,
-    history: typing.Optional[typing.DefaultDict[str, typing.List]] = None,
-) -> typing.Tuple[float, float]:
+    history: Optional[DefaultDict[str, List]] = None,
+) -> Tuple[float, float]:
     """Find the highest density interval (HDI) corresponding to a certain credible interval probability level.
 
     Parameters
     ----------
     x_cdf : numpy.ndarray
         Coordinates where the cumulative density function was evaluated
     cdf : numpy.ndarray
@@ -596,15 +595,15 @@
                 if not numpy.shape(result) == numpy.shape(x):
                     raise ValueError("The underlying model does not seem to implement broadcasting.")
                 return result
             except:
                 return numpy.exp([self.loglikelihood(y=y, x=xi, theta=theta) for xi in x])
         return numpy.exp(self.loglikelihood(y=y, x=x, theta=theta))
 
-    def objective(self, independent, dependent, minimize=True) -> typing.Callable:
+    def objective(self, independent, dependent, minimize=True) -> Callable:
         """Creates an objective function for fitting to data.
 
         Parameters
         ----------
         independent : array-like
             numeric or symbolic values of the independent variable
         dependent : array-like
@@ -624,15 +623,15 @@
             if minimize:
                 return -L
             else:
                 return L
 
         return objective
 
-    def save(self, filepath: Union[Path, os.PathLike]):
+    def save(self, filepath: Union[str, Path, os.PathLike]):
         """Save key properties of the calibration model to a JSON file.
 
         Parameters
         ----------
         filepath : path-like
             path to the output file
         """
@@ -650,15 +649,15 @@
             cal_dependent=self.cal_dependent.tolist() if self.cal_dependent is not None else None,
         )
         with open(filepath, "w") as jfile:
             json.dump(data, jfile, indent=4)
         return
 
     @classmethod
-    def load(cls, filepath: Union[Path, os.PathLike]):
+    def load(cls, filepath: Union[str, Path, os.PathLike]):
         """Instantiates a model from a JSON file of key properties.
 
         Parameters
         ----------
         filepath : path-like
             path to the input file
```

### Comparing `calibr8-7.1.1/calibr8/optimization.py` & `calibr8-7.1.2/calibr8/optimization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 The optimization module implements convenience functions for maximum
 likelihood estimation of calibration model parameters.
 """
 import logging
-import typing
-from typing import Any, Mapping, Optional, Sequence, Tuple, Union
+from typing import Any, Literal, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy
 import scipy.optimize
 
 from . import core
 
 _log = logging.getLogger("calibr8.optimization")
 
 
-def _mask_and_warn_inf_or_nan(x: numpy.ndarray, y: numpy.ndarray, on: typing.Optional[str] = None):
+def _mask_and_warn_inf_or_nan(
+    x: Union[Sequence[float], numpy.ndarray],
+    y: Union[Sequence[float], numpy.ndarray],
+    on: Optional[Literal["x", "y"]] = None,
+) -> Tuple[numpy.ndarray, numpy.ndarray]:
     """Filters `x` and `y` such that only finite elements remain.
 
     Parameters
     ----------
     x : ndarray
         1-dimensional array of values, same shape as y
     y : ndarray
@@ -27,14 +30,16 @@
         May be passed to filter on only x, or y instead of both (None, default).
 
     Returns
     -------
     x : array
     y : array
     """
+    x = numpy.asarray(x)
+    y = numpy.asarray(y)
     xdims = numpy.ndim(x)
     if xdims == 1:
         mask_x = numpy.isfinite(x)
     elif xdims == 2:
         mask_x = ~numpy.any(numpy.ma.masked_invalid(x).mask, axis=1)
     else:
         raise ValueError(f"The independent values are {numpy.ndim(x)}-dimensional. That's not supported.")
@@ -78,16 +83,16 @@
             bound_hit = True
     return bound_hit
 
 
 def fit_scipy(
     model: core.CalibrationModel,
     *,
-    independent: numpy.ndarray,
-    dependent: numpy.ndarray,
+    independent: Union[Sequence[float], numpy.ndarray],
+    dependent: Union[Sequence[float], numpy.ndarray],
     theta_guess: Union[Sequence[float], numpy.ndarray],
     theta_bounds: Sequence[Tuple[float, float]],
     minimize_kwargs: Optional[Mapping[str, Any]] = None,
 ):
     """Function to fit the calibration model with observed data.
 
     Parameters
@@ -150,16 +155,16 @@
     model.cal_dependent = numpy.array(dependent)
     return fit.x, history
 
 
 def fit_scipy_global(
     model: core.CalibrationModel,
     *,
-    independent: numpy.ndarray,
-    dependent: numpy.ndarray,
+    independent: Union[Sequence[float], numpy.ndarray],
+    dependent: Union[Sequence[float], numpy.ndarray],
     theta_bounds: list,
     method: Optional[str] = None,
     maxiter: int = 5000,
     minimizer_kwargs: Optional[Mapping[str, Any]] = None,
 ):
     """Function to fit the calibration model with observed data using global optimization.
```

### Comparing `calibr8-7.1.1/calibr8/test_all.py` & `calibr8-7.1.2/calibr8/test_all.py`

 * *Files identical despite different names*

### Comparing `calibr8-7.1.1/calibr8/utils.py` & `calibr8-7.1.2/calibr8/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 This module implements helper functions for a variety of tasks, including
 imports, timestamp parsing and plotting.
 """
 import datetime
-import typing
 import warnings
 from collections.abc import Iterable
-from typing import Literal, Optional, Sequence, Tuple
+from typing import List, Literal, Optional, Sequence, Tuple
 
 import matplotlib
 import numpy
 import scipy.stats
 from matplotlib import pyplot
 from typing_extensions import TypeAlias
 
@@ -48,28 +47,28 @@
     HAS_PYMC = True
 except ModuleNotFoundError:
     DistributionType: TypeAlias = Literal[None]  # type: ignore
     HAS_PYMC = False
     pm = ImportWarner("pymc")
 
 
-def parse_datetime(s: typing.Optional[str]) -> typing.Optional[datetime.datetime]:
+def parse_datetime(s: Optional[str]) -> Optional[datetime.datetime]:
     """Parses a timezone-aware datetime formatted like 2020-08-05T13:37:00Z.
 
     Returns
     -------
     result : optional, datetime
         may be None when the input was None
     """
     if s is None:
         return None
     return datetime.datetime.strptime(s.replace("Z", "+0000"), "%Y-%m-%dT%H:%M:%S%z")
 
 
-def format_datetime(dt: typing.Optional[datetime.datetime]) -> typing.Optional[str]:
+def format_datetime(dt: Optional[datetime.datetime]) -> Optional[str]:
     """Formats a datetime like 2020-08-05T13:37:00Z.
 
     Returns
     -------
     result : optional, str
         may be None when the input was None
     """
@@ -172,15 +171,17 @@
                 color="green",
             )
         )
         artists.append(ax.fill_between([], [], [], color=c, label=f"{percent:.1f} % likelihood band"))
     return artists
 
 
-def plot_t_band(ax, independent, mu, scale, df, *, residual_type: typing.Optional[str] = None):
+def plot_t_band(
+    ax, independent, mu, scale, df, *, residual_type: Optional[Literal["absolute", "relative"]] = None
+):
     """Helper function for plotting the 68, 90 and 95 % likelihood-bands of a t-distribution.
 
     Parameters
     ----------
     ax : matplotlib.Axes
         subplot object to plot into
     independent : array-like
@@ -237,15 +238,17 @@
                 color="green",
             )
         )
         artists.append(ax.fill_between([], [], [], color=c, label=f"{percent:.1f} % likelihood band"))
     return artists
 
 
-def plot_continuous_band(ax, independent, model, residual_type: typing.Optional[str] = None):
+def plot_continuous_band(
+    ax, independent, model, residual_type: Optional[Literal["absolute", "relative"]] = None
+):
     """Helper function for plotting the 68, 90 and 95 % likelihood-bands of a univariate distribution.
 
     Parameters
     ----------
     ax : matplotlib.Axes
         subplot object to plot into
     independent : array-like
@@ -360,17 +363,17 @@
 
 
 def plot_model(
     model,
     *,
     fig: Optional[matplotlib.figure.Figure] = None,
     axs: Optional[Sequence[matplotlib.axes.Axes]] = None,
-    residual_type="absolute",
+    residual_type: Literal["absolute", "relative"] = "absolute",
     band_xlim: Tuple[Optional[float], Optional[float]] = (None, None),
-):
+) -> Tuple[matplotlib.figure.Figure, List[matplotlib.axes.Axes]]:
     """Makes a plot of the model with its data.
 
     Parameters
     -----------
     model : CalibrationModel
         A fitted calibration model with data.
         The predict_dependent method should return a tuple where the mean is the first entry.
@@ -412,14 +415,16 @@
         gs1 = fig.add_gridspec(1, 3, wspace=0.05, width_ratios=[1.125, 1.125, 1.5])
         gs2 = fig.add_gridspec(1, 3, wspace=0.5, width_ratios=[1.125, 1.125, 1.5])
         axs = []
         axs.append(fig.add_subplot(gs1[0, 0]))
         axs.append(fig.add_subplot(gs1[0, 1], sharey=axs[0]))
         pyplot.setp(axs[1].get_yticklabels(), visible=False)
         axs.append(fig.add_subplot(gs2[0, 2]))
+    else:
+        axs = list(axs)
 
     # ======= Left =======
     # Untransformed, outer range
     ax = axs[0]
     if hasattr(model.scipy_dist, "ppf"):
         plot_continuous_band(
             ax,
```

### Comparing `calibr8-7.1.1/calibr8.egg-info/PKG-INFO` & `calibr8-7.1.2/calibr8.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibr8
-Version: 7.1.1
+Version: 7.1.2
 Summary: Toolbox for non-linear calibration modeling.
 Home-page: https://github.com/JuBiotech/calibr8
 Author: Laura Marie Helleckes, Michael Osthege
 Author-email: l.helleckes@fz-juelich.de, m.osthege@fz-juelich.de
 License: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
@@ -14,18 +14,14 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: scipy>1.6.0
-Requires-Dist: typing_extensions
 
 [![PyPI version](https://img.shields.io/pypi/v/calibr8)](https://pypi.org/project/calibr8)
 [![pipeline](https://github.com/jubiotech/calibr8/workflows/pipeline/badge.svg)](https://github.com/jubiotech/calibr8/actions)
 [![coverage](https://codecov.io/gh/jubiotech/calibr8/branch/master/graph/badge.svg)](https://codecov.io/gh/jubiotech/calibr8)
 [![documentation](https://readthedocs.org/projects/calibr8/badge/?version=latest)](https://calibr8.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/306862348.svg)](https://zenodo.org/badge/latestdoi/306862348)
```

### Comparing `calibr8-7.1.1/calibr8.egg-info/SOURCES.txt` & `calibr8-7.1.2/calibr8.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 calibr8/test_all.py
 calibr8/utils.py
 calibr8.egg-info/PKG-INFO
 calibr8.egg-info/SOURCES.txt
 calibr8.egg-info/dependency_links.txt
 calibr8.egg-info/requires.txt
 calibr8.egg-info/top_level.txt
-calibr8/__pycache__/__init__.cpython-39.pyc
-calibr8/__pycache__/core.cpython-39.pyc
-calibr8/__pycache__/optimization.cpython-39.pyc
-calibr8/__pycache__/test_all.cpython-39-pytest-8.0.0.pyc
-calibr8/__pycache__/utils.cpython-39.pyc
+calibr8/__pycache__/__init__.cpython-311.pyc
+calibr8/__pycache__/core.cpython-311.pyc
+calibr8/__pycache__/optimization.cpython-311.pyc
+calibr8/__pycache__/test_all.cpython-311-pytest-8.2.0.pyc
+calibr8/__pycache__/utils.cpython-311.pyc
 calibr8/contrib/__init__.py
 calibr8/contrib/noise.py
 calibr8/contrib/normal.py
 calibr8/contrib/studentt.py
-calibr8/contrib/__pycache__/__init__.cpython-39.pyc
-calibr8/contrib/__pycache__/noise.cpython-39.pyc
-calibr8/contrib/__pycache__/normal.cpython-39.pyc
-calibr8/contrib/__pycache__/studentt.cpython-39.pyc
+calibr8/contrib/__pycache__/__init__.cpython-311.pyc
+calibr8/contrib/__pycache__/noise.cpython-311.pyc
+calibr8/contrib/__pycache__/normal.cpython-311.pyc
+calibr8/contrib/__pycache__/studentt.cpython-311.pyc
```

### Comparing `calibr8-7.1.1/setup.py` & `calibr8-7.1.2/setup.py`

 * *Files identical despite different names*

