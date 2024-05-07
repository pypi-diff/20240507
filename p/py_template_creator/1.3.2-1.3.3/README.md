# Comparing `tmp/py_template_creator-1.3.2.tar.gz` & `tmp/py_template_creator-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_template_creator-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_template_creator-1.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_template_creator-1.3.2.tar` & `py_template_creator-1.3.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     1800 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/.gitignore
--rw-r--r--   0        0        0    11325 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/LICENSE
--rw-r--r--   0        0        0      578 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/README.md
--rw-r--r--   0        0        0       80 2024-04-26 11:12:26.138265 py_template_creator-1.3.2/py_template_creator/__init__.py
--rw-r--r--   0        0        0      150 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/cookiecutter.json
--rw-r--r--   0        0        0      543 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.env
--rw-r--r--   0        0        0      543 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.env.example
--rw-r--r--   0        0        0       91 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.flake8
--rw-r--r--   0        0        0     2533 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.gitignore
--rw-r--r--   0        0        0      366 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2255 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/docker-compose.yaml
--rw-r--r--   0        0        0      966 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/Dockerfile
--rw-r--r--   0        0        0     1224 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/Makefile
--rw-r--r--   0        0        0        0 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/README.md
--rwxr-xr-x   0        0        0      122 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/config/run.sh
--rwxr-xr-x   0        0        0      301 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/config/test.sh
--rw-r--r--   0        0        0        0 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/__init__.py
--rw-r--r--   0        0        0     1984 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/alembic.ini
--rw-r--r--   0        0        0        0 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/__init__.py
--rw-r--r--   0        0        0       38 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/README
--rw-r--r--   0        0        0        0 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/__init__.py
--rw-r--r--   0        0        0     2247 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/env.py
--rw-r--r--   0        0        0      510 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/script.py.mako
--rw-r--r--   0        0        0        0 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/versions/.gitkeep
--rw-r--r--   0        0        0       57 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/api/__init__.py
--rw-r--r--   0        0        0      312 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/api/base.py
--rw-r--r--   0        0        0     3007 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/main.py
--rw-r--r--   0        0        0      173 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/models/__init__.py
--rw-r--r--   0        0        0     2107 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/models/base.py
--rw-r--r--   0        0        0        0 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/schemas/__init__.py
--rw-r--r--   0        0        0       73 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/utilities/__init__.py
--rw-r--r--   0        0        0      217 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/utilities/dependecies.py
--rw-r--r--   0        0        0        0 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/tests/__init__.py
--rw-r--r--   0        0        0     3560 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/tests/conftest.py
--rw-r--r--   0        0        0      412 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/tests/test_health.py
--rw-r--r--   0        0        0      662 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/pyproject.toml
--rw-r--r--   0        0        0      148 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/requirements/common.txt
--rw-r--r--   0        0        0       67 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/requirements/local.txt
--rw-r--r--   0        0        0       15 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/requirements/prod.txt
--rw-r--r--   0        0        0      176 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/requirements/test.txt
--rw-r--r--   0        0        0      792 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/main.py
--rw-r--r--   0        0        0      115 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/cookiecutter.json
--rw-r--r--   0        0        0      917 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/Dockerfile
--rw-r--r--   0        0        0     1256 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/Makefile
--rw-r--r--   0        0        0      909 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/README.md
--rwxr-xr-x   0        0        0       52 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/config/run.sh
--rw-r--r--   0        0        0      328 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/config/test.sh
--rw-r--r--   0        0        0        0 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/__init__.py
--rw-r--r--   0        0        0     1984 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/alembic.ini
--rw-r--r--   0        0        0        1 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/__init__.py
--rw-r--r--   0        0        0       38 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/README
--rw-r--r--   0        0        0        0 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/__init__.py
--rw-r--r--   0        0        0     2124 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/env.py
--rw-r--r--   0        0        0      510 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/script.py.mako
--rw-r--r--   0        0        0        0 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/versions/.gitkeep
--rw-r--r--   0        0        0       80 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/handlers/__init__.py
--rw-r--r--   0        0        0      460 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/handlers/example_handler.py
--rw-r--r--   0        0        0      135 2024-04-26 09:45:01.712921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/models/__init__.py
--rw-r--r--   0        0        0      717 2024-04-26 11:11:46.490671 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/models/base.py
--rw-r--r--   0        0        0     1533 2024-04-26 09:45:01.716921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/run.py
--rw-r--r--   0        0        0        0 2024-04-26 09:45:01.716921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/tests/__init__.py
--rw-r--r--   0        0        0     1847 2024-04-26 09:45:01.716921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/tests/conftest.py
--rw-r--r--   0        0        0      642 2024-04-26 09:45:01.716921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/pyproject.toml
--rw-r--r--   0        0        0      118 2024-04-26 09:45:01.716921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/requirements/common.txt
--rw-r--r--   0        0        0       48 2024-04-26 09:45:01.716921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/requirements/local.txt
--rw-r--r--   0        0        0       13 2024-04-26 09:45:01.716921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/requirements/prod.txt
--rw-r--r--   0        0        0      138 2024-04-26 09:45:01.716921 py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/requirements/test.txt
--rw-r--r--   0        0        0      448 2024-04-26 09:45:01.716921 py_template_creator-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 py_template_creator-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1800 2024-04-11 06:33:56.852609 py_template_creator-1.3.3/.gitignore
+-rw-r--r--   0        0        0    11325 2024-04-11 06:33:56.852609 py_template_creator-1.3.3/LICENSE
+-rw-r--r--   0        0        0      578 2024-04-11 06:33:56.852609 py_template_creator-1.3.3/README.md
+-rw-r--r--   0        0        0       80 2024-05-07 08:41:17.638014 py_template_creator-1.3.3/py_template_creator/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-11 09:45:18.402626 py_template_creator-1.3.3/py_template_creator/api-scelet/cookiecutter.json
+-rw-r--r--   0        0        0      543 2024-04-20 18:42:57.898424 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.env
+-rw-r--r--   0        0        0      543 2024-04-20 18:42:55.026391 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.env.example
+-rw-r--r--   0        0        0       91 2024-04-20 17:37:49.032906 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.flake8
+-rw-r--r--   0        0        0     2533 2024-04-20 17:36:22.772304 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.gitignore
+-rw-r--r--   0        0        0      366 2024-04-20 17:37:37.756828 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2255 2024-04-20 18:44:33.763522 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/docker-compose.yaml
+-rw-r--r--   0        0        0     1003 2024-05-07 08:39:40.660837 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/Dockerfile
+-rw-r--r--   0        0        0     1224 2024-04-20 19:14:38.680183 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/Makefile
+-rw-r--r--   0        0        0        0 2024-04-20 17:39:18.117516 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/README.md
+-rwxr-xr-x   0        0        0      122 2024-04-20 17:41:14.786304 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/config/run.sh
+-rwxr-xr-x   0        0        0      301 2024-04-20 19:30:07.007483 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/config/test.sh
+-rw-r--r--   0        0        0        0 2024-04-20 17:28:35.404787 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/__init__.py
+-rw-r--r--   0        0        0     1984 2024-04-20 17:28:35.404787 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/alembic.ini
+-rw-r--r--   0        0        0        0 2024-04-20 17:28:35.404787 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-20 17:28:35.408788 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/README
+-rw-r--r--   0        0        0        0 2024-04-20 17:28:35.408788 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/__init__.py
+-rw-r--r--   0        0        0     2247 2024-04-20 20:02:42.583219 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/env.py
+-rw-r--r--   0        0        0      510 2024-04-20 17:28:35.408788 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/script.py.mako
+-rw-r--r--   0        0        0        0 2024-04-20 17:28:35.408788 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/versions/.gitkeep
+-rw-r--r--   0        0        0       57 2024-04-20 17:28:35.412788 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/api/__init__.py
+-rw-r--r--   0        0        0      312 2024-04-20 17:28:35.412788 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/api/base.py
+-rw-r--r--   0        0        0     3007 2024-04-20 17:28:35.412788 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/main.py
+-rw-r--r--   0        0        0      173 2024-04-20 17:28:35.412788 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/models/__init__.py
+-rw-r--r--   0        0        0     2107 2024-04-20 17:28:35.416787 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/models/base.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:28:35.416787 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/schemas/__init__.py
+-rw-r--r--   0        0        0       73 2024-04-20 17:28:35.416787 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/utilities/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-20 17:28:35.416787 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/utilities/dependecies.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:28:35.416787 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/tests/__init__.py
+-rw-r--r--   0        0        0     3560 2024-04-20 17:28:35.420788 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/tests/conftest.py
+-rw-r--r--   0        0        0      412 2024-04-20 17:28:35.420788 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/tests/test_health.py
+-rw-r--r--   0        0        0      662 2024-04-20 18:21:55.965797 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/pyproject.toml
+-rw-r--r--   0        0        0      148 2024-04-24 14:34:12.630682 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/requirements/common.txt
+-rw-r--r--   0        0        0       67 2024-04-20 17:28:35.420788 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/requirements/local.txt
+-rw-r--r--   0        0        0       15 2024-04-20 17:28:35.424788 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/requirements/prod.txt
+-rw-r--r--   0        0        0      176 2024-04-20 17:28:35.424788 py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/requirements/test.txt
+-rw-r--r--   0        0        0      792 2024-04-11 09:55:32.622141 py_template_creator-1.3.3/py_template_creator/main.py
+-rw-r--r--   0        0        0      115 2024-04-20 20:04:06.404111 py_template_creator-1.3.3/py_template_creator/service-scelet/cookiecutter.json
+-rw-r--r--   0        0        0     1014 2024-05-07 08:39:27.220673 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/Dockerfile
+-rw-r--r--   0        0        0     1256 2024-04-20 19:31:37.044792 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/Makefile
+-rw-r--r--   0        0        0      909 2024-04-20 20:04:06.412110 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/README.md
+-rwxr-xr-x   0        0        0       52 2024-04-20 20:04:06.412110 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/config/run.sh
+-rw-r--r--   0        0        0      328 2024-04-20 19:30:50.488121 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/config/test.sh
+-rw-r--r--   0        0        0        0 2024-04-11 09:17:53.922471 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/__init__.py
+-rw-r--r--   0        0        0     1984 2024-04-20 18:06:41.933333 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/alembic.ini
+-rw-r--r--   0        0        0        1 2024-04-11 09:22:01.116037 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-20 17:57:52.311352 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/README
+-rw-r--r--   0        0        0        0 2024-04-20 17:57:52.311352 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/__init__.py
+-rw-r--r--   0        0        0     2124 2024-04-20 20:02:01.538787 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/env.py
+-rw-r--r--   0        0        0      510 2024-04-20 17:57:52.311352 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/script.py.mako
+-rw-r--r--   0        0        0        0 2024-04-20 17:57:52.315352 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/versions/.gitkeep
+-rw-r--r--   0        0        0       80 2024-04-11 06:33:56.856609 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/handlers/__init__.py
+-rw-r--r--   0        0        0      460 2024-04-11 09:22:29.040252 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/handlers/example_handler.py
+-rw-r--r--   0        0        0      135 2024-04-20 18:59:12.391435 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/models/__init__.py
+-rw-r--r--   0        0        0      717 2024-05-07 08:40:34.685492 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/models/base.py
+-rw-r--r--   0        0        0     1533 2024-04-20 20:04:06.412110 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/run.py
+-rw-r--r--   0        0        0        0 2024-04-20 18:12:49.849111 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/tests/__init__.py
+-rw-r--r--   0        0        0     1847 2024-04-20 19:29:16.362724 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/tests/conftest.py
+-rw-r--r--   0        0        0      638 2024-05-07 08:39:10.392469 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-04-24 14:34:17.094733 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/requirements/common.txt
+-rw-r--r--   0        0        0       48 2024-04-11 06:33:56.856609 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/requirements/local.txt
+-rw-r--r--   0        0        0       13 2024-04-11 06:33:56.856609 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/requirements/prod.txt
+-rw-r--r--   0        0        0      138 2024-04-20 18:30:03.917007 py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/requirements/test.txt
+-rw-r--r--   0        0        0      448 2024-04-11 09:55:59.354480 py_template_creator-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 py_template_creator-1.3.3/PKG-INFO
```

### Comparing `py_template_creator-1.3.2/.gitignore` & `py_template_creator-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/LICENSE` & `py_template_creator-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/README.md` & `py_template_creator-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.env` & `py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.env`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.env.example` & `py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.env.example`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.gitignore` & `py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/docker-compose.yaml` & `py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/Dockerfile` & `py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/Dockerfile`

 * *Files 6% similar despite different names*

```diff
@@ -26,12 +26,13 @@
 WORKDIR /opt/app
 
 COPY ./ /opt/app/
 COPY ./config /opt/app/config
 
 # Ensuring script permissions
 RUN chmod +x /opt/app/config/run.sh
+RUN chmod +x /opt/app/config/test.sh
 
 RUN pip install -e .
 
 # Specify the command to run when the image is run.
 CMD "/opt/app/config/run.sh"
```

### Comparing `py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/Makefile` & `py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/Makefile`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/alembic.ini` & `py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/alembic.ini`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/env.py` & `py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/alembic/env.py`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/main.py` & `py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/main.py`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/models/base.py` & `py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/app/models/base.py`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/tests/conftest.py` & `py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/package/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/pyproject.toml` & `py_template_creator-1.3.3/py_template_creator/api-scelet/{{ cookiecutter.project_name }}/rest_api/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/main.py` & `py_template_creator-1.3.3/py_template_creator/main.py`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/Dockerfile` & `py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/Dockerfile`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,21 @@
        && pip install -r /wheels/requirements/prod.txt \
                       -f /wheels \
        && rm -rf /wheels \
        && rm -rf /root/.cache/pip/*
 
 
 # Copy code to docker
-COPY ./ /opt/app/
-COPY ./config/ /opt/app/config/
 WORKDIR /opt/app
-RUN python -m pip install .
+
+COPY ./ /opt/app/
+COPY ./config /opt/app/config
+
+# Ensuring script permissions
+RUN chmod +x /opt/app/config/run.sh
+RUN chmod +x /opt/app/config/test.sh
+
+RUN pip install -e .
 
 # Specify the command to run when the image is run.
 CMD "/opt/app/config/run.sh"
```

### Comparing `py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/Makefile` & `py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/Makefile`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/README.md` & `py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/README.md`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/alembic.ini` & `py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/alembic.ini`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/env.py` & `py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/alembic/env.py`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/models/base.py` & `py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/app/models/base.py`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/run.py` & `py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/run.py`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/tests/conftest.py` & `py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/package/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py_template_creator-1.3.2/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/pyproject.toml` & `py_template_creator-1.3.3/py_template_creator/service-scelet/{{ cookiecutter.project_name }}/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 {{ cookiecutter.project_name }} = "package.run:main"
 
 [tool.setuptools]
 packages = ["package"]
 
 [tool.coverage.run]
 source = ["./"]
-omit = ["package/app/run.py", "package/app/models/base.py", "package/app/alembic/*"]
+omit = ["package/run.py", "package/app/models/base.py", "package/app/alembic/*"]
 
 [tool.coverage.report]
 fail_under = 80
 show_missing = true
 exclude_lines = ["pragma: no cover"]
 
 [tool.pytest.ini_options]
```

### Comparing `py_template_creator-1.3.2/PKG-INFO` & `py_template_creator-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_template_creator
-Version: 1.3.2
+Version: 1.3.3
 Summary: Generate your python project template with ease.
 Author-email: Ivan Djuraki <ivan.djuraki@bridgewaterlabs.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: cookiecutter
```

