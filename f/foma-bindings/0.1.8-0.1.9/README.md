# Comparing `tmp/foma_bindings-0.1.8.tar.gz` & `tmp/foma_bindings-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foma_bindings-0.1.8.tar", last modified: Thu Aug 17 16:44:19 2023, max compression
+gzip compressed data, was "foma_bindings-0.1.9.tar", last modified: Thu Aug 17 18:59:08 2023, max compression
```

## Comparing `foma_bindings-0.1.8.tar` & `foma_bindings-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-08-17 16:44:19.614271 foma_bindings-0.1.8/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)    11361 2023-06-22 16:58:19.000000 foma_bindings-0.1.8/LICENSE.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3849 2023-08-17 16:44:19.614271 foma_bindings-0.1.8/PKG-INFO
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3049 2023-07-06 16:28:10.000000 foma_bindings-0.1.8/README.md
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-08-17 16:44:19.614271 foma_bindings-0.1.8/foma_bindings/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     4769 2023-06-23 12:54:26.000000 foma_bindings-0.1.8/foma_bindings/__init__.py
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-08-17 16:44:19.614271 foma_bindings-0.1.8/foma_bindings/fst/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)    17580 2023-08-17 16:43:45.000000 foma_bindings-0.1.8/foma_bindings/fst/__init__.py
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-08-17 16:44:19.614271 foma_bindings-0.1.8/foma_bindings/mtfst/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     6343 2023-06-22 18:17:49.000000 foma_bindings-0.1.8/foma_bindings/mtfst/__init__.py
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-08-17 16:44:19.614271 foma_bindings-0.1.8/foma_bindings.egg-info/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3849 2023-08-17 16:44:19.000000 foma_bindings-0.1.8/foma_bindings.egg-info/PKG-INFO
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)      281 2023-08-17 16:44:19.000000 foma_bindings-0.1.8/foma_bindings.egg-info/SOURCES.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)        1 2023-08-17 16:44:19.000000 foma_bindings-0.1.8/foma_bindings.egg-info/dependency_links.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       14 2023-08-17 16:44:19.000000 foma_bindings-0.1.8/foma_bindings.egg-info/top_level.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       98 2023-06-23 14:47:50.000000 foma_bindings-0.1.8/pyproject.toml
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       38 2023-08-17 16:44:19.614271 foma_bindings-0.1.8/setup.cfg
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     1663 2023-08-17 16:44:07.000000 foma_bindings-0.1.8/setup.py
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-08-17 18:59:08.048459 foma_bindings-0.1.9/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)    11361 2023-06-22 16:58:19.000000 foma_bindings-0.1.9/LICENSE.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3849 2023-08-17 18:59:08.048459 foma_bindings-0.1.9/PKG-INFO
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3049 2023-07-06 16:28:10.000000 foma_bindings-0.1.9/README.md
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-08-17 18:59:08.048459 foma_bindings-0.1.9/foma_bindings/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     4823 2023-08-17 18:09:16.000000 foma_bindings-0.1.9/foma_bindings/__init__.py
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-08-17 18:59:08.048459 foma_bindings-0.1.9/foma_bindings/fst/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)    17788 2023-08-17 18:49:53.000000 foma_bindings-0.1.9/foma_bindings/fst/__init__.py
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-08-17 18:59:08.048459 foma_bindings-0.1.9/foma_bindings/mtfst/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     6343 2023-06-22 18:17:49.000000 foma_bindings-0.1.9/foma_bindings/mtfst/__init__.py
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-08-17 18:59:08.048459 foma_bindings-0.1.9/foma_bindings.egg-info/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3849 2023-08-17 18:59:08.000000 foma_bindings-0.1.9/foma_bindings.egg-info/PKG-INFO
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)      281 2023-08-17 18:59:08.000000 foma_bindings-0.1.9/foma_bindings.egg-info/SOURCES.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)        1 2023-08-17 18:59:08.000000 foma_bindings-0.1.9/foma_bindings.egg-info/dependency_links.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       14 2023-08-17 18:59:08.000000 foma_bindings-0.1.9/foma_bindings.egg-info/top_level.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       98 2023-06-23 14:47:50.000000 foma_bindings-0.1.9/pyproject.toml
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       38 2023-08-17 18:59:08.048459 foma_bindings-0.1.9/setup.cfg
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     1663 2023-08-17 18:58:49.000000 foma_bindings-0.1.9/setup.py
```

### Comparing `foma_bindings-0.1.8/LICENSE.txt` & `foma_bindings-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foma_bindings-0.1.8/PKG-INFO` & `foma_bindings-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foma_bindings
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python bindings for the foma finite-state technology suite
 Home-page: https://github.com/CultureFoundryCA/foma_bindings
 Author: CultureFoundry
 Author-email: info@culturefoundrystudios.com
 License: Apache 2.0
 Keywords: foma,xfst,hfst,fst,fsm,mtfst,mtfsm
 Platform: UNKNOWN
```

### Comparing `foma_bindings-0.1.8/README.md` & `foma_bindings-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `foma_bindings-0.1.8/foma_bindings/__init__.py` & `foma_bindings-0.1.9/foma_bindings/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 foma_apply_words = foma.apply_words
 foma_apply_words.restype = c_char_p
 
 # Set functions.
 foma_apply_set_print_space = foma.apply_set_print_space
 foma_apply_set_show_flags = foma.apply_set_show_flags
 foma_apply_set_space_symbol = foma.apply_set_space_symbol
+foma_apply_set_obey_flags = foma.apply_set_obey_flags
 
 # Define functions.
 defined_functions_init = foma.defined_functions_init
 defined_functions_init.restype = c_void_p
 defined_networks_init = foma.defined_networks_init
 defined_networks_init.restype = c_void_p
 foma_add_defined = foma.add_defined
```

### Comparing `foma_bindings-0.1.8/foma_bindings/fst/__init__.py` & `foma_bindings-0.1.9/foma_bindings/fst/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     fst = Fst.load('/path/to/foma/binary')
     fst.apply_up('fox', flags=Fst.PRINT_FLAGS | Fst.PRINT_SPACES)
     ```
 
     Constants for printing:
         - PRINT_SPACES
         - PRINT_FLAGS
+        - DONT_OBEY_FLAGS
         - TOKENIZE
         - VERBOSE = TOKENIZE | PRINT_FLAGS
 
     Word-Accessor Functions:
         - apply_down
         - apply_up
         - lower_words
@@ -76,15 +77,16 @@
     # Bit flags for different options when printing output.
     # TODO PRINT_SPACES and TOKENIZE do not mesh well together. What to do?
     NO_FLAGS = 0
     SHOW_SPACES = 1
     PRINT_SPACES = SHOW_SPACES
     SHOW_FLAGS = 2
     PRINT_FLAGS = SHOW_FLAGS
-    TOKENIZE = 4
+    DONT_OBEY_FLAGS = 4
+    TOKENIZE = 8
     VERBOSE = TOKENIZE | PRINT_FLAGS
 
     #region Class and Static Methods
     @classmethod
     def define(cls, definition, name):
         '''Defines an FSM constant; can be supplied regex or existing FSM.
         This link explains the Xerox regex formalism:
@@ -179,14 +181,17 @@
             foma_apply_set_space_symbol(c_void_p(applyer_handle), c_char_p(Fst._TOKENIZE_SYMBOL))
 
         if flags & Fst.PRINT_FLAGS:
             foma_apply_set_show_flags(c_void_p(applyer_handle), c_bool(True))
 
         if flags & Fst.PRINT_SPACES:
             foma_apply_set_print_space(c_void_p(applyer_handle), c_bool(True))
+
+        if flags & Fst.DONT_OBEY_FLAGS:
+            foma_apply_set_obey_flags(c_void_p(applyer_handle),  c_bool(False))
         
         return applyer_handle
 
     def _apply(self, apply_strategy, word=None, flags=NO_FLAGS):
         '''Takes an application function and executes it on the FST.'''
         if not self.fst_handle:
             raise ValueError('FST not defined')
@@ -256,26 +261,26 @@
     def upper_words(self, flags=NO_FLAGS):
         return self._apply(foma_apply_upper_words, flags=flags)
 
     def words(self, flags=NO_FLAGS):
         return self._apply(foma_apply_words, flags=flags)
         
     # FST operations.
-    def get_alphabet(self, minimize=True, flags=NO_FLAGS):
+    def get_alphabet(self, minimize=True, flags=SHOW_FLAGS | DONT_OBEY_FLAGS):
         '''Gets the alphabet of the FST.'''
         sigma = Fst()
         sigma.fst_handle = self._foma_call_unary(foma_fsm_sigma_net, minimize)
         return sigma.words(flags)
     
     # Alias to get_alphabet since both are very different yet valid names for the same function.
     get_sigma = get_alphabet
 
     def get_flag_diacritics(self, minimize=True):
         '''Returns a list of all the flag diacritics in the FST.'''
-        alphabet = ' '.join(self.get_alphabet(minimize, flags=Fst.SHOW_FLAGS))
+        alphabet = ' '.join(self.get_alphabet(minimize, flags=Fst.SHOW_FLAGS | Fst.DONT_OBEY_FLAGS))
         flag_diacritics = [match.groupdict()[MATCH_NAME] for match in FLAGS_REGEX.finditer(alphabet)]
         return flag_diacritics
 
     def union(self, other, minimize=True):
         '''Returns the union of two FSTs.'''
         fst = Fst()
         fst.fst_handle = self._foma_call_binary(other, foma_fsm_union, minimize)
@@ -468,10 +473,10 @@
         if debug:
             print(f'Query: {query}')
 
         selector_fst = Fst(query)
 
         # Apply query to fst and return generator of the analyses.
         resulting_fst = selector_fst.compose(self)
-        return zip(resulting_fst.upper_words(), resulting_fst.lower_words())
+        return resulting_fst.upper_words(), resulting_fst.lower_words()
 
     #endregion
```

### Comparing `foma_bindings-0.1.8/foma_bindings/mtfst/__init__.py` & `foma_bindings-0.1.9/foma_bindings/mtfst/__init__.py`

 * *Files identical despite different names*

### Comparing `foma_bindings-0.1.8/foma_bindings.egg-info/PKG-INFO` & `foma_bindings-0.1.9/foma_bindings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foma-bindings
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python bindings for the foma finite-state technology suite
 Home-page: https://github.com/CultureFoundryCA/foma_bindings
 Author: CultureFoundry
 Author-email: info@culturefoundrystudios.com
 License: Apache 2.0
 Keywords: foma,xfst,hfst,fst,fsm,mtfst,mtfsm
 Platform: UNKNOWN
```

### Comparing `foma_bindings-0.1.8/setup.py` & `foma_bindings-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 from setuptools import setup, find_packages
 
 setup(
     name='foma_bindings',
-    version='0.1.8',
+    version='0.1.9',
     description='Python bindings for the foma finite-state technology suite',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/CultureFoundryCA/foma_bindings',
     author='CultureFoundry',
     author_email='info@culturefoundrystudios.com',
     license='Apache 2.0',
```

