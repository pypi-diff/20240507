# Comparing `tmp/wheelz_idp_validations-2.1.4.tar.gz` & `tmp/wheelz_idp_validations-2.2.0.tar.gz`

## Comparing `wheelz_idp_validations-2.1.4.tar` & `wheelz_idp_validations-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/LICESNSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/requirements.txt
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/__init__.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/id_sanitizer.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/pcv1_sanitizer.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/pcv2_sanitizer.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitize_exception.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/exceptions/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/exceptions/date_exceptions.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/exceptions/full_name_exceptions.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/exceptions/gender_exceptions.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/exceptions/id_exceptions.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/exceptions/plate_exceptions.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/exceptions/vin_exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/__init__.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/cif.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/date.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/full_name.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/gender.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/id_number.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/plate.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/vin.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/.gitignore
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/readme.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/LICESNSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/requirements.txt
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/__init__.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/id_sanitizer.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/pcv1_sanitizer.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/pcv2_sanitizer.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitize_exception.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/cif_exceptions.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/date_exceptions.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/full_name_exceptions.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/gender_exceptions.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/id_exceptions.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/plate_exceptions.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/vin_exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/cif.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/date.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/full_name.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/gender.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/id_number.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/plate.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/vin.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/.gitignore
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/readme.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 wheelz_idp_validations-2.2.0/PKG-INFO
```

### Comparing `wheelz_idp_validations-2.1.4/LICESNSE` & `wheelz_idp_validations-2.2.0/LICESNSE`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.1.4/.github/workflows/python-publish.yml` & `wheelz_idp_validations-2.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/id_sanitizer.py` & `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/id_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/pcv1_sanitizer.py` & `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/pcv1_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/exceptions/id_exceptions.py` & `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/exceptions/id_exceptions.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/cif.py` & `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/cif.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 import re
-#from ..exceptions.date_exceptions import *
-
+from ..exceptions.cif_exceptions import *
 
 # Cif algorithm documentation https://www.mapa.gob.es/app/materialvegetal/docs/CIF.pdf
 def sanitize_cif(received_cif):
-    cif_regexp_default = "([ABCDEFGHQSKLM])(\d{7})(\d)"
-    # CIF Letters P and X may be on the end
-    cif_regexp_special = "(\d)(\d{7})([PX])"
+    cif_regexp_default = r"([ABCDEFGHQSKLM])(\d{7})(\d)"
+    cif_regexp_special = r"(\d)(\d{7})([PX])"
     special = False
 
-    # Get only the CIF number (try first default CIF Format)
+    # Intentar extraer el CIF usando el formato estándar
     match = re.search(cif_regexp_default, received_cif)
 
-    # If there is no match, try second format, if failed, throw exception
+    # Si no hay coincidencia, intentar con el formato especial
     if not match:
         match = re.search(cif_regexp_special, received_cif)
         special = True
         if not match:
-            print('hola')
-            #raise NoCIFMatchFoundException(received_cif)
+            raise NoCIFMatchFoundException(received_cif)
 
-    # Replace O (letter) for 0 (number) in case of errors
-    # We store digits and letter because we will use it later to validate CIF
+    # Preparar los componentes del CIF para validación
     digits = match.group(2).replace('O', '0')
     if not special:
         letter = match.group(1)
-        processed_cif = letter + digits + match.group(3).replace('O', '0')
+        control_digit = match.group(3).replace('O', '0')
     else:
         letter = match.group(3)
-        processed_cif = match.group(1).replace('O', '0') + digits + letter
+        control_digit = match.group(1).replace('O', '0')
+
+    processed_cif = letter + digits + control_digit
 
-    # CIF Validation algorithm
-    # 1 - Add pair position digits from digits string to total_sum
-    # 2 - Multiply by two odd positions, then add their digits, finally add them to total+_sum
+    # Validar el CIF según el algoritmo especificado
     total_sum = 0
-    for pos in range(0, len(digits)):
-        # Pair digits are in positions 1,3,5...
-        if pos % 2:
-            total_sum += int(digits[pos])
-        # Odd digits are in position 0,2,4...
+    for pos in range(len(digits)):
+        num = int(digits[pos])
+        if pos % 2 == 0:
+            total_sum += sum(int(x) for x in str(num * 2))
         else:
-            total_sum += sum(int(digit) for digit in str(digits[pos] * 2))
-
-    print(total_sum)
+            total_sum += num
 
+    # Calcular el dígito de control esperado
+    check_digit = str((10 - (total_sum % 10)) % 10)
+    if (check_digit != control_digit and not (control_digit == 'P' and check_digit == '0')):
+        raise InvalidCIFException(processed_cif)
 
-sanitize_cif("A58818501")
+    return processed_cif
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/date.py` & `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/date.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/full_name.py` & `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/full_name.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/gender.py` & `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/gender.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/id_number.py` & `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/id_number.py`

 * *Files identical despite different names*

### Comparing `wheelz_idp_validations-2.1.4/src/wheelz_idp_validations/sanitizers/vin.py` & `wheelz_idp_validations-2.2.0/src/wheelz_idp_validations/sanitizers/vin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import re
+from ..exceptions.vin_exceptions import *
 
 def calculate_check_digit(vin):
-    # Mapeo de letras a valores para cálculo del VIN
-    vin_map = "0123456789.ABCDEFGH..JKLMN.P.R..STUVWXYZ"
+    # Mapeo de letras a valores para cálculo del VIN según la norma ISO 3779
+    vin_values = {
+        '0': 0, '1': 1, '2': 2, '3': 3, '4': 4, '5': 5, '6': 6, '7': 7, '8': 8, '9': 9,
+        'A': 1, 'B': 2, 'C': 3, 'D': 4, 'E': 5, 'F': 6, 'G': 7, 'H': 8,
+        'J': 1, 'K': 2, 'L': 3, 'M': 4, 'N': 5, 'P': 7, 'R': 9,
+        'S': 2, 'T': 3, 'U': 4, 'V': 5, 'W': 6, 'X': 7, 'Y': 8, 'Z': 9
+    }
     weights = [8, 7, 6, 5, 4, 3, 2, 10, 0, 9, 8, 7, 6, 5, 4, 3, 2]
     
     # Calcular el valor del VIN
     sum = 0
     for i in range(len(vin)):
-        value = vin_map.index(vin[i])
-        sum += value * weights[i]
+        char = vin[i]
+        if char in vin_values:
+            value = vin_values[char]
+            sum += value * weights[i]
     
     # Calcular dígito de verificación
     check_digit = sum % 11
     check_digit = 'X' if check_digit == 10 else str(check_digit)
     
     return check_digit
 
-def vin_sanitizer(text):
+def sanitize_vin(received_vin):
     # Buscar VIN en el texto (17 caracteres, excluyendo I, O y Q)
     vin_pattern = r'[A-HJ-NPR-Z0-9]{17}'
-    matches = re.findall(vin_pattern, text.upper())
+    matches = re.findall(vin_pattern, received_vin.upper())
 
     for vin in matches:
         # Validar el dígito de verificación
         if vin[8] == calculate_check_digit(vin):
             return vin
 
     # Si no se encuentra ningún VIN válido, lanzar excepción
-    raise InvalidVINException("No valid VIN found in the text")
-
-"""
-# Ejemplo de uso:
-text = "El VIN del vehículo es 1HGCM82633A004352 y otro dato 2FMDK3GC4BBA28456."
-vin_found = vin_sanitizer(text)
-print(vin_found)
-"""
+    raise InvalidVinException(received_vin)
```

### Comparing `wheelz_idp_validations-2.1.4/pyproject.toml` & `wheelz_idp_validations-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/wheelz_idp_validations"]
 
 
 [project]
 name = "wheelz_idp_validations"
-version = "2.1.4"
+version = "2.2.0"
 authors = [
   { name="Lluis" },
 ]
 description = "Validation for spasnish documents"
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `wheelz_idp_validations-2.1.4/PKG-INFO` & `wheelz_idp_validations-2.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wheelz_idp_validations
-Version: 2.1.4
+Version: 2.2.0
 Summary: Validation for spasnish documents
 Project-URL: Homepage, https://github.com/albertvazquezm/wheelz-idp-validations
 Project-URL: Issues, https://github.com/albertvazquezm/wheelz-idp-validationsissues
 Author: Lluis
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

