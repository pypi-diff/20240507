# Comparing `tmp/algotom-1.5.0.tar.gz` & `tmp/algotom-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algotom-1.5.0.tar", last modified: Mon Mar 25 01:48:13 2024, max compression
+gzip compressed data, was "algotom-1.6.0.tar", last modified: Tue May  7 03:16:30 2024, max compression
```

## Comparing `algotom-1.5.0.tar` & `algotom-1.6.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 01:48:13.190731 algotom-1.5.0/
--rw-rw-rw-   0        0        0    11572 2022-09-02 17:52:52.000000 algotom-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     8962 2024-03-25 01:48:13.175059 algotom-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     8017 2024-03-03 21:10:11.000000 algotom-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-25 01:48:12.590103 algotom-1.5.0/algotom/
--rw-rw-rw-   0        0        0        0 2022-09-02 17:52:52.000000 algotom-1.5.0/algotom/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 01:48:12.689850 algotom-1.5.0/algotom/io/
--rw-rw-rw-   0        0        0        0 2022-09-02 17:52:52.000000 algotom-1.5.0/algotom/io/__init__.py
--rw-rw-rw-   0        0        0     5638 2023-02-03 15:55:27.000000 algotom-1.5.0/algotom/io/converter.py
--rw-rw-rw-   0        0        0    45336 2024-03-15 15:31:29.000000 algotom-1.5.0/algotom/io/loadersaver.py
-drwxrwxrwx   0        0        0        0 2024-03-25 01:48:12.730954 algotom-1.5.0/algotom/post/
--rw-rw-rw-   0        0        0        0 2022-09-02 17:52:52.000000 algotom-1.5.0/algotom/post/__init__.py
--rw-rw-rw-   0        0        0    43231 2024-03-12 21:38:24.000000 algotom-1.5.0/algotom/post/postprocessing.py
-drwxrwxrwx   0        0        0        0 2024-03-25 01:48:12.949690 algotom-1.5.0/algotom/prep/
--rw-rw-rw-   0        0        0        0 2022-09-02 17:52:52.000000 algotom-1.5.0/algotom/prep/__init__.py
--rw-rw-rw-   0        0        0    33467 2024-03-12 21:39:33.000000 algotom-1.5.0/algotom/prep/calculation.py
--rw-rw-rw-   0        0        0    27260 2022-12-30 21:56:00.000000 algotom-1.5.0/algotom/prep/conversion.py
--rw-rw-rw-   0        0        0    22263 2023-03-25 22:38:12.000000 algotom-1.5.0/algotom/prep/correction.py
--rw-rw-rw-   0        0        0     7639 2023-04-17 20:33:20.000000 algotom-1.5.0/algotom/prep/filtering.py
--rw-rw-rw-   0        0        0    39234 2023-10-15 00:34:32.000000 algotom-1.5.0/algotom/prep/phase.py
--rw-rw-rw-   0        0        0    36446 2024-02-28 16:18:10.000000 algotom-1.5.0/algotom/prep/removal.py
-drwxrwxrwx   0        0        0        0 2024-03-25 01:48:12.996610 algotom-1.5.0/algotom/rec/
--rw-rw-rw-   0        0        0        0 2022-09-02 17:52:52.000000 algotom-1.5.0/algotom/rec/__init__.py
--rw-rw-rw-   0        0        0    49647 2024-03-24 21:20:22.000000 algotom-1.5.0/algotom/rec/reconstruction.py
-drwxrwxrwx   0        0        0        0 2024-03-25 01:48:13.152516 algotom-1.5.0/algotom/util/
--rw-rw-rw-   0        0        0        0 2022-09-02 17:52:52.000000 algotom-1.5.0/algotom/util/__init__.py
--rw-rw-rw-   0        0        0    15821 2024-03-25 01:30:40.000000 algotom-1.5.0/algotom/util/calibration.py
--rw-rw-rw-   0        0        0   138794 2023-03-30 19:41:51.000000 algotom-1.5.0/algotom/util/correlation.py
--rw-rw-rw-   0        0        0    18999 2023-03-25 22:38:12.000000 algotom-1.5.0/algotom/util/simulation.py
--rw-rw-rw-   0        0        0    52961 2024-02-28 16:18:10.000000 algotom-1.5.0/algotom/util/utility.py
-drwxrwxrwx   0        0        0        0 2024-03-25 01:48:13.168055 algotom-1.5.0/algotom.egg-info/
--rw-rw-rw-   0        0        0     8962 2024-03-25 01:48:12.000000 algotom-1.5.0/algotom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      694 2024-03-25 01:48:12.000000 algotom-1.5.0/algotom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 01:48:12.000000 algotom-1.5.0/algotom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-03-25 01:48:12.000000 algotom-1.5.0/algotom.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-25 01:48:12.000000 algotom-1.5.0/algotom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-25 01:48:13.190731 algotom-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1649 2024-03-25 01:45:08.000000 algotom-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:16:30.213862 algotom-1.6.0/
+-rw-rw-rw-   0        0        0    11572 2022-09-02 17:52:52.000000 algotom-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0     9586 2024-05-07 03:16:30.202909 algotom-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8641 2024-05-07 03:14:53.000000 algotom-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 03:16:29.795380 algotom-1.6.0/algotom/
+-rw-rw-rw-   0        0        0        0 2022-09-02 17:52:52.000000 algotom-1.6.0/algotom/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:16:29.874629 algotom-1.6.0/algotom/io/
+-rw-rw-rw-   0        0        0        0 2022-09-02 17:52:52.000000 algotom-1.6.0/algotom/io/__init__.py
+-rw-rw-rw-   0        0        0     8275 2024-05-05 02:55:12.000000 algotom-1.6.0/algotom/io/converter.py
+-rw-rw-rw-   0        0        0    45363 2024-05-07 01:12:09.000000 algotom-1.6.0/algotom/io/loadersaver.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:16:29.895537 algotom-1.6.0/algotom/post/
+-rw-rw-rw-   0        0        0        0 2022-09-02 17:52:52.000000 algotom-1.6.0/algotom/post/__init__.py
+-rw-rw-rw-   0        0        0    43229 2024-05-07 01:12:09.000000 algotom-1.6.0/algotom/post/postprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:16:30.011802 algotom-1.6.0/algotom/prep/
+-rw-rw-rw-   0        0        0        0 2022-09-02 17:52:52.000000 algotom-1.6.0/algotom/prep/__init__.py
+-rw-rw-rw-   0        0        0    35620 2024-05-07 01:12:09.000000 algotom-1.6.0/algotom/prep/calculation.py
+-rw-rw-rw-   0        0        0    27260 2022-12-30 21:56:00.000000 algotom-1.6.0/algotom/prep/conversion.py
+-rw-rw-rw-   0        0        0    22263 2023-03-25 22:38:12.000000 algotom-1.6.0/algotom/prep/correction.py
+-rw-rw-rw-   0        0        0     7639 2023-04-17 20:33:20.000000 algotom-1.6.0/algotom/prep/filtering.py
+-rw-rw-rw-   0        0        0    39234 2023-10-15 00:34:32.000000 algotom-1.6.0/algotom/prep/phase.py
+-rw-rw-rw-   0        0        0    36446 2024-02-28 16:18:10.000000 algotom-1.6.0/algotom/prep/removal.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:16:30.057600 algotom-1.6.0/algotom/rec/
+-rw-rw-rw-   0        0        0        0 2022-09-02 17:52:52.000000 algotom-1.6.0/algotom/rec/__init__.py
+-rw-rw-rw-   0        0        0    62736 2024-05-07 02:45:07.000000 algotom-1.6.0/algotom/rec/reconstruction.py
+-rw-rw-rw-   0        0        0    68999 2024-05-07 02:45:07.000000 algotom-1.6.0/algotom/rec/vertrec.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:16:30.161091 algotom-1.6.0/algotom/util/
+-rw-rw-rw-   0        0        0        0 2022-09-02 17:52:52.000000 algotom-1.6.0/algotom/util/__init__.py
+-rw-rw-rw-   0        0        0    15821 2024-03-25 01:30:40.000000 algotom-1.6.0/algotom/util/calibration.py
+-rw-rw-rw-   0        0        0   138855 2024-04-26 21:16:45.000000 algotom-1.6.0/algotom/util/correlation.py
+-rw-rw-rw-   0        0        0    18999 2023-03-25 22:38:12.000000 algotom-1.6.0/algotom/util/simulation.py
+-rw-rw-rw-   0        0        0    51038 2024-04-26 21:16:45.000000 algotom-1.6.0/algotom/util/utility.py
+drwxrwxrwx   0        0        0        0 2024-05-07 03:16:30.184987 algotom-1.6.0/algotom.egg-info/
+-rw-rw-rw-   0        0        0     9586 2024-05-07 03:16:29.000000 algotom-1.6.0/algotom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-05-07 03:16:29.000000 algotom-1.6.0/algotom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 03:16:29.000000 algotom-1.6.0/algotom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-07 03:16:29.000000 algotom-1.6.0/algotom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 03:16:29.000000 algotom-1.6.0/algotom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 03:16:30.213862 algotom-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2024-05-07 01:12:10.000000 algotom-1.6.0/setup.py
```

### Comparing `algotom-1.5.0/LICENSE` & `algotom-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `algotom-1.5.0/PKG-INFO` & `algotom-1.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algotom
-Version: 1.5.0
+Version: 1.6.0
 Summary: Data processing algorithms for tomography
 Home-page: https://github.com/algotom/algotom
 Author: Nghia Vo
 Author-email: nvo@bnl.gov
 License: Apache 2.0
 Keywords: Parallel-beam Computed Tomography,Image Processing,Tomography,X-ray Imaging,Phase Contrast Imaging,Ring artifact removal
 Platform: Any
@@ -29,24 +29,27 @@
 ### Data processing (**ALGO**)rithms for (**TOM**)ography.
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/algotom/algotom/algotom_ga.yml) [![Downloads](https://static.pepy.tech/personalized-badge/algotom?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi-downloads)](https://pepy.tech/project/algotom) ![Conda](https://img.shields.io/conda/dn/algotom/algotom?label=conda-downloads) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/algotom/algotom) ![Conda](https://img.shields.io/conda/pn/algotom/algotom) ![GitHub issues](https://img.shields.io/github/issues-raw/algotom/algotom) ![Conda](https://img.shields.io/conda/dn/conda-forge/algotom?label=conda-forge%20downloads) ![Coverage](https://github.com/algotom/algotom/raw/doc/docs/coverage_report/coverage.svg)
 
 
 ![logo](https://github.com/algotom/algotom/raw/master/figs/readme/logo2.png)
 
-**Algotom** is a Python package that implements data processing methods for tomography. 
-It offers a comprehensive pipeline for data processing; including reading and writing data, 
-pre-processing, tomographic reconstruction, post-processing, and data simulation. 
-The package provides numerous utility methods to assist users in rapidly developing 
-prototype methods or constructing a pipeline for processing their own data.
-The main standout features of Algotom are its wealth of pre-processing methods: 
-artifact removal, distortion correction, phase retrieval, processing automation,... 
-The software excels in readability, minimal dependencies, maintainability, 
-and rich documentation. Starting from version 1.1, methods for speckle-based 
-phase-contrast tomography have been incorporated into the package.
+**Algotom** is a Python package designed for tomography data processing. It 
+offers a complete data processing pipeline; including reading and writing data, 
+pre-processing, tomographic reconstruction, post-processing, data simulation, 
+and calibration techniques. The package provides many utility methods to 
+assist users in constructing a pipeline for processing their own data or 
+developing new methods. Key features of Algotom include a wide range of 
+processing methods such as artifact removal, distortion correction, 
+speckle-based phase-contrast imaging, data reduction; and the capability of 
+processing non-standard tomography acquisitions such as grid scans or helical scans. 
+The software stands out for its readability, minimal dependencies, and rich documentation. 
+Developed specifically for synchrotron-based tomographic beamlines, Algotom aims to 
+maximize data quality, enhance workflow throughput, and exploit full beamline 
+capabilities.
 
 Features
 --------
 
 Algotom is a lightweight package. The software is built on top of a few core
 Python libraries to ensure its ease-of-installation. Methods distributed in 
 Algotom have been developed and tested at synchrotron beamlines where massive
@@ -68,26 +71,26 @@
 - Methods for processing helical scans (with/without the offset rotation-axis).
   
   ![helical_scan](https://github.com/algotom/algotom/raw/master/figs/readme/helical_scan.jpg)
 
 - Methods for determining the center-of-rotation (COR) and auto-stitching images 
   in half-acquisition scans (360-degree acquisition with the offset COR).
 
-- Some practical methods developed and implemented for the package:
-  zinger removal, tilted sinogram generation, sinogram distortion correction, 
-  beam hardening correction, DFI (direct Fourier inversion) reconstruction, FBP reconstruction,
-  and double-wedge filter for removing sample parts larger than the FOV in
-  a sinogram.
+- Practical methods developed and implemented for the package: zinger removal, 
+  tilted sinogram generation, sinogram distortion correction, simplified form of Paganin's filter,
+  beam hardening correction, DFI (direct Fourier inversion) reconstruction,
+  FBP (filtered back-projection) reconstruction, BPF (back-projection filtering) reconstruction, 
+  and double-wedge filter for removing sample parts larger than the FOV in a sinogram.
   
   ![pipe_line](https://github.com/algotom/algotom/raw/master/figs/readme/double_wedge_filter.jpg)
   
 - Utility methods for [customizing ring/stripe artifact removal methods](https://algotom.readthedocs.io/en/latest/toc/section4/section4_3.html) 
   and parallelizing computational work.
 
-- Calibration methods for determining pixel-size in helical scans.
+- Calibration methods for helical scans and tomography alignment.
 
 - Methods for generating simulation data: phantom creation, sinogram calculation
   based on the Fourier slice theorem, and artifact generation.
   
   ![simulation](https://github.com/algotom/algotom/raw/master/figs/readme/simulation.png)
 
 - Methods for phase-contrast imaging: phase unwrapping, speckle-based phase retrieval, image correlation, and image alignment.
@@ -95,14 +98,23 @@
   ![speckle](https://github.com/algotom/algotom/raw/master/figs/readme/speckle_based_tomography.png)
 
 - Methods for downsampling, rescaling, and reslicing (+rotating, cropping) 
   3D reconstructed image without large memory usage.
 
   ![reslicing](https://github.com/algotom/algotom/raw/master/figs/readme/reslicing.jpg)
 
+- Direct vertical reconstruction for single slice, multiple slices, and multiple slices at 
+  different orientations.
+  
+  ![vertical_slice1](https://github.com/algotom/algotom/raw/master/figs/readme/direct_vertical_reconstruction.png)
+
+  ![vertical_slice1](https://github.com/algotom/algotom/raw/master/figs/readme/limited_angle_tomography.png)
+  
+   
+
 Installation
 ------------
 
 - https://algotom.readthedocs.io/en/latest/toc/section3.html
 - If users install Algotom to an existing environment and Numba fails to install due to the latest Numpy:
   + Downgrade Numpy and install Algotom/Numba again.
   + Create a new environment and install Algotom first, then other packages.
@@ -115,17 +127,18 @@
 - https://algotom.readthedocs.io/en/latest/toc/section1/section1_4.html
 - https://algotom.readthedocs.io/en/latest/toc/section4.html
 - https://github.com/algotom/algotom/tree/master/examples
 
 Development principles
 ----------------------
 
-- While Algotom offers a comprehensive range of tools for tomographic data processing covering raw-data reading, 
-  pre-processing, reconstruction, post-processing, and data saving; its development primarily focuses on 
-  pre-processing techniques. This distinction makes it a prominent feature among other tomographic software.   
+- While Algotom offers a complete set of tools for tomographic data processing covering 
+  pre-processing, reconstruction, post-processing, data simulation, and calibration techniques;
+  its development strongly focuses on pre-processing techniques. This distinction makes it a
+  prominent feature among other tomographic software.   
 
 - To ensure that the software can work across platforms and is easy-to-install; dependencies are minimized, and only 
   well-maintained [Python libraries](https://github.com/algotom/algotom/blob/master/requirements.txt) are used.
 
 - To achieve high-performance computing and leverage GPU utilization while ensuring ease of understanding, usage, and software 
   maintenance, Numba is used instead of Cupy or PyCuda.
```

### Comparing `algotom-1.5.0/README.md` & `algotom-1.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 ### Data processing (**ALGO**)rithms for (**TOM**)ography.
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/algotom/algotom/algotom_ga.yml) [![Downloads](https://static.pepy.tech/personalized-badge/algotom?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi-downloads)](https://pepy.tech/project/algotom) ![Conda](https://img.shields.io/conda/dn/algotom/algotom?label=conda-downloads) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/algotom/algotom) ![Conda](https://img.shields.io/conda/pn/algotom/algotom) ![GitHub issues](https://img.shields.io/github/issues-raw/algotom/algotom) ![Conda](https://img.shields.io/conda/dn/conda-forge/algotom?label=conda-forge%20downloads) ![Coverage](https://github.com/algotom/algotom/raw/doc/docs/coverage_report/coverage.svg)
 
 
 ![logo](https://github.com/algotom/algotom/raw/master/figs/readme/logo2.png)
 
-**Algotom** is a Python package that implements data processing methods for tomography. 
-It offers a comprehensive pipeline for data processing; including reading and writing data, 
-pre-processing, tomographic reconstruction, post-processing, and data simulation. 
-The package provides numerous utility methods to assist users in rapidly developing 
-prototype methods or constructing a pipeline for processing their own data.
-The main standout features of Algotom are its wealth of pre-processing methods: 
-artifact removal, distortion correction, phase retrieval, processing automation,... 
-The software excels in readability, minimal dependencies, maintainability, 
-and rich documentation. Starting from version 1.1, methods for speckle-based 
-phase-contrast tomography have been incorporated into the package.
+**Algotom** is a Python package designed for tomography data processing. It 
+offers a complete data processing pipeline; including reading and writing data, 
+pre-processing, tomographic reconstruction, post-processing, data simulation, 
+and calibration techniques. The package provides many utility methods to 
+assist users in constructing a pipeline for processing their own data or 
+developing new methods. Key features of Algotom include a wide range of 
+processing methods such as artifact removal, distortion correction, 
+speckle-based phase-contrast imaging, data reduction; and the capability of 
+processing non-standard tomography acquisitions such as grid scans or helical scans. 
+The software stands out for its readability, minimal dependencies, and rich documentation. 
+Developed specifically for synchrotron-based tomographic beamlines, Algotom aims to 
+maximize data quality, enhance workflow throughput, and exploit full beamline 
+capabilities.
 
 Features
 --------
 
 Algotom is a lightweight package. The software is built on top of a few core
 Python libraries to ensure its ease-of-installation. Methods distributed in 
 Algotom have been developed and tested at synchrotron beamlines where massive
@@ -41,26 +44,26 @@
 - Methods for processing helical scans (with/without the offset rotation-axis).
   
   ![helical_scan](https://github.com/algotom/algotom/raw/master/figs/readme/helical_scan.jpg)
 
 - Methods for determining the center-of-rotation (COR) and auto-stitching images 
   in half-acquisition scans (360-degree acquisition with the offset COR).
 
-- Some practical methods developed and implemented for the package:
-  zinger removal, tilted sinogram generation, sinogram distortion correction, 
-  beam hardening correction, DFI (direct Fourier inversion) reconstruction, FBP reconstruction,
-  and double-wedge filter for removing sample parts larger than the FOV in
-  a sinogram.
+- Practical methods developed and implemented for the package: zinger removal, 
+  tilted sinogram generation, sinogram distortion correction, simplified form of Paganin's filter,
+  beam hardening correction, DFI (direct Fourier inversion) reconstruction,
+  FBP (filtered back-projection) reconstruction, BPF (back-projection filtering) reconstruction, 
+  and double-wedge filter for removing sample parts larger than the FOV in a sinogram.
   
   ![pipe_line](https://github.com/algotom/algotom/raw/master/figs/readme/double_wedge_filter.jpg)
   
 - Utility methods for [customizing ring/stripe artifact removal methods](https://algotom.readthedocs.io/en/latest/toc/section4/section4_3.html) 
   and parallelizing computational work.
 
-- Calibration methods for determining pixel-size in helical scans.
+- Calibration methods for helical scans and tomography alignment.
 
 - Methods for generating simulation data: phantom creation, sinogram calculation
   based on the Fourier slice theorem, and artifact generation.
   
   ![simulation](https://github.com/algotom/algotom/raw/master/figs/readme/simulation.png)
 
 - Methods for phase-contrast imaging: phase unwrapping, speckle-based phase retrieval, image correlation, and image alignment.
@@ -68,14 +71,23 @@
   ![speckle](https://github.com/algotom/algotom/raw/master/figs/readme/speckle_based_tomography.png)
 
 - Methods for downsampling, rescaling, and reslicing (+rotating, cropping) 
   3D reconstructed image without large memory usage.
 
   ![reslicing](https://github.com/algotom/algotom/raw/master/figs/readme/reslicing.jpg)
 
+- Direct vertical reconstruction for single slice, multiple slices, and multiple slices at 
+  different orientations.
+  
+  ![vertical_slice1](https://github.com/algotom/algotom/raw/master/figs/readme/direct_vertical_reconstruction.png)
+
+  ![vertical_slice1](https://github.com/algotom/algotom/raw/master/figs/readme/limited_angle_tomography.png)
+  
+   
+
 Installation
 ------------
 
 - https://algotom.readthedocs.io/en/latest/toc/section3.html
 - If users install Algotom to an existing environment and Numba fails to install due to the latest Numpy:
   + Downgrade Numpy and install Algotom/Numba again.
   + Create a new environment and install Algotom first, then other packages.
@@ -88,17 +100,18 @@
 - https://algotom.readthedocs.io/en/latest/toc/section1/section1_4.html
 - https://algotom.readthedocs.io/en/latest/toc/section4.html
 - https://github.com/algotom/algotom/tree/master/examples
 
 Development principles
 ----------------------
 
-- While Algotom offers a comprehensive range of tools for tomographic data processing covering raw-data reading, 
-  pre-processing, reconstruction, post-processing, and data saving; its development primarily focuses on 
-  pre-processing techniques. This distinction makes it a prominent feature among other tomographic software.   
+- While Algotom offers a complete set of tools for tomographic data processing covering 
+  pre-processing, reconstruction, post-processing, data simulation, and calibration techniques;
+  its development strongly focuses on pre-processing techniques. This distinction makes it a
+  prominent feature among other tomographic software.   
 
 - To ensure that the software can work across platforms and is easy-to-install; dependencies are minimized, and only 
   well-maintained [Python libraries](https://github.com/algotom/algotom/blob/master/requirements.txt) are used.
 
 - To achieve high-performance computing and leverage GPU utilization while ensuring ease of understanding, usage, and software 
   maintenance, Numba is used instead of Cupy or PyCuda.
```

### Comparing `algotom-1.5.0/algotom/io/loadersaver.py` & `algotom-1.6.0/algotom/io/loadersaver.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         be used by speckle-based phase contrast tomography.
 """
 
 import os
 import glob
 import warnings
 import multiprocessing as mp
-from joblib import Parallel, delayed, parallel_backend
+from joblib import Parallel, delayed
 from collections import OrderedDict, deque
 import h5py
 import numpy as np
 from PIL import Image
 
 
 PIPE = "│"
@@ -1209,14 +1209,16 @@
 
     Parameters
     ----------
     list_path : str
         List of output paths or a folder path
     image_stack : array_like
         3D array.
+    axis : int
+        Axis to slice data.
     overwrite : bool
         Overwrite an existing file if True.
     ncore : int or None
         Number of cpu-cores. Automatically selected if None.
     prefer : {"threads", "processes"}
         Prefer backend for parallel processing.
     start_idx : int
```

### Comparing `algotom-1.5.0/algotom/post/postprocessing.py` & `algotom-1.6.0/algotom/post/postprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,16 +112,15 @@
         (depth, height, width) = input_.shape
     elif in_type == "tif":
         list_file = losa.find_file(input_ + "/*.tif*")
         depth = len(list_file)
         (height, width) = np.shape(losa.load_image(list_file[0]))
     elif in_type == "hdf":
         if key_path is None:
-            raise ValueError(
-                "Please provide the key path to the dataset!!!")
+            raise ValueError("Please provide the key path to the dataset!!!")
         else:
             hdf_object = h5py.File(input_, 'r')
             check = key_path in hdf_object
             if not check:
                 raise ValueError("!!! Wrong key !!!")
             data = hdf_object[key_path]
             (depth, height, width) = data.shape
@@ -657,15 +656,15 @@
                         mat_tmp.append(np.transpose(mat[h1:h2, w1:w2]))
                     data_tmp[depth1 - last_chunk: depth1] = np.asarray(mat_tmp)
             else:
                 hdf_chunk = (chunk, min(100, height1), min(100, width1))
                 data_tmp = ofile.create_dataset(out_key,
                                                 (depth1, height1, width1),
                                                 dtype=data_type,
-                                                chunks = hdf_chunk)
+                                                chunks=hdf_chunk)
                 for i in np.arange(0, depth1 - last_chunk, chunk):
                     if show_progress:
                         t1 = timeit.default_timer()
                         f_size = os.path.getsize(file_tmp) / b_unit
                         msg = "Writing to an intermediate hdf-file: {0:0.2f}" \
                               "MB. Time: {1:0.2f}s".format(f_size, t1 - t0)
                         len_msg = len(msg)
@@ -778,16 +777,16 @@
               "{1:0.2f}s. The file will be deleted at the end!"
               "".format(f_size, t1 - t0))
     return file_tmp, out_key, folder_tmp
 
 
 def reslice_dataset(input_, output, axis=1, key_path=None, rescaling=False,
                     nbit=16, minmax=None, skip=None, rotate=0.0, chunk=16,
-                    mode="constant", crop=(0, 0, 0, 0, 0, 0),
-                    ncore=None, show_progress=True, overwrite=False):
+                    mode="constant", crop=(0, 0, 0, 0, 0, 0), ncore=None,
+                    show_progress=True, overwrite=False):
     """
     Reslice a 3d dataset. Input can be a folder of tif files or a hdf file.
 
     Parameters
     ----------
     input_ : str, array_like
         It can be a folder path to tif files or a hdf file.
@@ -896,28 +895,28 @@
                 if rescaling:
                     mat_tmp = []
                     for j in np.arange(chunk):
                         mat = rescale(mat_chunk[:, j, :], nbit, minmax)
                         mat_tmp.append(mat)
                     mat_tmp = np.asarray(mat_tmp)
                 else:
-                    mat_tmp = np.moveaxis(mat_chunk, 1, 0)
+                    mat_tmp = np.copy(np.moveaxis(mat_chunk, 1, 0))
                 data_slice[i:i + chunk] = mat_tmp
                 if show_progress:
                     sys.stdout.write("\r" + " " * len_msg + "\r")
             if last_chunk != 0:
                 mat_chunk = data[:, height1 - last_chunk: height1, :]
                 if rescaling:
                     mat_tmp = []
                     for j in np.arange(last_chunk):
                         mat = rescale(mat_chunk[:, j, :], nbit, minmax)
                         mat_tmp.append(mat)
                     mat_tmp = np.asarray(mat_tmp)
                 else:
-                    mat_tmp = np.moveaxis(mat_chunk, 1, 0)
+                    mat_tmp = np.copy(np.moveaxis(mat_chunk, 1, 0))
                 data_slice[height1 - last_chunk: height1] = mat_tmp
         else:
             list_file, len_msg = None, None
             for i in np.arange(0, height1 - last_chunk, chunk):
                 if show_progress:
                     t1 = timeit.default_timer()
                     list_file = glob.glob(output + "/*tif*")
```

### Comparing `algotom-1.5.0/algotom/prep/calculation.py` & `algotom-1.6.0/algotom/prep/calculation.py`

 * *Files 7% similar despite different names*

```diff
@@ -195,19 +195,19 @@
         list_metric = Parallel(n_jobs=ncore, prefer="threads")(
             delayed(calculate_center_metric)(list_cor[i], sino_180, sino_flip,
                                              sino_comp, mask) for i in
             range(num_metric))
     min_pos = np.argmin(list_metric)
     if min_pos == 0:
         msg = "Global minimum is out of the searching range. Please " \
-              "reduce the start-value !!!"
+              "reduce the starting value !!!"
         warnings.warn(msg)
     if min_pos == (num_metric - 1):
         msg = "Global minimum is out of the searching range. Please " \
-              "increase the stop-value !!!"
+              "increase the stopping value !!!"
         warnings.warn(msg)
     return list_cor[min_pos]
 
 
 def fine_search_cor(sino_180, start, radius, step, ratio=0.5, denoise=True,
                     ncore=None, hor_drop=None, ver_drop=None):
     """
@@ -418,16 +418,42 @@
         Correlation metric.
     """
     metric = np.abs(
         1.0 - stats.pearsonr(mat1.flatten('F'), mat2.flatten('F'))[0])
     return metric
 
 
+def __calc_overlap_metric(mat1, pos, offset, use_overlap, side, norm, wei_down,
+                          wei_up, win_width, mat2_roi, mat2_roi_wei,
+                          list_mean2):
+    mat1_roi = mat1[:, pos - offset:pos + offset]
+    if use_overlap is True:
+        if side == 1:
+            mat1_roi_wei = mat1_roi * wei_down
+        else:
+            mat1_roi_wei = mat1_roi * wei_up
+    if norm is True:
+        list_mean1 = np.mean(np.abs(mat1_roi), axis=1)
+        list_fact = list_mean2 / list_mean1
+        mat_fact = np.transpose(np.tile(list_fact, (win_width, 1)))
+        mat1_roi = mat1_roi * mat_fact
+        if use_overlap is True:
+            mat1_roi_wei = mat1_roi_wei * mat_fact
+    if use_overlap is True:
+        mat_comb = mat1_roi_wei + mat2_roi_wei
+        metric_val = (correlation_metric(mat1_roi, mat2_roi) +
+                      correlation_metric(mat1_roi, mat_comb) +
+                      correlation_metric(mat2_roi, mat_comb)) / 3.0
+    else:
+        metric_val = correlation_metric(mat1_roi, mat2_roi)
+    return metric_val
+
+
 def search_overlap(mat1, mat2, win_width, side, denoise=True, norm=False,
-                   use_overlap=False):
+                   use_overlap=False, ncore=None):
     """
     Calculate the correlation metrics between a rectangular region, defined
     by the window width, on the utmost left/right side of image 2 and the
     same size region in image 1 where the region is slided across image 1.
 
     Parameters
     ----------
@@ -444,23 +470,27 @@
     denoise : bool, optional
         Apply the Gaussian filter if True.
     norm : bool, optional
         Apply the normalization if True.
     use_overlap : bool, optional
         Use the combination of images in the overlap area for calculating
         correlation coefficients if True.
+    ncore: int or None
+        Number of cpu-cores used for computing. Automatically selected if None.
 
     Returns
     -------
     list_metric : array_like
         1D array. List of the correlation metrics.
     offset : int
         Initial position of the searching window where the position
         corresponds to the center of the window.
     """
+    if ncore is None:
+        ncore = np.clip(mp.cpu_count() - 1, 1, None)
     if denoise is True:
         mat1 = ndi.gaussian_filter(mat1, (2, 2), mode='reflect')
         mat2 = ndi.gaussian_filter(mat2, (2, 2), mode='reflect')
     (nrow1, ncol1) = mat1.shape
     (nrow2, ncol2) = mat2.shape
     if nrow1 != nrow2:
         raise ValueError("Two images are not at the same height!!!")
@@ -475,45 +505,40 @@
         mat2_roi = mat2[:, 0:win_width]
         mat2_roi_wei = mat2_roi * wei_up
     else:
         mat2_roi = mat2[:, ncol2 - win_width:]
         mat2_roi_wei = mat2_roi * wei_down
     list_mean2 = np.mean(np.abs(mat2_roi), axis=1)
     list_pos = np.arange(offset, ncol1 - offset)
-    num_metric = len(list_pos)
-    list_metric = np.ones(num_metric, dtype=np.float32)
-    for i, pos in enumerate(list_pos):
-        mat1_roi = mat1[:, pos - offset:pos + offset]
-        if use_overlap is True:
-            if side == 1:
-                mat1_roi_wei = mat1_roi * wei_down
-            else:
-                mat1_roi_wei = mat1_roi * wei_up
-        if norm is True:
-            list_mean1 = np.mean(np.abs(mat1_roi), axis=1)
-            list_fact = list_mean2 / list_mean1
-            mat_fact = np.transpose(np.tile(list_fact, (win_width, 1)))
-            mat1_roi = mat1_roi * mat_fact
-            if use_overlap is True:
-                mat1_roi_wei = mat1_roi_wei * mat_fact
-        if use_overlap is True:
-            mat_comb = mat1_roi_wei + mat2_roi_wei
-            list_metric[i] = (correlation_metric(mat1_roi, mat2_roi)
-                              + correlation_metric(mat1_roi, mat_comb)
-                              + correlation_metric(mat2_roi, mat_comb)) / 3.0
-        else:
-            list_metric[i] = correlation_metric(mat1_roi, mat2_roi)
+    nump = len(list_pos)
+    if ncore == 1:
+        list_metric = np.ones(nump, dtype=np.float32)
+        for i, pos in enumerate(list_pos):
+            list_metric[i] = __calc_overlap_metric(mat1, pos, offset,
+                                                   use_overlap, side, norm,
+                                                   wei_down, wei_up,
+                                                   win_width, mat2_roi,
+                                                   mat2_roi_wei,
+                                                   list_mean2)
+    else:
+        list_metric = Parallel(n_jobs=ncore, prefer="threads")(
+            delayed(__calc_overlap_metric)(mat1, list_pos[i], offset,
+                                           use_overlap, side, norm,
+                                           wei_down, wei_up, win_width,
+                                           mat2_roi, mat2_roi_wei,
+                                           list_mean2) for i in range(nump))
+        list_metric = np.asarray(list_metric)
     min_metric = np.min(list_metric)
     if min_metric != 0.0:
         list_metric = list_metric / min_metric
     return list_metric, offset
 
 
 def find_overlap(mat1, mat2, win_width, side=None, denoise=True, norm=False,
-                 use_overlap=False):
+                 use_overlap=False, ncore=None):
     """
     Find the overlap area and overlap side between two images (Ref. [1]) where
     the overlap side referring to the first image.
 
     Parameters
     ----------
     mat1 : array_like
@@ -529,14 +554,16 @@
     denoise : bool, optional
         Apply the Gaussian filter if True.
     norm : bool, optional
         Apply the normalization if True.
     use_overlap : bool, optional
         Use the combination of images in the overlap area for calculating
         correlation coefficients if True.
+    ncore: int or None
+        Number of cpu-cores used for computing. Automatically selected if None.
 
     Returns
     -------
     overlap : float
         Width of the overlap area between two images.
     side : int
         Overlap side between two images.
@@ -549,29 +576,33 @@
     [1] : https://doi.org/10.1364/OE.418448
     """
     (_, ncol1) = mat1.shape
     (_, ncol2) = mat2.shape
     win_width = int(np.clip(win_width, 6, min(ncol1, ncol2) // 2))
     if side == 1:
         (list_metric, offset) = search_overlap(mat1, mat2, win_width, side,
-                                               denoise, norm, use_overlap)
+                                               denoise, norm, use_overlap,
+                                               ncore)
         (_, overlap_position) = calculate_curvature(list_metric)
         overlap_position = overlap_position + offset
         overlap = ncol1 - overlap_position + win_width // 2
     elif side == 0:
         (list_metric, offset) = search_overlap(mat1, mat2, win_width, side,
-                                               denoise, norm, use_overlap)
+                                               denoise, norm, use_overlap,
+                                               ncore)
         (_, overlap_position) = calculate_curvature(list_metric)
         overlap_position = overlap_position + offset
         overlap = overlap_position + win_width // 2
     else:
         (list_metric1, offset1) = search_overlap(mat1, mat2, win_width, 1,
-                                                 norm, denoise, use_overlap)
+                                                 norm, denoise, use_overlap,
+                                                 ncore)
         (list_metric2, offset2) = search_overlap(mat1, mat2, win_width, 0,
-                                                 norm, denoise, use_overlap)
+                                                 norm, denoise, use_overlap,
+                                                 ncore)
         (curvature1, overlap_position1) = calculate_curvature(list_metric1)
         overlap_position1 = overlap_position1 + offset1
         (curvature2, overlap_position2) = calculate_curvature(list_metric2)
         overlap_position2 = overlap_position2 + offset2
         if curvature1 > curvature2:
             side = 1
             overlap_position = overlap_position1
@@ -580,15 +611,15 @@
             side = 0
             overlap_position = overlap_position2
             overlap = overlap_position + win_width // 2
     return overlap, side, overlap_position
 
 
 def find_overlap_multiple(list_mat, win_width, side=None, denoise=True,
-                          norm=False, use_overlap=False):
+                          norm=False, use_overlap=False, ncore=None):
     """
     Find the overlap-areas and overlap-sides of a list of images where the
     overlap side referring to the previous image.
 
     Parameters
     ----------
     list_mat : list of array_like
@@ -602,14 +633,16 @@
     denoise : bool, optional
         Apply the Gaussian filter if True.
     norm : bool, optional
         Apply the normalization if True.
     use_overlap : bool, optional
         Use the combination of images in the overlap area for calculating
         correlation coefficients if True.
+    ncore: int or None
+        Number of cpu-cores used for computing. Automatically selected if None.
 
     Returns
     -------
     list_overlap : list of tuple of floats
         List of [overlap, side, overlap_position].
         overlap : Width of the overlap area between two images.
         side : Overlap side between two images.
@@ -617,23 +650,23 @@
         image giving the best correlation metric.
     """
     list_overlap = []
     num_mat = len(list_mat)
     if num_mat > 1:
         for i in range(num_mat-1):
             results = find_overlap(list_mat[i], list_mat[i + 1], win_width,
-                                   side, denoise, norm, use_overlap)
+                                   side, denoise, norm, use_overlap, ncore)
             list_overlap.append(results)
     else:
         raise ValueError("Need at least 2 images to work!!!")
     return list_overlap
 
 
 def find_center_360(sino_360, win_width, side=None, denoise=True, norm=False,
-                    use_overlap=False):
+                    use_overlap=False, ncore=None):
     """
     Find the center-of-rotation (COR) in a 360-degree scan with offset COR use
     the method presented in Ref. [1].
 
     Parameters
     ----------
     sino_360 : array_like
@@ -647,14 +680,16 @@
     denoise : bool, optional
         Apply the Gaussian filter if True.
     norm : bool, optional
         Apply the normalization if True.
     use_overlap : bool, optional
         Use the combination of images in the overlap area for calculating
         correlation coefficients if True.
+    ncore: int or None
+        Number of cpu-cores used for computing. Automatically selected if None.
 
     Returns
     -------
     cor : float
         Center-of-rotation.
     overlap : float
         Width of the overlap area between two halves of the sinogram.
@@ -668,16 +703,17 @@
     ----------
     [1] : https://doi.org/10.1364/OE.418448
     """
     (nrow, ncol) = sino_360.shape
     nrow_180 = nrow // 2 + 1
     sino_top = sino_360[0:nrow_180, :]
     sino_bot = np.fliplr(sino_360[-nrow_180:, :])
-    (overlap, side, overlap_position) = find_overlap(
-        sino_top, sino_bot, win_width, side, denoise, norm, use_overlap)
+    (overlap, side, overlap_position) = find_overlap(sino_top, sino_bot,
+                                                     win_width, side, denoise,
+                                                     norm, use_overlap, ncore)
     if side == 0:
         cor = overlap / 2.0 - 1.0
     else:
         cor = ncol - overlap / 2.0 - 1.0
     return cor, overlap, side, overlap_position
 
 
@@ -781,77 +817,80 @@
     if flip is True:
         mat2 = np.fliplr(mat2)
     tx = find_shift_based_phase_correlation(mat1, mat2, gradient=gradient)[-1]
     cor = (ncol - 1.0 + tx) * 0.5
     return cor
 
 
-def find_center_projection(mat1, mat2, flip=True, chunk_height=None,
-                           start_row=None, denoise=True, norm=False,
-                           use_overlap=False):
+def find_center_projection(mat1, mat2, flip=True, win_width=None,
+                           chunk_height=None, start_row=None, denoise=True,
+                           norm=False, use_overlap=False, ncore=None):
     """
     Find the center-of-rotation (COR) using projection images at 0-degree
     and 180-degree based on a method in Ref. [1].
 
     Parameters
     ----------
     mat1 : array_like
         2D array. Projection image at 0-degree.
     mat2 : array_like
         2D array. Projection image at 180-degree.
     flip : bool, optional
         Flip the 180-degree projection in the left-right direction if True.
+    win_width : int, optional
+        Width of the searching window.
     chunk_height : int or float, optional
         Height of the sub-area of projection images. If a float is given, it
         must be in the range of [0.0, 1.0].
     start_row : int, optional
         Starting row used to extract the sub-area.
     denoise : bool, optional
         Apply the Gaussian filter if True.
     norm : bool, optional
         Apply the normalization if True.
     use_overlap : bool, optional
         Use the combination of images in the overlap area for calculating
         correlation coefficients if True.
+    ncore: int or None
+        Number of cpu-cores used for computing. Automatically selected if None.
 
     Returns
     -------
     cor : float
         Center-of-rotation.
 
     References
     ----------
     [1] : https://doi.org/10.1364/OE.418448
     """
     (nrow, ncol) = mat1.shape
     if flip is True:
         mat2 = np.fliplr(mat2)
-    win_width = ncol // 2
+    if win_width is None:
+        win_width = min(250, int(0.2 * ncol))
     if chunk_height is None:
-        chunk_height = int(0.1 * nrow)
+        chunk_height = min(500, int(0.9 * nrow))
     if isinstance(chunk_height, float):
         if 0.0 < chunk_height <= 1.0:
             chunk_height = int(chunk_height * nrow)
         else:
-            chunk_height = int(0.1 * nrow)
+            chunk_height = min(500, int(0.5 * nrow))
     chunk_height = np.clip(chunk_height, 1, nrow - 1)
     if start_row is None:
         start = nrow // 2 - chunk_height // 2
-    elif start_row < 0:
-        start = nrow + start_row - chunk_height // 2
     else:
-        start = start_row - chunk_height // 2
+        start = np.clip(start_row, 0, nrow // 2 - chunk_height // 2)
     stop = start + chunk_height
     start = np.clip(start, 0, nrow - chunk_height - 1)
-    stop = np.clip(stop, chunk_height, nrow - 1)
+    stop = np.clip(stop, chunk_height, nrow)
     mat1_roi = mat1[start: stop]
     mat2_roi = mat2[start: stop]
     (overlap, side, _) = find_overlap(mat1_roi, mat2_roi, win_width, side=None,
                                       denoise=denoise, norm=norm,
-                                      use_overlap=use_overlap)
+                                      use_overlap=use_overlap, ncore=ncore)
     if side == 0:
         cor = overlap / 2.0 - 1.0
     else:
         cor = ncol - overlap / 2.0 - 1.0
     return cor
```

### Comparing `algotom-1.5.0/algotom/prep/conversion.py` & `algotom-1.6.0/algotom/prep/conversion.py`

 * *Files identical despite different names*

### Comparing `algotom-1.5.0/algotom/prep/correction.py` & `algotom-1.6.0/algotom/prep/correction.py`

 * *Files identical despite different names*

### Comparing `algotom-1.5.0/algotom/prep/filtering.py` & `algotom-1.6.0/algotom/prep/filtering.py`

 * *Files identical despite different names*

### Comparing `algotom-1.5.0/algotom/prep/phase.py` & `algotom-1.6.0/algotom/prep/phase.py`

 * *Files identical despite different names*

### Comparing `algotom-1.5.0/algotom/prep/removal.py` & `algotom-1.6.0/algotom/prep/removal.py`

 * *Files identical despite different names*

### Comparing `algotom-1.5.0/algotom/util/calibration.py` & `algotom-1.6.0/algotom/util/calibration.py`

 * *Files identical despite different names*

### Comparing `algotom-1.5.0/algotom/util/correlation.py` & `algotom-1.6.0/algotom/util/correlation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1164,15 +1164,15 @@
             delayed(f_alias)(
                 ref_mat[i - start:i + start1, j - start:j + start1],
                 mat[i - radi:i + radi1, j - radi:j + radi1],
                 margin, None, sub_pixel, method, 2, size, False, block)
             for i in range(start, stop_row) for j in range(start, stop_col)))
         shifts = np.reshape(np.asarray(shifts),
                             (stop_row - start, stop_col - start, 2))
-    (x_shifts, y_shifts) = np.moveaxis(shifts, 2, 0)
+    (x_shifts, y_shifts) = np.copy(np.moveaxis(shifts, 2, 0))
     x_shifts = np.pad(x_shifts, radi + margin, mode="constant")
     y_shifts = np.pad(y_shifts, radi + margin, mode="constant")
     return x_shifts, y_shifts
 
 
 def _get_2d_shift_multi_rows_3d_input(ref_mat, mat, win_size=7, margin=10,
                                       sub_pixel=True, method="diff", size=3,
@@ -1268,15 +1268,15 @@
                 ref_mat[:, i - start:i + start1, j - start:j + start1],
                 mat[:, i - radi:i + radi1, j - radi:j + radi1],
                 margin, None, sub_pixel, method, 2, size, False, None)
                                    for i in range(start, stop_row)
                                    for j in range(start, stop_col)))
         shifts = np.reshape(np.asarray(shifts),
                             (stop_row - start, stop_col - start, 2))
-    (x_shifts, y_shifts) = np.moveaxis(shifts, 2, 0)
+    (x_shifts, y_shifts) = np.copy(np.moveaxis(shifts, 2, 0))
     if pad:
         x_shifts = np.pad(x_shifts, radi + margin, mode="constant")
         y_shifts = np.pad(y_shifts, radi + margin, mode="constant")
     return x_shifts, y_shifts
 
 
 def _get_2d_shift_full_image_3d_input_cpu(ref_mat, mat, chunk_size=None,
@@ -1391,16 +1391,15 @@
     for j in range(width2):
         ref_mat1 = ref_mat[:, j: j + width1]
         ref_mean = __mean_2d(ref_mat1)
         ref_sqr = __sum_square_2d(ref_mat1, ref_mean)
         sum_mul = __sum_multiply_2d(ref_mat1, mat, ref_mean, mat_mean)
         num = math.sqrt(ref_sqr * mat_sqr)
         if num != 0.0:
-            num_tmp = sum_mul / num
-        list_coef[j] = num_tmp
+            list_coef[j] = sum_mul / num
     return list_coef
 
 
 @cuda.jit(device=True)
 def __locate_1d_peak_kernel(list_data):  # pragma: no cover
     """
     GPU-kernel function to locate the position of the maximum value of a
@@ -1529,16 +1528,16 @@
     if len(ref_mat.shape) != 3:
         raise ValueError("Inputs must be 3d arrays !!!")
     if direction != "x" and direction != "y":
         raise ValueError("Only two options: 'x' or 'y''")
     if direction != "x":
         ref_mat = np.transpose(ref_mat, axes=(0, 2, 1))
         mat = np.transpose(mat, axes=(0, 2, 1))
-    ref_mat = np.moveaxis(ref_mat, 1, 0)
-    mat = np.moveaxis(mat, 1, 0)
+    ref_mat = np.copy(np.moveaxis(ref_mat, 1, 0))
+    mat = np.copy(np.moveaxis(mat, 1, 0))
     (height, depth, width) = ref_mat.shape
     if norm:
         ref_mat = np.asarray(
             [normalize_image(ref_mat[i]) for i in range(height)])
         mat = np.asarray([normalize_image(mat[i]) for i in range(height)])
     win_size = 2 * (win_size // 2) + 1
     radi = win_size // 2
@@ -1889,15 +1888,15 @@
     """
     (x_index, y_index) = cuda.grid(2)
     if (y_index < height) and (x_index < width):
         radi_ref = radi + margin
         j = x_index + radi_ref
         i = y_index + radi_ref
         ref_mat1 = ref_mat[i - radi_ref:i + radi_ref + 1,
-                   j - radi_ref: j + radi_ref + 1]
+                           j - radi_ref: j + radi_ref + 1]
         mat1 = mat[i - radi:i + radi + 1, j - radi: j + radi + 1]
         coef_mat1 = coef_4d[y_index, x_index, :, :]
         coef_mat1 = __gen_2d_corr_map_2d_input(ref_mat1, mat1, coef_mat1)
         x_max, y_max = __locate_max_value(coef_mat1)
         x_pos, y_pos = __locate_2d_peak_kernel(coef_mat1, x_max, y_max)
         shifts[0, y_index, x_index] = x_pos - margin
         shifts[1, y_index, x_index] = y_pos - margin
@@ -2079,15 +2078,15 @@
     """
     (x_index, y_index) = cuda.grid(2)
     if (y_index < height) and (x_index < width):
         radi_ref = margin + radi
         j = x_index + radi_ref
         i = y_index + radi_ref
         ref_mat1 = ref_mat[:, i - radi_ref:i + radi_ref + 1,
-                   j - radi_ref: j + radi_ref + 1]
+                           j - radi_ref: j + radi_ref + 1]
         mat1 = mat[:, i - radi:i + radi + 1, j - radi: j + radi + 1]
         coef_mat1 = coef_4d[y_index, x_index, :, :]
         coef_mat1 = __gen_2d_corr_map_3d_input(ref_mat1, mat1, coef_mat1)
         x_max, y_max = __locate_max_value(coef_mat1)
         x_pos, y_pos = __locate_2d_peak_kernel(coef_mat1, x_max, y_max)
         shifts[0, y_index, x_index] = x_pos - margin
         shifts[1, y_index, x_index] = y_pos - margin
@@ -2274,15 +2273,15 @@
     (x_index, y_index) = cuda.grid(2)
     if (y_index < height) and (x_index < width):
         radi_ref = margin + radi
         size = 2 * margin + 1
         j = x_index + radi_ref
         i = y_index + radi_ref
         ref_mat1 = ref_mat[:, i - radi_ref:i + radi_ref + 1,
-                   j - radi_ref: j + radi_ref + 1]
+                           j - radi_ref: j + radi_ref + 1]
         mat1 = mat[:, i - radi:i + radi + 1, j - radi: j + radi + 1]
         coef_mat1 = coef_4d[y_index, x_index, :, :]
         coef_mat1 = __gen_2d_corr_map_3d_input(ref_mat1, mat1, coef_mat1)
         for i in range(size):
             for j in range(size):
                 coef_4d[y_index, x_index, i, j] = coef_mat1[i, j]
 
@@ -2737,17 +2736,17 @@
         shifts = np.asarray(shifts)
     else:
         if ncore is None:
             ncore = np.clip(mp.cpu_count() - 1, 1, None)
         shifts = np.asarray(Parallel(n_jobs=ncore)(
             delayed(f_alias)(
                 ref_mat[list_i[k] - start:list_i[k] + start1,
-                list_j[k] - start:list_j[k] + start1],
+                        list_j[k] - start:list_j[k] + start1],
                 mat[list_i[k] - radi:list_i[k] + radi1,
-                list_j[k] - radi:list_j[k] + radi1],
+                    list_j[k] - radi:list_j[k] + radi1],
                 margin, None, sub_pixel, method, 2, size, False, None)
             for k in range(num_point)))
     x_shifts, y_shifts = shifts[:, 0], shifts[:, 1]
     if return_list:
         return x_shifts, y_shifts
     else:
         if global_value == "median":
@@ -2807,15 +2806,15 @@
     """
     idx = cuda.grid(1)
     if idx < num_point:
         radi_ref = radi + margin
         i = list_i[idx]
         j = list_j[idx]
         ref_mat1 = ref_mat[i - radi_ref:i + radi_ref + 1,
-                   j - radi_ref: j + radi_ref + 1]
+                           j - radi_ref: j + radi_ref + 1]
         mat1 = mat[i - radi:i + radi + 1, j - radi: j + radi + 1]
         coef_mat1 = list_2d_coef[idx, :, :]
         coef_mat1 = __gen_2d_corr_map_2d_input(ref_mat1, mat1, coef_mat1)
         x_max, y_max = __locate_max_value(coef_mat1)
         x_pos, y_pos = __locate_2d_peak_kernel(coef_mat1, x_max, y_max)
         shifts[0, idx] = x_pos - margin
         shifts[1, idx] = y_pos - margin
@@ -3163,15 +3162,15 @@
         radi_ref1 = radi_ref + 1
         margin1 = margin + 1
         radi1 = radi + 1
         size = 2 * margin + 1
         j = x_index + radi_ref
         i = y_index + radi_ref
         ref_mat1 = ref_mat[:, i - radi_ref:i + radi_ref1,
-                   j - radi_ref: j + radi_ref1]
+                           j - radi_ref: j + radi_ref1]
         mat1 = mat[:, i - radi:i + radi1, j - radi: j + radi1]
         A = A0[y_index, x_index, :, :]
         V = V0[y_index, x_index, :, :]
         D = D0[y_index, x_index, :, :]
         t5 = coef_4d[y_index, x_index, :, :]
         for k in range(depth):
             __accu_correlate(ref_mat1[k], mat1[k], window, t5)
```

### Comparing `algotom-1.5.0/algotom/util/simulation.py` & `algotom-1.6.0/algotom/util/simulation.py`

 * *Files identical despite different names*

### Comparing `algotom-1.5.0/algotom/util/utility.py` & `algotom-1.6.0/algotom/util/utility.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,85 +45,93 @@
     -   Methods for grid scans:
             +   detect_sample
             +   fix_non_sample_areas
             +   locate_slice
             +   locate_slice_chunk
     -   Methods for speckle-based tomography
             +   generate_spiral_positions
-    -   Methods for finding the center of rotation by visual inspection.
+    -   Method for finding the center of rotation by visual inspection.
             +   find_center_visual_sinograms
-            +   find_center_visual_slices
  """
 
 import sys
 import multiprocessing as mp
 import pywt
 import numpy as np
 import numpy.fft as fft
 from numba import cuda
 import scipy.ndimage as ndi
 from scipy import interpolate
 import scipy.signal.windows as win
 from scipy.signal import savgol_filter
 from joblib import Parallel, delayed
 import algotom.io.loadersaver as losa
-import algotom.prep.removal as remo
-import algotom.prep.filtering as filt
-import algotom.rec.reconstruction as rec
 
 
-def apply_method_to_multiple_sinograms(data, method, para, ncore=None,
-                                       prefer="threads"):
+def parallel_process_slices(data, method, parameters, axis=1, ncore=None,
+                            prefer="threads", **kwargs):
     """
-    Apply a processing method (in "filtering", "removal", and "reconstruction"
-    module) to multiple sinograms or multiple slices in parallel.
+    Apply a processing method to slices of a 3D array in parallel.
 
     Parameters
     ----------
     data : array_like or hdf object
-        3D array data where sinograms/slices are extracted along axis 1,
-        e.g [:, i, :].
-    method : str
-        Name of a method. e.g. "remove_stripe_based_sorting".
-    para : list
-        Parameters of the method. e.g. [21, 1]
-    ncore: int or None
+        3D data array or HDF dataset.
+    method : callable
+        Function to apply to each slice.
+    parameters : list
+        List of positional parameters for the method.
+    axis : int
+        Axis along which the method is applied.
+    ncore : int, optional
         Number of cpu-cores used for computing. Automatically selected if None.
     prefer : {"threads", "processes"}
-        Prefer backend for parallel processing.
+        Preferred parallel backend ("threads" for I/O bound tasks or
+        "processes" for CPU-bound tasks).
+    **kwargs : dict
+        Additional keyword parameters to pass to the method.
 
     Returns
     -------
     array_like
         Same axis-definition as the input.
     """
+    (depth, height, width) = data.shape
     if ncore is None:
         ncore = np.clip(mp.cpu_count() - 1, 1, None)
     else:
         ncore = np.clip(ncore, 1, None)
-    if not isinstance(para, list):
-        para = tuple(list([para]))
+    if not isinstance(parameters, list):
+        parameters = list([parameters])
+    if axis == 2:
+        data_out = Parallel(n_jobs=ncore, prefer=prefer)(
+            delayed(method)(data[:, :, i], *parameters, **kwargs) for i in
+            range(width))
+        data_out = np.copy(np.moveaxis(np.float32(data_out), 0, 2))
+    elif axis == 1:
+        data_out = Parallel(n_jobs=ncore, prefer=prefer)(
+            delayed(method)(data[:, i, :], *parameters, **kwargs) for i in
+            range(height))
+        data_out = np.copy(np.moveaxis(np.float32(data_out), 0, 1))
     else:
-        para = tuple(para)
-    (depth, height, width) = data.shape
-    if method in dir(remo):
-        method_used = getattr(remo, method)
-    elif method in dir(filt):
-        method_used = getattr(filt, method)
-    elif method in dir(rec):
-        method_used = getattr(rec, method)
-    else:
-        raise ValueError("Can't find the method: '{}' in the namespace"
-                         "".format(method))
-    data_out = Parallel(n_jobs=ncore, prefer=prefer)(
-        delayed(method_used)(data[:, i, :], *para) for i in range(height))
-    data_out = np.moveaxis(np.asarray(data_out), 0, 1)
+        data_out = Parallel(n_jobs=ncore, prefer=prefer)(
+            delayed(method)(data[i, :, :], *parameters, **kwargs) for i in
+            range(depth))
+        data_out = np.float32(data_out)
     return data_out
 
 
+def apply_method_to_multiple_sinograms(*args, **kwargs):
+    msg = "!!! 'apply_method_to_multiple_sinograms' has been removed after " \
+          "version 1.5.0. Please use 'parallel_process_slices' instead. " \
+          "Refer to the documentation for details on parameters and usage " \
+          "adjustments needed!!!"
+    raise NotImplementedError(msg)
+
+
 def mapping(mat, x_mat, y_mat, order=1, mode="reflect"):
     """
     Apply a geometric transformation to a 2D array
 
     Parameters
     ----------
     mat : array_like
@@ -910,23 +918,29 @@
     mat = np.asarray(Parallel(n_jobs=ncore, prefer="threads")(
         delayed(apply_1d_regularizer)(mat[i], sijmat) for i in range(nrow)))
     if axis == 0:
         mat = np.transpose(mat)
     return mat
 
 
-def transform_1d_window_to_2d(win_1d):
+def transform_1d_window_to_2d(win_1d, order=1, mode="reflect"):
     """
     Transform a 1d-window to 2d-window.
     Useful for designing a Fourier filter.
 
     Parameters
     ----------
     win_1d : array_like
         1D array.
+    order : int, optional
+        The order of the spline interpolation, default is 1.
+        The order has to be in the range 0-5.
+    mode : {'reflect', 'constant', 'nearest', 'mirror', 'wrap'}, optional
+        The mode parameter determines how the input array is extended beyond
+        its boundaries. Default is 'reflect'.
 
     Returns
     --------
     win_2d : array_like
         Square array, a 2D version of the 1d-window.
     """
     width0 = len(win_1d)
@@ -941,15 +955,15 @@
     r_mat = np.float32(np.clip(np.sqrt(x_mat ** 2 + y_mat ** 2), 0, center))
     theta_mat = np.arctan2(y_mat, x_mat)
     r_mat[theta_mat < 0] *= -1
     r_mat = np.float32(np.clip(r_mat + center, 0, width - 1))
     theta_mat = np.clip(np.float32(theta_mat * (width - 1.0) / np.pi), 0,
                         width - 1)
     mat = np.tile(win_1d, (width, 1))
-    win_2d = mapping(mat, r_mat, theta_mat)
+    win_2d = mapping(mat, r_mat, theta_mat, order=order, mode=mode)
     return win_2d[0:width0, 0:width0]
 
 
 def detect_sample(sinogram, sino_type="180"):
     """
     To check if there is a sample in a sinogram using the "double-wedge"
     property of the Fourier transform of the sinogram (Ref. [1]).
@@ -1403,81 +1417,12 @@
         file_name = "/center_{0:6.2f}".format(center) + ".tif"
         losa.save_image(output_base + file_name, sino_360)
         if display:
             print("Done: {}".format(output_base + file_name))
     return output_base
 
 
-def find_center_visual_slices(sinogram, output, start, stop, step=1, zoom=1.0,
-                              method="dfi", gpu=False, angles=None,
-                              ratio=1.0, filter_name="hann", apply_log=True,
-                              ncore=None, display=False):
-    """
-    For visually finding the center-of-rotation (COR) using reconstructed
-    slices at different CORs.
-
-    Parameters
-    ----------
-    sinogram : array_like
-        2D array. Sinogram image.
-    output : str
-        Base folder for saving reconstructed slices.
-    start : float
-        Starting point for searching CoR.
-    stop : float
-        Ending point for searching CoR.
-    step : float
-        Searching step.
-    zoom : float
-        To resize input and output images. For example, 0.5 <=> reduce the
-        size of images by half.
-    method : {"dfi", "gridrec", "fbp", "astra"}
-        To select a backend method for reconstruction.
-    gpu : bool, optional
-        Use GPU for computing if True.
-    angles : array_like, optional
-        1D array. List of angles (in radian) corresponding to the sinogram.
-    ratio : float, optional
-        To apply a circle mask to the reconstructed image.
-    filter_name : {None, "hann", "bartlett", "blackman", "hamming",\
-                  "nuttall", "parzen", "triang"}
-        Apply a smoothing filter.
-    apply_log : bool, optional
-        Apply the logarithm function to the sinogram before reconstruction.
-    ncore : int or None
-        Number of cpu-cores used for computing. Automatically selected if None.
-    display : bool
-        Print the output if True.
-
-    Returns
-    -------
-    str
-        Folder path to tif images.
-    """
-    output_name = losa.make_folder_name(output, name_prefix="Find_center",
-                                        zero_prefix=3)
-    output_base = output + "/" + output_name
-    (nrow, ncol) = sinogram.shape
-    step = np.clip(step, 0.05, ncol - 1)
-    start = np.clip(start, 0, ncol - 1)
-    stop = np.clip(stop + step, start + step, ncol - 1)
-    if zoom != 1.0:
-        sinogram = ndi.zoom(sinogram, zoom, order=1, mode="nearest")
-        start = start * zoom
-        stop = stop * zoom
-        step = step * zoom
-        list_center = np.arange(start, stop, step)
-        if angles is not None:
-            angles = ndi.zoom(np.tile(angles, (1, 1)), (1.0, zoom))[0]
-    else:
-        list_center = np.arange(start, stop, step)
-    if not cuda.is_available():
-        gpu = False
-    for center in list_center:
-        rec_img = rec._reconstruct_slice(sinogram, center, method, angles,
-                                         ratio, filter_name, apply_log, gpu,
-                                         ncore)
-        file_name = "center_{0:6.2f}".format(center / zoom) + ".tif"
-        losa.save_image(output_base + "/" + file_name, rec_img)
-        if display:
-            print("Done: {}".format(output_base + file_name))
-    return output_base
+def find_center_visual_slices(*args, **kwargs):
+    msg = "!!!'find_center_visual_slices' has been moved to the " \
+          "'reconstruction' module. Please update your import to use " \
+          "'reconstruction.find_center_visual_slices'.!!!"
+    raise ImportError(msg)
```

### Comparing `algotom-1.5.0/algotom.egg-info/PKG-INFO` & `algotom-1.6.0/algotom.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algotom
-Version: 1.5.0
+Version: 1.6.0
 Summary: Data processing algorithms for tomography
 Home-page: https://github.com/algotom/algotom
 Author: Nghia Vo
 Author-email: nvo@bnl.gov
 License: Apache 2.0
 Keywords: Parallel-beam Computed Tomography,Image Processing,Tomography,X-ray Imaging,Phase Contrast Imaging,Ring artifact removal
 Platform: Any
@@ -29,24 +29,27 @@
 ### Data processing (**ALGO**)rithms for (**TOM**)ography.
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/algotom/algotom/algotom_ga.yml) [![Downloads](https://static.pepy.tech/personalized-badge/algotom?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi-downloads)](https://pepy.tech/project/algotom) ![Conda](https://img.shields.io/conda/dn/algotom/algotom?label=conda-downloads) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/algotom/algotom) ![Conda](https://img.shields.io/conda/pn/algotom/algotom) ![GitHub issues](https://img.shields.io/github/issues-raw/algotom/algotom) ![Conda](https://img.shields.io/conda/dn/conda-forge/algotom?label=conda-forge%20downloads) ![Coverage](https://github.com/algotom/algotom/raw/doc/docs/coverage_report/coverage.svg)
 
 
 ![logo](https://github.com/algotom/algotom/raw/master/figs/readme/logo2.png)
 
-**Algotom** is a Python package that implements data processing methods for tomography. 
-It offers a comprehensive pipeline for data processing; including reading and writing data, 
-pre-processing, tomographic reconstruction, post-processing, and data simulation. 
-The package provides numerous utility methods to assist users in rapidly developing 
-prototype methods or constructing a pipeline for processing their own data.
-The main standout features of Algotom are its wealth of pre-processing methods: 
-artifact removal, distortion correction, phase retrieval, processing automation,... 
-The software excels in readability, minimal dependencies, maintainability, 
-and rich documentation. Starting from version 1.1, methods for speckle-based 
-phase-contrast tomography have been incorporated into the package.
+**Algotom** is a Python package designed for tomography data processing. It 
+offers a complete data processing pipeline; including reading and writing data, 
+pre-processing, tomographic reconstruction, post-processing, data simulation, 
+and calibration techniques. The package provides many utility methods to 
+assist users in constructing a pipeline for processing their own data or 
+developing new methods. Key features of Algotom include a wide range of 
+processing methods such as artifact removal, distortion correction, 
+speckle-based phase-contrast imaging, data reduction; and the capability of 
+processing non-standard tomography acquisitions such as grid scans or helical scans. 
+The software stands out for its readability, minimal dependencies, and rich documentation. 
+Developed specifically for synchrotron-based tomographic beamlines, Algotom aims to 
+maximize data quality, enhance workflow throughput, and exploit full beamline 
+capabilities.
 
 Features
 --------
 
 Algotom is a lightweight package. The software is built on top of a few core
 Python libraries to ensure its ease-of-installation. Methods distributed in 
 Algotom have been developed and tested at synchrotron beamlines where massive
@@ -68,26 +71,26 @@
 - Methods for processing helical scans (with/without the offset rotation-axis).
   
   ![helical_scan](https://github.com/algotom/algotom/raw/master/figs/readme/helical_scan.jpg)
 
 - Methods for determining the center-of-rotation (COR) and auto-stitching images 
   in half-acquisition scans (360-degree acquisition with the offset COR).
 
-- Some practical methods developed and implemented for the package:
-  zinger removal, tilted sinogram generation, sinogram distortion correction, 
-  beam hardening correction, DFI (direct Fourier inversion) reconstruction, FBP reconstruction,
-  and double-wedge filter for removing sample parts larger than the FOV in
-  a sinogram.
+- Practical methods developed and implemented for the package: zinger removal, 
+  tilted sinogram generation, sinogram distortion correction, simplified form of Paganin's filter,
+  beam hardening correction, DFI (direct Fourier inversion) reconstruction,
+  FBP (filtered back-projection) reconstruction, BPF (back-projection filtering) reconstruction, 
+  and double-wedge filter for removing sample parts larger than the FOV in a sinogram.
   
   ![pipe_line](https://github.com/algotom/algotom/raw/master/figs/readme/double_wedge_filter.jpg)
   
 - Utility methods for [customizing ring/stripe artifact removal methods](https://algotom.readthedocs.io/en/latest/toc/section4/section4_3.html) 
   and parallelizing computational work.
 
-- Calibration methods for determining pixel-size in helical scans.
+- Calibration methods for helical scans and tomography alignment.
 
 - Methods for generating simulation data: phantom creation, sinogram calculation
   based on the Fourier slice theorem, and artifact generation.
   
   ![simulation](https://github.com/algotom/algotom/raw/master/figs/readme/simulation.png)
 
 - Methods for phase-contrast imaging: phase unwrapping, speckle-based phase retrieval, image correlation, and image alignment.
@@ -95,14 +98,23 @@
   ![speckle](https://github.com/algotom/algotom/raw/master/figs/readme/speckle_based_tomography.png)
 
 - Methods for downsampling, rescaling, and reslicing (+rotating, cropping) 
   3D reconstructed image without large memory usage.
 
   ![reslicing](https://github.com/algotom/algotom/raw/master/figs/readme/reslicing.jpg)
 
+- Direct vertical reconstruction for single slice, multiple slices, and multiple slices at 
+  different orientations.
+  
+  ![vertical_slice1](https://github.com/algotom/algotom/raw/master/figs/readme/direct_vertical_reconstruction.png)
+
+  ![vertical_slice1](https://github.com/algotom/algotom/raw/master/figs/readme/limited_angle_tomography.png)
+  
+   
+
 Installation
 ------------
 
 - https://algotom.readthedocs.io/en/latest/toc/section3.html
 - If users install Algotom to an existing environment and Numba fails to install due to the latest Numpy:
   + Downgrade Numpy and install Algotom/Numba again.
   + Create a new environment and install Algotom first, then other packages.
@@ -115,17 +127,18 @@
 - https://algotom.readthedocs.io/en/latest/toc/section1/section1_4.html
 - https://algotom.readthedocs.io/en/latest/toc/section4.html
 - https://github.com/algotom/algotom/tree/master/examples
 
 Development principles
 ----------------------
 
-- While Algotom offers a comprehensive range of tools for tomographic data processing covering raw-data reading, 
-  pre-processing, reconstruction, post-processing, and data saving; its development primarily focuses on 
-  pre-processing techniques. This distinction makes it a prominent feature among other tomographic software.   
+- While Algotom offers a complete set of tools for tomographic data processing covering 
+  pre-processing, reconstruction, post-processing, data simulation, and calibration techniques;
+  its development strongly focuses on pre-processing techniques. This distinction makes it a
+  prominent feature among other tomographic software.   
 
 - To ensure that the software can work across platforms and is easy-to-install; dependencies are minimized, and only 
   well-maintained [Python libraries](https://github.com/algotom/algotom/blob/master/requirements.txt) are used.
 
 - To achieve high-performance computing and leverage GPU utilization while ensuring ease of understanding, usage, and software 
   maintenance, Numba is used instead of Cupy or PyCuda.
```

### Comparing `algotom-1.5.0/algotom.egg-info/SOURCES.txt` & `algotom-1.6.0/algotom.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,12 +17,13 @@
 algotom/prep/conversion.py
 algotom/prep/correction.py
 algotom/prep/filtering.py
 algotom/prep/phase.py
 algotom/prep/removal.py
 algotom/rec/__init__.py
 algotom/rec/reconstruction.py
+algotom/rec/vertrec.py
 algotom/util/__init__.py
 algotom/util/calibration.py
 algotom/util/correlation.py
 algotom/util/simulation.py
 algotom/util/utility.py
```

### Comparing `algotom-1.5.0/setup.py` & `algotom-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         "joblib"]
 
 current_folder = pathlib.Path(__file__).parent
 readme = (current_folder / "README.md").read_text()
 
 setuptools.setup(
     name="algotom",
-    version="1.5.0",
+    version="1.6.0",
     author="Nghia Vo",
     author_email="nvo@bnl.gov",
     description="Data processing algorithms for tomography",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords=["Parallel-beam Computed Tomography", "Image Processing",
               "Tomography", "X-ray Imaging", "Phase Contrast Imaging",
```

