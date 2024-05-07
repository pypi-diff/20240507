# Comparing `tmp/pysparkplug-0.3.1.tar.gz` & `tmp/pysparkplug-0.3.2.tar.gz`

## Comparing `pysparkplug-0.3.1.tar` & `pysparkplug-0.3.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/.dockerignore
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/.readthedocs.yaml
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/Dockerfile
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/compose.yaml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/notebook.Dockerfile
--rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/nox.sh
--rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/noxfile.py
--rw-r--r--   0        0        0    20970 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/pylintrc
--rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/sparkplug_b.proto
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/.github/CODEOWNERS
--rw-r--r--   0        0        0    13358 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/.github/workflows/cicd.yaml
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/docs/api.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/docs/changelog.md
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/docs/conf.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/docs/contributor_guide.md
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/docs/index.md
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/docs/linkcode.py
--rw-r--r--   0        0        0   136631 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/docs/static/logo.png
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/docs/templates/sidebar/brand.html
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/notebooks/dcmd_demo.ipynb
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/notebooks/device_demo.ipynb
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/notebooks/edge_node_demo.ipynb
--rw-r--r--   0        0        0    16717 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/notebooks/inspect_mqtt.ipynb
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/notebooks/run.sh
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/black.in
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/black.txt
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/coverage.in
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/coverage.txt
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/docs.in
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/docs.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/draft_release.in
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/draft_release.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/isort.in
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/isort.txt
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/mypy.in
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/mypy.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/packaging.in
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/packaging.txt
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/publish.in
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/publish.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/pylint.in
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/pylint.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/requirements.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/unit_tests.in
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/requirements/unit_tests.txt
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/__init__.py
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_client.py
--rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_config.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_constants.py
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_datatype.py
--rw-r--r--   0        0        0    16816 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_edge_node.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_enums.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_error.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_message.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_metric.py
--rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_payload.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_strenum.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_time.py
--rw-r--r--   0        0        0     5593 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_topic.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_types.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/py.typed
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_protobuf/__init__.py
--rw-r--r--   0        0        0     8621 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/src/pysparkplug/_protobuf/sparkplug_b_pb2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/test/unit_tests/__init__.py
--rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/test/unit_tests/test_topic.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/test/unit_tests/test_version.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/.gitignore
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/LICENSE
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/README.md
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 pysparkplug-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/.dockerignore
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/Dockerfile
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/compose.yaml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/notebook.Dockerfile
+-rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/nox.sh
+-rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/noxfile.py
+-rw-r--r--   0        0        0    20970 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/pylintrc
+-rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/sparkplug_b.proto
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0    13358 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/.github/workflows/cicd.yaml
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/docs/api.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/docs/changelog.md
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/docs/conf.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/docs/contributor_guide.md
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/docs/index.md
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/docs/linkcode.py
+-rw-r--r--   0        0        0   136631 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/docs/static/logo.png
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/docs/templates/sidebar/brand.html
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/notebooks/dcmd_demo.ipynb
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/notebooks/device_demo.ipynb
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/notebooks/edge_node_demo.ipynb
+-rw-r--r--   0        0        0    16717 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/notebooks/inspect_mqtt.ipynb
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/notebooks/run.sh
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/black.in
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/black.txt
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/coverage.in
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/coverage.txt
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/docs.in
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/docs.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/draft_release.in
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/draft_release.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/isort.in
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/isort.txt
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/mypy.in
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/mypy.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/packaging.in
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/packaging.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/publish.in
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/publish.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/pylint.in
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/pylint.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/requirements.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/unit_tests.in
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/requirements/unit_tests.txt
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/__init__.py
+-rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_client.py
+-rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_config.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_constants.py
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_datatype.py
+-rw-r--r--   0        0        0    16849 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_edge_node.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_enums.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_error.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_message.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_metric.py
+-rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_payload.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_strenum.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_time.py
+-rw-r--r--   0        0        0     5593 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_topic.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_types.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/py.typed
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_protobuf/__init__.py
+-rw-r--r--   0        0        0     8621 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/src/pysparkplug/_protobuf/sparkplug_b_pb2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/test/unit_tests/test_topic.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/test/unit_tests/test_version.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/.gitignore
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/README.md
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 pysparkplug-0.3.2/PKG-INFO
```

### Comparing `pysparkplug-0.3.1/.readthedocs.yaml` & `pysparkplug-0.3.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/CHANGELOG.md` & `pysparkplug-0.3.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Changelog
 
 All notable changes for `pysparkplug` will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/) and [Keep a Changelog](http://keepachangelog.com/).
 
-## 0.3.1. (2024-02-13)
+## 0.3.2 (2024-05-06)
+
+### Fixed
+- Fixed topic for DDATA payloads resulting from the `EdgeNode.update_device` method.
+
+## 0.3.1 (2024-02-13)
 
 ### Changed
 - Pysparkplug is not compatible with the new 2.0 releasee of Paho, the underlying Python MQTT client.
 
 ## 0.3.0 (2024-01-13)
 
 ### Added
```

### Comparing `pysparkplug-0.3.1/Dockerfile` & `pysparkplug-0.3.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/compose.yaml` & `pysparkplug-0.3.2/compose.yaml`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/noxfile.py` & `pysparkplug-0.3.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/pylintrc` & `pysparkplug-0.3.2/pylintrc`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/sparkplug_b.proto` & `pysparkplug-0.3.2/sparkplug_b.proto`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/.github/CONTRIBUTING.md` & `pysparkplug-0.3.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/.github/PULL_REQUEST_TEMPLATE.md` & `pysparkplug-0.3.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `pysparkplug-0.3.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md` & `pysparkplug-0.3.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/.github/workflows/cicd.yaml` & `pysparkplug-0.3.2/.github/workflows/cicd.yaml`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/docs/api.rst` & `pysparkplug-0.3.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/docs/conf.py` & `pysparkplug-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/docs/linkcode.py` & `pysparkplug-0.3.2/docs/linkcode.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/docs/static/logo.png` & `pysparkplug-0.3.2/docs/static/logo.png`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/notebooks/dcmd_demo.ipynb` & `pysparkplug-0.3.2/notebooks/dcmd_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/notebooks/device_demo.ipynb` & `pysparkplug-0.3.2/notebooks/device_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/notebooks/edge_node_demo.ipynb` & `pysparkplug-0.3.2/notebooks/edge_node_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/notebooks/inspect_mqtt.ipynb` & `pysparkplug-0.3.2/notebooks/inspect_mqtt.ipynb`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/requirements/docs.txt` & `pysparkplug-0.3.2/requirements/docs.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,69 +2,69 @@
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    ./nox.sh -s update_requirements
 #
 alabaster==0.7.16
     # via sphinx
-babel==2.14.0
+babel==2.15.0
     # via sphinx
 beautifulsoup4==4.12.3
     # via furo
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   sphinx
-furo==2024.1.29
+furo==2024.5.6
     # via -r /root/pysparkplug/requirements/docs.in
-idna==3.6
+idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   myst-parser
     #   sphinx
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via jinja2
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-myst-parser==2.0.0
+myst-parser==3.0.1
     # via -r /root/pysparkplug/requirements/docs.in
-packaging==23.2
+packaging==24.0
     # via
     #   -r /root/pysparkplug/requirements/docs.in
     #   sphinx
 paho-mqtt==1.6.1
     # via -r /root/pysparkplug/requirements/requirements.txt
-protobuf==4.25.2
+protobuf==5.26.1
     # via -r /root/pysparkplug/requirements/requirements.txt
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   furo
     #   sphinx
 pyyaml==6.0.1
     # via myst-parser
 requests==2.31.0
     # via sphinx
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   -r /root/pysparkplug/requirements/docs.in
     #   furo
     #   myst-parser
     #   sphinx-basic-ng
     #   sphinx-copybutton
     #   sphinx-notfound-page
@@ -85,9 +85,9 @@
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 sphinxext-opengraph==0.9.1
     # via -r /root/pysparkplug/requirements/docs.in
-urllib3==2.2.0
+urllib3==2.2.1
     # via requests
```

### Comparing `pysparkplug-0.3.1/requirements/mypy.txt` & `pysparkplug-0.3.2/requirements/mypy.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    ./nox.sh -s update_requirements
 #
-argcomplete==3.2.2
+argcomplete==3.3.0
     # via nox
 colorlog==6.8.2
     # via nox
 distlib==0.3.8
     # via virtualenv
-filelock==3.13.1
+filelock==3.14.0
     # via virtualenv
-mypy==1.8.0
+mypy==1.10.0
     # via -r /root/pysparkplug/requirements/mypy.in
 mypy-extensions==1.0.0
     # via mypy
-nox==2023.4.22
+nox==2024.4.15
     # via -r /root/pysparkplug/requirements/mypy.in
-packaging==23.2
+packaging==24.0
     # via
     #   -r /root/pysparkplug/requirements/mypy.in
     #   nox
 paho-mqtt==1.6.1
     # via -r /root/pysparkplug/requirements/requirements.txt
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via virtualenv
-protobuf==4.25.2
+protobuf==5.26.1
     # via -r /root/pysparkplug/requirements/requirements.txt
-types-colorama==0.4.15.20240205
+types-colorama==0.4.15.20240311
     # via -r /root/pysparkplug/requirements/mypy.in
-types-paho-mqtt==1.6.0.20240106
+types-paho-mqtt==1.6.0.20240321
     # via -r /root/pysparkplug/requirements/mypy.in
-types-protobuf==4.24.0.20240129
+types-protobuf==5.26.0.20240422
     # via -r /root/pysparkplug/requirements/mypy.in
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via mypy
-virtualenv==20.25.0
+virtualenv==20.26.1
     # via nox
```

### Comparing `pysparkplug-0.3.1/requirements/packaging.txt` & `pysparkplug-0.3.2/requirements/packaging.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,91 +4,99 @@
 #
 #    ./nox.sh -s update_requirements
 #
 annotated-types==0.6.0
     # via pydantic
 attrs==23.2.0
     # via check-wheel-contents
-build==1.0.3
+backports-tarfile==1.1.1
+    # via jaraco-context
+build==1.2.1
     # via -r /root/pysparkplug/requirements/packaging.in
 certifi==2024.2.2
     # via requests
 cffi==1.16.0
     # via cryptography
 charset-normalizer==3.3.2
     # via requests
 check-wheel-contents==0.6.0
     # via -r /root/pysparkplug/requirements/packaging.in
 click==8.1.7
     # via check-wheel-contents
-cryptography==42.0.2
+cryptography==42.0.7
     # via secretstorage
-docutils==0.20.1
+docutils==0.21.2
     # via readme-renderer
-idna==3.6
+idna==3.7
     # via requests
-importlib-metadata==7.0.1
+importlib-metadata==7.1.0
     # via
     #   keyring
     #   twine
-jaraco-classes==3.3.1
+jaraco-classes==3.4.0
+    # via keyring
+jaraco-context==5.3.0
+    # via keyring
+jaraco-functools==4.0.1
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-keyring==24.3.0
+keyring==25.2.0
     # via twine
 markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==10.2.0
-    # via jaraco-classes
-nh3==0.2.15
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
+nh3==0.2.17
     # via readme-renderer
-packaging==23.2
+packaging==24.0
     # via
     #   build
     #   check-wheel-contents
-pkginfo==1.9.6
+pkginfo==1.10.0
     # via twine
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==2.6.1
+pydantic==2.7.1
     # via check-wheel-contents
-pydantic-core==2.16.2
+pydantic-core==2.18.2
     # via pydantic
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   readme-renderer
     #   rich
-pyproject-hooks==1.0.0
+pyproject-hooks==1.1.0
     # via build
-readme-renderer==42.0
+readme-renderer==43.0
     # via twine
 requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.7.0
+rich==13.7.1
     # via twine
 secretstorage==3.3.3
     # via keyring
 twine==5.0.0
     # via -r /root/pysparkplug/requirements/packaging.in
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   pydantic
     #   pydantic-core
-urllib3==2.2.0
+urllib3==2.2.1
     # via
     #   requests
     #   twine
 wheel-filename==1.4.1
     # via check-wheel-contents
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-metadata
```

### Comparing `pysparkplug-0.3.1/requirements/publish.txt` & `pysparkplug-0.3.2/requirements/publish.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,86 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    ./nox.sh -s update_requirements
 #
-build==1.0.3
+backports-tarfile==1.1.1
+    # via jaraco-context
+build==1.2.1
     # via -r /root/pysparkplug/requirements/publish.in
 certifi==2024.2.2
     # via requests
 cffi==1.16.0
     # via cryptography
 charset-normalizer==3.3.2
     # via requests
-cryptography==42.0.2
+cryptography==42.0.7
     # via secretstorage
-docutils==0.20.1
+docutils==0.21.2
     # via readme-renderer
-idna==3.6
+idna==3.7
     # via requests
-importlib-metadata==7.0.1
+importlib-metadata==7.1.0
     # via
     #   keyring
     #   twine
-jaraco-classes==3.3.1
+jaraco-classes==3.4.0
+    # via keyring
+jaraco-context==5.3.0
+    # via keyring
+jaraco-functools==4.0.1
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-keyring==24.3.0
+keyring==25.2.0
     # via twine
 markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==10.2.0
-    # via jaraco-classes
-nh3==0.2.15
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
+nh3==0.2.17
     # via readme-renderer
-packaging==23.2
+packaging==24.0
     # via build
 paho-mqtt==1.6.1
     # via -r /root/pysparkplug/requirements/requirements.txt
-pkginfo==1.9.6
+pkginfo==1.10.0
     # via twine
-protobuf==4.25.2
+protobuf==5.26.1
     # via -r /root/pysparkplug/requirements/requirements.txt
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   readme-renderer
     #   rich
-pyproject-hooks==1.0.0
+pyproject-hooks==1.1.0
     # via build
-readme-renderer==42.0
+readme-renderer==43.0
     # via twine
 requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.7.0
+rich==13.7.1
     # via twine
 secretstorage==3.3.3
     # via keyring
 twine==5.0.0
     # via -r /root/pysparkplug/requirements/publish.in
-urllib3==2.2.0
+urllib3==2.2.1
     # via
     #   requests
     #   twine
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-metadata
```

### Comparing `pysparkplug-0.3.1/requirements/pylint.txt` & `pysparkplug-0.3.2/requirements/pylint.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    ./nox.sh -s update_requirements
 #
-argcomplete==3.2.2
+argcomplete==3.3.0
     # via nox
-astroid==3.0.3
+astroid==3.1.0
     # via pylint
 colorlog==6.8.2
     # via nox
 dill==0.3.8
     # via pylint
 distlib==0.3.8
     # via virtualenv
-filelock==3.13.1
+filelock==3.14.0
     # via virtualenv
 isort==5.13.2
     # via pylint
 mccabe==0.7.0
     # via pylint
-nox==2023.4.22
+nox==2024.4.15
     # via -r /root/pysparkplug/requirements/pylint.in
-packaging==23.2
+packaging==24.0
     # via
     #   -r /root/pysparkplug/requirements/pylint.in
     #   nox
 paho-mqtt==1.6.1
     # via -r /root/pysparkplug/requirements/requirements.txt
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   pylint
     #   virtualenv
-protobuf==4.25.2
+protobuf==5.26.1
     # via -r /root/pysparkplug/requirements/requirements.txt
-pylint==3.0.3
+pylint==3.1.0
     # via -r /root/pysparkplug/requirements/pylint.in
-tomlkit==0.12.3
+tomlkit==0.12.4
     # via pylint
-virtualenv==20.25.0
+virtualenv==20.26.1
     # via nox
```

### Comparing `pysparkplug-0.3.1/requirements/unit_tests.txt` & `pysparkplug-0.3.2/requirements/unit_tests.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    ./nox.sh -s update_requirements
 #
-coverage[toml]==7.4.1
+coverage[toml]==7.5.1
     # via -r /root/pysparkplug/requirements/unit_tests.in
 iniconfig==2.0.0
     # via pytest
-packaging==23.2
+packaging==24.0
     # via
     #   -r /root/pysparkplug/requirements/unit_tests.in
     #   pytest
 paho-mqtt==1.6.1
     # via -r /root/pysparkplug/requirements/requirements.txt
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-protobuf==4.25.2
+protobuf==5.26.1
     # via -r /root/pysparkplug/requirements/requirements.txt
-pytest==8.0.0
+pytest==8.2.0
     # via -r /root/pysparkplug/requirements/unit_tests.in
```

### Comparing `pysparkplug-0.3.1/src/pysparkplug/__init__.py` & `pysparkplug-0.3.2/src/pysparkplug/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/src/pysparkplug/_client.py` & `pysparkplug-0.3.2/src/pysparkplug/_client.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/src/pysparkplug/_config.py` & `pysparkplug-0.3.2/src/pysparkplug/_config.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/src/pysparkplug/_datatype.py` & `pysparkplug-0.3.2/src/pysparkplug/_datatype.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/src/pysparkplug/_edge_node.py` & `pysparkplug-0.3.2/src/pysparkplug/_edge_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,14 +406,15 @@
                 "registered to this edge node"
             ) from exc
         device.update(metrics)
         d_data_topic = Topic(
             message_type=MessageType.DDATA,
             group_id=self.group_id,
             edge_node_id=self.edge_node_id,
+            device_id=device_id,
         )
         d_data = DData(get_current_timestamp(), seq=self._seq, metrics=metrics)
         self._client.publish(
             Message(
                 topic=d_data_topic, payload=d_data, qos=QoS.AT_MOST_ONCE, retain=False
             ),
             include_dtypes=True,
```

### Comparing `pysparkplug-0.3.1/src/pysparkplug/_enums.py` & `pysparkplug-0.3.2/src/pysparkplug/_enums.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/src/pysparkplug/_error.py` & `pysparkplug-0.3.2/src/pysparkplug/_error.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/src/pysparkplug/_message.py` & `pysparkplug-0.3.2/src/pysparkplug/_message.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/src/pysparkplug/_metric.py` & `pysparkplug-0.3.2/src/pysparkplug/_metric.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/src/pysparkplug/_payload.py` & `pysparkplug-0.3.2/src/pysparkplug/_payload.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/src/pysparkplug/_strenum.py` & `pysparkplug-0.3.2/src/pysparkplug/_strenum.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/src/pysparkplug/_topic.py` & `pysparkplug-0.3.2/src/pysparkplug/_topic.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/src/pysparkplug/_protobuf/__init__.py` & `pysparkplug-0.3.2/src/pysparkplug/_protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/src/pysparkplug/_protobuf/sparkplug_b_pb2.py` & `pysparkplug-0.3.2/src/pysparkplug/_protobuf/sparkplug_b_pb2.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/test/unit_tests/test_topic.py` & `pysparkplug-0.3.2/test/unit_tests/test_topic.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/test/unit_tests/test_version.py` & `pysparkplug-0.3.2/test/unit_tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/LICENSE` & `pysparkplug-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/README.md` & `pysparkplug-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/pyproject.toml` & `pysparkplug-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysparkplug-0.3.1/PKG-INFO` & `pysparkplug-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pysparkplug
-Version: 0.3.1
+Version: 0.3.2
 Summary: An open-source, Python implementation of Sparkplug B, an MQTT topic and payload definition standard
 Project-URL: Documentation, https://pysparkplug.mattefay.com
 Project-URL: Changelog, https://pysparkplug.mattefay.com/en/stable/changelog.html
 Project-URL: Source, https://github.com/matteosox/pysparkplug
 Project-URL: Bug Tracker, https://github.com/matteosox/pysparkplug/issues
 Author-email: Matt Fay <matt.e.fay@gmail.com>
 License: Apache License, Version 2.0
```

