# Comparing `tmp/swh_core-3.0.1.tar.gz` & `tmp/swh_core-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh_core-3.0.1.tar", last modified: Fri Apr 26 09:58:29 2024, max compression
+gzip compressed data, was "swh_core-3.1.0.tar", last modified: Tue May  7 13:49:24 2024, max compression
```

## Comparing `swh_core-3.0.1.tar` & `swh_core-3.1.0.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.350315 swh_core-3.0.1/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      342 2024-04-26 09:58:23.000000 swh_core-3.0.1/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-04-26 09:58:23.000000 swh_core-3.0.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-04-26 09:58:23.000000 swh_core-3.0.1/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1410 2024-04-26 09:58:23.000000 swh_core-3.0.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-04-26 09:58:23.000000 swh_core-3.0.1/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-04-26 09:58:23.000000 swh_core-3.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-04-26 09:58:23.000000 swh_core-3.0.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-04-26 09:58:23.000000 swh_core-3.0.1/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-26 09:58:23.000000 swh_core-3.0.1/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       95 2024-04-26 09:58:23.000000 swh_core-3.0.1/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3541 2024-04-26 09:58:29.350315 swh_core-3.0.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)      293 2024-04-26 09:58:23.000000 swh_core-3.0.1/README.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      712 2024-04-26 09:58:23.000000 swh_core-3.0.1/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.306316 swh_core-3.0.1/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      293 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.306316 swh_core-3.0.1/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.306316 swh_core-3.0.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      383 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6486 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/db.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      273 2024-04-26 09:58:23.000000 swh_core-3.0.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      982 2024-04-26 09:58:23.000000 swh_core-3.0.1/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2117 2024-04-26 09:58:23.000000 swh_core-3.0.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      156 2024-04-26 09:58:23.000000 swh_core-3.0.1/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-04-26 09:58:23.000000 swh_core-3.0.1/requirements-db.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      147 2024-04-26 09:58:23.000000 swh_core-3.0.1/requirements-http.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-04-26 09:58:23.000000 swh_core-3.0.1/requirements-logging.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      159 2024-04-26 09:58:23.000000 swh_core-3.0.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       71 2024-04-26 09:58:23.000000 swh_core-3.0.1/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-04-26 09:58:29.350315 swh_core-3.0.1/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.306316 swh_core-3.0.1/swh/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      143 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/__main__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.310316 swh_core-3.0.1/swh/core/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.314316 swh_core-3.0.1/swh/core/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20373 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6379 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/asynchronous.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2073 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/classes.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1192 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/gunicorn_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5812 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/negotiation.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10114 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/serializers.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.318316 swh_core-3.0.1/swh/core/api/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4292 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/server_testing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7863 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_async.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2755 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_classes.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5404 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_gunicorn.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      862 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_init.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6129 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_rpc_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5170 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_rpc_client_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7968 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_rpc_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4871 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_rpc_server_asynchronous.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8925 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       63 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/api_async.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.318316 swh_core-3.0.1/swh/core/cli/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5496 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/cli/__init__.py
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)    14013 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/cli/db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2044 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/collections.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9207 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/config.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.318316 swh_core-3.0.1/swh/core/db/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10619 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4888 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    24051 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/db_utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.318316 swh_core-3.0.1/swh/core/db/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      664 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/sql/35-dbversion.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      683 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/sql/36-dbmodule.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.322316 swh_core-3.0.1/swh/core/db/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2554 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.294316 swh_core-3.0.1/swh/core/db/tests/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.294316 swh_core-3.0.1/swh/core/db/tests/data/cli/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.322316 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       41 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/0-superuser-init.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      790 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/15-flavor.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      156 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/40-funcs.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      126 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/50-data.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.326315 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/001.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/002.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/003.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/004.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      306 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/005-bis.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/005.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      196 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/data/cli/sql/upgrades/006.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15397 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13826 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/test_db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9400 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/db/tests/test_db_utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.326315 swh_core-3.0.1/swh/core/github/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/github/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6612 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/github/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.326315 swh_core-3.0.1/swh/core/github/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/github/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14265 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/github/tests/test_github_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1440 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/github/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11211 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/github/utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4331 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/logger.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2583 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/logging.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12994 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3271 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3603 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/sentry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16759 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/statsd.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8364 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tarball.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.330315 swh_core-3.0.1/swh/core/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       98 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.330315 swh_core-3.0.1/swh/core/tests/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.338315 swh_core-3.0.1/swh/core/tests/data/archives/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2028 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/ca-certificates-20210603-1-any.pkg.tar.zst
--rw-r--r--   0 jenkins    (115) jenkins    (120)  1087901 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/groff-1.02.tar.Z
--rw-r--r--   0 jenkins    (115) jenkins    (120)      550 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.jar
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tar
--rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tar.bz2
--rw-r--r--   0 jenkins    (115) jenkins    (120)      181 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tar.gz
--rw-r--r--   0 jenkins    (115) jenkins    (120)      190 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tar.lz
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tar.x
--rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tbz
--rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.tbz2
--rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.war
--rw-r--r--   0 jenkins    (115) jenkins    (120)      162 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/hello.zip
--rw-r--r--   0 jenkins    (115) jenkins    (120)   845917 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/msk316src.zip
--rw-r--r--   0 jenkins    (115) jenkins    (120)    45185 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/archives/tokei-12.1.2.crate
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.338315 swh_core-3.0.1/swh/core/tests/data/http_example.com/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/http_example.com/something.json
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.338315 swh_core-3.0.1/swh/core/tests/data/https_example.com/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/https_example.com/file.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)       28 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/https_example.com/file.json,name=doe,firstname=jane
--rw-r--r--   0 jenkins    (115) jenkins    (120)       25 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/https_example.com/file.json_visit1
--rw-r--r--   0 jenkins    (115) jenkins    (120)        9 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/https_example.com/other.json
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.338315 swh_core-3.0.1/swh/core/tests/data/https_forge.s.o/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/https_forge.s.o/api_diffusion,attachments[uris]=1
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.338315 swh_core-3.0.1/swh/core/tests/data/https_www.reference.com/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       17 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/https_www.reference.com/web,q=What+Is+an+Example+of+a+URL?,qo=contentPageRelatedSearch,o=600605,l=dir,sga=1
--rw-r--r--   0 jenkins    (115) jenkins    (120)      642 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/data/logging-config.yaml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.342315 swh_core-3.0.1/swh/core/tests/fixture/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/fixture/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      401 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/fixture/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.294316 swh_core-3.0.1/swh/core/tests/fixture/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.342315 swh_core-3.0.1/swh/core/tests/fixture/data/https_example.com/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       25 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/fixture/data/https_example.com/file.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      797 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/fixture/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11911 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2439 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_collections.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10147 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3738 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_logger.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2826 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_logging.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4018 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2580 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4879 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_sentry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18746 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_statsd.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9873 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_tarball.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5422 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5788 2024-04-26 09:58:23.000000 swh_core-3.0.1/swh/core/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-26 09:58:29.342315 swh_core-3.0.1/swh.core.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3541 2024-04-26 09:58:29.000000 swh_core-3.0.1/swh.core.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4363 2024-04-26 09:58:29.000000 swh_core-3.0.1/swh.core.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-04-26 09:58:29.000000 swh_core-3.0.1/swh.core.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      148 2024-04-26 09:58:29.000000 swh_core-3.0.1/swh.core.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-04-26 09:58:29.000000 swh_core-3.0.1/swh.core.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-04-26 09:58:29.000000 swh_core-3.0.1/swh.core.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1550 2024-04-26 09:58:23.000000 swh_core-3.0.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.157636 swh_core-3.1.0/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      342 2024-05-07 13:49:17.000000 swh_core-3.1.0/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-05-07 13:49:17.000000 swh_core-3.1.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-07 13:49:17.000000 swh_core-3.1.0/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1410 2024-05-07 13:49:17.000000 swh_core-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-07 13:49:17.000000 swh_core-3.1.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-07 13:49:17.000000 swh_core-3.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-05-07 13:49:17.000000 swh_core-3.1.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-07 13:49:17.000000 swh_core-3.1.0/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-07 13:49:17.000000 swh_core-3.1.0/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       95 2024-05-07 13:49:17.000000 swh_core-3.1.0/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3541 2024-05-07 13:49:24.157636 swh_core-3.1.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      293 2024-05-07 13:49:17.000000 swh_core-3.1.0/README.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      712 2024-05-07 13:49:17.000000 swh_core-3.1.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.117637 swh_core-3.1.0/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      293 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.117637 swh_core-3.1.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.117637 swh_core-3.1.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      383 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6486 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/db.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      273 2024-05-07 13:49:17.000000 swh_core-3.1.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      982 2024-05-07 13:49:17.000000 swh_core-3.1.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2117 2024-05-07 13:49:17.000000 swh_core-3.1.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      156 2024-05-07 13:49:17.000000 swh_core-3.1.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-07 13:49:17.000000 swh_core-3.1.0/requirements-db.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      147 2024-05-07 13:49:17.000000 swh_core-3.1.0/requirements-http.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-05-07 13:49:17.000000 swh_core-3.1.0/requirements-logging.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      159 2024-05-07 13:49:17.000000 swh_core-3.1.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       71 2024-05-07 13:49:17.000000 swh_core-3.1.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      170 2024-05-07 13:49:24.157636 swh_core-3.1.0/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.117637 swh_core-3.1.0/swh/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      143 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/__main__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.121636 swh_core-3.1.0/swh/core/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.125636 swh_core-3.1.0/swh/core/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    21775 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6379 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/asynchronous.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2073 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/classes.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1192 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/gunicorn_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5812 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/negotiation.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10114 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/serializers.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.125636 swh_core-3.1.0/swh/core/api/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4292 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/server_testing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7863 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_async.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2755 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_classes.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5404 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_gunicorn.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      862 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6944 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_rpc_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5170 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_rpc_client_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7968 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_rpc_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4871 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_rpc_server_asynchronous.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8925 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       63 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/api_async.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.129636 swh_core-3.1.0/swh/core/cli/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5496 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/cli/__init__.py
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)    14013 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/cli/db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2044 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/collections.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9207 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/config.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.129636 swh_core-3.1.0/swh/core/db/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10619 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4888 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24051 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/db_utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.129636 swh_core-3.1.0/swh/core/db/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      664 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/sql/35-dbversion.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      683 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/sql/36-dbmodule.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.129636 swh_core-3.1.0/swh/core/db/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2554 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.105637 swh_core-3.1.0/swh/core/db/tests/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.105637 swh_core-3.1.0/swh/core/db/tests/data/cli/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.133636 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       41 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/0-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      790 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/15-flavor.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      156 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/40-funcs.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      126 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/50-data.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.133636 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/001.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/002.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/003.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/004.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      306 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/005-bis.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       82 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/005.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      196 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/data/cli/sql/upgrades/006.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15397 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13826 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/test_db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9400 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/db/tests/test_db_utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.133636 swh_core-3.1.0/swh/core/github/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/github/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6612 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/github/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.137636 swh_core-3.1.0/swh/core/github/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/github/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14265 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/github/tests/test_github_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1440 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/github/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11211 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/github/utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4331 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/logger.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2583 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/logging.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12994 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3271 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3603 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/sentry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16759 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/statsd.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8364 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tarball.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.137636 swh_core-3.1.0/swh/core/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       98 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.141636 swh_core-3.1.0/swh/core/tests/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.145636 swh_core-3.1.0/swh/core/tests/data/archives/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2028 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/ca-certificates-20210603-1-any.pkg.tar.zst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)  1087901 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/groff-1.02.tar.Z
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      550 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.jar
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tar
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tar.bz2
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      181 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tar.gz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      190 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tar.lz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tar.x
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tbz
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      199 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.tbz2
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.war
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      162 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/hello.zip
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   845917 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/msk316src.zip
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    45185 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/archives/tokei-12.1.2.crate
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.145636 swh_core-3.1.0/swh/core/tests/data/http_example.com/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/http_example.com/something.json
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.145636 swh_core-3.1.0/swh/core/tests/data/https_example.com/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/https_example.com/file.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       28 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/https_example.com/file.json,name=doe,firstname=jane
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       25 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/https_example.com/file.json_visit1
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        9 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/https_example.com/other.json
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.145636 swh_core-3.1.0/swh/core/tests/data/https_forge.s.o/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/https_forge.s.o/api_diffusion,attachments[uris]=1
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.145636 swh_core-3.1.0/swh/core/tests/data/https_www.reference.com/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       17 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/https_www.reference.com/web,q=What+Is+an+Example+of+a+URL?,qo=contentPageRelatedSearch,o=600605,l=dir,sga=1
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      642 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/data/logging-config.yaml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.149636 swh_core-3.1.0/swh/core/tests/fixture/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/fixture/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      401 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/fixture/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.109637 swh_core-3.1.0/swh/core/tests/fixture/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.149636 swh_core-3.1.0/swh/core/tests/fixture/data/https_example.com/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       25 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/fixture/data/https_example.com/file.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      797 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/fixture/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11911 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2439 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_collections.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10147 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3738 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_logger.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2826 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_logging.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4018 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2580 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4879 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_sentry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18746 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_statsd.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9873 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_tarball.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5422 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5788 2024-05-07 13:49:17.000000 swh_core-3.1.0/swh/core/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-07 13:49:24.149636 swh_core-3.1.0/swh.core.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3541 2024-05-07 13:49:24.000000 swh_core-3.1.0/swh.core.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4363 2024-05-07 13:49:24.000000 swh_core-3.1.0/swh.core.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-07 13:49:24.000000 swh_core-3.1.0/swh.core.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      148 2024-05-07 13:49:24.000000 swh_core-3.1.0/swh.core.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-05-07 13:49:24.000000 swh_core-3.1.0/swh.core.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-07 13:49:24.000000 swh_core-3.1.0/swh.core.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1550 2024-05-07 13:49:17.000000 swh_core-3.1.0/tox.ini
```

### Comparing `swh_core-3.0.1/.pre-commit-config.yaml` & `swh_core-3.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/CODE_OF_CONDUCT.md` & `swh_core-3.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/LICENSE` & `swh_core-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/PKG-INFO` & `swh_core-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.core
-Version: 3.0.1
+Version: 3.1.0
 Summary: Software Heritage core utilities
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-core
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-core/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-core/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-core.git
```

### Comparing `swh_core-3.0.1/conftest.py` & `swh_core-3.1.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/docs/db.rst` & `swh_core-3.1.0/docs/db.rst`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/mypy.ini` & `swh_core-3.1.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/pyproject.toml` & `swh_core-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/__init__.py` & `swh_core-3.1.0/swh/core/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,65 +190,96 @@
             return self._post(meth._endpoint_path, post_data)
 
         if meth_name not in attributes:
             attributes[meth_name] = meth_
 
 
 class RPCClient(metaclass=MetaRPCClient):
-    """Proxy to an internal SWH RPC"""
+    """Proxy to an internal SWH RPC.
 
-    backend_class = None  # type: ClassVar[Optional[type]]
+    Arguments:
+      url: base url for the RPC endpoints
+      timeout: request timeout. Can be a pair of floats, used to distinguish
+        between connection and read timeouts.
+      chunk_size: used for iteration on chunked responses
+      max_retries: number of automatic retries issued for requests
+      pool_connections: number of connections instantiated in the default connection pool
+      pool_maxsize: maximum size of the connection pool
+      adapter_kwargs: extra keyword arguments to pass to the
+        :class:`requests.adapters.HTTPAdapter`
+      api_exception: The exception class to raise in case of communication error
+        with the server.
+      reraise_exceptions: On server errors, if any of the exception classes in
+        this list has the same name as the error name, then the exception will
+        be instantiated and raised instead of a generic RemoteException.
+
+    """
+
+    backend_class: ClassVar[Optional[type]] = None
     """For each method of `backend_class` decorated with
     :func:`remote_api_endpoint`, a method with the same prototype and
     docstring will be added to this class. Calls to this new method will
     be translated into HTTP requests to a remote server.
 
     This backend class will never be instantiated, it only serves as
     a template."""
 
-    api_exception = APIError  # type: ClassVar[Type[Exception]]
+    api_exception: Type[Exception] = APIError
     """The exception class to raise in case of communication error with
     the server."""
 
-    reraise_exceptions: ClassVar[List[Type[Exception]]] = []
+    reraise_exceptions: List[Type[Exception]] = []
     """On server errors, if any of the exception classes in this list
     has the same name as the error name, then the exception will
     be instantiated and raised instead of a generic RemoteException."""
 
     extra_type_encoders: List[Tuple[type, str, Callable]] = []
     """Value of `extra_encoders` passed to `json_dumps` or `msgpack_dumps`
     to be able to serialize more object types."""
     extra_type_decoders: Dict[str, Callable] = {}
     """Value of `extra_decoders` passed to `json_loads` or `msgpack_loads`
     to be able to deserialize more object types."""
 
     def __init__(
         self,
-        url,
-        api_exception=None,
-        timeout=None,
-        chunk_size=4096,
-        reraise_exceptions=None,
+        url: str,
+        timeout: Union[None, Tuple[float, float], List[float], float] = None,
+        chunk_size: int = 4096,
+        max_retries: int = 3,
+        pool_connections: int = 20,
+        pool_maxsize: int = 100,
+        adapter_kwargs: Optional[Dict[str, Any]] = None,
+        api_exception: Optional[Type[Exception]] = None,
+        reraise_exceptions: Optional[List[Type[Exception]]] = None,
         **kwargs,
     ):
         if api_exception:
             self.api_exception = api_exception
         if reraise_exceptions:
             self.reraise_exceptions = reraise_exceptions
         base_url = url if url.endswith("/") else url + "/"
         self.url = base_url
+
         self.session = requests.Session()
         adapter = requests.adapters.HTTPAdapter(
-            max_retries=kwargs.get("max_retries", 3),
-            pool_connections=kwargs.get("pool_connections", 20),
-            pool_maxsize=kwargs.get("pool_maxsize", 100),
+            max_retries=max_retries,
+            pool_connections=pool_connections,
+            pool_maxsize=pool_maxsize,
+            **(adapter_kwargs or {}),
         )
         self.session.mount(self.url, adapter)
 
+        if isinstance(timeout, list):
+            if len(timeout) != 2:
+                raise ValueError(
+                    "timeout must be a pair of (connect, read) floats, not %r" % timeout
+                )
+            timeout = (timeout[0], timeout[1])
         self.timeout = timeout
+
         self.chunk_size = chunk_size
 
     def _url(self, endpoint):
         return "%s%s" % (self.url, endpoint)
 
     def raw_verb(self, verb, endpoint, **opts):
         if "chunk_size" in opts:
```

### Comparing `swh_core-3.0.1/swh/core/api/asynchronous.py` & `swh_core-3.1.0/swh/core/api/asynchronous.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/classes.py` & `swh_core-3.1.0/swh/core/api/classes.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/gunicorn_config.py` & `swh_core-3.1.0/swh/core/api/gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/negotiation.py` & `swh_core-3.1.0/swh/core/api/negotiation.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/serializers.py` & `swh_core-3.1.0/swh/core/api/serializers.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/tests/server_testing.py` & `swh_core-3.1.0/swh/core/api/tests/server_testing.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/tests/test_async.py` & `swh_core-3.1.0/swh/core/api/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/tests/test_classes.py` & `swh_core-3.1.0/swh/core/api/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/tests/test_gunicorn.py` & `swh_core-3.1.0/swh/core/api/tests/test_gunicorn.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/tests/test_init.py` & `swh_core-3.1.0/swh/core/api/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/tests/test_rpc_client.py` & `swh_core-3.1.0/swh/core/api/tests/test_rpc_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 class ReraiseException(Exception):
     pass
 
 
 @pytest.fixture
-def rpc_client(requests_mock):
+def rpc_client_class(requests_mock):
     class TestStorage:
         @remote_api_endpoint("test_endpoint_url")
         def test_endpoint(self, test_data, db=None, cur=None):
             ...
 
         @remote_api_endpoint("path/to/endpoint")
         def something(self, data, db=None, cur=None):
@@ -74,15 +74,20 @@
             context.content = b"<h1>413 request entity too large</h1>\r\n"
         else:
             assert False
         return context.content
 
     requests_mock.post(re.compile("mock://example.com/"), content=callback)
 
-    return Testclient(url="mock://example.com")
+    return Testclient
+
+
+@pytest.fixture
+def rpc_client(rpc_client_class):
+    return rpc_client_class(url="mock://example.com")
 
 
 def test_client(rpc_client):
     assert hasattr(rpc_client, "test_endpoint")
     assert hasattr(rpc_client, "something")
 
     res = rpc_client.test_endpoint("spam")
@@ -186,7 +191,28 @@
 
     assert str(exc_info.value.args[0]["type"]) == "Exception"
     assert str(exc_info.value.args[0]["message"]) == error_message
     if status_code in (502, 503):
         assert isinstance(exc_info.value, TransientRemoteException)
     else:
         assert not isinstance(exc_info.value, TransientRemoteException)
+
+
+@pytest.mark.parametrize(
+    "timeout_arg,timeout_value",
+    [
+        pytest.param(None, None, id="default"),
+        pytest.param(1.0, 1.0, id="float"),
+        pytest.param((1, 2), (1, 2), id="tuple"),
+        pytest.param([1, 2], (1, 2), id="list"),
+    ],
+)
+def test_client_timeout_param(rpc_client_class, timeout_arg, timeout_value):
+    client = rpc_client_class(url="mock://example.com/", timeout=timeout_arg)
+    assert client.timeout == timeout_value
+
+
+def test_client_timeout_valueerror(rpc_client_class):
+    for timeout in ([], [1], [1, 2, 3]):
+        with pytest.raises(ValueError) as exc:
+            rpc_client_class(url="mock://example.com/", timeout=timeout)
+        assert repr(timeout) in str(exc.value)
```

### Comparing `swh_core-3.0.1/swh/core/api/tests/test_rpc_client_server.py` & `swh_core-3.1.0/swh/core/api/tests/test_rpc_client_server.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/tests/test_rpc_server.py` & `swh_core-3.1.0/swh/core/api/tests/test_rpc_server.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/tests/test_rpc_server_asynchronous.py` & `swh_core-3.1.0/swh/core/api/tests/test_rpc_server_asynchronous.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/api/tests/test_serializers.py` & `swh_core-3.1.0/swh/core/api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/cli/__init__.py` & `swh_core-3.1.0/swh/core/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/cli/db.py` & `swh_core-3.1.0/swh/core/cli/db.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/collections.py` & `swh_core-3.1.0/swh/core/collections.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/config.py` & `swh_core-3.1.0/swh/core/config.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/db/__init__.py` & `swh_core-3.1.0/swh/core/db/__init__.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/db/common.py` & `swh_core-3.1.0/swh/core/db/common.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/db/db_utils.py` & `swh_core-3.1.0/swh/core/db/db_utils.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/db/sql/35-dbversion.sql` & `swh_core-3.1.0/swh/core/db/sql/35-dbversion.sql`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/db/sql/36-dbmodule.sql` & `swh_core-3.1.0/swh/core/db/sql/36-dbmodule.sql`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/db/tests/conftest.py` & `swh_core-3.1.0/swh/core/db/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/db/tests/data/cli/sql/15-flavor.sql` & `swh_core-3.1.0/swh/core/db/tests/data/cli/sql/15-flavor.sql`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/db/tests/test_cli.py` & `swh_core-3.1.0/swh/core/db/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/db/tests/test_db.py` & `swh_core-3.1.0/swh/core/db/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/db/tests/test_db_utils.py` & `swh_core-3.1.0/swh/core/db/tests/test_db_utils.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/github/pytest_plugin.py` & `swh_core-3.1.0/swh/core/github/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/github/tests/test_github_utils.py` & `swh_core-3.1.0/swh/core/github/tests/test_github_utils.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/github/tests/test_pytest_plugin.py` & `swh_core-3.1.0/swh/core/github/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/github/utils.py` & `swh_core-3.1.0/swh/core/github/utils.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/logger.py` & `swh_core-3.1.0/swh/core/logger.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/logging.py` & `swh_core-3.1.0/swh/core/logging.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/pytest_plugin.py` & `swh_core-3.1.0/swh/core/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/retry.py` & `swh_core-3.1.0/swh/core/retry.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/sentry.py` & `swh_core-3.1.0/swh/core/sentry.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/statsd.py` & `swh_core-3.1.0/swh/core/statsd.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tarball.py` & `swh_core-3.1.0/swh/core/tarball.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/data/archives/ca-certificates-20210603-1-any.pkg.tar.zst` & `swh_core-3.1.0/swh/core/tests/data/archives/ca-certificates-20210603-1-any.pkg.tar.zst`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/data/archives/groff-1.02.tar.Z` & `swh_core-3.1.0/swh/core/tests/data/archives/groff-1.02.tar.Z`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/data/archives/hello.jar` & `swh_core-3.1.0/swh/core/tests/data/archives/hello.jar`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/data/archives/hello.tar` & `swh_core-3.1.0/swh/core/tests/data/archives/hello.tar`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/data/archives/hello.tar.x` & `swh_core-3.1.0/swh/core/tests/data/archives/hello.tar.x`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/data/archives/hello.war` & `swh_core-3.1.0/swh/core/tests/data/archives/hello.war`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/data/archives/msk316src.zip` & `swh_core-3.1.0/swh/core/tests/data/archives/msk316src.zip`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/data/archives/tokei-12.1.2.crate` & `swh_core-3.1.0/swh/core/tests/data/archives/tokei-12.1.2.crate`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/data/logging-config.yaml` & `swh_core-3.1.0/swh/core/tests/data/logging-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/fixture/test_pytest_plugin.py` & `swh_core-3.1.0/swh/core/tests/fixture/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/test_cli.py` & `swh_core-3.1.0/swh/core/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/test_collections.py` & `swh_core-3.1.0/swh/core/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/test_config.py` & `swh_core-3.1.0/swh/core/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/test_logger.py` & `swh_core-3.1.0/swh/core/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/test_logging.py` & `swh_core-3.1.0/swh/core/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/test_pytest_plugin.py` & `swh_core-3.1.0/swh/core/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/test_retry.py` & `swh_core-3.1.0/swh/core/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/test_sentry.py` & `swh_core-3.1.0/swh/core/tests/test_sentry.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/test_statsd.py` & `swh_core-3.1.0/swh/core/tests/test_statsd.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/test_tarball.py` & `swh_core-3.1.0/swh/core/tests/test_tarball.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/tests/test_utils.py` & `swh_core-3.1.0/swh/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh/core/utils.py` & `swh_core-3.1.0/swh/core/utils.py`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh.core.egg-info/PKG-INFO` & `swh_core-3.1.0/swh.core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.core
-Version: 3.0.1
+Version: 3.1.0
 Summary: Software Heritage core utilities
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-core
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-core/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-core/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-core.git
```

### Comparing `swh_core-3.0.1/swh.core.egg-info/SOURCES.txt` & `swh_core-3.1.0/swh.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/swh.core.egg-info/requires.txt` & `swh_core-3.1.0/swh.core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `swh_core-3.0.1/tox.ini` & `swh_core-3.1.0/tox.ini`

 * *Files identical despite different names*

