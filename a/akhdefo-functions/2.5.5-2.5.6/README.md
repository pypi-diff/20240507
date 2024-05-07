# Comparing `tmp/akhdefo_functions-2.5.5.tar.gz` & `tmp/akhdefo_functions-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akhdefo_functions-2.5.5.tar", last modified: Fri May  3 18:44:03 2024, max compression
+gzip compressed data, was "akhdefo_functions-2.5.6.tar", last modified: Tue May  7 01:51:25 2024, max compression
```

## Comparing `akhdefo_functions-2.5.5.tar` & `akhdefo_functions-2.5.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 18:44:03.216259 akhdefo_functions-2.5.5/
--rw-rw-rw-   0        0        0     9914 2024-05-03 18:44:03.216259 akhdefo_functions-2.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     8947 2024-04-08 23:20:02.000000 akhdefo_functions-2.5.5/README.md
--rw-rw-rw-   0        0        0     8982 2024-04-14 02:06:02.000000 akhdefo_functions-2.5.5/README_pypi.md
-drwxrwxrwx   0        0        0        0 2024-05-03 18:44:03.200753 akhdefo_functions-2.5.5/akhdefo_functions/
--rw-rw-rw-   0        0        0    79472 2024-04-26 05:03:44.000000 akhdefo_functions-2.5.5/akhdefo_functions/AkhdefoPlot.py
--rw-rw-rw-   0        0        0    10947 2024-04-06 22:52:15.000000 akhdefo_functions-2.5.5/akhdefo_functions/Akhdefo_Classification.py
--rw-rw-rw-   0        0        0     9269 2024-04-06 23:22:26.000000 akhdefo_functions-2.5.5/akhdefo_functions/Akhdefo_Coreg.py
--rw-rw-rw-   0        0        0   114256 2024-04-07 00:41:09.000000 akhdefo_functions-2.5.5/akhdefo_functions/Akhdefo_GOI.py
--rw-rw-rw-   0        0        0    45641 2024-02-16 03:08:55.000000 akhdefo_functions-2.5.5/akhdefo_functions/Akhdefo_TS.py
--rw-rw-rw-   0        0        0    82914 2024-05-03 18:38:57.000000 akhdefo_functions-2.5.5/akhdefo_functions/Akhdefo_Tools.py
--rw-rw-rw-   0        0        0   156103 2024-04-18 20:56:23.000000 akhdefo_functions-2.5.5/akhdefo_functions/Akhdefo_Utilities.py
--rw-rw-rw-   0        0        0    27027 2024-04-07 01:34:16.000000 akhdefo_functions-2.5.5/akhdefo_functions/Filter_PreProc.py
--rw-rw-rw-   0        0        0     8035 2024-04-07 00:09:47.000000 akhdefo_functions-2.5.5/akhdefo_functions/Mosaic_Crop.py
--rw-rw-rw-   0        0        0    45101 2024-01-03 23:08:00.000000 akhdefo_functions-2.5.5/akhdefo_functions/OpticalFlow.py
--rw-rw-rw-   0        0        0    38672 2024-04-07 00:13:18.000000 akhdefo_functions-2.5.5/akhdefo_functions/Stacked_Velocity.py
--rw-rw-rw-   0        0        0    11726 2024-04-06 23:46:27.000000 akhdefo_functions-2.5.5/akhdefo_functions/Unzip_CopyFiles.py
--rw-rw-rw-   0        0        0     3321 2024-04-09 19:48:10.000000 akhdefo_functions-2.5.5/akhdefo_functions/Video_Streamer.py
--rw-rw-rw-   0        0        0      718 2024-05-03 18:39:36.000000 akhdefo_functions-2.5.5/akhdefo_functions/__init__.py
--rw-rw-rw-   0        0        0     3715 2024-04-20 03:34:34.000000 akhdefo_functions-2.5.5/akhdefo_functions/backend.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:44:03.216259 akhdefo_functions-2.5.5/akhdefo_functions.egg-info/
--rw-rw-rw-   0        0        0     9914 2024-05-03 18:44:02.000000 akhdefo_functions-2.5.5/akhdefo_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      760 2024-05-03 18:44:02.000000 akhdefo_functions-2.5.5/akhdefo_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 18:44:02.000000 akhdefo_functions-2.5.5/akhdefo_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-05 01:42:12.000000 akhdefo_functions-2.5.5/akhdefo_functions.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2024-05-03 18:44:02.000000 akhdefo_functions-2.5.5/akhdefo_functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 18:44:03.216259 akhdefo_functions-2.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1834 2024-05-03 18:40:04.000000 akhdefo_functions-2.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:51:25.459773 akhdefo_functions-2.5.6/
+-rw-rw-rw-   0        0        0     9914 2024-05-07 01:51:25.458773 akhdefo_functions-2.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8947 2024-04-08 23:20:02.000000 akhdefo_functions-2.5.6/README.md
+-rw-rw-rw-   0        0        0     8982 2024-04-14 02:06:02.000000 akhdefo_functions-2.5.6/README_pypi.md
+drwxrwxrwx   0        0        0        0 2024-05-07 01:51:25.437673 akhdefo_functions-2.5.6/akhdefo_functions/
+-rw-rw-rw-   0        0        0    79472 2024-04-26 05:03:44.000000 akhdefo_functions-2.5.6/akhdefo_functions/AkhdefoPlot.py
+-rw-rw-rw-   0        0        0    10947 2024-04-06 22:52:15.000000 akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Classification.py
+-rw-rw-rw-   0        0        0     9269 2024-04-06 23:22:26.000000 akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Coreg.py
+-rw-rw-rw-   0        0        0   114256 2024-04-07 00:41:09.000000 akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_GOI.py
+-rw-rw-rw-   0        0        0    45641 2024-02-16 03:08:55.000000 akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_TS.py
+-rw-rw-rw-   0        0        0    82914 2024-05-03 18:38:57.000000 akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Tools.py
+-rw-rw-rw-   0        0        0   156263 2024-05-07 01:45:01.000000 akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Utilities.py
+-rw-rw-rw-   0        0        0    27027 2024-04-07 01:34:16.000000 akhdefo_functions-2.5.6/akhdefo_functions/Filter_PreProc.py
+-rw-rw-rw-   0        0        0     8035 2024-04-07 00:09:47.000000 akhdefo_functions-2.5.6/akhdefo_functions/Mosaic_Crop.py
+-rw-rw-rw-   0        0        0    45101 2024-01-03 23:08:00.000000 akhdefo_functions-2.5.6/akhdefo_functions/OpticalFlow.py
+-rw-rw-rw-   0        0        0    38672 2024-04-07 00:13:18.000000 akhdefo_functions-2.5.6/akhdefo_functions/Stacked_Velocity.py
+-rw-rw-rw-   0        0        0    11726 2024-04-06 23:46:27.000000 akhdefo_functions-2.5.6/akhdefo_functions/Unzip_CopyFiles.py
+-rw-rw-rw-   0        0        0     3321 2024-04-09 19:48:10.000000 akhdefo_functions-2.5.6/akhdefo_functions/Video_Streamer.py
+-rw-rw-rw-   0        0        0      718 2024-05-07 01:50:57.000000 akhdefo_functions-2.5.6/akhdefo_functions/__init__.py
+-rw-rw-rw-   0        0        0     3715 2024-04-20 03:34:34.000000 akhdefo_functions-2.5.6/akhdefo_functions/backend.py
+drwxrwxrwx   0        0        0        0 2024-05-07 01:51:25.457773 akhdefo_functions-2.5.6/akhdefo_functions.egg-info/
+-rw-rw-rw-   0        0        0     9914 2024-05-07 01:51:25.000000 akhdefo_functions-2.5.6/akhdefo_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2024-05-07 01:51:25.000000 akhdefo_functions-2.5.6/akhdefo_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 01:51:25.000000 akhdefo_functions-2.5.6/akhdefo_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-05 01:42:12.000000 akhdefo_functions-2.5.6/akhdefo_functions.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2024-05-07 01:51:25.000000 akhdefo_functions-2.5.6/akhdefo_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 01:51:25.460773 akhdefo_functions-2.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1834 2024-05-07 01:51:14.000000 akhdefo_functions-2.5.6/setup.py
```

### Comparing `akhdefo_functions-2.5.5/PKG-INFO` & `akhdefo_functions-2.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akhdefo_functions
-Version: 2.5.5
+Version: 2.5.6
 Summary: Land Deformation Monitoring Using Optical and SAR Satellite Imagery
 Home-page: https://github.com/mahmudsfu/AkhDefo
 Author: Mahmud Mustafa Muhammad
 Author-email: mahmud.muhamm1@gmail.com
 License: Academic Free License (AFL)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `akhdefo_functions-2.5.5/README.md` & `akhdefo_functions-2.5.6/README.md`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/README_pypi.md` & `akhdefo_functions-2.5.6/README_pypi.md`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/AkhdefoPlot.py` & `akhdefo_functions-2.5.6/akhdefo_functions/AkhdefoPlot.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/Akhdefo_Classification.py` & `akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Classification.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/Akhdefo_Coreg.py` & `akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Coreg.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/Akhdefo_GOI.py` & `akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_GOI.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/Akhdefo_TS.py` & `akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_TS.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/Akhdefo_Tools.py` & `akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Tools.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/Akhdefo_Utilities.py` & `akhdefo_functions-2.5.6/akhdefo_functions/Akhdefo_Utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -2539,15 +2539,15 @@
             delete_older_mp4('plots/Videos', 1500)
             
             frame_suffix = f"_{frame_count}"
         else:
             release_flag==False
         ###################################################################################################################
         label_plot = os.path.join(plot_folder, f"frame_{now.strftime('%Y-%m-%d')}.jpg")
-        file_path_data_csv = os.path.join(data_folder, f"frame_{now.strftime('%Y-%m-%d')}.csv")
+        file_path_data_csv = os.path.join(data_folder, f"frame_{now.strftime('%Y-%m-%d_%H')}.csv")
         
         image_sequence_label=os.path.join(full_path_img, f"frame_{current_time.strftime('%Y-%m-%d_%H-%M-%S')}_{frame_count}.jpg")
         stats_sequence_label=os.path.join(base_directory, f"frame_{current_time.strftime('%Y-%m-%d_%H')}.jpg")
         #stats_sequence_label=os.path.join(full_path_stats, f"frame_{current_time.strftime('%Y-%m-%d_%H')}.jpg")
         stats_sequence_label_H=os.path.join(full_path_stats, f"frame_{current_time.strftime('%Y-%m-%d_%H')}_{frame_count}.jpg")
         #find_and_clean_stats_folders(base_directory)
         
@@ -2804,15 +2804,15 @@
         normalized_magnitudes = cv2.normalize(magnitude, None, norm_type=cv2.NORM_MINMAX, dtype=cv2.CV_32F)
 
         # Convert normalized magnitudes to colors using a colormap
         colormap = plt.get_cmap('hot')  # You can use other colormaps like 'viridis', 'plasma', etc.
         colors = (colormap(normalized_magnitudes)[:, :, :3] * 255).astype(np.uint8)
         ########################################################################3#
        
-        plt.style.use('seaborn-notebook')
+        #plt.style.use('seaborn-notebook')
         
         fig, ax = plt.subplots(1, 1, figsize=(7, 7))
 
         # Display the grayscale image
         ax.imshow(frame_gray_ini_crop, cmap='gray')  # Specifying cmap='gray' for clarity
 
         # Display the velocity data with a professional color map
@@ -2899,15 +2899,15 @@
 
         # Generate Y values for the trendline
         Y_trendline = intercept + slope * datetimes_from_frame
         
         
         total_time=np.cumsum(processing_times)
         total_time=total_time[-1]
-        ax1.plot(datetimes_from_frame, Y_trendline, label=f'(Mean-Displacement Rate: {slope:.4f}) m/{total_minutes:.4f}minutes', color='red', linestyle='-')
+        ax1.plot(datetimes_from_frame, Y_trendline, label=f'(Mean-Displacement Rate:\n {slope:.4f}) m/{total_minutes:.4f}minutes', color='red', linestyle='-')
         
         # Calculate the mean square error (MSE) of the residuals
         residuals = mean_displacement - (slope * datetimes_from_frame + intercept)
         MSE = np.mean(residuals**2)
 
         # Calculate the standard deviation of the y-values
         std_dev = np.sqrt(MSE)
@@ -2988,15 +2988,15 @@
         handles3, labels3 = ax3.get_legend_handles_labels()
 
         # Combining handles and labels
         handles = handles1 + handles3
         labels = labels1 + labels3
 
         # Creating a single legend
-        ax1.legend(handles, labels, loc='upper right', fontsize=12, framealpha=0.85)
+        ax1.legend(handles, labels, loc='center left', fontsize=12, framealpha=0.85, bbox_to_anchor=(1.1, 0.5))
         
         ###ax2##########
         cumulative_processing_times=np.cumsum(processing_times)
         # Adjusted plotting for latency
         target_processing_time = 0.0001  # Approximate real-time target
         latency_times = np.array(processing_times) - target_processing_time
         
@@ -3012,26 +3012,27 @@
         ax2.set_ylabel('Latency Time (seconds)', fontsize=12, fontweight='bold', color='darkred')
 
         # Marking areas to indicate performance
         ax2.fill_between(frame_numbers, latency_times, 0, where=(latency_times > 0), color='red', alpha=0.3, label='Above Real-time Threshold')
         ax2.fill_between(frame_numbers, latency_times, 0, where=(latency_times <= 0), color='green', alpha=0.3, label='Within Real-time Threshold')
 
         # Adding a legend
-        ax2.legend(loc="lower right", fontsize=12)
+        ax2.legend(loc="center left", fontsize=12, bbox_to_anchor=(1, 0.5))
 
         # Styling the ticks
         ax2.tick_params(axis='x', which='both', bottom=True, top=False, labelbottom=True, color='green', direction='in')
         ax2.tick_params(axis='y', which='both', left=True, right=False, labelleft=True, color='green', direction='in')
 
         # Adding minor ticks
         ax2.minorticks_on()
         #ax2.grid(True)
         # Styling the plot background
-        plt.style.use('seaborn-notebook')
-        
+        #plt.style.use('seaborn-notebook')
+        # Adjust plot layout so it doesn't cut off the legend
+        plt.tight_layout(rect=[0, 0, 0.85, 1])
         #########
         
        #######################
         
         ### Save data to csv files
         DD_list=[dd.strftime("%Y-%m-%d") for dd in frame_datetimes ]
         TT_list=[tt.strftime("%H:%M:%S") for tt in frame_datetimes ]
```

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/Filter_PreProc.py` & `akhdefo_functions-2.5.6/akhdefo_functions/Filter_PreProc.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/Mosaic_Crop.py` & `akhdefo_functions-2.5.6/akhdefo_functions/Mosaic_Crop.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/OpticalFlow.py` & `akhdefo_functions-2.5.6/akhdefo_functions/OpticalFlow.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/Stacked_Velocity.py` & `akhdefo_functions-2.5.6/akhdefo_functions/Stacked_Velocity.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/Unzip_CopyFiles.py` & `akhdefo_functions-2.5.6/akhdefo_functions/Unzip_CopyFiles.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/Video_Streamer.py` & `akhdefo_functions-2.5.6/akhdefo_functions/Video_Streamer.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/__init__.py` & `akhdefo_functions-2.5.6/akhdefo_functions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 akhdefo_functions
 
 collection of python modules performs geospatial image processing to moniter land deformation
 """
 
-__version__ = "2.5.5"
+__version__ = "2.5.6"
 __author__ = 'Mahmud Mustafa Muhammad: mahmud.muhamm1@gmail.com'
 __credits__ = 'Simon Fraser university-Department of Earth Sciences'
 
 
 
 
 from  .backend import*
```

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions/backend.py` & `akhdefo_functions-2.5.6/akhdefo_functions/backend.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions.egg-info/PKG-INFO` & `akhdefo_functions-2.5.6/akhdefo_functions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akhdefo-functions
-Version: 2.5.5
+Version: 2.5.6
 Summary: Land Deformation Monitoring Using Optical and SAR Satellite Imagery
 Home-page: https://github.com/mahmudsfu/AkhDefo
 Author: Mahmud Mustafa Muhammad
 Author-email: mahmud.muhamm1@gmail.com
 License: Academic Free License (AFL)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `akhdefo_functions-2.5.5/akhdefo_functions.egg-info/SOURCES.txt` & `akhdefo_functions-2.5.6/akhdefo_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.5/setup.py` & `akhdefo_functions-2.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # Read the long description from the README file
 with open("./README_pypi.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 # Setup configuration
 setup(
     name='akhdefo_functions',
-    version='2.5.5',
+    version='2.5.6',
     description='Land Deformation Monitoring Using Optical and SAR Satellite Imagery',
     url='https://github.com/mahmudsfu/AkhDefo',
     author='Mahmud Mustafa Muhammad',
     author_email='mahmud.muhamm1@gmail.com',
     license='Academic Free License (AFL)',
     packages=['akhdefo_functions'],
     long_description=long_description,
```

