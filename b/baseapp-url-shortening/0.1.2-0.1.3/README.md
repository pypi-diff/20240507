# Comparing `tmp/baseapp-url-shortening-0.1.2.tar.gz` & `tmp/baseapp-url-shortening-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseapp-url-shortening-0.1.2.tar", last modified: Tue Apr 16 18:17:51 2024, max compression
+gzip compressed data, was "baseapp-url-shortening-0.1.3.tar", last modified: Tue May  7 20:53:37 2024, max compression
```

## Comparing `baseapp-url-shortening-0.1.2.tar` & `baseapp-url-shortening-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.607351 baseapp-url-shortening-0.1.2/baseapp_url_shortening/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/baseapp_url_shortening/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/migrations/0002_alter_shorturl_full_url.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/integration/test_url_shortening.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-16 18:17:51.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-16 18:17:51.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:17:51.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 18:17:51.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 18:17:51.000000 baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:51.611351 baseapp-url-shortening-0.1.2/testproject/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/testproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/testproject/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-16 18:17:49.000000 baseapp-url-shortening-0.1.2/testproject/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:53:37.834558 baseapp-url-shortening-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-07 20:53:37.834558 baseapp-url-shortening-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:53:37.830558 baseapp-url-shortening-0.1.3/baseapp_url_shortening/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:53:37.834558 baseapp-url-shortening-0.1.3/baseapp_url_shortening/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/migrations/0002_alter_shorturl_full_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:53:37.834558 baseapp-url-shortening-0.1.3/baseapp_url_shortening/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/tests/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:53:37.834558 baseapp-url-shortening-0.1.3/baseapp_url_shortening/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/tests/integration/test_url_shortening.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:53:37.834558 baseapp-url-shortening-0.1.3/baseapp_url_shortening.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/baseapp_url_shortening.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-07 20:53:37.834558 baseapp-url-shortening-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:53:37.834558 baseapp-url-shortening-0.1.3/testproject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/testproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/testproject/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-07 20:53:37.000000 baseapp-url-shortening-0.1.3/testproject/urls.py
```

### Comparing `baseapp-url-shortening-0.1.2/PKG-INFO` & `baseapp-url-shortening-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp-url-shortening
-Version: 0.1.2
+Version: 0.1.3
 Summary: BaseApp URL Shortening
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause  # Example license
 Description: # BaseApp URL Shortening
```

### Comparing `baseapp-url-shortening-0.1.2/README.md` & `baseapp-url-shortening-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `baseapp-url-shortening-0.1.2/baseapp_url_shortening/migrations/0001_initial.py` & `baseapp-url-shortening-0.1.3/baseapp_url_shortening/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `baseapp-url-shortening-0.1.2/baseapp_url_shortening/models.py` & `baseapp-url-shortening-0.1.3/baseapp_url_shortening/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class ShortUrl(TimeStampedModel):
     short_code = models.CharField(max_length=30, editable=False, unique=True, db_index=True)
     full_url = models.URLField(max_length=2000)
 
     @property
     def short_url_path(self) -> str:
-        return reverse("short_url_redirect_full_url", kwargs=dict(short_code=self.short_code))
+        return reverse("v1:short_url_redirect_full_url", kwargs=dict(short_code=self.short_code))
 
     def save(self, *args, **kwargs):
         creating = not self.pk
         super().save(*args, **kwargs)
         if creating:
             self.short_code = short_url.encode_url(self.pk)
             super().save(update_fields=["short_code"])
```

### Comparing `baseapp-url-shortening-0.1.2/baseapp_url_shortening/tests/integration/test_url_shortening.py` & `baseapp-url-shortening-0.1.3/baseapp_url_shortening/tests/integration/test_url_shortening.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,9 @@
     def test_short_url_redirects_to_full_url(self, client):
         instance = f.ShortUrlFactory()
         r = client.get(instance.short_url_path)
         assert r.status_code == 302
         assert r.url == instance.full_url
 
     def test_redirect_nonexistent_short_code(self, client):
-        response = client.get("/c/invalid_code")
+        response = client.get("/v1/c/invalid_code")
         assert response.status_code == 404
```

### Comparing `baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/PKG-INFO` & `baseapp-url-shortening-0.1.3/baseapp_url_shortening.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp-url-shortening
-Version: 0.1.2
+Version: 0.1.3
 Summary: BaseApp URL Shortening
 Home-page: https://github.com/silverlogic/baseapp-backend
 Author: The SilverLogic
 Author-email: dev@tsl.io
 License: BSD-3-Clause  # Example license
 Description: # BaseApp URL Shortening
```

### Comparing `baseapp-url-shortening-0.1.2/baseapp_url_shortening.egg-info/SOURCES.txt` & `baseapp-url-shortening-0.1.3/baseapp_url_shortening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baseapp-url-shortening-0.1.2/setup.cfg` & `baseapp-url-shortening-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = baseapp_url_shortening
-version = 0.1.2
+version = 0.1.3
 description = BaseApp URL Shortening
 long_description = file: README.md
 url = https://github.com/silverlogic/baseapp-backend
 author = The SilverLogic
 author_email = dev@tsl.io
 license = BSD-3-Clause  # Example license
```

