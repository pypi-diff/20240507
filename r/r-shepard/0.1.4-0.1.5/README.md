# Comparing `tmp/r_shepard-0.1.4.tar.gz` & `tmp/r_shepard-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r_shepard-0.1.4.tar", max compression
+gzip compressed data, was "r_shepard-0.1.5.tar", max compression
```

## Comparing `r_shepard-0.1.4.tar` & `r_shepard-0.1.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     3517 2024-05-07 13:27:13.812834 r_shepard-0.1.4/README.md
--rwxr-xr-x   0        0        0      666 2024-05-01 08:42:22.525077 r_shepard-0.1.4/manage.py
--rw-r--r--   0        0        0      744 2024-05-07 13:28:22.868717 r_shepard-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      174 2024-05-06 20:18:43.831721 r_shepard-0.1.4/r_shepard/__init__.py
--rw-r--r--   0        0        0       52 2024-05-06 21:14:06.784472 r_shepard-0.1.4/r_shepard/api/__init__.py
--rw-r--r--   0        0        0     3231 2024-05-07 10:03:25.055844 r_shepard-0.1.4/r_shepard/api/admin.py
--rw-r--r--   0        0        0      457 2024-05-07 10:02:03.501832 r_shepard-0.1.4/r_shepard/api/apps.py
--rw-r--r--   0        0        0      179 2024-05-06 21:14:06.784472 r_shepard-0.1.4/r_shepard/api/appy.py
--rw-r--r--   0        0        0     1137 2024-05-07 10:01:34.041125 r_shepard-0.1.4/r_shepard/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      442 2024-05-07 10:01:34.041125 r_shepard-0.1.4/r_shepard/api/migrations/0002_project_is_active.py
--rw-r--r--   0        0        0      505 2024-05-07 10:01:34.041125 r_shepard-0.1.4/r_shepard/api/migrations/0003_project_url.py
--rw-r--r--   0        0        0      460 2024-05-07 10:01:34.041125 r_shepard-0.1.4/r_shepard/api/migrations/0004_project_rstudio_version.py
--rw-r--r--   0        0        0     1103 2024-05-07 10:01:34.042125 r_shepard-0.1.4/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py
--rw-r--r--   0        0        0     3210 2024-05-07 10:01:34.042125 r_shepard-0.1.4/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py
--rw-r--r--   0        0        0      491 2024-05-07 10:01:34.043125 r_shepard-0.1.4/r_shepard/api/migrations/0007_alter_container_container_id.py
--rw-r--r--   0        0        0     1688 2024-04-22 08:54:16.989356 r_shepard-0.1.4/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py
--rw-r--r--   0        0        0      506 2024-05-07 10:01:34.043125 r_shepard-0.1.4/r_shepard/api/migrations/0009_alter_container_port.py
--rw-r--r--   0        0        0      479 2024-05-07 10:01:34.043125 r_shepard-0.1.4/r_shepard/api/migrations/0010_alter_container_port.py
--rw-r--r--   0        0        0      518 2024-05-07 10:01:34.043125 r_shepard-0.1.4/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py
--rw-r--r--   0        0        0      586 2024-04-23 09:28:07.929488 r_shepard-0.1.4/r_shepard/api/migrations/0012_project_slug.py
--rw-r--r--   0        0        0      656 2024-04-23 11:30:47.550693 r_shepard-0.1.4/r_shepard/api/migrations/0013_remove_project_password_container_password.py
--rw-r--r--   0        0        0      541 2024-04-24 10:26:22.152733 r_shepard-0.1.4/r_shepard/api/migrations/0014_project_max_containers.py
--rw-r--r--   0        0        0      918 2024-04-24 13:21:19.864083 r_shepard-0.1.4/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py
--rw-r--r--   0        0        0     1381 2024-04-24 13:32:06.450029 r_shepard-0.1.4/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py
--rw-r--r--   0        0        0        0 2024-04-20 15:09:46.014593 r_shepard-0.1.4/r_shepard/api/migrations/__init__.py
--rw-r--r--   0        0        0     5512 2024-05-07 10:02:03.501832 r_shepard-0.1.4/r_shepard/api/models.py
--rw-r--r--   0        0        0     4346 2024-05-07 10:04:34.289600 r_shepard-0.1.4/r_shepard/api/podman.py
--rw-r--r--   0        0        0     3104 2024-05-07 09:58:12.404696 r_shepard-0.1.4/r_shepard/api/static/custom.css
--rw-r--r--   0        0        0    48101 2024-04-22 17:57:33.717054 r_shepard-0.1.4/r_shepard/api/static/htmx.min.js
--rw-r--r--   0        0        0    82210 2024-04-22 16:54:30.950446 r_shepard-0.1.4/r_shepard/api/static/pico.blue.min.css
--rw-r--r--   0        0        0    74999 2024-04-23 06:39:38.438525 r_shepard-0.1.4/r_shepard/api/static/pico.colors.min.css
--rw-r--r--   0        0        0     2982 2024-04-23 09:15:45.253107 r_shepard-0.1.4/r_shepard/api/tailscale.py
--rw-r--r--   0        0        0     1397 2024-04-25 07:52:49.580151 r_shepard-0.1.4/r_shepard/api/tasks.py
--rw-r--r--   0        0        0     5807 2024-05-07 10:02:03.502833 r_shepard-0.1.4/r_shepard/api/views.py
--rw-r--r--   0        0        0      395 2024-04-26 07:51:03.905968 r_shepard-0.1.4/r_shepard/asgi.py
--rw-r--r--   0        0        0      226 2024-04-26 08:04:10.741465 r_shepard-0.1.4/r_shepard/celery.py
--rw-r--r--   0        0        0     4252 2024-05-07 13:26:50.170216 r_shepard-0.1.4/r_shepard/settings.py
--rw-r--r--   0        0        0     1983 2024-04-26 08:33:25.063331 r_shepard-0.1.4/r_shepard/tests/test_models.py
--rw-r--r--   0        0        0     1549 2024-04-30 14:46:22.169959 r_shepard-0.1.4/r_shepard/tests/test_views.py
--rw-r--r--   0        0        0     2275 2024-04-30 14:28:56.240315 r_shepard-0.1.4/r_shepard/tests/utils.py
--rw-r--r--   0        0        0     2527 2024-04-23 09:40:06.216686 r_shepard-0.1.4/r_shepard/urls.py
--rw-r--r--   0        0        0      395 2024-04-22 08:53:11.183304 r_shepard-0.1.4/r_shepard/wsgi.py
--rw-r--r--   0        0        0     4343 1970-01-01 00:00:00.000000 r_shepard-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3517 2024-05-07 13:27:13.812834 r_shepard-0.1.5/README.md
+-rwxr-xr-x   0        0        0      666 2024-05-01 08:42:22.525077 r_shepard-0.1.5/manage.py
+-rw-r--r--   0        0        0      744 2024-05-07 13:36:52.222687 r_shepard-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      174 2024-05-06 20:18:43.831721 r_shepard-0.1.5/r_shepard/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-06 21:14:06.784472 r_shepard-0.1.5/r_shepard/api/__init__.py
+-rw-r--r--   0        0        0     3231 2024-05-07 10:03:25.055844 r_shepard-0.1.5/r_shepard/api/admin.py
+-rw-r--r--   0        0        0      457 2024-05-07 10:02:03.501832 r_shepard-0.1.5/r_shepard/api/apps.py
+-rw-r--r--   0        0        0      179 2024-05-06 21:14:06.784472 r_shepard-0.1.5/r_shepard/api/appy.py
+-rw-r--r--   0        0        0     1137 2024-05-07 10:01:34.041125 r_shepard-0.1.5/r_shepard/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      442 2024-05-07 10:01:34.041125 r_shepard-0.1.5/r_shepard/api/migrations/0002_project_is_active.py
+-rw-r--r--   0        0        0      505 2024-05-07 10:01:34.041125 r_shepard-0.1.5/r_shepard/api/migrations/0003_project_url.py
+-rw-r--r--   0        0        0      460 2024-05-07 10:01:34.041125 r_shepard-0.1.5/r_shepard/api/migrations/0004_project_rstudio_version.py
+-rw-r--r--   0        0        0     1103 2024-05-07 10:01:34.042125 r_shepard-0.1.5/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py
+-rw-r--r--   0        0        0     3210 2024-05-07 10:01:34.042125 r_shepard-0.1.5/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py
+-rw-r--r--   0        0        0      491 2024-05-07 10:01:34.043125 r_shepard-0.1.5/r_shepard/api/migrations/0007_alter_container_container_id.py
+-rw-r--r--   0        0        0     1688 2024-04-22 08:54:16.989356 r_shepard-0.1.5/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py
+-rw-r--r--   0        0        0      506 2024-05-07 10:01:34.043125 r_shepard-0.1.5/r_shepard/api/migrations/0009_alter_container_port.py
+-rw-r--r--   0        0        0      479 2024-05-07 10:01:34.043125 r_shepard-0.1.5/r_shepard/api/migrations/0010_alter_container_port.py
+-rw-r--r--   0        0        0      518 2024-05-07 10:01:34.043125 r_shepard-0.1.5/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py
+-rw-r--r--   0        0        0      586 2024-04-23 09:28:07.929488 r_shepard-0.1.5/r_shepard/api/migrations/0012_project_slug.py
+-rw-r--r--   0        0        0      656 2024-04-23 11:30:47.550693 r_shepard-0.1.5/r_shepard/api/migrations/0013_remove_project_password_container_password.py
+-rw-r--r--   0        0        0      541 2024-04-24 10:26:22.152733 r_shepard-0.1.5/r_shepard/api/migrations/0014_project_max_containers.py
+-rw-r--r--   0        0        0      918 2024-04-24 13:21:19.864083 r_shepard-0.1.5/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py
+-rw-r--r--   0        0        0     1381 2024-04-24 13:32:06.450029 r_shepard-0.1.5/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-20 15:09:46.014593 r_shepard-0.1.5/r_shepard/api/migrations/__init__.py
+-rw-r--r--   0        0        0     5512 2024-05-07 10:02:03.501832 r_shepard-0.1.5/r_shepard/api/models.py
+-rw-r--r--   0        0        0     4346 2024-05-07 10:04:34.289600 r_shepard-0.1.5/r_shepard/api/podman.py
+-rw-r--r--   0        0        0     3104 2024-05-07 09:58:12.404696 r_shepard-0.1.5/r_shepard/api/static/custom.css
+-rw-r--r--   0        0        0    48101 2024-04-22 17:57:33.717054 r_shepard-0.1.5/r_shepard/api/static/htmx.min.js
+-rw-r--r--   0        0        0    82210 2024-04-22 16:54:30.950446 r_shepard-0.1.5/r_shepard/api/static/pico.blue.min.css
+-rw-r--r--   0        0        0    74999 2024-04-23 06:39:38.438525 r_shepard-0.1.5/r_shepard/api/static/pico.colors.min.css
+-rw-r--r--   0        0        0     2982 2024-04-23 09:15:45.253107 r_shepard-0.1.5/r_shepard/api/tailscale.py
+-rw-r--r--   0        0        0     1397 2024-04-25 07:52:49.580151 r_shepard-0.1.5/r_shepard/api/tasks.py
+-rw-r--r--   0        0        0     5807 2024-05-07 10:02:03.502833 r_shepard-0.1.5/r_shepard/api/views.py
+-rw-r--r--   0        0        0      395 2024-04-26 07:51:03.905968 r_shepard-0.1.5/r_shepard/asgi.py
+-rw-r--r--   0        0        0      226 2024-04-26 08:04:10.741465 r_shepard-0.1.5/r_shepard/celery.py
+-rw-r--r--   0        0        0     4324 2024-05-07 13:36:39.120077 r_shepard-0.1.5/r_shepard/settings.py
+-rw-r--r--   0        0        0     1983 2024-04-26 08:33:25.063331 r_shepard-0.1.5/r_shepard/tests/test_models.py
+-rw-r--r--   0        0        0     1549 2024-04-30 14:46:22.169959 r_shepard-0.1.5/r_shepard/tests/test_views.py
+-rw-r--r--   0        0        0     2275 2024-04-30 14:28:56.240315 r_shepard-0.1.5/r_shepard/tests/utils.py
+-rw-r--r--   0        0        0     2527 2024-04-23 09:40:06.216686 r_shepard-0.1.5/r_shepard/urls.py
+-rw-r--r--   0        0        0      395 2024-04-22 08:53:11.183304 r_shepard-0.1.5/r_shepard/wsgi.py
+-rw-r--r--   0        0        0     4343 1970-01-01 00:00:00.000000 r_shepard-0.1.5/PKG-INFO
```

### Comparing `r_shepard-0.1.4/README.md` & `r_shepard-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/manage.py` & `r_shepard-0.1.5/manage.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/pyproject.toml` & `r_shepard-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 packages = [{ include = "r_shepard", from = "." }, { include = "manage.py" }]
 name = "r-shepard"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["linozen <linus@sehn.dev>"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `r_shepard-0.1.4/r_shepard/api/admin.py` & `r_shepard-0.1.5/r_shepard/api/admin.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/migrations/0001_initial.py` & `r_shepard-0.1.5/r_shepard/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py` & `r_shepard-0.1.5/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py` & `r_shepard-0.1.5/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py` & `r_shepard-0.1.5/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py` & `r_shepard-0.1.5/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/migrations/0012_project_slug.py` & `r_shepard-0.1.5/r_shepard/api/migrations/0012_project_slug.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/migrations/0013_remove_project_password_container_password.py` & `r_shepard-0.1.5/r_shepard/api/migrations/0013_remove_project_password_container_password.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/migrations/0014_project_max_containers.py` & `r_shepard-0.1.5/r_shepard/api/migrations/0014_project_max_containers.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py` & `r_shepard-0.1.5/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py` & `r_shepard-0.1.5/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/models.py` & `r_shepard-0.1.5/r_shepard/api/models.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/podman.py` & `r_shepard-0.1.5/r_shepard/api/podman.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/static/custom.css` & `r_shepard-0.1.5/r_shepard/api/static/custom.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/static/htmx.min.js` & `r_shepard-0.1.5/r_shepard/api/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/static/pico.blue.min.css` & `r_shepard-0.1.5/r_shepard/api/static/pico.blue.min.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/static/pico.colors.min.css` & `r_shepard-0.1.5/r_shepard/api/static/pico.colors.min.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/tailscale.py` & `r_shepard-0.1.5/r_shepard/api/tailscale.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/tasks.py` & `r_shepard-0.1.5/r_shepard/api/tasks.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/api/views.py` & `r_shepard-0.1.5/r_shepard/api/views.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/settings.py` & `r_shepard-0.1.5/r_shepard/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = "django-insecure-yc+#%@i2_hyrl1ut+c-9#ejwrv6(cv2de=-2+dv375a+oal*n7"
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
-ALLOWED_HOSTS = os.getenv('ALLOWED_HOSTS', '').split(',')
+ALLOWED_HOSTS = os.getenv("ALLOWED_HOSTS", "").split(",")
+CSRF_TRUSTED_ORIGINS = os.getenv("CSRF_TRUSTED_ORIGINS", "").split(",")
 
 LOGIN_URL = "two_factor:login"
 
 # this one is optional
 LOGIN_REDIRECT_URL = "two_factor:profile"
 
 # Application definition
```

### Comparing `r_shepard-0.1.4/r_shepard/tests/test_models.py` & `r_shepard-0.1.5/r_shepard/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/tests/test_views.py` & `r_shepard-0.1.5/r_shepard/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/tests/utils.py` & `r_shepard-0.1.5/r_shepard/tests/utils.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/r_shepard/urls.py` & `r_shepard-0.1.5/r_shepard/urls.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.4/PKG-INFO` & `r_shepard-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r-shepard
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: GPL-3.0
 Author: linozen
 Author-email: linus@sehn.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

