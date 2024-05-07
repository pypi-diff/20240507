# Comparing `tmp/newrelic-lambda-cli-0.9.0.tar.gz` & `tmp/newrelic_lambda_cli-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrelic-lambda-cli-0.9.0.tar", last modified: Fri Jan 26 02:31:35 2024, max compression
+gzip compressed data, was "newrelic_lambda_cli-0.9.1.tar", last modified: Tue May  7 07:50:28 2024, max compression
```

## Comparing `newrelic-lambda-cli-0.9.0.tar` & `newrelic_lambda_cli-0.9.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-26 02:31:35.727978 newrelic-lambda-cli-0.9.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3220 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2403 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/CONTRIBUTING.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11345 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21655 2024-01-26 02:31:35.727978 newrelic-lambda-cli-0.9.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21135 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9547 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/THIRD_PARTY_NOTICES.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-26 02:31:35.723978 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      149 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14848 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/api.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-26 02:31:35.727978 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cli/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      544 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1786 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cli/decorators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2601 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cli/functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10461 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cli/integrations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5678 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cli/layers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4067 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cli/subscriptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      902 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cliutils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2800 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30864 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/integrations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14263 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/layers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9093 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/permissions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6166 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/subscriptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-26 02:31:35.727978 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3771 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/templates/import-template.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1849 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/templates/license-key-secret.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2874 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/templates/nr-lambda-integration-role.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2304 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4855 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-26 02:31:35.727978 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21655 2024-01-26 02:31:35.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1328 2024-01-26 02:31:35.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-01-26 02:31:35.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2024-01-26 02:31:35.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-01-26 02:31:35.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2024-01-26 02:31:35.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2024-01-26 02:31:35.000000 newrelic-lambda-cli-0.9.0/newrelic_lambda_cli.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2024-01-26 02:31:35.727978 newrelic-lambda-cli-0.9.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-01-26 02:31:35.727978 newrelic-lambda-cli-0.9.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6327 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/tests/test_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2332 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/tests/test_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16699 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/tests/test_integrations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16069 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/tests/test_layers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/tests/test_new_relic_gql.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7112 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/tests/test_permissions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3990 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/tests/test_subscriptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2504 2024-01-26 02:31:24.000000 newrelic-lambda-cli-0.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:50:28.830241 newrelic_lambda_cli-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-05-07 07:50:28.830241 newrelic_lambda_cli-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21178 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/THIRD_PARTY_NOTICES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:50:28.826241 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:50:28.830241 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cli/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cli/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cli/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cli/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cliutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30864 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14270 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/subscriptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:50:28.830241 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/templates/import-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/templates/license-key-secret.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/templates/nr-lambda-integration-role.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:50:28.830241 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-05-07 07:50:28.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-07 07:50:28.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:50:28.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 07:50:28.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:50:28.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 07:50:28.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 07:50:28.000000 newrelic_lambda_cli-0.9.1/newrelic_lambda_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 07:50:28.830241 newrelic_lambda_cli-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:50:28.830241 newrelic_lambda_cli-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16699 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/tests/test_new_relic_gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/tests/test_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-07 07:50:21.000000 newrelic_lambda_cli-0.9.1/tests/test_utils.py
```

### Comparing `newrelic-lambda-cli-0.9.0/CODE_OF_CONDUCT.md` & `newrelic_lambda_cli-0.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/CONTRIBUTING.md` & `newrelic_lambda_cli-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/LICENSE` & `newrelic_lambda_cli-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/PKG-INFO` & `newrelic_lambda_cli-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic-lambda-cli
-Version: 0.9.0
+Version: 0.9.1
 Summary: A CLI to install the New Relic AWS Lambda integration and layers.
 Home-page: https://github.com/newrelic/newrelic-lambda-cli
 Author: New Relic
 Author-email: serverless-dev@newrelic.com
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -42,36 +42,39 @@
 
 ## Features
 
 * Installs the New Relic AWS Lambda integration onto your AWS account
 * Installs and configures a New Relic AWS Lambda layer onto your AWS Lambda functions
 * Automatically selects the correct New Relic layer for your function's runtime and region
 * Wraps your AWS Lambda functions without requiring a code change
-* Supports Go, Java, .NET, Node.js and Python AWS Lambda runtimes
+* Supports Go, Java, .NET, Node.js, Python, and Ruby AWS Lambda runtimes
 * Easily uninstall the AWS Lambda layer with a single command
 
 ## Runtimes Supported
 
 * dotnetcore3.1
 * java8.al2
 * java11
 * java17
+* java21
 * nodejs16.x
 * nodejs18.x
 * nodejs20.x
 * provided
 * provided.al2
 * python3.7
 * python3.8
 * python3.9
 * python3.10
 * python3.11
 * python3.12
+* ruby3.2
+* ruby3.3
 
-**Note:** Automatic handler wrapping is only supported for Node.js, Python and Java. For other runtimes,
+**Note:** Automatic handler wrapping is only supported for Node.js, Python, Java, and Ruby. For other runtimes,
 manual function wrapping is required using the runtime specific New Relic agent.
 
 ## Requirements
 
 * Python >= 3.3 <= 3.12
 * Retrieve your [New relic Account ID](https://docs.newrelic.com/docs/accounts/install-new-relic/account-setup/account-id) and [User API Key](https://docs.newrelic.com/docs/apis/get-started/intro-apis/types-new-relic-api-keys#user-api-key)
```

### Comparing `newrelic-lambda-cli-0.9.0/README.md` & `newrelic_lambda_cli-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,36 +24,39 @@
 
 ## Features
 
 * Installs the New Relic AWS Lambda integration onto your AWS account
 * Installs and configures a New Relic AWS Lambda layer onto your AWS Lambda functions
 * Automatically selects the correct New Relic layer for your function's runtime and region
 * Wraps your AWS Lambda functions without requiring a code change
-* Supports Go, Java, .NET, Node.js and Python AWS Lambda runtimes
+* Supports Go, Java, .NET, Node.js, Python, and Ruby AWS Lambda runtimes
 * Easily uninstall the AWS Lambda layer with a single command
 
 ## Runtimes Supported
 
 * dotnetcore3.1
 * java8.al2
 * java11
 * java17
+* java21
 * nodejs16.x
 * nodejs18.x
 * nodejs20.x
 * provided
 * provided.al2
 * python3.7
 * python3.8
 * python3.9
 * python3.10
 * python3.11
 * python3.12
+* ruby3.2
+* ruby3.3
 
-**Note:** Automatic handler wrapping is only supported for Node.js, Python and Java. For other runtimes,
+**Note:** Automatic handler wrapping is only supported for Node.js, Python, Java, and Ruby. For other runtimes,
 manual function wrapping is required using the runtime specific New Relic agent.
 
 ## Requirements
 
 * Python >= 3.3 <= 3.12
 * Retrieve your [New relic Account ID](https://docs.newrelic.com/docs/accounts/install-new-relic/account-setup/account-id) and [User API Key](https://docs.newrelic.com/docs/apis/get-started/intro-apis/types-new-relic-api-keys#user-api-key)
```

### Comparing `newrelic-lambda-cli-0.9.0/THIRD_PARTY_NOTICES.md` & `newrelic_lambda_cli-0.9.1/THIRD_PARTY_NOTICES.md`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/api.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/api.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cli/__init__.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cli/decorators.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cli/functions.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cli/functions.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cli/integrations.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cli/integrations.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cli/layers.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cli/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,28 +104,31 @@
     type=click.Choice(["handleRequest", "handleStreamsRequest"]),
 )
 @click.pass_context
 def install(ctx, **kwargs):
     """Install New Relic AWS Lambda Layers"""
     input = LayerInstall(session=None, verbose=ctx.obj["VERBOSE"], **kwargs)
 
-    input = input._replace(
-        session=boto3.Session(
-            profile_name=input.aws_profile, region_name=input.aws_region
-        )
-    )
-
     if input.aws_permissions_check:
         permissions.ensure_layer_install_permissions(input)
 
     functions = get_aliased_functions(input)
 
     with ThreadPoolExecutor() as executor:
         futures = [
-            executor.submit(layers.install, input, function) for function in functions
+            executor.submit(
+                layers.install,
+                input._replace(
+                    session=boto3.Session(
+                        profile_name=input.aws_profile, region_name=input.aws_region
+                    )
+                ),
+                function,
+            )
+            for function in functions
         ]
         install_success = all(future.result() for future in as_completed(futures))
 
     if install_success:
         done("Install Complete")
         if ctx.obj["VERBOSE"]:
             click.echo(
@@ -175,28 +178,31 @@
     multiple=True,
 )
 @click.pass_context
 def uninstall(ctx, **kwargs):
     """Uninstall New Relic AWS Lambda Layers"""
     input = LayerUninstall(session=None, verbose=ctx.obj["VERBOSE"], **kwargs)
 
-    input = input._replace(
-        session=boto3.Session(
-            profile_name=input.aws_profile, region_name=input.aws_region
-        )
-    )
-
     if input.aws_permissions_check:
         permissions.ensure_layer_uninstall_permissions(input)
 
     functions = get_aliased_functions(input)
 
     with ThreadPoolExecutor() as executor:
         futures = [
-            executor.submit(layers.uninstall, input, function) for function in functions
+            executor.submit(
+                layers.uninstall,
+                input._replace(
+                    session=boto3.Session(
+                        profile_name=input.aws_profile, region_name=input.aws_region
+                    )
+                ),
+                function,
+            )
+            for function in functions
         ]
         uninstall_success = all(future.result() for future in as_completed(futures))
 
     if uninstall_success:
         done("Uninstall Complete")
     else:
         failure("Uninstall Incomplete. See messages above for details.", exit=True)
```

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cli/subscriptions.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cli/subscriptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,28 +61,30 @@
     metavar="<pattern>",
     show_default=False,
 )
 def install(**kwargs):
     """Install New Relic AWS Lambda Log Subscriptions"""
     input = SubscriptionInstall(session=None, **kwargs)
 
-    input = input._replace(
-        session=boto3.Session(
-            profile_name=input.aws_profile, region_name=input.aws_region
-        )
-    )
-
     if input.aws_permissions_check:
         permissions.ensure_subscription_install_permissions(input)
 
     functions = get_aliased_functions(input)
 
     with ThreadPoolExecutor() as executor:
         futures = [
-            executor.submit(subscriptions.create_log_subscription, input, function)
+            executor.submit(
+                subscriptions.create_log_subscription,
+                input._replace(
+                    session=boto3.Session(
+                        profile_name=input.aws_profile, region_name=input.aws_region
+                    )
+                ),
+                function,
+            )
             for function in functions
         ]
         install_success = all(future.result() for future in as_completed(futures))
 
     if install_success:
         done("Install Complete")
     else:
@@ -116,28 +118,30 @@
     metavar="<name>",
     multiple=True,
 )
 def uninstall(**kwargs):
     """Uninstall New Relic AWS Lambda Log Subscriptions"""
     input = SubscriptionUninstall(session=None, **kwargs)
 
-    input = input._replace(
-        session=boto3.Session(
-            profile_name=input.aws_profile, region_name=input.aws_region
-        )
-    )
-
     if input.aws_permissions_check:
         permissions.ensure_subscription_uninstall_permissions(input)
 
     functions = get_aliased_functions(input)
 
     with ThreadPoolExecutor() as executor:
         futures = [
-            executor.submit(subscriptions.remove_log_subscription, input, function)
+            executor.submit(
+                subscriptions.remove_log_subscription,
+                input._replace(
+                    session=boto3.Session(
+                        profile_name=input.aws_profile, region_name=input.aws_region
+                    )
+                ),
+                function,
+            )
             for function in functions
         ]
         uninstall_success = all(future.result() for future in as_completed(futures))
 
     if uninstall_success:
         done("Uninstall Complete")
     else:
```

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/cliutils.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/cliutils.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/functions.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/functions.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/integrations.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/integrations.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/layers.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     }
 
     # We don't want to modify the handler if the NewRelicLambdaExtension layer
     # has been selected
     if any("NewRelicLambdaExtension" in s for s in new_relic_layer):
         runtime_handler = None
 
-    # Only used by Python, Node.js and Java runtimes not using the
+    # Only used by Python, Node.js, Ruby, and Java runtimes not using the
     # NewRelicLambdaExtension layer
     if runtime_handler:
         update_kwargs["Handler"] = runtime_handler
 
     # Update the account id
     update_kwargs["Environment"]["Variables"]["NEW_RELIC_ACCOUNT_ID"] = str(
         input.nr_account_id
```

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/permissions.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/permissions.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/subscriptions.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/subscriptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/templates/import-template.yaml` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/templates/import-template.yaml`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/templates/license-key-secret.yaml` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/templates/license-key-secret.yaml`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/templates/nr-lambda-integration-role.yaml` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/templates/nr-lambda-integration-role.yaml`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/types.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/types.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli/utils.py` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 import botocore
 import click
 
 NR_DOCS_ACT_LINKING_URL = "https://docs.newrelic.com/docs/serverless-function-monitoring/aws-lambda-monitoring/enable-lambda-monitoring/account-linking/#manually-configuring-the-license-key-secret"
 NEW_RELIC_ARN_PREFIX_TEMPLATE = "arn:aws:lambda:%s:451483290750"
 RUNTIME_CONFIG = {
     "dotnetcore3.1": {"LambdaExtension": True},
+    "java21": {
+        "Handler": "com.newrelic.java.HandlerWrapper::",
+        "LambdaExtension": True,
+    },
     "java17": {
         "Handler": "com.newrelic.java.HandlerWrapper::",
         "LambdaExtension": True,
     },
     "java11": {
         "Handler": "com.newrelic.java.HandlerWrapper::",
         "LambdaExtension": True,
@@ -32,14 +36,15 @@
     },
     "nodejs20.x": {
         "Handler": "newrelic-lambda-wrapper.handler",
         "LambdaExtension": True,
     },
     "provided": {"LambdaExtension": True},
     "provided.al2": {"LambdaExtension": True},
+    "provided.al2023": {"LambdaExtension": True},
     "python3.7": {
         "Handler": "newrelic_lambda_wrapper.handler",
         "LambdaExtension": True,
     },
     "python3.8": {
         "Handler": "newrelic_lambda_wrapper.handler",
         "LambdaExtension": True,
@@ -56,14 +61,22 @@
         "Handler": "newrelic_lambda_wrapper.handler",
         "LambdaExtension": True,
     },
     "python3.12": {
         "Handler": "newrelic_lambda_wrapper.handler",
         "LambdaExtension": True,
     },
+    "ruby3.2": {
+        "Handler": "newrelic_lambda_wrapper.handler",
+        "LambdaExtension": True,
+    },
+    "ruby3.3": {
+        "Handler": "newrelic_lambda_wrapper.handler",
+        "LambdaExtension": True,
+    },
 }
 
 
 def catch_boto_errors(func):
     def _boto_error_wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
```

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli.egg-info/PKG-INFO` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic-lambda-cli
-Version: 0.9.0
+Version: 0.9.1
 Summary: A CLI to install the New Relic AWS Lambda integration and layers.
 Home-page: https://github.com/newrelic/newrelic-lambda-cli
 Author: New Relic
 Author-email: serverless-dev@newrelic.com
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -42,36 +42,39 @@
 
 ## Features
 
 * Installs the New Relic AWS Lambda integration onto your AWS account
 * Installs and configures a New Relic AWS Lambda layer onto your AWS Lambda functions
 * Automatically selects the correct New Relic layer for your function's runtime and region
 * Wraps your AWS Lambda functions without requiring a code change
-* Supports Go, Java, .NET, Node.js and Python AWS Lambda runtimes
+* Supports Go, Java, .NET, Node.js, Python, and Ruby AWS Lambda runtimes
 * Easily uninstall the AWS Lambda layer with a single command
 
 ## Runtimes Supported
 
 * dotnetcore3.1
 * java8.al2
 * java11
 * java17
+* java21
 * nodejs16.x
 * nodejs18.x
 * nodejs20.x
 * provided
 * provided.al2
 * python3.7
 * python3.8
 * python3.9
 * python3.10
 * python3.11
 * python3.12
+* ruby3.2
+* ruby3.3
 
-**Note:** Automatic handler wrapping is only supported for Node.js, Python and Java. For other runtimes,
+**Note:** Automatic handler wrapping is only supported for Node.js, Python, Java, and Ruby. For other runtimes,
 manual function wrapping is required using the runtime specific New Relic agent.
 
 ## Requirements
 
 * Python >= 3.3 <= 3.12
 * Retrieve your [New relic Account ID](https://docs.newrelic.com/docs/accounts/install-new-relic/account-setup/account-id) and [User API Key](https://docs.newrelic.com/docs/apis/get-started/intro-apis/types-new-relic-api-keys#user-api-key)
```

### Comparing `newrelic-lambda-cli-0.9.0/newrelic_lambda_cli.egg-info/SOURCES.txt` & `newrelic_lambda_cli-0.9.1/newrelic_lambda_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/setup.py` & `newrelic_lambda_cli-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_packages, setup
 
 README = open(os.path.join(os.path.dirname(__file__), "README.md"), "r").read()
 
 setup(
     name="newrelic-lambda-cli",
-    version="0.9.0",
+    version="0.9.1",
     python_requires=">=3.3",
     description="A CLI to install the New Relic AWS Lambda integration and layers.",
     long_description=README,
     long_description_content_type="text/markdown",
     author="New Relic",
     author_email="serverless-dev@newrelic.com",
     url="https://github.com/newrelic/newrelic-lambda-cli",
```

### Comparing `newrelic-lambda-cli-0.9.0/tests/test_api.py` & `newrelic_lambda_cli-0.9.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/tests/test_functions.py` & `newrelic_lambda_cli-0.9.1/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/tests/test_integrations.py` & `newrelic_lambda_cli-0.9.1/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/tests/test_layers.py` & `newrelic_lambda_cli-0.9.1/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/tests/test_new_relic_gql.py` & `newrelic_lambda_cli-0.9.1/tests/test_new_relic_gql.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/tests/test_permissions.py` & `newrelic_lambda_cli-0.9.1/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/tests/test_subscriptions.py` & `newrelic_lambda_cli-0.9.1/tests/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.9.0/tests/test_utils.py` & `newrelic_lambda_cli-0.9.1/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 
 
 def test_supports_lambda_extension():
     assert all(
         supports_lambda_extension(runtime)
         for runtime in (
             "dotnetcore3.1",
+            "java21",
             "java17",
             "java11",
             "java8.al2",
             "nodejs16.x",
             "nodejs18.x",
             "nodejs20.x",
             "provided",
```

