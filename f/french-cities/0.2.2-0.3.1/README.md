# Comparing `tmp/french_cities-0.2.2.tar.gz` & `tmp/french_cities-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "french_cities-0.2.2.tar", max compression
+gzip compressed data, was "french_cities-0.3.1.tar", max compression
```

## Comparing `french_cities-0.2.2.tar` & `french_cities-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     9777 2024-05-07 12:02:37.894947 french_cities-0.2.2/README.fr.md
--rw-r--r--   0        0        0     8299 2024-05-07 12:02:37.894947 french_cities-0.2.2/README.md
--rw-r--r--   0        0        0      394 2024-05-07 12:02:37.894947 french_cities-0.2.2/french_cities/__init__.py
--rw-r--r--   0        0        0    31541 2024-05-07 12:02:37.894947 french_cities-0.2.2/french_cities/city_finder.py
--rw-r--r--   0        0        0     9502 2024-05-07 12:02:37.894947 french_cities-0.2.2/french_cities/departement_finder.py
--rw-r--r--   0        0        0      519 2024-05-07 12:02:37.894947 french_cities-0.2.2/french_cities/utils.py
--rw-r--r--   0        0        0     8302 2024-05-07 12:02:37.894947 french_cities-0.2.2/french_cities/vintage.py
--rw-r--r--   0        0        0     1308 2024-05-07 12:02:37.894947 french_cities-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    19666 1970-01-01 00:00:00.000000 french_cities-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    10260 2024-05-07 14:03:30.600273 french_cities-0.3.1/README.fr.md
+-rw-r--r--   0        0        0     8729 2024-05-07 14:03:30.600273 french_cities-0.3.1/README.md
+-rw-r--r--   0        0        0      430 2024-05-07 14:03:30.600273 french_cities-0.3.1/french_cities/__init__.py
+-rw-r--r--   0        0        0    31541 2024-05-07 14:03:30.600273 french_cities-0.3.1/french_cities/city_finder.py
+-rw-r--r--   0        0        0    10978 2024-05-07 14:03:30.600273 french_cities-0.3.1/french_cities/departement_finder.py
+-rw-r--r--   0        0        0      519 2024-05-07 14:03:30.600273 french_cities-0.3.1/french_cities/utils.py
+-rw-r--r--   0        0        0     8302 2024-05-07 14:03:30.600273 french_cities-0.3.1/french_cities/vintage.py
+-rw-r--r--   0        0        0     1308 2024-05-07 14:03:30.600273 french_cities-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    20579 1970-01-01 00:00:00.000000 french_cities-0.3.1/PKG-INFO
```

### Comparing `french_cities-0.2.2/README.fr.md` & `french_cities-0.3.1/README.fr.md`

 * *Files 4% similar despite different names*

```diff
@@ -82,17 +82,34 @@
 )
 df = find_departements(df, source="code_postal", alias="dep_A", type_code="postcode")
 df = find_departements(df, source="code_commune", alias="dep_B", type_code="insee")
 
 print(df)
 ```
 
-Pour une documentation complète sur la fonction `find_departements`, merci 
-d'utiliser la commande suivante :
-`help(find_departements)`.
+On peut également travailler directement à partir des noms de départements,
+en utilisant à la place la fonction `find_departements_from_names` :
+
+```
+from french_cities import find_departements_from_names
+import pandas as pd
+
+df = pd.DataFrame(
+    {
+        "deps": ["Corse sud", "Alpe de Haute-Provence", "Aisne", "Ain"],
+    }
+)
+df = find_departements_from_names(df, label="deps")
+
+print(df)
+```
+
+Pour une documentation complète sur les fonctions `find_departements` ou
+`find_departements_from_names`, merci d'utiliser les commandes suivantes : 
+`help(find_departements)` ou `help(find_departements_from_names)`.
 
 ### Trouver les codes communes
 `french-cities` peut retrouver le code commune à partir de champs multiples.
 Il est capable de détecter certaines erreurs simples dans les champs (jusqu'à 
 une certaine limite).
 
 Les colonnes utilisées par l'algorithme pour cette détection sont (par ordre
```

### Comparing `french_cities-0.2.2/README.md` & `french_cities-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -78,16 +78,34 @@
 )
 df = find_departements(df, source="code_postal", alias="dep_A", type_code="postcode")
 df = find_departements(df, source="code_commune", alias="dep_B", type_code="insee")
 
 print(df)
 ```
 
-For a complete documentation on `find_departements`, please type 
-`help(find_departements)`.
+One can also work directly from departement's names, using 
+`find_departements_from_names` instead :
+
+```
+from french_cities import find_departements_from_names
+import pandas as pd
+
+df = pd.DataFrame(
+    {
+        "deps": ["Corse sud", "Alpe de Haute-Provence", "Aisne", "Ain"],
+    }
+)
+df = find_departements_from_names(df, label="deps")
+
+print(df)
+```
+
+For a complete documentation on `find_departements` or 
+`find_departements_from_names`, please type `help(find_departements)` or
+`help(find_departements_from_names)`.
 
 ### Retrieve cities' codes
 `french-cities` can retrieve cities' codes from multiple fields. It will work
 out basic mistakes (up to a certain limit).
 
 The columns used by the algorithm can be (in the order of precedence used by
 the algorithm):
```

### Comparing `french_cities-0.2.2/french_cities/city_finder.py` & `french_cities-0.3.1/french_cities/city_finder.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.2.2/french_cities/departement_finder.py` & `french_cities-0.3.1/french_cities/departement_finder.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from requests_cache import CachedSession
 from requests import Session
 from datetime import timedelta
 import logging
 import time
 from tqdm import tqdm
 from pebble import ThreadPool
-from rapidfuzz import fuzz
+from pynsee.localdata import get_area_list
+from rapidfuzz import fuzz, process
 from unidecode import unidecode
 
 from french_cities.utils import init_pynsee
 
 
 logger = logging.getLogger(__name__)
 
@@ -287,7 +288,65 @@
 
     df = df.copy()
     if type_code == "postcode":
         func = _process_departements_from_postal
     elif type_code == "insee":
         func = _process_departements_from_insee_code
     return func(df, source, alias, session)
+
+
+def find_departements_from_names(
+    df: pd.DataFrame, label: str, alias: str = "DEP_CODE"
+) -> pd.DataFrame:
+    """
+    Retrieve departement's codes from their names.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        DataFrame containing official departement's names
+    label : str
+        Field containing the label of the departements
+    alias : str, optional
+        Column to store the departements' codes unto.
+        Default is "DEP_CODE"
+
+    Returns
+    -------
+    df : pd.DataFrame
+        Updated DataFrame with departement's codes
+
+    """
+
+    init_pynsee()
+    candidates = get_area_list("departements")
+    candidates = candidates[["CODE", "TITLE"]]
+    candidates["TITLE"] = (
+        candidates["TITLE"]
+        .apply(unidecode)
+        .str.upper()
+        .str.replace(r"\W+", " ", regex=True)
+    )
+    candidates = dict(candidates[["TITLE", "CODE"]].values)
+    candidates_keys = list(candidates.keys())
+
+    df = df.copy()
+    df["FORMATTED"] = (
+        df[label]
+        .apply(unidecode)
+        .str.upper()
+        .str.replace(r"\W+", " ", regex=True)
+    )
+
+    df[alias] = df["FORMATTED"].apply(
+        lambda x: candidates[
+            process.extractOne(
+                x,
+                candidates_keys,
+                scorer=fuzz.token_set_ratio,
+                score_cutoff=80,
+            )[0]
+        ]
+    )
+    df = df.drop("FORMATTED", axis=1)
+
+    return df
```

### Comparing `french_cities-0.2.2/french_cities/utils.py` & `french_cities-0.3.1/french_cities/utils.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.2.2/french_cities/vintage.py` & `french_cities-0.3.1/french_cities/vintage.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.2.2/pyproject.toml` & `french_cities-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "french-cities"
-version = "0.2.2"
+version = "0.3.1"
 description = "Toolbox on french cities: set vintage, find departments, find cities..."
 authors = ["thomas.grandjean <thomas.grandjean@developpement-durable.gouv.fr>"]
 license = "GPL-3.0-or-later"
 readme = ["README.md", "README.fr.md"]
 homepage = "https://github.com/tgrandje/french-cities/"
 repository = "https://github.com/tgrandje/french-cities/"
 documentation = "https://github.com/tgrandje/french-cities/"
```

### Comparing `french_cities-0.2.2/PKG-INFO` & `french_cities-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: french-cities
-Version: 0.2.2
+Version: 0.3.1
 Summary: Toolbox on french cities: set vintage, find departments, find cities...
 Home-page: https://github.com/tgrandje/french-cities/
 License: GPL-3.0-or-later
 Keywords: france,cities
 Author: thomas.grandjean
 Author-email: thomas.grandjean@developpement-durable.gouv.fr
 Requires-Python: >=3.9,<4.0
@@ -114,16 +114,34 @@
 )
 df = find_departements(df, source="code_postal", alias="dep_A", type_code="postcode")
 df = find_departements(df, source="code_commune", alias="dep_B", type_code="insee")
 
 print(df)
 ```
 
-For a complete documentation on `find_departements`, please type 
-`help(find_departements)`.
+One can also work directly from departement's names, using 
+`find_departements_from_names` instead :
+
+```
+from french_cities import find_departements_from_names
+import pandas as pd
+
+df = pd.DataFrame(
+    {
+        "deps": ["Corse sud", "Alpe de Haute-Provence", "Aisne", "Ain"],
+    }
+)
+df = find_departements_from_names(df, label="deps")
+
+print(df)
+```
+
+For a complete documentation on `find_departements` or 
+`find_departements_from_names`, please type `help(find_departements)` or
+`help(find_departements_from_names)`.
 
 ### Retrieve cities' codes
 `french-cities` can retrieve cities' codes from multiple fields. It will work
 out basic mistakes (up to a certain limit).
 
 The columns used by the algorithm can be (in the order of precedence used by
 the algorithm):
@@ -349,17 +367,34 @@
 )
 df = find_departements(df, source="code_postal", alias="dep_A", type_code="postcode")
 df = find_departements(df, source="code_commune", alias="dep_B", type_code="insee")
 
 print(df)
 ```
 
-Pour une documentation complète sur la fonction `find_departements`, merci 
-d'utiliser la commande suivante :
-`help(find_departements)`.
+On peut également travailler directement à partir des noms de départements,
+en utilisant à la place la fonction `find_departements_from_names` :
+
+```
+from french_cities import find_departements_from_names
+import pandas as pd
+
+df = pd.DataFrame(
+    {
+        "deps": ["Corse sud", "Alpe de Haute-Provence", "Aisne", "Ain"],
+    }
+)
+df = find_departements_from_names(df, label="deps")
+
+print(df)
+```
+
+Pour une documentation complète sur les fonctions `find_departements` ou
+`find_departements_from_names`, merci d'utiliser les commandes suivantes : 
+`help(find_departements)` ou `help(find_departements_from_names)`.
 
 ### Trouver les codes communes
 `french-cities` peut retrouver le code commune à partir de champs multiples.
 Il est capable de détecter certaines erreurs simples dans les champs (jusqu'à 
 une certaine limite).
 
 Les colonnes utilisées par l'algorithme pour cette détection sont (par ordre
```

