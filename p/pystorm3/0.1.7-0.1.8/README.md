# Comparing `tmp/pystorm3-0.1.7.tar.gz` & `tmp/pystorm3-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystorm3-0.1.7.tar", last modified: Thu Apr 18 11:54:57 2024, max compression
+gzip compressed data, was "pystorm3-0.1.8.tar", last modified: Tue May  7 15:05:51 2024, max compression
```

## Comparing `pystorm3-0.1.7.tar` & `pystorm3-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-18 11:54:57.264073 pystorm3-0.1.7/
--rw-r--r--   0 dboutet   (3170) meg       (1042)    35140 2024-04-10 15:50:21.000000 pystorm3-0.1.7/LICENSE
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2815 2024-04-18 11:54:57.264073 pystorm3-0.1.7/PKG-INFO
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1933 2024-04-17 17:48:22.000000 pystorm3-0.1.7/README.md
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-18 11:54:57.263073 pystorm3-0.1.7/pystorm/
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1102 2024-04-17 17:40:11.000000 pystorm3-0.1.7/pystorm/__init__.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-18 11:54:57.263073 pystorm3-0.1.7/pystorm/connectivity/
--rw-r--r--   0 dboutet   (3170) meg       (1042)      658 2024-04-18 11:34:27.000000 pystorm3-0.1.7/pystorm/connectivity/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     8715 2024-04-18 11:34:17.000000 pystorm3-0.1.7/pystorm/connectivity/amplitude_envelope_correlation.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-18 11:54:57.263073 pystorm3-0.1.7/pystorm/signal_processing/
--rw-r--r--   0 dboutet   (3170) meg       (1042)      652 2024-04-12 12:13:01.000000 pystorm3-0.1.7/pystorm/signal_processing/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)    39804 2024-04-18 11:54:47.000000 pystorm3-0.1.7/pystorm/signal_processing/band_filter.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-18 11:54:57.263073 pystorm3-0.1.7/pystorm/timefreq/
--rw-r--r--   0 dboutet   (3170) meg       (1042)      761 2024-04-12 11:20:10.000000 pystorm3-0.1.7/pystorm/timefreq/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)    43227 2024-04-18 11:52:47.000000 pystorm3-0.1.7/pystorm/timefreq/analytical_signal.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     4621 2024-04-18 11:10:14.000000 pystorm3-0.1.7/pystorm/timefreq/welch_psd.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-18 11:54:57.263073 pystorm3-0.1.7/pystorm/utils/
--rw-r--r--   0 dboutet   (3170) meg       (1042)      409 2024-04-12 11:26:22.000000 pystorm3-0.1.7/pystorm/utils/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)    36696 2024-04-18 10:48:52.000000 pystorm3-0.1.7/pystorm/utils/minitorch.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)       19 2024-04-18 10:07:02.000000 pystorm3-0.1.7/pystorm/version.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-18 11:54:57.264073 pystorm3-0.1.7/pystorm3.egg-info/
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2815 2024-04-18 11:54:57.000000 pystorm3-0.1.7/pystorm3.egg-info/PKG-INFO
--rw-r--r--   0 dboutet   (3170) meg       (1042)      541 2024-04-18 11:54:57.000000 pystorm3-0.1.7/pystorm3.egg-info/SOURCES.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)        1 2024-04-18 11:54:57.000000 pystorm3-0.1.7/pystorm3.egg-info/dependency_links.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)       69 2024-04-18 11:54:57.000000 pystorm3-0.1.7/pystorm3.egg-info/requires.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)        8 2024-04-18 11:54:57.000000 pystorm3-0.1.7/pystorm3.egg-info/top_level.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)       38 2024-04-18 11:54:57.264073 pystorm3-0.1.7/setup.cfg
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1572 2024-04-17 17:48:50.000000 pystorm3-0.1.7/setup.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-05-07 15:05:51.678763 pystorm3-0.1.8/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    35140 2024-04-10 15:50:21.000000 pystorm3-0.1.8/LICENSE
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2815 2024-05-07 15:05:51.678763 pystorm3-0.1.8/PKG-INFO
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1933 2024-04-17 17:48:22.000000 pystorm3-0.1.8/README.md
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-05-07 15:05:51.654763 pystorm3-0.1.8/pystorm/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1102 2024-04-17 17:40:11.000000 pystorm3-0.1.8/pystorm/__init__.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-05-07 15:05:51.676763 pystorm3-0.1.8/pystorm/connectivity/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      658 2024-04-18 11:34:27.000000 pystorm3-0.1.8/pystorm/connectivity/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     8715 2024-04-18 11:34:17.000000 pystorm3-0.1.8/pystorm/connectivity/amplitude_envelope_correlation.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-05-07 15:05:51.677763 pystorm3-0.1.8/pystorm/signal_processing/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      652 2024-04-12 12:13:01.000000 pystorm3-0.1.8/pystorm/signal_processing/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    39432 2024-05-07 14:55:28.000000 pystorm3-0.1.8/pystorm/signal_processing/band_filter.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-05-07 15:05:51.677763 pystorm3-0.1.8/pystorm/timefreq/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      761 2024-04-12 11:20:10.000000 pystorm3-0.1.8/pystorm/timefreq/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    43311 2024-05-07 14:54:14.000000 pystorm3-0.1.8/pystorm/timefreq/analytical_signal.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     4621 2024-04-18 11:10:14.000000 pystorm3-0.1.8/pystorm/timefreq/welch_psd.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-05-07 15:05:51.677763 pystorm3-0.1.8/pystorm/utils/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      409 2024-04-12 11:26:22.000000 pystorm3-0.1.8/pystorm/utils/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    36720 2024-05-07 14:57:15.000000 pystorm3-0.1.8/pystorm/utils/minitorch.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       19 2024-05-07 14:54:31.000000 pystorm3-0.1.8/pystorm/version.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-05-07 15:05:51.677763 pystorm3-0.1.8/pystorm3.egg-info/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2815 2024-05-07 15:05:51.000000 pystorm3-0.1.8/pystorm3.egg-info/PKG-INFO
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      541 2024-05-07 15:05:51.000000 pystorm3-0.1.8/pystorm3.egg-info/SOURCES.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)        1 2024-05-07 15:05:51.000000 pystorm3-0.1.8/pystorm3.egg-info/dependency_links.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       69 2024-05-07 15:05:51.000000 pystorm3-0.1.8/pystorm3.egg-info/requires.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)        8 2024-05-07 15:05:51.000000 pystorm3-0.1.8/pystorm3.egg-info/top_level.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       38 2024-05-07 15:05:51.678763 pystorm3-0.1.8/setup.cfg
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1572 2024-04-17 17:48:50.000000 pystorm3-0.1.8/setup.py
```

### Comparing `pystorm3-0.1.7/LICENSE` & `pystorm3-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.7/PKG-INFO` & `pystorm3-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorm3
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python implementation of some Brainstorm functions
 Home-page: https://github.com/NeuroLife77/pystorm
 Author: Dominic Boutet
 Author-email: dominic.boutet@mail.mcgill.ca
 Maintainer: Dominic Boutet
 Maintainer-email: dominic.boutet@mail.mcgill.ca
 License: GPL-3.0 license
```

### Comparing `pystorm3-0.1.7/README.md` & `pystorm3-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.7/pystorm/__init__.py` & `pystorm3-0.1.8/pystorm/__init__.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.7/pystorm/connectivity/__init__.py` & `pystorm3-0.1.8/pystorm/connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.7/pystorm/connectivity/amplitude_envelope_correlation.py` & `pystorm3-0.1.8/pystorm/connectivity/amplitude_envelope_correlation.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.7/pystorm/signal_processing/__init__.py` & `pystorm3-0.1.8/pystorm/signal_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.7/pystorm/signal_processing/band_filter.py` & `pystorm3-0.1.8/pystorm/signal_processing/band_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,15 +325,14 @@
 
 
 # This is likely bloated from multiple functions that do the same thing but with different signal dimensions and floating point precisions, but that's my current best solution to this technical problem. 
 def _numba_get_firwin(ntaps, centered_band, beta, fs, precision):
     if precision == "float32":
         return _firwin(ntaps, centered_band, window=("kaiser", beta), scale = True, pass_zero=False,fs=fs).astype(mnt._np_float32)
     elif precision == "float64":
-        print(_firwin(ntaps, centered_band, window=("kaiser", beta), scale = True, pass_zero=False,fs=fs).astype(mnt._np_float64).dtype)
         return _firwin(ntaps, centered_band, window=("kaiser", beta), scale = True, pass_zero=False,fs=fs).astype(mnt._np_float64)
     else:
         return _firwin(ntaps, centered_band, window=("kaiser", beta), scale = True, pass_zero=False,fs=fs)
 @njit
 def _numba_get_fir_window_float32(band, ripple:float, width:float, fs:int):
     """ This function computes the impulse response of the band-pass filter to get the exact same filter as bst-hfilter-2019 in brainstorm.
     
@@ -375,15 +374,14 @@
     centered_band = mnt._np_array([1e-5,fs//2 - 1])
     if band[0] is not None:
         centered_band[0] = band[0]-width/2
     if band[1] is not None:
         centered_band[1] = band[1]+width/2
     with objmode(window='float32[:]'):
         window = _numba_get_firwin(ntaps, centered_band,beta, fs, precision="float32")
-    print(window.dtype)
     return window
 
 
 
 @njit
 def _numba_get_fir_window_float64(band, ripple:float, width:float, fs:int):
     """ This function computes the impulse response of the band-pass filter to get the exact same filter as bst-hfilter-2019 in brainstorm.
@@ -438,15 +436,14 @@
         bp_signal = band_pass_torchaudio(signal,win, fs, return_pad = return_pad, convolve_type = convolve_type, device = device, verbose = 0, return_numba_compatible=True)
     return bp_signal[0], bp_signal[1]
 
 @njit
 def _numba_band_pass_torchaudio_float64_1d(signal,win, fs, return_pad = 0.2, convolve_type = "auto", device="cpu"):
     with objmode(bp_signal='float64[:,:]'):
         bp_signal = band_pass_torchaudio(signal,win, fs, return_pad = return_pad, convolve_type = convolve_type, device = device, verbose = 0, return_numba_compatible=True)
-    print(bp_signal.shape)
     
     return bp_signal[0], bp_signal[1]
 
 @njit
 def _numba_band_pass_torchaudio_float32_2d(signal,win, fs, return_pad = 0.2, convolve_type = "auto", device="cpu"):
     with objmode(bp_signal='float32[:,:]'):
         bp_signal = band_pass_torchaudio(signal,win, fs, return_pad = return_pad, convolve_type = convolve_type, device = device, verbose = 0, return_numba_compatible=True)
@@ -540,19 +537,17 @@
         Returns: 
             filtered_signal: numpy array                       
                 The (possibly still padded) filtered signal.
             signal_mask: numpy array
                 The mask of the signal (specifying the location of the signal within the padded signal) 
     """
     win = _numba_get_fir_window_float64(band,ripple,width,fs)
-    print(signal.shape, win.shape)
     # 1D Torch
     if backend == "torch":
         filtered_signal, filtered_mask = _numba_band_pass_torchaudio_float64_1d(signal,win,fs,return_pad=keep_pad_percent, convolve_type = convolve_type, device = device)
-        print(filtered_signal.shape,filtered_mask.shape)
     elif backend == "scipy":
         filtered_signal, filtered_mask = _numba_band_pass_scipy_float64_1d(signal,win,fs,return_pad=keep_pad_percent, convolve_type = convolve_type)
     else: # For future use
         raise NotImplementedError('The only backends available for now are "torch" and "scipy".')
     return filtered_signal, filtered_mask
 
 @njit
@@ -693,19 +688,17 @@
         Returns: 
             filtered_signal: numpy array                       
                 The (possibly still padded) filtered signal.
             signal_mask: numpy array
                 The mask of the signal (specifying the location of the signal within the padded signal) 
     """
     win = _numba_get_fir_window_float32(band,ripple,width,fs)
-    print(signal.shape, win.shape)
     # 1D Torch
     if backend == "torch":
         filtered_signal, filtered_mask = _numba_band_pass_torchaudio_float32_1d(signal,win,fs,return_pad=keep_pad_percent, convolve_type = convolve_type, device = device)
-        print(filtered_signal.shape,filtered_mask.shape)
     elif backend == "scipy":
         filtered_signal, filtered_mask = _numba_band_pass_scipy_float32_1d(signal,win,fs,return_pad=keep_pad_percent, convolve_type = convolve_type)
     else: # For future use
         raise NotImplementedError('The only backends available for now are "torch" and "scipy".')
     return filtered_signal, filtered_mask
 
 @njit
```

### Comparing `pystorm3-0.1.7/pystorm/timefreq/__init__.py` & `pystorm3-0.1.8/pystorm/timefreq/__init__.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.7/pystorm/timefreq/analytical_signal.py` & `pystorm3-0.1.8/pystorm/timefreq/analytical_signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
                 Specifies the device in which to apply the filtering.
         Returns: 
             analytical_signal: numpy array                       
                 The analytical signal.
     """
 
     if backend == "torch":
+        signal = mnt.ensure_torch(signal)
         if device == "cuda" and signal.nelement() * signal.element_size() > mnt._check_available_memory():
             stderr.write(f'Resource Warning [band_pass()]: Your signal (of size {signal.nelement() * signal.element_size()*1e-6}MB) is too big to be moved to your GPU. Consider splitting the job into blocks. The process will likely crash now. \n')
         analytical_signal = get_hilbert_torch(signal, fs, pad_size = pad_size, window_mask=window_mask, device=device)
     else: # For future use
         raise NotImplementedError('The only backend available for now is "torch".')
     if return_envelope:
         return ensure_numpy(analytical_signal.abs())
@@ -150,14 +151,15 @@
                                                 keep_pad_percent=keep_pad_percent_for_hilbert,
                                                 convolve_type=convolve_type,
                                                 return_with_pad=True,
                                                 backend=backend,device=device,
                                                 verbose = verbose
                                     )
     if backend == "torch":
+        signal = mnt.ensure_torch(signal)
         if device == "cuda" and signal.nelement() * signal.element_size() > mnt._check_available_memory():
             stderr.write(f'Resource Warning [band_pass()]: Your signal (of size {signal.nelement() * signal.element_size()*1e-6}MB) is too big to be moved to your GPU. Consider splitting the job into blocks. The process will likely crash now. \n')
         signal_mask = ensure_torch(signal_mask==1.0)
         pad_size = mnt.argwhere(signal_mask)[0]//fs
         analytical_signal = get_hilbert_torch(filtered_signal[...,signal_mask], fs, pad_size = pad_size, window_mask=None, device=device)
     else: # For future use
         raise NotImplementedError('The only backend available for now is "torch".')
```

### Comparing `pystorm3-0.1.7/pystorm/timefreq/welch_psd.py` & `pystorm3-0.1.8/pystorm/timefreq/welch_psd.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.7/pystorm/utils/minitorch.py` & `pystorm3-0.1.8/pystorm/utils/minitorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from torch import complex64, complex128
 from torch import cos as _cos
 from torch import eye as _eye
 from torch import argwhere as _argwhere
 from torchaudio.functional import convolve as _convolve
 from torchaudio.functional import fftconvolve as _fftconvolve
 from torch import float16,float32,float64
-from torch import set_default_dtype
+from torch import set_default_dtype as _set_default_dtype
 from numpy import ndarray as _ndarray
 from numpy import float32 as _np_float32
 from numpy import float64 as _np_float64
 from numpy import complex64 as _np_complex64
 from numpy import complex128 as _np_complex128
 from numpy import array as _np_array
 from torch import Tensor as _Tensor
@@ -54,15 +54,15 @@
 __default_dtype__ = float64
 __default_complex_dtype__ = complex128
 __default_np_dtype__ = _np_float64
 __default_np_complex_dtype__ = _np_complex128
 __default_dtype_str__ = "float64"
 __default_complex_dtype_str__ = "complex128"
 
-set_default_dtype(__default_dtype__)
+_set_default_dtype(__default_dtype__)
 def set_minitorch_default_dtype(default_type: str = "float64"):
     """ This function allows for specifying a floating point precision (and its matching complex precision). Default is float64 and complex128.
 
         Args: 
             None
         Keyword Args: 
             default_type: str     
@@ -87,15 +87,15 @@
     else:
         __default_dtype__ = float64
         __default_np_dtype__ = _np_float64
         __default_np_complex_dtype__ = _np_complex128
         __default_complex_dtype__ = complex128
         __default_dtype_str__ = "float64"
         __default_complex_dtype_str__ = "complex128"
-    set_default_dtype(__default_dtype__)
+    _set_default_dtype(__default_dtype__)
     print("Type Warning [set_minitorch_default_dtype()]: All previously defined tensors or arrays might have incompatible types with the new default, this could cause some functions to crash, especially those that depend on numba.")
     
 
 def ensure_torch(x, type_float: bool = False, type_complex: bool = False):
     """ This function ensures that the variable is a torch tensor. It optionally also ensures that it is of the default type (as set by 'set_minitorch_default_dtype').
     
         Args:
```

### Comparing `pystorm3-0.1.7/pystorm3.egg-info/PKG-INFO` & `pystorm3-0.1.8/pystorm3.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorm3
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python implementation of some Brainstorm functions
 Home-page: https://github.com/NeuroLife77/pystorm
 Author: Dominic Boutet
 Author-email: dominic.boutet@mail.mcgill.ca
 Maintainer: Dominic Boutet
 Maintainer-email: dominic.boutet@mail.mcgill.ca
 License: GPL-3.0 license
```

### Comparing `pystorm3-0.1.7/pystorm3.egg-info/SOURCES.txt` & `pystorm3-0.1.8/pystorm3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.7/setup.py` & `pystorm3-0.1.8/setup.py`

 * *Files identical despite different names*

