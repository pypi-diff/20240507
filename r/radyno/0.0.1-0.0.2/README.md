# Comparing `tmp/radyno-0.0.1.tar.gz` & `tmp/radyno-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radyno-0.0.1.tar", last modified: Sun Mar 24 21:48:57 2024, max compression
+gzip compressed data, was "radyno-0.0.2.tar", last modified: Tue May  7 14:47:33 2024, max compression
```

## Comparing `radyno-0.0.1.tar` & `radyno-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 21:48:57.167652 radyno-0.0.1/
--rw-rw-rw-   0        0        0      616 2024-03-24 21:48:57.166412 radyno-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       92 2024-03-24 21:47:43.000000 radyno-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-24 21:48:57.154095 radyno-0.0.1/radyno/
--rw-rw-rw-   0        0        0      259 2024-03-24 21:30:26.000000 radyno-0.0.1/radyno/__init__.py
--rw-rw-rw-   0        0        0    12240 2024-03-22 15:40:46.000000 radyno-0.0.1/radyno/beam_utils.py
--rw-rw-rw-   0        0        0      970 2024-03-14 17:00:39.000000 radyno-0.0.1/radyno/drift_beam_test.py
--rw-rw-rw-   0        0        0     2724 2024-03-22 17:47:55.000000 radyno-0.0.1/radyno/ion_channel_test.py
--rw-rw-rw-   0        0        0    28781 2024-03-22 17:53:53.000000 radyno-0.0.1/radyno/rad_utils.py
--rw-rw-rw-   0        0        0     2965 2024-03-22 17:54:20.000000 radyno-0.0.1/radyno/undulator_test.py
-drwxrwxrwx   0        0        0        0 2024-03-24 21:48:57.164413 radyno-0.0.1/radyno.egg-info/
--rw-rw-rw-   0        0        0      616 2024-03-24 21:48:57.000000 radyno-0.0.1/radyno.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-03-24 21:48:57.000000 radyno-0.0.1/radyno.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 21:48:57.000000 radyno-0.0.1/radyno.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-03-24 21:48:57.000000 radyno-0.0.1/radyno.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-24 21:48:57.000000 radyno-0.0.1/radyno.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-24 21:48:57.167652 radyno-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1095 2024-03-24 21:39:53.000000 radyno-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:47:33.315068 radyno-0.0.2/
+-rw-rw-rw-   0        0        0      537 2024-05-07 14:47:33.315068 radyno-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2024-03-24 21:47:43.000000 radyno-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 14:47:33.313994 radyno-0.0.2/radyno.egg-info/
+-rw-rw-rw-   0        0        0      537 2024-05-07 14:47:33.000000 radyno-0.0.2/radyno.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2024-05-07 14:47:33.000000 radyno-0.0.2/radyno.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:47:33.000000 radyno-0.0.2/radyno.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:47:33.000000 radyno-0.0.2/radyno.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 14:47:33.315068 radyno-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1097 2024-05-07 14:46:34.000000 radyno-0.0.2/setup.py
```

### Comparing `radyno-0.0.1/setup.py` & `radyno-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
-DESCRIPTION = 'Particle tracking and radiation spectrum evaluation'
+VERSION = '0.0.2'
+DESCRIPTION = 'Particles tracking and radiation spectrum evaluation'
 
 # Setting up
 setup(
     name="radyno",
     version=VERSION,
     author="exborgg (Andrea Frazzitta)",
     author_email="<andrea.frazzitta@uniroma1.it>",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=['opencv-python', 'pyautogui', 'pyaudio'],
+    #install_requires=['opencv-python', 'pyautogui', 'pyaudio'],
     keywords=['python', 'beam', 'radiation', 'spectrum', 'mpi', 'parallel'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

