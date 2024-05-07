# Comparing `tmp/r_shepard-0.1.2.tar.gz` & `tmp/r_shepard-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r_shepard-0.1.2.tar", max compression
+gzip compressed data, was "r_shepard-0.1.3.tar", max compression
```

## Comparing `r_shepard-0.1.2.tar` & `r_shepard-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,43 @@
--rw-r--r--   0        0        0     2351 2024-04-26 08:04:27.931471 r_shepard-0.1.2/README.md
--rwxr-xr-x   0        0        0      666 2024-04-26 07:52:56.307083 r_shepard-0.1.2/manage.py
--rw-r--r--   0        0        0      669 2024-04-26 08:05:59.512499 r_shepard-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      174 2024-04-25 07:52:12.024837 r_shepard-0.1.2/r_shepard/__init__.py
--rw-r--r--   0        0        0      276 2024-04-23 15:09:26.819096 r_shepard-0.1.2/r_shepard/api/admin.py
--rw-r--r--   0        0        0      149 2024-04-23 15:10:07.254460 r_shepard-0.1.2/r_shepard/api/apps.py
--rw-r--r--   0        0        0     1137 2024-04-20 16:40:07.830596 r_shepard-0.1.2/r_shepard/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      442 2024-04-20 17:08:30.708782 r_shepard-0.1.2/r_shepard/api/migrations/0002_project_is_active.py
--rw-r--r--   0        0        0      505 2024-04-20 17:39:58.221267 r_shepard-0.1.2/r_shepard/api/migrations/0003_project_url.py
--rw-r--r--   0        0        0      460 2024-04-20 17:49:45.047866 r_shepard-0.1.2/r_shepard/api/migrations/0004_project_rstudio_version.py
--rw-r--r--   0        0        0     1103 2024-04-21 17:44:57.288648 r_shepard-0.1.2/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py
--rw-r--r--   0        0        0     3210 2024-04-21 18:32:44.456273 r_shepard-0.1.2/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py
--rw-r--r--   0        0        0      491 2024-04-22 05:25:57.373534 r_shepard-0.1.2/r_shepard/api/migrations/0007_alter_container_container_id.py
--rw-r--r--   0        0        0     1688 2024-04-22 08:54:16.989356 r_shepard-0.1.2/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py
--rw-r--r--   0        0        0      506 2024-04-22 07:28:12.933948 r_shepard-0.1.2/r_shepard/api/migrations/0009_alter_container_port.py
--rw-r--r--   0        0        0      479 2024-04-22 08:58:14.828153 r_shepard-0.1.2/r_shepard/api/migrations/0010_alter_container_port.py
--rw-r--r--   0        0        0      518 2024-04-22 08:59:48.236196 r_shepard-0.1.2/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py
--rw-r--r--   0        0        0      586 2024-04-23 09:28:07.929488 r_shepard-0.1.2/r_shepard/api/migrations/0012_project_slug.py
--rw-r--r--   0        0        0      656 2024-04-23 11:30:47.550693 r_shepard-0.1.2/r_shepard/api/migrations/0013_remove_project_password_container_password.py
--rw-r--r--   0        0        0      541 2024-04-24 10:26:22.152733 r_shepard-0.1.2/r_shepard/api/migrations/0014_project_max_containers.py
--rw-r--r--   0        0        0      918 2024-04-24 13:21:19.864083 r_shepard-0.1.2/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py
--rw-r--r--   0        0        0     1381 2024-04-24 13:32:06.450029 r_shepard-0.1.2/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py
--rw-r--r--   0        0        0        0 2024-04-20 15:09:46.014593 r_shepard-0.1.2/r_shepard/api/migrations/__init__.py
--rw-r--r--   0        0        0     5069 2024-04-25 07:52:12.024837 r_shepard-0.1.2/r_shepard/api/models.py
--rw-r--r--   0        0        0     4346 2024-04-25 07:49:10.152645 r_shepard-0.1.2/r_shepard/api/podman.py
--rw-r--r--   0        0        0     2213 2024-04-25 07:47:41.407870 r_shepard-0.1.2/r_shepard/api/static/custom.css
--rw-r--r--   0        0        0    48101 2024-04-22 17:57:33.717054 r_shepard-0.1.2/r_shepard/api/static/htmx.min.js
--rw-r--r--   0        0        0    82210 2024-04-22 16:54:30.950446 r_shepard-0.1.2/r_shepard/api/static/pico.blue.min.css
--rw-r--r--   0        0        0    74999 2024-04-23 06:39:38.438525 r_shepard-0.1.2/r_shepard/api/static/pico.colors.min.css
--rw-r--r--   0        0        0     2982 2024-04-23 09:15:45.253107 r_shepard-0.1.2/r_shepard/api/tailscale.py
--rw-r--r--   0        0        0     1397 2024-04-25 07:52:49.580151 r_shepard-0.1.2/r_shepard/api/tasks.py
--rw-r--r--   0        0        0       60 2024-04-26 07:21:34.490123 r_shepard-0.1.2/r_shepard/api/tests.py
--rw-r--r--   0        0        0     5402 2024-04-25 07:51:40.716987 r_shepard-0.1.2/r_shepard/api/views.py
--rw-r--r--   0        0        0      395 2024-04-26 07:51:03.905968 r_shepard-0.1.2/r_shepard/asgi.py
--rw-r--r--   0        0        0      226 2024-04-26 08:04:10.741465 r_shepard-0.1.2/r_shepard/celery.py
--rw-r--r--   0        0        0     4181 2024-04-26 08:04:10.741465 r_shepard-0.1.2/r_shepard/settings.py
--rw-r--r--   0        0        0     2527 2024-04-23 09:40:06.216686 r_shepard-0.1.2/r_shepard/urls.py
--rw-r--r--   0        0        0      395 2024-04-22 08:53:11.183304 r_shepard-0.1.2/r_shepard/wsgi.py
--rw-r--r--   0        0        0     3177 1970-01-01 00:00:00.000000 r_shepard-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2420 2024-05-01 08:58:26.257040 r_shepard-0.1.3/README.md
+-rwxr-xr-x   0        0        0      666 2024-05-01 08:42:22.525077 r_shepard-0.1.3/manage.py
+-rw-r--r--   0        0        0      744 2024-05-07 10:05:12.141574 r_shepard-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      174 2024-05-06 20:18:43.831721 r_shepard-0.1.3/r_shepard/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-06 21:14:06.784472 r_shepard-0.1.3/r_shepard/api/__init__.py
+-rw-r--r--   0        0        0     3231 2024-05-07 10:03:25.055844 r_shepard-0.1.3/r_shepard/api/admin.py
+-rw-r--r--   0        0        0      457 2024-05-07 10:02:03.501832 r_shepard-0.1.3/r_shepard/api/apps.py
+-rw-r--r--   0        0        0      179 2024-05-06 21:14:06.784472 r_shepard-0.1.3/r_shepard/api/appy.py
+-rw-r--r--   0        0        0     1137 2024-05-07 10:01:34.041125 r_shepard-0.1.3/r_shepard/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      442 2024-05-07 10:01:34.041125 r_shepard-0.1.3/r_shepard/api/migrations/0002_project_is_active.py
+-rw-r--r--   0        0        0      505 2024-05-07 10:01:34.041125 r_shepard-0.1.3/r_shepard/api/migrations/0003_project_url.py
+-rw-r--r--   0        0        0      460 2024-05-07 10:01:34.041125 r_shepard-0.1.3/r_shepard/api/migrations/0004_project_rstudio_version.py
+-rw-r--r--   0        0        0     1103 2024-05-07 10:01:34.042125 r_shepard-0.1.3/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py
+-rw-r--r--   0        0        0     3210 2024-05-07 10:01:34.042125 r_shepard-0.1.3/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py
+-rw-r--r--   0        0        0      491 2024-05-07 10:01:34.043125 r_shepard-0.1.3/r_shepard/api/migrations/0007_alter_container_container_id.py
+-rw-r--r--   0        0        0     1688 2024-04-22 08:54:16.989356 r_shepard-0.1.3/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py
+-rw-r--r--   0        0        0      506 2024-05-07 10:01:34.043125 r_shepard-0.1.3/r_shepard/api/migrations/0009_alter_container_port.py
+-rw-r--r--   0        0        0      479 2024-05-07 10:01:34.043125 r_shepard-0.1.3/r_shepard/api/migrations/0010_alter_container_port.py
+-rw-r--r--   0        0        0      518 2024-05-07 10:01:34.043125 r_shepard-0.1.3/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py
+-rw-r--r--   0        0        0      586 2024-04-23 09:28:07.929488 r_shepard-0.1.3/r_shepard/api/migrations/0012_project_slug.py
+-rw-r--r--   0        0        0      656 2024-04-23 11:30:47.550693 r_shepard-0.1.3/r_shepard/api/migrations/0013_remove_project_password_container_password.py
+-rw-r--r--   0        0        0      541 2024-04-24 10:26:22.152733 r_shepard-0.1.3/r_shepard/api/migrations/0014_project_max_containers.py
+-rw-r--r--   0        0        0      918 2024-04-24 13:21:19.864083 r_shepard-0.1.3/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py
+-rw-r--r--   0        0        0     1381 2024-04-24 13:32:06.450029 r_shepard-0.1.3/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-20 15:09:46.014593 r_shepard-0.1.3/r_shepard/api/migrations/__init__.py
+-rw-r--r--   0        0        0     5512 2024-05-07 10:02:03.501832 r_shepard-0.1.3/r_shepard/api/models.py
+-rw-r--r--   0        0        0     4346 2024-05-07 10:04:34.289600 r_shepard-0.1.3/r_shepard/api/podman.py
+-rw-r--r--   0        0        0     3104 2024-05-07 09:58:12.404696 r_shepard-0.1.3/r_shepard/api/static/custom.css
+-rw-r--r--   0        0        0    48101 2024-04-22 17:57:33.717054 r_shepard-0.1.3/r_shepard/api/static/htmx.min.js
+-rw-r--r--   0        0        0    82210 2024-04-22 16:54:30.950446 r_shepard-0.1.3/r_shepard/api/static/pico.blue.min.css
+-rw-r--r--   0        0        0    74999 2024-04-23 06:39:38.438525 r_shepard-0.1.3/r_shepard/api/static/pico.colors.min.css
+-rw-r--r--   0        0        0     2982 2024-04-23 09:15:45.253107 r_shepard-0.1.3/r_shepard/api/tailscale.py
+-rw-r--r--   0        0        0     1397 2024-04-25 07:52:49.580151 r_shepard-0.1.3/r_shepard/api/tasks.py
+-rw-r--r--   0        0        0     5807 2024-05-07 10:02:03.502833 r_shepard-0.1.3/r_shepard/api/views.py
+-rw-r--r--   0        0        0      395 2024-04-26 07:51:03.905968 r_shepard-0.1.3/r_shepard/asgi.py
+-rw-r--r--   0        0        0      226 2024-04-26 08:04:10.741465 r_shepard-0.1.3/r_shepard/celery.py
+-rw-r--r--   0        0        0     4208 2024-04-30 14:46:26.058059 r_shepard-0.1.3/r_shepard/settings.py
+-rw-r--r--   0        0        0     1983 2024-04-26 08:33:25.063331 r_shepard-0.1.3/r_shepard/tests/test_models.py
+-rw-r--r--   0        0        0     1549 2024-04-30 14:46:22.169959 r_shepard-0.1.3/r_shepard/tests/test_views.py
+-rw-r--r--   0        0        0     2275 2024-04-30 14:28:56.240315 r_shepard-0.1.3/r_shepard/tests/utils.py
+-rw-r--r--   0        0        0     2527 2024-04-23 09:40:06.216686 r_shepard-0.1.3/r_shepard/urls.py
+-rw-r--r--   0        0        0      395 2024-04-22 08:53:11.183304 r_shepard-0.1.3/r_shepard/wsgi.py
+-rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 r_shepard-0.1.3/PKG-INFO
```

### Comparing `r_shepard-0.1.2/README.md` & `r_shepard-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # r-shepard
 
+![Coverage Status](./coverage-badge.svg)
+
 Simple, self-hosted solution for collaborative (not real-time) R computing leveraging podman,
 RStudio, and Tailscale.
 
 Built with Django and HTMX.
 
 ## Develop
 
 First start the development environment:
 
 ```bash
 devenv up # starts redis, celery worker and celery beat
+run-tests # runs the tests
 ```
 
 Then start the Django development server:
 
 ```bash
 python manage.py runserver # This could also be done from your IDE / debugging environment
 ```
```

### Comparing `r_shepard-0.1.2/manage.py` & `r_shepard-0.1.3/manage.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/pyproject.toml` & `r_shepard-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 packages = [{ include = "r_shepard", from = "." }, { include = "manage.py" }]
 name = "r-shepard"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["linozen <linus@sehn.dev>"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -20,11 +20,13 @@
 
 [tool.poetry.scripts]
 r-shepard = "manage:main"
 
 [tool.poetry.group.dev.dependencies]
 djlint = "^1.34.1"
 bumpversion = "^0.6.0"
+coverage = "^7.5.0"
+genbadge = {extras = ["coverage"], version = "^1.1.1"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `r_shepard-0.1.2/r_shepard/api/migrations/0001_initial.py` & `r_shepard-0.1.3/r_shepard/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py` & `r_shepard-0.1.3/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py` & `r_shepard-0.1.3/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py` & `r_shepard-0.1.3/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py` & `r_shepard-0.1.3/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/migrations/0012_project_slug.py` & `r_shepard-0.1.3/r_shepard/api/migrations/0012_project_slug.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/migrations/0013_remove_project_password_container_password.py` & `r_shepard-0.1.3/r_shepard/api/migrations/0013_remove_project_password_container_password.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/migrations/0014_project_max_containers.py` & `r_shepard-0.1.3/r_shepard/api/migrations/0014_project_max_containers.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py` & `r_shepard-0.1.3/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py` & `r_shepard-0.1.3/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/models.py` & `r_shepard-0.1.3/r_shepard/api/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,63 +88,71 @@
 
     project = models.ForeignKey(
         Project,
         on_delete=models.CASCADE,
         related_name="containers",
         help_text="The project to which this container belongs.",
     )
+    container_id = models.CharField(
+        max_length=8,
+        default=generate_container_id,
+        verbose_name="Container ID",
+        help_text="The unique identifier of the container within the project.",
+    )
     image = models.CharField(
         default="rocker/rstudio",
         max_length=255,
         help_text="The name of the container image.",
     )
     tag = models.CharField(
         default="latest",
         max_length=255,
         help_text="The tag of the container image.",
     )
     password = models.CharField(
         max_length=255,
         help_text="Password for the RStudio Rocker container.",
     )
-    container_id = models.CharField(
-        max_length=8,
-        default=generate_container_id,
-        help_text="The unique identifier of the container within the project.",
-    )
     ram = models.PositiveIntegerField(
         default=2,
-        help_text="Amount of RAM in GB allocated for the container.",
+        verbose_name="RAM Allocation (GB)",
+        help_text="The maximum amount of RAM in GB the container can use. Will only take effect after restarting the container.",
     )
     cpus = models.PositiveIntegerField(
         default=2,
-        help_text="Number of CPUs allocated to the container.",
+        verbose_name="CPU Allocation",
+        help_text="The maximum number of CPU cores the container can use. Will only take effect after restarting the container.",
     )
     port = models.PositiveIntegerField(
         default=8787,
-        help_text="The host port on which the container's RStudio instance is accessible.",
+        verbose_name="Host Port",
+        help_text="The host port on which the container's RStudio instance is accessible locally.",
     )
     local_url = models.URLField(
         default="",
         max_length=1024,
+        verbose_name="Local URL",
         help_text="Local URL to access this container's RStudio instance",
     )
     tailscale_funnel_url = models.URLField(
         default="",
         max_length=1024,
+        verbose_name="Tailscale Funnel URL",
         help_text="Tailscale Funnel URL to access this container's RStudio instance from the web",
     )
     tailscale_serve_url = models.URLField(
         default="",
         null=True,
         max_length=1024,
+        verbose_name="Tailscale Serve URL",
         help_text="Tailscale Serve URL to access this container's RStudio instance from the tailnet",
     )
     is_running = models.BooleanField(
         default=False,
+        verbose_name="Running",
         help_text="Indicates whether the container is running",
     )
 
     def save(self, *args, **kwargs):
         if not check_password(self.password, self.__original_password):
             self.password = make_password(self.password)
         super().save(*args, **kwargs)
```

### Comparing `r_shepard-0.1.2/r_shepard/api/podman.py` & `r_shepard-0.1.3/r_shepard/api/podman.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/static/custom.css` & `r_shepard-0.1.3/r_shepard/api/static/custom.css`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+:root {
+  --pico-border-radius: 0.2rem;
+  --pico-font-size: 85%;
+  --pico-form-element-spacing-vertical: 0.3rem;
+  --pico-form-element-spacing-horizontal: 0.5rem;
+}
+
+h1 {
+  --pico-font-weight: 800;
+}
+
+.header-line {
+  display: inline-block;
+  margin-bottom: 20px;
+}
+
+.header-line h1,
+h2 {
+  display: inline;
+}
+
+.header-line a {
+  float: right;
+  margin-left: 10px;
+}
+
+button {
+  --pico-font-weight: 700;
+}
+
 .delete-button {
   --pico-background-color: var(--pico-color-red-500);
   --pico-border-color: var(--pico-color-red-500);
   --pico-color: var(--pico-primary-inverse);
   --pico-box-shadow: var(--pico-button-box-shadow, 0 0 0 rgba(0, 0, 0, 0));
   --pico-primary-hover-background: var(--pico-color-red-600);
   --pico-primary-hover-border: var(--pico-color-red-600);
@@ -19,22 +49,48 @@
   background-color: #f44336; /* Red */
   border: none;
   border-radius: 4px;
   margin: 10px 0;
   padding: 10px;
 }
 
+.project-info {
+  margin-right: 5px;
+}
+
 .action-button {
   display: flex;
   justify-content: center;
   align-items: center;
 }
 
+.container-list {
+  display: flex;
+  flex-wrap: wrap;
+  justify-content: start;
+}
+
 .container-card {
-  max-width: 600px;
+  width: 100%;
+}
+
+@media (min-width: 600px) {
+  .container-card {
+    width: calc(50% - 20px); /* Adjust for desired gap */
+    margin: 10px; /* Half of the gap */
+    box-sizing: border-box;
+  }
+}
+
+@media (min-width: 900px) {
+  .container-card {
+    width: calc(33.33% - 20px); /* Adjust for desired gap */
+    margin: 10px; /* Half of the gap */
+    box-sizing: border-box;
+  }
 }
 
 .container-title {
   font-size: 20px;
   margin-top: 4px;
   margin-bottom: 30px;
 }
@@ -45,20 +101,20 @@
   padding: 4px 8px;
   border-radius: 4px;
   margin-top: 16px;
   margin-bottom: 16px;
 }
 
 .open-button {
+  font-weight: 700;
   text-decoration: none;
   background-color: transparent;
   color: var(--pico-color-green-600);
-  padding: 2px 16px;
+  padding: 4px 12px;
   border-radius: 4px;
-  font-size: 16px;
   border: 2px solid var(--pico-color-green-600);
   cursor: pointer;
   text-align: center;
   display: flex;
   justify-content: center;
   align-items: center;
   max-height: 40px;
```

### Comparing `r_shepard-0.1.2/r_shepard/api/static/htmx.min.js` & `r_shepard-0.1.3/r_shepard/api/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/static/pico.blue.min.css` & `r_shepard-0.1.3/r_shepard/api/static/pico.blue.min.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/static/pico.colors.min.css` & `r_shepard-0.1.3/r_shepard/api/static/pico.colors.min.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/tailscale.py` & `r_shepard-0.1.3/r_shepard/api/tailscale.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/tasks.py` & `r_shepard-0.1.3/r_shepard/api/tasks.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/r_shepard/api/views.py` & `r_shepard-0.1.3/r_shepard/api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,19 @@
         cpus = int(request.POST.get("cpus"))
 
         # Calculate total resources used by all containers of the project
         total_ram = sum(container.ram for container in project.containers.all())
         total_cpus = sum(container.cpus for container in project.containers.all())
 
         # Check if the project has enough resources
+        if len(project.containers.all()) >= project.max_containers:
+            messages.error(request, "Maximum number of containers reached.")
+            return HttpResponseRedirect(reverse("project_detail", args=[project.pk]))
         if total_ram + ram > project.max_ram or total_cpus + cpus > project.max_cpus:
-            messages.error(request, "Not enough resources to create a new container.")
+            messages.error(request, "Not enough resources for this action.")
             return HttpResponseRedirect(reverse("project_detail", args=[project.pk]))
 
         # Create container instance with project and password
         container = Container.objects.create(
             project=project, password=password, ram=ram, cpus=cpus
         )
 
@@ -76,16 +79,20 @@
         return HttpResponseRedirect(reverse("project_detail", args=[project.pk]))
 
 
 class StartContainerView(OTPRequiredMixin, View):
     def post(self, request, *args, **kwargs):
         project = get_object_or_404(Project, pk=kwargs["project_pk"])
         container = get_object_or_404(Container, pk=kwargs["container_pk"])
-        if not is_container_running(project, container):
-            start_container(project, container)
+        try:
+            if not is_container_running(project, container):
+                start_container(project, container)
+        except PodmanError as e:
+            messages.error(request, str(e))
+            return HttpResponseRedirect(reverse("project_detail", args=[project.pk]))
         container.is_running = True
         container.save()
 
         html = render_to_string("container_list.html", {"project": project})
         return HttpResponse(html)
```

### Comparing `r_shepard-0.1.2/r_shepard/settings.py` & `r_shepard-0.1.3/r_shepard/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 # Database
 # https://docs.djangoproject.com/en/5.0/ref/settings/#databases
 
 DATABASES = {
     "default": {
         "ENGINE": "django.db.backends.sqlite3",
-        "NAME": BASE_DIR / "db.sqlite3",
+        "NAME": os.environ.get("DB_PATH", BASE_DIR / "db.sqlite3"),
     }
 }
 
 
 # Password validation
 # https://docs.djangoproject.com/en/5.0/ref/settings/#auth-password-validators
```

### Comparing `r_shepard-0.1.2/r_shepard/urls.py` & `r_shepard-0.1.3/r_shepard/urls.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.2/PKG-INFO` & `r_shepard-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r-shepard
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: GPL-3.0
 Author: linozen
 Author-email: linus@sehn.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -19,25 +19,28 @@
 Requires-Dist: phonenumberslite (>=8.13.35,<9.0.0)
 Requires-Dist: podman (>=5.0.0,<6.0.0)
 Requires-Dist: redis (>=5.0.4,<6.0.0)
 Description-Content-Type: text/markdown
 
 # r-shepard
 
+![Coverage Status](./coverage-badge.svg)
+
 Simple, self-hosted solution for collaborative (not real-time) R computing leveraging podman,
 RStudio, and Tailscale.
 
 Built with Django and HTMX.
 
 ## Develop
 
 First start the development environment:
 
 ```bash
 devenv up # starts redis, celery worker and celery beat
+run-tests # runs the tests
 ```
 
 Then start the Django development server:
 
 ```bash
 python manage.py runserver # This could also be done from your IDE / debugging environment
 ```
```

