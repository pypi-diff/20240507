# Comparing `tmp/Yoteelijo-1.0.0.tar.gz` & `tmp/Yoteelijo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Yoteelijo-1.0.0.tar", last modified: Tue May  7 20:45:22 2024, max compression
+gzip compressed data, was "Yoteelijo-1.0.2.tar", last modified: Tue May  7 03:18:05 2024, max compression
```

## Comparing `Yoteelijo-1.0.0.tar` & `Yoteelijo-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 20:45:22.570767 Yoteelijo-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-07 20:45:22.522926 Yoteelijo-1.0.0/Impactrueno/
--rw-rw-rw-   0        0        0       45 2024-05-07 03:01:24.000000 Yoteelijo-1.0.0/Impactrueno/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 Yoteelijo-1.0.0/Impactrueno/pokemon.csv
--rw-rw-rw-   0        0        0      737 2024-05-07 02:59:39.000000 Yoteelijo-1.0.0/Impactrueno/random_Pokemon.py
--rw-rw-rw-   0        0        0      345 2024-05-07 20:45:22.567835 Yoteelijo-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 20:45:22.561977 Yoteelijo-1.0.0/Yoteelijo.egg-info/
--rw-rw-rw-   0        0        0      345 2024-05-07 20:45:22.000000 Yoteelijo-1.0.0/Yoteelijo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-07 20:45:22.000000 Yoteelijo-1.0.0/Yoteelijo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 20:45:22.000000 Yoteelijo-1.0.0/Yoteelijo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-07 20:45:22.000000 Yoteelijo-1.0.0/Yoteelijo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-07 20:45:22.000000 Yoteelijo-1.0.0/Yoteelijo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 20:45:22.571742 Yoteelijo-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      475 2024-05-07 20:44:38.000000 Yoteelijo-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:18:04.981244 Yoteelijo-1.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-07 03:18:04.657112 Yoteelijo-1.0.2/Impactrueno/
+-rw-rw-rw-   0        0        0       45 2024-05-07 03:01:24.000000 Yoteelijo-1.0.2/Impactrueno/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 Yoteelijo-1.0.2/Impactrueno/pokemon.csv
+-rw-rw-rw-   0        0        0      737 2024-05-07 02:59:39.000000 Yoteelijo-1.0.2/Impactrueno/random_Pokemon.py
+-rw-rw-rw-   0        0        0      345 2024-05-07 03:18:04.975385 Yoteelijo-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 03:18:04.924617 Yoteelijo-1.0.2/Yoteelijo.egg-info/
+-rw-rw-rw-   0        0        0      345 2024-05-07 03:18:03.000000 Yoteelijo-1.0.2/Yoteelijo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-07 03:18:03.000000 Yoteelijo-1.0.2/Yoteelijo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 03:18:03.000000 Yoteelijo-1.0.2/Yoteelijo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-07 03:18:03.000000 Yoteelijo-1.0.2/Yoteelijo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-07 03:18:03.000000 Yoteelijo-1.0.2/Yoteelijo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 03:18:05.017366 Yoteelijo-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      475 2024-05-07 03:17:14.000000 Yoteelijo-1.0.2/setup.py
```

### Comparing `Yoteelijo-1.0.0/Impactrueno/pokemon.csv` & `Yoteelijo-1.0.2/Impactrueno/pokemon.csv`

 * *Files identical despite different names*

### Comparing `Yoteelijo-1.0.0/Impactrueno/random_Pokemon.py` & `Yoteelijo-1.0.2/Impactrueno/random_Pokemon.py`

 * *Files identical despite different names*

