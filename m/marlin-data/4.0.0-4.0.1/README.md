# Comparing `tmp/marlin_data-4.0.0.tar.gz` & `tmp/marlin_data-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marlin_data-4.0.0.tar", last modified: Tue May  7 13:59:02 2024, max compression
+gzip compressed data, was "marlin_data-4.0.1.tar", last modified: Tue May  7 17:35:17 2024, max compression
```

## Comparing `marlin_data-4.0.0.tar` & `marlin_data-4.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:59:02.704330 marlin_data-4.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:59:02.692330 marlin_data-4.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:59:02.704330 marlin_data-4.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-07 13:58:49.000000 marlin_data-4.0.0/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-07 13:58:49.000000 marlin_data-4.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 13:58:49.000000 marlin_data-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-07 13:59:02.704330 marlin_data-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-07 13:58:49.000000 marlin_data-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 13:58:49.000000 marlin_data-4.0.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:59:02.704330 marlin_data-4.0.0/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-05-07 13:58:49.000000 marlin_data-4.0.0/__pycache__/marlin_data.cpython-311.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:59:02.704330 marlin_data-4.0.0/marlin_data/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 13:58:49.000000 marlin_data-4.0.0/marlin_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 13:58:49.000000 marlin_data-4.0.0/marlin_data/data.env
--rw-r--r--   0 runner    (1001) docker     (127)    51702 2024-05-07 13:58:49.000000 marlin_data-4.0.0/marlin_data/marlin_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:59:02.704330 marlin_data-4.0.0/marlin_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-07 13:59:02.000000 marlin_data-4.0.0/marlin_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 13:59:02.000000 marlin_data-4.0.0/marlin_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:59:02.000000 marlin_data-4.0.0/marlin_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 13:59:02.000000 marlin_data-4.0.0/marlin_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17996 2024-05-07 13:58:49.000000 marlin_data-4.0.0/marlin_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 13:58:49.000000 marlin_data-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:59:02.704330 marlin_data-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-07 13:58:49.000000 marlin_data-4.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)  5292000 2024-05-07 13:58:49.000000 marlin_data-4.0.0/testfile.vixen
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 13:58:49.000000 marlin_data-4.0.0/token
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:35:17.120061 marlin_data-4.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:35:17.112061 marlin_data-4.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:35:17.120061 marlin_data-4.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-07 17:35:01.000000 marlin_data-4.0.1/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-07 17:35:01.000000 marlin_data-4.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 17:35:01.000000 marlin_data-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-07 17:35:17.120061 marlin_data-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-07 17:35:01.000000 marlin_data-4.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 17:35:01.000000 marlin_data-4.0.1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:35:17.120061 marlin_data-4.0.1/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-05-07 17:35:01.000000 marlin_data-4.0.1/__pycache__/marlin_data.cpython-311.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:35:17.120061 marlin_data-4.0.1/marlin_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 17:35:01.000000 marlin_data-4.0.1/marlin_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 17:35:01.000000 marlin_data-4.0.1/marlin_data/data.env
+-rw-r--r--   0 runner    (1001) docker     (127)    52548 2024-05-07 17:35:01.000000 marlin_data-4.0.1/marlin_data/marlin_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:35:17.120061 marlin_data-4.0.1/marlin_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-07 17:35:17.000000 marlin_data-4.0.1/marlin_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 17:35:17.000000 marlin_data-4.0.1/marlin_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:35:17.000000 marlin_data-4.0.1/marlin_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 17:35:17.000000 marlin_data-4.0.1/marlin_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17996 2024-05-07 17:35:01.000000 marlin_data-4.0.1/marlin_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 17:35:01.000000 marlin_data-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:35:17.124061 marlin_data-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-07 17:35:01.000000 marlin_data-4.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)  5292000 2024-05-07 17:35:01.000000 marlin_data-4.0.1/testfile.vixen
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 17:35:01.000000 marlin_data-4.0.1/token
```

### Comparing `marlin_data-4.0.0/.github/workflows/python-app.yml` & `marlin_data-4.0.1/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `marlin_data-4.0.0/.github/workflows/python-publish.yml` & `marlin_data-4.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `marlin_data-4.0.0/LICENSE` & `marlin_data-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `marlin_data-4.0.0/PKG-INFO` & `marlin_data-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marlin_data
-Version: 4.0.0
+Version: 4.0.1
 Summary: Marlin | Data Framework
 Author: Rahul Tandon
 Author-email: r.tandon@rsaqua.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `marlin_data-4.0.0/README.md` & `marlin_data-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `marlin_data-4.0.0/__pycache__/marlin_data.cpython-311.pyc` & `marlin_data-4.0.1/__pycache__/marlin_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `marlin_data-4.0.0/marlin_data/marlin_data.py` & `marlin_data-4.0.1/marlin_data/marlin_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -565,14 +565,16 @@
         meta_data['snapshot_id'] = snapshot_data['ss_id']
         meta_data['data_frame_start'] = snapshot_data['data_frame_start']
         meta_data['data_frame_end'] = snapshot_data['data_frame_end']
         meta_data['listener_location'] = snapshot_data['data_receiver_location']
         meta_data['location_name'] = snapshot_data['data_receiver_location_name']
         meta_data['frame_delta_t'] = snapshot_data['data_delta_time']
         meta_data['sample_rate'] =  snapshot_data['sample_rate']
+        # meta_data['marlin_time'] = 
+        #print (meta_data['data_frame_start'])
         return meta_data
     
     def load_from_path(self, load_args : {} = None):
         
         load_limit = 5
         load_cnt = 1
         if 'limit' in load_args.keys():
@@ -610,15 +612,15 @@
                         meta_data = json.load(fr)
                     
                     # time considerations
                     start_t_dt = dt.strptime(meta_data['data_frame_start'], '%y%m%d_%H%M%S.%f')
                     snapshot_times[start_t_dt] = snapshot_id
                     
                     end_t_dt = dt.strptime(meta_data['data_frame_end'], '%y%m%d_%H%M%S.%f')
-                    
+                    #print (meta_data['data_frame_end'], end_t_dt)
                     
                     if load_args['snapshot_type'] == "simulation":
                         
                         sig_data = SimulationData(frequency_ts_np = np_data, frequency_ts_pd = pd_data, meta_data = meta_data, start_time=start_t_dt, end_time=end_t_dt)
                         self.simulation_data[snapshot_id] = sig_data
                         # self.simulation_index.append(snapshot_id)
                         
@@ -662,14 +664,26 @@
             _ss = len(self.simulation_data.keys())
             # print (f'{_times} | {_ss}')
             res['number snapshots'] = _ss
             res['number times'] = _times
             res['index size'] = _num
         # for id, time in snapshot_times.items():
         #     print (time)
+        
+        if load_args['snapshot_type'] == "signature":
+            _num = len(self.signature_index)
+            # print (f'{_num} snapshots loaded. Limit : {load_limit}')
+            _times = len(snapshot_times.keys())
+            _ss = len(self.simulation_data.keys())
+            # print (f'{_times} | {_ss}')
+            res['number snapshots'] = _ss
+            res['number times'] = _times
+            res['index size'] = _num
+        
+        
         return res
     
     def build_game(self):
         """
             Add signature / labelled data to the simulation mix in order to ensure we have labelled data in the simulation.
         """
         # --- add siganture snapshots to simulation game if not already present
@@ -677,25 +691,29 @@
             if sig_snap_id  not in self.simulation_index:
                 self.simulation_index.append(sig_snap_id)
                 self.simulation_data[sig_snap_id] = self.signature_data[sig_snap_id]
         
         # --- re order snapshot ids into chronological order
         snapshot_times = {}
         for snapshot in self.simulation_index:
-            start_t_dt = dt.strptime(self.simulation_index[snapshot].meta_data['data_frame_start'], '%y%m%d_%H%M%S.%f')
-            snapshot_times[start_t_dt] = snapshot.metadata['snapshot_id']
-            
+            # print (self.simulation_data[snapshot])
+            start_t_dt = dt.strptime(self.simulation_data[snapshot].meta_data['data_frame_start'], '%y%m%d_%H%M%S.%f')
+            snapshot_times[start_t_dt] = self.simulation_data[snapshot].meta_data['snapshot_id']
+        
+        
         dates_sorted = sorted(snapshot_times.keys())
         # clear index
         self.simulation_index = []
         # rebuild index
         
         for time_ in dates_sorted:
             snapshot_id = snapshot_times[time_]
             self.simulation_index.append(snapshot_id)
+            
+        print (self.simulation_index)
      
     def deserial_data(self, raw_data : {} = None, path : str = "", meta_data : {} = None) -> (np.array, pd.DataFrame):
         """
         Read/stream remote serial data and load into a readable format / data structure.
 
         Args:
             raw_data from a snapshot data query from Marlin API
@@ -1182,16 +1200,16 @@
     
     """--- Tutorial / Quick Start ---
     Download both signature data & run data for use in a ML / simulation setup.
     """
     
     # # 1. instantiate a Marlin Data object
     marlin_data = MarlinData(load_args={'limit' : 100000})
-    simulation_data_path = "/media/vixen/e126674a-75c3-4516-94d2-e59af82d0158/data/downloads/forest_trader/sim"
-    signature_data_path = "/media/vixen/e126674a-75c3-4516-94d2-e59af82d0158/data/downloads/forest_trader/sig"
+    simulation_data_path = "/home/vixen/rs/data/acoustic/ellen/raw_repo/hp/sim"
+    signature_data_path = "/home/vixen/rs/data/acoustic/ellen/raw_repo/hp/sig"
     # # 2. download signatures from RSA signature database
     # #marlin_data.download_signatures()
     # # 3. download simulation / ML run snapshot data
     # # marlin_data.download_simulation_snapshots()
     # # src_data_snapshots = [525010]
     # # 4. create a datafeed from the downloaded snapshot data
     # # data_feed = MarlinDataStreamer(load_args = {'location' : 'clyde_surfer_', 'ss_ids' : src_data_snapshots})
@@ -1270,15 +1288,15 @@
     # data_feed.init_data(marlin_data.signature_data, marlin_data.signature_index)
     
     # for data_inst in data_feed:
     #     print (data_inst.frequency_ts_np)
     #     marlin_data.derived_data.build_derived_labelled_data(signature_data=data_inst)
     
     # path = "/home/vixen/rs/data/acoustic/ellen/raw_repo/model_snaps"
-    marlin_data.download_simulation_snapshots(load_args = {'location' : ['forest_trader'], 'limit':1000000000,'simulation_path' : simulation_data_path})
+    # marlin_data.download_simulation_snapshots(load_args = {'location' : ['forest_trader'], 'limit':1000000000,'simulation_path' : simulation_data_path})
     # # sim_data_feed = MarlinDataStreamer()
     # sim_data_feed.init_data(marlin_data.simulation_data, marlin_data.simulation_index)
     
     # for data_inst in sim_data_feed:
     #     marlin_data.derived_data.build_derived_data(data_inst)
     
     
@@ -1289,16 +1307,19 @@
     #     print (xr)
     # 2023-07-12 20:46:15
     # time_of_interest_str = "12/07/2023, 20:46:00"
     # time_of_interest = time_of_interest_str.strftime("%d/%m/%Y, %H:%M:%S")
     # time_of_interest = dt.strptime(time_of_interest_str, "%d/%m/%Y, %H:%M:%S")
     # print (time_of_interest)
 
-    # r = marlin_data.load_from_path(load_args={'load_path':simulation_data_path, "snapshot_type":"simulation", 'limit':50000, "location":['port_alberni']})
-    # # print (r)
+    r = marlin_data.load_from_path(load_args={'load_path':simulation_data_path, "snapshot_type":"simulation", 'limit':5, "location":['port_alberni']})
+    t = marlin_data.load_from_path(load_args={'load_path':signature_data_path, "snapshot_type":"signature", 'limit':5, "location":['port_alberni']})
+    # marlin_data.build_game()
+    # print (r)
+    # print (t)
     # # data = marlin_data.init_multithread(1, load_args={'location':['clyde_surfer_1']})
     # print (data.mt_snapshot_ids[0])
     # print(marlin_data.simulation_index)
     # sim_data_feed = MarlinDataStreamer()
 
     # initialise data feed
     # sim_data_feed.init_data(marlin_data.simulation_data, marlin_data.simulation_index)
```

### Comparing `marlin_data-4.0.0/marlin_data.egg-info/PKG-INFO` & `marlin_data-4.0.1/marlin_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marlin_data
-Version: 4.0.0
+Version: 4.0.1
 Summary: Marlin | Data Framework
 Author: Rahul Tandon
 Author-email: r.tandon@rsaqua.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `marlin_data-4.0.0/marlin_data.py` & `marlin_data-4.0.1/marlin_data.py`

 * *Files identical despite different names*

### Comparing `marlin_data-4.0.0/setup.py` & `marlin_data-4.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
 
     name="marlin_data", # Replace with your own username
-    version="4.0.0",
+    version="4.0.1",
     author="Rahul Tandon",
     author_email="r.tandon@rsaqua.co.uk",
     description="Marlin | Data Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/vixencapital/brahma/archive/0.0.5.tar.gz",
     packages=setuptools.find_packages(),
```

### Comparing `marlin_data-4.0.0/testfile.vixen` & `marlin_data-4.0.1/testfile.vixen`

 * *Files identical despite different names*

