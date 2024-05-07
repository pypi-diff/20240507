# Comparing `tmp/fabrictestbed_extensions-1.6.4.tar.gz` & `tmp/fabrictestbed-extensions-1.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed_extensions-1.6.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.7.0b1.tar", last modified: Tue May  7 21:35:03 2024, max compression
```

## Comparing `fabrictestbed_extensions-1.6.4.tar` & `fabrictestbed-extensions-1.7.0b1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1025 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/.github/workflows/build.yml
--rw-r--r--   0        0        0     2035 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2122 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2419 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/.github/workflows/test.yml
--rw-r--r--   0        0        0     1839 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/.gitignore
--rw-r--r--   0        0        0      666 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/.readthedocs.yaml
--rw-r--r--   0        0        0     8774 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/CHANGELOG.md
--rw-r--r--   0        0        0     4063 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/CONTRIBUTING.md
--rw-r--r--   0        0        0     1071 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/LICENSE
--rw-r--r--   0        0        0     3139 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/README.md
--rw-r--r--   0        0        0      638 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/docs/Makefile
--rw-r--r--   0        0        0      799 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/docs/make.bat
--rw-r--r--   0        0        0        0 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/docs/source/_static/.empty
--rw-r--r--   0        0        0      202 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/docs/source/component.rst
--rw-r--r--   0        0        0     2085 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/docs/source/conf.py
--rw-r--r--   0        0        0      194 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/docs/source/fablib.rst
--rw-r--r--   0        0        0      221 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/docs/source/facility_port.rst
--rw-r--r--   0        0        0     4660 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/docs/source/index.rst
--rw-r--r--   0        0        0      202 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/docs/source/interface.rst
--rw-r--r--   0        0        0      231 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/docs/source/network_service.rst
--rw-r--r--   0        0        0      177 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/docs/source/node.rst
--rw-r--r--   0        0        0      202 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/docs/source/resources.rst
--rw-r--r--   0        0        0      182 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/docs/source/slice.rst
--rw-r--r--   0        0        0     1275 2024-03-05 18:11:07.626160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18044 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6203 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68406 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0    22176 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0        0 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/config/__init__.py
--rw-r--r--   0        0        0    27012 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/config/config.py
--rw-r--r--   0        0        0      937 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/config/fabric_rc
--rw-r--r--   0        0        0     2188 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/config/fabric_rc.yml
--rw-r--r--   0        0        0     5980 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/constants.py
--rw-r--r--   0        0        0    70882 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5918 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    27519 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    44090 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0   128313 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    44659 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    85468 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2024-03-05 18:11:07.630160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3081 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8437 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     3344 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/utils/utils.py
--rw-r--r--   0        0        0     1857 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/pyproject.toml
--rw-r--r--   0        0        0    13331 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/benchmarks/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    20582 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/benchmarks/link_benchmark.py
--rw-r--r--   0        0        0    20886 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/benchmarks/local_network_benchmark.py
--rw-r--r--   0        0        0    44920 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/benchmarks/network_benchmark_tests.py
--rw-r--r--   0        0        0    10017 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/benchmarks/nvme_benchmark.py
--rw-r--r--   0        0        0    14764 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/integration/abc_test.py
--rw-r--r--   0        0        0    34368 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/integration/component_tests.py
--rw-r--r--   0        0        0     6055 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/integration/test_L2_reconfig_post_reboot.py
--rw-r--r--   0        0        0     1574 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/integration/test_bastion_ssh.py
--rw-r--r--   0        0        0     2333 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/integration/test_fablib_node.py
--rw-r--r--   0        0        0     4724 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/integration/test_fabnetv4_ext.py
--rw-r--r--   0        0        0     2106 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/integration/test_hello_fabric.py
--rw-r--r--   0        0        0     1742 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/integration/test_list_resources.py
--rw-r--r--   0        0        0     6165 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/integration/test_modify.py
--rw-r--r--   0        0        0        1 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/unit/__init__.py
--rw-r--r--   0        0        0       85 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/unit/data/dummy-token.json
--rw-r--r--   0        0        0        0 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/unit/data/dummy_fabric_rc
--rw-r--r--   0        0        0     9703 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tests/unit/test_basic.py
--rw-r--r--   0        0        0      574 2024-03-05 18:11:07.634160 fabrictestbed_extensions-1.6.4/tox.ini
--rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 fabrictestbed_extensions-1.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1025 2024-01-03 17:13:50.029023 fabrictestbed-extensions-1.7.0b1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2035 2024-01-21 19:20:59.048027 fabrictestbed-extensions-1.7.0b1/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2122 2024-01-03 17:13:50.029249 fabrictestbed-extensions-1.7.0b1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2419 2024-01-03 17:13:50.029347 fabrictestbed-extensions-1.7.0b1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1839 2024-01-03 17:13:50.029463 fabrictestbed-extensions-1.7.0b1/.gitignore
+-rw-r--r--   0        0        0      666 2024-01-03 17:13:50.029564 fabrictestbed-extensions-1.7.0b1/.readthedocs.yaml
+-rw-r--r--   0        0        0     9535 2024-04-12 02:30:44.048179 fabrictestbed-extensions-1.7.0b1/CHANGELOG.md
+-rw-r--r--   0        0        0     4063 2024-01-03 17:13:50.029859 fabrictestbed-extensions-1.7.0b1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1071 2024-01-03 17:13:50.030147 fabrictestbed-extensions-1.7.0b1/LICENSE
+-rw-r--r--   0        0        0     3139 2024-01-03 17:13:50.030275 fabrictestbed-extensions-1.7.0b1/README.md
+-rw-r--r--   0        0        0      638 2024-01-03 17:13:50.030423 fabrictestbed-extensions-1.7.0b1/docs/Makefile
+-rw-r--r--   0        0        0      799 2024-01-03 17:13:50.030515 fabrictestbed-extensions-1.7.0b1/docs/make.bat
+-rw-r--r--   0        0        0        0 2024-01-03 17:13:50.030647 fabrictestbed-extensions-1.7.0b1/docs/source/_static/.empty
+-rw-r--r--   0        0        0      202 2024-01-26 16:31:25.056208 fabrictestbed-extensions-1.7.0b1/docs/source/component.rst
+-rw-r--r--   0        0        0     2085 2024-01-26 16:31:25.056490 fabrictestbed-extensions-1.7.0b1/docs/source/conf.py
+-rw-r--r--   0        0        0      194 2024-01-26 16:31:25.056860 fabrictestbed-extensions-1.7.0b1/docs/source/fablib.rst
+-rw-r--r--   0        0        0      221 2024-01-26 16:31:25.057306 fabrictestbed-extensions-1.7.0b1/docs/source/facility_port.rst
+-rw-r--r--   0        0        0     4660 2024-01-03 17:13:50.031193 fabrictestbed-extensions-1.7.0b1/docs/source/index.rst
+-rw-r--r--   0        0        0      202 2024-01-26 16:31:25.057692 fabrictestbed-extensions-1.7.0b1/docs/source/interface.rst
+-rw-r--r--   0        0        0      231 2024-01-26 16:31:25.057917 fabrictestbed-extensions-1.7.0b1/docs/source/network_service.rst
+-rw-r--r--   0        0        0      177 2024-01-26 16:31:25.058093 fabrictestbed-extensions-1.7.0b1/docs/source/node.rst
+-rw-r--r--   0        0        0      202 2024-01-26 16:31:25.058265 fabrictestbed-extensions-1.7.0b1/docs/source/resources.rst
+-rw-r--r--   0        0        0      182 2024-01-26 16:31:25.058427 fabrictestbed-extensions-1.7.0b1/docs/source/slice.rst
+-rw-r--r--   0        0        0     1275 2024-01-03 17:13:50.031839 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2024-01-03 17:13:50.031979 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18044 2024-04-01 13:48:09.192195 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6203 2024-01-03 17:13:50.032506 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68406 2024-04-04 15:13:02.815679 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2024-01-03 17:13:50.032855 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0    22218 2024-04-11 20:25:15.953846 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0        0 2024-01-21 19:20:59.049407 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/config/__init__.py
+-rw-r--r--   0        0        0    27012 2024-04-01 13:48:09.193153 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/config/config.py
+-rw-r--r--   0        0        0      937 2024-01-21 19:20:59.051547 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/config/fabric_rc
+-rw-r--r--   0        0        0     2188 2024-01-21 19:20:59.052184 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/config/fabric_rc.yml
+-rw-r--r--   0        0        0     5980 2024-01-21 19:20:59.052774 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/constants.py
+-rw-r--r--   0        0        0    79094 2024-04-29 13:08:58.629831 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     6448 2024-04-01 13:48:09.197245 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    29298 2024-04-26 18:11:21.349989 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    45196 2024-04-18 21:56:59.872123 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0   130565 2024-04-19 00:06:13.943171 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    38833 2024-04-15 14:38:44.633650 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    87733 2024-04-19 00:06:13.956844 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2024-01-03 17:13:50.037482 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2024-01-03 17:13:50.038812 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2024-01-03 17:13:50.039141 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2024-01-03 17:13:50.039555 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2024-01-03 17:13:50.039928 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3081 2024-01-03 17:13:50.040240 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2024-01-03 17:13:50.040416 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8437 2024-01-03 17:13:50.040640 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     3344 2024-01-21 19:20:59.057473 fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/utils/utils.py
+-rw-r--r--   0        0        0     1861 2024-05-07 21:34:23.745606 fabrictestbed-extensions-1.7.0b1/pyproject.toml
+-rw-r--r--   0        0        0    13331 2024-01-03 17:13:50.041343 fabrictestbed-extensions-1.7.0b1/tests/benchmarks/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    20582 2024-01-03 17:13:50.041656 fabrictestbed-extensions-1.7.0b1/tests/benchmarks/link_benchmark.py
+-rw-r--r--   0        0        0    20886 2024-01-03 17:13:50.041910 fabrictestbed-extensions-1.7.0b1/tests/benchmarks/local_network_benchmark.py
+-rw-r--r--   0        0        0    44920 2024-01-03 17:13:50.042329 fabrictestbed-extensions-1.7.0b1/tests/benchmarks/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10017 2024-01-03 17:13:50.042624 fabrictestbed-extensions-1.7.0b1/tests/benchmarks/nvme_benchmark.py
+-rw-r--r--   0        0        0    14764 2024-01-03 17:13:50.042922 fabrictestbed-extensions-1.7.0b1/tests/integration/abc_test.py
+-rw-r--r--   0        0        0    34368 2024-01-03 17:13:50.043157 fabrictestbed-extensions-1.7.0b1/tests/integration/component_tests.py
+-rw-r--r--   0        0        0     6055 2024-01-03 17:13:50.043447 fabrictestbed-extensions-1.7.0b1/tests/integration/test_L2_reconfig_post_reboot.py
+-rw-r--r--   0        0        0     1574 2024-01-03 17:13:50.043635 fabrictestbed-extensions-1.7.0b1/tests/integration/test_bastion_ssh.py
+-rw-r--r--   0        0        0     2333 2024-01-03 17:13:50.043815 fabrictestbed-extensions-1.7.0b1/tests/integration/test_fablib_node.py
+-rw-r--r--   0        0        0     4724 2024-01-03 17:13:50.044060 fabrictestbed-extensions-1.7.0b1/tests/integration/test_fabnetv4_ext.py
+-rw-r--r--   0        0        0     2106 2024-01-03 17:13:50.044206 fabrictestbed-extensions-1.7.0b1/tests/integration/test_hello_fabric.py
+-rw-r--r--   0        0        0     1742 2024-01-03 17:13:50.044332 fabrictestbed-extensions-1.7.0b1/tests/integration/test_list_resources.py
+-rw-r--r--   0        0        0     6165 2024-01-03 17:13:50.044545 fabrictestbed-extensions-1.7.0b1/tests/integration/test_modify.py
+-rw-r--r--   0        0        0        1 2024-01-03 17:13:50.044830 fabrictestbed-extensions-1.7.0b1/tests/unit/__init__.py
+-rw-r--r--   0        0        0       85 2024-01-03 17:13:50.045253 fabrictestbed-extensions-1.7.0b1/tests/unit/data/dummy-token.json
+-rw-r--r--   0        0        0        0 2024-01-21 19:20:59.058394 fabrictestbed-extensions-1.7.0b1/tests/unit/data/dummy_fabric_rc
+-rw-r--r--   0        0        0     9703 2024-01-21 19:20:59.059468 fabrictestbed-extensions-1.7.0b1/tests/unit/test_basic.py
+-rw-r--r--   0        0        0      574 2024-01-03 17:13:50.045807 fabrictestbed-extensions-1.7.0b1/tox.ini
+-rw-r--r--   0        0        0     4559 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.7.0b1/PKG-INFO
```

### Comparing `fabrictestbed_extensions-1.6.4/.github/workflows/build.yml` & `fabrictestbed-extensions-1.7.0b1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/.github/workflows/checks.yml` & `fabrictestbed-extensions-1.7.0b1/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/.github/workflows/publish.yml` & `fabrictestbed-extensions-1.7.0b1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/.github/workflows/test.yml` & `fabrictestbed-extensions-1.7.0b1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/.gitignore` & `fabrictestbed-extensions-1.7.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/.readthedocs.yaml` & `fabrictestbed-extensions-1.7.0b1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/CHANGELOG.md` & `fabrictestbed-extensions-1.7.0b1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 This is the changelog file for FABRIC testbed extensions.  All notable
 changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+# Unreleased
+
+### Fixed
+- Add display of switch port name to network service table listing (Issue [#152](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/152))
+- Error *may* be inaccurate or wrong when I issue an invalid configuration. (Issue [#304](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/304))
+- Add Facility Port to allow adding multiple interfaces (Issue [#289](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/289))
+- validate_config errors out when config directory does not exist (Issue [#299](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/299)
+- create_ssh_config adds extra indentation (Issue [#300](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/300)
+
 ## [1.6.4] - 2024-03-05
 
 ### Fixed
 - Can't instantiate FablibManager without config file (Issue [#286](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/286))
 - Reduce the time taken for the call node.get_ssh_command() (Issue [#280](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/280))
 - Allow access to other user's slices in a project (Issue [#279](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/279))
 - Allow user to specify Lease End time for Slice creation (Issue [#51](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/51)]
```

### Comparing `fabrictestbed_extensions-1.6.4/CONTRIBUTING.md` & `fabrictestbed-extensions-1.7.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/LICENSE` & `fabrictestbed-extensions-1.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/README.md` & `fabrictestbed-extensions-1.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/docs/Makefile` & `fabrictestbed-extensions-1.7.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/docs/make.bat` & `fabrictestbed-extensions-1.7.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/docs/source/conf.py` & `fabrictestbed-extensions-1.7.0b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/docs/source/index.rst` & `fabrictestbed-extensions-1.7.0b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/__init__.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -665,13 +665,14 @@
     def get_user_data(self):
         try:
             return json.loads(str(self.get_fim().get_property(pname="user_data")))
         except:
             return {}
 
     def delete(self):
-        for interface in self.get_interfaces():
-            interface.delete()
+        if self.get_interfaces():
+            for interface in self.get_interfaces():
+                interface.delete()
 
         self.get_slice().get_fim_topology().nodes[
             self.get_node().get_name()
         ].remove_component(name=self.get_name())
```

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/config/config.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/config/config.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/config/fabric_rc` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/config/fabric_rc`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/config/fabric_rc.yml` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/config/fabric_rc.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/constants.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/constants.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/fablib.py`

 * *Files 12% similar despite different names*

```diff
@@ -65,30 +65,36 @@
 
 import datetime
 import json
 import logging
 import os
 import random
 import time
+import traceback
+import warnings
+
+warnings.filterwarnings("always", category=DeprecationWarning)
+
 from concurrent.futures import ThreadPoolExecutor
 from ipaddress import IPv4Network, IPv6Network
-from typing import TYPE_CHECKING, Dict, List
+from typing import TYPE_CHECKING, Dict, List, Tuple
 
 import pandas as pd
 import paramiko
 from IPython import get_ipython
 from IPython.core.display_functions import display
 from tabulate import tabulate
 
 from fabrictestbed_extensions.fablib.config.config import Config, ConfigException
 from fabrictestbed_extensions.fablib.constants import Constants
 from fabrictestbed_extensions.utils.utils import Utils
 
 if TYPE_CHECKING:
     from fabric_cf.orchestrator.swagger_client import Slice as OrchestratorSlice
+    from fabrictestbed_extensions.fablib.node import Node
 
 from fabrictestbed.slice_manager import SliceManager, SliceState, Status
 from fim.user import Node as FimNode
 
 from fabrictestbed_extensions.fablib.resources import FacilityPorts, Links, Resources
 from fabrictestbed_extensions.fablib.slice import Slice
 
@@ -668,27 +674,60 @@
             self.ssh_thread_pool_executor = ThreadPoolExecutor(execute_thread_pool_size)
             self.setup_logging()
             self.__build_slice_manager()
         self.required_check()
 
     def validate_config(self):
         """
-        Validate Fablib config - checks if all the required configuration exists for slice provisioning to work successfully
+        Validate and create Fablib config - checks if all the required configuration exists for slice
+        provisioning to work successfully
 
         - Checks Credential Manager Host is configured properly
 
         - Checks Orchestrator Host is configured properly
 
         - Checks Core API Host is configured properly
 
         - Checks Bastion Host is configured properly
 
-        - Check Sliver keys exist
+        - Check Sliver keys exist; create sliver keys if they do not exist
 
-        - Check Bastion keys exist and are not expired
+        - Check Bastion keys exist and are not expired; update/create bastion keys if expired or do not exist
+
+        - Check Bastion Username is configured
+
+        - Check Project Id is configured
+
+        .. deprecated:: 1.6.5
+           Use `verify_and_configure()` instead.
+        @raises Exception if the configuration is invalid
+        """
+        warnings.warn(
+            "This function is deprecated and will be removed in future releases, "
+            "please use 'verify_and_configure' instead.",
+            DeprecationWarning,
+        )
+        self.verify_and_configure()
+
+    def verify_and_configure(self):
+        """
+        Validate and create Fablib config - checks if all the required configuration exists for slice
+        provisioning to work successfully
+
+        - Checks Credential Manager Host is configured properly
+
+        - Checks Orchestrator Host is configured properly
+
+        - Checks Core API Host is configured properly
+
+        - Checks Bastion Host is configured properly
+
+        - Check Sliver keys exist; create sliver keys if they do not exist
+
+        - Check Bastion keys exist and are not expired; update/create bastion keys if expired or do not exist
 
         - Check Bastion Username is configured
 
         - Check Project Id is configured
 
         @raises Exception if the configuration is invalid
         """
@@ -754,29 +793,38 @@
         if bastion_ssh_config_file is None:
             raise ConfigException("Bastion SSH Config File location not specified")
 
         if os.path.exists(bastion_ssh_config_file) and not overwrite:
             print("Bastion SSH Config file already exists, not making updates!")
             return
 
+        dir_path = os.path.dirname(bastion_ssh_config_file)
+        if not os.path.exists(dir_path):
+            msg = (
+                f"Directory {dir_path} does not exist, can not create ssh_config file!"
+            )
+            print(msg)
+            logging.error(msg)
+            raise Exception(msg)
+
         with open(bastion_ssh_config_file, "w") as f:
             f.write(
                 f"""UserKnownHostsFile /dev/null
-    StrictHostKeyChecking no
-    ServerAliveInterval 120 
+StrictHostKeyChecking no
+ServerAliveInterval 120 
 
-    Host bastion.fabric-testbed.net
-         User {self.get_bastion_username()}
-         ForwardAgent yes
-         Hostname %h
-         IdentityFile {self.get_bastion_key_location()}
-         IdentitiesOnly yes
+Host bastion.fabric-testbed.net
+     User {self.get_bastion_username()}
+     ForwardAgent yes
+     Hostname %h
+     IdentityFile {self.get_bastion_key_location()}
+     IdentitiesOnly yes
 
-    Host * !bastion.fabric-testbed.net
-         ProxyJump {self.get_bastion_username()}@bastion.fabric-testbed.net:22
+Host * !bastion.fabric-testbed.net
+     ProxyJump {self.get_bastion_username()}@bastion.fabric-testbed.net:22
     """
             )
 
     def validate_and_update_bastion_keys(self):
         """
         Validate Bastion Key; if key does not exist or is expired, it create bastion keys
         """
@@ -923,14 +971,22 @@
 
         :param public_file_path: public key location
         :type public_file_path: str
 
         :param store_pubkey flag indicating if the public key should be saved
         :type store_pubkey: bool
         """
+        dir_path = os.path.dirname(private_file_path)
+        if not os.path.exists(dir_path):
+            msg = (
+                f"Directory {dir_path} does not exist, can not create {key_type} keys!"
+            )
+            print(msg)
+            logging.error(msg)
+            raise Exception(msg)
         comment = os.path.basename(private_file_path)
         ssh_keys = self.get_slice_manager().create_ssh_keys(
             key_type=key_type,
             description=description,
             comment=comment,
             store_pubkey=store_pubkey,
         )
@@ -2160,7 +2216,160 @@
         if fields is None:
             for key, value in data.items():
                 table.append([key, value])
         else:
             for field in fields:
                 table.append([field, data[field]])
         return table
+
+    @staticmethod
+    def __can_allocate_node_in_worker(
+        worker: FimNode, node: Node, allocated: dict, site: FimNode
+    ) -> Tuple[bool, str]:
+        """
+        Check if a node can be provisioned on a worker node on a site w.r.t available resources on that site
+
+        :return: Tuple indicating status for validation and error message in case of failure
+        :rtype: Tuple[bool, str]
+        """
+        if worker is None or site is None:
+            return True, f"Ignoring validation: Worker: {worker}, Site: {site} not available."
+
+        msg = f"Node can be allocated on the host: {worker.name}."
+
+        worker_maint_info = site.maintenance_info.get(worker.name)
+        if worker_maint_info and str(worker_maint_info.state) != "Active":
+            msg = f"Node cannot be allocated on {worker.name}, {worker.name} is in {worker_maint_info.state}!"
+            return False, msg
+
+        allocated_core = allocated.setdefault("core", 0)
+        allocated_ram = allocated.setdefault("ram", 0)
+        allocated_disk = allocated.setdefault("disk", 0)
+        available_cores = (
+            worker.capacities.core
+            - (
+                worker.capacity_allocations.core
+                if worker.capacity_allocations is not None
+                else 0
+            )
+            - allocated_core
+        )
+        available_ram = (
+            worker.capacities.ram
+            - (
+                worker.capacity_allocations.ram
+                if worker.capacity_allocations is not None
+                else 0
+            )
+            - allocated_ram
+        )
+        available_disk = (
+            worker.capacities.disk
+            - (
+                worker.capacity_allocations.disk
+                if worker.capacity_allocations is not None
+                else 0
+            )
+            - allocated_disk
+        )
+
+        if (
+            node.get_requested_cores() > available_cores
+            or node.get_requested_disk() > available_disk
+            or node.get_requested_ram() > available_ram
+        ):
+            msg = f"Insufficient Resources: Host: {worker.name} does not meet core/ram/disk requirements."
+            return False, msg
+
+        # Check if there are enough components available
+        for c in node.get_components():
+            comp_model_type = f"{c.get_type()}-{c.get_fim_model()}"
+            if comp_model_type not in worker.components:
+                msg = f"Invalid Request: Host: {worker.name} does not have the requested component: {comp_model_type}."
+                return False, msg
+
+            allocated_comp_count = allocated.setdefault(comp_model_type, 0)
+            available_comps = (
+                worker.components[comp_model_type].capacities.unit
+                - (
+                    worker.components[comp_model_type].capacity_allocations.unit
+                    if worker.components[comp_model_type].capacity_allocations
+                    else 0
+                )
+                - allocated_comp_count
+            )
+            if available_comps <= 0:
+                msg = f"Insufficient Resources: Host: {worker.name} has reached the limit for component: {comp_model_type}."
+                return False, msg
+
+            allocated[comp_model_type] += 1
+
+        allocated["core"] += node.get_requested_cores()
+        allocated["ram"] += node.get_requested_ram()
+        allocated["disk"] += node.get_requested_disk()
+
+        return True, msg
+
+    def validate_node(self, node: Node, allocated: dict = None) -> Tuple[bool, str]:
+        """
+        Validate a node w.r.t available resources on a site before submission
+
+        :return: Tuple indicating status for validation and error message in case of failure
+        :rtype: Tuple[bool, str]
+        """
+        try:
+            error = None
+            if allocated is None:
+                allocated = {}
+            site = self.get_resources().get_topology_site(site_name=node.get_site())
+
+            if not site:
+                logging.warning(f"Ignoring validation: Site: {node.get_site()} not available in resources.")
+                return True, f"Ignoring validation: Site: {node.get_site()} not available in resources."
+
+            site_maint_info = site.maintenance_info.get(site.name)
+            if site_maint_info and str(site_maint_info.state) != "Active":
+                msg = f"Node cannot be allocated on {node.get_site()}, {node.get_site()} is in {site_maint_info.state}."
+                logging.error(msg)
+                return False, msg
+            workers = self.get_resources().get_nodes(site=site)
+            if not workers:
+                msg = (
+                    f"Node cannot be validated, host information not available for {site}."
+                )
+                logging.error(msg)
+                return False, msg
+
+            if node.get_host():
+                if node.get_host() not in workers:
+                    msg = f"Invalid Request: Requested Host {node.get_host()} does not exist on site: {node.get_site()}."
+                    logging.error(msg)
+                    return False, msg
+
+                worker = workers.get(node.get_host())
+
+                allocated_comps = allocated.setdefault(node.get_host(), {})
+                status, error = self.__can_allocate_node_in_worker(
+                    worker=worker, node=node, allocated=allocated_comps, site=site
+                )
+
+                if not status:
+                    logging.error(error)
+                    return status, error
+
+            for worker in workers.values():
+                allocated_comps = allocated.setdefault(worker.name, {})
+                status, error = self.__can_allocate_node_in_worker(
+                    worker=worker, node=node, allocated=allocated_comps, site=site
+                )
+                if status:
+                    return status, error
+
+            msg = f"Invalid Request: Requested Node cannot be accommodated by any of the hosts on site: {site.name}."
+            if error:
+                msg += f" Details: {error}"
+            logging.error(msg)
+            return False, msg
+        except Exception as e:
+            logging.error(e)
+            logging.error(traceback.format_exc())
+            return False, str(e)
```

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,33 +28,33 @@
 
 .. _`facility ports`: https://learn.fabric-testbed.net/knowledge-base/glossary/#facility_port
 """
 
 from __future__ import annotations
 
 import json
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, List, Union
 
 import jinja2
 from fabrictestbed.slice_editor import Capacities, Labels
 from tabulate import tabulate
 
 from fabrictestbed_extensions.fablib.interface import Interface
 
 if TYPE_CHECKING:
-    from fim.user.interface import Interface as FimInterface
+    from fim.user.node import Node as FimNode
 
     from fabrictestbed_extensions.fablib.slice import Slice
 
 
 class FacilityPort:
     fim_interface = None
     slice = None
 
-    def __init__(self, slice: Slice, fim_interface: FimInterface):
+    def __init__(self, slice: Slice, fim_interface: FimNode):
         """
         :param slice: the fablib slice to have this node on
         :type slice: Slice
 
         :param fim_interface:
         :type fim_interface: FimInterface
         """
@@ -115,15 +115,15 @@
             output=output,
             quiet=quiet,
             pretty_names_dict=pretty_names_dict,
         )
 
         return table
 
-    def get_fim_interface(self) -> FimInterface:
+    def get_fim_interface(self) -> FimNode:
         return self.fim_interface
 
     def get_model(self) -> str:
         return "Facility_Port"
 
     def get_name(self) -> str:
         """
@@ -137,27 +137,43 @@
         return self.fim_interface.site
 
     @staticmethod
     def new_facility_port(
         slice: Slice = None,
         name: str = None,
         site: str = None,
-        vlan: str = None,
+        vlan: Union[str, list] = None,
         bandwidth: int = 10,
     ):
-        fim_facility_port = slice.get_fim_topology().add_facility(
-            name=name,
-            site=site,
-            capacities=Capacities(bw=bandwidth),
-            labels=Labels(vlan=vlan),
-        )
+        if isinstance(vlan, list):
+            interfaces = []
+            index = 1
+            for v in vlan:
+                iface_tuple = (
+                    f"iface-{index}",
+                    Labels(vlan=v),
+                    Capacities(bw=bandwidth),
+                )
+                interfaces.append(iface_tuple)
+            fim_facility_port = slice.get_fim_topology().add_facility(
+                name=name,
+                site=site,
+                interfaces=interfaces,
+            )
+        else:
+            fim_facility_port = slice.get_fim_topology().add_facility(
+                name=name,
+                site=site,
+                capacities=Capacities(bw=bandwidth),
+                labels=Labels(vlan=vlan),
+            )
         return FacilityPort(slice, fim_facility_port)
 
     @staticmethod
-    def get_facility_port(slice: Slice = None, facility_port: FimInterface = None):
+    def get_facility_port(slice: Slice = None, facility_port: FimNode = None):
         """
 
         :param slice:
         :param facility_port:
         :return:
         """
         return FacilityPort(slice, facility_port)
@@ -191,10 +207,10 @@
         :raise Exception: if interface is not found
 
         :return: an interface on the node
         :rtype: Interface
         """
         ifaces = []
         for fim_interface in self.get_fim_interface().interface_list:
-            ifaces.append(Interface(component=self, fim_interface=fim_interface))
+            ifaces.append(Interface(node=self, fim_interface=fim_interface))
 
         return ifaces
```

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,56 +29,66 @@
 
 from __future__ import annotations
 
 import ipaddress
 import json
 import logging
 from ipaddress import IPv4Address
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Union
 
 import jinja2
 from fabrictestbed.slice_editor import Flags
 from tabulate import tabulate
 
 if TYPE_CHECKING:
     from fabrictestbed_extensions.fablib.slice import Slice
     from fabrictestbed_extensions.fablib.node import Node
     from fabrictestbed_extensions.fablib.network_service import NetworkService
     from fabrictestbed_extensions.fablib.component import Component
+    from fabrictestbed_extensions.fablib.facility_port import FacilityPort
 
 from fabrictestbed.slice_editor import UserData
 from fim.user.interface import Interface as FimInterface
 
 
 class Interface:
     CONFIGURED = "configured"
     MODE = "mode"
     AUTO = "auto"
     MANUAL = "manual"
     ADDR = "addr"
     CONFIG = "config"
 
-    def __init__(self, component: Component = None, fim_interface: FimInterface = None):
+    def __init__(
+        self,
+        component: Component = None,
+        fim_interface: FimInterface = None,
+        node: FacilityPort = None,
+    ):
         """
         .. note::
 
             Objects of this class are not created directly.
 
         :param component: the component to set on this interface
         :type component: Component
 
         :param fim_interface: the FABRIC information model interface
             to set on this fablib interface
         :type fim_interface: FimInterface
+
+        :param node: the facility Port to which interface is assoicated with
+        :type node: FacilityPort
         """
         super().__init__()
         self.fim_interface = fim_interface
         self.component = component
         self.network = None
         self.dev = None
+        self.node = node
 
     def get_fablib_manager(self):
         return self.get_slice().get_fablib_manager()
 
     def __str__(self):
         """
         Creates a tabulated string describing the properties of the interface.
@@ -100,14 +110,15 @@
             ["Mode", self.get_mode()],
             ["VLAN", self.get_vlan()],
             ["MAC", self.get_mac()],
             ["Physical Device", self.get_physical_os_interface_name()],
             ["Device", self.get_os_interface()],
             ["Address", self.get_ip_addr()],
             ["Numa Node", self.get_numa_node()],
+            ["Switch Port", self.get_switch_port()],
         ]
 
         return tabulate(table)
 
     def toJson(self):
         """
         Returns the interface attributes as a json string
@@ -135,14 +146,15 @@
             "error": "Error",
             "ssh_command": "SSH Command",
             "public_ssh_key_file": "Public SSH Key File",
             "private_ssh_key_file": "Private SSH Key File",
             "mode": "Mode",
             "ip_addr": "IP Address",
             "numa": "Numa Node",
+            "switch_port": "Switch Port",
         }
 
     def toDict(self, skip=[]):
         """
         Returns the interface attributes as a dictionary
 
         :return: slice attributes as dictionary
@@ -186,16 +198,28 @@
                 str(self.get_vlan()) if self.get_vlan() else ""
             ),  # str(self.get_vlan()),
             "mac": mac,
             "physical_dev": physical_dev,
             "dev": dev,
             "ip_addr": ip_addr,
             "numa": str(self.get_numa_node()),
+            "switch_port": str(self.get_switch_port()),
         }
 
+    def get_switch_port(self) -> str:
+        network = self.get_network()
+        if network and network.get_fim():
+            ifs = None
+            for ifs_name in network.get_fim().interfaces.keys():
+                if self.get_name() in ifs_name:
+                    ifs = network.get_fim().interfaces[ifs_name]
+                    break
+            if ifs and ifs.labels and ifs.labels.local_name:
+                return ifs.labels.local_name
+
     def get_numa_node(self) -> str:
         if self.get_component() is not None:
             return self.get_component().get_numa_node()
 
     def generate_template_context(self):
         context = self.toDict()
         return context
@@ -516,35 +540,51 @@
 
         if_labels = self.get_fim_interface().get_property(pname="labels")
         if_labels.vlan = str(vlan)
         self.get_fim_interface().set_properties(labels=if_labels)
 
         return self
 
+    def set_bandwidth(self, bw: int):
+        """
+        Set the Bandwidths on the FABRIC request.
+
+        :param addr: bw
+        :type addr: int
+        """
+        if not bw:
+            return
+
+        if_capacities = self.get_fim_interface().get_property(pname="capacities")
+        if_capacities.bw = int(bw)
+        self.get_fim_interface().set_properties(capacities=if_capacities)
+
+        return self
+
     def get_fim_interface(self) -> FimInterface:
         """
         Not recommended for most users.
 
         Gets the node's FABRIC Information Model (fim) object. This method
         is used to access data at a lower level than FABlib.
 
         :return: the FABRIC model node
         :rtype: fim interface
         """
         return self.fim_interface
 
-    def get_bandwidth(self) -> str:
+    def get_bandwidth(self) -> int:
         """
         Gets the bandwidth of an interface. Basic NICs claim 0 bandwidth but
         are 100 Gbps shared by all Basic NICs on the host.
 
         :return: bandwith
         :rtype: String
         """
-        if self.get_component().get_model() == "NIC_Basic":
+        if self.get_component() and self.get_component().get_model() == "NIC_Basic":
             return 100
         else:
             return self.get_fim_interface().capacities.bw
 
     def get_vlan(self) -> str:
         """
         Gets the FABRIC VLAN of an interface.
@@ -554,14 +594,27 @@
         """
         try:
             vlan = self.get_fim_interface().get_property(pname="labels").vlan
         except:
             vlan = None
         return vlan
 
+    def get_bandwidth(self) -> int:
+        """
+        Gets the FABRIC bandwidth of an interface.
+
+        :return: VLAN
+        :rtype: String
+        """
+        try:
+            bw = self.get_fim_interface().get_property(pname="capacities").bw
+        except:
+            bw = None
+        return bw
+
     def get_reservation_id(self) -> str or None:
         try:
             # TODO THIS DOESNT WORK.
             # print(f"{self.get_fim_interface()}")
             return (
                 self.get_fim_interface()
                 .get_property(pname="reservation_info")
@@ -631,42 +684,48 @@
     def get_model(self) -> str:
         """
         Gets the component model type on this interface's component.
 
         :return: the model of this interface's component
         :rtype: str
         """
-        return self.get_component().get_model()
+        if self.node:
+            return self.node.get_model()
+        else:
+            return self.get_component().get_model()
 
     def get_site(self) -> str:
         """
         Gets the site this interface's component is on.
 
         :return: the site this interface is on
         :rtype: str
         """
-        return self.get_component().get_site()
+        return self.get_node().get_site()
 
     def get_slice(self) -> Slice:
         """
         Gets the FABLIB slice this interface's node is attached to.
 
         :return: the slice this interface is attached to
         :rtype: Slice
         """
         return self.get_node().get_slice()
 
-    def get_node(self) -> Node:
+    def get_node(self) -> Union[Node, FacilityPort]:
         """
         Gets the node this interface's component is on.
 
         :return: the node this interface is attached to
         :rtype: Node
         """
-        return self.get_component().get_node()
+        if self.node:
+            return self.node
+        else:
+            return self.get_component().get_node()
 
     def get_network(self) -> NetworkService:
         """
         Gets the network this interface is on.
 
         :return: the network service this interface is on
         :rtype: NetworkService
@@ -686,16 +745,14 @@
                 if net.has_interface(self):
                     self.network = net
                     logging.debug(
                         f"Interface network found. interface {self.get_name()}, network {self.network.get_name()}"
                     )
                     return self.network
 
-        return None
-
     # fablib.Interface.get_ip_link()
     def get_ip_link(self):
         """
         Gets the ip link info for this interface.
 
         :return ip link info
         :rtype: str
@@ -720,22 +777,20 @@
         try:
             if not dev:
                 dev = self.get_os_interface()
 
             stdout, stderr = self.get_node().execute(
                 f"ip -j addr show {dev}", quiet=True
             )
+            return stdout
         except Exception as e:
-            (f"Exception: {e}")
             logging.error(
-                f"Failed to get ip addr show info for interface {self.get_name()}"
+                f"Failed to get ip addr show info for interface {self.get_name()} Exception: {e}"
             )
 
-        return stdout
-
     # fablib.Interface.get_ip_addr()
     def get_ip_addr_ssh(self, dev=None):
         """
         Gets the ip addr info for this interface.
 
         :return ip addr info
         :rtype: str
@@ -919,9 +974,9 @@
             name=name,
             from_interface_name=port_name,
             to_interface=self.get_fim_interface(),
         )
 
     def delete(self):
         net = self.get_network()
-
-        net.remove_interface(self)
+        if net:
+            net.remove_interface(self)
```

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/network_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,29 +28,30 @@
 
 .. _`network services`: https://learn.fabric-testbed.net/knowledge-base/glossary/#network_service
 """
 
 from __future__ import annotations
 
 import logging
+import threading
 from typing import TYPE_CHECKING, List, Union
 
 from tabulate import tabulate
 
 if TYPE_CHECKING:
     from fabrictestbed_extensions.fablib.slice import Slice
     from fabrictestbed_extensions.fablib.interface import Interface
     from fabric_cf.orchestrator.swagger_client import Sliver as OrchestratorSliver
 
 import ipaddress
 import json
 from ipaddress import IPv4Address, IPv4Network, IPv6Address, IPv6Network
 
 import jinja2
-from fabrictestbed.slice_editor import Flags, Labels
+from fabrictestbed.slice_editor import Labels
 from fabrictestbed.slice_editor import NetworkService as FimNetworkService
 from fabrictestbed.slice_editor import ServiceType, UserData
 from fim.slivers.network_service import NSLayer, ServiceType
 from fim.user.network_service import MirrorDirection
 
 
 class NetworkService:
@@ -130,22 +131,22 @@
         basic_nic_count = 0
 
         sites = set([])
         includes_facility_port = False
         facility_port_interfaces = 0
         for interface in interfaces:
             sites.add(interface.get_site())
-            if isinstance(interface.get_component(), FacilityPort):
+            if isinstance(interface.get_node(), FacilityPort):
                 includes_facility_port = True
                 facility_port_interfaces += 1
             if interface.get_model() == "NIC_Basic":
                 basic_nic_count += 1
 
         rtn_nstype = None
-        if len(sites) <= 1 and len(sites) >= 0:
+        if 1 >= len(sites) >= 0:
             rtn_nstype = NetworkService.network_service_map["L2Bridge"]
         # elif basic_nic_count == 0 and len(sites) == 2 and len(interfaces) == 2:
         #    #TODO: remove this when STS works on all links.
         #    rtn_nstype = NetworkService.network_service_map['L2PTP']
         elif len(sites) == 2:
             # Use L2STS when connecting two facility ports instead of L2PTP
             # L2PTP limitation for Facility Ports:
@@ -162,28 +163,30 @@
             )
 
         return rtn_nstype
 
     @staticmethod
     def validate_nstype(type, interfaces):
         """
-        Not inteded for API use
+        Not intended for API use
 
 
         Verifies the network service type against the number of interfaces.
 
         :param type: the network service type to check
         :type type: ServiceType
         :param interfaces: the list of interfaces to check
         :type interfaces: list[Interface]
         :raises Exception: if the network service type is invalid based on the number of interfaces
         :return: true if the network service type is valid based on the number of interfaces
         :rtype: bool
         """
 
+        from fabrictestbed_extensions.fablib.facility_port import FacilityPort
+
         sites = set([])
         nics = set([])
         nodes = set([])
         for interface in interfaces:
             try:
                 sites.add(interface.get_site())
                 nics.add(interface.get_model())
@@ -193,45 +196,63 @@
                     f"validate_nstype: skipping interface {interface.get_name()}, likely its a facility port"
                 )
 
         # models: 'NIC_Basic', 'NIC_ConnectX_6', 'NIC_ConnectX_5'
         if type == NetworkService.network_service_map["L2Bridge"]:
             if len(sites) > 1:
                 raise Exception(
-                    f"Network type {type} must be empty or include interfaces from exactly one site. {len(sites)} sites requested: {sites}"
+                    f"Network type {type} must be empty or include interfaces from exactly one site. {len(sites)} "
+                    f"sites requested: {sites}"
                 )
 
         elif type == NetworkService.network_service_map["L2PTP"]:
             if not len(sites) == 2:
                 raise Exception(
-                    f"Network type {type} must include interfaces from exactly two sites. {len(sites)} sites requested: {sites}"
+                    f"Network type {type} must include interfaces from exactly two sites. {len(sites)} sites "
+                    f"requested: {sites}"
                 )
             if "NIC_Basic" in nics:
                 raise Exception(
                     f"Network type {type} does not support interfaces of type 'NIC_Basic'"
                 )
 
         elif type == NetworkService.network_service_map["L2STS"]:
             exception_list = []
             if len(sites) != 2:
                 exception_list.append(
-                    f"Network type {type} must include interfaces from exactly two sites. {len(sites)} sites requested: {sites}"
+                    f"Network type {type} must include interfaces from exactly two sites. {len(sites)} sites "
+                    f"requested: {sites}"
                 )
             if len(interfaces) > 2:
                 hosts = set([])
+                nodes_per_site = {}
+                for interface in interfaces:
+                    node = interface.get_node()
+                    if node.get_site() not in nodes_per_site:
+                        nodes_per_site[node.get_site()] = 0
+                    if isinstance(node, FacilityPort):
+                        continue
+                    nodes_per_site[node.get_site()] += 1
                 for interface in interfaces:
                     node = interface.get_node()
-                    if interface.get_model() == "NIC_Basic":
-                        if node.get_host() == None:
+                    if (
+                        interface.get_model() == "NIC_Basic"
+                        and nodes_per_site[node.get_site()] > 1
+                    ):
+                        if node.get_host() is None:
                             exception_list.append(
-                                f"Network type {type} does not support multiple NIC_Basic interfaces on VMs residing on the same host. Please see Node.set_host(host_nane) to explicitily bind a nodes to a specific host. Node {node.get_name()} is unbound."
+                                f"Network type {type} does not support multiple NIC_Basic interfaces on VMs "
+                                f"residing on the same host. Please see Node.set_host(host_name) to explicitly "
+                                f"bind a nodes to a specific host. Node {node.get_name()} is unbound."
                             )
                         elif node.get_host() in hosts:
                             exception_list.append(
-                                f"Network type {type} does not support multiple NIC_Basic interfaces on VMs residing on the same host. Please see Node.set_host(host_nane) to explicitily bind a nodes to a specific host. Multiple nodes bound to {node.get_host()}."
+                                f"Network type {type} does not support multiple NIC_Basic interfaces on VMs residing "
+                                f"on the same host. Please see Node.set_host(host_name) to explicitly bind a nodes "
+                                f"to a specific host. Multiple nodes bound to {node.get_host()}."
                             )
                         else:
                             hosts.add(node.get_host())
 
             if len(exception_list) > 0:
                 raise Exception(f"{exception_list}")
         else:
@@ -385,23 +406,23 @@
         NetworkService.validate_nstype(nstype, interfaces)
 
         # Set default VLANs for P2P networks that did not pass in VLANs
         if nstype == ServiceType.L2PTP:  # or nstype == ServiceType.L2STS:
             vlan1 = interfaces[0].get_vlan()
             vlan2 = interfaces[1].get_vlan()
 
-            if vlan1 == None and vlan2 == None:
+            if vlan1 is None and vlan2 is None:
                 # TODO: Long term we might have multiple vlan on one property
                 # and will need to make sure they are unique.  For now this okay
                 interfaces[0].set_vlan("100")
                 interfaces[1].set_vlan("100")
-            elif vlan1 == None and vlan2 != None:
+            elif vlan1 is None and vlan2 is not None:
                 # Match VLANs if one is set.
                 interfaces[0].set_vlan(vlan2)
-            elif vlan1 != None and vlan2 == None:
+            elif vlan1 is not None and vlan2 is None:
                 # Match VLANs if one is set.
                 interfaces[1].set_vlan(vlan1)
 
             # for interface in interfaces:
             #    if interface.get_model() != 'NIC_Basic' and not interface.get_vlan():
             #
             #        interface.set_vlan("100")
@@ -600,14 +621,15 @@
                 self.sliver = self.slice.get_sliver(
                     reservation_id=self.get_reservation_id()
                 )
         except:
             pass
 
         self.sliver = None
+        self.lock = threading.Lock()
 
     def __str__(self):
         """
         Creates a tabulated string describing the properties of the network service.
 
         Intended for printing network service information.
 
@@ -1161,50 +1183,58 @@
         if "subnet" not in fablib_data:
             fablib_data["subnet"] = {}
         allocated_ips = fablib_data["subnet"]["allocated_ips"]
         allocated_ips.append(str(addr))
         self.set_fablib_data(fablib_data)
 
     def allocate_ip(self, addr: IPv4Address or IPv6Address = None):
-        subnet = self.get_subnet()
-        allocated_ips = self.get_allocated_ips()
+        try:
+            self.lock.acquire()
+            subnet = self.get_subnet()
+            allocated_ips = self.get_allocated_ips()
 
-        if addr:
-            # if addr != subnet.network_address and addr not in allocated_ips:
-            if addr not in allocated_ips:
-                self.set_allocated_ip(addr)
-                return addr
-        elif (
-            type(subnet) == ipaddress.IPv4Network
-            or type(subnet) == ipaddress.IPv6Network
-        ):
-            for host in subnet:
-                if host != subnet.network_address and host not in allocated_ips:
-                    self.set_allocated_ip(host)
+            if addr:
+                # if addr != subnet.network_address and addr not in allocated_ips:
+                if addr not in allocated_ips:
+                    self.set_allocated_ip(addr)
+                    return addr
+            elif (
+                type(subnet) == ipaddress.IPv4Network
+                or type(subnet) == ipaddress.IPv6Network
+            ):
+                for host in subnet:
+                    if host != subnet.network_address and host not in allocated_ips:
+                        self.set_allocated_ip(host)
 
-                    return host
-        return None
+                        return host
+            return None
+        finally:
+            self.lock.release()
 
     def set_allocated_ips(self, allocated_ips: list[IPv4Address or IPv6Address]):
         fablib_data = self.get_fablib_data()
         allocated_ips_strs = []
         for ip in allocated_ips:
             allocated_ips_strs.append(str(ip))
 
         if "subnet" not in fablib_data:
             fablib_data["subnet"] = {}
 
         fablib_data["subnet"]["allocated_ips"] = allocated_ips_strs
         self.set_fablib_data(fablib_data)
 
     def free_ip(self, addr: IPv4Address or IPv6Address):
-        allocated_ips = self.get_allocated_ips()
-        if addr in allocated_ips:
-            allocated_ips.remove(addr)
-        self.set_allocated_ips(allocated_ips)
+        try:
+            self.lock.acquire()
+            allocated_ips = self.get_allocated_ips()
+            if addr in allocated_ips:
+                allocated_ips.remove(addr)
+            self.set_allocated_ips(allocated_ips)
+        finally:
+            self.lock.release()
 
     def make_ip_publicly_routable(self, ipv6: list[str] = None, ipv4: list[str] = None):
         labels = self.fim_network_service.labels
         if labels is None:
             labels = Labels()
         if self.fim_network_service.type == ServiceType.FABNetv4Ext:
             labels = Labels.update(labels, ipv4=ipv4)
```

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,35 +41,31 @@
     node.execute('echo Hello, FABRIC from node `hostname -s`')
 
     slice.delete()
 """
 
 from __future__ import annotations
 
-import concurrent.futures
 import ipaddress
 import json
 import logging
-import os
 import re
 import select
 import threading
 import time
 import traceback
-from concurrent.futures import ThreadPoolExecutor
 from typing import TYPE_CHECKING, Dict, List, Tuple, Union
 
 import jinja2
 import paramiko
 from fabric_cf.orchestrator.orchestrator_proxy import Status
 from IPython.core.display_functions import display
 from tabulate import tabulate
 
 from fabrictestbed_extensions.fablib.network_service import NetworkService
-from fabrictestbed_extensions.utils.utils import Utils
 
 if TYPE_CHECKING:
     from fabrictestbed_extensions.fablib.slice import Slice
     from fabric_cf.orchestrator.swagger_client import Sliver as OrchestratorSliver
 
 from ipaddress import IPv4Address, IPv4Network, IPv6Address, IPv6Network, ip_address
 
@@ -84,29 +80,40 @@
 
 class Node:
     default_cores = 2
     default_ram = 8
     default_disk = 10
     default_image = "default_rocky_8"
 
-    def __init__(self, slice: Slice, node: FimNode):
+    def __init__(
+        self, slice: Slice, node: FimNode, validate: bool = False, raise_exception: bool = False
+    ):
         """
         Node constructor, usually invoked by ``Slice.add_node()``.
 
         :param slice: the fablib slice to have this node on
         :type slice: Slice
 
         :param node: the FIM node that this Node represents
         :type node: Node
+
+        :param validate: Validate node can be allocated w.r.t available resources
+        :type validate: bool
+
+        :param raise_exception: Raise exception in case validation failes
+        :type raise_exception: bool
+
         """
         super().__init__()
         self.fim_node = node
         self.slice = slice
         self.host = None
         self.ip_addr_list_json = None
+        self.validate = validate
+        self.raise_exception = raise_exception
 
         # Try to set the username.
         try:
             self.set_username()
         except:
             self.username = None
 
@@ -160,15 +167,20 @@
         :return: SM sliver for the node
         :rtype: Sliver
         """
         return self.sliver
 
     @staticmethod
     def new_node(
-        slice: Slice = None, name: str = None, site: str = None, avoid: List[str] = []
+        slice: Slice = None,
+        name: str = None,
+        site: str = None,
+        avoid: List[str] = [],
+        validate: bool = False,
+        raise_exception: bool = False,
     ):
         """
         Not intended for API call.  See: Slice.add_node()
 
         Creates a new FABRIC node and returns a fablib node with the
         new node.
 
@@ -180,22 +192,35 @@
 
         :param site: the name of the site to build the node on
         :type site: str
 
         :param avoid: a list of node names to avoid
         :type avoid: List[str]
 
+        :param validate: Validate node can be allocated w.r.t available resources
+        :type validate: bool
+
+        :param raise_exception: Raise exception in case of failure
+        :type raise_exception: bool
+
         :return: a new fablib node
         :rtype: Node
         """
         if site is None:
-            [site] = slice.get_fablib_manager().get_random_sites(avoid=avoid)
+            [site] = slice.get_fablib_manager().get_random_sites(
+                avoid=avoid,
+            )
 
         logging.info(f"Adding node: {name}, slice: {slice.get_name()}, site: {site}")
-        node = Node(slice, slice.topology.add_node(name=name, site=site))
+        node = Node(
+            slice,
+            slice.topology.add_node(name=name, site=site),
+            validate=validate,
+            raise_exception=raise_exception,
+        )
         node.set_capacities(
             cores=Node.default_cores, ram=Node.default_ram, disk=Node.default_disk
         )
         node.set_image(Node.default_image)
 
         node.init_fablib_data()
 
@@ -817,38 +842,74 @@
         :rtype: int
         """
         try:
             return self.get_fim_node().get_property(pname="capacity_allocations").core
         except:
             return None
 
+    def get_requested_cores(self) -> int or None:
+        """
+        Gets the requested number of cores on the FABRIC node.
+
+        :return: the requested number of cores on the node
+        :rtype: int
+        """
+        try:
+            return self.get_fim_node().get_property(pname="capacities").core
+        except:
+            return 0
+
     def get_ram(self) -> int or None:
         """
         Gets the amount of RAM on the FABRIC node.
 
         :return: the amount of RAM on the node
         :rtype: int
         """
         try:
             return self.get_fim_node().get_property(pname="capacity_allocations").ram
         except:
             return None
 
+    def get_requested_ram(self) -> int or None:
+        """
+        Gets the requested amount of RAM on the FABRIC node.
+
+        :return: the requested amount of RAM on the node
+        :rtype: int
+        """
+        try:
+            return self.get_fim_node().get_property(pname="capacities").ram
+        except:
+            return 0
+
     def get_disk(self) -> int or None:
         """
         Gets the amount of disk space on the FABRIC node.
 
         :return: the amount of disk space on the node
         :rtype: int
         """
         try:
             return self.get_fim_node().get_property(pname="capacity_allocations").disk
         except:
             return None
 
+    def get_requested_disk(self) -> int or None:
+        """
+        Gets the amount of disk space on the FABRIC node.
+
+        :return: the amount of disk space on the node
+        :rtype: int
+        """
+        try:
+            return self.get_fim_node().get_property(pname="capacities").disk
+        except:
+            return 0
+
     def get_image(self) -> str or None:
         """
         Gets the image reference on the FABRIC node.
 
         :return: the image reference on the node
         :rtype: String
         """
@@ -875,19 +936,22 @@
 
         :return: the hostname on the node
         :rtype: String
         """
         try:
             if self.host is not None:
                 return self.host
-            return (
-                self.get_fim_node()
-                .get_property(pname="label_allocations")
-                .instance_parent
+            label_allocations = self.get_fim_node().get_property(
+                pname="label_allocations"
             )
+            labels = self.get_fim_node().get_property(pname="labels")
+            if label_allocations:
+                return label_allocations.instance_parent
+            if labels:
+                return labels.instance_parent
         except:
             return None
 
     def get_site(self) -> str or None:
         """
         Gets the sitename on the FABRIC node.
 
@@ -1110,17 +1174,26 @@
 
         :param name: the name of the new component
         :type name: String
 
         :return: the new component
         :rtype: Component
         """
-        return Component.new_component(
+        component = Component.new_component(
             node=self, model=model, name=name, user_data=user_data
         )
+        if self.validate:
+            status, error = self.get_fablib_manager().validate_node(node=self)
+            if not status:
+                component.delete()
+                component = None
+                logging.warning(error)
+                if self.raise_exception:
+                    raise ValueError(error)
+        return component
 
     def get_components(self) -> List[Component]:
         """
         Gets a list of components associated with this node.
 
         :return: a list of components on this node
         :rtype: List[Component]
@@ -3189,15 +3262,15 @@
         'Node 6': {'Heap': '6', 'Huge': '0', 'Private': '32812', 'Stack': '0', 'Total': '32817'},
         'Node 7': {'Heap': '0', 'Huge': '0', 'Private': '0', 'Stack': '0', 'Total': '0'},
         'Total': {'Heap': '6', 'Huge': '0', 'Private': '32813', 'Stack': '0', 'Total': '32818'}}
 
         VM INFO looks like:
         In this example below, no CPU pinning has been applied so CPU Affinity lists all the CPUs
         After the pinning has been applied, CPU Affinity would show only the pinned CPU
-        [{'CPU': '116', 'CPU Affinity': '0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,70,71,72,73,74,75,76,77,78,79,80,81,82,83,84,85,86,87,88,89,90,91,92,93,94,95,96,97,98,99,100,101,102,103,104,105,106,107,108,109,110,111,112,113,114,115,116,117,118,119,120,121,122,123,124,125,126,127', 'CPU time': '20.2s', 'State': 'running', 'VCPU': '0'},
+            [{'CPU': '116', 'CPU Affinity': '0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,70,71,72,73,74,75,76,77,78,79,80,81,82,83,84,85,86,87,88,89,90,91,92,93,94,95,96,97,98,99,100,101,102,103,104,105,106,107,108,109,110,111,112,113,114,115,116,117,118,119,120,121,122,123,124,125,126,127', 'CPU time': '20.2s', 'State': 'running', 'VCPU': '0'},
         {'CPU': '118', 'CPU Affinity': '0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,70,71,72,73,74,75,76,77,78,79,80,81,82,83,84,85,86,87,88,89,90,91,92,93,94,95,96,97,98,99,100,101,102,103,104,105,106,107,108,109,110,111,112,113,114,115,116,117,118,119,120,121,122,123,124,125,126,127', 'CPU time': '9.0s', 'State': 'running', 'VCPU': '1'},
         {'CPU': '117', 'CPU Affinity': '0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,70,71,72,73,74,75,76,77,78,79,80,81,82,83,84,85,86,87,88,89,90,91,92,93,94,95,96,97,98,99,100,101,102,103,104,105,106,107,108,109,110,111,112,113,114,115,116,117,118,119,120,121,122,123,124,125,126,127', 'CPU time': '8.9s', 'State': 'running', 'VCPU': '2'},
         {'CPU': '119', 'CPU Affinity': '0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,70,71,72,73,74,75,76,77,78,79,80,81,82,83,84,85,86,87,88,89,90,91,92,93,94,95,96,97,98,99,100,101,102,103,104,105,106,107,108,109,110,111,112,113,114,115,116,117,118,119,120,121,122,123,124,125,126,127', 'CPU time': '8.8s', 'State': 'running', 'VCPU': '3'},
         {'CPU': '52', 'CPU Affinity': '0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,70,71,72,73,74,75,76,77,78,79,80,81,82,83,84,85,86,87,88,89,90,91,92,93,94,95,96,97,98,99,100,101,102,103,104,105,106,107,108,109,110,111,112,113,114,115,116,117,118,119,120,121,122,123,124,125,126,127', 'CPU time': '0.8s', 'State': 'running', 'VCPU': '4'},
         {'CPU': '88', 'CPU Affinity': '0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,70,71,72,73,74,75,76,77,78,79,80,81,82,83,84,85,86,87,88,89,90,91,92,93,94,95,96,97,98,99,100,101,102,103,104,105,106,107,108,109,110,111,112,113,114,115,116,117,118,119,120,121,122,123,124,125,126,127', 'CPU time': '0.4s', 'State': 'running', 'VCPU': '5'},
         {'CPU': '54', 'CPU Affinity': '0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,70,71,72,73,74,75,76,77,78,79,80,81,82,83,84,85,86,87,88,89,90,91,92,93,94,95,96,97,98,99,100,101,102,103,104,105,106,107,108,109,110,111,112,113,114,115,116,117,118,119,120,121,122,123,124,125,126,127', 'CPU time': '1.4s', 'State': 'running', 'VCPU': '6'},
         {'CPU': '55', 'CPU Affinity': '0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,70,71,72,73,74,75,76,77,78,79,80,81,82,83,84,85,86,87,88,89,90,91,92,93,94,95,96,97,98,99,100,101,102,103,104,105,106,107,108,109,110,111,112,113,114,115,116,117,118,119,120,121,122,123,124,125,126,127', 'CPU time': '0.8s', 'State': 'running', 'VCPU': '7'},
```

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/resources.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,69 +29,129 @@
 .. _`resources`: https://learn.fabric-testbed.net/knowledge-base/glossary/#resource
 """
 
 from __future__ import annotations
 
 import json
 import logging
-from typing import List, Tuple
+import traceback
+from typing import Dict, List, Tuple
 
 from fabrictestbed.slice_editor import AdvertisedTopology, Capacities
 from fabrictestbed.slice_manager import Status
-from fim.slivers import maintenance_mode, network_node
-from fim.user import composite_node, interface, link, node
+from fim.slivers import network_node
+from fim.user import interface, link, node
+from fim.view_only_dict import ViewOnlyDict
 from tabulate import tabulate
 
 
 class Resources:
+    NON_PRETTY_NAME = "non_pretty_name"
+    PRETTY_NAME = "pretty_name"
+    HEADER_NAME = "header_name"
+    AVAILABLE = "Available"
+    CAPACITY = "Capacity"
+    ALLOCATED = "Allocated"
+    VALUE = "value"
+
+    NIC_SHARED_CONNECTX_6 = "SharedNIC-ConnectX-6"
+    SMART_NIC_CONNECTX_6 = "SmartNIC-ConnectX-6"
+    SMART_NIC_CONNECTX_5 = "SmartNIC-ConnectX-5"
+    NVME_P4510 = "NVME-P4510"
+    GPU_TESLA_T4 = "GPU-Tesla T4"
+    GPU_RTX6000 = "GPU-RTX6000"
+    GPU_A30 = "GPU-A30"
+    GPU_A40 = "GPU-A40"
+    FPGA_XILINX_U280 = "FPGA-Xilinx-U280"
+    CORES = "Cores"
+    RAM = "Ram"
+    DISK = "Disk"
+    CPUS = "CPUs"
+    HOSTS = "Hosts"
+
+    site_attribute_name_mappings = {
+        CORES.lower(): {NON_PRETTY_NAME: CORES.lower(), PRETTY_NAME: CORES, HEADER_NAME: CORES},
+        RAM.lower(): {
+            NON_PRETTY_NAME: RAM.lower(),
+            PRETTY_NAME: RAM,
+            HEADER_NAME: f"{RAM} ({Capacities.UNITS[RAM.lower()]})",
+        },
+        DISK: {
+            NON_PRETTY_NAME: DISK.lower(),
+            PRETTY_NAME: DISK,
+            HEADER_NAME: f"{DISK} ({Capacities.UNITS[DISK.lower()]})",
+        },
+        NIC_SHARED_CONNECTX_6: {
+            NON_PRETTY_NAME: "nic_basic",
+            PRETTY_NAME: "Basic NIC",
+            HEADER_NAME: "Basic (100 Gbps NIC)",
+        },
+        SMART_NIC_CONNECTX_6: {
+            NON_PRETTY_NAME: "nic_connectx_6",
+            PRETTY_NAME: "ConnectX-6",
+            HEADER_NAME: "ConnectX-6 (100 Gbps x2 NIC)",
+        },
+        SMART_NIC_CONNECTX_5: {
+            NON_PRETTY_NAME: "nic_connectx_5",
+            PRETTY_NAME: "ConnectX-5",
+            HEADER_NAME: "ConnectX-5 (25 Gbps x2 NIC)",
+        },
+        NVME_P4510: {
+            NON_PRETTY_NAME: "nvme",
+            PRETTY_NAME: "NVMe",
+            HEADER_NAME: "P4510 (NVMe 1TB)",
+        },
+        GPU_TESLA_T4: {
+            NON_PRETTY_NAME: "tesla_t4",
+            PRETTY_NAME: "Tesla T4",
+            HEADER_NAME: "Tesla T4 (GPU)",
+        },
+        GPU_RTX6000: {
+            NON_PRETTY_NAME: "rtx6000",
+            PRETTY_NAME: "RTX6000",
+            HEADER_NAME: "RTX6000 (GPU)",
+        },
+        GPU_A30: {
+            NON_PRETTY_NAME: "a30",
+            PRETTY_NAME: "A30",
+            HEADER_NAME: "A30 (GPU)",
+        },
+        GPU_A40: {
+            NON_PRETTY_NAME: "a40",
+            PRETTY_NAME: "A40",
+            HEADER_NAME: "A40 (GPU)",
+        },
+        FPGA_XILINX_U280: {
+            NON_PRETTY_NAME: "fpga_u280",
+            PRETTY_NAME: "U280",
+            HEADER_NAME: "FPGA-Xilinx-U280",
+        },
+    }
     site_pretty_names = {
         "name": "Name",
         "state": "State",
         "address": "Address",
         "location": "Location",
         "ptp_capable": "PTP Capable",
-        "hosts": "Hosts",
-        "cpus": "CPUs",
-        "cores_available": "Cores Available",
-        "cores_capacity": "Cores Capacity",
-        "cores_allocated": "Cores Allocated",
-        "ram_available": "RAM Available",
-        "ram_capacity": "RAM Capacity",
-        "ram_allocated": "RAM Allocated",
-        "disk_available": "Disk Available",
-        "disk_capacity": "Disk Capacity",
-        "disk_allocated": "Disk Allocated",
-        "nic_basic_available": "Basic NIC Available",
-        "nic_basic_capacity": "Basic NIC Capacity",
-        "nic_basic_allocated": "Basic NIC Allocated",
-        "nic_connectx_6_available": "ConnectX-6 Available",
-        "nic_connectx_6_capacity": "ConnectX-6 Capacity",
-        "nic_connectx_6_allocated": "ConnectX-6 Allocated",
-        "nic_connectx_5_available": "ConnectX-5 Available",
-        "nic_connectx_5_capacity": "ConnectX-5 Capacity",
-        "nic_connectx_5_allocated": "ConnectX-5 Allocated",
-        "nvme_available": "NVMe Available",
-        "nvme_capacity": "NVMe Capacity",
-        "nvme_allocated": "NVMe Allocated",
-        "tesla_t4_available": "Tesla T4 Available",
-        "tesla_t4_capacity": "Tesla T4 Capacity",
-        "tesla_t4_allocated": "Tesla T4 Allocated",
-        "rtx6000_available": "RTX6000 Available",
-        "rtx6000_capacity": "RTX6000 Capacity",
-        "rtx6000_allocated": "RTX6000 Allocated",
-        "a30_available": "A30 Available",
-        "a30_capacity": "A30 Capacity",
-        "a30_allocated": "A30 Allocated",
-        "a40_available": "A40 Available",
-        "a40_capacity": "A40 Capacity",
-        "a40_allocated": "A40 Allocated",
-        "fpga_u280_available": "U280 Available",
-        "fpga_u280_capacity": "U280 Capacity",
-        "fpga_u280_allocated": "U280 Allocated",
+        HOSTS.lower(): HOSTS,
+        CPUS.lower(): CPUS,
     }
+    for attribute, names in site_attribute_name_mappings.items():
+        non_pretty_name = names.get(NON_PRETTY_NAME)
+        pretty_name = names.get(PRETTY_NAME)
+        site_pretty_names[non_pretty_name] = pretty_name
+        site_pretty_names[
+            f"{non_pretty_name}_{AVAILABLE.lower()}"
+        ] = f"{pretty_name} {AVAILABLE}"
+        site_pretty_names[
+            f"{non_pretty_name}_{CAPACITY.lower()}"
+        ] = f"{pretty_name} {CAPACITY}"
+        site_pretty_names[
+            f"{non_pretty_name}_{ALLOCATED.lower()}"
+        ] = f"{pretty_name} {ALLOCATED}"
 
     def __init__(self, fablib_manager, force_refresh: bool = False):
         """
         :param fablib_manager: a :class:`FablibManager` instance.
         :type fablib_manager: fablib.FablibManager
 
         :param force_refresh: force a refresh of available testbed
@@ -112,62 +172,38 @@
 
         Intended for printing available resources.
 
         :return: Tabulated string of available resources
         :rtype: String
         """
         table = []
+        headers = [
+            "Name",
+            "PTP Capable",
+            self.CPUS,
+        ]
         for site_name, site in self.topology.sites.items():
-            # logging.debug(f"site -- {site}")
-            site_sliver = site.get_sliver()
-            table.append(
-                [
-                    site.name,
-                    f"{self.get_ptp_capable()}",
-                    self.get_cpu_capacity(site_sliver),
-                    f"{self.get_core_available(site_sliver)}/{self.get_core_capacity(site_sliver)}",
-                    f"{self.get_ram_available(site_sliver)}/{self.get_ram_capacity(site_sliver)}",
-                    f"{self.get_disk_available(site_sliver)}/{self.get_disk_capacity(site_sliver)}",
-                    # self.get_host_capacity(site),
-                    # self.get_location_postal(site),
-                    # self.get_location_lat_long(site),
-                    f"{self.get_component_available(site_sliver,'SharedNIC-ConnectX-6')}/{self.get_component_capacity(site_sliver,'SharedNIC-ConnectX-6')}",
-                    f"{self.get_component_available(site_sliver,'SmartNIC-ConnectX-6')}/{self.get_component_capacity(site_sliver,'SmartNIC-ConnectX-6')}",
-                    f"{self.get_component_available(site_sliver,'SmartNIC-ConnectX-5')}/{self.get_component_capacity(site_sliver,'SmartNIC-ConnectX-5')}",
-                    f"{self.get_component_available(site_sliver,'NVME-P4510')}/{self.get_component_capacity(site_sliver,'NVME-P4510')}",
-                    f"{self.get_component_available(site_sliver,'GPU-Tesla T4')}/{self.get_component_capacity(site_sliver,'GPU-Tesla T4')}",
-                    f"{self.get_component_available(site_sliver,'GPU-RTX6000')}/{self.get_component_capacity(site_sliver,'GPU-RTX6000')}",
-                    f"{self.get_component_available(site_sliver, 'GPU-A30')}/{self.get_component_capacity(site_sliver, 'GPU-A30')}",
-                    f"{self.get_component_available(site_sliver, 'GPU-A40')}/{self.get_component_capacity(site_sliver, 'GPU-A40')}",
-                    f"{self.get_component_available(site_sliver, 'FPGA-Xilinx-U280')}/{self.get_component_capacity(site_sliver, 'FPGA-Xilinx-U280')}",
-                ]
-            )
+            site_info = self.get_site_info(site)
+            row = [
+                site.name,
+                self.get_ptp_capable(site),
+                self.get_cpu_capacity(site),
+            ]
+            for attribute, names in self.site_attribute_name_mappings.items():
+                allocated = site_info.get(attribute, {}).get(self.ALLOCATED.lower(), 0)
+                capacity = site_info.get(attribute, {}).get(self.CAPACITY.lower(), 0)
+                available = capacity - allocated
+                row.append(f"{available}/{capacity}")
+                headers.append(names.get(self.HEADER_NAME))
+
+            table.append(row)
 
         return tabulate(
             table,
-            headers=[
-                "Name",
-                "PTP Capable",
-                "CPUs",
-                "Cores",
-                f"RAM ({Capacities.UNITS['ram']})",
-                f"Disk ({Capacities.UNITS['disk']})",
-                # "Workers"
-                # "Physical Address",
-                # "Location Coordinates"
-                "Basic (100 Gbps NIC)",
-                "ConnectX-6 (100 Gbps x2 NIC)",
-                "ConnectX-5 (25 Gbps x2 NIC)",
-                "P4510 (NVMe 1TB)",
-                "Tesla T4 (GPU)",
-                "RTX6000 (GPU)",
-                "A30 (GPU)",
-                "A40 (GPU)",
-                "FPGA-Xilinx-U280",
-            ],
+            headers=headers,
         )
 
     def show_site(
         self,
         site_name: str,
         output: str = None,
         fields: list[str] = None,
@@ -183,15 +219,15 @@
         :param site_name: site name
         :type site_name: String
         :return: Tabulated string of available resources
         :rtype: String
         """
         site = self.topology.sites[site_name]
 
-        data = self.site_to_dict(site.get_sliver(), latlon=latlon)
+        data = self.site_to_dict(site, latlon=latlon)
 
         if pretty_names:
             pretty_names_dict = self.site_pretty_names
         else:
             pretty_names_dict = {}
 
         site_table = self.get_fablib_manager().show_table(
@@ -222,15 +258,14 @@
         """
         Not recommended for most users.
         """
         try:
             return self.topology.sites[site_name]
         except Exception as e:
             logging.warning(f"Failed to get site {site_name}")
-            return None
 
     def get_state(self, site: str or node.Node or network_node.NodeSliver) -> str:
         """
         Gets the maintenance state of the node
 
         :param site: site Node or NodeSliver object or name
         :type site: String or Node or NodeSliver
@@ -243,14 +278,101 @@
             if isinstance(site, node.Node):
                 return str(site.maintenance_info.get(site.name).state)
             return str(self.get_topology_site(site).maintenance_info.get(site).state)
         except Exception as e:
             # logging.warning(f"Failed to get site state {site_name}")
             return ""
 
+    def get_nodes(self, site: str or network_node.NodeSliver) -> ViewOnlyDict:
+        """
+        Get worker nodes on a site
+        :param site: site name
+        :type site: String
+        """
+        try:
+            from fim.graph.abc_property_graph import ABCPropertyGraph
+
+            if isinstance(site, str):
+                site = self.get_topology_site(site)
+
+            node_id_list = site.topo.graph_model.get_first_neighbor(
+                node_id=site.node_id,
+                rel=ABCPropertyGraph.REL_HAS,
+                node_label=ABCPropertyGraph.CLASS_NetworkNode,
+            )
+            ret = dict()
+            for nid in node_id_list:
+                _, node_props = site.topo.graph_model.get_node_properties(node_id=nid)
+                n = node.Node(
+                    name=node_props[ABCPropertyGraph.PROP_NAME],
+                    node_id=nid,
+                    topo=site.topo,
+                )
+                # exclude Facility nodes
+                from fim.user import NodeType
+
+                if n.type != NodeType.Facility:
+                    ret[n.name] = n
+            return ViewOnlyDict(ret)
+        except Exception as e:
+            logging.error(f"Error occurred - {e}")
+            logging.error(traceback.format_exc())
+
+    def get_site_info(
+        self, site: str or node.Node or network_node.NodeSliver
+    ) -> Dict[str, Dict[str, int]]:
+        """
+        Gets the total site capacity of all components for a site
+
+        :param site: site object or sliver or site name
+        :type site: String or Node or NodeSliver
+        :return: total component capacity for all components
+        :rtype: Dict[str, int]
+        """
+        site_info = {}
+
+        try:
+            nodes = self.get_nodes(site=site)
+            site_info[self.CORES.lower()] = {
+                self.CAPACITY.lower(): site.capacities.core,
+                self.ALLOCATED.lower(): site.capacity_allocations.core
+                if site.capacity_allocations
+                else 0,
+            }
+            site_info[self.RAM.lower()] = {
+                self.CAPACITY.lower(): site.capacities.ram,
+                self.ALLOCATED.lower(): site.capacity_allocations.ram
+                if site.capacity_allocations
+                else 0,
+            }
+            site_info[self.DISK.lower()] = {
+                self.CAPACITY.lower(): site.capacities.disk,
+                self.ALLOCATED.lower(): site.capacity_allocations.disk
+                if site.capacity_allocations
+                else 0,
+            }
+
+            if nodes:
+                for w in nodes.values():
+                    if w.components:
+                        for component_model_name, c in w.components.items():
+                            comp_cap = site_info.setdefault(component_model_name, {})
+                            comp_cap.setdefault(self.CAPACITY.lower(), 0)
+                            comp_cap.setdefault(self.ALLOCATED.lower(), 0)
+                            comp_cap[self.CAPACITY.lower()] += c.capacities.unit
+                            if c.capacity_allocations:
+                                comp_cap[
+                                    self.ALLOCATED.lower()
+                                ] += c.capacity_allocations.unit
+
+            return site_info
+        except Exception as e:
+            # logging.error(f"Failed to get {component_model_name} capacity {site}: {e}")
+            return site_info
+
     def get_component_capacity(
         self,
         site: str or node.Node or network_node.NodeSliver,
         component_model_name: str,
     ) -> int:
         """
         Gets the total site capacity of a component by model name.
@@ -258,29 +380,27 @@
         :param site: site object or sliver or site name
         :type site: String or Node or NodeSliver
         :param component_model_name: component model name
         :type component_model_name: String
         :return: total component capacity
         :rtype: int
         """
+        component_capacity = 0
         try:
-            if isinstance(site, network_node.NodeSliver):
-                return site.attached_components_info.get_device(
-                    component_model_name
-                ).capacities.unit
-            if isinstance(site, node.Node):
-                return site.components[component_model_name].capacities.unit
-            return (
-                self.get_topology_site(site)
-                .components[component_model_name]
-                .capacities.unit
-            )
+            nodes = self.get_nodes(site=site)
+            if nodes:
+                for w in nodes.values():
+                    if component_model_name in w.components:
+                        component_capacity += w.components[
+                            component_model_name
+                        ].capacities.unit
+            return component_capacity
         except Exception as e:
-            # logging.debug(f"Failed to get {component_model_name} capacity {site}")
-            return 0
+            # logging.error(f"Failed to get {component_model_name} capacity {site}: {e}")
+            return component_capacity
 
     def get_component_allocated(
         self,
         site: str or node.Node or network_node.NodeSliver,
         component_model_name: str,
     ) -> int:
         """
@@ -290,29 +410,30 @@
         :param site: site object or site name
         :type site: String or Node or NodeSliver
         :param component_model_name: component model name
         :type component_model_name: String
         :return: currently allocated component of this model
         :rtype: int
         """
+        component_allocated = 0
         try:
-            if isinstance(site, network_node.NodeSliver):
-                return site.attached_components_info.get_device(
-                    component_model_name
-                ).capacity_allocations.unit
-            if isinstance(site, node.Node):
-                return site.components[component_model_name].capacity_allocations.unit
-            return (
-                self.get_topology_site(site)
-                .components[component_model_name]
-                .capacity_allocations.unit
-            )
+            nodes = self.get_nodes(site=site)
+            if nodes:
+                for w in nodes.values():
+                    if (
+                        component_model_name in w.components
+                        and w.components[component_model_name].capacity_allocations
+                    ):
+                        component_allocated += w.components[
+                            component_model_name
+                        ].capacity_allocations.unit
+            return component_allocated
         except Exception as e:
-            # logging.debug(f"Failed to get {component_model_name} allocated {site}")
-            return 0
+            # logging.error(f"Failed to get {component_model_name} allocated {site}: {e}")
+            return component_allocated
 
     def get_component_available(
         self,
         site: str or node.Node or network_node.NodeSliver,
         component_model_name: str,
     ) -> int:
         """
@@ -623,15 +744,15 @@
         Update the available resources by querying the FABRIC services
 
         """
         logging.info(f"Updating available resources")
         return_status, topology = (
             self.get_fablib_manager()
             .get_slice_manager()
-            .resources(force_refresh=force_refresh)
+            .resources(force_refresh=force_refresh, level=2)
         )
         if return_status != Status.OK:
             raise Exception(
                 "Failed to get advertised_topology: {}, {}".format(
                     return_status, topology
                 )
             )
@@ -691,282 +812,99 @@
     ):
         """
         Convert site information into a dictionary
 
         :param site: site name or site object
         :param latlon: convert address to latlon (makes online call to openstreetmaps.org)
         """
-        core_a = self.get_core_available(site)
-        core_c = self.get_core_capacity(site)
-        ram_a = self.get_ram_available(site)
-        ram_c = self.get_ram_capacity(site)
-        disk_a = self.get_disk_available(site)
-        disk_c = self.get_disk_capacity(site)
-        nic_basic_a = self.get_component_available(site, "SharedNIC-ConnectX-6")
-        nic_basic_c = self.get_component_capacity(site, "SharedNIC-ConnectX-6")
-        nic_cx6_a = self.get_component_available(site, "SmartNIC-ConnectX-6")
-        nic_cx6_c = self.get_component_capacity(site, "SmartNIC-ConnectX-6")
-        nic_cx5_a = self.get_component_available(site, "SmartNIC-ConnectX-5")
-        nic_cx5_c = self.get_component_capacity(site, "SmartNIC-ConnectX-5")
-        nvme_a = self.get_component_available(site, "NVME-P4510")
-        nvme_c = self.get_component_capacity(site, "NVME-P4510")
-        tesla_t4_a = self.get_component_available(site, "GPU-Tesla T4")
-        tesla_t4_c = self.get_component_capacity(site, "GPU-Tesla T4")
-        rtx6000_a = self.get_component_available(site, "GPU-RTX6000")
-        rtx6000_c = self.get_component_capacity(site, "GPU-RTX6000")
-        a30_a = self.get_component_available(site, "GPU-A30")
-        a30_c = self.get_component_capacity(site, "GPU-A30")
-        a40_a = self.get_component_available(site, "GPU-A40")
-        a40_c = self.get_component_capacity(site, "GPU-A40")
-        u280_a = self.get_component_available(site, "FPGA-Xilinx-U280")
-        u280_c = self.get_component_capacity(site, "FPGA-Xilinx-U280")
-        ptp = self.get_ptp_capable(site)
-
+        site_info = self.get_site_info(site)
         d = {
             "name": site.name if isinstance(site, node.Node) else site.get_name(),
             "state": self.get_state(site),
             "address": self.get_location_postal(site),
             "location": self.get_location_lat_long(site) if latlon else "",
-            "ptp_capable": ptp,
+            "ptp_capable": self.get_ptp_capable(site),
             "hosts": self.get_host_capacity(site),
             "cpus": self.get_cpu_capacity(site),
-            "cores_available": core_a,
-            "cores_capacity": core_c,
-            "cores_allocated": core_c - core_a,
-            "ram_available": ram_a,
-            "ram_capacity": ram_c,
-            "ram_allocated": ram_c - ram_a,
-            "disk_available": disk_a,
-            "disk_capacity": disk_c,
-            "disk_allocated": disk_c - disk_a,
-            "nic_basic_available": nic_basic_a,
-            "nic_basic_capacity": nic_basic_c,
-            "nic_basic_allocated": nic_basic_c - nic_basic_a,
-            "nic_connectx_6_available": nic_cx6_a,
-            "nic_connectx_6_capacity": nic_cx6_c,
-            "nic_connectx_6_allocated": nic_cx6_c - nic_cx6_a,
-            "nic_connectx_5_available": nic_cx5_a,
-            "nic_connectx_5_capacity": nic_cx5_c,
-            "nic_connectx_5_allocated": nic_cx5_c - nic_cx5_a,
-            "nvme_available": nvme_a,
-            "nvme_capacity": nvme_c,
-            "nvme_allocated": nvme_c - nvme_a,
-            "tesla_t4_available": tesla_t4_a,
-            "tesla_t4_capacity": tesla_t4_c,
-            "tesla_t4_allocated": tesla_t4_c - tesla_t4_a,
-            "rtx6000_available": rtx6000_a,
-            "rtx6000_capacity": rtx6000_c,
-            "rtx6000_allocated": rtx6000_c - rtx6000_a,
-            "a30_available": a30_a,
-            "a30_capacity": a30_c,
-            "a30_allocated": a30_c - a30_a,
-            "a40_available": a40_a,
-            "a40_capacity": a40_c,
-            "a40_allocated": a40_c - a40_a,
-            "fpga_u280_available": u280_a,
-            "fpga_u280_capacity": u280_c,
-            "fpga_u280_allocated": u280_c - u280_a,
         }
+
+        for attribute, names in self.site_attribute_name_mappings.items():
+            capacity = site_info.get(attribute, {}).get(self.CAPACITY.lower(), 0)
+            allocated = site_info.get(attribute, {}).get(self.ALLOCATED.lower(), 0)
+            available = capacity - allocated
+            d[f"{names.get(self.NON_PRETTY_NAME)}_{self.AVAILABLE.lower()}"] = available
+            d[f"{names.get(self.NON_PRETTY_NAME)}_{self.CAPACITY.lower()}"] = capacity
+            d[f"{names.get(self.NON_PRETTY_NAME)}_{self.ALLOCATED.lower()}"] = allocated
+
         if not latlon:
             d.pop("location")
+
         return d
 
     def site_to_dictXXX(self, site):
         site_name = site.name
-        return {
-            "name": {"pretty_name": "Name", "value": site.name},
+        site_info = self.get_site_info(site)
+        d = {
+            "name": {self.PRETTY_NAME: "Name", self.VALUE: site.name},
             "address": {
-                "pretty_name": "Address",
-                "value": self.get_location_postal(site_name),
+                self.PRETTY_NAME: "Address",
+                self.VALUE: self.get_location_postal(site_name),
             },
             "location": {
-                "pretty_name": "Location",
-                "value": self.get_location_lat_long(site_name),
+                self.PRETTY_NAME: "Location",
+                self.VALUE: self.get_location_lat_long(site_name),
             },
             "ptp": {
-                "pretty_name": "PTP Capable",
-                "value": self.get_ptp_capable(),
-            },
-            "hosts": {
-                "pretty_name": "Hosts",
-                "value": self.get_host_capacity(site_name),
-            },
-            "cpus": {"pretty_name": "CPUs", "value": self.get_cpu_capacity(site_name)},
-            "cores_available": {
-                "pretty_name": "Cores Available",
-                "value": self.get_core_available(site_name),
+                self.PRETTY_NAME: "PTP Capable",
+                self.VALUE: self.get_ptp_capable(site),
             },
-            "cores_capacity": {
-                "pretty_name": "Cores Capacity",
-                "value": self.get_core_capacity(site_name),
-            },
-            "cores_allocated": {
-                "pretty_name": "Cores Allocated",
-                "value": self.get_core_capacity(site_name)
-                - self.get_core_available(site_name),
-            },
-            "ram_available": {
-                "pretty_name": "RAM Available",
-                "value": self.get_ram_available(site_name),
-            },
-            "ram_capacity": {
-                "pretty_name": "RAM Capacity",
-                "value": self.get_ram_capacity(site_name),
-            },
-            "ram_allocated": {
-                "pretty_name": "RAM Allocated",
-                "value": self.get_ram_capacity(site_name)
-                - self.get_ram_available(site_name),
-            },
-            "disk_available": {
-                "pretty_name": "Disk Available",
-                "value": self.get_disk_available(site_name),
-            },
-            "disk_capacity": {
-                "pretty_name": "Disk Capacity",
-                "value": self.get_disk_capacity(site_name),
-            },
-            "disk_allocated": {
-                "pretty_name": "Disk Allocated",
-                "value": self.get_disk_capacity(site_name)
-                - self.get_disk_available(site_name),
-            },
-            "nic_basic_available": {
-                "pretty_name": "Basic NIC Available",
-                "value": self.get_component_available(
-                    site_name, "SharedNIC-ConnectX-6"
-                ),
-            },
-            "nic_basic_capacity": {
-                "pretty_name": "Basic NIC Capacity",
-                "value": self.get_component_capacity(site_name, "SharedNIC-ConnectX-6"),
-            },
-            "nic_basic_allocated": {
-                "pretty_name": "Basic NIC Allocated",
-                "value": self.get_component_capacity(site_name, "SharedNIC-ConnectX-6")
-                - self.get_component_available(site_name, "SharedNIC-ConnectX-6"),
-            },
-            "nic_connectx_6_available": {
-                "pretty_name": "ConnectX-6 Available",
-                "value": self.get_component_available(site_name, "SmartNIC-ConnectX-6"),
-            },
-            "nic_connectx_6_capacity": {
-                "pretty_name": "ConnectX-6 Capacity",
-                "value": self.get_component_capacity(site_name, "SmartNIC-ConnectX-6"),
-            },
-            "nic_connectx_6_allocated": {
-                "pretty_name": "ConnectX-6 Allocated",
-                "value": self.get_component_capacity(site_name, "SmartNIC-ConnectX-6")
-                - self.get_component_available(site_name, "SmartNIC-ConnectX-6"),
-            },
-            "nic_connectx_5_available": {
-                "pretty_name": "ConnectX-5 Available",
-                "value": self.get_component_available(site_name, "SmartNIC-ConnectX-5"),
-            },
-            "nic_connectx_5_capacity": {
-                "pretty_name": "ConnectX-5 Capacity",
-                "value": self.get_component_capacity(site_name, "SmartNIC-ConnectX-5"),
-            },
-            "nic_connectx_5_allocated": {
-                "pretty_name": "ConnectX-5 Allocated",
-                "value": self.get_component_capacity(site_name, "SmartNIC-ConnectX-5")
-                - self.get_component_available(site_name, "SmartNIC-ConnectX-5"),
-            },
-            "nvme_available": {
-                "pretty_name": "NVMe Available",
-                "value": self.get_component_available(site_name, "NVME-P4510"),
-            },
-            "nvme_capacity": {
-                "pretty_name": "NVMe Capacity",
-                "value": self.get_component_capacity(site_name, "NVME-P4510"),
-            },
-            "nvme_allocated": {
-                "pretty_name": "NVMe Allocated",
-                "value": self.get_component_capacity(site_name, "NVME-P4510")
-                - self.get_component_available(site_name, "NVME-P4510"),
-            },
-            "tesla_t4_available": {
-                "pretty_name": "Tesla T4 Available",
-                "value": self.get_component_available(site_name, "GPU-Tesla T4"),
-            },
-            "tesla_t4_capacity": {
-                "pretty_name": "Tesla T4 Capacity",
-                "value": self.get_component_capacity(site_name, "GPU-Tesla T4"),
-            },
-            "tesla_t4_allocated": {
-                "pretty_name": "Tesla T4 Allocated",
-                "value": self.get_component_capacity(site_name, "GPU-Tesla T4")
-                - self.get_component_available(site_name, "GPU-Tesla T4"),
-            },
-            "rtx6000_available": {
-                "pretty_name": "RTX6000 Available",
-                "value": self.get_component_available(site_name, "GPU-RTX6000"),
-            },
-            "rtx6000_capacity": {
-                "pretty_name": "RTX6000 Capacity",
-                "value": self.get_component_capacity(site_name, "GPU-RTX6000"),
-            },
-            "rtx6000_allocated": {
-                "pretty_name": "RTX6000 Allocated",
-                "value": self.get_component_capacity(site_name, "GPU-RTX6000")
-                - self.get_component_available(site_name, "GPU-RTX6000"),
-            },
-            "a30_available": {
-                "pretty_name": "A30 Available",
-                "value": self.get_component_available(site_name, "GPU-A30"),
-            },
-            "a30_capacity": {
-                "pretty_name": "A30 Capacity",
-                "value": self.get_component_capacity(site_name, "GPU-A30"),
-            },
-            "a30_allocated": {
-                "pretty_name": "A30 Allocated",
-                "value": self.get_component_capacity(site_name, "GPU-A30")
-                - self.get_component_available(site_name, "GPU-A30"),
-            },
-            "a40_available": {
-                "pretty_name": "A40 Available",
-                "value": self.get_component_available(site_name, "GPU-A40"),
-            },
-            "a40_capacity": {
-                "pretty_name": "A40 Capacity",
-                "value": self.get_component_capacity(site_name, "GPU-A40"),
-            },
-            "a40_allocated": {
-                "pretty_name": "A40 Allocated",
-                "value": self.get_component_capacity(site_name, "GPU-A40")
-                - self.get_component_available(site_name, "GPU-A40"),
-            },
-            "fpga_u280_available": {
-                "pretty_name": "FPGA U280 Available",
-                "value": self.get_component_available(site_name, "FPGA-Xilinx-U280"),
-            },
-            "fpga_u280_capacity": {
-                "pretty_name": "FPGA U280 Capacity",
-                "value": self.get_component_capacity(site_name, "FPGA-Xilinx-U280"),
-            },
-            "fpga_u280_allocated": {
-                "pretty_name": "FPGA U280 Allocated",
-                "value": self.get_component_capacity(site_name, "FPGA-Xilinx-U280")
-                - self.get_component_available(site_name, "FPGA-Xilinx-U280"),
+            self.HOSTS.lower(): {
+                self.PRETTY_NAME: self.HOSTS,
+                self.VALUE: self.get_host_capacity(site_name),
+            },
+            self.CPUS.lower(): {
+                self.PRETTY_NAME: self.CPUS,
+                self.VALUE: self.get_cpu_capacity(site_name),
             },
         }
 
+        for attribute, names in self.site_attribute_name_mappings.items():
+            capacity = site_info.get(attribute, {}).get(self.CAPACITY.lower(), 0)
+            allocated = site_info.get(attribute, {}).get(self.ALLOCATED.lower(), 0)
+            available = capacity - allocated
+
+            d[f"{names.get(self.NON_PRETTY_NAME)}_{self.AVAILABLE.lower()}"] = {
+                self.PRETTY_NAME: f"{names.get(self.PRETTY_NAME)} {self.AVAILABLE}",
+                self.VALUE: available,
+            }
+            d[f"{names.get(self.NON_PRETTY_NAME)}_{self.CAPACITY.lower()}"] = {
+                self.PRETTY_NAME: f"{names.get(self.PRETTY_NAME)} {self.CAPACITY}",
+                self.VALUE: capacity,
+            }
+            d[f"{names.get(self.NON_PRETTY_NAME)}_{self.ALLOCATED.lower()}"] = {
+                self.PRETTY_NAME: f"{names.get(self.PRETTY_NAME)} {self.ALLOCATED}",
+                self.VALUE: allocated,
+            }
+
+        return d
+
     def list_sites(
         self,
         output=None,
         fields=None,
         quiet=False,
         filter_function=None,
         pretty_names=True,
         latlon=True,
     ):
         table = []
         for site_name, site in self.topology.sites.items():
-            table.append(self.site_to_dict(site.get_sliver(), latlon=latlon))
+            site_dict = self.site_to_dict(site, latlon=latlon)
+            if site_dict.get("hosts"):
+                table.append(site_dict)
 
         if pretty_names:
             pretty_names_dict = self.site_pretty_names
         else:
             pretty_names_dict = {}
 
         return self.get_fablib_manager().list_table(
```

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/fablib/slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 import ipaddress
 import json
 import logging
 import sys
 import time
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timedelta, timezone
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Tuple
 
 import pandas as pd
 from fss_utils.sshkey import FABRICSSHKey
 from IPython.core.display_functions import display
 
 from fabrictestbed_extensions.fablib.constants import Constants
 from fabrictestbed_extensions.fablib.facility_port import FacilityPort
@@ -1028,15 +1028,15 @@
             name=name,
             interfaces=interfaces,
             type=type,
             user_data=user_data,
         )
 
     def add_facility_port(
-        self, name: str = None, site: str = None, vlan: str = None
+        self, name: str = None, site: str = None, vlan: Union[str, list] = None
     ) -> NetworkService:
         """
         Adds a new L2 facility port to this slice
 
         :param name: name of the facility port
         :type name: String
         :param site: site
@@ -1058,14 +1058,16 @@
         ram: int = 8,
         disk: int = 10,
         image: str = None,
         instance_type: str = None,
         host: str = None,
         user_data: dict = {},
         avoid: List[str] = [],
+        validate: bool = False,
+        raise_exception: bool = False,
     ) -> Node:
         """
         Creates a new node on this fablib slice.
 
         :param name: Name of the new node
         :type name: String
 
@@ -1101,18 +1103,26 @@
         :param user_data
         :type user_data: dict
 
         :param avoid: (Optional) A list of sites to avoid is allowing
             random site.
         :type avoid: List[String]
 
+        :param validate: Validate node can be allocated w.r.t available resources
+        :type validate: bool
+
+        :param raise_exception: Raise exception in case of Failure
+        :type raise_exception: bool
+
         :return: a new node
         :rtype: Node
         """
-        node = Node.new_node(slice=self, name=name, site=site, avoid=avoid)
+        node = Node.new_node(
+            slice=self, name=name, site=site, avoid=avoid, validate=validate, raise_exception=raise_exception
+        )
 
         node.init_fablib_data()
 
         user_data_working = node.get_user_data()
         for k, v in user_data.items():
             user_data_working[k] = v
         node.set_user_data(user_data_working)
@@ -1127,14 +1137,22 @@
 
         if host:
             node.set_host(host)
 
         self.nodes = None
         self.interfaces = None
 
+        if validate:
+            status, error = self.get_fablib_manager().validate_node(node=node)
+            if not status:
+                node.delete()
+                node = None
+                logging.warning(error)
+                if raise_exception:
+                    raise ValueError(error)
         return node
 
     def get_object_by_reservation(
         self, reservation_id: str
     ) -> Union[Node, NetworkService, Interface, None]:
         """
         Gets an object associated with this slice by its reservation ID.
@@ -1957,41 +1975,66 @@
         wait_interval: int = 20,
         progress: bool = True,
         wait_jupyter: str = "text",
         post_boot_config: bool = True,
         wait_ssh: bool = True,
         extra_ssh_keys: List[str] = None,
         lease_in_days: int = None,
+        validate: bool = False
     ) -> str:
         """
         Submits a slice request to FABRIC.
 
         Can be blocking or non-blocking.
 
         Blocking calls can, optionally,configure timeouts and intervals.
 
         Blocking calls can, optionally, print progress info.
 
 
         :param wait: indicator for whether to wait for the slice's resources to be active
+        :type wait: bool
+
         :param wait_timeout: how many seconds to wait on the slice resources
+        :type wait_timeout: int
+
         :param wait_interval: how often to check on the slice resources
+        :type wait_interval: int
+
         :param progress: indicator for whether to show progress while waiting
+        :type progress: bool
+
         :param wait_jupyter: Special wait for jupyter notebooks.
+        :type wait_jupyter: str
+
         :param post_boot_config:
+        :type post_boot_config: bool
+
         :param wait_ssh:
+        :type wait_ssh: bool
+
         :param extra_ssh_keys: Optional list of additional SSH public keys to be installed in the slivers of this slice
+        :type extra_ssh_keys: List[str]
+
         :param lease_in_days: Optional lease duration in days, by default the slice is active for 24 hours i.e 1 day,
                               only used for create.
+        :type lease_in_days: int
+
+        :param validate: Validate node can be allocated w.r.t available resources
+        :type validate: bool
+
         :return: slice_id
         """
 
         if not wait:
             progress = False
 
+        if validate:
+            self.validate()
+
         # Generate Slice Graph
         slice_graph = self.get_fim_topology().serialize()
 
         # Request slice from Orchestrator
         if self._is_modify():
             (
                 return_status,
@@ -2585,7 +2628,35 @@
         """
         Indicate if we should submit a modify request to orchestrator.
         """
         if self.get_state() is None:
             return False
         else:
             return True
+
+    def validate(self, raise_exception: bool = True) -> Tuple[bool, Dict[str, str]]:
+        """
+        Validate the slice w.r.t available resources before submission
+
+        :param raise_exception: raise exception if validation fails
+        :type raise_exception: bool
+
+        :return: Tuple indicating status for validation and dictionary of the errors corresponding to
+                 each requested node
+        :rtype: Tuple[bool, Dict[str, str]]
+        """
+        allocated = {}
+        errors = {}
+        nodes_to_remove = []
+        for n in self.get_nodes():
+            status, error = self.get_fablib_manager().validate_node(
+                node=n, allocated=allocated
+            )
+            if not status:
+                nodes_to_remove.append(n)
+                errors[n.get_name()] = error
+                logging.warning(f"{n.get_name()} - {error}")
+        for n in nodes_to_remove:
+            n.delete()
+        if raise_exception and len(errors):
+            raise Exception(f"Slice validation failed - {errors}!")
+        return len(errors) == 0, errors
```

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/utils/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/fabrictestbed_extensions/utils/utils.py` & `fabrictestbed-extensions-1.7.0b1/fabrictestbed_extensions/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/pyproject.toml` & `fabrictestbed-extensions-1.7.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "fabrictestbed-extensions"
-version = "1.6.4"
+version = "1.7.0b1"
 description = "FABRIC Python Client Library and CLI Extensions"
 authors = [
   { name = "Paul Ruth", email = "pruth@renci.org" },
   { name = "Komal Thareja", email = "kthare10@renci.org" },
 ]
 
 readme = { file = "README.md", content-type = "text/markdown" }
@@ -16,15 +16,15 @@
 requires-python = ">=3.9"
 dependencies = [
     "ipycytoscape",
     "ipywidgets",
     "ipyleaflet",
     "ipycytoscape",
     "tabulate",
-    "fabrictestbed==1.6.8",
+    "fabrictestbed==1.7.0b2",
     "paramiko",
     "jinja2>=3.0.0",
     "pandas",
     "numpy",
     "ipython>=8.12.0",
     "fabric_fss_utils>=1.5.1",
     "atomicwrites"
```

### Comparing `fabrictestbed_extensions-1.6.4/tests/benchmarks/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.7.0b1/tests/benchmarks/gpu_tesla_t4_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/benchmarks/link_benchmark.py` & `fabrictestbed-extensions-1.7.0b1/tests/benchmarks/link_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/benchmarks/local_network_benchmark.py` & `fabrictestbed-extensions-1.7.0b1/tests/benchmarks/local_network_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/benchmarks/network_benchmark_tests.py` & `fabrictestbed-extensions-1.7.0b1/tests/benchmarks/network_benchmark_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/benchmarks/nvme_benchmark.py` & `fabrictestbed-extensions-1.7.0b1/tests/benchmarks/nvme_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/integration/abc_test.py` & `fabrictestbed-extensions-1.7.0b1/tests/integration/abc_test.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/integration/component_tests.py` & `fabrictestbed-extensions-1.7.0b1/tests/integration/component_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/integration/test_L2_reconfig_post_reboot.py` & `fabrictestbed-extensions-1.7.0b1/tests/integration/test_L2_reconfig_post_reboot.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/integration/test_bastion_ssh.py` & `fabrictestbed-extensions-1.7.0b1/tests/integration/test_bastion_ssh.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/integration/test_fablib_node.py` & `fabrictestbed-extensions-1.7.0b1/tests/integration/test_fablib_node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/integration/test_fabnetv4_ext.py` & `fabrictestbed-extensions-1.7.0b1/tests/integration/test_fabnetv4_ext.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/integration/test_hello_fabric.py` & `fabrictestbed-extensions-1.7.0b1/tests/integration/test_hello_fabric.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/integration/test_list_resources.py` & `fabrictestbed-extensions-1.7.0b1/tests/integration/test_list_resources.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/integration/test_modify.py` & `fabrictestbed-extensions-1.7.0b1/tests/integration/test_modify.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tests/unit/test_basic.py` & `fabrictestbed-extensions-1.7.0b1/tests/unit/test_basic.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/tox.ini` & `fabrictestbed-extensions-1.7.0b1/tox.ini`

 * *Files identical despite different names*

### Comparing `fabrictestbed_extensions-1.6.4/PKG-INFO` & `fabrictestbed-extensions-1.7.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.6.4
+Version: 1.7.0b1
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: ipycytoscape
 Requires-Dist: ipywidgets
 Requires-Dist: ipyleaflet
 Requires-Dist: ipycytoscape
 Requires-Dist: tabulate
-Requires-Dist: fabrictestbed==1.6.8
+Requires-Dist: fabrictestbed==1.7.0b2
 Requires-Dist: paramiko
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: ipython>=8.12.0
 Requires-Dist: fabric_fss_utils>=1.5.1
 Requires-Dist: atomicwrites
```

