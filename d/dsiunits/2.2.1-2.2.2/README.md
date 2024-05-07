# Comparing `tmp/dsiunits-2.2.1.tar.gz` & `tmp/dsiunits-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsiunits-2.2.1.tar", last modified: Thu Apr 25 09:23:20 2024, max compression
+gzip compressed data, was "dsiunits-2.2.2.tar", last modified: Tue May  7 13:06:51 2024, max compression
```

## Comparing `dsiunits-2.2.1.tar` & `dsiunits-2.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-25 09:23:20.400226 dsiunits-2.2.1/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    26516 2024-04-25 08:43:02.000000 dsiunits-2.2.1/LICENSE
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    33557 2024-04-25 09:23:20.400226 dsiunits-2.2.1/PKG-INFO
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)     2403 2024-04-25 09:18:30.000000 dsiunits-2.2.1/README.md
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      764 2024-04-25 09:22:26.000000 dsiunits-2.2.1/pyproject.toml
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      376 2024-04-25 09:23:20.401226 dsiunits-2.2.1/setup.cfg
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-25 09:23:20.400226 dsiunits-2.2.1/src/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)        0 2024-04-25 08:36:12.000000 dsiunits-2.2.1/src/__init__.py
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    39343 2024-04-25 08:46:51.000000 dsiunits-2.2.1/src/dsiUnits.py
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-25 09:23:20.400226 dsiunits-2.2.1/src/dsiunits.egg-info/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    33557 2024-04-25 09:23:20.000000 dsiunits-2.2.1/src/dsiunits.egg-info/PKG-INFO
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      241 2024-04-25 09:23:20.000000 dsiunits-2.2.1/src/dsiunits.egg-info/SOURCES.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)        1 2024-04-25 09:23:20.000000 dsiunits-2.2.1/src/dsiunits.egg-info/dependency_links.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)       18 2024-04-25 09:23:20.000000 dsiunits-2.2.1/src/dsiunits.egg-info/top_level.txt
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-04-25 09:23:20.400226 dsiunits-2.2.1/tests/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    17848 2024-04-25 08:46:51.000000 dsiunits-2.2.1/tests/test_dsiUnits.py
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-07 13:06:51.199603 dsiunits-2.2.2/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    26516 2024-04-25 08:43:02.000000 dsiunits-2.2.2/LICENSE
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    33557 2024-05-07 13:06:51.199603 dsiunits-2.2.2/PKG-INFO
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)     2403 2024-04-25 09:18:30.000000 dsiunits-2.2.2/README.md
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)      764 2024-05-07 13:06:33.000000 dsiunits-2.2.2/pyproject.toml
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)      376 2024-05-07 13:06:51.199603 dsiunits-2.2.2/setup.cfg
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-07 13:06:51.198603 dsiunits-2.2.2/src/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)        0 2024-04-25 08:36:12.000000 dsiunits-2.2.2/src/__init__.py
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    40343 2024-05-07 13:04:53.000000 dsiunits-2.2.2/src/dsiUnits.py
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-07 13:06:51.199603 dsiunits-2.2.2/src/dsiunits.egg-info/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    33557 2024-05-07 13:06:51.000000 dsiunits-2.2.2/src/dsiunits.egg-info/PKG-INFO
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)      241 2024-05-07 13:06:51.000000 dsiunits-2.2.2/src/dsiunits.egg-info/SOURCES.txt
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)        1 2024-05-07 13:06:51.000000 dsiunits-2.2.2/src/dsiunits.egg-info/dependency_links.txt
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)       18 2024-05-07 13:06:51.000000 dsiunits-2.2.2/src/dsiunits.egg-info/top_level.txt
+drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-07 13:06:51.198603 dsiunits-2.2.2/tests/
+-rw-r--r--   0 seeger01  (1000) seeger01  (1000)    18195 2024-05-07 13:04:53.000000 dsiunits-2.2.2/tests/test_dsiUnits.py
```

### Comparing `dsiunits-2.2.1/LICENSE` & `dsiunits-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsiunits-2.2.1/PKG-INFO` & `dsiunits-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsiunits
-Version: 2.2.1
+Version: 2.2.2
 Summary: This is a Python module for handling the SI units as objects in Python, parsing them from strings and converting them to Latex and Unicode, as well as performing math operations and calculating scale factors.
 Author-email: Benedikt Seeger <benedikt.seeger@ptb.de>, Vanessa Stehr <vanessa.stehr@ptb.de>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
```

### Comparing `dsiunits-2.2.1/README.md` & `dsiunits-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dsiunits-2.2.1/pyproject.toml` & `dsiunits-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dsiunits"  # Ensure this is correctly specified
-version = "2.2.1"
+version = "2.2.2"
 description = "This is a Python module for handling the SI units as objects in Python, parsing them from strings and converting them to Latex and Unicode, as well as performing math operations and calculating scale factors."
 authors = [
     { name="Benedikt Seeger", email="benedikt.seeger@ptb.de" },
     { name="Vanessa Stehr", email="vanessa.stehr@ptb.de" }
 ]
 license = { file="LICENSE" }
 readme = "README.md"
```

### Comparing `dsiunits-2.2.1/src/dsiUnits.py` & `dsiunits-2.2.2/src/dsiUnits.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
             items.pop(0)
         else:
             warningMessages.append(
                 _warn(f"string should start with \\, string given was «{dsiString}»", RuntimeWarning))
         nodes = []
 
         (prefix, unit, exponent) = ('', '', '')
+        valid=True
         item = items.pop(0)
         while True:
             if item in _dsiPrefixesLatex:
                 prefix = item
                 try:
                     item = items.pop(0)
                 except IndexError:
@@ -166,14 +167,15 @@
                     item = ''
             elif re.match(r'tothe\{.*\}', item):
                 exponent = item.split('{')[1].split('}')[0]
                 try:
                     floatCast = float(exponent)
                 except ValueError:
                     warningMessages.append(_warn(f"The exponent «{exponent}» is not a number!", RuntimeWarning))
+                    valid=False
                 try:
                     item = items.pop(0)
                 except IndexError:
                     item = ''
             if (prefix, unit, exponent) == ('', '', ''):
                 unit = item
                 try:
@@ -183,29 +185,32 @@
                 closestMatches = _getClosestStr(unit)
                 if len(closestMatches) > 0:
                     closestMatchesStr = ', \\'.join(closestMatches)
                     closestMatchesStr = '\\' + closestMatchesStr
                     warningMessages.append(_warn(
                         fr"The identifier «{unit}» does not match any D-SI units! Did you mean one of these «{closestMatchesStr}» ?",
                         RuntimeWarning))
+                    valid=False
                 else:
                     warningMessages.append(
                         _warn(fr"The identifier «{unit}» does not match any D-SI units!", RuntimeWarning))
+                    valid=False
             elif unit == '':
                 itemStr = ""
                 if prefix != "":
                     itemStr = itemStr + "\\" + prefix
                 if exponent != "":
                     itemStr = itemStr + r"\tothe{" + exponent + r"}"
                 warningMessages.append(
                     _warn(f"This D-SI unit seems to be missing the base unit! «{itemStr}»", RuntimeWarning))
-
-            nodes.append(_node(prefix, unit, exponent))
+                valid=False
+            nodes.append(_node(prefix, unit, exponent, valid=valid))
             if (len(items) == 0) and (item == ''): break
             (prefix, unit, exponent) = ('', '', '')
+            valid=True
         return (nodes, warningMessages)
 
     def info(self):
         infoStr = "D-SI Parser Version: " + str(self) + "using D-SI Schema Version: " + str(
             self.__dsiVersion) + "from: " + str(self.__dsiRepositoryURL) + "using D-SI Schema: " + str(
             self.__dsiSchemaUrl)
         print(infoStr)
@@ -315,18 +320,18 @@
             return ''.join(superscripts.get(char, char) for char in exp_str)
 
         utf8Array = []
         for fraction in self.tree:
             fractionUtf8Array = []
             for node in fraction:
                 # Fetch UTF-8 unit representation
-                unitStr = _dsiUnitsUTF8.get(node.unit, node.unit)
+                unitStr = _dsiUnitsUTF8.get(node.unit,'⚠'+node.unit+'⚠')#second arg is returend on itemError
 
                 # Handle prefix (if any) and unit
-                prefixStr = _dsiPrefixesUTF8.get(node.prefix, node.prefix) if node.prefix else ""
+                prefixStr = _dsiPrefixesUTF8.get(node.prefix, '⚠'+node.prefix+'⚠') if node.prefix else ""
                 utf8Str = f"{prefixStr}{unitStr}"  # Direct concatenation for compactness
 
                 # Handle exponent, converting to UTF-8 subscript, if not 1
                 if node.exponent and node.exponent != 1:
                     utf8Str += exponent_to_utf8(node.exponent)
 
                 fractionUtf8Array.append(utf8Str)
@@ -387,15 +392,15 @@
             consolidated_nodes = [node for node in self.tree[0]]
 
             # Copy nodes from the second fraction, adjusting the exponents
             for node in self.tree[1]:
                 # Inverting the exponent for nodes in the denominator
                 invertedExponent = -1 * node.exponent
                 fractionalScaleFactor = 1 / node.scaleFactor
-                consolidated_nodes.append(_node(node.prefix, node.unit, invertedExponent, fractionalScaleFactor))
+                consolidated_nodes.append(_node(node.prefix, node.unit, invertedExponent,  scaleFactor=fractionalScaleFactor))
 
         # Consolidating nodes with the same unit
         i = 0
         while i < len(consolidated_nodes):
             j = i + 1
             while j < len(consolidated_nodes):
                 if consolidated_nodes[i].unit == consolidated_nodes[j].unit:
@@ -521,15 +526,15 @@
             for node in self.tree[1]:
                 result += str(node)
         return result
 
     def __repr__(self):
         contentStr=self.toUTF8()
         if not self.valid:
-            contentStr+=' INVALIDE'
+            contentStr+='INVALIDE'
         if self.warnings:
             contentStr+=f" {len(self.warnings)} WARNINGS"
         # Simple representation: class name and D-SI string
         return f"{contentStr}"
 
 
     def __pow__(self, other):
@@ -560,17 +565,18 @@
     def __truediv__(self, other):
         return self * other**-1
 
 
 class _node:
     """one node of the D-SI tree, containing prefix, unit, power
     """
-    def __init__(self,    prefix: str,unit: str,exponent: float=1.0,scaleFactor: float = 1.0  ):# Adding scale factor with default value 1.0
+    def __init__(self, prefix: str,unit: str,exponent: float=1.0, valid:bool=True,scaleFactor: float = 1.0  ):# Adding scale factor with default value 1.0
         self.prefix=prefix
         self.unit=unit
+        self.valid=valid
         if isinstance(exponent,float) or isinstance(exponent,int):
             self.exponent=float(exponent)
         if isinstance(exponent,str):
             if exponent== '':
                 exponent= 1.0
             else:
                 try:
@@ -590,17 +596,21 @@
         latexString = ""
         if self.prefix:
             latexString += _dsiPrefixesLatex[self.prefix]
         try:
             latexString += _dsiUnitsLatex[self.unit]
         except KeyError:
             latexString += r'{\color{red}\mathrm{'+self.unit+r'}}'
+            if self.valid==True:
+                raise RuntimeError("Found invalid unit in valid node, this should not happen! Report this incident at: https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/issues/new")
         if isinstance(self.exponent,str):
             #exponet is str this souldnt happen!
             latexString += r'^{{\color{red}\mathrm{'+self.exponent+r'}}}'
+            if self.valid==True:
+                raise RuntimeError("Found invalid unit in valid node, this should not happen! Report this incident at: https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/issues/new")
         elif self.exponent != 1.0:
             if not self.exponent.is_integer():
                 if self.exponent == 0.5:
                     latexString = r'\sqrt{' + latexString + r'}'
                 else:
                     exponent_fraction = Fraction(self.exponent).limit_denominator()
                     if exponent_fraction.denominator == 1:
@@ -616,14 +626,16 @@
             else:
                 #TODO better formating
                 latexString += r'^{' + str(int(self.exponent)) + r'}'
 
         
         if self.unit == "":
             latexString = r'{\color{red}'+latexString+r'}'
+            if self.valid==True:
+                raise RuntimeError("Found invalid unit in valid node, this should not happen! Report this incident at: https://gitlab1.ptb.de/digitaldynamicmeasurement/dsiUnits/-/issues/new")
 
         return latexString
 
     def toBaseUnits(self, complete=False) -> List['_node']:
         """
         Converts this node to its base unit representation.
         Adjusts the scale factor during the conversion. Optionally resolves to kg, s, and m units,
@@ -642,28 +654,28 @@
         # Convert to base units if it's a derived unit
         if self.unit in _derivedToBaseUnits:
             baseUnitsInfo = _derivedToBaseUnits[self.unit]
             baseUnits = []
             for i, (baseUnit, exponent, scaleFactor) in enumerate(baseUnitsInfo):
                 # Apply the adjusted scale factor only to the first base unit
                 finalScaleFactor = math.pow(adjustedScaleFactor * scaleFactor, self.exponent) if i == 0 else 1.0
-                baseUnits.append(_node('', baseUnit, exponent * self.exponent, finalScaleFactor))
+                baseUnits.append(_node('', baseUnit, exponent * self.exponent, scaleFactor=finalScaleFactor))
             return baseUnits
         elif complete:
             # Additional logic for converting ampere, volt, and mole to kg, s, and m equivalents
             if self.unit in _additionalConversions:
                 kgsUnitsInfo = _additionalConversions[self.unit]
                 kgsUnits = []
                 for i, (kgsUnit, exponent, scaleFactor) in enumerate(kgsUnitsInfo):
                     finalScaleFactor = math.pow(adjustedScaleFactor * scaleFactor, self.exponent) if i == 0 else 1.0
-                    kgsUnits.append(_node('', kgsUnit, exponent * self.exponent, finalScaleFactor))
+                    kgsUnits.append(_node('', kgsUnit, exponent * self.exponent, scaleFactor=finalScaleFactor))
                 return kgsUnits
 
         # Return the node as is if it's already a base unit, with adjusted scale factor
-        return [_node('', self.unit, self.exponent, adjustedScaleFactor)]
+        return [_node('', self.unit, self.exponent,  scaleFactor=adjustedScaleFactor)]
 
     def __eq__(self, other):
         """Checks if two nodes are identical after sorting their nodes alphabetically."""
         return self.prefix == other.prefix and self.unit == other.unit and self.exponent == other.exponent and self.scaleFactor == other.scaleFactor
 
     def __str__(self):
         result=''
```

### Comparing `dsiunits-2.2.1/src/dsiunits.egg-info/PKG-INFO` & `dsiunits-2.2.2/src/dsiunits.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsiunits
-Version: 2.2.1
+Version: 2.2.2
 Summary: This is a Python module for handling the SI units as objects in Python, parsing them from strings and converting them to Latex and Unicode, as well as performing math operations and calculating scale factors.
 Author-email: Benedikt Seeger <benedikt.seeger@ptb.de>, Vanessa Stehr <vanessa.stehr@ptb.de>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
```

### Comparing `dsiunits-2.2.1/tests/test_dsiUnits.py` & `dsiunits-2.2.2/tests/test_dsiUnits.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     assert dsiUnit(r'\metre\tothe{0.3333333333333333333}').toLatex(wrapper='') == r'\mathrm{m}\sqrt[3]{\mathrm{m}}'
     assert dsiUnit(r'\metre\tothe{0.666666666666666}').toLatex(wrapper='') == r'\mathrm{m}\sqrt[3]{\mathrm{m}^{2}}'
 
 def test_baseUnitConversion():
     # Test conversion of a single derived unit to its base unit
     derivedUnitTree = dsiUnit(r'\kilo\metre')
     baseUnitTree = derivedUnitTree.toBaseUnitTree()
-    assert baseUnitTree.tree == [[_node('', 'metre', '', 1000)]]
+    assert baseUnitTree.tree == [[_node('', 'metre', '', scaleFactor=1000.0)]]
     assert baseUnitTree.toLatex() == '$$\\mathrm{m}$$'
 
     # Test conversion of a complex unit with a fraction to base units
     complexUnitTree = dsiUnit(r'\kilo\watt\hour')
     complexUnitTree2 = dsiUnit(r'\kilo\watt\hour')
     complexBaseUnitTree = complexUnitTree.toBaseUnitTree()
     reduceFractionTree = complexBaseUnitTree.reduceFraction()
@@ -292,14 +292,22 @@
     ]
 
     for unit_input, expected_output in units_of_power:
         dsiTree = dsiUnit(unit_input)
         utf8_output = dsiTree.toUTF8()
         assert utf8_output == expected_output, f"Expected {expected_output}, got {utf8_output}"
 
+
+def test_toUTF8WError():
+    unitStrWithError=r'\molli\metre'
+    with pytest.warns(RuntimeWarning, match=r'The identifier «molli» does not match any D-SI units! Did you mean one of these «\\milli, \\mole» ?'):
+        unitWError = dsiUnit(unitStrWithError)
+    utf8Str=unitWError.toUTF8()
+    assert utf8Str == '⚠molli⚠m'
+
 def test_fromAscii():
     test_cases = [
         # Compact form without spaces
         # Form using ^ for exponents
         ("A^2Ω", r"\ampere\tothe{2}\ohm"),
         # Handling fractions
         ("J/s", r"\joule\per\second"),
```

