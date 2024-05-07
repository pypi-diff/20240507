# Comparing `tmp/napari-stpt-0.1.2.5.tar.gz` & `tmp/napari_stpt-0.1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-stpt-0.1.2.5.tar", last modified: Thu Mar  7 23:01:30 2024, max compression
+gzip compressed data, was "napari_stpt-0.1.2.6.tar", last modified: Tue May  7 15:43:26 2024, max compression
```

## Comparing `napari-stpt-0.1.2.5.tar` & `napari_stpt-0.1.2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2024-03-07 23:01:30.349673 napari-stpt-0.1.2.5/
--rw-r--r--   0 tristan   (1000) tristan   (1000)    35149 2021-10-27 12:13:32.000000 napari-stpt-0.1.2.5/LICENSE
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3916 2024-03-07 23:01:30.347673 napari-stpt-0.1.2.5/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3170 2021-07-01 22:42:19.000000 napari-stpt-0.1.2.5/README.md
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2024-03-07 23:01:30.328673 napari-stpt-0.1.2.5/napari_stpt/
--rw-r--r--   0 tristan   (1000) tristan   (1000)       46 2021-10-27 12:13:32.000000 napari-stpt-0.1.2.5/napari_stpt/__init__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)      267 2022-01-28 14:11:11.000000 napari-stpt-0.1.2.5/napari_stpt/__main__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)     2182 2024-02-13 15:23:08.000000 napari-stpt-0.1.2.5/napari_stpt/custom_qt_dims_slider.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)    39823 2024-03-07 17:20:52.000000 napari-stpt-0.1.2.5/napari_stpt/data.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)     9727 2024-03-07 22:37:17.000000 napari-stpt-0.1.2.5/napari_stpt/my_widgets.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)    77723 2024-03-07 23:00:13.000000 napari-stpt-0.1.2.5/napari_stpt/napari_stpt.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)      726 2024-01-15 16:05:56.000000 napari-stpt-0.1.2.5/napari_stpt/utilities.py
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2024-03-07 23:01:30.345673 napari-stpt-0.1.2.5/napari_stpt.egg-info/
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3916 2024-03-07 23:01:30.000000 napari-stpt-0.1.2.5/napari_stpt.egg-info/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)      421 2024-03-07 23:01:30.000000 napari-stpt-0.1.2.5/napari_stpt.egg-info/SOURCES.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2024-03-07 23:01:30.000000 napari-stpt-0.1.2.5/napari_stpt.egg-info/dependency_links.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       58 2024-03-07 23:01:30.000000 napari-stpt-0.1.2.5/napari_stpt.egg-info/entry_points.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)      160 2024-03-07 23:01:30.000000 napari-stpt-0.1.2.5/napari_stpt.egg-info/requires.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       12 2024-03-07 23:01:30.000000 napari-stpt-0.1.2.5/napari_stpt.egg-info/top_level.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       38 2024-03-07 23:01:30.350673 napari-stpt-0.1.2.5/setup.cfg
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1416 2024-03-07 23:00:38.000000 napari-stpt-0.1.2.5/setup.py
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2024-05-07 15:43:26.889440 napari_stpt-0.1.2.6/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)    35149 2021-10-27 12:13:32.000000 napari_stpt-0.1.2.6/LICENSE
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3916 2024-05-07 15:43:26.885440 napari_stpt-0.1.2.6/PKG-INFO
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3170 2021-07-01 22:42:19.000000 napari_stpt-0.1.2.6/README.md
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2024-05-07 15:43:26.808439 napari_stpt-0.1.2.6/napari_stpt/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       46 2021-10-27 12:13:32.000000 napari_stpt-0.1.2.6/napari_stpt/__init__.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      267 2022-01-28 14:11:11.000000 napari_stpt-0.1.2.6/napari_stpt/__main__.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     2182 2024-02-13 15:23:08.000000 napari_stpt-0.1.2.6/napari_stpt/custom_qt_dims_slider.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)    40045 2024-03-11 14:20:22.000000 napari_stpt-0.1.2.6/napari_stpt/data.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     9727 2024-03-07 22:37:17.000000 napari_stpt-0.1.2.6/napari_stpt/my_widgets.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)    77723 2024-03-07 23:00:13.000000 napari_stpt-0.1.2.6/napari_stpt/napari_stpt.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      726 2024-01-15 16:05:56.000000 napari_stpt-0.1.2.6/napari_stpt/utilities.py
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2024-05-07 15:43:26.878440 napari_stpt-0.1.2.6/napari_stpt.egg-info/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3916 2024-05-07 15:43:26.000000 napari_stpt-0.1.2.6/napari_stpt.egg-info/PKG-INFO
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      421 2024-05-07 15:43:26.000000 napari_stpt-0.1.2.6/napari_stpt.egg-info/SOURCES.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2024-05-07 15:43:26.000000 napari_stpt-0.1.2.6/napari_stpt.egg-info/dependency_links.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       58 2024-05-07 15:43:26.000000 napari_stpt-0.1.2.6/napari_stpt.egg-info/entry_points.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      160 2024-05-07 15:43:26.000000 napari_stpt-0.1.2.6/napari_stpt.egg-info/requires.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       12 2024-05-07 15:43:26.000000 napari_stpt-0.1.2.6/napari_stpt.egg-info/top_level.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       38 2024-05-07 15:43:26.889440 napari_stpt-0.1.2.6/setup.cfg
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     1416 2024-05-07 15:42:42.000000 napari_stpt-0.1.2.6/setup.py
```

### Comparing `napari-stpt-0.1.2.5/LICENSE` & `napari_stpt-0.1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.2.5/PKG-INFO` & `napari_stpt-0.1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stpt
-Version: 0.1.2.5
+Version: 0.1.2.6
 Summary: napari viewer which can read stpt, axio and imc images as zarr files
 Home-page: https://github.com/TristanWhitmarsh/napari-stpt
 Author: Tristan Whitmarsh
 Author-email: tw401@cam.ac.uk
 License: GNU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-stpt-0.1.2.5/README.md` & `napari_stpt-0.1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.2.5/napari_stpt/custom_qt_dims_slider.py` & `napari_stpt-0.1.2.6/napari_stpt/custom_qt_dims_slider.py`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.2.5/napari_stpt/data.py` & `napari_stpt-0.1.2.6/napari_stpt/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,38 +305,40 @@
 
             transform = sitk.Euler2DTransform()
             
             
             slice_name_stpt = f"S{(z+1):03d}"
             home_directory = os.path.expanduser('~')
             
+            #file_path = home_directory + f"/Storage/imaxt/imaxt_reg.2023_v3/{sample_name}/{sample_name}_INT_STPT_STPT_all_reg.parquet"
             file_path = home_directory + f"/Storage/imaxt/imaxt_reg/{sample_name}/{sample_name}_INT_STPT_STPT_all_reg.parquet"
                         
             alignX = 0
             alignY = 0
-            if os.path.exists(file_path):
-                internal_df_stpt = pd.read_parquet(file_path, engine='pyarrow')
-                internal_filtered_df_stpt = internal_df_stpt[(internal_df_stpt['ranking'] == 1) & ((internal_df_stpt['FLAG'] == 1) | (internal_df_stpt['FLAG'] == 0))]
-                internal_row_stpt = internal_filtered_df_stpt[internal_filtered_df_stpt['S_S'] == slice_name_stpt]
-                M = np.array([[internal_row_stpt.iloc[0, 24], internal_row_stpt.iloc[0, 25], internal_row_stpt.iloc[0, 26]], [internal_row_stpt.iloc[0, 27], internal_row_stpt.iloc[0, 28], internal_row_stpt.iloc[0, 29]]])
-
-                #print(M)
-
-                #print(f"resolution*0.1*current_spacing[1] {0.1*current_spacing[1]}")
-    #             align_pos = z + start_slice_number
-    #             alignY = 0
-    #             if not np.isnan(self.corrected_align_y[align_pos]):
-    #                 alignY = -self.corrected_align_y[align_pos]*0.1*current_spacing[1]
-
-    #             alignX = 0
-    #             if not np.isnan(self.corrected_align_x[align_pos]):
-    #                 alignX = -self.corrected_align_x[align_pos]*0.1*current_spacing[0]
+            if False:
+                if os.path.exists(file_path):
+                    internal_df_stpt = pd.read_parquet(file_path, engine='pyarrow')
+                    internal_filtered_df_stpt = internal_df_stpt[(internal_df_stpt['ranking'] == 1) & ((internal_df_stpt['FLAG'] == 1) | (internal_df_stpt['FLAG'] == 0))]
+                    internal_row_stpt = internal_filtered_df_stpt[internal_filtered_df_stpt['S_S'] == slice_name_stpt]
+                    M = np.array([[internal_row_stpt.iloc[0, 24], internal_row_stpt.iloc[0, 25], internal_row_stpt.iloc[0, 26]], [internal_row_stpt.iloc[0, 27], internal_row_stpt.iloc[0, 28], internal_row_stpt.iloc[0, 29]]])
+
+                    #print(M)
+
+                    #print(f"resolution*0.1*current_spacing[1] {0.1*current_spacing[1]}")
+        #             align_pos = z + start_slice_number
+        #             alignY = 0
+        #             if not np.isnan(self.corrected_align_y[align_pos]):
+        #                 alignY = -self.corrected_align_y[align_pos]*0.1*current_spacing[1]
+
+        #             alignX = 0
+        #             if not np.isnan(self.corrected_align_x[align_pos]):
+        #                 alignX = -self.corrected_align_x[align_pos]*0.1*current_spacing[0]
 
-                alignX = -M[0, 2] * 0.1*current_spacing[0] # t_x
-                alignY = -M[1, 2] * 0.1*current_spacing[1]
+                    alignX = -M[0, 2] * 0.1*current_spacing[0] # t_x
+                    alignY = -M[1, 2] * 0.1*current_spacing[1]
 
             #print(f"alignX {alignX}")
             #print(f"alignY {alignY}")
 
             transform.SetTranslation([alignX, alignY])
 
             resampler = sitk.ResampleImageFilter()
```

### Comparing `napari-stpt-0.1.2.5/napari_stpt/my_widgets.py` & `napari_stpt-0.1.2.6/napari_stpt/my_widgets.py`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.2.5/napari_stpt/napari_stpt.py` & `napari_stpt-0.1.2.6/napari_stpt/napari_stpt.py`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.2.5/napari_stpt/utilities.py` & `napari_stpt-0.1.2.6/napari_stpt/utilities.py`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.2.5/napari_stpt.egg-info/PKG-INFO` & `napari_stpt-0.1.2.6/napari_stpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stpt
-Version: 0.1.2.5
+Version: 0.1.2.6
 Summary: napari viewer which can read stpt, axio and imc images as zarr files
 Home-page: https://github.com/TristanWhitmarsh/napari-stpt
 Author: Tristan Whitmarsh
 Author-email: tw401@cam.ac.uk
 License: GNU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-stpt-0.1.2.5/setup.py` & `napari_stpt-0.1.2.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # this grabs the requirements from requirements.txt
 #REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 # This call to setup() does all the work
 setup(
     name="napari-stpt",
-    version="0.1.2.5",
+    version="0.1.2.6",
     description="napari viewer which can read stpt, axio and imc images as zarr files",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/TristanWhitmarsh/napari-stpt",
     author="Tristan Whitmarsh",
     author_email="tw401@cam.ac.uk",
     license="GNU",
```

