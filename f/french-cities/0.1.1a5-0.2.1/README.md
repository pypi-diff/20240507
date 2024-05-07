# Comparing `tmp/french_cities-0.1.1a5.tar.gz` & `tmp/french_cities-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "french_cities-0.1.1a5.tar", max compression
+gzip compressed data, was "french_cities-0.2.1.tar", max compression
```

## Comparing `french_cities-0.1.1a5.tar` & `french_cities-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10122 2023-08-07 13:49:31.923573 french_cities-0.1.1a5/README.fr.md
--rw-r--r--   0        0        0     8563 2023-08-07 13:49:31.923573 french_cities-0.1.1a5/README.md
--rw-r--r--   0        0        0      394 2023-08-07 13:49:31.923573 french_cities-0.1.1a5/french_cities/__init__.py
--rw-r--r--   0        0        0    30927 2023-08-07 13:49:31.923573 french_cities-0.1.1a5/french_cities/city_finder.py
--rw-r--r--   0        0        0     9317 2023-08-07 13:49:31.923573 french_cities-0.1.1a5/french_cities/departement_finder.py
--rw-r--r--   0        0        0      519 2023-08-07 13:49:31.923573 french_cities-0.1.1a5/french_cities/utils.py
--rw-r--r--   0        0        0     7956 2023-08-07 13:49:31.923573 french_cities-0.1.1a5/french_cities/vintage.py
--rw-r--r--   0        0        0     1279 2023-08-07 13:49:31.923573 french_cities-0.1.1a5/pyproject.toml
--rw-r--r--   0        0        0    20232 1970-01-01 00:00:00.000000 french_cities-0.1.1a5/PKG-INFO
+-rw-r--r--   0        0        0     9777 2024-05-07 08:53:03.807199 french_cities-0.2.1/README.fr.md
+-rw-r--r--   0        0        0     8299 2024-05-07 08:53:03.807199 french_cities-0.2.1/README.md
+-rw-r--r--   0        0        0      394 2024-05-07 08:53:03.807199 french_cities-0.2.1/french_cities/__init__.py
+-rw-r--r--   0        0        0    31541 2024-05-07 08:53:03.807199 french_cities-0.2.1/french_cities/city_finder.py
+-rw-r--r--   0        0        0     9502 2024-05-07 08:53:03.807199 french_cities-0.2.1/french_cities/departement_finder.py
+-rw-r--r--   0        0        0      519 2024-05-07 08:53:03.807199 french_cities-0.2.1/french_cities/utils.py
+-rw-r--r--   0        0        0     8302 2024-05-07 08:53:03.807199 french_cities-0.2.1/french_cities/vintage.py
+-rw-r--r--   0        0        0     1270 2024-05-07 08:53:03.807199 french_cities-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    19617 1970-01-01 00:00:00.000000 french_cities-0.2.1/PKG-INFO
```

### Comparing `french_cities-0.1.1a5/README.fr.md` & `french_cities-0.2.1/README.fr.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,14 @@
 départements ou de communes...
 
 
 # Installation
 
 `pip install french-cities[full]`
 
-Notez qu'à cette heure, `pynsee` ne supporte pas les projections de codes commune. 
-Dans l'immédiat, après avoir installé `french-cities` depuis pypi, il faut donc
-désinstaller `pynsee` puis réinstaller la version master courante depuis son repo 
-github :
-```
-pip uninstall pynsee
-pip install git+https://github.com/InseeFrLab/pynsee
-```
-
 L'installation "full" permet d'installer geopy qui est une dépendance 
 optionnelle utilisable en dernier ressort.
 
 # Configuration
 
 ## Ajout des clefs API INSEE
 `french-cities` utilise `pynsee`, qui nécessite des cles API INSEE pour être
```

### Comparing `french_cities-0.1.1a5/README.md` & `french_cities-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,14 @@
 Toolbox on french cities: set vintage, find departments, find cities...
 
 
 # Installation
 
 `pip install french-cities[full]`
 
-Note that at this instant, `pynsee` doesn't support communal projection.
-After installing `french-cities` from pypi, please uninstall pynsee and replace
-it with the current master:
-```
-pip uninstall pynsee
-pip install git+https://github.com/InseeFrLab/pynsee
-```
-
 Note that the "full" installation will also install geopy, which might use
 Nominatim API for city recognition as a last resort.
 
 
 # Configuration
 
 ## Setting INSEE's API keys
```

### Comparing `french_cities-0.1.1a5/french_cities/city_finder.py` & `french_cities-0.2.1/french_cities/city_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from datetime import date, timedelta
 from typing import Union
 import numpy as np
 from functools import partial
 from uuid import uuid4
 from tqdm import tqdm
 from pebble import ThreadPool
+
 try:
     from geopy.extra.rate_limiter import RateLimiter
     from geopy.geocoders import Nominatim
 except ModuleNotFoundError:
     pass
 
 
@@ -156,15 +157,16 @@
         )
         raise ValueError(msg)
 
     init_pynsee()
 
     if not session:
         session = CachedSession(
-            allowable_methods=("GET", "POST"), expire_after=timedelta(days=30)
+            allowable_methods=("GET", "POST"),
+            expire_after=timedelta(days=30),
         )
 
     if len(necessary3 - columns) == 0 and not epsg:
         logger.warning(
             "x and y columns where found, but a valid EPSG projection was not "
             "set: geolocation will not be performed"
         )
@@ -190,15 +192,17 @@
             )  # Neuville-Housset (La) -> Neuville-Housset
             .str.upper()
             .apply(unidecode)  # A voir si on conserve
             .str.split(r"\W+")
             .str.join(" ")
             .str.replace(r"(^|\s)(ST)\s", " SAINT ", regex=True)
             .str.replace(r"(^|\s)(STE)\s", " SAINTE ", regex=True)
-            .str.replace(r"[0-9]* ?EME KM", "", regex=True)  # TAMPON 14EME KM
+            .str.replace(
+                r"[0-9]* ?EME KM", "", regex=True
+            )  # TAMPON 14EME KM
             .str.strip(" ")
             .str.replace(r" ?CEDEX$", "", regex=True)  # LOOS CEDEX -> LOOS
         )
 
     # Control which configuration can be used
     # Note that the order is relevant here, as this will determine the result's
     # preference
@@ -266,15 +270,17 @@
             if isinstance(x, str) and x.startswith("candidat_")
         ]
 
         ix = addresses[
             np.all(
                 [addresses[col].isnull() for col in cols_candidates], axis=0
             )
-            & np.all([addresses[col].notnull() for col in components], axis=0)
+            & np.all(
+                [addresses[col].notnull() for col in components], axis=0
+            )
         ].index
         if len(ix) == 0:
             addresses[f"candidat_{k+1}"] = np.nan
             continue
 
         temp_addresses = addresses.loc[ix].drop(cols_candidates, axis=1)
         temp_addresses = temp_addresses.drop_duplicates().fillna("")
@@ -293,15 +299,17 @@
             list_map(temp_addresses.copy(), components).to_frame("full")
         )
         temp_addresses = temp_addresses.drop_duplicates("full", keep="first")
 
         if "full" in set(addresses.columns):
             addresses = addresses.drop("full", axis=1)
         addresses = addresses.join(
-            list_map(addresses.fillna("").copy(), components).to_frame("full")
+            list_map(addresses.fillna("").copy(), components).to_frame(
+                "full"
+            )
         )
 
         results_api = _query_BAN_csv_geocoder(
             addresses=temp_addresses,
             components=components,
             session=session,
             dep=dep,
@@ -464,15 +472,15 @@
         geolocator = Nominatim(user_agent=user_agent)
     except NameError:
         logger.error(
             "geopy not installed - please install optional dependencies "
             "to use Nominatim geocoder with: pip install french-cities[full]"
         )
         return pd.DataFrame()
-        
+
     geocode = RateLimiter(
         partial(
             geolocator.geocode,
             language="fr",
             country_codes="fr",
             featuretype="settlement ",
         ),
@@ -561,15 +569,20 @@
             columns=df.loc[ix2, "CODE"],
             # index=look_for.loc[ix1, "city_cleaned"],
             # columns=df.loc[ix2, "TITLE_SHORT"],
         ).replace(0, np.nan)
         # print(match_)
 
         try:
-            results.append(pd.Series(match_.idxmax(axis=1), index=ix1))
+            results.append(
+                pd.Series(
+                    match_.dropna(how="all", axis=1).idxmax(axis=1),
+                    index=ix1,
+                )
+            )
         except ValueError:
             continue
 
     results = pd.concat(results, ignore_index=False).sort_index()
 
     try:
         year = int(year)
@@ -647,15 +660,17 @@
             "setting: the querying of cities using coordinates WILL have "
             "approximative results."
         )
 
     com = get_geodata("ADMINEXPRESS-COG-CARTO.LATEST:commune")
     com = gpd.GeoDataFrame(com).set_crs("EPSG:3857")
 
-    transformer = Transformer.from_crs(epsg, 3857, accuracy=1, always_xy=True)
+    transformer = Transformer.from_crs(
+        epsg, 3857, accuracy=1, always_xy=True
+    )
 
     temp = transformer.transform(df[x].tolist(), df[y].tolist())
     temp = gpd.GeoSeries(
         gpd.points_from_xy(x=temp[0], y=temp[1], crs=3857),
         name="geometry",
         index=df.index,
     )
@@ -700,43 +715,55 @@
         DataFrame (same as original + columns ['result_score', 'result_city',
         'result_citycode'])
 
     """
     # Use the BAN's CSV geocoder
     logger.info(f"request BAN with CSV geocoder and {components}...")
 
+    files = [
+        ("data", addresses.to_csv(index=False)),
+        ("type", (None, "municipality")),
+        ("result_columns", (None, "full")),
+        ("result_columns", (None, "result_score")),
+        ("result_columns", (None, "result_city")),
+        ("result_columns", (None, "result_citycode")),
+    ]
+
     r = session.post(
         "https://api-adresse.data.gouv.fr/search/csv/",
-        files=[
-            ("data", addresses.to_csv(index=False)),
-            ("type", (None, "municipality")),
-            ("result_columns", (None, "full")),
-            ("result_columns", (None, "result_score")),
-            ("result_columns", (None, "result_city")),
-            ("result_columns", (None, "result_citycode")),
-        ],
+        files=files,
     )
+    if not r.ok:
+        raise Exception(
+            f"Failed to query BAN's API with {files=} - response was {r}"
+        )
 
     logger.info("résultat obtenu")
 
-    results_api = (
-        pd.read_csv(
-            io.BytesIO(r.content),
-            dtype={"dep": str, "result_citycode": str},
-        )
-        .drop_duplicates()
-        .loc[
-            :,
-            ["full", "result_score", "result_city", "result_citycode"],
-        ]
-        .merge(
-            addresses[[dep, "full", "city_cleaned"]].drop_duplicates(),
-            on="full",
+    try:
+        results_api = (
+            pd.read_csv(
+                io.BytesIO(r.content),
+                dtype={"dep": str, "result_citycode": str},
+            )
+            .drop_duplicates()
+            .loc[
+                :,
+                ["full", "result_score", "result_city", "result_citycode"],
+            ]
+            .merge(
+                addresses[[dep, "full", "city_cleaned"]].drop_duplicates(),
+                on="full",
+            )
+        )
+    except Exception:
+        raise ValueError(
+            "Failed to parse BAN's return with following content :\n\n"
+            f"{r.content}"
         )
-    )
     return results_api
 
 
 def _query_BAN_individual_geocoder(
     addresses: pd.DataFrame,
     components: list,
     session: Session,
@@ -893,17 +920,17 @@
     results_api["result_city"] = (
         results_api["result_city"]
         .str.upper()
         .apply(unidecode)
         .str.split(r"\W+")
         .str.join(" ")
     )
-    results_api["score"] = results_api[["city_cleaned", "result_city"]].apply(
-        lambda xy: fuzz.token_set_ratio(*xy), axis=1
-    )
+    results_api["score"] = results_api[
+        ["city_cleaned", "result_city"]
+    ].apply(lambda xy: fuzz.token_set_ratio(*xy), axis=1)
 
     ix = results_api[
         # Either a good fuzzy match
         (
             (results_api["city_cleaned"] != "")
             & (results_api["score"] > fuzzymatch_threshold)
         )
@@ -912,26 +939,29 @@
         | (
             (results_api["city_cleaned"] != "")
             & (results_api["result_score"] > ban_score_threshold_city_known)
         )
         # Or a goodish match on BAN but no available city label:
         | (
             (results_api["city_cleaned"] == "")
-            & (results_api["result_score"] > ban_score_threshold_city_unknown)
+            & (
+                results_api["result_score"]
+                > ban_score_threshold_city_unknown
+            )
         )
     ].index
 
     if rename_candidat in addresses.columns:
         results_api = results_api.loc[ix, ["full", "result_citycode"]]
         addresses = addresses.merge(results_api, on="full", how="left")
         ix = addresses[addresses.result_citycode.notnull()].index
         addresses.loc[ix, rename_candidat] = addresses.loc[
             ix, "result_citycode"
         ]
         addresses = addresses.drop("result_citycode", axis=1)
 
     else:
-        results_api = results_api.loc[ix, ["full", "result_citycode"]].rename(
-            {"result_citycode": rename_candidat}, axis=1
-        )
+        results_api = results_api.loc[
+            ix, ["full", "result_citycode"]
+        ].rename({"result_citycode": rename_candidat}, axis=1)
         addresses = addresses.merge(results_api, on="full", how="left")
     return addresses
```

### Comparing `french_cities-0.1.1a5/french_cities/departement_finder.py` & `french_cities-0.2.1/french_cities/departement_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,31 +46,39 @@
     df : pd.DataFrame
         Updated DataFrame with departement's codes
 
     """
 
     if not session:
         session = CachedSession(
-            allowable_methods=("GET", "POST"), expire_after=timedelta(days=30)
+            allowable_methods=("GET", "POST"),
+            expire_after=timedelta(days=30),
         )
 
     postal_codes = df[[source]].drop_duplicates(keep="first")
+    files = [
+        ("data", postal_codes.to_csv(index=False)),
+        ("postcode", (None, source)),
+        ("result_columns", (None, source)),
+        ("result_columns", (None, "result_context")),
+    ]
     r = session.post(
         # recherche grâce à l'API de la BAN
         "https://api-adresse.data.gouv.fr/search/csv/",
-        files=[
-            ("data", postal_codes.to_csv(index=False)),
-            ("postcode", (None, source)),
-            ("result_columns", (None, source)),
-            ("result_columns", (None, "result_context")),
-        ],
+        files=files,
     )
+    if not r.ok:
+        raise Exception(
+            f"Failed to query BAN's API with {files=} - response was {r}"
+        )
     result = pd.read_csv(io.BytesIO(r.content), dtype=str)
     result[alias] = (
-        result["result_context"].str.split(",", expand=True)[0].str.strip(" ")
+        result["result_context"]
+        .str.split(",", expand=True)[0]
+        .str.strip(" ")
     )
     result = result.drop("result_context", axis=1)
 
     # where code is unknown, use Christian Quest Dataset with Cedex codes and
     # OpenDataSoft API (v2.1 contrairement à la doc disponible) en Freemium
     # https://www.data.gouv.fr/fr/datasets/liste-des-cedex/#_
     # https://public.opendatasoft.com/explore/dataset/correspondance-code-cedex-code-insee/information/?flg=fr&q=code%3D68013&lang=fr
@@ -148,15 +156,17 @@
                 r" CEDEX", ""
             )
             results_cedex["score"] = results_cedex[
                 ["libelle", "nom_com"]
             ].apply(lambda xy: fuzz.token_set_ratio(*xy), axis=1)
 
             results_cedex = results_cedex.sort_values([source, "score"])
-            results_cedex = results_cedex.drop_duplicates(source, keep="last")
+            results_cedex = results_cedex.drop_duplicates(
+                source, keep="last"
+            )
             results_cedex = results_cedex.drop(
                 ["nom_com", "score", "libelle"], axis=1
             )
             results_cedex = results_cedex.drop_duplicates()
 
             results_cedex = _process_departements_from_insee_code(
                 results_cedex,
```

### Comparing `french_cities-0.1.1a5/french_cities/utils.py` & `french_cities-0.2.1/french_cities/utils.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.1a5/french_cities/vintage.py` & `french_cities-0.2.1/french_cities/vintage.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,14 +87,18 @@
     2  01004
     3  01005
     4  01006
 
     """
     date = f"{year}-01-01"
     cog = get_area_list(area="communes", date=date)
+    try:
+        cog = cog.drop("DATE_DELETION", axis=1)
+    except KeyError:
+        pass
     cog = cog.drop(
         [
             "URI",
             "AREA_TYPE",
             "DETERMINER_TYPE",
             "TITLE",
             "TITLE_SHORT",
@@ -177,23 +181,28 @@
     2  13203  13055
     3  13204  13055
     4  13205  13055
 
     """
     date = f"{year}-01-01"
     subareas = get_area_list(area=type_, date=date)
+    try:
+        subareas = subareas.drop("DATE_DELETION", axis=1)
+    except KeyError:
+        pass
     drop = [
         "URI",
         "AREA_TYPE",
         "DETERMINER_TYPE",
         "TITLE",
         "DATE_CREATION",
         "TITLE_SHORT",
     ]
     subareas = subareas.drop(drop, axis=1)
+
     if look_for:
         subareas = subareas[subareas.CODE.isin(look_for)]
     if subareas.empty:
         return pd.DataFrame()
 
     single_area = {
         "arrondissementsMunicipaux": "arrondissementMunicipal",
@@ -240,15 +249,17 @@
 
     if uniques.empty:
         return df
 
     cities = _get_cities_year_full(year, set(uniques[field]))
 
     # Uptodate cities (cities, municipal districts, delegated cities, ...)
-    uniques = uniques.merge(cities, left_on=field, right_on="CODE", how="left")
+    uniques = uniques.merge(
+        cities, left_on=field, right_on="CODE", how="left"
+    )
     uniques = uniques.rename({"NEW_CODE": "PROJECTED"}, axis=1)
 
     # Obsolete cities : merge, etc. : look for projection starting from an old
     # date, using INSEE API
     date = f"{year}-01-01"
     starting_dates = [
         "1943-01-01",
@@ -263,14 +274,18 @@
             # Hack to deactivate standard error log entries by pynsee which are
             # concieved with a valid date in mind.
             previous_level = logging.root.manager.disable
             logging.disable(logging.ERROR)
             df = get_area_projection(
                 code=x, area="commune", date=date_init, dateProjection=date
             )
+            try:
+                df = df.drop("DATE_DELETION", axis=1)
+            except (KeyError, AttributeError):
+                pass
             logging.disable(previous_level)
 
             if df is not None:
                 break
         try:
             return df.at[0, "code"]
         except Exception:
```

### Comparing `french_cities-0.1.1a5/pyproject.toml` & `french_cities-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "french-cities"
-version = "0.1.1a5"
+version = "0.2.1"
 description = "Toolbox on french cities: set vintage, find departments, find cities..."
 authors = ["thomas.grandjean <thomas.grandjean@developpement-durable.gouv.fr>"]
-license = "etalab-2.0"
+license = "MIT"
 readme = ["README.md", "README.fr.md"]
 homepage = "https://github.com/tgrandje/french-cities/"
 repository = "https://github.com/tgrandje/french-cities/"
 documentation = "https://github.com/tgrandje/french-cities/"
 keywords = ["france", "cities"]
 packages = [{include = "french_cities"}]
 classifiers = [
@@ -17,22 +17,22 @@
     "Topic :: Scientific/Engineering",
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tgrandje/french-cities/issues"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 requests-cache = "^1.1.0"
 unidecode = "^1.3.6"
 python-dotenv = "^1.0.0"
-pandas = "^2.0.3"
-geopandas = "^0.13.2"
+pandas = "^2.2.2"
+geopandas = "^0.14.4"
 rapidfuzz = "^3.1.1"
-pynsee = "^0.1.4"
+pynsee = "^0.1.7"
 pebble = "^5.0.3"
 tqdm = "^4.65.0"
 importlib-metadata = "^6.8.0"
 geopy = "^2.3.0"
 
 [tool.poetry.extras]
 full = ["geopy"]
```

### Comparing `french_cities-0.1.1a5/PKG-INFO` & `french_cities-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: french-cities
-Version: 0.1.1a5
+Version: 0.2.1
 Summary: Toolbox on french cities: set vintage, find departments, find cities...
 Home-page: https://github.com/tgrandje/french-cities/
-License: etalab-2.0
+License: MIT
 Keywords: france,cities
 Author: thomas.grandjean
 Author-email: thomas.grandjean@developpement-durable.gouv.fr
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: full
-Requires-Dist: geopandas (>=0.13.2,<0.14.0)
+Requires-Dist: geopandas (>=0.14.4,<0.15.0)
 Requires-Dist: geopy (>=2.3.0,<3.0.0) ; extra == "full"
 Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0)
-Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pebble (>=5.0.3,<6.0.0)
-Requires-Dist: pynsee (>=0.1.4,<0.2.0)
+Requires-Dist: pynsee (>=0.1.7,<0.2.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rapidfuzz (>=3.1.1,<4.0.0)
 Requires-Dist: requests-cache (>=1.1.0,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: unidecode (>=1.3.6,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/tgrandje/french-cities/issues
 Project-URL: Documentation, https://github.com/tgrandje/french-cities/
@@ -38,22 +38,14 @@
 Toolbox on french cities: set vintage, find departments, find cities...
 
 
 # Installation
 
 `pip install french-cities[full]`
 
-Note that at this instant, `pynsee` doesn't support communal projection.
-After installing `french-cities` from pypi, please uninstall pynsee and replace
-it with the current master:
-```
-pip uninstall pynsee
-pip install git+https://github.com/InseeFrLab/pynsee
-```
-
 Note that the "full" installation will also install geopy, which might use
 Nominatim API for city recognition as a last resort.
 
 
 # Configuration
 
 ## Setting INSEE's API keys
@@ -278,23 +270,14 @@
 départements ou de communes...
 
 
 # Installation
 
 `pip install french-cities[full]`
 
-Notez qu'à cette heure, `pynsee` ne supporte pas les projections de codes commune. 
-Dans l'immédiat, après avoir installé `french-cities` depuis pypi, il faut donc
-désinstaller `pynsee` puis réinstaller la version master courante depuis son repo 
-github :
-```
-pip uninstall pynsee
-pip install git+https://github.com/InseeFrLab/pynsee
-```
-
 L'installation "full" permet d'installer geopy qui est une dépendance 
 optionnelle utilisable en dernier ressort.
 
 # Configuration
 
 ## Ajout des clefs API INSEE
 `french-cities` utilise `pynsee`, qui nécessite des cles API INSEE pour être
```

