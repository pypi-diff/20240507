# Comparing `tmp/themoviedb-lib-0.0.2.tar.gz` & `tmp/themoviedb_lib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themoviedb-lib-0.0.2.tar", last modified: Thu Apr  4 14:37:31 2024, max compression
+gzip compressed data, was "themoviedb_lib-0.0.3.tar", last modified: Tue May  7 16:37:18 2024, max compression
```

## Comparing `themoviedb-lib-0.0.2.tar` & `themoviedb_lib-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:37:31.502574 themoviedb-lib-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-04 14:37:31.502574 themoviedb-lib-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:37:31.502574 themoviedb-lib-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:37:31.502574 themoviedb-lib-0.0.2/themoviedb_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-04 14:37:31.000000 themoviedb-lib-0.0.2/themoviedb_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-04 14:37:31.000000 themoviedb-lib-0.0.2/themoviedb_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:37:31.000000 themoviedb-lib-0.0.2/themoviedb_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 14:37:31.000000 themoviedb-lib-0.0.2/themoviedb_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 14:37:31.000000 themoviedb-lib-0.0.2/themoviedb_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:37:31.498574 themoviedb-lib-0.0.2/tmdb/
--rw-r--r--   0 runner    (1001) docker     (127)    17524 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/tmdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:37:31.502574 themoviedb-lib-0.0.2/tmdb/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/tmdb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/tmdb/tests/test_tmdb_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/tmdb/tests/test_tmdb_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-04 14:37:16.000000 themoviedb-lib-0.0.2/tmdb/tests/test_tmdb_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:37:18.355175 themoviedb_lib-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-07 16:37:18.355175 themoviedb_lib-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:37:18.355175 themoviedb_lib-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:37:18.355175 themoviedb_lib-0.0.3/themoviedb_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-07 16:37:18.000000 themoviedb_lib-0.0.3/themoviedb_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-07 16:37:18.000000 themoviedb_lib-0.0.3/themoviedb_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:37:18.000000 themoviedb_lib-0.0.3/themoviedb_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 16:37:18.000000 themoviedb_lib-0.0.3/themoviedb_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 16:37:18.000000 themoviedb_lib-0.0.3/themoviedb_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:37:18.355175 themoviedb_lib-0.0.3/tmdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/tmdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:37:18.355175 themoviedb_lib-0.0.3/tmdb/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/tmdb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/tmdb/tests/test_tmdb_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/tmdb/tests/test_tmdb_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-07 16:37:14.000000 themoviedb_lib-0.0.3/tmdb/tests/test_tmdb_request.py
```

### Comparing `themoviedb-lib-0.0.2/LICENSE` & `themoviedb_lib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `themoviedb-lib-0.0.2/PKG-INFO` & `themoviedb_lib-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themoviedb-lib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library providing useful tools for The Movie Database (TMDb). Not dependent on API-keys.
 Home-page: https://github.com/inwerk/themoviedb-lib
 Author: 
 Author-email: 
 Keywords: tmdb,themoviedb,the movie database,the movie db,movie,movies,tv,tv show,tv shows
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `themoviedb-lib-0.0.2/README.md` & `themoviedb_lib-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `themoviedb-lib-0.0.2/setup.py` & `themoviedb_lib-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Setting up
 setup(
     name="themoviedb-lib",  # Required
-    version="0.0.2",  # Required
+    version="0.0.3",  # Required
     description="Library providing useful tools for The Movie Database (TMDb). Not dependent on API-keys.",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional
     url="https://github.com/inwerk/themoviedb-lib",  # Optional
     author="",  # Optional
     author_email="",  # Optional
     classifiers=[  # Optional (https://pypi.org/classifiers/)
```

### Comparing `themoviedb-lib-0.0.2/themoviedb_lib.egg-info/PKG-INFO` & `themoviedb_lib-0.0.3/themoviedb_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themoviedb-lib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library providing useful tools for The Movie Database (TMDb). Not dependent on API-keys.
 Home-page: https://github.com/inwerk/themoviedb-lib
 Author: 
 Author-email: 
 Keywords: tmdb,themoviedb,the movie database,the movie db,movie,movies,tv,tv show,tv shows
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `themoviedb-lib-0.0.2/tmdb/__init__.py` & `themoviedb_lib-0.0.3/tmdb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,16 +160,17 @@
 
             if div_title.find('a') is not None:
                 tmdb_entry.tmdb_id = re.search(r'(\d+)', div_title.find('a').get('href')).group()
 
             if div_title.find('h2') is not None:
                 tmdb_entry.title = div_title.find('h2').get_text().replace('amp;', '')
 
-            if div_title.find('span') is not None:
-                tmdb_entry.release_year = re.search(r'(\d){4}', div_title.find('span').get_text()).group()
+            if div_title.find('span', {'class': 'release_date'}) is not None:
+                tmdb_entry.release_year = re.search(r'(\d){4}', div_title
+                                                    .find('span', {'class': 'release_date'}).get_text()).group()
 
             if div_card.find('p') is not None:
                 tmdb_entry.description = div_card.find('p').get_text()
 
             if div_card.find('img') is not None:
                 tmdb_entry.poster_id = (re.search(r'(\w)+.jpg', div_card.find('img').get('src')).group()
                                         .replace(".jpg", ""))
```

### Comparing `themoviedb-lib-0.0.2/tmdb/tests/test_tmdb_api.py` & `themoviedb_lib-0.0.3/tmdb/tests/test_tmdb_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,12 +133,12 @@
         width = 1000
         height = 2000
 
         self.assertRaises(ValueError, lambda: API.poster_path(poster_id=poster_id, width=width, height=height))
 
     # tests for TV.number_of_seasons()
     def test_number_of_seasons(self):
-        self.assertEqual(3, API.TV.number_of_seasons(series_id=253))
+        self.assertEqual(3, API.TV.number_of_seasons(series_id="253"))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `themoviedb-lib-0.0.2/tmdb/tests/test_tmdb_entry.py` & `themoviedb_lib-0.0.3/tmdb/tests/test_tmdb_entry.py`

 * *Files identical despite different names*

### Comparing `themoviedb-lib-0.0.2/tmdb/tests/test_tmdb_request.py` & `themoviedb_lib-0.0.3/tmdb/tests/test_tmdb_request.py`

 * *Files identical despite different names*

