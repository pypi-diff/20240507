# Comparing `tmp/tllab_common-2024.4.3.tar.gz` & `tmp/tllab_common-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tllab_common-2024.4.3.tar", max compression
+gzip compressed data, was "tllab_common-2024.5.0.tar", max compression
```

## Comparing `tllab_common-2024.4.3.tar` & `tllab_common-2024.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2024.4.3/LICENSE
--rw-r--r--   0        0        0      706 2023-08-24 13:53:49.878008 tllab_common-2024.4.3/README.md
--rw-r--r--   0        0        0      970 2024-04-24 15:35:40.347543 tllab_common-2024.4.3/pyproject.toml
--rw-r--r--   0        0        0      462 2024-02-27 12:16:59.090201 tllab_common-2024.4.3/tllab_common/__init__.py
--rwxr-xr-x   0        0        0     9595 2024-03-26 10:33:49.874564 tllab_common-2024.4.3/tllab_common/findcells.py
--rw-r--r--   0        0        0    11888 2024-04-23 15:33:24.285649 tllab_common-2024.4.3/tllab_common/fit.py
--rw-r--r--   0        0        0     7944 2024-04-11 14:21:45.280730 tllab_common-2024.4.3/tllab_common/io.py
--rw-r--r--   0        0        0    19686 2024-04-22 15:46:32.391104 tllab_common-2024.4.3/tllab_common/misc.py
--rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 tllab_common-2024.4.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2024.5.0/LICENSE
+-rw-r--r--   0        0        0      706 2023-08-24 13:53:49.878008 tllab_common-2024.5.0/README.md
+-rw-r--r--   0        0        0      970 2024-05-07 08:46:53.232445 tllab_common-2024.5.0/pyproject.toml
+-rw-r--r--   0        0        0      462 2024-02-27 12:16:59.090201 tllab_common-2024.5.0/tllab_common/__init__.py
+-rwxr-xr-x   0        0        0     9595 2024-04-26 14:06:02.366979 tllab_common-2024.5.0/tllab_common/findcells.py
+-rw-r--r--   0        0        0    11898 2024-04-25 15:27:14.428669 tllab_common-2024.5.0/tllab_common/fit.py
+-rw-r--r--   0        0        0     8394 2024-04-30 15:37:00.023778 tllab_common-2024.5.0/tllab_common/io.py
+-rw-r--r--   0        0        0    19925 2024-05-07 08:47:12.268517 tllab_common-2024.5.0/tllab_common/misc.py
+-rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 tllab_common-2024.5.0/PKG-INFO
```

### Comparing `tllab_common-2024.4.3/LICENSE` & `tllab_common-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tllab_common-2024.4.3/README.md` & `tllab_common-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tllab_common-2024.4.3/pyproject.toml` & `tllab_common-2024.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tllab_common"
-version = "2024.4.3"
+version = "2024.5.0"
 description = "Common code for the Lenstra lab."
 authors = ["Lenstra lab NKI <t.lenstra@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["burst", "transcription"]
 include = ["transform.txt"]
 repository = "https://github.com/Lenstralab/tllab_common"
```

### Comparing `tllab_common-2024.4.3/tllab_common/findcells.py` & `tllab_common-2024.5.0/tllab_common/findcells.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2024.4.3/tllab_common/fit.py` & `tllab_common-2024.5.0/tllab_common/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         df = np.sqrt(np.sum((self.dfun(self.p, x).T * self.p_ci95).T ** 2, 0))
         return x.real, f - df, f + df
 
     def get_cost_fun(self) -> Callable[[ArrayLike], float]:
         s = self.s if self.fit_s else 1
         if self.log_scale:
             def cost(p: ArrayLike) -> float:
-                return np.nansum(np.abs(self.w / s * np.log(self.y / self.fun(p, self.x)) ** 2))
+                return np.nansum(np.abs(self.w / s * (np.log(self.y) - np.log(self.fun(p, self.x))) ** 2))
         else:
             def cost(p: ArrayLike) -> float:
                 return np.nansum(np.abs(self.w / s * (self.y - self.fun(p, self.x)) ** 2))
         return cost
 
     def fit(self) -> Fit:
         _ = self.r
```

### Comparing `tllab_common-2024.4.3/tllab_common/io.py` & `tllab_common-2024.5.0/tllab_common/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pickle
 from contextlib import ExitStack
 from functools import wraps
 from io import BytesIO
 from pathlib import Path
+from re import sub
 from typing import IO, Any, Callable, Hashable, Iterator, Optional, Sequence, Type
 
 import dill
 import pandas
 import roifile
 from bidict import bidict
 from ruamel import yaml
@@ -112,16 +113,19 @@
 
 
 @wraps(yaml.load)
 def yaml_load(stream: [str, bytes, Path, IO]) -> Any:
     with ExitStack() as stack:
         y = yaml.YAML()
         y.Constructor = RoundTripConstructor
-        if isinstance(stream, (str, bytes, Path)):
-            stream = stack.enter_context(open(stream, 'r'))
+        try:
+            if isinstance(stream, (str, bytes, Path)):
+                stream = stack.enter_context(open(stream, 'r'))
+        except (FileNotFoundError, OSError):
+            pass
         return y.load(stream)
 
 
 @wraps(yaml.dump)
 def yaml_dump(data: Any, stream: Optional[IO] = None) -> Optional[str]:
     with ExitStack() as stack:
         y = yaml.YAML()
@@ -135,24 +139,31 @@
                required: Sequence[dict] = None) -> CommentedDefaultMap:
     """ Load parameters from a parameterfile and parameters missing from that from the templatefile. Raise an error when
         parameters in required are missing. Return a dictionary with the parameters.
     """
 
     from .misc import cprint
 
+    parameter_file = Path(parameter_file)
+
+    def yaml_load_and_format(file: Path) -> CommentedDefaultMap:
+        with open(file) as f:
+            return yaml_load(sub(r'{{\s*(.+)\s*}}', r'{\1}', f.read()).format(
+                name=parameter_file.stem, folder=str(parameter_file.parent), suffix=parameter_file.suffix))
+
     def more_params(parameters: dict, file: [str, Path]) -> None:
         """ recursively load more parameters from another file """
         file = Path(file)
         more_parameters_file = parameters['more_parameters'] or parameters['more_params'] or parameters['moreParams']
         if more_parameters_file is not None:
             more_parameters_file = Path(more_parameters_file)
             if not more_parameters_file.is_absolute():
                 more_parameters_file = Path(file).absolute().parent / more_parameters_file
             cprint(f'<Loading more parameters from <{more_parameters_file}:.b>:g>')
-            more_parameters = yaml_load(more_parameters_file)
+            more_parameters = yaml_load_and_format(more_parameters_file)
             more_params(more_parameters, file)
 
             def add_items(sub_params, item):
                 for k, v in item.items():
                     if k not in sub_params:
                         sub_params[k] = v
                     elif isinstance(v, dict):
@@ -175,15 +186,15 @@
                 if isinstance(p, dict):
                     for key, value in p.items():
                         check_required(parameters[key], value)
                 else:
                     if p not in parameters:
                         raise Exception(f'Parameter {p} not given in parameter file.')
 
-    params = yaml_load(parameter_file)
+    params = yaml_load_and_format(parameter_file)
     more_params(params, parameter_file)
     check_required(params, required)
 
     if template_file is not None:
         check_params(params, yaml_load(template_file))
     return params
```

### Comparing `tllab_common-2024.4.3/tllab_common/misc.py` & `tllab_common-2024.5.0/tllab_common/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import pickle
 import re
 import sys
+import warnings
 from abc import ABCMeta
 from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
+from functools import wraps
 from glob import glob
-from inspect import signature, Parameter
+from inspect import Parameter, signature
 from pathlib import Path
 from traceback import format_exc, print_exception
 from typing import Any, Callable, Hashable, Sequence, TypeVar
 
+import makefun
 import numpy as np
 import pandas
 import regex
 from IPython import embed
-from makefun import wraps
 from ruamel import yaml
 
 from .io import get_params, pickle_dump, yaml_load
 
 Number = int | float | complex
 
 
@@ -163,14 +165,19 @@
         text and color format in <> is separated using : and text color, decoration and background color are separated
         using . or any character not a letter, digit or :
         colors: 'krgybmcw' (darker if capitalized) or terminal color codes (int up to 255)
         decorations: b: bold, u: underlined, r: swap color with background color """
     print(*(cfmt(arg) for arg in args), **kwargs)
 
 
+@wraps(warnings.warn)
+def warn(message: str, category: type = None, stacklevel: int = 1, source: Any = None) -> None:
+    warnings.warn(cfmt(f'<{message}:208>'), category, stacklevel + 1, source)
+
+
 def format_list(string: str, lst: Sequence, fmt: str = None) -> str:
     """ format a list in a grammatically correct way
         example: format_list('in {channel|channels}: {}', (1, 2, 5))
             'in channels: 1, 2 and 5'
     """
     if fmt is None:
         fmt = ''
@@ -529,15 +536,15 @@
         elif wrapped.__doc__:
             doc = wrapped.__doc__
         elif wrapper.__doc__:
             doc = wrapper.__doc__
         else:
             doc = None
 
-        @wraps(wrapped, new_sig=sig_wrapper.replace(parameters=new_parameters), doc=doc)
+        @makefun.wraps(wrapped, new_sig=sig_wrapper.replace(parameters=new_parameters), doc=doc)
         def fun(*args: Any, **kwargs: Any) -> R:
             return wrapped(*args, **kwargs)
 
         return fun
 
     return wrap  # type: ignore
```

### Comparing `tllab_common-2024.4.3/PKG-INFO` & `tllab_common-2024.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tllab_common
-Version: 2024.4.3
+Version: 2024.5.0
 Summary: Common code for the Lenstra lab.
 Home-page: https://github.com/Lenstralab/tllab_common
 License: GPLv3
 Keywords: burst,transcription
 Author: Lenstra lab NKI
 Author-email: t.lenstra@nki.nl
 Requires-Python: >=3.10,<4.0
```

