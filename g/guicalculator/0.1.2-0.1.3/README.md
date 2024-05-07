# Comparing `tmp/guicalculator-0.1.2.tar.gz` & `tmp/guicalculator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guicalculator-0.1.2.tar", max compression
+gzip compressed data, was "guicalculator-0.1.3.tar", max compression
```

## Comparing `guicalculator-0.1.2.tar` & `guicalculator-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,61 @@
--rw-r--r--   0        0        0     1093 2024-04-17 17:58:02.039277 guicalculator-0.1.2/LICENSE
--rw-r--r--   0        0        0      695 2024-04-23 12:08:32.555663 guicalculator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      619 2024-04-18 13:49:29.244697 guicalculator-0.1.2/README.md
--rw-r--r--   0        0        0     1229 2024-04-23 11:23:56.017110 guicalculator-0.1.2/src/guicalculator/__init__.py
--rw-r--r--   0        0        0     1365 2024-04-23 11:24:19.849845 guicalculator-0.1.2/src/guicalculator/__main__.py
--rw-r--r--   0        0        0     7854 2024-04-23 11:21:52.638136 guicalculator-0.1.2/src/guicalculator/buttoncfg.py
--rw-r--r--   0        0        0     1797 2024-04-23 11:23:58.373463 guicalculator-0.1.2/src/guicalculator/globals.py
--rw-r--r--   0        0        0    44051 2024-04-23 11:32:23.420997 guicalculator-0.1.2/src/guicalculator/guicalculator.py
--rw-r--r--   0        0        0     8983 2024-04-23 11:23:25.196817 guicalculator-0.1.2/src/guicalculator/supportfuncs.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 guicalculator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-17 17:58:02.039277 guicalculator-0.1.3/LICENSE
+-rw-r--r--   0        0        0      695 2024-05-07 11:30:01.440029 guicalculator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      619 2024-04-18 13:49:29.244697 guicalculator-0.1.3/README.md
+-rw-r--r--   0        0        0     1706 2024-05-04 11:26:42.726267 guicalculator-0.1.3/src/guicalculator/__init__.py
+-rw-r--r--   0        0        0     4542 2024-05-03 16:46:58.467709 guicalculator-0.1.3/src/guicalculator/__main__.py
+-rw-r--r--   0        0        0     6611 2024-05-06 13:38:55.229178 guicalculator-0.1.3/src/guicalculator/buttoncfg.py
+-rw-r--r--   0        0        0     2579 2024-05-06 15:44:40.948953 guicalculator-0.1.3/src/guicalculator/calculator/__init__.py
+-rw-r--r--   0        0        0     1968 2024-05-06 15:55:39.485534 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/__init__.py
+-rw-r--r--   0        0        0     2200 2024-05-06 15:47:21.706289 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/calculatordata.py
+-rw-r--r--   0        0        0     1907 2024-05-06 15:57:21.743332 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/functions/__init__.py
+-rw-r--r--   0        0        0     2621 2024-05-06 15:49:51.459829 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/functions/displaycalc.py
+-rw-r--r--   0        0        0     2949 2024-05-06 15:50:31.818854 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/functions/evalcalc.py
+-rw-r--r--   0        0        0     1660 2024-05-06 19:35:38.629695 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/functions/getuservar.py
+-rw-r--r--   0        0        0     4157 2024-05-06 15:52:33.046615 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/functions/processbutton.py
+-rw-r--r--   0        0        0     1844 2024-05-06 19:35:21.859254 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/functions/setuservar.py
+-rw-r--r--   0        0        0     2485 2024-05-06 16:37:27.044155 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/__init__.py
+-rw-r--r--   0        0        0     2879 2024-05-06 19:36:45.201894 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/backspace.py
+-rw-r--r--   0        0        0     3276 2024-05-06 19:37:21.652769 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/buttonpress.py
+-rw-r--r--   0        0        0     3088 2024-05-06 19:38:40.899141 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/calculate.py
+-rw-r--r--   0        0        0     1571 2024-05-06 19:39:11.950467 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/clearall.py
+-rw-r--r--   0        0        0     1571 2024-05-06 19:39:34.343819 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/clearvalue.py
+-rw-r--r--   0        0        0     1709 2024-05-06 19:40:05.344073 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/getcurinpt.py
+-rw-r--r--   0        0        0     1738 2024-05-06 19:40:33.744486 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/getmem.py
+-rw-r--r--   0        0        0     4424 2024-05-06 19:41:42.744969 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/getnumfncsym.py
+-rw-r--r--   0        0        0     2397 2024-05-06 19:42:34.657791 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/getuservarnames.py
+-rw-r--r--   0        0        0     1835 2024-05-06 19:43:09.698608 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/invnum.py
+-rw-r--r--   0        0        0     2368 2024-05-06 19:43:33.002300 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/memadd.py
+-rw-r--r--   0        0        0     1390 2024-05-06 19:43:51.013685 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/memclear.py
+-rw-r--r--   0        0        0     1667 2024-05-06 19:44:12.007336 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/memrecall.py
+-rw-r--r--   0        0        0     1801 2024-05-06 19:44:33.118391 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/memstore.py
+-rw-r--r--   0        0        0     2306 2024-05-06 19:44:53.165882 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/memswap.py
+-rw-r--r--   0        0        0     1832 2024-05-06 19:45:11.854274 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/negate.py
+-rw-r--r--   0        0        0     1827 2024-05-06 19:45:42.053121 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/rootnum.py
+-rw-r--r--   0        0        0     1817 2024-05-06 19:45:57.682935 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/squarenum.py
+-rw-r--r--   0        0        0     5206 2024-05-06 19:46:41.379701 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/types.py
+-rw-r--r--   0        0        0     3862 2024-05-06 19:48:08.274363 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/updatecalc.py
+-rw-r--r--   0        0        0     2908 2024-05-06 19:48:37.972682 guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/validatesymfunc.py
+-rw-r--r--   0        0        0     6617 2024-05-03 19:33:19.627392 guicalculator-0.1.3/src/guicalculator/calculator/evaluate_calculation.py
+-rw-r--r--   0        0        0     5357 2024-05-01 19:03:27.531506 guicalculator-0.1.3/src/guicalculator/calculator/logwrapper.py
+-rw-r--r--   0        0        0     3016 2024-05-01 19:03:36.217709 guicalculator-0.1.3/src/guicalculator/calculator/numtostr.py
+-rw-r--r--   0        0        0     1713 2024-05-01 19:03:42.961460 guicalculator-0.1.3/src/guicalculator/calculator/strtodecimal.py
+-rw-r--r--   0        0        0     2864 2024-05-01 19:03:53.034348 guicalculator-0.1.3/src/guicalculator/calculator/validate_user_var.py
+-rw-r--r--   0        0        0     2059 2024-05-01 16:06:04.372655 guicalculator-0.1.3/src/guicalculator/globals/__init__.py
+-rw-r--r--   0        0        0     2749 2024-05-06 14:14:29.973995 guicalculator-0.1.3/src/guicalculator/globals/buttoninfo.py
+-rw-r--r--   0        0        0     1735 2024-04-27 17:18:30.573906 guicalculator-0.1.3/src/guicalculator/globals/constants.py
+-rw-r--r--   0        0        0     4844 2024-05-06 13:38:55.001417 guicalculator-0.1.3/src/guicalculator/globals/enums.py
+-rw-r--r--   0        0        0     1409 2024-05-06 14:14:52.096130 guicalculator-0.1.3/src/guicalculator/globals/functionstype.py
+-rw-r--r--   0        0        0     2159 2024-04-27 17:18:29.213341 guicalculator-0.1.3/src/guicalculator/globals/types.py
+-rw-r--r--   0        0        0     2413 2024-04-28 15:43:22.930029 guicalculator-0.1.3/src/guicalculator/gui/__init__.py
+-rw-r--r--   0        0        0     4870 2024-05-06 12:56:06.159984 guicalculator-0.1.3/src/guicalculator/gui/btndispfrm.py
+-rw-r--r--   0        0        0     5064 2024-05-06 12:55:05.600813 guicalculator-0.1.3/src/guicalculator/gui/calcfrm.py
+-rw-r--r--   0        0        0     1935 2024-04-27 15:56:34.841712 guicalculator-0.1.3/src/guicalculator/gui/calcstyle.py
+-rw-r--r--   0        0        0     2319 2024-05-03 16:49:53.887570 guicalculator-0.1.3/src/guicalculator/gui/guicalculator.py
+-rw-r--r--   0        0        0     1815 2024-05-06 14:19:14.843498 guicalculator-0.1.3/src/guicalculator/gui/memdispfrm.py
+-rw-r--r--   0        0        0    15249 2024-05-06 12:57:46.224751 guicalculator-0.1.3/src/guicalculator/gui/uservarseditfrm.py
+-rw-r--r--   0        0        0     2119 2024-04-27 17:37:25.025536 guicalculator-0.1.3/src/guicalculator/gui/uservarseditpopup.py
+-rw-r--r--   0        0        0     2629 2024-05-06 14:15:18.776883 guicalculator-0.1.3/src/guicalculator/gui/varspopup.py
+-rw-r--r--   0        0        0     3812 2024-05-06 12:58:37.629653 guicalculator-0.1.3/src/guicalculator/gui/varspopuptreefrm.py
+-rw-r--r--   0        0        0     4125 2024-05-06 14:15:33.717053 guicalculator-0.1.3/src/guicalculator/gui/varspopuptreefrmbuttons.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:31:19.889488 guicalculator-0.1.3/src/guicalculator/py.typed
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 guicalculator-0.1.3/PKG-INFO
```

### Comparing `guicalculator-0.1.2/LICENSE` & `guicalculator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `guicalculator-0.1.2/pyproject.toml` & `guicalculator-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "guicalculator"
-version = "0.1.2"
+version = "0.1.3"
 license = "MIT"
 description = "A calculator written with python and tkinter"
 authors = ["Thomas Brotherton <tombroth@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/tombroth/guicalculator"
 classifiers = [
     "Programming Language :: Python :: 3.12",
```

### Comparing `guicalculator-0.1.2/README.md` & `guicalculator-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `guicalculator-0.1.2/src/guicalculator/__init__.py` & `guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/memclear.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
-guicalculator - A calculator written with python and tkinter
+memclear.py - The memory_clear function.
+"""
 
+"""
 Copyright (c) 2024 Thomas Brotherton
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
@@ -18,10 +20,16 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__all__ = ["GuiCalculator"]
+from ...logwrapper import object_wrapper
+from ..calculatordata import CalculatorData
+
+
+@object_wrapper
+def memory_clear(self: CalculatorData) -> None:
+    """memory_clear - Clear the value stored in memory"""
 
-from .guicalculator import GuiCalculator
+    self._memval.set("")
```

### Comparing `guicalculator-0.1.2/src/guicalculator/__main__.py` & `guicalculator-0.1.3/src/guicalculator/calculator/calculatordata/private/clearall.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-""""
-__main__.py - To make the module executable.
+"""
+clearall.py - The clear_all function.
+"""
 
+"""
 Copyright (c) 2024 Thomas Brotherton
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
@@ -18,18 +20,24 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-from guicalculator import GuiCalculator
+from ...logwrapper import object_wrapper
+from ..calculatordata import CalculatorData
+
 
+@object_wrapper
+def clear_all(self: CalculatorData) -> None:
+    """
+    clear_all - Clear the current number being input, the current
+    calculation, and the display. Does not clear the value in memory.
+    """
 
-# poetry build system seems to run better having a target function to run
-def main():
-    app = GuiCalculator()
-    app.mainloop()
+    self.clear_display()
 
+    self._current_calc = []
+    self._current_input = ""
 
-if __name__ == "__main__":
-    main()
+    self.update_display()
```

### Comparing `guicalculator-0.1.2/src/guicalculator/globals.py` & `guicalculator-0.1.3/src/guicalculator/globals/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
-globals.py - Variables needed by more than one module.
+constants.py - Constants needed by more than one module.
+"""
 
+"""
 Copyright (c) 2024 Thomas Brotherton
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
@@ -19,25 +21,24 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from decimal import Decimal
-from typing import NewType
 from unicodedata import normalize
 
-PI = "\u03c0"
+from .types import VariablesType
 
+PI = "\u03c0"
 
-VariablesType = NewType("VariablesType", dict[str, Decimal])
-"""Type to store varaibles and values for the parser: dict[str, Decimal]"""
+NORMALIZE_FORM = "NFKC"  # for unicode comparison
 
 # stores default variables pi and e
 # including first 30 digits because default precision is 28 in Decimal
 # hard coding instead of using math.pi due to float to Decimal rounding issues
 DEFAULT_VARIABLES: VariablesType = VariablesType(
     {
-        normalize("NFKC", PI): Decimal("3.141592653589793238462643383279"),
+        normalize(NORMALIZE_FORM, PI): Decimal("3.141592653589793238462643383279"),
         "e": Decimal("2.718281828459045235360287471352"),
     }
 )
```

### Comparing `guicalculator-0.1.2/src/guicalculator/supportfuncs.py` & `guicalculator-0.1.3/src/guicalculator/calculator/evaluate_calculation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
-supportfuncs.py - Support functions needed by guicalculator. These functions do 
-not depend on the calculator interface or data, other than data passed in to and
-back from the function.
+evaluate_calculation.py - Evaluate the provided calculation, returning the
+    result as Decimal. This is  the parser.
+"""
 
+"""
 Copyright (c) 2024 Thomas Brotherton
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
@@ -21,115 +22,36 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import ast
-import keyword
 import operator
 from decimal import Decimal
-from typing import Callable, Type
+from typing import Any, Callable, Type
 from unicodedata import normalize
 
-from .globals import DEFAULT_VARIABLES, VariablesType
+from ..globals import DEFAULT_VARIABLES, NORMALIZE_FORM, VariablesType
+from .logwrapper import plain_wrapper
+from .validate_user_var import validate_user_vars
 
 # map of ast operators to functions used by parser
 OPERATOR_MAP: dict[Type[ast.AST], Callable] = {
     ast.Div: operator.truediv,
     ast.Mult: operator.mul,
     ast.Sub: operator.sub,
     ast.Add: operator.add,
     ast.USub: operator.neg,
     ast.UAdd: operator.pos,
     ast.Pow: operator.pow,
 }
 
 
-def numtostr(
-    val: int | float | Decimal,
-    commas: bool = False,
-    removeZeroes: bool = True,
-) -> str:
-    """
-    numtostr - Convert number to string.
-
-    Converts an int or float or Decimal to a string representation. Can
-    add thousand separators and/or remove trailing zeroes after a decimal
-    point.
-
-    Notes
-    -----
-    As a side effect, will round the number currently being input to the
-    precision in the Decimal context if removeZeroes is True.
-
-    Parameters
-    ----------
-    val : int | float | Decimal
-        Number to be converted
-    commas : bool, optional
-        True means add thosands separators (commas). By default False.
-    removeZeroes : bool, optional
-        True means remove trailing zeroes after the decimal point.
-        By default True.
-
-    Returns
-    -------
-    str
-        The string representation of the number
-    """
-    v: int | float | Decimal
-    if commas:
-        c = ","
-    else:
-        c = ""
-
-    if isinstance(val, Decimal):
-        if val == val.to_integral_value() and removeZeroes:
-            v = val.to_integral_value()
-        else:
-            if removeZeroes:
-                v = (
-                    val.quantize(Decimal(1))
-                    if val == val.to_integral()
-                    else val.normalize()
-                )
-            else:
-                v = val
-        fmt = "{0:" + c + "f}"
-    elif val == int(val) and removeZeroes:
-        v = int(val)
-        fmt = "{0:" + c + "d}"
-    else:
-        v = val
-        fmt = "{0:" + c + ".28g}"
-
-    return fmt.format(v)
-
-
-def strtodecimal(val: str) -> Decimal:
-    """
-    strtodecimal  - convert string value to Decimal.
-
-    Parameters
-    ----------
-    val : str
-        Value to be converted
-
-    Returns
-    -------
-    Decimal
-        Converted value
-    """
-    if val:
-        return Decimal(val.replace(",", ""))
-    else:
-        return Decimal(0)
-
-
+@plain_wrapper
 def evaluate_calculation(
     current_calculation: str, user_variables: VariablesType
 ) -> Decimal:
     """
     evaluate_calculation - Evaluate the provided calculation, returning the
     result as Decimal.
 
@@ -148,120 +70,121 @@
     Raises
     ------
     TypeError
         Used for custom errors, message indicates what the specific error was.
 
     """
 
-    # validate that nothing improper is in user_variables
-    # we should be able to trust DEFAULT_VARIABLES
-    for nam, val in user_variables.items():
-        if (
-            not nam
-            or type(nam) != str
-            or not nam.isidentifier()
-            or keyword.iskeyword(nam)
-        ):
-            raise TypeError("Invalid variable name {nam!r}")
-        if nam in DEFAULT_VARIABLES.keys():
-            raise TypeError("Attempt to overwrite default variable {nam!r}")
-        if not val or type(val) != Decimal:
-            raise TypeError("Invalid value for variable {nam!r}: {val!r}")
-
-    # validate we actually have a str in current_calculation
-    if not current_calculation or type(current_calculation) != str:
-        raise TypeError("Invalid calculation")
-
-    root_node = ast.parse(current_calculation, mode="eval")
-
     # internal function, nested so it can't be called directly
-    # unnesting would require moving above validation inside the function
+    #
+    # unnesting would remove the validation done in the outer procedure
     def _eval(node: ast.AST) -> Decimal:
         """_eval - Internal recursive function to evaluate the ast nodes"""
 
         # used in multiple error messages
-        node_fmtd = ast.dump(node, indent=2)
+        node_fmtd = ast.dump(node, annotate_fields=False)
 
         match node:
             case ast.Expression():
                 return _eval(node.body)
 
             # replaced with Decimal numbers, left in just in case
             case ast.Constant():
                 if isinstance(node.value, (int, float)):
                     return +Decimal(node.value)
                 else:
-                    raise TypeError(f"Unknown constant: ast.{node_fmtd}")
+                    raise TypeError(f"Unknown constant {node_fmtd}")
 
             case ast.BinOp():
                 left, right, op = node.left, node.right, node.op
                 method = OPERATOR_MAP[type(op)]
                 return method(_eval(left), _eval(right))
 
             case ast.UnaryOp():
                 operand, uop = node.operand, node.op
                 method = OPERATOR_MAP[type(uop)]
                 return method(_eval(operand))
 
             case ast.Name():
-                if normalize("NFKC", node.id) in DEFAULT_VARIABLES:
-                    return +DEFAULT_VARIABLES[normalize("NFKC", node.id)]
 
-                elif normalize("NFKC", node.id) in user_variables:
-                    return +user_variables[normalize("NFKC", node.id)]
+                if normalize(NORMALIZE_FORM, node.id) in DEFAULT_VARIABLES:
+                    return +DEFAULT_VARIABLES[normalize(NORMALIZE_FORM, node.id)]
+
+                elif normalize(NORMALIZE_FORM, node.id) in user_variables:
+                    return +user_variables[normalize(NORMALIZE_FORM, node.id)]
 
                 else:
                     node_escpd = node.id.encode("unicode_escape")
-                    raise TypeError(f"Unknown variable: {node_escpd!r}")
+                    raise TypeError(f"Unknown variable {node_escpd!r}")
 
             case ast.Call():
                 pkg, func = _get_caller(node, node_fmtd)
 
                 # if I ever allow more function calls, will have to make another dict
                 if (pkg, func) in (("decimal", "Decimal"), ("", "Decimal")):
                     parm = _get_str_parameter(node)
                     return +Decimal(parm)
-                elif (pkg, func) == ("Decimal", "sqrt"):
 
+                elif (pkg, func) == ("Decimal", "sqrt"):
                     return Decimal.sqrt(_eval(node.args[0]))
+
                 else:
-                    raise TypeError(
-                        f"Unknown function call: {pkg}.{func}: \nast.{node_fmtd}"
-                    )
+                    raise TypeError(f"Unknown function call {pkg}.{func}: {node_fmtd}")
 
             case _:
-                raise TypeError(f"Unknown ast node: \nast.{node_fmtd}")
+                raise TypeError(f"Unknown ast node: {node_fmtd}")
 
-    def _get_str_parameter(node):
-        """_get_str_parameter - Internal function to return a single str parameter"""
+    # back to the outer function
+    #
+    # validate that nothing improper is in user_variables
+    # we should be able to trust DEFAULT_VARIABLES
+    validate_user_vars(user_variables)
 
-        if len(node.args) == 1 and isinstance(node.args[0], ast.Constant):
-            parm = node.args[0].value
-        else:
-            raise TypeError("Decimal function accepts exactly one argument")
-        if type(parm) == str:
-            return parm
-        else:
-            raise TypeError("Decimal function should only have str parameter")
-
-    def _get_caller(node, node_fmtd):
-        """_get_caller - Internal function to get calling module/function name"""
-
-        if isinstance(node.func, ast.Attribute):  # package.procedure
-            if isinstance(node.func.value, ast.Name):
-                pkg = node.func.value.id
-                func = node.func.attr
-            else:  # ??? not sure if this can happen
-                errmsg = f"Unknown type of ast.Call: \nast.{node_fmtd}"
-                raise TypeError(errmsg)
-
-        elif isinstance(node.func, ast.Name):  # procedure
-            pkg = ""
-            func = node.func.id
+    # validate we actually have a str in current_calculation
+    if not current_calculation or type(current_calculation) != str:
+        raise TypeError("Invalid calculation")
 
-        else:  # ??? not sure if this can happen
-            errmsg = f"Unknown type of ast.Call: \nast.{node_fmtd}"
-            raise TypeError(errmsg)
-        return pkg, func
+    root_node = ast.parse(current_calculation, mode="eval")
 
     val = _eval(root_node)
     return val
+
+
+@plain_wrapper
+def _get_str_parameter(node: ast.Call) -> str:
+    """
+    _get_str_parameter - Internal function to return a single str
+    parameter of an ast Call.
+    """
+
+    if len(node.args) == 1 and isinstance(node.args[0], ast.Constant):
+        parm = node.args[0].value
+    else:
+        raise TypeError("Decimal function accepts exactly one argument")
+    if type(parm) == str:
+        return parm
+    else:
+        raise TypeError("Decimal function should only have str parameter")
+
+
+@plain_wrapper
+def _get_caller(node: ast.Call, node_fmtd: str) -> tuple[Any, Any]:
+    """
+    _get_caller - Internal function to get calling module/function name.
+    """
+
+    if isinstance(node.func, ast.Attribute):  # package.procedure
+        if isinstance(node.func.value, ast.Name):
+            pkg = node.func.value.id
+            func = node.func.attr
+        else:  # ??? not sure if this can happen
+            errmsg = f"Unknown type of ast.Call: {node_fmtd}"
+            raise TypeError(errmsg)
+
+    elif isinstance(node.func, ast.Name):  # procedure
+        pkg = ""
+        func = node.func.id
+
+    else:  # ??? not sure if this can happen
+        errmsg = f"Unknown type of ast.Call: {node_fmtd}"
+        raise TypeError(errmsg)
+    return pkg, func
```

### Comparing `guicalculator-0.1.2/PKG-INFO` & `guicalculator-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guicalculator
-Version: 0.1.2
+Version: 0.1.3
 Summary: A calculator written with python and tkinter
 Home-page: https://github.com/tombroth/guicalculator
 License: MIT
 Author: Thomas Brotherton
 Author-email: tombroth@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

