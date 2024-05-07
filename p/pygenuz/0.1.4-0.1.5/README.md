# Comparing `tmp/pygenuz-0.1.4.tar.gz` & `tmp/pygenuz-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenuz-0.1.4.tar", last modified: Mon May  6 10:53:37 2024, max compression
+gzip compressed data, was "pygenuz-0.1.5.tar", last modified: Tue May  7 17:15:36 2024, max compression
```

## Comparing `pygenuz-0.1.4.tar` & `pygenuz-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-06 10:53:37.031062 pygenuz-0.1.4/
--rw-r--r--   0 khezozbek   (501) staff       (20)     9038 2024-05-06 10:53:37.030583 pygenuz-0.1.4/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)     8407 2024-05-06 10:00:00.000000 pygenuz-0.1.4/README.md
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-06 10:53:37.029374 pygenuz-0.1.4/pygenuz/
--rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-06 10:08:02.000000 pygenuz-0.1.4/pygenuz/__init__.py
--rw-r--r--   0 khezozbek   (501) staff       (20)     3785 2024-05-06 09:20:00.000000 pygenuz-0.1.4/pygenuz/app.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.1.4/pygenuz/middelware.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.1.4/pygenuz/response.py
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-06 10:53:37.030351 pygenuz-0.1.4/pygenuz.egg-info/
--rw-r--r--   0 khezozbek   (501) staff       (20)     9038 2024-05-06 10:53:36.000000 pygenuz-0.1.4/pygenuz.egg-info/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)      249 2024-05-06 10:53:37.000000 pygenuz-0.1.4/pygenuz.egg-info/SOURCES.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-06 10:53:36.000000 pygenuz-0.1.4/pygenuz.egg-info/dependency_links.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)      105 2024-05-06 10:53:36.000000 pygenuz-0.1.4/pygenuz.egg-info/requires.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-06 10:53:36.000000 pygenuz-0.1.4/pygenuz.egg-info/top_level.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-06 10:53:37.031135 pygenuz-0.1.4/setup.cfg
--rw-r--r--   0 khezozbek   (501) staff       (20)     3894 2024-05-06 10:53:36.000000 pygenuz-0.1.4/setup.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:15:36.471612 pygenuz-0.1.5/
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13897 2024-05-07 17:15:36.471324 pygenuz-0.1.5/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13266 2024-05-07 17:14:28.000000 pygenuz-0.1.5/README.md
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:15:36.469934 pygenuz-0.1.5/pygenuz/
+-rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.1.5/pygenuz/__init__.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.1.5/pygenuz/app.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.1.5/pygenuz/configs.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.1.5/pygenuz/db.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.1.5/pygenuz/middelware.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.1.5/pygenuz/response.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-07 17:15:36.470943 pygenuz-0.1.5/pygenuz.egg-info/
+-rw-r--r--   0 khezozbek   (501) staff       (20)    13897 2024-05-07 17:15:36.000000 pygenuz-0.1.5/pygenuz.egg-info/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-07 17:15:36.000000 pygenuz-0.1.5/pygenuz.egg-info/SOURCES.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-07 17:15:36.000000 pygenuz-0.1.5/pygenuz.egg-info/dependency_links.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-07 17:15:36.000000 pygenuz-0.1.5/pygenuz.egg-info/requires.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-07 17:15:36.000000 pygenuz-0.1.5/pygenuz.egg-info/top_level.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-07 17:15:36.471690 pygenuz-0.1.5/setup.cfg
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-07 16:21:28.000000 pygenuz-0.1.5/setup.py
```

### Comparing `pygenuz-0.1.4/pygenuz/app.py` & `pygenuz-0.1.5/pygenuz/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         )
         self.exception_handler = None
 
         self.whitenoise = WhiteNoise(self.wsgi_app, root=static_dir, prefix="/static")
 
         self.middleware = Middleware(self)
 
+
     def __call__(self, environ, start_response):
         path_inf = environ["PATH_INFO"]
 
         if path_inf.startswith("/static"):
             return self.whitenoise(environ, start_response)
         return self.middleware(environ, start_response)
     
@@ -104,8 +105,8 @@
             context = {}
         return self.template_env.get_template(template_name).render(**context)
     
     def add_exception_handler(self, handler):
         self.exception_handler = handler
 
     def add_middleware(self, middleware_cls):
-        self.middleware.add(middleware_cls)
+        self.middleware.add(middleware_cls)
```

### Comparing `pygenuz-0.1.4/pygenuz/middelware.py` & `pygenuz-0.1.5/pygenuz/middelware.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.1.4/pygenuz/response.py` & `pygenuz-0.1.5/pygenuz/response.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.1.4/setup.py` & `pygenuz-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,25 @@
 # Package meta-data.
 NAME = 'pygenuz'
 DESCRIPTION = 'My first Python web framework.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'cssezozbel@gmail.com'
 AUTHOR = "E'zozbek Kholbutayev"
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
     "WebOb==1.8.7",
-    "whitenoise==6.6.0"
+    "whitenoise==6.6.0",
+    "sqlalchemy"
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

