# Comparing `tmp/griptape_cli-0.4.1.tar.gz` & `tmp/griptape_cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_cli-0.4.1.tar", max compression
+gzip compressed data, was "griptape_cli-0.5.0.tar", max compression
```

## Comparing `griptape_cli-0.4.1.tar` & `griptape_cli-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,12 @@
--rw-r--r--   0        0        0    11339 2023-07-26 21:21:47.436236 griptape_cli-0.4.1/LICENSE
--rw-r--r--   0        0        0     2730 2023-12-18 23:54:56.170199 griptape_cli-0.4.1/README.md
--rw-r--r--   0        0        0       65 2023-07-26 21:21:47.436414 griptape_cli-0.4.1/griptape/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 21:21:47.436495 griptape_cli-0.4.1/griptape/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 21:21:47.436579 griptape_cli-0.4.1/griptape/cli/commands/__init__.py
--rw-r--r--   0        0        0     2026 2023-12-18 23:54:56.170359 griptape_cli-0.4.1/griptape/cli/commands/app.py
--rw-r--r--   0        0        0     9271 2024-01-08 17:33:11.028805 griptape_cli-0.4.1/griptape/cli/commands/cloud.py
--rw-r--r--   0        0        0        0 2023-07-26 21:21:47.436756 griptape_cli-0.4.1/griptape/cli/core/__init__.py
--rw-r--r--   0        0        0     1589 2023-12-11 19:34:34.087579 griptape_cli-0.4.1/griptape/cli/core/app.py
--rw-r--r--   0        0        0     2610 2024-01-09 17:24:18.182544 griptape_cli-0.4.1/griptape/cli/core/app_packager.py
--rw-r--r--   0        0        0     7179 2023-12-18 23:54:56.171124 griptape_cli-0.4.1/griptape/cli/core/cloud_client.py
--rw-r--r--   0        0        0     1705 2023-12-16 00:23:54.785915 griptape_cli-0.4.1/griptape/cli/core/structure_runner.py
--rw-r--r--   0        0        0      127 2023-12-11 18:25:42.177392 griptape_cli-0.4.1/griptape/cli/core/templates/app/cookiecutter.json
--rw-r--r--   0        0        0      384 2023-12-11 17:25:14.427832 griptape_cli-0.4.1/griptape/cli/core/templates/app/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-07-26 21:21:47.437144 griptape_cli-0.4.1/griptape/cli/core/templates/app/hooks/pre_gen_project.py
--rw-r--r--   0        0        0       38 2023-12-12 18:51:11.024920 griptape_cli-0.4.1/griptape/cli/core/templates/app/{{cookiecutter.app_name}}/.gitignore
--rw-r--r--   0        0        0       27 2023-07-26 21:21:47.437262 griptape_cli-0.4.1/griptape/cli/core/templates/app/{{cookiecutter.app_name}}/README.md
--rw-r--r--   0        0        0      171 2023-12-15 03:12:35.585824 griptape_cli-0.4.1/griptape/cli/core/templates/app/{{cookiecutter.app_name}}/app.py
--rw-r--r--   0        0        0      323 2023-12-11 18:46:47.966943 griptape_cli-0.4.1/griptape/cli/core/templates/app/{{cookiecutter.app_name}}/pyproject.toml
--rw-r--r--   0        0        0       55 2023-12-11 18:45:58.655456 griptape_cli-0.4.1/griptape/cli/core/templates/app/{{cookiecutter.app_name}}/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-26 21:21:47.437541 griptape_cli-0.4.1/griptape/cli/core/templates/app/{{cookiecutter.app_name}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 22:20:17.950327 griptape_cli-0.4.1/griptape/cli/core/utils/__init__.py
--rw-r--r--   0        0        0       92 2023-12-18 23:54:56.171257 griptape_cli-0.4.1/griptape/cli/core/utils/constants.py
--rw-r--r--   0        0        0      187 2023-12-16 00:54:44.176454 griptape_cli-0.4.1/griptape/cli/core/utils/endpoint_utils.py
--rw-r--r--   0        0        0      216 2023-08-02 21:45:03.982699 griptape_cli-0.4.1/griptape/cli/main.py
--rw-r--r--   0        0        0      738 2024-01-09 17:24:18.182895 griptape_cli-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3601 1970-01-01 00:00:00.000000 griptape_cli-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-11-13 19:20:13.142150 griptape_cli-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7388 2024-05-06 19:30:13.767839 griptape_cli-0.5.0/README.md
+-rw-r--r--   0        0        0       65 2024-04-16 21:16:07.159900 griptape_cli-0.5.0/griptapecli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 21:16:07.159954 griptape_cli-0.5.0/griptapecli/commands/__init__.py
+-rw-r--r--   0        0        0     4885 2024-05-06 19:30:13.768632 griptape_cli-0.5.0/griptapecli/commands/skatepark.py
+-rw-r--r--   0        0        0        0 2024-04-16 21:16:07.160292 griptape_cli-0.5.0/griptapecli/core/__init__.py
+-rw-r--r--   0        0        0     1853 2024-04-29 20:44:33.823901 griptape_cli-0.5.0/griptapecli/core/models.py
+-rw-r--r--   0        0        0     7603 2024-04-29 20:44:42.939557 griptape_cli-0.5.0/griptapecli/core/skatepark.py
+-rw-r--r--   0        0        0     1086 2024-04-23 16:38:36.101669 griptape_cli-0.5.0/griptapecli/core/state.py
+-rw-r--r--   0        0        0      164 2024-04-17 21:13:33.319121 griptape_cli-0.5.0/griptapecli/main.py
+-rw-r--r--   0        0        0      769 2024-05-07 18:19:25.397975 griptape_cli-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8174 1970-01-01 00:00:00.000000 griptape_cli-0.5.0/PKG-INFO
```

### Comparing `griptape_cli-0.4.1/LICENSE` & `griptape_cli-0.5.0/LICENSE`

 * *Files identical despite different names*

