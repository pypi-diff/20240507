# Comparing `tmp/flash_amr_tools-1.0.0.dev1.tar.gz` & `tmp/flash_amr_tools-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flash_amr_tools-1.0.0.dev1.tar", last modified: Mon May  6 13:25:06 2024, max compression
+gzip compressed data, was "flash_amr_tools-1.1.0a1.tar", last modified: Tue May  7 14:50:48 2024, max compression
```

## Comparing `flash_amr_tools-1.0.0.dev1.tar` & `flash_amr_tools-1.1.0a1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-06 13:25:06.451863 flash_amr_tools-1.0.0.dev1/
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     1501 2024-04-30 14:06:17.000000 flash_amr_tools-1.0.0.dev1/LICENSE
--rw-r--r--   0 watanabe  (1000) watanabe  (1000)     6025 2024-05-06 13:25:06.451863 flash_amr_tools-1.0.0.dev1/PKG-INFO
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     3606 2024-05-06 13:07:30.000000 flash_amr_tools-1.0.0.dev1/README.md
-drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-06 13:25:06.451863 flash_amr_tools-1.0.0.dev1/flash_amr_tools/
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       68 2024-05-06 13:05:29.000000 flash_amr_tools-1.0.0.dev1/flash_amr_tools/__init__.py
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)    33133 2024-05-06 13:05:04.000000 flash_amr_tools-1.0.0.dev1/flash_amr_tools/amr_tools.py
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     8991 2024-04-30 14:06:32.000000 flash_amr_tools-1.0.0.dev1/flash_amr_tools/zorder.py
-drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-06 13:25:06.451863 flash_amr_tools-1.0.0.dev1/flash_amr_tools.egg-info/
--rw-r--r--   0 watanabe  (1000) watanabe  (1000)     6025 2024-05-06 13:25:06.000000 flash_amr_tools-1.0.0.dev1/flash_amr_tools.egg-info/PKG-INFO
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)      332 2024-05-06 13:25:06.000000 flash_amr_tools-1.0.0.dev1/flash_amr_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)        1 2024-05-06 13:25:06.000000 flash_amr_tools-1.0.0.dev1/flash_amr_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       44 2024-05-06 13:25:06.000000 flash_amr_tools-1.0.0.dev1/flash_amr_tools.egg-info/requires.txt
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       16 2024-05-06 13:25:06.000000 flash_amr_tools-1.0.0.dev1/flash_amr_tools.egg-info/top_level.txt
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)      741 2024-05-06 13:22:00.000000 flash_amr_tools-1.0.0.dev1/pyproject.toml
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       38 2024-05-06 13:25:06.451863 flash_amr_tools-1.0.0.dev1/setup.cfg
-drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-06 13:25:06.451863 flash_amr_tools-1.0.0.dev1/tests/
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     2278 2024-05-06 13:07:53.000000 flash_amr_tools-1.0.0.dev1/tests/test_amrtools.py
+drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-07 14:50:48.895331 flash_amr_tools-1.1.0a1/
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     1501 2024-04-30 14:06:17.000000 flash_amr_tools-1.1.0a1/LICENSE
+-rw-r--r--   0 watanabe  (1000) watanabe  (1000)     6918 2024-05-07 14:50:48.895331 flash_amr_tools-1.1.0a1/PKG-INFO
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     4502 2024-05-07 14:44:30.000000 flash_amr_tools-1.1.0a1/README.md
+drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-07 14:50:48.895331 flash_amr_tools-1.1.0a1/flash_amr_tools/
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       74 2024-05-07 13:59:02.000000 flash_amr_tools-1.1.0a1/flash_amr_tools/__init__.py
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)    20018 2024-05-07 14:23:33.000000 flash_amr_tools-1.1.0a1/flash_amr_tools/amr_tools.py
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     9694 2024-05-07 14:09:54.000000 flash_amr_tools-1.1.0a1/flash_amr_tools/block_tools.py
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     8991 2024-04-30 14:06:32.000000 flash_amr_tools-1.1.0a1/flash_amr_tools/zorder.py
+drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-07 14:50:48.895331 flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/
+-rw-r--r--   0 watanabe  (1000) watanabe  (1000)     6918 2024-05-07 14:50:48.000000 flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)      363 2024-05-07 14:50:48.000000 flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)        1 2024-05-07 14:50:48.000000 flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       44 2024-05-07 14:50:48.000000 flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/requires.txt
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       16 2024-05-07 14:50:48.000000 flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/top_level.txt
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)      739 2024-05-07 14:29:00.000000 flash_amr_tools-1.1.0a1/pyproject.toml
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       38 2024-05-07 14:50:48.895331 flash_amr_tools-1.1.0a1/setup.cfg
+drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-07 14:50:48.895331 flash_amr_tools-1.1.0a1/tests/
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     3557 2024-05-07 14:28:24.000000 flash_amr_tools-1.1.0a1/tests/test_amrtools.py
```

### Comparing `flash_amr_tools-1.0.0.dev1/LICENSE` & `flash_amr_tools-1.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `flash_amr_tools-1.0.0.dev1/PKG-INFO` & `flash_amr_tools-1.1.0a1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash_amr_tools
-Version: 1.0.0.dev1
+Version: 1.1.0a1
 Summary: Small tool to create uniform data cubes of FLASH datasets. Port from bitbucket.org/pierrenbg/flash-amr-tools
 Author-email: Keito Watanabe <k.wat8973@gmail.com>, Pierre Nürnberger <nuernb@ph1.uni-koeln.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Keito Watanabe
         
         Redistribution and use in source and binary forms, with or without
@@ -57,115 +57,130 @@
 
 ```
 pip install flash-amr-tools
 ```
 
 ## Usage
 
-1. Specify your filename that you want to look at:
+1. Specify your filename, and optionally the region of interest, that you want to look at:
    
 ```
 filename = "SILCC_hdf5_plt_cnt_0150"
+xmin = np.array([2.8931249e+20, -5.78625013e+20, -1.9287499e+20], dtype=np.float32)
+xmax = np.array([6.7506249e+20, -1.92874993e+20,  1.9287499e+20], dtype=np.float32)
 ```
 
-2. Initialise the `AMRToolkit` object:
+If no xmin, xmax are provided, then it defaults to using the whole domain. 
+
+2. Get the block list corresponding to the region of interest.
 
 ```
-from flash_amr_tools import AMRToolkit
+import flash_amr_tools
 
-toolkit = AMRToolkit(filename)
+blist, brefs, bns = flash_amr_tools.get_true_blocks(filename, xmin, xmax)
 ```
 
-The initialisation will calculate the complete list of blocks, the minimum and maximum refinement of the whole domain, and the number of blocks in each dimension.
+This will calculate the complete list of blocks, the maximum and minimum refinement, and the number of blocks at the lowest refinement level within the region of interest.
 
-3. Retrive the data (as specified in `flash.par`) as a uniform grid:
+3. Read in the data using `h5py`
 
 ```
-# ex. density
-dens = toolkit.get_cube("dens")
+import h5py
+
+# read in the data
+pf = h5py.File(filename)
+dens = pf["dens"][()][blist]  # ex. density
+ref_lvl = pf["refine level"][()][blist]
+bbox = pf["bounding box"][()][blist]
+bsize = pf["block size"][()][blist]
+pf.close()
 ```
 
-Note that the naming convention of the argument must follow the variable name in `flash.par`. This now transforms the density as a cube with gridsizes following the highest resolution.
+Note that the naming convention of the argument must follow the variable name in `flash.par`. Note that the refinement levels, the bounding box, and the block size are necessary to determine the coordinates and the refinement levels in each block.
+
+4. Convert the data into a uniform cube
+
+```
+dens_cube = flash_amr_tools.get_cube(dens, ref_lvl=ref_lvl, bbox=bbox, bsize=bsize, brefs=brefs, bns=bns)
+```
+
+This now transforms the density as a cube with gridsizes following the highest resolution.
 
 ### Plotting Routines
 
 Optional plotting routines for slice & on-axis (weighted) projections are also available.
 
 #### Slices
 
-To retrive the slice, we require the field name (as specified in `flash.par`), the position, and the axis(0, 1, or 2) in which the slicing takes place. 
+To retrive the slice, we require the dataset, the position, and the axis(0, 1, or 2) in which the slicing takes place. 
 
 ```
 # ex. density slice along the mid-plane
-dens_sl = toolkit.get_slice("dens", pos=0.0, axis=2)
+dens_sl = flash_amr_tools.get_slice(dens, pos=0.5, axis=2, ref_lvl=ref_lvl, bbox=bbox, bsize=bsize, brefs=brefs, bns=bns)
 ```
 
 #### On-Axis Projections
 
-To obtain the projection, we require the field name (as specified in `flash.par`) and the axis(0, 1, or 2) of the projection.
+To obtain the projection, we require the dataset and the axis(0, 1, or 2) of the projection.
 
 ```
 # ex. column density along the z-axis
-cdens = toolkit.get_cdens("dens", axis=2)
+cdens = flash_amr_tools.get_cdens(dens, axis=2, ref_lvl=ref_lvl, bbox=bbox, bsize=bsize, brefs=brefs, bns=bns)
 ```
 
-Optionally, one can also specify weights to have weighted projections instead. Note that the field name for the weights must also be specified as in `flash.par`
+Optionally, one can also specify weights to have weighted projections instead. Note that the shape of the weights must be the same as that of the dataset.
 
 ```
 # ex. temperature-weighted projection along the z-axis
-cdens_wtemp = toolkit.get_cdens("dens", axis=2, weights_field = "temp")
+
+# first read in other data from h5py
+# read in the data
+pf = h5py.File(filename)
+temp = pf["temp"][()][blist]  # temperature
+pf.close()
+
+# now get temperature-weighted projection along z-axis
+cdens_wtemp = flash_amr_tools.get_cdens(dens, axis=2, ref_lvl=ref_lvl, bbox=bbox, bsize=bsize, brefs=brefs, bns=bns, weights=temp)
 ```
 
 ### Optional routines
 
 #### Further initialisation routines
 
-Optionally, one can specify a particular region of interest to look into. The units should be the same as with those defined in your simulation:
-
-```
-# optional, if one wants to look at a specific region
-xmin = np.array([2.8931249e+20, -5.78625013e+20, -1.9287499e+20], dtype=np.float32)
-xmax = np.array([6.7506249e+20, -1.92874993e+20,  1.9287499e+20], dtype=np.float32)
-
-toolkit = AMRToolkit(filename, xmin, xmax)
-```
-
 One can also optionally force a region to have maximum / minimum refinement by passing the following arguments:
 
 ```
-toolkit = AMRToolkit(filename, xmin, xmax, max_ref_given=10, min_ref_given=3)
+blist, brefs, bns = flash_amr_tools.get_true_blocks(filename, xmin, xmax, max_ref_given=10, min_ref_given=3)
 ```
 which may be useful to conserve memory.
 
-#### Extracting data with preserved AMR structure
-
-If you want to retrive the data **not** as a uniform cube, this can be done with the following function call:
-
-```
-# ex. density
-dens = toolkit.get_data("dens")
-```
-
-This returns the data that is still preserving the AMR structure, which can be useful for ex. scatter plots.
-
 #### Cubes of refinement levels
 
 One can also retrieve the refinement level as a uniform grid as well:
 
 ```
-reflvl_cube = toolkit.get_reflvl_cube()
+reflvl_cube = flash_amr_tools.get_reflvl_cube(ref_lvl=ref_lvl, bbox=bbox, bsize=bsize, brefs=brefs, bns=bns)
 ```
 
 which can be used for (for example) plotting the AMR mesh grid.
 
 #### Vector quantities
 
 One can also retrive a uniform grid of vector quantities (ex. velocity, magnetic field) from the following:
 
 ```
-vel = toolkit.get_vector_cube("vel")
+# read in and save vectorial data as list
+pf = h5py.File(filename)
+vel_vec = [pf["velx"][()][blist], pf["vely"][()][blist], pf["velz"][()][blist]]
+ref_lvl = pf["refine level"][()][blist]
+bbox = pf["bounding box"][()][blist]
+bsize = pf["block size"][()][blist]
+pf.close()
+
+# return uniform cube of vectorial data in each direction
+vel_cube = flash_amr_tools.get_vector_cube(vel_vec, ref_lvl=ref_lvl, bbox=bbox, bsize=bsize, brefs=brefs, bns=bns)
 ```
 
-This will return a 4D array consisting of a 3-D array in each direction.
+This will return a 4D array consisting of a 3-D array in each direction (as the last axis).
 
 ## License
 This code is under the BSD3 license. See [LICENSE](https://github.com/kwat0308/flash-amr-tools/blob/main/LICENSE) for more details.
```

### Comparing `flash_amr_tools-1.0.0.dev1/flash_amr_tools/zorder.py` & `flash_amr_tools-1.1.0a1/flash_amr_tools/zorder.py`

 * *Files identical despite different names*

### Comparing `flash_amr_tools-1.0.0.dev1/flash_amr_tools.egg-info/PKG-INFO` & `flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash_amr_tools
-Version: 1.0.0.dev1
+Version: 1.1.0a1
 Summary: Small tool to create uniform data cubes of FLASH datasets. Port from bitbucket.org/pierrenbg/flash-amr-tools
 Author-email: Keito Watanabe <k.wat8973@gmail.com>, Pierre Nürnberger <nuernb@ph1.uni-koeln.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Keito Watanabe
         
         Redistribution and use in source and binary forms, with or without
@@ -57,115 +57,130 @@
 
 ```
 pip install flash-amr-tools
 ```
 
 ## Usage
 
-1. Specify your filename that you want to look at:
+1. Specify your filename, and optionally the region of interest, that you want to look at:
    
 ```
 filename = "SILCC_hdf5_plt_cnt_0150"
+xmin = np.array([2.8931249e+20, -5.78625013e+20, -1.9287499e+20], dtype=np.float32)
+xmax = np.array([6.7506249e+20, -1.92874993e+20,  1.9287499e+20], dtype=np.float32)
 ```
 
-2. Initialise the `AMRToolkit` object:
+If no xmin, xmax are provided, then it defaults to using the whole domain. 
+
+2. Get the block list corresponding to the region of interest.
 
 ```
-from flash_amr_tools import AMRToolkit
+import flash_amr_tools
 
-toolkit = AMRToolkit(filename)
+blist, brefs, bns = flash_amr_tools.get_true_blocks(filename, xmin, xmax)
 ```
 
-The initialisation will calculate the complete list of blocks, the minimum and maximum refinement of the whole domain, and the number of blocks in each dimension.
+This will calculate the complete list of blocks, the maximum and minimum refinement, and the number of blocks at the lowest refinement level within the region of interest.
 
-3. Retrive the data (as specified in `flash.par`) as a uniform grid:
+3. Read in the data using `h5py`
 
 ```
-# ex. density
-dens = toolkit.get_cube("dens")
+import h5py
+
+# read in the data
+pf = h5py.File(filename)
+dens = pf["dens"][()][blist]  # ex. density
+ref_lvl = pf["refine level"][()][blist]
+bbox = pf["bounding box"][()][blist]
+bsize = pf["block size"][()][blist]
+pf.close()
 ```
 
-Note that the naming convention of the argument must follow the variable name in `flash.par`. This now transforms the density as a cube with gridsizes following the highest resolution.
+Note that the naming convention of the argument must follow the variable name in `flash.par`. Note that the refinement levels, the bounding box, and the block size are necessary to determine the coordinates and the refinement levels in each block.
+
+4. Convert the data into a uniform cube
+
+```
+dens_cube = flash_amr_tools.get_cube(dens, ref_lvl=ref_lvl, bbox=bbox, bsize=bsize, brefs=brefs, bns=bns)
+```
+
+This now transforms the density as a cube with gridsizes following the highest resolution.
 
 ### Plotting Routines
 
 Optional plotting routines for slice & on-axis (weighted) projections are also available.
 
 #### Slices
 
-To retrive the slice, we require the field name (as specified in `flash.par`), the position, and the axis(0, 1, or 2) in which the slicing takes place. 
+To retrive the slice, we require the dataset, the position, and the axis(0, 1, or 2) in which the slicing takes place. 
 
 ```
 # ex. density slice along the mid-plane
-dens_sl = toolkit.get_slice("dens", pos=0.0, axis=2)
+dens_sl = flash_amr_tools.get_slice(dens, pos=0.5, axis=2, ref_lvl=ref_lvl, bbox=bbox, bsize=bsize, brefs=brefs, bns=bns)
 ```
 
 #### On-Axis Projections
 
-To obtain the projection, we require the field name (as specified in `flash.par`) and the axis(0, 1, or 2) of the projection.
+To obtain the projection, we require the dataset and the axis(0, 1, or 2) of the projection.
 
 ```
 # ex. column density along the z-axis
-cdens = toolkit.get_cdens("dens", axis=2)
+cdens = flash_amr_tools.get_cdens(dens, axis=2, ref_lvl=ref_lvl, bbox=bbox, bsize=bsize, brefs=brefs, bns=bns)
 ```
 
-Optionally, one can also specify weights to have weighted projections instead. Note that the field name for the weights must also be specified as in `flash.par`
+Optionally, one can also specify weights to have weighted projections instead. Note that the shape of the weights must be the same as that of the dataset.
 
 ```
 # ex. temperature-weighted projection along the z-axis
-cdens_wtemp = toolkit.get_cdens("dens", axis=2, weights_field = "temp")
+
+# first read in other data from h5py
+# read in the data
+pf = h5py.File(filename)
+temp = pf["temp"][()][blist]  # temperature
+pf.close()
+
+# now get temperature-weighted projection along z-axis
+cdens_wtemp = flash_amr_tools.get_cdens(dens, axis=2, ref_lvl=ref_lvl, bbox=bbox, bsize=bsize, brefs=brefs, bns=bns, weights=temp)
 ```
 
 ### Optional routines
 
 #### Further initialisation routines
 
-Optionally, one can specify a particular region of interest to look into. The units should be the same as with those defined in your simulation:
-
-```
-# optional, if one wants to look at a specific region
-xmin = np.array([2.8931249e+20, -5.78625013e+20, -1.9287499e+20], dtype=np.float32)
-xmax = np.array([6.7506249e+20, -1.92874993e+20,  1.9287499e+20], dtype=np.float32)
-
-toolkit = AMRToolkit(filename, xmin, xmax)
-```
-
 One can also optionally force a region to have maximum / minimum refinement by passing the following arguments:
 
 ```
-toolkit = AMRToolkit(filename, xmin, xmax, max_ref_given=10, min_ref_given=3)
+blist, brefs, bns = flash_amr_tools.get_true_blocks(filename, xmin, xmax, max_ref_given=10, min_ref_given=3)
 ```
 which may be useful to conserve memory.
 
-#### Extracting data with preserved AMR structure
-
-If you want to retrive the data **not** as a uniform cube, this can be done with the following function call:
-
-```
-# ex. density
-dens = toolkit.get_data("dens")
-```
-
-This returns the data that is still preserving the AMR structure, which can be useful for ex. scatter plots.
-
 #### Cubes of refinement levels
 
 One can also retrieve the refinement level as a uniform grid as well:
 
 ```
-reflvl_cube = toolkit.get_reflvl_cube()
+reflvl_cube = flash_amr_tools.get_reflvl_cube(ref_lvl=ref_lvl, bbox=bbox, bsize=bsize, brefs=brefs, bns=bns)
 ```
 
 which can be used for (for example) plotting the AMR mesh grid.
 
 #### Vector quantities
 
 One can also retrive a uniform grid of vector quantities (ex. velocity, magnetic field) from the following:
 
 ```
-vel = toolkit.get_vector_cube("vel")
+# read in and save vectorial data as list
+pf = h5py.File(filename)
+vel_vec = [pf["velx"][()][blist], pf["vely"][()][blist], pf["velz"][()][blist]]
+ref_lvl = pf["refine level"][()][blist]
+bbox = pf["bounding box"][()][blist]
+bsize = pf["block size"][()][blist]
+pf.close()
+
+# return uniform cube of vectorial data in each direction
+vel_cube = flash_amr_tools.get_vector_cube(vel_vec, ref_lvl=ref_lvl, bbox=bbox, bsize=bsize, brefs=brefs, bns=bns)
 ```
 
-This will return a 4D array consisting of a 3-D array in each direction.
+This will return a 4D array consisting of a 3-D array in each direction (as the last axis).
 
 ## License
 This code is under the BSD3 license. See [LICENSE](https://github.com/kwat0308/flash-amr-tools/blob/main/LICENSE) for more details.
```

### Comparing `flash_amr_tools-1.0.0.dev1/pyproject.toml` & `flash_amr_tools-1.1.0a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flash_amr_tools"
-version = "1.0.0dev1"
+version = "1.1.0a1"
 authors = [
   { name="Keito Watanabe", email="k.wat8973@gmail.com" },
   { name="Pierre Nürnberger", email="nuernb@ph1.uni-koeln.de"},
 ]
 description = "Small tool to create uniform data cubes of FLASH datasets. Port from bitbucket.org/pierrenbg/flash-amr-tools"
 readme = "README.md"
 license = {file = "LICENSE"}
```

