# Comparing `tmp/cell_data_loader-0.0.3.tar.gz` & `tmp/cell_data_loader-0.0.4.tar.gz`

## Comparing `cell_data_loader-0.0.3.tar` & `cell_data_loader-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/__init__.py
--rwxr-xr-x   0        0        0     1509 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/example_numpy.py
--rwxr-xr-x   0        0        0     1568 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/example_torch.py
--rwxr-xr-x   0        0        0      329 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/github_push.sh
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/pypi_push.sh
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/requirements.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/setup.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/src/cell_data_loader/__init__.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/src/cell_data_loader/base_dataset.py
--rwxr-xr-x   0        0        0    16470 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/src/cell_data_loader/cell_data_loader.py
--rwxr-xr-x   0        0        0    29083 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/src/cell_data_loader/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/tests/__init__.py
--rwxr-xr-x   0        0        0     5722 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/tests/unit_tests.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/README.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 cell_data_loader-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    38037 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/__init__.py
+-rwxr-xr-x   0        0        0     1659 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/example_numpy.py
+-rwxr-xr-x   0        0        0     2451 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/example_torch.py
+-rwxr-xr-x   0        0        0      367 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/github_push.sh
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/pypi_push.sh
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/setup.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/src/cell_data_loader/__init__.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/src/cell_data_loader/base_dataset.py
+-rwxr-xr-x   0        0        0    16625 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/src/cell_data_loader/cell_data_loader.py
+-rwxr-xr-x   0        0        0    29083 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/src/cell_data_loader/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/tests/__init__.py
+-rwxr-xr-x   0        0        0     5774 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/tests/unit_tests.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/README.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 cell_data_loader-0.0.4/PKG-INFO
```

### Comparing `cell_data_loader-0.0.3/src/cell_data_loader/base_dataset.py` & `cell_data_loader-0.0.4/src/cell_data_loader/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cell_data_loader-0.0.3/src/cell_data_loader/cell_data_loader.py` & `cell_data_loader-0.0.4/src/cell_data_loader/cell_data_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,14 @@
 		batch_size = 64,
 		verbose = True,
 		dtype = "torch",
 		gpu_ids = None,
 		label_balance = True,
 		cell_box_regex = None,
 		cell_box_filelist = None,
-		filelists = None,
 		n_channels = None,
 		channels_first = True,
 		match_labels=False):
 		
 		self.verbose = verbose
 		self.label_balance = label_balance
 		self.segment_image = segment_image.lower()
@@ -355,15 +354,15 @@
 		"""
 		self.batch = None
 		self.label_batch = None # [ 0 for _ in range(self.batch_size) ]
 		if self.return_labels():
 			if self.dtype == "numpy":
 				self.label_batch = np.zeros((self.batch_size,self.n_labels))
 			elif self.dtype == "torch":
-				self.label_batch = torch.zeros(self.batch_size,self.n_labels,
+				self.label_batch = torch.zeros((self.batch_size,self.n_labels),
 					device = self.gpu_ids)
 		sample = self.image_objects[0]
 		if n_channels is None:
 			self.n_channels = sample.get_n_channels()
 		else:
 			self.n_channels = n_channels
 		for image_object in self.image_objects:
@@ -482,20 +481,24 @@
 					self.label_batch[i,y] = 1
 			else:
 				im = self.next_im()
 				while isinstance(im,int) and im == -1:
 					im = self.next_im()
 			assert(not isinstance(im,int))
 			if self.dtype == "torch":
+				if len(im.size()) == 2 and self.n_channels == 1:
+					im = torch.unsqueeze(im,2)
 				self.batch[i,...] = torch.unsqueeze(im,0)
 				if self.channels_first:
 					b = torch.moveaxis(self.batch,-1,1)
 				else:
 					b = self.batch
 			elif self.dtype == "numpy":
+				if len(im.shape) == 2 and self.n_channels == 1:
+					im = np.expand_dims(im,axis=2)
 				self.batch[i,...] = np.expand_dims(im,axis=0)
 				if self.channels_first:
 					b = np.moveaxis(self.batch,-1,1)
 				else:
 					b = self.batch
 			else:
 				raise Exception("Unimplemented dtype: %s" % self.dtype)
```

### Comparing `cell_data_loader-0.0.3/src/cell_data_loader/util.py` & `cell_data_loader-0.0.4/src/cell_data_loader/util.py`

 * *Files identical despite different names*

### Comparing `cell_data_loader-0.0.3/tests/unit_tests.py` & `cell_data_loader-0.0.4/tests/unit_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #from src.cell_data_loader import *
 import os,sys,time
 import numpy as np
 import torch
 
 wd         = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
-im_root    = os.path.join(os.path.dirname(wd),'cell_data_loader_data')
+im_root    = os.path.join(wd,'data')
 #imfile_svs = os.path.join(im_root,'10447627_1.svs')
 imfolder1  = os.path.join(im_root,'4173633_5')
 imfolder2  = os.path.join(im_root,'3368914_4_non_tumor')
 imfolder3  = os.path.join(im_root,'H6-13_Mars1+dapi')
 sys.path.insert(0,os.path.join(wd))
 from src.cell_data_loader import *
 
@@ -155,25 +155,26 @@
 		batch_size = 5
 		dim = (6,7)
 		for dtype in ["torch","numpy"]:
 			if dtype == "torch":
 				if not torch.cuda.is_available():
 					print("No available GPU for torch -- skipping")
 					continue
-				device = torch.cuda.current_device()
+				devices = [torch.cuda.device(i) for i in range(torch.cuda.device_count())]
 			elif dtype == "numpy":
 				continue
-			dataset = CellDataloader(imfolder1,imfolder2,imfolder3,dim=dim,
-				batch_size=batch_size,dtype=dtype,match_labels=True,
-				gpu_ids = device)
-			for x,y in dataset:
-				if dtype == "torch":
-					self.assertEquals(device,x.device.index)
-					self.assertEquals(device,y.device.index)
-					break
-				elif dtype == "numpy":
-					break
-				else:
-					break
+			for device in devices:
+				dataset = CellDataloader(imfolder1,imfolder2,imfolder3,dim=dim,
+					batch_size=batch_size,dtype=dtype,match_labels=True,
+					gpu_ids = device.idx)
+				for x,y in dataset:
+					if dtype == "torch":
+						self.assertEqual(device.idx,x.device.index)
+						self.assertEqual(device.idx,y.device.index)
+						break
+					elif dtype == "numpy":
+						break
+					else:
+						break
 
 if __name__ == "__main__":
 	unittest.main()
```

### Comparing `cell_data_loader-0.0.3/pyproject.toml` & `cell_data_loader-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "cell_data_loader"
 
-version = "0.0.3"
+version = "0.0.4"
 
 dependencies = [
   "numpy",
   "scipy",
   "torch",
   "torchvision",
   "opencv-python>=4.5.4",
```

