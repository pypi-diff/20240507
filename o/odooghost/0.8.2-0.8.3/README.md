# Comparing `tmp/odooghost-0.8.2.tar.gz` & `tmp/odooghost-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odooghost-0.8.2.tar", max compression
+gzip compressed data, was "odooghost-0.8.3.tar", max compression
```

## Comparing `odooghost-0.8.2.tar` & `odooghost-0.8.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1069 2024-05-01 11:12:19.041932 odooghost-0.8.2/LICENSE
--rw-r--r--   0        0        0     1967 2024-05-01 11:12:19.041932 odooghost-0.8.2/README.md
--rw-r--r--   0        0        0      369 2024-05-01 11:13:00.706432 odooghost-0.8.2/odooghost/__init__.py
--rw-r--r--   0        0        0       94 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/__main__.py
--rw-r--r--   0        0        0      127 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/cli/__init__.py
--rw-r--r--   0        0        0      451 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/cli/config.py
--rw-r--r--   0        0        0     1861 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/cli/root.py
--rw-r--r--   0        0        0       42 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/cli/stack/__init__.py
--rw-r--r--   0        0        0      959 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/cli/stack/config.py
--rw-r--r--   0        0        0     9765 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/cli/stack/data.py
--rw-r--r--   0        0        0    13134 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/cli/stack/root.py
--rw-r--r--   0        0        0      271 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/config/__init__.py
--rw-r--r--   0        0        0     4440 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/config/addons.py
--rw-r--r--   0        0        0      267 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/config/app.py
--rw-r--r--   0        0        0     2445 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/config/dependency.py
--rw-r--r--   0        0        0     2082 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/config/service.py
--rw-r--r--   0        0        0     2854 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/config/stack.py
--rw-r--r--   0        0        0      789 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/constant.py
--rw-r--r--   0        0        0     9501 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/container.py
--rw-r--r--   0        0        0     7516 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/context.py
--rw-r--r--   0        0        0     1139 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/exceptions.py
--rw-r--r--   0        0        0      585 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/filters.py
--rw-r--r--   0        0        0     3702 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/git.py
--rw-r--r--   0        0        0     1111 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/logger.py
--rw-r--r--   0        0        0      466 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/renderer.py
--rw-r--r--   0        0        0       63 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/services/__init__.py
--rw-r--r--   0        0        0    14691 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/services/base.py
--rw-r--r--   0        0        0     3972 2024-05-01 11:12:19.041932 odooghost-0.8.2/odooghost/services/db.py
--rw-r--r--   0        0        0      102 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/services/odoo/__init__.py
--rw-r--r--   0        0        0     3756 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/services/odoo/addons.py
--rw-r--r--   0        0        0     4838 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/services/odoo/service.py
--rw-r--r--   0        0        0    10382 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/stack.py
--rw-r--r--   0        0        0     1710 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/templates/Dockerfile.j2
--rw-r--r--   0        0        0      580 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/types.py
--rw-r--r--   0        0        0       93 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/utils/__init__.py
--rw-r--r--   0        0        0      790 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/utils/autocomplete.py
--rw-r--r--   0        0        0      993 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/utils/exec.py
--rw-r--r--   0        0        0     2159 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/utils/misc.py
--rw-r--r--   0        0        0     3914 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/utils/progress_stream.py
--rw-r--r--   0        0        0      884 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/utils/signals.py
--rw-r--r--   0        0        0     2567 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/utils/stream.py
--rw-r--r--   0        0        0     1516 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/utils/sync_to_async.py
--rw-r--r--   0        0        0        0 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/web/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/web/api/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/web/api/query/__init__.py
--rw-r--r--   0        0        0      305 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/web/api/query/dashboard.py
--rw-r--r--   0        0        0     1156 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/web/api/query/stack.py
--rw-r--r--   0        0        0      233 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/web/api/schema.py
--rw-r--r--   0        0        0     2578 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/web/api/schema_types.py
--rw-r--r--   0        0        0     1679 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/web/api/subscription.py
--rw-r--r--   0        0        0     1579 2024-05-01 11:12:19.045932 odooghost-0.8.2/odooghost/web/application.py
--rw-r--r--   0        0        0     8986 2024-05-01 11:12:58.806409 odooghost-0.8.2/odooghost/web/dist/android-chrome-192x192.png
--rw-r--r--   0        0        0    13346 2024-05-01 11:12:58.806409 odooghost-0.8.2/odooghost/web/dist/android-chrome-512x512.png
--rw-r--r--   0        0        0     8702 2024-05-01 11:12:58.806409 odooghost-0.8.2/odooghost/web/dist/apple-touch-icon.png
--rw-r--r--   0        0        0      636 2024-05-01 11:12:59.074413 odooghost-0.8.2/odooghost/web/dist/assets/ContainersView-CQGACCyA.js
--rw-r--r--   0        0        0     1162 2024-05-01 11:12:59.074413 odooghost-0.8.2/odooghost/web/dist/assets/DashboardView-DaNsKC6f.js
--rw-r--r--   0        0        0      275 2024-05-01 11:12:59.070413 odooghost-0.8.2/odooghost/web/dist/assets/SettingsView-BStxbQD1.js
--rw-r--r--   0        0        0      286 2024-05-01 11:12:59.070413 odooghost-0.8.2/odooghost/web/dist/assets/StackItemContainersView-cTSpFQBD.js
--rw-r--r--   0        0        0      611 2024-05-01 11:12:59.074413 odooghost-0.8.2/odooghost/web/dist/assets/StackItemIndexView-CYLOsCmC.js
--rw-r--r--   0        0        0      280 2024-05-01 11:12:59.070413 odooghost-0.8.2/odooghost/web/dist/assets/StackItemLogsView-D5NV0km8.js
--rw-r--r--   0        0        0      284 2024-05-01 11:12:59.074413 odooghost-0.8.2/odooghost/web/dist/assets/StackItemServicesView-CNydrgOE.js
--rw-r--r--   0        0        0     5418 2024-05-01 11:12:59.070413 odooghost-0.8.2/odooghost/web/dist/assets/StackItemView-BtdLvO3L.js
--rw-r--r--   0        0        0     2081 2024-05-01 11:12:59.074413 odooghost-0.8.2/odooghost/web/dist/assets/StackView-C0gt5mfw.js
--rw-r--r--   0        0        0      272 2024-05-01 11:12:59.070413 odooghost-0.8.2/odooghost/web/dist/assets/UsageView-NG-QxEdS.js
--rw-r--r--   0        0        0     2082 2024-05-01 11:12:59.074413 odooghost-0.8.2/odooghost/web/dist/assets/VContainers-CS_dVxEN.js
--rw-r--r--   0        0        0     1206 2024-05-01 11:12:59.070413 odooghost-0.8.2/odooghost/web/dist/assets/VHeader-B9IRV133.js
--rw-r--r--   0        0        0      418 2024-05-01 11:12:59.074413 odooghost-0.8.2/odooghost/web/dist/assets/VStat-AcXitZbU.js
--rw-r--r--   0        0        0     1744 2024-05-01 11:12:59.074413 odooghost-0.8.2/odooghost/web/dist/assets/VWarningAlert-B-onwvMS.js
--rw-r--r--   0        0        0      721 2024-05-01 11:12:59.070413 odooghost-0.8.2/odooghost/web/dist/assets/VWarningAlert-DWujdwvy.css
--rw-r--r--   0        0        0      310 2024-05-01 11:12:59.070413 odooghost-0.8.2/odooghost/web/dist/assets/constant-DWkFHeG6.js
--rw-r--r--   0        0        0    26276 2024-05-01 11:12:59.070413 odooghost-0.8.2/odooghost/web/dist/assets/index-BCu_nn1R.css
--rw-r--r--   0        0        0   345242 2024-05-01 11:12:59.074413 odooghost-0.8.2/odooghost/web/dist/assets/index-aZbCTR1y.js
--rw-r--r--   0        0        0      564 2024-05-01 11:12:59.070413 odooghost-0.8.2/odooghost/web/dist/assets/stack-FDe_L0Se.js
--rw-r--r--   0        0        0      575 2024-05-01 11:12:58.806409 odooghost-0.8.2/odooghost/web/dist/favicon-16x16.png
--rw-r--r--   0        0        0     1199 2024-05-01 11:12:58.806409 odooghost-0.8.2/odooghost/web/dist/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2024-05-01 11:12:58.806409 odooghost-0.8.2/odooghost/web/dist/favicon.ico
--rw-r--r--   0        0        0      787 2024-05-01 11:12:59.074413 odooghost-0.8.2/odooghost/web/dist/index.html
--rw-r--r--   0        0        0     3531 2024-05-01 11:12:58.806409 odooghost-0.8.2/odooghost/web/dist/logo.svg
--rw-r--r--   0        0        0      286 2024-05-01 11:12:58.806409 odooghost-0.8.2/odooghost/web/dist/site.webmanifest
--rw-r--r--   0        0        0     3811 2024-05-01 11:13:00.706432 odooghost-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 odooghost-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-07 11:39:37.206381 odooghost-0.8.3/LICENSE
+-rw-r--r--   0        0        0     1967 2024-05-07 11:39:37.206381 odooghost-0.8.3/README.md
+-rw-r--r--   0        0        0      369 2024-05-07 11:40:15.002879 odooghost-0.8.3/odooghost/__init__.py
+-rw-r--r--   0        0        0       94 2024-05-07 11:39:37.206381 odooghost-0.8.3/odooghost/__main__.py
+-rw-r--r--   0        0        0      127 2024-05-07 11:39:37.206381 odooghost-0.8.3/odooghost/cli/__init__.py
+-rw-r--r--   0        0        0      451 2024-05-07 11:39:37.206381 odooghost-0.8.3/odooghost/cli/config.py
+-rw-r--r--   0        0        0     1861 2024-05-07 11:39:37.206381 odooghost-0.8.3/odooghost/cli/root.py
+-rw-r--r--   0        0        0       42 2024-05-07 11:39:37.206381 odooghost-0.8.3/odooghost/cli/stack/__init__.py
+-rw-r--r--   0        0        0      959 2024-05-07 11:39:37.206381 odooghost-0.8.3/odooghost/cli/stack/config.py
+-rw-r--r--   0        0        0     9765 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/cli/stack/data.py
+-rw-r--r--   0        0        0    13134 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/cli/stack/root.py
+-rw-r--r--   0        0        0      271 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/config/__init__.py
+-rw-r--r--   0        0        0     4440 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/config/addons.py
+-rw-r--r--   0        0        0      267 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/config/app.py
+-rw-r--r--   0        0        0     2445 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/config/dependency.py
+-rw-r--r--   0        0        0     2082 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/config/service.py
+-rw-r--r--   0        0        0     2854 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/config/stack.py
+-rw-r--r--   0        0        0      789 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/constant.py
+-rw-r--r--   0        0        0     9501 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/container.py
+-rw-r--r--   0        0        0     7516 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/context.py
+-rw-r--r--   0        0        0     1139 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/exceptions.py
+-rw-r--r--   0        0        0      585 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/filters.py
+-rw-r--r--   0        0        0     3702 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/git.py
+-rw-r--r--   0        0        0     1111 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/logger.py
+-rw-r--r--   0        0        0      466 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/renderer.py
+-rw-r--r--   0        0        0       63 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/services/__init__.py
+-rw-r--r--   0        0        0    14691 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/services/base.py
+-rw-r--r--   0        0        0     3972 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/services/db.py
+-rw-r--r--   0        0        0      102 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/services/odoo/__init__.py
+-rw-r--r--   0        0        0     3756 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/services/odoo/addons.py
+-rw-r--r--   0        0        0     4838 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/services/odoo/service.py
+-rw-r--r--   0        0        0    10382 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/stack.py
+-rw-r--r--   0        0        0     1710 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/templates/Dockerfile.j2
+-rw-r--r--   0        0        0      580 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/types.py
+-rw-r--r--   0        0        0       93 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/utils/__init__.py
+-rw-r--r--   0        0        0      790 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/utils/autocomplete.py
+-rw-r--r--   0        0        0      993 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/utils/exec.py
+-rw-r--r--   0        0        0     2159 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/utils/misc.py
+-rw-r--r--   0        0        0     3914 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/utils/progress_stream.py
+-rw-r--r--   0        0        0      884 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/utils/signals.py
+-rw-r--r--   0        0        0     2567 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/utils/stream.py
+-rw-r--r--   0        0        0     1516 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/utils/sync_to_async.py
+-rw-r--r--   0        0        0        0 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/web/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/web/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/web/api/query/__init__.py
+-rw-r--r--   0        0        0      305 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/web/api/query/dashboard.py
+-rw-r--r--   0        0        0     1156 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/web/api/query/stack.py
+-rw-r--r--   0        0        0      233 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/web/api/schema.py
+-rw-r--r--   0        0        0     2578 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/web/api/schema_types.py
+-rw-r--r--   0        0        0     1679 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/web/api/subscription.py
+-rw-r--r--   0        0        0     1579 2024-05-07 11:39:37.210381 odooghost-0.8.3/odooghost/web/application.py
+-rw-r--r--   0        0        0     8986 2024-05-07 11:40:13.182856 odooghost-0.8.3/odooghost/web/dist/android-chrome-192x192.png
+-rw-r--r--   0        0        0    13346 2024-05-07 11:40:13.186856 odooghost-0.8.3/odooghost/web/dist/android-chrome-512x512.png
+-rw-r--r--   0        0        0     8702 2024-05-07 11:40:13.186856 odooghost-0.8.3/odooghost/web/dist/apple-touch-icon.png
+-rw-r--r--   0        0        0      636 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/ContainersView-BE5deGhZ.js
+-rw-r--r--   0        0        0     1162 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/DashboardView-D7R6tEBr.js
+-rw-r--r--   0        0        0      275 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/SettingsView-BAzeCNyE.js
+-rw-r--r--   0        0        0      286 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/StackItemContainersView-Dni9Qael.js
+-rw-r--r--   0        0        0      611 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/StackItemIndexView-Bi3wNjjv.js
+-rw-r--r--   0        0        0      280 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/StackItemLogsView-QMXp-UnQ.js
+-rw-r--r--   0        0        0      284 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/StackItemServicesView-CFfNOwHX.js
+-rw-r--r--   0        0        0     5418 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/StackItemView-NU6ZoWkH.js
+-rw-r--r--   0        0        0     2081 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/StackView-B3ysXA8u.js
+-rw-r--r--   0        0        0      272 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/UsageView-DaVpkoWP.js
+-rw-r--r--   0        0        0     2082 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/VContainers-Dk3P-tJN.js
+-rw-r--r--   0        0        0     1206 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/VHeader-DE-7o50y.js
+-rw-r--r--   0        0        0      418 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/VStat-BuNxdvtd.js
+-rw-r--r--   0        0        0     1744 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/VWarningAlert-D3_O5a8o.js
+-rw-r--r--   0        0        0      721 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/VWarningAlert-DWujdwvy.css
+-rw-r--r--   0        0        0      310 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/constant-DWkFHeG6.js
+-rw-r--r--   0        0        0    26276 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/index-BCu_nn1R.css
+-rw-r--r--   0        0        0   345242 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/index-B_2Yopjn.js
+-rw-r--r--   0        0        0      564 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/assets/stack-ooq4hns8.js
+-rw-r--r--   0        0        0      575 2024-05-07 11:40:13.202856 odooghost-0.8.3/odooghost/web/dist/favicon-16x16.png
+-rw-r--r--   0        0        0     1199 2024-05-07 11:40:13.218857 odooghost-0.8.3/odooghost/web/dist/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2024-05-07 11:40:13.218857 odooghost-0.8.3/odooghost/web/dist/favicon.ico
+-rw-r--r--   0        0        0      787 2024-05-07 11:40:13.470860 odooghost-0.8.3/odooghost/web/dist/index.html
+-rw-r--r--   0        0        0     3531 2024-05-07 11:40:13.218857 odooghost-0.8.3/odooghost/web/dist/logo.svg
+-rw-r--r--   0        0        0      286 2024-05-07 11:40:13.218857 odooghost-0.8.3/odooghost/web/dist/site.webmanifest
+-rw-r--r--   0        0        0     3811 2024-05-07 11:40:15.002879 odooghost-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 odooghost-0.8.3/PKG-INFO
```

### Comparing `odooghost-0.8.2/LICENSE` & `odooghost-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/README.md` & `odooghost-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/cli/root.py` & `odooghost-0.8.3/odooghost/cli/root.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/cli/stack/config.py` & `odooghost-0.8.3/odooghost/cli/stack/config.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/cli/stack/data.py` & `odooghost-0.8.3/odooghost/cli/stack/data.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/cli/stack/root.py` & `odooghost-0.8.3/odooghost/cli/stack/root.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/config/addons.py` & `odooghost-0.8.3/odooghost/config/addons.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/config/dependency.py` & `odooghost-0.8.3/odooghost/config/dependency.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/config/service.py` & `odooghost-0.8.3/odooghost/config/service.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/config/stack.py` & `odooghost-0.8.3/odooghost/config/stack.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/constant.py` & `odooghost-0.8.3/odooghost/constant.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/container.py` & `odooghost-0.8.3/odooghost/container.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/context.py` & `odooghost-0.8.3/odooghost/context.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/exceptions.py` & `odooghost-0.8.3/odooghost/exceptions.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/filters.py` & `odooghost-0.8.3/odooghost/filters.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/git.py` & `odooghost-0.8.3/odooghost/git.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/logger.py` & `odooghost-0.8.3/odooghost/logger.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/services/base.py` & `odooghost-0.8.3/odooghost/services/base.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/services/db.py` & `odooghost-0.8.3/odooghost/services/db.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/services/odoo/addons.py` & `odooghost-0.8.3/odooghost/services/odoo/addons.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/services/odoo/service.py` & `odooghost-0.8.3/odooghost/services/odoo/service.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/stack.py` & `odooghost-0.8.3/odooghost/stack.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/templates/Dockerfile.j2` & `odooghost-0.8.3/odooghost/templates/Dockerfile.j2`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 USER root
 RUN chown -R odoo:odoo /etc/odoo
 
 {% if dependencies.apt %}
 USER root
 # Fix for 11.0 Odoo_Version
-{% if odoo_version <= 11.0 %}
+{% if odoo_version <= 12.0 %}
 RUN sed -i -e 's/deb.debian.org/archive.debian.org/g' \
     -e 's|security.debian.org|archive.debian.org/|g' \
     -e '/stretch-updates/d' /etc/apt/sources.list
 RUN rm -rf /etc/apt/sources.list.d/backports.list
 {% endif %}
 RUN apt-get update && apt-get install -y --no-install-recommends \
     {% for dep in dependencies.apt %}
```

### Comparing `odooghost-0.8.2/odooghost/types.py` & `odooghost-0.8.3/odooghost/types.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/utils/autocomplete.py` & `odooghost-0.8.3/odooghost/utils/autocomplete.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/utils/exec.py` & `odooghost-0.8.3/odooghost/utils/exec.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/utils/misc.py` & `odooghost-0.8.3/odooghost/utils/misc.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/utils/progress_stream.py` & `odooghost-0.8.3/odooghost/utils/progress_stream.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/utils/signals.py` & `odooghost-0.8.3/odooghost/utils/signals.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/utils/stream.py` & `odooghost-0.8.3/odooghost/utils/stream.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/utils/sync_to_async.py` & `odooghost-0.8.3/odooghost/utils/sync_to_async.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/web/api/query/stack.py` & `odooghost-0.8.3/odooghost/web/api/query/stack.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/web/api/schema_types.py` & `odooghost-0.8.3/odooghost/web/api/schema_types.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/web/api/subscription.py` & `odooghost-0.8.3/odooghost/web/api/subscription.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/web/application.py` & `odooghost-0.8.3/odooghost/web/application.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/web/dist/android-chrome-192x192.png` & `odooghost-0.8.3/odooghost/web/dist/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/web/dist/android-chrome-512x512.png` & `odooghost-0.8.3/odooghost/web/dist/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/web/dist/apple-touch-icon.png` & `odooghost-0.8.3/odooghost/web/dist/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/web/dist/assets/ContainersView-CQGACCyA.js` & `odooghost-0.8.3/odooghost/web/dist/assets/ContainersView-BE5deGhZ.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,27 +1,27 @@
 import {
     b as n
-} from "./stack-FDe_L0Se.js";
+} from "./stack-ooq4hns8.js";
 import {
     _ as o,
     a as i
-} from "./VHeader-B9IRV133.js";
+} from "./VHeader-DE-7o50y.js";
 import {
     _ as l
-} from "./VContainers-CS_dVxEN.js";
+} from "./VContainers-Dk3P-tJN.js";
 import {
     u as c,
     c as _,
     a as r,
     d as u,
     w as m,
     b as e,
     o as f
-} from "./index-aZbCTR1y.js";
-import "./VWarningAlert-B-onwvMS.js";
+} from "./index-B_2Yopjn.js";
+import "./VWarningAlert-D3_O5a8o.js";
 const B = {
     __name: "ContainersView",
     setup(p) {
         const {
             loading: s,
             result: a,
             error: t
```

### Comparing `odooghost-0.8.2/odooghost/web/dist/assets/DashboardView-DaNsKC6f.js` & `odooghost-0.8.3/odooghost/web/dist/assets/DashboardView-D7R6tEBr.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -3,26 +3,26 @@
     u as c,
     c as l,
     a as e,
     w as u,
     b as s,
     o as _,
     d as a
-} from "./index-aZbCTR1y.js";
+} from "./index-B_2Yopjn.js";
 import {
     _ as d
-} from "./VContainers-CS_dVxEN.js";
+} from "./VContainers-Dk3P-tJN.js";
 import {
     _ as m,
     a as f
-} from "./VHeader-B9IRV133.js";
+} from "./VHeader-DE-7o50y.js";
 import {
     _ as o
-} from "./VStat-AcXitZbU.js";
-import "./VWarningAlert-B-onwvMS.js";
+} from "./VStat-BuNxdvtd.js";
+import "./VWarningAlert-D3_O5a8o.js";
 const g = i`
   query getDashboard {
     version
     dockerVersion
     stackCount
     containers(stopped: false) {
       id
```

### Comparing `odooghost-0.8.2/odooghost/web/dist/assets/StackItemIndexView-CYLOsCmC.js` & `odooghost-0.8.3/odooghost/web/dist/assets/StackItemIndexView-Bi3wNjjv.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 import {
     _ as a
-} from "./VContainers-CS_dVxEN.js";
+} from "./VContainers-Dk3P-tJN.js";
 import {
     _ as o
-} from "./VStat-AcXitZbU.js";
+} from "./VStat-BuNxdvtd.js";
 import {
     x as c,
     c as r,
     d as s,
     a as t,
     b as n,
     o as i
-} from "./index-aZbCTR1y.js";
+} from "./index-B_2Yopjn.js";
 const l = {
         class: "grid grid-cols-1 gap-4 sm:grid-cols-3"
     },
     _ = s("h3", null, "Containers", -1),
     k = {
         __name: "StackItemIndexView",
         setup(d) {
```

### Comparing `odooghost-0.8.2/odooghost/web/dist/assets/StackItemView-BtdLvO3L.js` & `odooghost-0.8.3/odooghost/web/dist/assets/StackItemView-NU6ZoWkH.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as w
-} from "./stack-FDe_L0Se.js";
+} from "./stack-ooq4hns8.js";
 import {
     V as g,
     _ as b
-} from "./VWarningAlert-B-onwvMS.js";
+} from "./VWarningAlert-D3_O5a8o.js";
 import {
     o as e,
     c as t,
     d as a,
     h as y,
     r as V,
     a as n,
@@ -28,15 +28,15 @@
     s as I,
     n as z,
     _ as Z,
     V as O,
     f as T,
     v as U,
     R as A
-} from "./index-aZbCTR1y.js";
+} from "./index-B_2Yopjn.js";
 import {
     s as k
 } from "./constant-DWkFHeG6.js";
 
 function D(l, s) {
     return e(), t("svg", {
         xmlns: "http://www.w3.org/2000/svg",
```

### Comparing `odooghost-0.8.2/odooghost/web/dist/assets/StackView-C0gt5mfw.js` & `odooghost-0.8.3/odooghost/web/dist/assets/StackView-B3ysXA8u.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     Q as h
-} from "./stack-FDe_L0Se.js";
+} from "./stack-ooq4hns8.js";
 import {
     a as p,
     _ as x
-} from "./VHeader-B9IRV133.js";
+} from "./VHeader-DE-7o50y.js";
 import {
     s as d
 } from "./constant-DWkFHeG6.js";
 import {
     o,
     c as n,
     d as t,
@@ -18,16 +18,16 @@
     w as l,
     b as s,
     F as v,
     e as w,
     f as k,
     t as a,
     n as y
-} from "./index-aZbCTR1y.js";
-import "./VWarningAlert-B-onwvMS.js";
+} from "./index-B_2Yopjn.js";
+import "./VWarningAlert-D3_O5a8o.js";
 
 function b(u, i) {
     return o(), n("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         viewBox: "0 0 24 24",
         fill: "currentColor",
         "aria-hidden": "true",
```

### Comparing `odooghost-0.8.2/odooghost/web/dist/assets/VContainers-CS_dVxEN.js` & `odooghost-0.8.3/odooghost/web/dist/assets/VContainers-Dk3P-tJN.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     d as e,
     F as d,
     e as _,
     n as r,
     t,
     a as p,
     b as x
-} from "./index-aZbCTR1y.js";
+} from "./index-B_2Yopjn.js";
 
 function u(i, o) {
     return n(), a("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         viewBox: "0 0 20 20",
         fill: "currentColor",
         "aria-hidden": "true",
```

### Comparing `odooghost-0.8.2/odooghost/web/dist/assets/VHeader-B9IRV133.js` & `odooghost-0.8.3/odooghost/web/dist/assets/VHeader-DE-7o50y.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 import {
     V as d,
     _ as u
-} from "./VWarningAlert-B-onwvMS.js";
+} from "./VWarningAlert-D3_O5a8o.js";
 import {
     o as s,
     c as a,
     j as o,
     a as l,
     d as c,
     _,
     t as p
-} from "./index-aZbCTR1y.js";
+} from "./index-B_2Yopjn.js";
 const m = {
         key: 0,
         class: "py-20"
     },
     h = {
         key: 1
     },
```

### Comparing `odooghost-0.8.2/odooghost/web/dist/assets/VWarningAlert-B-onwvMS.js` & `odooghost-0.8.3/odooghost/web/dist/assets/VWarningAlert-D3_O5a8o.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     q as n,
     F as b,
     e as S,
     A as p,
     f as $,
     b as k,
     B
-} from "./index-aZbCTR1y.js";
+} from "./index-B_2Yopjn.js";
 
 function C(r, e) {
     return a(), l("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         fill: "none",
         viewBox: "0 0 24 24",
         "stroke-width": "1.5",
```

### Comparing `odooghost-0.8.2/odooghost/web/dist/assets/VWarningAlert-DWujdwvy.css` & `odooghost-0.8.3/odooghost/web/dist/assets/VWarningAlert-DWujdwvy.css`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/web/dist/assets/index-BCu_nn1R.css` & `odooghost-0.8.3/odooghost/web/dist/assets/index-BCu_nn1R.css`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/web/dist/assets/index-aZbCTR1y.js` & `odooghost-0.8.3/odooghost/web/dist/assets/index-B_2Yopjn.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-const __vite__fileDeps = ["assets/DashboardView-DaNsKC6f.js", "assets/VContainers-CS_dVxEN.js", "assets/VHeader-B9IRV133.js", "assets/VWarningAlert-B-onwvMS.js", "assets/VWarningAlert-DWujdwvy.css", "assets/VStat-AcXitZbU.js", "assets/StackView-C0gt5mfw.js", "assets/stack-FDe_L0Se.js", "assets/constant-DWkFHeG6.js", "assets/StackItemView-BtdLvO3L.js", "assets/StackItemIndexView-CYLOsCmC.js", "assets/ContainersView-CQGACCyA.js"],
+const __vite__fileDeps = ["assets/DashboardView-D7R6tEBr.js", "assets/VContainers-Dk3P-tJN.js", "assets/VHeader-DE-7o50y.js", "assets/VWarningAlert-D3_O5a8o.js", "assets/VWarningAlert-DWujdwvy.css", "assets/VStat-BuNxdvtd.js", "assets/StackView-B3ysXA8u.js", "assets/stack-ooq4hns8.js", "assets/constant-DWkFHeG6.js", "assets/StackItemView-NU6ZoWkH.js", "assets/StackItemIndexView-Bi3wNjjv.js", "assets/ContainersView-BE5deGhZ.js"],
     __vite__mapDeps = i => i.map(i => __vite__fileDeps[i]);
 (function() {
     const t = document.createElement("link").relList;
     if (t && t.supports && t.supports("modulepreload")) return;
     for (const i of document.querySelectorAll('link[rel="modulepreload"]')) r(i);
     new MutationObserver(i => {
         for (const o of i)
@@ -22,15 +22,15 @@
         if (i.ep) return;
         i.ep = !0;
         const o = n(i);
         fetch(i.href, o)
     }
 })();
 /**
- * @vue/shared v3.4.26
+ * @vue/shared v3.4.27
  * (c) 2018-present Yuxi (Evan) You and Vue contributors
  * @license MIT
  **/
 /*! #__NO_SIDE_EFFECTS__ */
 function ca(e, t) {
     const n = new Set(e.split(","));
     return r => n.has(r)
@@ -145,15 +145,15 @@
         [`Set(${t.size})`]: [...t.values()].map(n => No(n))
     } : qn(t) ? No(t) : De(t) && !le(t) && !kc(t) ? String(t) : t,
     No = (e, t = "") => {
         var n;
         return qn(e) ? `Symbol(${(n=e.description)!=null?n:t})` : e
     };
 /**
- * @vue/reactivity v3.4.26
+ * @vue/reactivity v3.4.27
  * (c) 2018-present Yuxi (Evan) You and Vue contributors
  * @license MIT
  **/
 let ft;
 class Nc {
     constructor(t = !1) {
         this.detached = t, this._active = !0, this.effects = [], this.cleanups = [], this.parent = ft, !t && ft && (this.index = (ft.scopes || (ft.scopes = [])).push(this) - 1)
@@ -799,15 +799,15 @@
 }
 
 function Ap(e, t, n) {
     const r = e[t];
     return Ve(r) ? r : new kp(e, t, n)
 }
 /**
- * @vue/runtime-core v3.4.26
+ * @vue/runtime-core v3.4.27
  * (c) 2018-present Yuxi (Evan) You and Vue contributors
  * @license MIT
  **/
 function hn(e, t, n, r) {
     try {
         return r ? e(...r) : e()
     } catch (i) {
@@ -3243,17 +3243,17 @@
 }
 const ue = (e, t) => xp(e, t, mo);
 
 function ze(e, t, n) {
     const r = arguments.length;
     return r === 2 ? De(t) && !le(t) ? Gi(t) ? me(e, null, [t]) : me(e, t) : me(e, null, t) : (r > 3 ? n = Array.prototype.slice.call(arguments, 2) : r === 3 && Gi(n) && (n = [n]), me(e, t, n))
 }
-const jv = "3.4.26";
+const jv = "3.4.27";
 /**
- * @vue/runtime-dom v3.4.26
+ * @vue/runtime-dom v3.4.27
  * (c) 2018-present Yuxi (Evan) You and Vue contributors
  * @license MIT
  **/
 const Vv = "http://www.w3.org/2000/svg",
     $v = "http://www.w3.org/1998/Math/MathML",
     nn = typeof document < "u" ? document : null,
     $l = nn && nn.createElement("template"),
@@ -3903,15 +3903,15 @@
             var t = console[e] || console.log;
             return t.apply(console, arguments)
         }
     }
 }(function(e) {
     e.debug = Ti("debug"), e.log = Ti("log"), e.warn = Ti("warn"), e.error = Ti("error")
 })(Nn || (Nn = {}));
-var Fa = "3.10.1";
+var Fa = "3.10.2";
 
 function wt(e) {
     try {
         return e()
     } catch {}
 }
 const Ts = wt(function() {
@@ -17113,52 +17113,52 @@
         })
     },
     S1 = R_({
         history: a_("/"),
         routes: [{
             path: "/",
             name: "dashboard",
-            component: () => Rt(() => import("./DashboardView-DaNsKC6f.js"), __vite__mapDeps([0, 1, 2, 3, 4, 5]))
+            component: () => Rt(() => import("./DashboardView-D7R6tEBr.js"), __vite__mapDeps([0, 1, 2, 3, 4, 5]))
         }, {
             path: "/stacks",
             name: "stacks",
-            component: () => Rt(() => import("./StackView-C0gt5mfw.js"), __vite__mapDeps([6, 7, 2, 3, 4, 8]))
+            component: () => Rt(() => import("./StackView-B3ysXA8u.js"), __vite__mapDeps([6, 7, 2, 3, 4, 8]))
         }, {
             path: "/stack/:stackId",
             name: "stack",
-            component: () => Rt(() => import("./StackItemView-BtdLvO3L.js"), __vite__mapDeps([9, 7, 3, 4, 8])),
+            component: () => Rt(() => import("./StackItemView-NU6ZoWkH.js"), __vite__mapDeps([9, 7, 3, 4, 8])),
             children: [{
                 path: "",
                 name: "stackIndex",
-                component: () => Rt(() => import("./StackItemIndexView-CYLOsCmC.js"), __vite__mapDeps([10, 1, 5]))
+                component: () => Rt(() => import("./StackItemIndexView-Bi3wNjjv.js"), __vite__mapDeps([10, 1, 5]))
             }, {
                 path: "services",
                 name: "stackServices",
-                component: () => Rt(() => import("./StackItemServicesView-CNydrgOE.js"), [])
+                component: () => Rt(() => import("./StackItemServicesView-CFfNOwHX.js"), [])
             }, {
                 path: "containers",
                 name: "stackContainers",
-                component: () => Rt(() => import("./StackItemContainersView-cTSpFQBD.js"), [])
+                component: () => Rt(() => import("./StackItemContainersView-Dni9Qael.js"), [])
             }, {
                 path: "logs",
                 name: "stackLogs",
-                component: () => Rt(() => import("./StackItemLogsView-D5NV0km8.js"), [])
+                component: () => Rt(() => import("./StackItemLogsView-QMXp-UnQ.js"), [])
             }]
         }, {
             path: "/containers",
             name: "containers",
-            component: () => Rt(() => import("./ContainersView-CQGACCyA.js"), __vite__mapDeps([11, 7, 2, 3, 4, 1]))
+            component: () => Rt(() => import("./ContainersView-BE5deGhZ.js"), __vite__mapDeps([11, 7, 2, 3, 4, 1]))
         }, {
             path: "/usage",
             name: "usage",
-            component: () => Rt(() => import("./UsageView-NG-QxEdS.js"), [])
+            component: () => Rt(() => import("./UsageView-DaVpkoWP.js"), [])
         }, {
             path: "/settings",
             name: "settings",
-            component: () => Rt(() => import("./SettingsView-BStxbQD1.js"), [])
+            component: () => Rt(() => import("./SettingsView-BAzeCNyE.js"), [])
         }]
     });
 hm({
     setup() {
         rt(Zd, E1)
     },
     render: () => ze(t1)
```

### Comparing `odooghost-0.8.2/odooghost/web/dist/assets/stack-FDe_L0Se.js` & `odooghost-0.8.3/odooghost/web/dist/assets/stack-ooq4hns8.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     g as e
-} from "./index-aZbCTR1y.js";
+} from "./index-B_2Yopjn.js";
 const t = e`
   query getStack($name: String!) {
     stack(name: $name) {
       id
       name
       state
       odooVersion
```

### Comparing `odooghost-0.8.2/odooghost/web/dist/favicon-16x16.png` & `odooghost-0.8.3/odooghost/web/dist/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/web/dist/favicon-32x32.png` & `odooghost-0.8.3/odooghost/web/dist/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/web/dist/favicon.ico` & `odooghost-0.8.3/odooghost/web/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/odooghost/web/dist/index.html` & `odooghost-0.8.3/odooghost/web/dist/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,14 @@
     <link rel="icon" href="/favicon.ico" />
     <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png" />
     <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png" />
     <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png" />
     <link rel="manifest" href="/site.webmanifest" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>OdooGhost</title>
-    <script type="module" crossorigin src="/assets/index-aZbCTR1y.js"></script>
+    <script type="module" crossorigin src="/assets/index-B_2Yopjn.js"></script>
     <link rel="stylesheet" crossorigin href="/assets/index-BCu_nn1R.css">
   </head>
   <body class="h-full">
     <div id="app" class="h-full"></div>
   </body>
 </html>
```

### Comparing `odooghost-0.8.2/odooghost/web/dist/logo.svg` & `odooghost-0.8.3/odooghost/web/dist/logo.svg`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.2/pyproject.toml` & `odooghost-0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odooghost"
-version = "0.8.2"
+version = "0.8.3"
 description = "Odoo developpement made easy"
 authors = ["Remy Zulauff <remy.zulauff@gmail.com>"]
 readme = "README.md"
 homepage = "https://remyz17.github.io/odooghost/"
 repository = "https://github.com/remyz17/odooghost"
 license = "MIT"
 include = ["odooghost/web/dist/**/*"]
```

### Comparing `odooghost-0.8.2/PKG-INFO` & `odooghost-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odooghost
-Version: 0.8.2
+Version: 0.8.3
 Summary: Odoo developpement made easy
 Home-page: https://remyz17.github.io/odooghost/
 License: MIT
 Author: Remy Zulauff
 Author-email: remy.zulauff@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

