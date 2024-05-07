# Comparing `tmp/pydeflate-1.4.0.tar.gz` & `tmp/pydeflate-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeflate-1.4.0.tar", max compression
+gzip compressed data, was "pydeflate-1.4.1.tar", max compression
```

## Comparing `pydeflate-1.4.0.tar` & `pydeflate-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1070 2024-05-06 09:26:03.547414 pydeflate-1.4.0/LICENSE
--rw-r--r--   0        0        0     8999 2024-05-06 09:26:03.547414 pydeflate-1.4.0/README.md
--rw-r--r--   0        0        0       25 2024-05-06 09:26:03.547414 pydeflate-1.4.0/pydeflate/.pydeflate_data/README.md
--rw-r--r--   0        0        0      817 2024-05-06 09:26:03.547414 pydeflate-1.4.0/pydeflate/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 09:26:03.547414 pydeflate-1.4.0/pydeflate/deflate/__init__.py
--rw-r--r--   0        0        0    11850 2024-05-06 09:26:03.547414 pydeflate-1.4.0/pydeflate/deflate/deflate.py
--rw-r--r--   0        0        0     2684 2024-05-06 09:26:03.547414 pydeflate-1.4.0/pydeflate/deflate/deflator.py
--rw-r--r--   0        0        0        0 2024-05-06 09:26:03.547414 pydeflate-1.4.0/pydeflate/get_data/__init__.py
--rw-r--r--   0        0        0     2285 2024-05-06 09:26:03.551414 pydeflate-1.4.0/pydeflate/get_data/deflate_data.py
--rw-r--r--   0        0        0    12091 2024-05-06 09:26:03.551414 pydeflate-1.4.0/pydeflate/get_data/exchange_data.py
--rw-r--r--   0        0        0     2693 2024-05-06 09:26:03.551414 pydeflate-1.4.0/pydeflate/get_data/imf_data.py
--rw-r--r--   0        0        0     4492 2024-05-06 09:26:03.551414 pydeflate-1.4.0/pydeflate/get_data/oecd_data.py
--rw-r--r--   0        0        0     2103 2024-05-06 09:26:03.551414 pydeflate-1.4.0/pydeflate/get_data/wb_data.py
--rw-r--r--   0        0        0      894 2024-05-06 09:26:03.551414 pydeflate-1.4.0/pydeflate/pydeflate_config.py
--rw-r--r--   0        0        0      133 2024-05-06 09:26:03.551414 pydeflate-1.4.0/pydeflate/settings/emu.json
--rw-r--r--   0        0        0      911 2024-05-06 09:26:03.551414 pydeflate-1.4.0/pydeflate/settings/oecd_codes.json
--rw-r--r--   0        0        0       47 2024-05-06 09:26:03.551414 pydeflate-1.4.0/pydeflate/tools/__init__.py
--rw-r--r--   0        0        0     5465 2024-05-06 09:26:03.551414 pydeflate-1.4.0/pydeflate/tools/exchange.py
--rw-r--r--   0        0        0     2109 2024-05-06 09:26:03.551414 pydeflate-1.4.0/pydeflate/tools/update_data.py
--rw-r--r--   0        0        0     1573 2024-05-06 09:26:03.551414 pydeflate-1.4.0/pydeflate/utils.py
--rw-r--r--   0        0        0     1023 2024-05-06 09:26:03.551414 pydeflate-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    10030 1970-01-01 00:00:00.000000 pydeflate-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-07 15:41:49.036891 pydeflate-1.4.1/LICENSE
+-rw-r--r--   0        0        0     8999 2024-05-07 15:41:49.036891 pydeflate-1.4.1/README.md
+-rw-r--r--   0        0        0       25 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/.pydeflate_data/README.md
+-rw-r--r--   0        0        0      817 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/deflate/__init__.py
+-rw-r--r--   0        0        0    11850 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/deflate/deflate.py
+-rw-r--r--   0        0        0     2684 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/deflate/deflator.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/get_data/__init__.py
+-rw-r--r--   0        0        0     2285 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/get_data/deflate_data.py
+-rw-r--r--   0        0        0    12248 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/get_data/exchange_data.py
+-rw-r--r--   0        0        0     2693 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/get_data/imf_data.py
+-rw-r--r--   0        0        0     4492 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/get_data/oecd_data.py
+-rw-r--r--   0        0        0     2103 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/get_data/wb_data.py
+-rw-r--r--   0        0        0      894 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/pydeflate_config.py
+-rw-r--r--   0        0        0      133 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/settings/emu.json
+-rw-r--r--   0        0        0      911 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/settings/oecd_codes.json
+-rw-r--r--   0        0        0       47 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/tools/__init__.py
+-rw-r--r--   0        0        0     5465 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/tools/exchange.py
+-rw-r--r--   0        0        0     2109 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/tools/update_data.py
+-rw-r--r--   0        0        0     1573 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pydeflate/utils.py
+-rw-r--r--   0        0        0     1023 2024-05-07 15:41:49.036891 pydeflate-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    10030 1970-01-01 00:00:00.000000 pydeflate-1.4.1/PKG-INFO
```

### Comparing `pydeflate-1.4.0/LICENSE` & `pydeflate-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeflate-1.4.0/README.md` & `pydeflate-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pydeflate-1.4.0/pydeflate/__init__.py` & `pydeflate-1.4.1/pydeflate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = """Jorge Rivera"""
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 
 from pydeflate.deflate.deflate import deflate
 from pydeflate.tools.exchange import exchange
 from pydeflate.tools.update_data import update_all_data, warn_updates
 from pydeflate.get_data.oecd_data import update_dac1
 from pydeflate import get_data
```

### Comparing `pydeflate-1.4.0/pydeflate/deflate/deflate.py` & `pydeflate-1.4.1/pydeflate/deflate/deflate.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.4.0/pydeflate/deflate/deflator.py` & `pydeflate-1.4.1/pydeflate/deflate/deflator.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.4.0/pydeflate/get_data/deflate_data.py` & `pydeflate-1.4.1/pydeflate/get_data/deflate_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.4.0/pydeflate/get_data/exchange_data.py` & `pydeflate-1.4.1/pydeflate/get_data/exchange_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,26 +171,33 @@
     def update(**kwargs) -> None:
         """Update the DAC1 data, which is the source for the OECD exchange rates."""
         from pydeflate.get_data import oecd_data
 
         oecd_data.update_dac1()
 
     def load_data(self, **kwargs) -> None:
-        """Load the DAC1 data, which is the source for the OECD exchange rates."""
-        # avoid infinite recursion
-        if self._load_try_count < 1:
-            try:
-                self._data = pd.read_feather(PYDEFLATE_PATHS.data / "dac1.feather")
-            except FileNotFoundError:
-                logger.info("OECD Data not found, downloading...")
-                self._load_try_count = +1
-                self.update()
-                self.load_data()
-        else:
-            raise FileNotFoundError("Could not load OECD data")
+        """Load the OECD DAC price deflators data.
+
+        If the data is not found, it will be downloaded.
+        DAC deflators are transformed into price deflators by using the
+        implied exchange rate information from the OECD DAC data.
+
+        The deflators that are loaded is therefore *not* the DAC deflator,
+        but the price deflator used to produce the DAC deflators.
+
+        """
+        try:
+            self._data = pd.read_feather(
+                PYDEFLATE_PATHS.data / "pydeflate_dac1.feather"
+            )
+        except FileNotFoundError:
+            logger.info("Data not found, downloading...")
+            self.update()
+            self.load_data()
+            return
 
     def usd_exchange_rate(self, direction: str = "lcu_usd") -> pd.DataFrame:
         """Get the exchange rate of a currency to USD (or vice versa)
 
         Args:
             direction: the direction of the exchange rate. Either "lcu_to_usd"
             or "usd_to_lcu".
```

### Comparing `pydeflate-1.4.0/pydeflate/get_data/imf_data.py` & `pydeflate-1.4.1/pydeflate/get_data/imf_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.4.0/pydeflate/get_data/oecd_data.py` & `pydeflate-1.4.1/pydeflate/get_data/oecd_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.4.0/pydeflate/get_data/wb_data.py` & `pydeflate-1.4.1/pydeflate/get_data/wb_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.4.0/pydeflate/pydeflate_config.py` & `pydeflate-1.4.1/pydeflate/pydeflate_config.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.4.0/pydeflate/settings/oecd_codes.json` & `pydeflate-1.4.1/pydeflate/settings/oecd_codes.json`

 * *Files identical despite different names*

### Comparing `pydeflate-1.4.0/pydeflate/tools/exchange.py` & `pydeflate-1.4.1/pydeflate/tools/exchange.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.4.0/pydeflate/tools/update_data.py` & `pydeflate-1.4.1/pydeflate/tools/update_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.4.0/pydeflate/utils.py` & `pydeflate-1.4.1/pydeflate/utils.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.4.0/pyproject.toml` & `pydeflate-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydeflate"
-version = "1.4.0"
+version = "1.4.1"
 description = "Package to convert current prices figures to constant prices and vice versa"
 authors = ["Jorge Rivera <jorge.rivera@one.org>"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: End Users/Desktop',
```

### Comparing `pydeflate-1.4.0/PKG-INFO` & `pydeflate-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeflate
-Version: 1.4.0
+Version: 1.4.1
 Summary: Package to convert current prices figures to constant prices and vice versa
 License: MIT
 Author: Jorge Rivera
 Author-email: jorge.rivera@one.org
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

