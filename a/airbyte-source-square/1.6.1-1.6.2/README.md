# Comparing `tmp/airbyte-source-square-1.6.1.tar.gz` & `tmp/airbyte_source_square-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-square-1.6.1.tar", last modified: Wed Jan 31 17:55:07 2024, max compression
+gzip compressed data, was "airbyte_source_square-1.6.2.tar", max compression
```

## Comparing `airbyte-source-square-1.6.1.tar` & `airbyte_source_square-1.6.2.tar`

### file list

```diff
@@ -1,59 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 17:55:07.693086 airbyte-source-square-1.6.1/
--rw-r--r--   0 root         (0) root         (0)     4215 2024-01-31 17:55:07.693086 airbyte-source-square-1.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3993 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 17:55:07.693086 airbyte-source-square-1.6.1/airbyte_source_square.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4215 2024-01-31 17:55:07.000000 airbyte-source-square-1.6.1/airbyte_source_square.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1938 2024-01-31 17:55:07.000000 airbyte-source-square-1.6.1/airbyte_source_square.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 17:55:07.000000 airbyte-source-square-1.6.1/airbyte_source_square.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-01-31 17:55:07.000000 airbyte-source-square-1.6.1/airbyte_source_square.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-01-31 17:55:07.000000 airbyte-source-square-1.6.1/airbyte_source_square.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-01-31 17:55:07.000000 airbyte-source-square-1.6.1/airbyte_source_square.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 17:55:07.681086 airbyte-source-square-1.6.1/integration_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1354 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      314 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     5919 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)     4526 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/configured_catalog_oauth.json
--rw-r--r--   0 root         (0) root         (0)      115 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      473 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/state.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 17:55:07.685086 airbyte-source-square-1.6.1/integration_tests/test_streams/
--rw-r--r--   0 root         (0) root         (0)     1193 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/test_streams/categories.json
--rw-r--r--   0 root         (0) root         (0)     3743 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/test_streams/customers.json
--rw-r--r--   0 root         (0) root         (0)     2236 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/test_streams/discounts.json
--rw-r--r--   0 root         (0) root         (0)     7280 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/test_streams/items.json
--rw-r--r--   0 root         (0) root         (0)     2913 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/test_streams/locations.json
--rw-r--r--   0 root         (0) root         (0)     3395 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/test_streams/modifier_list.json
--rw-r--r--   0 root         (0) root         (0)    30582 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/test_streams/orders.json
--rw-r--r--   0 root         (0) root         (0)     6412 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/test_streams/payments.json
--rw-r--r--   0 root         (0) root         (0)     2244 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/test_streams/refunds.json
--rw-r--r--   0 root         (0) root         (0)     2836 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/test_streams/shifts.json
--rw-r--r--   0 root         (0) root         (0)     2064 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/test_streams/taxes.json
--rw-r--r--   0 root         (0) root         (0)     1007 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/test_streams/team_member_wages.json
--rw-r--r--   0 root         (0) root         (0)     1515 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/integration_tests/test_streams/team_members.json
--rw-r--r--   0 root         (0) root         (0)     4032 2024-01-31 17:55:07.693086 airbyte-source-square-1.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      942 2024-01-31 17:55:05.000000 airbyte-source-square-1.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 17:55:07.689086 airbyte-source-square-1.6.1/source_square/
--rw-r--r--   0 root         (0) root         (0)      124 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3732 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/components.py
--rw-r--r--   0 root         (0) root         (0)    12108 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 17:55:07.693086 airbyte-source-square-1.6.1/source_square/schemas/
--rw-r--r--   0 root         (0) root         (0)      933 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/bank_accounts.json
--rw-r--r--   0 root         (0) root         (0)     1234 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/cash_drawers.json
--rw-r--r--   0 root         (0) root         (0)      574 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/categories.json
--rw-r--r--   0 root         (0) root         (0)     2480 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/customers.json
--rw-r--r--   0 root         (0) root         (0)     1362 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/discounts.json
--rw-r--r--   0 root         (0) root         (0)      547 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/inventory.json
--rw-r--r--   0 root         (0) root         (0)     5378 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/items.json
--rw-r--r--   0 root         (0) root         (0)     1842 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/locations.json
--rw-r--r--   0 root         (0) root         (0)      884 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/loyalty.json
--rw-r--r--   0 root         (0) root         (0)     2317 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/modifier_list.json
--rw-r--r--   0 root         (0) root         (0)    23335 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/orders.json
--rw-r--r--   0 root         (0) root         (0)     4512 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/payments.json
--rw-r--r--   0 root         (0) root         (0)     1398 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/refunds.json
--rw-r--r--   0 root         (0) root         (0)     1808 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/shifts.json
--rw-r--r--   0 root         (0) root         (0)     1234 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/taxes.json
--rw-r--r--   0 root         (0) root         (0)      456 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/team_member_wages.json
--rw-r--r--   0 root         (0) root         (0)      825 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/schemas/team_members.json
--rw-r--r--   0 root         (0) root         (0)      475 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/source.py
--rw-r--r--   0 root         (0) root         (0)     3451 2024-01-31 17:51:56.000000 airbyte-source-square-1.6.1/source_square/spec.yaml
+-rw-r--r--   0        0        0     4496 2024-05-07 07:35:59.542919 airbyte_source_square-1.6.2/README.md
+-rw-r--r--   0        0        0      760 2024-05-07 07:39:02.267299 airbyte_source_square-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/__init__.py
+-rw-r--r--   0        0        0    12116 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/manifest.yaml
+-rw-r--r--   0        0        0      230 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/run.py
+-rw-r--r--   0        0        0      726 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/TODO.md
+-rw-r--r--   0        0        0      933 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/bank_accounts.json
+-rw-r--r--   0        0        0     1234 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/cash_drawers.json
+-rw-r--r--   0        0        0      574 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/categories.json
+-rw-r--r--   0        0        0     2480 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/customers.json
+-rw-r--r--   0        0        0     1362 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/discounts.json
+-rw-r--r--   0        0        0      547 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/inventory.json
+-rw-r--r--   0        0        0     5378 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/items.json
+-rw-r--r--   0        0        0     1842 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/locations.json
+-rw-r--r--   0        0        0      884 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/loyalty.json
+-rw-r--r--   0        0        0     2317 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/modifier_list.json
+-rw-r--r--   0        0        0    23335 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/orders.json
+-rw-r--r--   0        0        0     4512 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/payments.json
+-rw-r--r--   0        0        0     1398 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/refunds.json
+-rw-r--r--   0        0        0     1808 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/shifts.json
+-rw-r--r--   0        0        0     1234 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/taxes.json
+-rw-r--r--   0        0        0      456 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/team_member_wages.json
+-rw-r--r--   0        0        0      825 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/schemas/team_members.json
+-rw-r--r--   0        0        0      475 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/source.py
+-rw-r--r--   0        0        0     3451 2024-05-07 07:35:59.546918 airbyte_source_square-1.6.2/source_square/spec.yaml
+-rw-r--r--   0        0        0     5198 1970-01-01 00:00:00.000000 airbyte_source_square-1.6.2/PKG-INFO
```

### Comparing `airbyte-source-square-1.6.1/PKG-INFO` & `airbyte_source_square-1.6.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-square
-Version: 1.6.1
+Version: 1.6.2
 Summary: Source implementation for Square.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (>=0,<1)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/square
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk>=0.51.31
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: freezegun; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Square Source
+# Square source connector
 
-This is the repository for the Square configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/square).
 
+This is the repository for the Square source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/square).
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/square)
+## Local development
+
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/square)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_square/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source square test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-square spec
+poetry run source-square check --config secrets/config.json
+poetry run source-square discover --config secrets/config.json
+poetry run source-square read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-square build
 ```
 
-An image will be built with the tag `airbyte/source-square:dev`.
+An image will be available on your host with the tag `airbyte/source-square:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-square:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-square:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-square:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-square:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-square:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-square test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-square test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/square.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/square.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-square-1.6.1/README.md` & `airbyte_source_square-1.6.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,91 @@
-# Square Source
+# Square source connector
 
-This is the repository for the Square configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/square).
+
+This is the repository for the Square source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/square).
 
 ## Local development
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/square)
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/square)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_square/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source square test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
+```
+poetry run source-square spec
+poetry run source-square check --config secrets/config.json
+poetry run source-square discover --config secrets/config.json
+poetry run source-square read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-square build
 ```
 
-An image will be built with the tag `airbyte/source-square:dev`.
+An image will be available on your host with the tag `airbyte/source-square:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-square:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-square:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-square:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-square:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-square:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-square test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
 
-### Publishing a new version of the connector
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-square test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/square.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/square.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-square-1.6.1/integration_tests/test_streams/categories.json` & `airbyte_source_square-1.6.2/source_square/schemas/discounts.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('type', ['null', 'object']), ('properties', OrderedDict([('type', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('id', OrderedDict([('type', ['null', "*

 * *            "'string'])])), ('updated_at', OrderedDict([('type', ['null', 'string'])])), "*

 * *            "('version', OrderedDict([('type', ['null', 'integer'])])), ('is_deleted', "*

 * *            "OrderedDict([('type', ['null', 'boolean'])])), ('present_at_all_locations', "*

 * *            "OrderedDict([('type', ['null', 'bo […]*

```diff
@@ -1,80 +1,120 @@
 {
-    "streams": [
-        {
-            "cursor_field": [
-                "updated_at"
-            ],
-            "destination_sync_mode": "append",
-            "stream": {
-                "default_cursor_field": [
-                    "updated_at"
-                ],
-                "json_schema": {
+    "properties": {
+        "discount_data": {
+            "properties": {
+                "amount_money": {
                     "properties": {
-                        "category_data": {
-                            "properties": {
-                                "name": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
+                        "amount": {
                             "type": [
                                 "null",
-                                "object"
-                            ]
-                        },
-                        "id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "is_deleted": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        },
-                        "present_at_all_locations": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        },
-                        "type": {
-                            "type": [
-                                "null",
-                                "string"
+                                "integer"
                             ]
                         },
-                        "updated_at": {
+                        "currency": {
                             "type": [
                                 "null",
                                 "string"
                             ]
-                        },
-                        "version": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
                         }
                     },
                     "type": [
                         "null",
                         "object"
                     ]
                 },
-                "name": "categories",
-                "source_defined_cursor": true,
-                "supported_sync_modes": [
-                    "incremental",
-                    "full_refresh"
+                "application_method": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "discount_type": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "modify_tax_basis": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "name": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "percentage": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "pin_required": {
+                    "type": [
+                        "null",
+                        "boolean"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "is_deleted": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "present_at_all_locations": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "present_at_location_ids": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
                 ]
             },
-            "sync_mode": "incremental"
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "type": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "updated_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "version": {
+            "type": [
+                "null",
+                "integer"
+            ]
         }
+    },
+    "type": [
+        "null",
+        "object"
     ]
 }
```

### Comparing `airbyte-source-square-1.6.1/integration_tests/test_streams/customers.json` & `airbyte_source_square-1.6.2/source_square/schemas/modifier_list.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('type', ['null', 'object']), ('properties', OrderedDict([('type', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('id', OrderedDict([('type', ['null', "*

 * *            "'string'])])), ('updated_at', OrderedDict([('type', ['null', 'string'])])), "*

 * *            "('version', OrderedDict([('type', ['null', 'integer'])])), ('is_deleted', "*

 * *            "OrderedDict([('type', ['null', 'boolean'])])), ('present_at_all_locations', "*

 * *            "OrderedDict([('type', ['null', 'bo […]*

```diff
@@ -1,238 +1,166 @@
 {
-    "streams": [
-        {
-            "cursor_field": [
-                "id"
-            ],
-            "destination_sync_mode": "overwrite",
-            "stream": {
-                "default_cursor_field": [
-                    "id"
-                ],
-                "json_schema": {
-                    "properties": {
-                        "address": {
-                            "properties": {
-                                "address_line_1": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "address_line_2": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "administrative_district_level_1": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "locality": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "postal_code": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "birthday": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "cards": {
-                            "items": {
+    "properties": {
+        "id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "is_deleted": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "modifier_list_data": {
+            "properties": {
+                "modifiers": {
+                    "items": {
+                        "properties": {
+                            "id": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "is_deleted": {
+                                "type": [
+                                    "null",
+                                    "boolean"
+                                ]
+                            },
+                            "modifier_data": {
                                 "properties": {
-                                    "billing_address": {
-                                        "properties": {
-                                            "postal_code": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "card_brand": {
+                                    "modifier_list_id": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
                                     },
-                                    "cardholder_name": {
+                                    "name": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
                                     },
-                                    "exp_month": {
+                                    "on_by_default": {
                                         "type": [
                                             "null",
-                                            "integer"
+                                            "boolean"
                                         ]
                                     },
-                                    "exp_year": {
+                                    "ordinal": {
                                         "type": [
                                             "null",
                                             "integer"
                                         ]
                                     },
-                                    "id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "last_4": {
+                                    "price_money": {
+                                        "properties": {
+                                            "amount": {
+                                                "type": [
+                                                    "null",
+                                                    "integer"
+                                                ]
+                                            },
+                                            "currency": {
+                                                "type": [
+                                                    "null",
+                                                    "string"
+                                                ]
+                                            }
+                                        },
                                         "type": [
                                             "null",
-                                            "string"
+                                            "object"
                                         ]
                                     }
                                 },
                                 "type": [
                                     "null",
                                     "object"
                                 ]
                             },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "company_name": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "created_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "creation_source": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "email_address": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "family_name": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "given_name": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "group_ids": {
-                            "items": {
+                            "present_at_all_locations": {
+                                "type": [
+                                    "null",
+                                    "boolean"
+                                ]
+                            },
+                            "type": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
                             },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "phone_number": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "preferences": {
-                            "properties": {
-                                "email_unsubscribed": {
-                                    "type": "boolean"
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "reference_id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "segment_ids": {
-                            "items": {
+                            "updated_at": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
                             },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "updated_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
+                            "version": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            }
                         },
-                        "version": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        }
+                        "type": [
+                            "null",
+                            "object"
+                        ]
                     },
                     "type": [
                         "null",
-                        "object"
+                        "array"
                     ]
                 },
-                "name": "customers",
-                "source_defined_cursor": true,
-                "supported_sync_modes": [
-                    "full_refresh"
-                ]
+                "name": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "selection_type": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
             },
-            "sync_mode": "full_refresh"
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "present_at_all_locations": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "type": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "updated_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "version": {
+            "type": [
+                "null",
+                "integer"
+            ]
         }
+    },
+    "type": [
+        "null",
+        "object"
     ]
 }
```

### Comparing `airbyte-source-square-1.6.1/integration_tests/test_streams/discounts.json` & `airbyte_source_square-1.6.2/source_square/schemas/refunds.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('type', ['null', 'object']), ('properties', OrderedDict([('id', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('status', OrderedDict([('type', "*

 * *            "['null', 'string'])])), ('amount_money', OrderedDict([('type', ['null', 'object']), "*

 * *            "('properties', OrderedDict([('amount', OrderedDict([('type', ['null', 'integer'])])), "*

 * *            "('currency', OrderedDict([('type', ['null', 'string'])]))])), ('required', ['amount', "*

 * *            "'currency'] […]*

```diff
@@ -1,142 +1,126 @@
 {
-    "streams": [
-        {
-            "cursor_field": [
-                "updated_at"
+    "properties": {
+        "amount_money": {
+            "properties": {
+                "amount": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "currency": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "required": [
+                "amount",
+                "currency"
             ],
-            "destination_sync_mode": "append",
-            "stream": {
-                "default_cursor_field": [
-                    "updated_at"
-                ],
-                "json_schema": {
-                    "properties": {
-                        "discount_data": {
-                            "properties": {
-                                "amount_money": {
-                                    "properties": {
-                                        "amount": {
-                                            "type": [
-                                                "null",
-                                                "integer"
-                                            ]
-                                        },
-                                        "currency": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                },
-                                "application_method": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "discount_type": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "modify_tax_basis": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "name": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "percentage": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "pin_required": {
-                                    "type": [
-                                        "null",
-                                        "boolean"
-                                    ]
-                                }
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "created_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "location_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "order_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "payment_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "processing_fee": {
+            "items": {
+                "properties": {
+                    "amount_money": {
+                        "properties": {
+                            "amount": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
                             },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "is_deleted": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        },
-                        "present_at_all_locations": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        },
-                        "present_at_location_ids": {
-                            "items": {
+                            "currency": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
-                            },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "type": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
+                            }
                         },
-                        "updated_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "version": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        }
+                        "type": [
+                            "null",
+                            "object"
+                        ]
                     },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
+                    "effective_at": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "type": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
                 },
-                "name": "discounts",
-                "source_defined_cursor": true,
-                "supported_sync_modes": [
-                    "incremental",
-                    "full_refresh"
+                "type": [
+                    "null",
+                    "object"
                 ]
             },
-            "sync_mode": "incremental"
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "reason": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "status": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "updated_at": {
+            "type": [
+                "null",
+                "string"
+            ]
         }
+    },
+    "type": [
+        "null",
+        "object"
     ]
 }
```

### Comparing `airbyte-source-square-1.6.1/integration_tests/test_streams/items.json` & `airbyte_source_square-1.6.2/source_square/schemas/items.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('type', ['null', 'object']), ('properties', OrderedDict([('type', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('id', OrderedDict([('type', ['null', "*

 * *            "'string'])])), ('updated_at', OrderedDict([('type', ['null', 'string'])])), "*

 * *            "('version', OrderedDict([('type', ['null', 'integer'])])), ('is_deleted', "*

 * *            "OrderedDict([('type', ['null', 'boolean'])])), ('custom_attribute_values', "*

 * *            "OrderedDict([('type', ['null', 'obj […]*

```diff
@@ -1,388 +1,366 @@
 {
-    "streams": [
-        {
-            "cursor_field": [
-                "updated_at"
-            ],
-            "destination_sync_mode": "append",
-            "stream": {
-                "default_cursor_field": [
-                    "updated_at"
-                ],
-                "json_schema": {
-                    "properties": {
-                        "custom_attribute_values": {
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "image_id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
+    "properties": {
+        "custom_attribute_values": {
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "image_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "is_deleted": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "item_data": {
+            "properties": {
+                "category_id": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "description": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "ecom_visibility": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "item_options": {
+                    "items": {
+                        "properties": {
+                            "item_option_id": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
                         },
-                        "is_deleted": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "type": [
+                        "null",
+                        "array"
+                    ]
+                },
+                "modifier_list_info": {
+                    "items": {
+                        "properties": {
+                            "enabled": {
+                                "type": [
+                                    "null",
+                                    "boolean"
+                                ]
+                            },
+                            "max_selected_modifiers": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "min_selected_modifiers": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "modifier_list_id": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "visibility": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
                         },
-                        "item_data": {
-                            "properties": {
-                                "category_id": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "description": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "ecom_visibility": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "item_options": {
-                                    "items": {
-                                        "properties": {
-                                            "item_option_id": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "type": [
+                        "null",
+                        "array"
+                    ]
+                },
+                "name": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "product_type": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "skip_modifier_screen": {
+                    "type": [
+                        "null",
+                        "boolean"
+                    ]
+                },
+                "tax_ids": {
+                    "items": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "type": [
+                        "null",
+                        "array"
+                    ]
+                },
+                "variations": {
+                    "items": {
+                        "properties": {
+                            "id": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "is_deleted": {
+                                "type": [
+                                    "null",
+                                    "boolean"
+                                ]
+                            },
+                            "item_variation_data": {
+                                "properties": {
+                                    "item_id": {
                                         "type": [
                                             "null",
-                                            "object"
+                                            "string"
                                         ]
                                     },
-                                    "type": [
-                                        "null",
-                                        "array"
-                                    ]
-                                },
-                                "modifier_list_info": {
-                                    "items": {
-                                        "properties": {
-                                            "enabled": {
-                                                "type": [
-                                                    "null",
-                                                    "boolean"
-                                                ]
-                                            },
-                                            "max_selected_modifiers": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "min_selected_modifiers": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
+                                    "item_option_values": {
+                                        "items": {
+                                            "properties": {
+                                                "item_option_id": {
+                                                    "type": [
+                                                        "null",
+                                                        "string"
+                                                    ]
+                                                },
+                                                "item_option_value_id": {
+                                                    "type": [
+                                                        "null",
+                                                        "string"
+                                                    ]
+                                                }
                                             },
-                                            "modifier_list_id": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
+                                            "type": [
+                                                "null",
+                                                "object"
+                                            ]
+                                        },
+                                        "type": [
+                                            "null",
+                                            "array"
+                                        ]
+                                    },
+                                    "location_overrides": {
+                                        "items": {
+                                            "properties": {
+                                                "location_id": {
+                                                    "type": [
+                                                        "null",
+                                                        "string"
+                                                    ]
+                                                },
+                                                "track_inventory": {
+                                                    "type": [
+                                                        "null",
+                                                        "boolean"
+                                                    ]
+                                                }
                                             },
-                                            "visibility": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
+                                            "type": [
+                                                "null",
+                                                "object"
+                                            ]
                                         },
                                         "type": [
                                             "null",
-                                            "object"
+                                            "array"
                                         ]
                                     },
-                                    "type": [
-                                        "null",
-                                        "array"
-                                    ]
-                                },
-                                "name": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "product_type": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "skip_modifier_screen": {
-                                    "type": [
-                                        "null",
-                                        "boolean"
-                                    ]
-                                },
-                                "tax_ids": {
-                                    "items": {
+                                    "name": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
                                     },
-                                    "type": [
-                                        "null",
-                                        "array"
-                                    ]
-                                },
-                                "variations": {
-                                    "items": {
+                                    "ordinal": {
+                                        "type": [
+                                            "null",
+                                            "integer"
+                                        ]
+                                    },
+                                    "price_money": {
                                         "properties": {
-                                            "id": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "is_deleted": {
-                                                "type": [
-                                                    "null",
-                                                    "boolean"
-                                                ]
-                                            },
-                                            "item_variation_data": {
-                                                "properties": {
-                                                    "item_id": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    },
-                                                    "item_option_values": {
-                                                        "items": {
-                                                            "properties": {
-                                                                "item_option_id": {
-                                                                    "type": [
-                                                                        "null",
-                                                                        "string"
-                                                                    ]
-                                                                },
-                                                                "item_option_value_id": {
-                                                                    "type": [
-                                                                        "null",
-                                                                        "string"
-                                                                    ]
-                                                                }
-                                                            },
-                                                            "type": [
-                                                                "null",
-                                                                "object"
-                                                            ]
-                                                        },
-                                                        "type": [
-                                                            "null",
-                                                            "array"
-                                                        ]
-                                                    },
-                                                    "location_overrides": {
-                                                        "items": {
-                                                            "properties": {
-                                                                "location_id": {
-                                                                    "type": [
-                                                                        "null",
-                                                                        "string"
-                                                                    ]
-                                                                },
-                                                                "track_inventory": {
-                                                                    "type": [
-                                                                        "null",
-                                                                        "boolean"
-                                                                    ]
-                                                                }
-                                                            },
-                                                            "type": [
-                                                                "null",
-                                                                "object"
-                                                            ]
-                                                        },
-                                                        "type": [
-                                                            "null",
-                                                            "array"
-                                                        ]
-                                                    },
-                                                    "name": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    },
-                                                    "ordinal": {
-                                                        "type": [
-                                                            "null",
-                                                            "integer"
-                                                        ]
-                                                    },
-                                                    "price_money": {
-                                                        "properties": {
-                                                            "amount": {
-                                                                "type": [
-                                                                    "null",
-                                                                    "integer"
-                                                                ]
-                                                            },
-                                                            "currency": {
-                                                                "type": [
-                                                                    "null",
-                                                                    "string"
-                                                                ]
-                                                            }
-                                                        },
-                                                        "type": [
-                                                            "null",
-                                                            "object"
-                                                        ]
-                                                    },
-                                                    "pricing_type": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    },
-                                                    "sku": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    }
-                                                },
-                                                "type": [
-                                                    "null",
-                                                    "object"
-                                                ]
-                                            },
-                                            "present_at_all_locations": {
-                                                "type": [
-                                                    "null",
-                                                    "boolean"
-                                                ]
-                                            },
-                                            "present_at_location_ids": {
-                                                "items": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "type": [
-                                                    "null",
-                                                    "array"
-                                                ]
-                                            },
-                                            "type": {
+                                            "amount": {
                                                 "type": [
                                                     "null",
-                                                    "string"
+                                                    "integer"
                                                 ]
                                             },
-                                            "updated_at": {
+                                            "currency": {
                                                 "type": [
                                                     "null",
                                                     "string"
                                                 ]
-                                            },
-                                            "version": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
                                             }
                                         },
                                         "type": [
                                             "null",
                                             "object"
                                         ]
                                     },
-                                    "type": [
-                                        "null",
-                                        "array"
-                                    ]
+                                    "pricing_type": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    },
+                                    "sku": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    }
                                 },
-                                "visibility": {
+                                "type": [
+                                    "null",
+                                    "object"
+                                ]
+                            },
+                            "present_at_all_locations": {
+                                "type": [
+                                    "null",
+                                    "boolean"
+                                ]
+                            },
+                            "present_at_location_ids": {
+                                "items": {
                                     "type": [
                                         "null",
                                         "string"
                                     ]
-                                }
+                                },
+                                "type": [
+                                    "null",
+                                    "array"
+                                ]
                             },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "present_at_all_locations": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        },
-                        "present_at_location_ids": {
-                            "items": {
+                            "type": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
                             },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "type": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "updated_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
+                            "updated_at": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "version": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            }
                         },
-                        "version": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        }
+                        "type": [
+                            "null",
+                            "object"
+                        ]
                     },
                     "type": [
                         "null",
-                        "object"
+                        "array"
                     ]
                 },
-                "name": "items",
-                "source_defined_cursor": true,
-                "supported_sync_modes": [
-                    "incremental",
-                    "full_refresh"
+                "visibility": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "present_at_all_locations": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "present_at_location_ids": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
                 ]
             },
-            "sync_mode": "incremental"
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "type": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "updated_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "version": {
+            "type": [
+                "null",
+                "integer"
+            ]
         }
+    },
+    "type": [
+        "null",
+        "object"
     ]
 }
```

### Comparing `airbyte-source-square-1.6.1/integration_tests/test_streams/locations.json` & `airbyte_source_square-1.6.2/source_square/schemas/shifts.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('type', ['null', 'object']), ('properties', OrderedDict([('id', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('employee_id', OrderedDict([('type', "*

 * *            "['null', 'string'])])), ('location_id', OrderedDict([('type', ['null', 'string'])])), "*

 * *            "('timezone', OrderedDict([('type', ['null', 'string'])])), ('start_at', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('end_at', OrderedDict([('type', "*

 * *            "['null', 'string'])])), ( […]*

```diff
@@ -1,199 +1,164 @@
 {
-    "streams": [
-        {
-            "cursor_field": [
-                "id"
-            ],
-            "destination_sync_mode": "overwrite",
-            "stream": {
-                "default_cursor_field": [
-                    "id"
-                ],
-                "json_schema": {
+    "properties": {
+        "breaks": {
+            "items": {
+                "properties": {
+                    "break_type_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "end_at": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "expected_duration": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "is_paid": {
+                        "type": [
+                            "null",
+                            "boolean"
+                        ]
+                    },
+                    "name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "start_at": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "created_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "employee_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "end_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "location_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "start_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "status": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "team_member_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "timezone": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "updated_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "version": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "wage": {
+            "properties": {
+                "hourly_rate": {
                     "properties": {
-                        "address": {
-                            "properties": {
-                                "address_line_1": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "administrative_district_level_1": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "country": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "locality": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "postal_code": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "business_email": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "business_hours": {
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "business_name": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "capabilities": {
-                            "items": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "country": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "created_at": {
+                        "amount": {
                             "type": [
                                 "null",
-                                "string"
+                                "integer"
                             ]
                         },
                         "currency": {
                             "type": [
                                 "null",
                                 "string"
                             ]
-                        },
-                        "description": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "facebook_url": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "instagram_username": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "language_code": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "mcc": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "merchant_id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "name": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "phone_number": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "status": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "timezone": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "twitter_username": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "type": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "website_url": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
                         }
                     },
                     "type": [
                         "null",
                         "object"
                     ]
                 },
-                "name": "locations",
-                "source_defined_cursor": true,
-                "supported_sync_modes": [
-                    "full_refresh"
-                ]
+                "title": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
             },
-            "sync_mode": "full_refresh"
+            "type": [
+                "null",
+                "object"
+            ]
         }
+    },
+    "type": [
+        "null",
+        "object"
     ]
 }
```

### Comparing `airbyte-source-square-1.6.1/integration_tests/test_streams/modifier_list.json` & `airbyte_source_square-1.6.2/source_square/schemas/customers.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('type', ['null', 'object']), ('properties', OrderedDict([('id', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('created_at', OrderedDict([('type', "*

 * *            "['null', 'string'])])), ('updated_at', OrderedDict([('type', ['null', 'string'])])), "*

 * *            "('cards', OrderedDict([('type', ['null', 'array']), ('items', OrderedDict([('type', "*

 * *            "['null', 'object']), ('properties', OrderedDict([('id', OrderedDict([('type', "*

 * *            "['null', 'string […]*

```diff
@@ -1,188 +1,217 @@
 {
-    "streams": [
-        {
-            "cursor_field": [
-                "updated_at"
-            ],
-            "destination_sync_mode": "append",
-            "stream": {
-                "default_cursor_field": [
-                    "updated_at"
-                ],
-                "json_schema": {
-                    "properties": {
-                        "id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "is_deleted": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        },
-                        "modifier_list_data": {
-                            "properties": {
-                                "modifiers": {
-                                    "items": {
-                                        "properties": {
-                                            "id": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "is_deleted": {
-                                                "type": [
-                                                    "null",
-                                                    "boolean"
-                                                ]
-                                            },
-                                            "modifier_data": {
-                                                "properties": {
-                                                    "modifier_list_id": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    },
-                                                    "name": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    },
-                                                    "on_by_default": {
-                                                        "type": [
-                                                            "null",
-                                                            "boolean"
-                                                        ]
-                                                    },
-                                                    "ordinal": {
-                                                        "type": [
-                                                            "null",
-                                                            "integer"
-                                                        ]
-                                                    },
-                                                    "price_money": {
-                                                        "properties": {
-                                                            "amount": {
-                                                                "type": [
-                                                                    "null",
-                                                                    "integer"
-                                                                ]
-                                                            },
-                                                            "currency": {
-                                                                "type": [
-                                                                    "null",
-                                                                    "string"
-                                                                ]
-                                                            }
-                                                        },
-                                                        "type": [
-                                                            "null",
-                                                            "object"
-                                                        ]
-                                                    }
-                                                },
-                                                "type": [
-                                                    "null",
-                                                    "object"
-                                                ]
-                                            },
-                                            "present_at_all_locations": {
-                                                "type": [
-                                                    "null",
-                                                    "boolean"
-                                                ]
-                                            },
-                                            "type": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "updated_at": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "version": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "type": [
-                                        "null",
-                                        "array"
-                                    ]
-                                },
-                                "name": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "selection_type": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "present_at_all_locations": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        },
-                        "type": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "updated_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "version": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        }
-                    },
+    "properties": {
+        "address": {
+            "properties": {
+                "address_line_1": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "address_line_2": {
                     "type": [
                         "null",
-                        "object"
+                        "string"
                     ]
                 },
-                "name": "modifier_list",
-                "source_defined_cursor": true,
-                "supported_sync_modes": [
-                    "incremental",
-                    "full_refresh"
+                "administrative_district_level_1": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "locality": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "postal_code": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "birthday": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "cards": {
+            "items": {
+                "properties": {
+                    "billing_address": {
+                        "properties": {
+                            "postal_code": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "card_brand": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "cardholder_name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "exp_month": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "exp_year": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "last_4": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "company_name": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "created_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "creation_source": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "email_address": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "family_name": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "given_name": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "group_ids": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "phone_number": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "preferences": {
+            "properties": {
+                "email_unsubscribed": {
+                    "type": "boolean"
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "reference_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "segment_ids": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
                 ]
             },
-            "sync_mode": "incremental"
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "updated_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "version": {
+            "type": [
+                "null",
+                "integer"
+            ]
         }
+    },
+    "type": [
+        "null",
+        "object"
     ]
 }
```

### Comparing `airbyte-source-square-1.6.1/integration_tests/test_streams/orders.json` & `airbyte_source_square-1.6.2/source_square/schemas/orders.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('type', ['null', 'object']), ('properties', OrderedDict([('id', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('location_id', OrderedDict([('type', "*

 * *            "['null', 'string'])])), ('customer_id', OrderedDict([('type', ['null', 'string'])])), "*

 * *            "('line_items', OrderedDict([('type', ['null', 'array']), ('items', "*

 * *            "OrderedDict([('type', ['null', 'object']), ('properties', OrderedDict([('uid', "*

 * *            "OrderedDict([('type', ['null', […]*

```diff
@@ -1,667 +1,320 @@
 {
-    "streams": [
-        {
-            "cursor_field": [
-                "id"
-            ],
-            "destination_sync_mode": "overwrite",
-            "stream": {
-                "default_cursor_field": [
-                    "id"
-                ],
-                "json_schema": {
-                    "properties": {
-                        "closed_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "created_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "discounts": {
-                            "items": {
-                                "properties": {
-                                    "applied_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "currency": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "name": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "percentage": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "scope": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "type": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "uid": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    }
-                                },
+    "properties": {
+        "closed_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "created_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "customer_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "discounts": {
+            "items": {
+                "properties": {
+                    "applied_money": {
+                        "properties": {
+                            "amount": {
                                 "type": [
                                     "null",
-                                    "object"
+                                    "integer"
                                 ]
                             },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
                         },
-                        "fulfillments": {
-                            "items": {
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "percentage": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "scope": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "type": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "uid": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "fulfillments": {
+            "items": {
+                "properties": {
+                    "pickup_details": {
+                        "properties": {
+                            "accepted_at": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "auto_complete_duration": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "expires_at": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "note": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "picked_up_at": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "pickup_at": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "placed_at": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "ready_at": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "recipient": {
                                 "properties": {
-                                    "pickup_details": {
-                                        "properties": {
-                                            "accepted_at": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "auto_complete_duration": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "expires_at": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "note": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "picked_up_at": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "pickup_at": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "placed_at": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "ready_at": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "recipient": {
-                                                "properties": {
-                                                    "display_name": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    },
-                                                    "phone_number": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    }
-                                                },
-                                                "type": [
-                                                    "null",
-                                                    "object"
-                                                ]
-                                            },
-                                            "schedule_type": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "shipment_details": {
-                                        "properties": {
-                                            "carrier": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "expected_shipped_at": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "in_progress_at": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "packaged_at": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "placed_at": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "recipient": {
-                                                "properties": {
-                                                    "address": {
-                                                        "properties": {
-                                                            "address_line_1": {
-                                                                "type": [
-                                                                    "null",
-                                                                    "string"
-                                                                ]
-                                                            },
-                                                            "administrative_district_level_1": {
-                                                                "type": [
-                                                                    "null",
-                                                                    "string"
-                                                                ]
-                                                            },
-                                                            "locality": {
-                                                                "type": [
-                                                                    "null",
-                                                                    "string"
-                                                                ]
-                                                            },
-                                                            "postal_code": {
-                                                                "type": [
-                                                                    "null",
-                                                                    "string"
-                                                                ]
-                                                            }
-                                                        },
-                                                        "type": [
-                                                            "null",
-                                                            "object"
-                                                        ]
-                                                    },
-                                                    "display_name": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    },
-                                                    "phone_number": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    }
-                                                },
-                                                "type": [
-                                                    "null",
-                                                    "object"
-                                                ]
-                                            },
-                                            "shipped_at": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "tracking_number": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "state": {
+                                    "display_name": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
                                     },
-                                    "type": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "uid": {
+                                    "phone_number": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
                                     }
                                 },
                                 "type": [
                                     "null",
                                     "object"
                                 ]
                             },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
+                            "schedule_type": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
                         },
-                        "line_items": {
-                            "items": {
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "shipment_details": {
+                        "properties": {
+                            "carrier": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "expected_shipped_at": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "in_progress_at": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "packaged_at": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "placed_at": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "recipient": {
                                 "properties": {
-                                    "applied_discounts": {
-                                        "items": {
-                                            "properties": {
-                                                "applied_money": {
-                                                    "properties": {
-                                                        "amount": {
-                                                            "type": [
-                                                                "null",
-                                                                "integer"
-                                                            ]
-                                                        },
-                                                        "currency": {
-                                                            "type": [
-                                                                "null",
-                                                                "string"
-                                                            ]
-                                                        }
-                                                    },
-                                                    "type": [
-                                                        "null",
-                                                        "object"
-                                                    ]
-                                                },
-                                                "discount_uid": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "uid": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                }
-                                            },
-                                            "type": [
-                                                "null",
-                                                "object"
-                                            ]
-                                        },
-                                        "type": [
-                                            "null",
-                                            "array"
-                                        ]
-                                    },
-                                    "applied_taxes": {
-                                        "items": {
-                                            "properties": {
-                                                "applied_money": {
-                                                    "properties": {
-                                                        "amount": {
-                                                            "type": [
-                                                                "null",
-                                                                "integer"
-                                                            ]
-                                                        },
-                                                        "currency": {
-                                                            "type": [
-                                                                "null",
-                                                                "string"
-                                                            ]
-                                                        }
-                                                    },
-                                                    "type": [
-                                                        "null",
-                                                        "object"
-                                                    ]
-                                                },
-                                                "tax_uid": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "uid": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                }
-                                            },
-                                            "type": [
-                                                "null",
-                                                "object"
-                                            ]
-                                        },
-                                        "type": [
-                                            "null",
-                                            "array"
-                                        ]
-                                    },
-                                    "base_price_money": {
+                                    "address": {
                                         "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "currency": {
+                                            "address_line_1": {
                                                 "type": [
                                                     "null",
                                                     "string"
                                                 ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "catalog_object_id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "gross_sales_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "currency": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "item_type": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "modifiers": {
-                                        "items": {
-                                            "properties": {
-                                                "base_price_money": {
-                                                    "properties": {
-                                                        "amount": {
-                                                            "type": [
-                                                                "null",
-                                                                "integer"
-                                                            ]
-                                                        },
-                                                        "currency": {
-                                                            "type": [
-                                                                "null",
-                                                                "string"
-                                                            ]
-                                                        }
-                                                    },
-                                                    "type": [
-                                                        "null",
-                                                        "object"
-                                                    ]
-                                                },
-                                                "catalog_object_id": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "name": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "total_price_money": {
-                                                    "properties": {
-                                                        "amount": {
-                                                            "type": [
-                                                                "null",
-                                                                "integer"
-                                                            ]
-                                                        },
-                                                        "currency": {
-                                                            "type": [
-                                                                "null",
-                                                                "string"
-                                                            ]
-                                                        }
-                                                    },
-                                                    "type": [
-                                                        "null",
-                                                        "object"
-                                                    ]
-                                                },
-                                                "uid": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                }
-                                            },
-                                            "type": [
-                                                "null",
-                                                "object"
-                                            ]
-                                        },
-                                        "type": [
-                                            "null",
-                                            "array"
-                                        ]
-                                    },
-                                    "name": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "note": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "quantity": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "total_discount_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
                                             },
-                                            "currency": {
+                                            "administrative_district_level_1": {
                                                 "type": [
                                                     "null",
                                                     "string"
                                                 ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "total_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
                                             },
-                                            "currency": {
+                                            "locality": {
                                                 "type": [
                                                     "null",
                                                     "string"
                                                 ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "total_tax_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
                                             },
-                                            "currency": {
+                                            "postal_code": {
                                                 "type": [
                                                     "null",
                                                     "string"
                                                 ]
                                             }
                                         },
                                         "type": [
                                             "null",
                                             "object"
                                         ]
                                     },
-                                    "uid": {
+                                    "display_name": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
                                     },
-                                    "variation_name": {
+                                    "phone_number": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
-                                    },
-                                    "variation_total_price_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "currency": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
                                     }
                                 },
                                 "type": [
                                     "null",
                                     "object"
                                 ]
                             },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "location_id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
+                            "shipped_at": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "tracking_number": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
                         },
-                        "net_amounts": {
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "state": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "type": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "uid": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "line_items": {
+            "items": {
+                "properties": {
+                    "applied_discounts": {
+                        "items": {
                             "properties": {
-                                "discount_money": {
+                                "applied_money": {
                                     "properties": {
                                         "amount": {
                                             "type": [
                                                 "null",
                                                 "integer"
                                             ]
                                         },
@@ -673,35 +326,41 @@
                                         }
                                     },
                                     "type": [
                                         "null",
                                         "object"
                                     ]
                                 },
-                                "service_charge_money": {
-                                    "properties": {
-                                        "amount": {
-                                            "type": [
-                                                "null",
-                                                "integer"
-                                            ]
-                                        },
-                                        "currency": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
+                                "discount_uid": {
                                     "type": [
                                         "null",
-                                        "object"
+                                        "string"
                                     ]
                                 },
-                                "tax_money": {
+                                "uid": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                }
+                            },
+                            "type": [
+                                "null",
+                                "object"
+                            ]
+                        },
+                        "type": [
+                            "null",
+                            "array"
+                        ]
+                    },
+                    "applied_taxes": {
+                        "items": {
+                            "properties": {
+                                "applied_money": {
                                     "properties": {
                                         "amount": {
                                             "type": [
                                                 "null",
                                                 "integer"
                                             ]
                                         },
@@ -713,15 +372,93 @@
                                         }
                                     },
                                     "type": [
                                         "null",
                                         "object"
                                     ]
                                 },
-                                "tip_money": {
+                                "tax_uid": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "uid": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                }
+                            },
+                            "type": [
+                                "null",
+                                "object"
+                            ]
+                        },
+                        "type": [
+                            "null",
+                            "array"
+                        ]
+                    },
+                    "base_price_money": {
+                        "properties": {
+                            "amount": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "catalog_object_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "gross_sales_money": {
+                        "properties": {
+                            "amount": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "item_type": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "modifiers": {
+                        "items": {
+                            "properties": {
+                                "base_price_money": {
                                     "properties": {
                                         "amount": {
                                             "type": [
                                                 "null",
                                                 "integer"
                                             ]
                                         },
@@ -733,15 +470,27 @@
                                         }
                                     },
                                     "type": [
                                         "null",
                                         "object"
                                     ]
                                 },
-                                "total_money": {
+                                "catalog_object_id": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "name": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "total_price_money": {
                                     "properties": {
                                         "amount": {
                                             "type": [
                                                 "null",
                                                 "integer"
                                             ]
                                         },
@@ -752,100 +501,458 @@
                                             ]
                                         }
                                     },
                                     "type": [
                                         "null",
                                         "object"
                                     ]
+                                },
+                                "uid": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
                                 }
                             },
                             "type": [
                                 "null",
                                 "object"
                             ]
                         },
-                        "refunds": {
-                            "items": {
-                                "properties": {
-                                    "amount_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "currency": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "created_at": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "location_id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "reason": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "status": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "tender_id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "transaction_id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    }
-                                },
+                        "type": [
+                            "null",
+                            "array"
+                        ]
+                    },
+                    "name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "note": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "quantity": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "total_discount_money": {
+                        "properties": {
+                            "amount": {
                                 "type": [
                                     "null",
-                                    "object"
+                                    "integer"
+                                ]
+                            },
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "total_money": {
+                        "properties": {
+                            "amount": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "total_tax_money": {
+                        "properties": {
+                            "amount": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "uid": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "variation_name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "variation_total_price_money": {
+                        "properties": {
+                            "amount": {
+                                "type": [
+                                    "null",
+                                    "integer"
                                 ]
                             },
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "location_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "net_amounts": {
+            "properties": {
+                "discount_money": {
+                    "properties": {
+                        "amount": {
                             "type": [
                                 "null",
-                                "array"
+                                "integer"
                             ]
                         },
-                        "return_amounts": {
+                        "currency": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "service_charge_money": {
+                    "properties": {
+                        "amount": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "currency": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "tax_money": {
+                    "properties": {
+                        "amount": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "currency": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "tip_money": {
+                    "properties": {
+                        "amount": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "currency": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "total_money": {
+                    "properties": {
+                        "amount": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "currency": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "refunds": {
+            "items": {
+                "properties": {
+                    "amount_money": {
+                        "properties": {
+                            "amount": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "created_at": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "location_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "reason": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "status": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "tender_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "transaction_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "return_amounts": {
+            "properties": {
+                "discount_money": {
+                    "properties": {
+                        "amount": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "currency": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "service_charge_money": {
+                    "properties": {
+                        "amount": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "currency": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "tax_money": {
+                    "properties": {
+                        "amount": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "currency": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "tip_money": {
+                    "properties": {
+                        "amount": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "currency": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "total_money": {
+                    "properties": {
+                        "amount": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "currency": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "returns": {
+            "items": {
+                "properties": {
+                    "return_line_items": {
+                        "items": {
                             "properties": {
-                                "discount_money": {
+                                "base_price_money": {
                                     "properties": {
                                         "amount": {
                                             "type": [
                                                 "null",
                                                 "integer"
                                             ]
                                         },
@@ -857,15 +964,15 @@
                                         }
                                     },
                                     "type": [
                                         "null",
                                         "object"
                                     ]
                                 },
-                                "service_charge_money": {
+                                "gross_return_money": {
                                     "properties": {
                                         "amount": {
                                             "type": [
                                                 "null",
                                                 "integer"
                                             ]
                                         },
@@ -877,15 +984,27 @@
                                         }
                                     },
                                     "type": [
                                         "null",
                                         "object"
                                     ]
                                 },
-                                "tax_money": {
+                                "item_type": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "quantity": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "total_discount_money": {
                                     "properties": {
                                         "amount": {
                                             "type": [
                                                 "null",
                                                 "integer"
                                             ]
                                         },
@@ -897,15 +1016,15 @@
                                         }
                                     },
                                     "type": [
                                         "null",
                                         "object"
                                     ]
                                 },
-                                "tip_money": {
+                                "total_money": {
                                     "properties": {
                                         "amount": {
                                             "type": [
                                                 "null",
                                                 "integer"
                                             ]
                                         },
@@ -917,15 +1036,41 @@
                                         }
                                     },
                                     "type": [
                                         "null",
                                         "object"
                                     ]
                                 },
-                                "total_money": {
+                                "total_tax_money": {
+                                    "properties": {
+                                        "amount": {
+                                            "type": [
+                                                "null",
+                                                "integer"
+                                            ]
+                                        },
+                                        "currency": {
+                                            "type": [
+                                                "null",
+                                                "string"
+                                            ]
+                                        }
+                                    },
+                                    "type": [
+                                        "null",
+                                        "object"
+                                    ]
+                                },
+                                "uid": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "variation_total_price_money": {
                                     "properties": {
                                         "amount": {
                                             "type": [
                                                 "null",
                                                 "integer"
                                             ]
                                         },
@@ -943,691 +1088,531 @@
                                 }
                             },
                             "type": [
                                 "null",
                                 "object"
                             ]
                         },
-                        "returns": {
-                            "items": {
-                                "properties": {
-                                    "return_line_items": {
-                                        "items": {
-                                            "properties": {
-                                                "base_price_money": {
-                                                    "properties": {
-                                                        "amount": {
-                                                            "type": [
-                                                                "null",
-                                                                "integer"
-                                                            ]
-                                                        },
-                                                        "currency": {
-                                                            "type": [
-                                                                "null",
-                                                                "string"
-                                                            ]
-                                                        }
-                                                    },
-                                                    "type": [
-                                                        "null",
-                                                        "object"
-                                                    ]
-                                                },
-                                                "gross_return_money": {
-                                                    "properties": {
-                                                        "amount": {
-                                                            "type": [
-                                                                "null",
-                                                                "integer"
-                                                            ]
-                                                        },
-                                                        "currency": {
-                                                            "type": [
-                                                                "null",
-                                                                "string"
-                                                            ]
-                                                        }
-                                                    },
-                                                    "type": [
-                                                        "null",
-                                                        "object"
-                                                    ]
-                                                },
-                                                "item_type": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "quantity": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "total_discount_money": {
-                                                    "properties": {
-                                                        "amount": {
-                                                            "type": [
-                                                                "null",
-                                                                "integer"
-                                                            ]
-                                                        },
-                                                        "currency": {
-                                                            "type": [
-                                                                "null",
-                                                                "string"
-                                                            ]
-                                                        }
-                                                    },
-                                                    "type": [
-                                                        "null",
-                                                        "object"
-                                                    ]
-                                                },
-                                                "total_money": {
-                                                    "properties": {
-                                                        "amount": {
-                                                            "type": [
-                                                                "null",
-                                                                "integer"
-                                                            ]
-                                                        },
-                                                        "currency": {
-                                                            "type": [
-                                                                "null",
-                                                                "string"
-                                                            ]
-                                                        }
-                                                    },
-                                                    "type": [
-                                                        "null",
-                                                        "object"
-                                                    ]
-                                                },
-                                                "total_tax_money": {
-                                                    "properties": {
-                                                        "amount": {
-                                                            "type": [
-                                                                "null",
-                                                                "integer"
-                                                            ]
-                                                        },
-                                                        "currency": {
-                                                            "type": [
-                                                                "null",
-                                                                "string"
-                                                            ]
-                                                        }
-                                                    },
-                                                    "type": [
-                                                        "null",
-                                                        "object"
-                                                    ]
-                                                },
-                                                "uid": {
-                                                    "type": [
-                                                        "null",
-                                                        "string"
-                                                    ]
-                                                },
-                                                "variation_total_price_money": {
-                                                    "properties": {
-                                                        "amount": {
-                                                            "type": [
-                                                                "null",
-                                                                "integer"
-                                                            ]
-                                                        },
-                                                        "currency": {
-                                                            "type": [
-                                                                "null",
-                                                                "string"
-                                                            ]
-                                                        }
-                                                    },
-                                                    "type": [
-                                                        "null",
-                                                        "object"
-                                                    ]
-                                                }
-                                            },
-                                            "type": [
-                                                "null",
-                                                "object"
-                                            ]
-                                        },
-                                        "type": [
-                                            "null",
-                                            "array"
-                                        ]
-                                    },
-                                    "source_order_id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "uid": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    }
-                                },
+                        "type": [
+                            "null",
+                            "array"
+                        ]
+                    },
+                    "source_order_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "uid": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "service_charges": {
+            "items": {
+                "properties": {
+                    "amount_money": {
+                        "properties": {
+                            "amount": {
                                 "type": [
                                     "null",
-                                    "object"
+                                    "integer"
                                 ]
                             },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "applied_money": {
+                        "properties": {
+                            "amount": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "calculation_phase": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "taxable": {
+                        "type": [
+                            "null",
+                            "boolean"
+                        ]
+                    },
+                    "total_money": {
+                        "properties": {
+                            "amount": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "total_tax_money": {
+                        "properties": {
+                            "amount": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "uid": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "source": {
+            "properties": {
+                "name": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "state": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "taxes": {
+            "items": {
+                "properties": {
+                    "applied_money": {
+                        "properties": {
+                            "amount": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
                         },
-                        "service_charges": {
-                            "items": {
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "catalog_object_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "percentage": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "scope": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "type": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "uid": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "tenders": {
+            "items": {
+                "properties": {
+                    "amount_money": {
+                        "properties": {
+                            "amount": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "currency": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "card_details": {
+                        "properties": {
+                            "card": {
                                 "properties": {
-                                    "amount_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "currency": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "applied_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "currency": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "calculation_phase": {
+                                    "card_brand": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
                                     },
-                                    "name": {
+                                    "fingerprint": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
                                     },
-                                    "taxable": {
-                                        "type": [
-                                            "null",
-                                            "boolean"
-                                        ]
-                                    },
-                                    "total_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "currency": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "total_tax_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "currency": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "uid": {
+                                    "last_4": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
                                     }
                                 },
                                 "type": [
                                     "null",
                                     "object"
                                 ]
                             },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "source": {
-                            "properties": {
-                                "name": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
+                            "entry_method": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
                             },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "state": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
+                            "status": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
                         },
-                        "taxes": {
-                            "items": {
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "cash_details": {
+                        "properties": {
+                            "buyer_tendered_money": {
                                 "properties": {
-                                    "applied_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "currency": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "catalog_object_id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "name": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "percentage": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "scope": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "type": {
+                                    "amount": {
                                         "type": [
                                             "null",
-                                            "string"
+                                            "integer"
                                         ]
                                     },
-                                    "uid": {
+                                    "currency": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
                                     }
                                 },
                                 "type": [
                                     "null",
                                     "object"
                                 ]
                             },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "tenders": {
-                            "items": {
+                            "change_back_money": {
                                 "properties": {
-                                    "amount_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "currency": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
+                                    "amount": {
                                         "type": [
                                             "null",
-                                            "object"
+                                            "integer"
                                         ]
                                     },
-                                    "card_details": {
-                                        "properties": {
-                                            "card": {
-                                                "properties": {
-                                                    "card_brand": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    },
-                                                    "fingerprint": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    },
-                                                    "last_4": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    }
-                                                },
-                                                "type": [
-                                                    "null",
-                                                    "object"
-                                                ]
-                                            },
-                                            "entry_method": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            },
-                                            "status": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "cash_details": {
-                                        "properties": {
-                                            "buyer_tendered_money": {
-                                                "properties": {
-                                                    "amount": {
-                                                        "type": [
-                                                            "null",
-                                                            "integer"
-                                                        ]
-                                                    },
-                                                    "currency": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    }
-                                                },
-                                                "type": [
-                                                    "null",
-                                                    "object"
-                                                ]
-                                            },
-                                            "change_back_money": {
-                                                "properties": {
-                                                    "amount": {
-                                                        "type": [
-                                                            "null",
-                                                            "integer"
-                                                        ]
-                                                    },
-                                                    "currency": {
-                                                        "type": [
-                                                            "null",
-                                                            "string"
-                                                        ]
-                                                    }
-                                                },
-                                                "type": [
-                                                    "null",
-                                                    "object"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "created_at": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "location_id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "note": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "payment_id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "transaction_id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "type": {
+                                    "currency": {
                                         "type": [
                                             "null",
                                             "string"
                                         ]
                                     }
                                 },
                                 "type": [
                                     "null",
                                     "object"
                                 ]
-                            },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
+                            }
                         },
-                        "total_discount_money": {
-                            "properties": {
-                                "amount": {
-                                    "type": [
-                                        "null",
-                                        "integer"
-                                    ]
-                                },
-                                "currency": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "total_money": {
-                            "properties": {
-                                "amount": {
-                                    "type": [
-                                        "null",
-                                        "integer"
-                                    ]
-                                },
-                                "currency": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "total_service_charge_money": {
-                            "properties": {
-                                "amount": {
-                                    "type": [
-                                        "null",
-                                        "integer"
-                                    ]
-                                },
-                                "currency": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "total_tax_money": {
-                            "properties": {
-                                "amount": {
-                                    "type": [
-                                        "null",
-                                        "integer"
-                                    ]
-                                },
-                                "currency": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "total_tip_money": {
-                            "properties": {
-                                "amount": {
-                                    "type": [
-                                        "null",
-                                        "integer"
-                                    ]
-                                },
-                                "currency": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "updated_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "version": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        }
+                        "type": [
+                            "null",
+                            "object"
+                        ]
+                    },
+                    "created_at": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "location_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "note": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
                     },
+                    "payment_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "transaction_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "type": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "total_discount_money": {
+            "properties": {
+                "amount": {
                     "type": [
                         "null",
-                        "object"
+                        "integer"
                     ]
                 },
-                "name": "orders",
-                "source_defined_cursor": true,
-                "supported_sync_modes": [
-                    "full_refresh"
-                ]
+                "currency": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "total_money": {
+            "properties": {
+                "amount": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "currency": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "total_service_charge_money": {
+            "properties": {
+                "amount": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "currency": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "total_tax_money": {
+            "properties": {
+                "amount": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "currency": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "total_tip_money": {
+            "properties": {
+                "amount": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "currency": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
             },
-            "sync_mode": "full_refresh"
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "updated_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "version": {
+            "type": [
+                "null",
+                "integer"
+            ]
         }
+    },
+    "type": [
+        "null",
+        "object"
     ]
 }
```

### Comparing `airbyte-source-square-1.6.1/integration_tests/test_streams/payments.json` & `airbyte_source_square-1.6.2/source_square/schemas/payments.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('type', ['null', 'object']), ('properties', OrderedDict([('id', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('created_at', OrderedDict([('type', "*

 * *            "['null', 'string'])])), ('updated_at', OrderedDict([('type', ['null', 'string'])])), "*

 * *            "('amount_money', OrderedDict([('type', ['null', 'object']), ('properties', "*

 * *            "OrderedDict([('amount', OrderedDict([('type', ['null', 'integer'])])), ('currency', "*

 * *            "OrderedDict([('type […]*

```diff
@@ -1,398 +1,382 @@
 {
-    "streams": [
-        {
-            "cursor_field": [
-                "created_at"
-            ],
-            "destination_sync_mode": "append",
-            "stream": {
-                "default_cursor_field": [
-                    "created_at"
-                ],
-                "json_schema": {
+    "properties": {
+        "amount_money": {
+            "properties": {
+                "amount": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "currency": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "approved_money": {
+            "properties": {
+                "amount": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "currency": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "card_details": {
+            "properties": {
+                "avs_status": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "card": {
                     "properties": {
-                        "amount_money": {
-                            "properties": {
-                                "amount": {
-                                    "type": [
-                                        "null",
-                                        "integer"
-                                    ]
-                                },
-                                "currency": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
+                        "bin": {
                             "type": [
                                 "null",
-                                "object"
-                            ]
-                        },
-                        "approved_money": {
-                            "properties": {
-                                "amount": {
-                                    "type": [
-                                        "null",
-                                        "integer"
-                                    ]
-                                },
-                                "currency": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
+                                "string"
                             ]
                         },
-                        "card_details": {
-                            "properties": {
-                                "avs_status": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "card": {
-                                    "properties": {
-                                        "bin": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        },
-                                        "card_brand": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        },
-                                        "card_type": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        },
-                                        "exp_month": {
-                                            "type": [
-                                                "null",
-                                                "integer"
-                                            ]
-                                        },
-                                        "exp_year": {
-                                            "type": [
-                                                "null",
-                                                "integer"
-                                            ]
-                                        },
-                                        "fingerprint": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        },
-                                        "last_4": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        },
-                                        "prepaid_type": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                },
-                                "card_payment_timeline": {
-                                    "properties": {
-                                        "authorized_at": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        },
-                                        "captured_at": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        },
-                                        "voided_at": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                },
-                                "cvv_status": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "entry_method": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "statement_description": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "status": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
+                        "card_brand": {
                             "type": [
                                 "null",
-                                "object"
+                                "string"
                             ]
                         },
-                        "created_at": {
+                        "card_type": {
                             "type": [
                                 "null",
                                 "string"
                             ]
                         },
-                        "delay_action": {
+                        "exp_month": {
                             "type": [
                                 "null",
-                                "string"
+                                "integer"
                             ]
                         },
-                        "delay_duration": {
+                        "exp_year": {
                             "type": [
                                 "null",
-                                "string"
+                                "integer"
                             ]
                         },
-                        "delayed_until": {
+                        "fingerprint": {
                             "type": [
                                 "null",
                                 "string"
                             ]
                         },
-                        "employee_id": {
+                        "last_4": {
                             "type": [
                                 "null",
                                 "string"
                             ]
                         },
-                        "id": {
+                        "prepaid_type": {
                             "type": [
                                 "null",
                                 "string"
                             ]
-                        },
-                        "location_id": {
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "card_payment_timeline": {
+                    "properties": {
+                        "authorized_at": {
                             "type": [
                                 "null",
                                 "string"
                             ]
                         },
-                        "note": {
+                        "captured_at": {
                             "type": [
                                 "null",
                                 "string"
                             ]
                         },
-                        "order_id": {
+                        "voided_at": {
                             "type": [
                                 "null",
                                 "string"
                             ]
-                        },
-                        "processing_fee": {
-                            "items": {
-                                "properties": {
-                                    "amount_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "currency": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "effective_at": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "type": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    }
-                                },
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "cvv_status": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "entry_method": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "statement_description": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "status": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "created_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "customer_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "delay_action": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "delay_duration": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "delayed_until": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "employee_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "location_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "note": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "order_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "processing_fee": {
+            "items": {
+                "properties": {
+                    "amount_money": {
+                        "properties": {
+                            "amount": {
                                 "type": [
                                     "null",
-                                    "object"
+                                    "integer"
                                 ]
                             },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "receipt_number": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "receipt_url": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "refund_ids": {
-                            "items": {
+                            "currency": {
                                 "type": [
                                     "null",
                                     "string"
                                 ]
-                            },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "refunded_money": {
-                            "properties": {
-                                "amount": {
-                                    "type": [
-                                        "null",
-                                        "integer"
-                                    ]
-                                },
-                                "currency": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "risk_evaluation": {
-                            "properties": {
-                                "created_at": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "risk_level": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "source_type": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "status": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "total_money": {
-                            "properties": {
-                                "amount": {
-                                    "type": [
-                                        "null",
-                                        "integer"
-                                    ]
-                                },
-                                "currency": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "updated_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
+                            }
                         },
-                        "version_token": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
+                        "type": [
+                            "null",
+                            "object"
+                        ]
                     },
+                    "effective_at": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "type": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "receipt_number": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "receipt_url": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "refund_ids": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "refunded_money": {
+            "properties": {
+                "amount": {
                     "type": [
                         "null",
-                        "object"
+                        "integer"
                     ]
                 },
-                "name": "payments",
-                "source_defined_cursor": true,
-                "supported_sync_modes": [
-                    "incremental",
-                    "full_refresh"
-                ]
+                "currency": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "risk_evaluation": {
+            "properties": {
+                "created_at": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "risk_level": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "source_type": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "status": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "total_money": {
+            "properties": {
+                "amount": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "currency": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
             },
-            "sync_mode": "incremental"
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "updated_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "version_token": {
+            "type": [
+                "null",
+                "string"
+            ]
         }
+    },
+    "type": [
+        "null",
+        "object"
     ]
 }
```

### Comparing `airbyte-source-square-1.6.1/integration_tests/test_streams/refunds.json` & `airbyte_source_square-1.6.2/source_square/schemas/cash_drawers.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('$schema', 'http://json-schema.org/draft-07/schema#'), ('title', 'Cash "*

 * *            "Drawer Shifts Schema'), ('additionalProperties', True), ('type', ['object', 'null']), "*

 * *            "('properties', OrderedDict([('id', OrderedDict([('type', ['string', 'null'])])), "*

 * *            "('state', OrderedDict([('type', ['string', 'null'])])), ('opened_at', "*

 * *            "OrderedDict([('type', ['string', 'null'])])), ('ended_at', OrderedDict([('type', "*

 * *            "['string', 'null'])]) […]*

```diff
@@ -1,144 +1,107 @@
 {
-    "streams": [
-        {
-            "cursor_field": [
-                "created_at"
-            ],
-            "destination_sync_mode": "append",
-            "stream": {
-                "default_cursor_field": [
-                    "created_at"
-                ],
-                "json_schema": {
-                    "properties": {
-                        "amount_money": {
-                            "properties": {
-                                "amount": {
-                                    "type": [
-                                        "null",
-                                        "integer"
-                                    ]
-                                },
-                                "currency": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "created_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "location_id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "order_id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "payment_id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "processing_fee": {
-                            "items": {
-                                "properties": {
-                                    "amount_money": {
-                                        "properties": {
-                                            "amount": {
-                                                "type": [
-                                                    "null",
-                                                    "integer"
-                                                ]
-                                            },
-                                            "currency": {
-                                                "type": [
-                                                    "null",
-                                                    "string"
-                                                ]
-                                            }
-                                        },
-                                        "type": [
-                                            "null",
-                                            "object"
-                                        ]
-                                    },
-                                    "effective_at": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "type": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    }
-                                },
-                                "type": [
-                                    "null",
-                                    "object"
-                                ]
-                            },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "reason": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "status": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "updated_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "additionalProperties": true,
+    "properties": {
+        "closed_at": {
+            "type": [
+                "string",
+                "null"
+            ]
+        },
+        "closed_cash_money": {
+            "properties": {
+                "amount": {
                     "type": [
-                        "null",
-                        "object"
+                        "number",
+                        "null"
                     ]
                 },
-                "name": "refunds",
-                "source_defined_cursor": true,
-                "supported_sync_modes": [
-                    "incremental",
-                    "full_refresh"
-                ]
+                "currency": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                }
+            },
+            "type": [
+                "object",
+                "null"
+            ]
+        },
+        "description": {
+            "type": [
+                "string",
+                "null"
+            ]
+        },
+        "ended_at": {
+            "type": [
+                "string",
+                "null"
+            ]
+        },
+        "expected_cash_money": {
+            "properties": {
+                "amount": {
+                    "type": [
+                        "number",
+                        "null"
+                    ]
+                },
+                "currency": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                }
+            },
+            "type": [
+                "object",
+                "null"
+            ]
+        },
+        "id": {
+            "type": [
+                "string",
+                "null"
+            ]
+        },
+        "opened_at": {
+            "type": [
+                "string",
+                "null"
+            ]
+        },
+        "opened_cash_money": {
+            "properties": {
+                "amount": {
+                    "type": [
+                        "number",
+                        "null"
+                    ]
+                },
+                "currency": {
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                }
             },
-            "sync_mode": "incremental"
+            "type": [
+                "object",
+                "null"
+            ]
+        },
+        "state": {
+            "type": [
+                "string",
+                "null"
+            ]
         }
+    },
+    "title": "Cash Drawer Shifts Schema",
+    "type": [
+        "object",
+        "null"
     ]
 }
```

### Comparing `airbyte-source-square-1.6.1/integration_tests/test_streams/shifts.json` & `airbyte_source_square-1.6.2/source_square/schemas/taxes.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('type', ['null', 'object']), ('properties', OrderedDict([('type', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('id', OrderedDict([('type', ['null', "*

 * *            "'string'])])), ('updated_at', OrderedDict([('type', ['null', 'string'])])), "*

 * *            "('version', OrderedDict([('type', ['null', 'integer'])])), ('is_deleted', "*

 * *            "OrderedDict([('type', ['null', 'boolean'])])), ('present_at_all_locations', "*

 * *            "OrderedDict([('type', ['null', 'bo […]*

```diff
@@ -1,185 +1,112 @@
 {
-    "streams": [
-        {
-            "cursor_field": [
-                "id"
-            ],
-            "destination_sync_mode": "overwrite",
-            "stream": {
-                "default_cursor_field": [
-                    "id"
-                ],
-                "json_schema": {
-                    "properties": {
-                        "breaks": {
-                            "items": {
-                                "properties": {
-                                    "break_type_id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "end_at": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "expected_duration": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "id": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "is_paid": {
-                                        "type": [
-                                            "null",
-                                            "boolean"
-                                        ]
-                                    },
-                                    "name": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    },
-                                    "start_at": {
-                                        "type": [
-                                            "null",
-                                            "string"
-                                        ]
-                                    }
-                                },
-                                "type": [
-                                    "null",
-                                    "object"
-                                ]
-                            },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "created_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "employee_id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "end_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "location_id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "start_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "status": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "team_member_id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "timezone": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "updated_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "version": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "wage": {
-                            "properties": {
-                                "hourly_rate": {
-                                    "properties": {
-                                        "amount": {
-                                            "type": [
-                                                "null",
-                                                "integer"
-                                            ]
-                                        },
-                                        "currency": {
-                                            "type": [
-                                                "null",
-                                                "string"
-                                            ]
-                                        }
-                                    },
-                                    "type": [
-                                        "null",
-                                        "object"
-                                    ]
-                                },
-                                "title": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "name": "shifts",
-                "source_defined_cursor": true,
-                "supported_sync_modes": [
-                    "full_refresh"
+    "properties": {
+        "absent_at_location_ids": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
                 ]
             },
-            "sync_mode": "full_refresh"
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "is_deleted": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "present_at_all_locations": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "tax_data": {
+            "properties": {
+                "applies_to_custom_amounts": {
+                    "type": [
+                        "null",
+                        "boolean"
+                    ]
+                },
+                "calculation_phase": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "enabled": {
+                    "type": [
+                        "null",
+                        "boolean"
+                    ]
+                },
+                "inclusion_type": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "name": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "percentage": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "tax_type_id": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "tax_type_name": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "type": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "updated_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "version": {
+            "type": [
+                "null",
+                "integer"
+            ]
         }
+    },
+    "type": [
+        "null",
+        "object"
     ]
 }
```

### Comparing `airbyte-source-square-1.6.1/integration_tests/test_streams/taxes.json` & `airbyte_source_square-1.6.2/source_square/schemas/locations.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('type', ['null', 'object']), ('properties', OrderedDict([('id', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('name', OrderedDict([('type', ['null', "*

 * *            "'string'])])), ('address', OrderedDict([('type', ['null', 'object']), ('properties', "*

 * *            "OrderedDict([('address_line_1', OrderedDict([('type', ['null', 'string'])])), "*

 * *            "('locality', OrderedDict([('type', ['null', 'string'])])), "*

 * *            "('administrative_district_level_1', Or […]*

```diff
@@ -1,134 +1,178 @@
 {
-    "streams": [
-        {
-            "cursor_field": [
-                "updated_at"
-            ],
-            "destination_sync_mode": "append",
-            "stream": {
-                "default_cursor_field": [
-                    "updated_at"
-                ],
-                "json_schema": {
-                    "properties": {
-                        "absent_at_location_ids": {
-                            "items": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "is_deleted": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        },
-                        "present_at_all_locations": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        },
-                        "tax_data": {
-                            "properties": {
-                                "applies_to_custom_amounts": {
-                                    "type": [
-                                        "null",
-                                        "boolean"
-                                    ]
-                                },
-                                "calculation_phase": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "enabled": {
-                                    "type": [
-                                        "null",
-                                        "boolean"
-                                    ]
-                                },
-                                "inclusion_type": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "name": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "percentage": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "tax_type_id": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                },
-                                "tax_type_name": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "type": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "updated_at": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "version": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        }
-                    },
+    "properties": {
+        "address": {
+            "properties": {
+                "address_line_1": {
                     "type": [
                         "null",
-                        "object"
+                        "string"
                     ]
                 },
-                "name": "taxes",
-                "source_defined_cursor": true,
-                "supported_sync_modes": [
-                    "incremental",
-                    "full_refresh"
+                "administrative_district_level_1": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "country": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "locality": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "postal_code": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "business_email": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "business_hours": {
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "business_name": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "capabilities": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
                 ]
             },
-            "sync_mode": "incremental"
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "country": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "created_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "currency": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "description": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "facebook_url": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "instagram_username": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "language_code": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "mcc": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "merchant_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "name": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "phone_number": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "status": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "timezone": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "twitter_username": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "type": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "website_url": {
+            "type": [
+                "null",
+                "string"
+            ]
         }
+    },
+    "type": [
+        "null",
+        "object"
     ]
 }
```

### Comparing `airbyte-source-square-1.6.1/integration_tests/test_streams/team_member_wages.json` & `airbyte_source_square-1.6.2/source_square/schemas/team_members.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('type', ['null', 'object']), ('properties', OrderedDict([('id', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('is_owner', OrderedDict([('type', "*

 * *            "['null', 'boolean'])])), ('status', OrderedDict([('type', ['null', 'string'])])), "*

 * *            "('given_name', OrderedDict([('type', ['null', 'string'])])), ('family_name', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('email_address', OrderedDict([('type', "*

 * *            "['null', 'string'])] […]*

```diff
@@ -1,67 +1,82 @@
 {
-    "streams": [
-        {
-            "cursor_field": [
-                "id"
-            ],
-            "destination_sync_mode": "overwrite",
-            "stream": {
-                "default_cursor_field": [
-                    "id"
-                ],
-                "json_schema": {
-                    "properties": {
-                        "hourly_rate": {
-                            "properties": {
-                                "amount": {
-                                    "type": [
-                                        "null",
-                                        "integer"
-                                    ]
-                                },
-                                "currency": {
-                                    "type": [
-                                        "null",
-                                        "string"
-                                    ]
-                                }
-                            },
-                            "type": [
-                                "null",
-                                "object"
-                            ]
-                        },
-                        "id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "team_member_id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "title": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
+    "properties": {
+        "assigned_locations": {
+            "properties": {
+                "assignment_type": {
                     "type": [
                         "null",
-                        "object"
+                        "string"
                     ]
-                },
-                "name": "team_member_wages",
-                "source_defined_cursor": true,
-                "supported_sync_modes": [
-                    "full_refresh"
-                ]
+                }
             },
-            "sync_mode": "full_refresh"
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "created_at": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "email_address": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "family_name": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "given_name": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "is_owner": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "phone_number": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "reference_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "status": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "updated_at": {
+            "type": [
+                "null",
+                "string"
+            ]
         }
+    },
+    "type": [
+        "null",
+        "object"
     ]
 }
```

### Comparing `airbyte-source-square-1.6.1/source_square/manifest.yaml` & `airbyte_source_square-1.6.2/source_square/manifest.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version: "0.29.0"
+version: "0.81.4"
 
 definitions:
   schema_loader:
     type: JsonFileSchemaLoader
     file_path: "./source_square/schemas/{{ parameters['name'] }}.json"
   oauth_authenticator:
     type: OAuthAuthenticator
@@ -19,24 +19,22 @@
     extractor:
       field_path: ["{{ parameters['name'] }}"]
 
   requester:
     url_base: "{{ 'https://connect.squareupsandbox.com/v2' if config['is_sandbox'] else 'https://connect.squareup.com/v2' }}"
     http_method: "GET"
     authenticator:
-      class_name: source_square.components.AuthenticatorSquare
-      bearer: "#/definitions/bearer_authenticator"
-      oauth: "#/definitions/oauth_authenticator"
-
-  #    Uncomment this block later. request_headers used to accidentally get overridden but this was fixed in beta release
-  #    However, because expected_records were originally generated with the buggy flow missing these, we need to
-  #    regenerate the expected records. Temporarily commenting it out to retain the old behavior until we do it.
-  #    request_headers:
-  #      Square-Version: "2022-10-19"
-  #      Content-Type: "application/json"
+      type: SelectiveAuthenticator
+      authenticator_selection_path: ["credentials", "auth_type"]
+      authenticators:
+        API Key: "#/definitions/bearer_authenticator"
+        OAuth: "#/definitions/oauth_authenticator"
+    request_headers:
+      Square-Version: "2022-10-19"
+      Content-Type: "application/json"
   retriever:
     record_selector:
       $ref: "#/definitions/selector"
     requester:
       $ref: "#/definitions/requester"
 
   base_stream:
@@ -325,41 +323,50 @@
           limit: "{{ 200 }}"
       record_selector:
         $ref: "#/definitions/selector"
         extractor:
           field_path: ["loyalty_accounts"]
 
   orders_stream:
+    # ToDo: Improve the efficiency of this stream by grouping location IDs into batches of 10.
     $ref: "#/definitions/base_stream_page_json_limit"
     $parameters:
       name: "orders"
       primary_key: "id"
       path: "/orders/search"
     incremental_sync:
-      type: CustomIncrementalSync
-      class_name: source_square.components.SquareSubstreamIncrementalSync
+      type: DatetimeBasedCursor
       start_datetime:
         datetime: "{{ format_datetime(config['start_date'], '%Y-%m-%dT%H:%M:%S.%fZ') }}"
         datetime_format: "%Y-%m-%dT%H:%M:%S.%fZ"
-      end_datetime:
-        datetime: "{{ now_utc().strftime('%Y-%m-%dT%H:%M:%S.%fZ') }}"
-        datetime_format: "%Y-%m-%dT%H:%M:%S.%fZ"
       step: P30D
       datetime_format: "%Y-%m-%dT%H:%M:%S.%fZ"
       cursor_granularity: "PT0.000001S"
-      parent_stream: "#/definitions/locations_stream"
       cursor_field: "updated_at"
-      parent_key: "id"
     retriever:
       $ref: "#/definitions/base_stream_page_json_limit/retriever"
       requester:
         $ref: "#/definitions/base_stream_page_json_limit/retriever/requester"
         http_method: "POST"
         request_body_json:
           limit: "{{ 500 }}"
+          filter:
+            date_time_filter:
+              updated_at:
+                start_at: "{{ stream_slice.start_time }}"
+          sort:
+            sort_field: "UPDATED_AT"
+            sort_order: "ASC"
+          location_ids: "{{ [ stream_slice.location_ids ] }}"
+      partition_router:
+        type: "SubstreamPartitionRouter"
+        parent_stream_configs:
+          - stream: "#/definitions/locations_stream"
+            parent_key: "id"
+            partition_field: "location_ids"
 
   bank_accounts_stream:
     $ref: "#/definitions/base_stream"
     $parameters:
       name: "bank_accounts"
       primary_key: "id"
       path: "/bank-accounts"
```

### Comparing `airbyte-source-square-1.6.1/source_square/schemas/bank_accounts.json` & `airbyte_source_square-1.6.2/source_square/schemas/bank_accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-square-1.6.1/source_square/schemas/cash_drawers.json` & `airbyte_source_square-1.6.2/source_square/schemas/loyalty.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.80625%*

 * *Differences: {"'properties'": "{'mapping': OrderedDict([('type', ['object', 'null']), ('properties', "*

 * *                 "OrderedDict([('id', OrderedDict([('type', ['string', 'null'])])), "*

 * *                 "('phone_number', OrderedDict([('type', ['string', 'null'])])), ('created_at', "*

 * *                 "OrderedDict([('type', ['string', 'null'])]))]))]), 'program_id': "*

 * *                 "OrderedDict([('type', ['string', 'null'])]), 'balance': OrderedDict([('type', "*

 * *                 "['number', 'null'])]), 'lifetime_poin […]*

```diff
@@ -1,107 +1,79 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": true,
     "properties": {
-        "closed_at": {
+        "balance": {
             "type": [
-                "string",
+                "number",
                 "null"
             ]
         },
-        "closed_cash_money": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "number",
-                        "null"
-                    ]
-                },
-                "currency": {
-                    "type": [
-                        "string",
-                        "null"
-                    ]
-                }
-            },
-            "type": [
-                "object",
-                "null"
-            ]
-        },
-        "description": {
+        "created_at": {
             "type": [
                 "string",
                 "null"
             ]
         },
-        "ended_at": {
+        "customer_id": {
             "type": [
                 "string",
                 "null"
             ]
         },
-        "expected_cash_money": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "number",
-                        "null"
-                    ]
-                },
-                "currency": {
-                    "type": [
-                        "string",
-                        "null"
-                    ]
-                }
-            },
-            "type": [
-                "object",
-                "null"
-            ]
-        },
         "id": {
             "type": [
                 "string",
                 "null"
             ]
         },
-        "opened_at": {
+        "lifetime_points": {
             "type": [
-                "string",
+                "number",
                 "null"
             ]
         },
-        "opened_cash_money": {
+        "mapping": {
             "properties": {
-                "amount": {
+                "created_at": {
                     "type": [
-                        "number",
+                        "string",
+                        "null"
+                    ]
+                },
+                "id": {
+                    "type": [
+                        "string",
                         "null"
                     ]
                 },
-                "currency": {
+                "phone_number": {
                     "type": [
                         "string",
                         "null"
                     ]
                 }
             },
             "type": [
                 "object",
                 "null"
             ]
         },
-        "state": {
+        "program_id": {
+            "type": [
+                "string",
+                "null"
+            ]
+        },
+        "updated_at": {
             "type": [
                 "string",
                 "null"
             ]
         }
     },
-    "title": "Cash Drawer Shifts Schema",
+    "title": "Loyalty schema",
     "type": [
         "object",
         "null"
     ]
 }
```

### Comparing `airbyte-source-square-1.6.1/source_square/schemas/categories.json` & `airbyte_source_square-1.6.2/source_square/schemas/categories.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-square-1.6.1/source_square/schemas/inventory.json` & `airbyte_source_square-1.6.2/source_square/schemas/inventory.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-square-1.6.1/source_square/spec.yaml` & `airbyte_source_square-1.6.2/source_square/spec.yaml`

 * *Files identical despite different names*

