# Comparing `tmp/easyreflectometrylib-0.0.6.tar.gz` & `tmp/easyreflectometrylib-0.0.7.tar.gz`

## Comparing `easyreflectometrylib-0.0.6.tar` & `easyreflectometrylib-0.0.7.tar`

### file list

```diff
@@ -1,137 +1,148 @@
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/. codecov.yml
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.coveragerc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/CONTRIBUTING.rst
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/Makefile
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/release-drafter.yml
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/documentation-build.yml
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/ossar-analysis.yml
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/python-ci.yml
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/release-drafter-verify-pr-labels.yml
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/__init__.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/data.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/fitting.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/main.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/plot.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/__init__.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/calculator_base.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/factory.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/wrapper_base.py
--rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/bornagain/calculator.py
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/bornagain/wrapper.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refl1d/calculator.py
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refl1d/wrapper.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refnx/calculator.py
--rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refnx/wrapper.py
--rw-r--r--   0        0        0     7240 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/experiment/model.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/experiment/models.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/measurement/data.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/base_core.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/sample.py
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/base_assembly.py
--rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/gradient_layer.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/multilayer.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/repeating_multilayer.py
--rw-r--r--   0        0        0    13079 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/surfactant_layer.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/base_element_collection.py
--rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/layers/layer.py
--rw-r--r--   0        0        0    12302 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/layers/layer_area_per_molecule.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/layers/layer_collection.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_collection.py
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_density.py
--rw-r--r--   0        0        0     7781 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_mixture.py
--rw-r--r--   0        0        0     6458 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_solvated.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/special/calculations.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/special/parsing.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/Makefile
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/authors.rst
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/calculators.rst
--rwxr-xr-x   0        0        0     5930 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/contributing.rst
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/index.rst
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/installation.rst
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/make.bat
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/usage.rst
--rw-r--r--   0        0        0    21690 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/_static/favicon.ico
--rw-r--r--   0        0        0   395415 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/_static/logo.png
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/_static/logo.svg
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/api.rst
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/data.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/model.rst
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/sample.rst
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/assemblies/gradient_layer.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/assemblies/multilayer.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/assemblies/repeating_multilayer.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/assemblies/surfactant_layer.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/elements/layer.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/elements/layer_area_per_molecule.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/elements/material.rst
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/elements/material_density.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/elements/material_mixture.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/elements/material_solvated.rst
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/sample/assemblies_library.rst
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/sample/layer_library.rst
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/sample/material_library.rst
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/sample/sample.rst
--rw-r--r--   0        0        0    11193 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/material_solvated.ipynb
--rw-r--r--   0        0        0    16625 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/monolayer.ipynb
--rw-r--r--   0        0        0    15983 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/multi_contrast.ipynb
--rw-r--r--   0        0        0    10735 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/repeating.ipynb
--rw-r--r--   0        0        0    16765 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/simple_fitting.ipynb
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/d70d2o.ort
--rw-r--r--   0        0        0     9511 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/dspc.png
--rw-r--r--   0        0        0    28683 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/example.ort
--rw-r--r--   0        0        0   118247 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/monolayer.png
--rw-r--r--   0        0        0    17846 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/monolayer.svg
--rw-r--r--   0        0        0    16065 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/multiple.ort
--rw-r--r--   0        0        0    40781 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/polymer_film.png
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/polymer_film.svg
--rw-r--r--   0        0        0    41627 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/repeating.png
--rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/repeating.svg
--rw-r--r--   0        0        0    38132 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/repeating_layers.ort
--rw-r--r--   0        0        0     5554 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/test_data.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/test_fitting.py
--rw-r--r--   0        0        0    29131 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/_static/example.ort
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/_static/test_example1.ort
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/_static/test_example1.txt
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/_static/test_example2.ort
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/_static/test_example3.ort
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/_static/test_example4.ort
--rw-r--r--   0        0        0     6068 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/calculators/bornagain/test_bornagain_calculator.py
--rw-r--r--   0        0        0    10642 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/calculators/bornagain/test_bornagain_wrapper.py
--rw-r--r--   0        0        0     5839 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/calculators/refl1d/test_refl1d_calculator.py
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/calculators/refl1d/test_refl1d_wrapper.py
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/calculators/refnx/test_refnx_calculator.py
--rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/calculators/refnx/test_refnx_wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/experiment/__init__.py
--rw-r--r--   0        0        0    18616 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/experiment/test_model.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/test_sample.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/assemblies/test_base_assembly.py
--rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/assemblies/test_gradient_layer.py
--rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/assemblies/test_multilayer.py
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/assemblies/test_repeating_multilayer.py
--rw-r--r--   0        0        0     8883 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/assemblies/test_surfactant_layer.py
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/test_layer_collection.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/test_material_collection.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/layers/test_layer.py
--rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/layers/test_layer_area_per_molecule.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material_density.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material_mixture.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material_solvated.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/special/test_calculations.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/vscode-template/README.rst
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/vscode-template/settings.json
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.gitignore
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/AUTHORS.rst
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/LICENSE
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/README.rst
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/. codecov.yml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/.coveragerc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/Makefile
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/.github/release-drafter.yml
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/.github/workflows/documentation-build.yml
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/.github/workflows/ossar-analysis.yml
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/.github/workflows/python-ci.yml
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/.github/workflows/release-drafter-verify-pr-labels.yml
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/__init__.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/data.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/fitting.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/main.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/parameter_utils.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/plot.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/calculators/__init__.py
+-rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/calculators/calculator_base.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/calculators/factory.py
+-rw-r--r--   0        0        0     5930 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/calculators/wrapper_base.py
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/calculators/bornagain/calculator.py
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/calculators/bornagain/wrapper.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/calculators/refl1d/calculator.py
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/calculators/refl1d/wrapper.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/calculators/refnx/calculator.py
+-rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/calculators/refnx/wrapper.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/experiment/__init__.py
+-rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/experiment/model.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/experiment/model_collection.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/experiment/resolution_functions.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/measurement/data.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/__init__.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/base_core.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/base_element_collection.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/sample.py
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/assemblies/base_assembly.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/assemblies/gradient_layer.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/assemblies/multilayer.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/assemblies/repeating_multilayer.py
+-rw-r--r--   0        0        0    10432 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/assemblies/surfactant_layer.py
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/elements/layers/layer.py
+-rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/elements/layers/layer_area_per_molecule.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/elements/layers/layer_collection.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/elements/materials/material.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/elements/materials/material_collection.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/elements/materials/material_density.py
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/elements/materials/material_mixture.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/sample/elements/materials/material_solvated.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/special/calculations.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/EasyReflectometry/special/parsing.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/Makefile
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/make.bat
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/authors.rst
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/calculators.rst
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/conf.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/contributing.rst
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/index.rst
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/installation.rst
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/usage.rst
+-rw-r--r--   0        0        0    21690 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/_static/favicon.ico
+-rw-r--r--   0        0        0   395415 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/_static/logo.png
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/_static/logo.svg
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/api.rst
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/data.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/model.rst
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/sample.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/assemblies/gradient_layer.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/assemblies/multilayer.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/assemblies/repeating_multilayer.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/assemblies/surfactant_layer.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/elements/layer.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/elements/layer_area_per_molecule.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/elements/material.rst
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/elements/material_density.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/elements/material_mixture.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/api/elements/material_solvated.rst
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/experiment/experiment.rst
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/sample/assemblies_library.rst
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/sample/layer_library.rst
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/sample/material_library.rst
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/sample/sample.rst
+-rw-r--r--   0        0        0    11543 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/material_solvated.ipynb
+-rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/monolayer.ipynb
+-rw-r--r--   0        0        0    17175 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/multi_contrast.ipynb
+-rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/repeating.ipynb
+-rw-r--r--   0        0        0    13511 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/resolution_functions.ipynb
+-rw-r--r--   0        0        0    16809 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/simple_fitting.ipynb
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/tutorials.rst
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/d70d2o.ort
+-rw-r--r--   0        0        0     9511 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/dspc.png
+-rw-r--r--   0        0        0    28683 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/example.ort
+-rw-r--r--   0        0        0   118247 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/monolayer.png
+-rw-r--r--   0        0        0    17846 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/monolayer.svg
+-rw-r--r--   0        0        0    16065 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/multiple.ort
+-rw-r--r--   0        0        0    40781 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/polymer_film.png
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/polymer_film.svg
+-rw-r--r--   0        0        0    41627 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/repeating.png
+-rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/repeating.svg
+-rw-r--r--   0        0        0    38131 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/repeating_layers.ort
+-rw-r--r--   0        0        0   130253 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/two_layers.png
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/two_layers.svg
+-rw-r--r--   0        0        0    18877 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/resolution/mod_pointwise_two_layer_sample_dq-0.0.ort
+-rw-r--r--   0        0        0    18785 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/resolution/mod_pointwise_two_layer_sample_dq-1.0.ort
+-rw-r--r--   0        0        0    18877 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/docs/src/tutorials/_static/resolution/mod_pointwise_two_layer_sample_dq-10.0.ort
+-rw-r--r--   0        0        0     5554 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/test_data.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/test_fitting.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/test_parameter_utils.py
+-rw-r--r--   0        0        0    29131 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/_static/example.ort
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/_static/test_example1.ort
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/_static/test_example1.txt
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/_static/test_example2.ort
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/_static/test_example3.ort
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/_static/test_example4.ort
+-rw-r--r--   0        0        0     6068 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/calculators/bornagain/test_bornagain_calculator.py
+-rw-r--r--   0        0        0    10642 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/calculators/bornagain/test_bornagain_wrapper.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/calculators/refl1d/test_refl1d_calculator.py
+-rw-r--r--   0        0        0    15595 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/calculators/refl1d/test_refl1d_wrapper.py
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/calculators/refnx/test_refnx_calculator.py
+-rw-r--r--   0        0        0    29003 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/calculators/refnx/test_refnx_wrapper.py
+-rw-r--r--   0        0        0    21266 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/experiment/test_model.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/experiment/test_resolution_functions.py
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/test_sample.py
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/assemblies/test_base_assembly.py
+-rw-r--r--   0        0        0     7370 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/assemblies/test_gradient_layer.py
+-rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/assemblies/test_multilayer.py
+-rw-r--r--   0        0        0     8618 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/assemblies/test_repeating_multilayer.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/assemblies/test_surfactant_layer.py
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/elements/layers/test_layer.py
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/elements/layers/test_layer_area_per_molecule.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/elements/layers/test_layer_collection.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/elements/materials/test_material.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/elements/materials/test_material_collection.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/elements/materials/test_material_density.py
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/elements/materials/test_material_mixture.py
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/sample/elements/materials/test_material_solvated.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/tests/special/test_calculations.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/vscode-template/README.rst
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/vscode-template/settings.json
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/.gitignore
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/AUTHORS.rst
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/README.rst
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.7/PKG-INFO
```

### Comparing `easyreflectometrylib-0.0.6/CONTRIBUTING.rst` & `easyreflectometrylib-0.0.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/Makefile` & `easyreflectometrylib-0.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/.github/release-drafter.yml` & `easyreflectometrylib-0.0.7/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/.github/workflows/codeql-analysis.yml` & `easyreflectometrylib-0.0.7/.github/workflows/codeql-analysis.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: "CodeQL"
 
 on:
   push:
-    branches: [ main, pre-release, develop ]
+    branches: [ master, pre-release, develop ]
   pull_request:
     # The branches below must be a subset of the branches above
-    branches: [ main ]
+    branches: [ master ]
   schedule:
     - cron: '0 16 * * 5'
 
 jobs:
   analyze:
     name: Analyze
     runs-on: ubuntu-latest
@@ -40,15 +40,15 @@
     - name: Initialize CodeQL
       uses: github/codeql-action/init@v3
       with:
         languages: ${{ matrix.language }}
         # If you wish to specify custom queries, you can do so here or in a config file.
         # By default, queries listed here will override any specified in a config file. 
         # Prefix the list here with "+" to use these queries and those in the config file.
-        # queries: ./path/to/local/query, your-org/your-repo/queries@main
+        # queries: ./path/to/local/query, your-org/your-repo/queries@master
 
     # Autobuild attempts to build any compiled languages  (C/C++, C#, or Java).
     # If this step fails, then you should remove it and run the build manually (see below)
     - name: Autobuild
       uses: github/codeql-action/autobuild@v3
 
     # ℹ️ Command-line programs to run using the OS shell.
```

### Comparing `easyreflectometrylib-0.0.6/.github/workflows/documentation-build.yml` & `easyreflectometrylib-0.0.7/.github/workflows/documentation-build.yml`

 * *Files 10% similar despite different names*

```diff
@@ -29,20 +29,19 @@
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: 3.9
     - name: Install Pandoc, repo and dependencies
       run: |
         sudo apt install pandoc
-        pip install . '.[docs]'
+        pip install . '.[dev,docs]'
 
     - name: Build and Commit
       uses: sphinx-notes/pages@master
       with:
         install_requirements: true
         documentation_path: docs/src
     - name: Push changes
       uses: ad-m/github-push-action@master
       continue-on-error: true
       with:
-        github_token: ${{ secrets.CORE_TOKEN }}
         branch: gh-pages
```

### Comparing `easyreflectometrylib-0.0.6/.github/workflows/ossar-analysis.yml` & `easyreflectometrylib-0.0.7/.github/workflows/ossar-analysis.yml`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/.github/workflows/python-ci.yml` & `easyreflectometrylib-0.0.7/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/.github/workflows/python-package.yml` & `easyreflectometrylib-0.0.7/.github/workflows/python-package.yml`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 #
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Create Python Package
 
 on:
   push:
-    branches: [ main, pre-release ]
+    branches: [ master, pre-release ]
   pull_request:
-    branches: [ main, pre-release ]
+    branches: [ master, pre-release ]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ['3.9', '3.10', '3.11']
```

### Comparing `easyreflectometrylib-0.0.6/.github/workflows/python-publish.yml` & `easyreflectometrylib-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/.github/workflows/release-drafter-verify-pr-labels.yml` & `easyreflectometrylib-0.0.7/.github/workflows/release-drafter-verify-pr-labels.yml`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/.github/workflows/release-drafter.yml` & `easyreflectometrylib-0.0.7/.github/workflows/release-drafter.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,11 +12,11 @@
     tags:
       - 'v*'
 
 jobs:
   update_release_draft:
     runs-on: ubuntu-latest
     steps:
-      # Drafts your next Release notes as Pull Requests are merged into "main"
+      # Drafts your next Release notes as Pull Requests are merged into "master"
       - uses: release-drafter/release-drafter@v6
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/data.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/data.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/fitting.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/fitting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = 'github.com/arm61'
 
 import numpy as np
 import scipp as sc
 from easyCore.Fitting.Fitting import MultiFitter as easyFitter
 
-from EasyReflectometry.experiment.model import Model
+from EasyReflectometry.experiment import Model
 
 
 class Fitter:
     def __init__(self, *args: Model):
         r"""A convinence class for the :py:class:`easyCore.Fitting.Fitting`
         which will populate the :py:class:`sc.DataGroup` appropriately
         after the fitting is performed.
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/plot.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/plot.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/__init__.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/calculators/__init__.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/calculator_base.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/calculators/calculator_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 from abc import ABCMeta
+from typing import Callable
 
 import numpy as np
 from easyCore.Objects.core import ComponentSerializer
 from easyCore.Objects.Inferface import ItemContainer
 
-from EasyReflectometry.experiment.model import Model
+from EasyReflectometry.experiment import Model
 from EasyReflectometry.sample import BaseAssembly
 from EasyReflectometry.sample import Layer
 from EasyReflectometry.sample import Material
 from EasyReflectometry.sample import MaterialMixture
 from EasyReflectometry.sample import Multilayer
 
 from .wrapper_base import WrapperBase
@@ -169,7 +170,10 @@
         """
         Return the scattering length density profile.
 
         :param model_id: The model id
         :return: z and sld(z)
         """
         return self._wrapper.sld_profile(model_id)
+
+    def set_resolution_function(self, resolution_function: Callable[[np.array], np.array]) -> None:
+        return self._wrapper.set_resolution_function(resolution_function)
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/wrapper_base.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/calculators/wrapper_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from abc import abstractmethod
+from typing import Callable
 
 import numpy as np
 
+from EasyReflectometry.experiment import percentage_fhwm_resolution_function
+
+DEFAULT_RESOLUTION_FWHM_PERCENTAGE = 5.0
+
 
 class WrapperBase:
     def __init__(self):
         """Constructor."""
         self.storage = {
             'material': {},
             'layer': {},
             'item': {},
             'model': {},
         }
+        self._resolution_function = percentage_fhwm_resolution_function(DEFAULT_RESOLUTION_FWHM_PERCENTAGE)
 
     def reset_storage(self):
         """Reset the storage area to blank."""
         self.storage = {
             'material': {},
             'layer': {},
             'item': {},
@@ -115,19 +121,20 @@
 
         :param item_name: The item name
         :param model_name: Name of the model
         """
         ...
 
     @abstractmethod
-    def calculate(self, x_array: np.ndarray, model_name: str) -> np.ndarray:
-        """For a given x calculate the corresponding y.
+    def calculate(self, q_array: np.ndarray, model_name: str) -> np.ndarray:
+        """For a given q array calculate the corresponding reflectivity.
 
-        :param x_array: array of data points to be calculated
-        :param model_name: Name for the model
+        :param q_array: array of data points to be calculated
+        :param model_name: the model name
+        :return: reflectivity calculated at q
         """
         ...
 
     @abstractmethod
     def sld_profile(self, model_name: str) -> tuple[np.ndarray, np.ndarray]:
         """Return the scattering length density profile.
 
@@ -194,7 +201,14 @@
         :param name: The item name
         :param key: The given value keys
         :return: The desired value
         """
         item = self.storage['item'][name]
         item = getattr(item, key)
         return getattr(item, 'value')
+
+    def set_resolution_function(self, resolution_function: Callable[[np.array], np.array]) -> None:
+        """Set the resolution function for the calculator.
+
+        :param resolution_function: The resolution function
+        """
+        self._resolution_function = resolution_function
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/bornagain/calculator.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/calculators/bornagain/calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __author__ = 'github.com/arm61'
 
 import numpy as np
 from easyCore.Objects.Inferface import ItemContainer
 
-from EasyReflectometry.experiment.model import Model
+from EasyReflectometry.experiment import Model
 from EasyReflectometry.sample import Layer
 from EasyReflectometry.sample import Material
 from EasyReflectometry.sample import MaterialMixture
 from EasyReflectometry.sample import Multilayer
 
 from ..calculator_base import CalculatorBase
 from .wrapper import BornAgainWrapper
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/bornagain/wrapper.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/calculators/bornagain/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = 'github.com/arm61'
 
 import bornagain as ba
-from easyCore import np
+import numpy as np
 from scipy.stats import norm
 
 from ..wrapper_base import WrapperBase
 
 """
 THIS CODE IS NOT FUNCTIONAL
 PLEASE CONSULT ONE OF THE OTHER WRAPPES FOR A FUNCTIONAL EXAMPLE
@@ -241,31 +241,31 @@
         :type item_name: int
         """
         item_idx = self.storage['model_items'].index(item_name)
         del self.storage['model_items'][item_idx]
         del self.storage['item_repeats'][item_name]
         del self.storage['item'][item_name]
 
-    def calculate(self, x_array: np.ndarray) -> np.ndarray:
-        """
-        For a given x calculate the corresponding y.
-
-        :param x_array: array of data points to be calculated
-        :type x_array: np.ndarray
-        :return: points calculated at `x`
-        :rtype: np.ndarray
+    # To conform the base class the signature should be
+    # def calculate(self, q_array: np.ndarray, model_name: str) -> np.ndarray:
+    def calculate(self, q_array: np.ndarray) -> np.ndarray:
+        """For a given q array calculate the corresponding reflectivity.
+
+        :param q_array: array of data points to be calculated
+        :param model_name: the model name
+        :return: reflectivity calculated at q
         """
         # 3.5 sigma to sync with refnx
         n_sig = 3.5
         n_samples = 21
         distr = ba.RangedDistributionGaussian(n_samples, n_sig)
 
-        scan = ba.QSpecScan(x_array / ba.angstrom)
+        scan = ba.QSpecScan(q_array / ba.angstrom)
         scan.setAbsoluteQResolution(
-            distr, x_array / ba.angstrom * (self.storage['model_parameters']['resolution'] * 0.5 / 100)
+            distr, q_array / ba.angstrom * (self.storage['model_parameters']['resolution'] * 0.5 / 100)
         )
 
         simulation = ba.SpecularSimulation()
         simulation.setScan(scan)
 
         total_model = ba.Multilayer()
         for i in self.storage['model_items']:
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refl1d/calculator.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/calculators/refl1d/calculator.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,13 +24,12 @@
     _item_link = {
         'repetitions': 'repeat',
     }
 
     _model_link = {
         'scale': 'scale',
         'background': 'bkg',
-        'resolution': 'dq',
     }
 
     def __init__(self):
         super().__init__()
         self._wrapper = Refl1dWrapper()
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refl1d/wrapper.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/calculators/refnx/wrapper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,203 +1,166 @@
 __author__ = 'github.com/arm61'
 
 from typing import Tuple
 
-from easyCore import np
-from refl1d import model
-from refl1d import names
+import numpy as np
+from refnx import reflect
+
+from EasyReflectometry.experiment.resolution_functions import is_percentage_fhwm_resolution_function
 
 from ..wrapper_base import WrapperBase
 
 
-class Refl1dWrapper(WrapperBase):
+class RefnxWrapper(WrapperBase):
     def create_material(self, name: str):
         """
         Create a material using SLD.
 
         :param name: The name of the material
         """
-        self.storage['material'][name] = names.SLD(str(name))
+        self.storage['material'][name] = reflect.SLD(0, name=name)
 
     def create_layer(self, name: str):
         """
         Create a layer using Slab.
 
         :param name: The name of the layer
         """
-        self.storage['layer'][name] = model.Slab(name=str(name))
+        self.storage['layer'][name] = reflect.Slab(0, 0, 0, name=name)
 
     def create_item(self, name: str):
         """
-        Create an item using Repeat.
+        Create an item using Stack.
 
         :param name: The name of the item
         """
-        self.storage['item'][name] = model.Repeat(
-            model.Stack(model.Slab(names.SLD(), thickness=0, interface=0)), name=str(name)
-        )
-        del self.storage['item'][name].stack[0]
-
-    def update_item(self, name: str, **kwargs):
-        """
-        Update a layer.
-
-        :param name: The item name
-        """
-        item = self.storage['item'][name]
-        for key in kwargs.keys():
-            ii = getattr(item, key)
-            setattr(ii, 'value', kwargs[key])
-
-    def get_item_value(self, name: str, key: str) -> float:
-        """
-        A function to get a given item value
-
-        :param name: The item name
-        :param key: The given value keys
-        :return: The desired value
-        """
-        item = self.storage['item'][name]
-        item = getattr(item, key)
-        return getattr(item, 'value')
+        self.storage['item'][name] = reflect.Stack(name=name)
 
     def create_model(self, name: str):
         """
         Create a model for analysis
 
         :param name: Name for the model
         """
-        self.storage['model'][name] = {'scale': 1, 'bkg': 0, 'dq': 0, 'items': []}
+        self.storage['model'][name] = reflect.ReflectModel(reflect.Structure())
 
     def update_model(self, name: str, **kwargs):
         """
         Update the non-structural parameters of the model
 
-        :param name: Name of the model
+        :param name: Name for the model
         """
         model = self.storage['model'][name]
         for key in kwargs.keys():
-            model[key] = kwargs[key]
+            item = getattr(model, key)
+            setattr(item, 'value', kwargs[key])
 
     def get_model_value(self, name: str, key: str) -> float:
         """
         A function to get a given model value
 
-        :param name: Name of the model
+        :param name: Name for the model
         :param key: The given value keys
         :return: The desired value
         """
         model = self.storage['model'][name]
-        return model[key]
+        item = getattr(model, key)
+        return getattr(item, 'value')
 
     def assign_material_to_layer(self, material_name: str, layer_name: str):
         """
         Assign a material to a layer.
 
         :param material_name: The material name
         :param layer_name: The layer name
         """
-        self.storage['layer'][layer_name].material = self.storage['material'][material_name]
+        self.storage['layer'][layer_name].sld = self.storage['material'][material_name]
 
     def add_layer_to_item(self, layer_name: str, item_name: str):
         """
         Create a layer from the material of the same name, in a given item.
 
         :param layer_name: The layer name
         :param item_name: The item name
         """
         item = self.storage['item'][item_name]
-        item.stack.add(self.storage['layer'][layer_name])
+        item.append(self.storage['layer'][layer_name])
 
     def add_item(self, item_name: str, model_name: str):
         """
         Add an item to the model.
 
         :param item_name: items to add to model
-        :param model_name: name for the model
+        :param model_name: Name for the model
         """
-        self.storage['model'][model_name]['items'].append(self.storage['item'][item_name])
+        self.storage['model'][model_name].structure.components.append(self.storage['item'][item_name])
 
     def remove_layer_from_item(self, layer_name: str, item_name: str):
         """
         Remove a layer in a given item.
 
         :param layer_name: The layer name
         :param item_name: The item name
         """
-        layer_idx = list(self.storage['item'][item_name].stack).index(self.storage['layer'][layer_name])
-        del self.storage['item'][item_name].stack[layer_idx]
+        layer_idx = self.storage['item'][item_name].components.index(self.storage['layer'][layer_name])
+        del self.storage['item'][item_name].components[layer_idx]
 
     def remove_item(self, item_name: str, model_name: str):
         """
         Remove a given item.
 
         :param item_name: The item name
-        :param model_name: The model name
+        :param model_name: Name of the model
         """
-        item_idx = self.storage['model'][model_name]['items'].index(self.storage['item'][item_name])
-        del self.storage['model'][model_name]['items'][item_idx]
+        item_idx = self.storage['model'][model_name].structure.components.index(self.storage['item'][item_name])
+        del self.storage['model'][model_name].structure.components[item_idx]
         del self.storage['item'][item_name]
 
-    def calculate(self, x_array: np.ndarray, model_name: str) -> np.ndarray:
-        """
-        For a given x calculate the corresponding y.
+    def calculate(self, q_array: np.ndarray, model_name: str) -> np.ndarray:
+        """For a given q array calculate the corresponding reflectivity.
 
-        :param x_array: array of data points to be calculated
+        :param q_array: array of data points to be calculated
         :param model_name: the model name
-        :return: points calculated at `x`
+        :return: reflectivity calculated at q
         """
-        structure = model.Stack()
-        for i in self.storage['model'][model_name]['items'][::-1]:
-            if i.repeat.value == 1:
-                for j in range(len(i.stack))[::-1]:
-                    structure |= i.stack[j]
-            else:
-                stack = model.Stack()
-                for j in range(len(i.stack))[::-1]:
-                    stack |= i.stack[j]
-                structure |= model.Repeat(stack, repeat=i.repeat.value)
-
-        argmin = np.argmin(x_array)
-        argmax = np.argmax(x_array)
-        dq_vector = x_array * self.storage['model'][model_name]['dq'] / 100 / (2 * np.sqrt(2 * np.log(2)))
-
-        q = names.QProbe(
-            x_array,
-            dq_vector,
-            intensity=self.storage['model'][model_name]['scale'],
-            background=self.storage['model'][model_name]['bkg'],
-        )
-        q.calc_Qo = np.linspace(
-            x_array[argmin] - 3.5 * dq_vector[argmin],
-            x_array[argmax] + 3.5 * dq_vector[argmax],
-            21 * len(x_array),
+        structure = _remove_unecessary_stacks(self.storage['model'][model_name].structure)
+        model = reflect.ReflectModel(
+            structure,
+            scale=self.storage['model'][model_name].scale.value,
+            bkg=self.storage['model'][model_name].bkg.value,
+            dq_type='pointwise',
         )
-        R = names.Experiment(probe=q, sample=structure).reflectivity()[1]
-        return R
+
+        dq_vector = self._resolution_function(q_array)
+        if is_percentage_fhwm_resolution_function(self._resolution_function):
+            # FWHM Percentage resolution is constant given as
+            # For a constant resolution percentage refnx supports to pass a scalar value rather than a vector
+            dq_vector = dq_vector[0]
+
+        return model(x=q_array, x_err=dq_vector)
 
     def sld_profile(self, model_name: str) -> Tuple[np.ndarray, np.ndarray]:
         """
         Return the scattering length density profile.
 
-        :param model_name: the model name
+        :param model_name: Name for the model
         :return: z and sld(z)
         """
-        structure = model.Stack()
-        for i in self.storage['model'][model_name]['items'][::-1]:
-            if i.repeat.value == 1:
-                for j in range(len(i.stack))[::-1]:
-                    structure |= i.stack[j]
-            else:
-                stack = model.Stack()
-                for j in range(len(i.stack))[::-1]:
-                    stack |= i.stack[j]
-                structure |= model.Repeat(stack, repeat=i.repeat.value)
-
-        q = names.QProbe(
-            np.linspace(0.001, 0.3, 10),
-            np.linspace(0.001, 0.3, 10),
-            intensity=self.storage['model'][model_name]['scale'],
-            background=self.storage['model'][model_name]['bkg'],
-        )
-        z, sld, _ = names.Experiment(probe=q, sample=structure).smooth_profile()
-        return z, sld[::-1]
+        return _remove_unecessary_stacks(self.storage['model'][model_name].structure).sld_profile()
+
+
+def _remove_unecessary_stacks(current_structure: reflect.Structure) -> reflect.Structure:
+    """
+    Removed unnecessary reflect.Stack objects from the structure.
+
+    :param current_structure: The current structure
+    :return: The structre without the unnecessary Stacks
+    :rtype: reflect.structure
+    """
+    structure = []
+    for i in current_structure.components:
+        if i.repeats.value == 1:
+            for j in i.components:
+                structure.append(j)
+        else:
+            structure.append(i)
+    return reflect.Structure(structure)
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refnx/calculator.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/calculators/refnx/calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,13 +24,12 @@
     _item_link = {
         'repetitions': 'repeats',
     }
 
     _model_link = {
         'scale': 'scale',
         'background': 'bkg',
-        'resolution': 'dq',
     }
 
     def __init__(self):
         super().__init__()
         self._wrapper = RefnxWrapper()
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/sample/__init__.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/sample/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 from .assemblies.repeating_multilayer import RepeatingMultilayer
 from .assemblies.surfactant_layer import SurfactantLayer
 from .elements.layers.layer import Layer
 from .elements.layers.layer_area_per_molecule import LayerAreaPerMolecule
 from .elements.layers.layer_collection import LayerCollection
 from .elements.materials.material import Material
 from .elements.materials.material_collection import MaterialCollection
+from .elements.materials.material_density import MaterialDensity
 from .elements.materials.material_mixture import MaterialMixture
 from .elements.materials.material_solvated import MaterialSolvated
 from .sample import Sample
 
 __all__ = (
     BaseAssembly,
     GradientLayer,
-    Multilayer,
-    RepeatingMultilayer,
-    SurfactantLayer,
     Layer,
     LayerAreaPerMolecule,
     LayerCollection,
     Material,
-    MaterialMixture,
     MaterialCollection,
+    MaterialDensity,
+    MaterialMixture,
     MaterialSolvated,
+    Multilayer,
+    RepeatingMultilayer,
     Sample,
+    SurfactantLayer,
 )
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/sample/base_core.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/sample/base_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import abstractmethod
-from typing import Any
 
 import yaml
 from easyCore.Objects.ObjectClasses import BaseObj
 
 
 class BaseCore(BaseObj):
     def __init__(
@@ -14,17 +13,14 @@
     ):
         super().__init__(name=name, **kwargs)
 
         # Updates interface using property in base object
         self.interface = interface
 
     @abstractmethod
-    def default(cls, interface=None) -> Any: ...
-
-    @abstractmethod
     def _dict_repr(self) -> dict[str, str]: ...
 
     @property
     def uid(self) -> int:
         """
         :return: UID from the borg map
         """
@@ -37,15 +33,15 @@
         :return: a string representation of the layer
         :rtype: str
         """
         return yaml.dump(self._dict_repr, sort_keys=False)
 
     # For classes with special serialization needs one must adopt the dict produced by super
     # def as_dict(self, skip: list = None) -> dict:
-    #    """Should produce a cleaned dict that matches the paramters in __init__
+    #    """Should produce a cleaned dict that matches the parameters in __init__
     #
     #    :param skip: List of keys to skip, defaults to `None`.
     #    """
     #    if skip is None:
     #        skip = []
     #    this_dict = super().as_dict(skip=skip)
     #    ...
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/sample/sample.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/sample/sample.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,53 @@
 from __future__ import annotations
 
 __author__ = 'github.com/arm61'
 
+from typing import Union
+
 import yaml
 from easyCore.Objects.Groups import BaseCollection
 
 from .assemblies.base_assembly import BaseAssembly
 from .assemblies.multilayer import Multilayer
 from .elements.layers.layer import Layer
 
+NR_DEFAULT_LAYERS = 2
+
 
 class Sample(BaseCollection):
     """Collection of assemblies that represent the sample for which experimental measurements exist."""
 
     def __init__(
         self,
-        *args: list[Layer | BaseAssembly],
+        *list_layer_like: list[Union[Layer, BaseAssembly]],
         name: str = 'EasySample',
         interface=None,
         **kwargs,
     ):
         """Constructor.
 
         :param args: The assemblies in the sample.
         :param name: Name of the sample, defaults to 'EasySample'.
-        :param interface: Calculator interface, defaults to :py:attr:`None`.
+        :param interface: Calculator interface, defaults to `None`.
         """
         new_items = []
-        for layer_like in args:
+        if not list_layer_like:
+            list_layer_like = [Multilayer(interface=interface) for _ in range(NR_DEFAULT_LAYERS)]
+
+        for layer_like in list_layer_like:
             if issubclass(type(layer_like), Layer):
-                new_items.append(Multilayer.from_pars(layer_like, name=layer_like.name))
+                new_items.append(Multilayer(layer_like, name=layer_like.name))
             elif issubclass(type(layer_like), BaseAssembly):
                 new_items.append(layer_like)
             else:
                 raise ValueError('The items must be either a Layer or an Assembly.')
         super().__init__(name, *new_items, **kwargs)
         self.interface = interface
 
-    # Class methods for instance creation
-    @classmethod
-    def default(cls, interface=None) -> Sample:
-        """
-        Default instance of the reflectometry sample.
-
-        :param interface: Calculator interface, defaults to :py:attr:`None`.
-        """
-        item1 = Multilayer.default()
-        item2 = Multilayer.default()
-        return cls(item1, item2, interface=interface)
-
-    @classmethod
-    def from_pars(
-        cls,
-        *args: list[Layer | BaseAssembly],
-        name: str = 'EasyStructure',
-        interface=None,
-    ) -> Sample:
-        """Constructor of a reflectometry sample where the parameters are known.
-
-        :param args: The assemblies in the sample
-        :param name: Name of the sample, defaults to 'EasySample'.
-        :param interface: Calculator interface, defaults to :py:attr:`None`.
-        """
-        return cls(*args, name=name, interface=interface)
-
     @property
     def uid(self) -> int:
         """The UID from the borg map."""
         return self._borg.map.convert_id_to_key(self)
 
     # Representation
     @property
@@ -77,17 +57,38 @@
 
     def __repr__(self) -> str:
         """String representation of the sample."""
         return yaml.dump(self._dict_repr, sort_keys=False)
 
     def as_dict(self, skip: list = None) -> dict:
         """Produces a cleaned dict using a custom as_dict method to skip necessary things.
-        The resulting dict matches the paramters in __init__
+        The resulting dict matches the parameters in __init__
 
         :param skip: List of keys to skip, defaults to `None`.
         """
         if skip is None:
             skip = []
         this_dict = super().as_dict(skip=skip)
         for i, layer in enumerate(self.data):
             this_dict['data'][i] = layer.as_dict()
         return this_dict
+
+    @classmethod
+    def from_dict(cls, data: dict) -> Sample:
+        """
+        Create a Sample from a dictionary.
+
+        :param data: dictionary of the Sample
+        :return: Sample
+        """
+        sample = super().from_dict(data)
+
+        # Remove the default multilayers
+        for i in range(NR_DEFAULT_LAYERS):
+            sample.__delitem__(0)
+
+        # Ensure that the data is also converted
+        # TODO Should probably be handled in easyscience
+        for i in range(len(sample.data)):
+            sample[i] = sample[i].__class__.from_dict(data['data'][i])
+
+        return sample
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/base_assembly.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/sample/assemblies/base_assembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         name: str,
         type: str,
         interface,
         **layers: LayerCollection,
     ):
         super().__init__(name=name, interface=interface, **layers)
 
-        # Type is needed when fitting in EasyCore
+        # Type is needed when fitting in easyscience
         self._type = type
         self._roughness_constraints_setup = False
         self._thickness_constraints_setup = False
 
     @property
     def type(self) -> str:
         """Get type of the assembly.
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/gradient_layer.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/sample/assemblies/gradient_layer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations
+from typing import Optional
 
 from numpy import arange
 
 from ..elements.layers.layer import Layer
 from ..elements.layers.layer_collection import LayerCollection
 from ..elements.materials.material import Material
 from .base_assembly import BaseAssembly
@@ -12,34 +12,41 @@
     """A set of discrete gradient layers changing from the front to the back material.
     The front layer is where the neutron beam starts in, it has an index of 0.
 
     """
 
     def __init__(
         self,
-        front_material: Material,
-        back_material: Material,
-        thickness: float,
-        roughness: float,
+        front_material: Optional[Material] = None,
+        back_material: Optional[Material] = None,
+        thickness: Optional[float] = 2.0,
+        roughness: Optional[float] = 0.2,
         discretisation_elements: int = 10,
         name: str = 'EasyGradienLayer',
         interface=None,
-    ) -> GradientLayer:
+    ):
         """Constructor.
 
         :param front_material: Material of front of the layer
         :param back_material: Material of back of the layer
         :param thickness: Thicknkess of the layer
         :param roughness: Roughness of the layer
         :param discretisation_elements: Number of discrete layers
         :param name: Name for gradient layer, defaults to 'EasyGradienLayer'.
         :param interface: Calculator interface, defaults to `None`.
         """
+
+        if front_material is None:
+            front_material = Material(0.0, 0.0, 'Air')
         self._front_material = front_material
+
+        if back_material is None:
+            back_material = Material(6.36, 0.0, 'D2O')
         self._back_material = back_material
+
         if discretisation_elements < 2:
             raise ValueError('Discretisation elements must be greater than 2.')
         self._discretisation_elements = discretisation_elements
 
         gradient_layers = _prepare_gradient_layers(
             front_material=front_material,
             back_material=back_material,
@@ -59,67 +66,14 @@
         self._setup_roughness_constraints()
         self._enable_roughness_constraints()
 
         # Set the thickness and roughness properties
         self.thickness = thickness
         self.roughness = roughness
 
-    # Class methods for instance creation
-    @classmethod
-    def default(cls, name: str = 'EasyGradientLayer', interface=None) -> GradientLayer:
-        """Default instance  for a gradient layer object. The default is air to deuterium.
-
-        :param name: Name for gradient layer, defaults to 'EasyGradienLayer'.
-        :param interface: Calculator interface, defaults to `None`.
-        """
-        front_material = Material.from_pars(0.0, 0.0, 'Air')
-        back_material = Material.from_pars(6.36, 0.0, 'D2O')
-
-        return cls(
-            front_material=front_material,
-            back_material=back_material,
-            thickness=2.0,
-            roughness=0.2,
-            discretisation_elements=10,
-            name=name,
-            interface=interface,
-        )
-
-    @classmethod
-    def from_pars(
-        cls,
-        front_material: Material,
-        back_material: Material,
-        thickness: float,
-        roughness: float,
-        discretisation_elements: int,
-        name: str = 'EasyGradientLayer',
-        interface=None,
-    ) -> GradientLayer:
-        """Instance for the gradient layer where the parameters are known,
-        `front` is facing the neutron beam.
-
-        :param front_material: Material of front of the layer
-        :param back_material: Material of back of the layer
-        :param thickness: Thicknkess of the layer
-        :param roughness: Roughness of the layer
-        :param discretisation_elements: Number of dicrete layers
-        :param name: Name for gradient layer
-        """
-
-        return cls(
-            front_material=front_material,
-            back_material=back_material,
-            thickness=thickness,
-            roughness=roughness,
-            discretisation_elements=discretisation_elements,
-            name=name,
-            interface=interface,
-        )
-
     @property
     def thickness(self) -> float:
         """Get the thickness of the gradient layer in Angstrom."""
         return self.front_layer.thickness.raw_value * self._discretisation_elements
 
     @thickness.setter
     def thickness(self, thickness: float) -> None:
@@ -150,15 +104,15 @@
             'discretisation_elements': self._discretisation_elements,
             'back_layer': self.back_layer._dict_repr,
             'front_layer': self.front_layer._dict_repr,
         }
 
     def as_dict(self, skip: list = None) -> dict:
         """Produces a cleaned dict using a custom as_dict method to skip necessary things.
-        The resulting dict matches the paramters in __init__
+        The resulting dict matches the parameters in __init__
 
         :param skip: List of keys to skip, defaults to `None`.
         """
         this_dict = super().as_dict(skip=skip)
         # Determined in __init__
         del this_dict['layers']
         return this_dict
@@ -192,16 +146,17 @@
     gradient_isld = _linear_gradient(
         front_value=front_material.isld.raw_value,
         back_value=back_material.isld.raw_value,
         discretisation_elements=discretisation_elements,
     )
     gradient_layers = []
     for i in range(discretisation_elements):
-        layer = Layer.from_pars(
-            material=Material.from_pars(gradient_sld[i], gradient_isld[i]),
+        material_i = Material(gradient_sld[i], gradient_isld[i], interface=interface)
+        layer = Layer(
+            material=material_i,
             thickness=0.0,
             roughness=0.0,
             name=str(i),
             interface=interface,
         )
         gradient_layers.append(layer)
     return LayerCollection(gradient_layers)
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/multilayer.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/sample/assemblies/multilayer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import annotations
 
+from typing import Union
+
 from ..elements.layers.layer import Layer
+from ..elements.layers.layer_collection import SIZE_DEFAULT_COLLECTION
 from ..elements.layers.layer_collection import LayerCollection
 from .base_assembly import BaseAssembly
 
 
 class Multilayer(BaseAssembly):
     """A multi layer is build from a single or a list of `Layer` or `LayerCollection`.
     The multi layer will arrange the layers as slabs, allowing the reflectometry to be determined from them.
@@ -14,61 +17,34 @@
     `multilayer documentation`_
 
     .. _`multilayer documentation`: ../sample/assemblies_library.html#multilayer
     """
 
     def __init__(
         self,
-        layers: LayerCollection | Layer | list[Layer],
+        layers: Union[Layer, list[Layer], LayerCollection, None] = None,
         name: str = 'EasyMultilayer',
         interface=None,
         type: str = 'Multi-layer',
     ):
         """Constructor.
 
         :param layers: The layers that make up the multi-layer.
         :param name: Name for multi layer, defaults to 'EasyMultilayer'.
         :param interface: Calculator interface, defaults to `None`.
         :param type: Type of the constructed instance, defaults to 'Multi-layer'
         """
-        if isinstance(layers, Layer):
+        if layers is None:
+            layers = LayerCollection()
+        elif isinstance(layers, Layer):
             layers = LayerCollection(layers, name=layers.name)
         elif isinstance(layers, list):
             layers = LayerCollection(*layers, name='/'.join([layer.name for layer in layers]))
         super().__init__(name, layers=layers, type=type, interface=interface)
 
-    # Class methods for instance creation
-    @classmethod
-    def default(cls, interface=None) -> Multilayer:
-        """Default instance of a multi-layer.
-
-        :param interface: Calculator interface, defaults to `None`.
-        """
-        layers = LayerCollection.default()
-        return cls(layers, interface=interface)
-
-    @classmethod
-    def from_pars(
-        cls,
-        layers: LayerCollection,
-        name: str = 'EasyMultilayer',
-        interface=None,
-    ) -> Multilayer:
-        """Instance of a multi-layer where the parameters are known.
-
-        :param layers: The layers in the multi-layer.
-        :param name: Name of the layer, defaults to 'EasyMultilayer'.
-        :param interface: Calculator interface, defaults to `None`.
-        """
-        return cls(
-            layers=layers,
-            name=name,
-            interface=interface,
-        )
-
     def add_layer(self, *layers: tuple[Layer]) -> None:
         """Add a layer to the multi layer.
 
         :param layers: Layers to add to the multi layer.
         """
         for arg in layers:
             if issubclass(arg.__class__, Layer):
@@ -79,15 +55,15 @@
     def duplicate_layer(self, idx: int) -> None:
         """Duplicate a given layer.
 
         :param idx: index of layer to duplicate.
         :type idx: int
         """
         to_duplicate = self.layers[idx]
-        duplicate_layer = Layer.from_pars(
+        duplicate_layer = Layer(
             material=to_duplicate.material,
             thickness=to_duplicate.thickness.raw_value,
             roughness=to_duplicate.roughness.raw_value,
             name=to_duplicate.name + ' duplicate',
         )
         self.add_layer(duplicate_layer)
 
@@ -103,7 +79,21 @@
     # Representation
     @property
     def _dict_repr(self) -> dict:
         """A simplified dict representation."""
         if len(self.layers) == 1:
             return self.front_layer._dict_repr
         return {self.name: self.layers._dict_repr}
+
+    @classmethod
+    def from_dict(cls, data: dict) -> Multilayer:
+        """
+        Create a Multilayer from a dictionary.
+
+        :param data: dictionary of the Multilayer
+        :return: Multilayer
+        """
+        multilayer = super().from_dict(data)
+        # Remove the default materials
+        for i in range(SIZE_DEFAULT_COLLECTION):
+            del multilayer.layers[0]
+        return multilayer
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/repeating_multilayer.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/sample/assemblies/repeating_multilayer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from __future__ import annotations
-
-from copy import deepcopy
+from typing import Union
 
 from easyCore.Objects.ObjectClasses import Parameter
 
+from EasyReflectometry.parameter_utils import get_as_parameter
+
 from ..elements.layers.layer import Layer
 from ..elements.layers.layer_collection import LayerCollection
 from .multilayer import Multilayer
 
-REPEATINGMULTILAYER_DETAILS = {
+DEFAULTS = {
     'repetitions': {
         'description': 'Number of repetitions of the given series of layers',
         'value': 1,
         'min': 1,
         'max': 9999,
         'fixed': True,
     }
@@ -31,83 +31,45 @@
     `repeating multilayer documentation`_
 
     .. _`repeating multilayer documentation`: ../sample/assemblies_library.html#repeatingmultilayer
     """
 
     def __init__(
         self,
-        layers: LayerCollection | Layer | list[Layer],
-        repetitions: Parameter,
+        layers: Union[LayerCollection, Layer, list[Layer], None] = None,
+        repetitions: Union[Parameter, int, None] = None,
         name: str = 'EasyRepeatingMultilayer',
         interface=None,
     ):
         """Constructor.
 
         :param layers: The layers that make up the multi-layer that will be repeated.
         :param repetitions: Number of repetitions of the given series of layers
         :param name: Name for the repeating multi layer, defaults to 'EasyRepeatingMultilayer'.
-        :param interface: Calculator interface, defaults to :py:attr:`None`.
+        :param interface: Calculator interface, defaults to `None`.
         """
 
-        if isinstance(layers, Layer):
+        if layers is None:
+            layers = LayerCollection()
+        elif isinstance(layers, Layer):
             layers = LayerCollection(layers, name=layers.name)
         elif isinstance(layers, list):
             layers = LayerCollection(*layers, name='/'.join([layer.name for layer in layers]))
+
+        repetitions = get_as_parameter('repetitions', repetitions, DEFAULTS)
+
         super().__init__(
             layers=layers,
             name=name,
             interface=interface,
             type='Repeating Multi-layer',
         )
         self._add_component('repetitions', repetitions)
         self.interface = interface
 
-    # Class methods for instance creation
-    @classmethod
-    def default(cls, interface=None) -> RepeatingMultilayer:
-        """Default instance of a repeating multi layer.
-
-        :return: Default repeating multi-layer container
-        """
-        layers = LayerCollection.default()
-        repetitions = Parameter('repetitions', **REPEATINGMULTILAYER_DETAILS['repetitions'])
-        return cls(
-            layers,
-            repetitions,
-            interface=interface,
-        )
-
-    @classmethod
-    def from_pars(
-        cls,
-        layers: LayerCollection,
-        repetitions: float = 1.0,
-        name: str = 'EasyRepeatingMultilayer',
-        interface=None,
-    ) -> RepeatingMultilayer:
-        """Instance of a repeating multi layer where the
-        parameters are known.
-
-        :param layers: The layers in the repeating multi layer.
-        :param repetitions: Number of repetitions, defaults to :py:attr`1`.
-        :param name: Name of the layer, defaults to 'EasyRepeatingMultilayer'.
-        :param interface: Calculator interface, defaults to :py:attr:`None`.
-        """
-        default_options = deepcopy(REPEATINGMULTILAYER_DETAILS)
-        del default_options['repetitions']['value']
-
-        repetitions = Parameter('repetitions', repetitions, **default_options['repetitions'])
-
-        return cls(
-            layers=layers,
-            repetitions=repetitions,
-            name=name,
-            interface=interface,
-        )
-
     # Representation
     @property
     def _dict_repr(self) -> dict:
         """A simplified dict representation."""
         d_dict = {self.name: self.layers._dict_repr}
         d_dict[self.name]['repetitions'] = self.repetitions.raw_value
         return d_dict
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/surfactant_layer.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/sample/assemblies/surfactant_layer.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,29 +23,53 @@
     `surfactant documentation`_
 
     .. _`surfactant documentation`: ../sample/assemblies_library.html#surfactantlayer
     """
 
     def __init__(
         self,
-        layers: list[LayerAreaPerMolecule],
+        tail_layer: Optional[LayerAreaPerMolecule] = None,
+        head_layer: Optional[LayerAreaPerMolecule] = None,
         name: str = 'EasySurfactantLayer',
         constrain_area_per_molecule: bool = False,
         conformal_roughness: bool = False,
         interface=None,
     ):
         """Constructor.
 
-        :param layers: List with the tail (index 0) and head (index 1) layer.
+        :param tail_layer: Layer representing the tail part of the surfactant layer.
+        :param head_layer: Layer representing the head part of the surfactant layer.
         :param name: Name for surfactant layer, defaults to 'EasySurfactantLayer'.
         :param constrain_area_per_molecule: Constrain the area per molecule, defaults to `False`.
         :param conformal_roughness: Constrain the roughness to be the same for both layers, defaults to `False`.
         :param interface: Calculator interface, defaults to `None`.
         """
-        surfactant = LayerCollection(layers[0], layers[1], name=name)
+        if tail_layer is None:
+            air = Material(0, 0, 'Air')
+            tail_layer = LayerAreaPerMolecule(
+                molecular_formula='C32D64',
+                thickness=16,
+                solvent=air,
+                solvent_fraction=0.0,
+                area_per_molecule=48.2,
+                roughness=3,
+                name='DPPC Tail',
+            )
+        if head_layer is None:
+            d2o = Material(6.36, 0, 'D2O')
+            head_layer = LayerAreaPerMolecule(
+                molecular_formula='C10H18NO8P',
+                thickness=10.0,
+                solvent=d2o,
+                solvent_fraction=0.2,
+                area_per_molecule=48.2,
+                roughness=3.0,
+                name='DPPC Head',
+            )
+        surfactant = LayerCollection(tail_layer, head_layer, name=name)
         super().__init__(
             name=name,
             type='Surfactant Layer',
             layers=surfactant,
             interface=interface,
         )
 
@@ -59,99 +83,14 @@
         self.tail_layer._area_per_molecule.user_constraints['area_per_molecule'] = area_per_molecule
         self.tail_layer._area_per_molecule.user_constraints['area_per_molecule'].enabled = constrain_area_per_molecule
 
         self._setup_roughness_constraints()
         if conformal_roughness:
             self._enable_roughness_constraints()
 
-    # Class methods for instance creation
-    @classmethod
-    def default(cls, interface=None) -> SurfactantLayer:
-        """Default instance of a surfactant layer object.
-        The default lipid type is DPPC.
-
-        :return: Surfactant layer object.
-        """
-        d2o = Material.from_pars(6.36, 0, 'D2O')
-        air = Material.from_pars(0, 0, 'Air')
-        tail = LayerAreaPerMolecule.from_pars(
-            molecular_formula='C32D64',
-            thickness=16,
-            solvent=air,
-            solvent_fraction=0.0,
-            area_per_molecule=48.2,
-            roughness=3,
-            name='DPPC Tail',
-        )
-        head = LayerAreaPerMolecule.from_pars(
-            molecular_formula='C10H18NO8P',
-            thickness=10.0,
-            solvent=d2o,
-            solvent_fraction=0.2,
-            area_per_molecule=48.2,
-            roughness=3.0,
-            name='DPPC Head',
-        )
-        return cls([tail, head], interface=interface)
-
-    @classmethod
-    def from_pars(
-        cls,
-        tail_layer_molecular_formula: str,
-        tail_layer_thickness: float,
-        tail_layer_solvent: Material,
-        tail_layer_solvent_fraction: float,
-        tail_layer_area_per_molecule: float,
-        tail_layer_roughness: float,
-        head_layer_molecular_formula: str,
-        head_layer_thickness: float,
-        head_layer_solvent: Material,
-        head_layer_solvent_fraction: float,
-        head_layer_area_per_molecule: float,
-        head_layer_roughness: float,
-        name: str = 'EasySurfactantLayer',
-        interface=None,
-    ) -> SurfactantLayer:
-        """Instance of a surfactant layer where the parameters are known,
-        `head_layer` is the hydrophilic part.
-
-        :param tail_layer_molecular_formula: Molecular formula of species constituting the tail layer.
-        :param tail_layer_thickness: Thickness of tail layer.
-        :param tail_layer_solvent: Solvent in tail layer.
-        :param tail_layer_solvent_fraction: Fraction of solvent in tail layer. Fx solvation or surface coverage.
-        :param tail_layer_area_per_molecule: Area per molecule of tail layer.
-        :param tail_layer_roughness: Roughness of tail layer.
-        :param head_layer_molecular_formula: Molecular formula of species constituting the head layer.
-        :param head_layer_thickness: Thickness of head layer.
-        :param head_layer_solvent: Solvent in head layer.
-        :param head_layer_solvent_fraction: Fraction of solvent in head layer. Fx solvation or surface coverage.
-        :param head_layer_area_per_molecule: Area per molecule of head layer.
-        :param head_layer_roughness: Roughness of head layer.
-        :param name: Name for surfactant layer.
-        """
-        head_layer = LayerAreaPerMolecule.from_pars(
-            molecular_formula=head_layer_molecular_formula,
-            thickness=head_layer_thickness,
-            solvent=head_layer_solvent,
-            solvent_fraction=head_layer_solvent_fraction,
-            area_per_molecule=head_layer_area_per_molecule,
-            roughness=head_layer_roughness,
-            name=name + ' Head Layer',
-        )
-        tail_layer = LayerAreaPerMolecule.from_pars(
-            molecular_formula=tail_layer_molecular_formula,
-            thickness=tail_layer_thickness,
-            solvent=tail_layer_solvent,
-            solvent_fraction=tail_layer_solvent_fraction,
-            area_per_molecule=tail_layer_area_per_molecule,
-            roughness=tail_layer_roughness,
-            name=name + ' Tail Layer',
-        )
-        return cls([tail_layer, head_layer], name, interface)
-
     @property
     def tail_layer(self) -> Optional[LayerAreaPerMolecule]:
         """Get the tail layer of the surfactant surface."""
         return self.front_layer
 
     @tail_layer.setter
     def tail_layer(self, layer: LayerAreaPerMolecule) -> None:
@@ -285,17 +224,18 @@
                 'area per molecule constrained': self.constrain_area_per_molecule,
                 'conformal roughness': self.conformal_roughness,
             }
         }
 
     def as_dict(self, skip: list = None) -> dict:
         """Produces a cleaned dict using a custom as_dict method to skip necessary things.
-        The resulting dict matches the paramters in __init__
+        The resulting dict matches the parameters in __init__
 
         :param skip: List of keys to skip, defaults to `None`.
         """
         this_dict = super().as_dict(skip=skip)
-        this_dict['layers']['data'][0] = self.tail_layer.as_dict()
-        this_dict['layers']['data'][1] = self.head_layer.as_dict()
+        this_dict['tail_layer'] = self.tail_layer.as_dict(skip=skip)
+        this_dict['head_layer'] = self.head_layer.as_dict(skip=skip)
         this_dict['constrain_area_per_molecule'] = self.constrain_area_per_molecule
         this_dict['conformal_roughness'] = self.conformal_roughness
+        del this_dict['layers']
         return this_dict
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/layers/layer.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/sample/elements/layers/layer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from __future__ import annotations
-
 __author__ = 'github.com/arm61'
+from typing import Union
 
-from copy import deepcopy
-
-from easyCore import np
+import numpy as np
 from easyCore.Objects.ObjectClasses import Parameter
 
+from EasyReflectometry.parameter_utils import get_as_parameter
+
 from ...base_core import BaseCore
 from ..materials.material import Material
 
-LAYER_DETAILS = {
+DEFAULTS = {
     'thickness': {
         'description': 'The thickness of the layer in angstroms',
         'url': 'https://github.com/reflectivity/edu_outreach/blob/master/refl_maths/paper.tex',
         'value': 10.0,
         'units': 'angstrom',
         'min': 0.0,
         'max': np.Inf,
@@ -39,83 +38,40 @@
     #: Thickness of the layer in Angstrom.
     thickness: Parameter
     #: Roughness of the layer in Angstrom.
     roughness: Parameter
 
     def __init__(
         self,
-        material: Material,
-        thickness: Parameter,
-        roughness: Parameter,
+        material: Union[Material, None] = None,
+        thickness: Union[Parameter, float, None] = None,
+        roughness: Union[Parameter, float, None] = None,
         name: str = 'EasyLayer',
         interface=None,
     ):
         """Constructor.
 
         :param material: The material for the layer.
         :param thickness: Layer thickness in Angstrom.
         :param roughness: Upper roughness on the layer in Angstrom.
         :param name: Name of the layer, defaults to 'EasyLayer'
-        :param interface: Interface object, defaults to :py:attr:`None`
+        :param interface: Interface object, defaults to `None`
         """
-        super().__init__(
-            name=name,
-            interface=interface,
-            material=material,
-            thickness=thickness,
-            roughness=roughness,
-        )
+        if material is None:
+            material = Material(interface=interface)
 
-    # Class methods for instance creation
-    @classmethod
-    def default(cls, interface=None) -> Layer:
-        """Default instance of the reflectometry layer.
+        thickness = get_as_parameter('thickness', thickness, DEFAULTS)
+        roughness = get_as_parameter('roughness', roughness, DEFAULTS)
 
-        :param interface: Calculator interface, defaults to :py:attr:`None`.
-        """
-        material = Material.default()
-        thickness = Parameter('thickness', **LAYER_DETAILS['thickness'])
-        roughness = Parameter('roughness', **LAYER_DETAILS['roughness'])
-        return cls(
-            material,
-            thickness,
-            roughness,
+        super().__init__(
+            name=name,
             interface=interface,
-        )
-
-    @classmethod
-    def from_pars(
-        cls,
-        material: Material,
-        thickness: float,
-        roughness: float,
-        name: str = 'EasyLayer',
-        interface=None,
-    ) -> Layer:
-        """Instance of a reflectometry layer where the parameters are known.
-
-        :param material: The material that makes up the layer.
-        :param thickness: Layer thickness in angstrom.
-        :param roughness: Layer roughness in angstrom.
-        :param name: Name of the layer, defaults to 'EasyLayer'.
-        :param interface: Calculator interface, defaults to :py:attr:`None`.
-        """
-        default_options = deepcopy(LAYER_DETAILS)
-        del default_options['thickness']['value']
-        del default_options['roughness']['value']
-
-        thickness = Parameter('thickness', thickness, **default_options['thickness'])
-        roughness = Parameter('roughness', roughness, **default_options['roughness'])
-
-        return cls(
             material=material,
             thickness=thickness,
             roughness=roughness,
-            name=name,
-            interface=interface,
         )
 
     def assign_material(self, material: Material) -> None:
         """Assign a material to the layer interface.
 
         :param material: The material to assign to the layer.
         """
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/sample/elements/materials/material.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from __future__ import annotations
-
 __author__ = 'github.com/arm61'
 
-from copy import deepcopy
-from typing import ClassVar
+from typing import Union
 
-from easyCore import np
+import numpy as np
 from easyCore.Objects.ObjectClasses import Parameter
 
+from EasyReflectometry.parameter_utils import get_as_parameter
+
 from ...base_core import BaseCore
 
-MATERIAL_DEFAULTS = {
+DEFAULTS = {
     'sld': {
         'description': 'The real scattering length density for a material in e-6 per squared angstrom.',
         'url': 'https://www.ncnr.nist.gov/resources/activation/',
         'value': 4.186,
         'units': '1 / angstrom ** 2',
         'min': -np.Inf,
         'max': np.Inf,
@@ -30,64 +29,35 @@
         'fixed': True,
     },
 }
 
 
 class Material(BaseCore):
     # Added in super().__init__
-    sld: ClassVar[Parameter]
-    isld: ClassVar[Parameter]
+    sld: Parameter
+    isld: Parameter
 
     def __init__(
         self,
-        sld: Parameter,
-        isld: Parameter,
+        sld: Union[Parameter, float, None] = None,
+        isld: Union[Parameter, float, None] = None,
         name: str = 'EasyMaterial',
         interface=None,
     ):
         """Constructor.
 
         :param sld: Real scattering length density.
         :param isld: Imaginary scattering length density.
         :param name: Name of the material, defaults to 'EasyMaterial'.
-        :param interface: Calculator interface, defaults to :py:attr:`None`.
+        :param interface: Calculator interface, defaults to `None`.
         """
-        super().__init__(name=name, interface=interface, sld=sld, isld=isld)
-
-    # Class methods for instance creation
-    @classmethod
-    def default(cls, interface=None) -> Material:
-        """Default instance of a material."""
-        sld = Parameter('sld', **MATERIAL_DEFAULTS['sld'])
-        isld = Parameter('isld', **MATERIAL_DEFAULTS['isld'])
-        return cls(sld, isld, interface=interface)
-
-    @classmethod
-    def from_pars(
-        cls,
-        sld: float,
-        isld: float,
-        name: str = 'EasyMaterial',
-        interface=None,
-    ) -> Material:
-        """Instance of a  material where the parameters are known.
-
-        :param sld: Real scattering length density.
-        :param isld: Imaginary scattering length density.
-        :param name: Name of the material, defaults to 'EasyMaterial'.
-        :param interface: Calculator interface, defaults to :py:attr:`None`.
-        """
-        default_options = deepcopy(MATERIAL_DEFAULTS)
-        del default_options['sld']['value']
-        del default_options['isld']['value']
-
-        sld = Parameter('sld', sld, **default_options['sld'])
-        isld = Parameter('isld', isld, **default_options['isld'])
+        sld = get_as_parameter('sld', sld, DEFAULTS)
+        isld = get_as_parameter('isld', isld, DEFAULTS)
 
-        return cls(sld=sld, isld=isld, name=name, interface=interface)
+        super().__init__(name=name, sld=sld, isld=isld, interface=interface)
 
     # Representation
     @property
     def _dict_repr(self) -> dict[str, str]:
         """A simplified dict representation."""
         return {
             self.name: {
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_density.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/sample/elements/materials/material_density.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from __future__ import annotations
-
-from copy import deepcopy
-from typing import ClassVar
+from typing import Union
 
 import numpy as np
 from easyCore.Fitting.Constraints import FunctionalConstraint
 from easyCore.Objects.ObjectClasses import Parameter
 
+from EasyReflectometry.parameter_utils import get_as_parameter
 from EasyReflectometry.special.calculations import density_to_sld
 from EasyReflectometry.special.calculations import molecular_weight
 from EasyReflectometry.special.calculations import neutron_scattering_length
 
-from .material import MATERIAL_DEFAULTS
+from .material import DEFAULTS as MATERIAL_DEFAULTS
 from .material import Material
 
-MATERIALDENSITY_DEFAULTS = {
+DEFAULTS = {
     'chemical_structure': 'Si',
     'sl': {
         'description': 'The real scattering length for a chemical formula in angstrom.',
         'url': 'https://www.ncnr.nist.gov/resources/activation/',
         'value': 4.1491,
         'units': 'angstrom',
         'min': -np.Inf,
@@ -49,57 +47,58 @@
         'value': 28.02,
         'units': 'g / mole',
         'min': -np.Inf,
         'max': np.Inf,
         'fixed': True,
     },
 }
+DEFAULTS.update(MATERIAL_DEFAULTS)
 
 
 class MaterialDensity(Material):
     # Added in __init__
-    scattering_length_real: ClassVar[Parameter]
-    scattering_length_imag: ClassVar[Parameter]
-    molecular_weight: ClassVar[Parameter]
-    density: ClassVar[Parameter]
+    scattering_length_real: Parameter
+    scattering_length_imag: Parameter
+    molecular_weight: Parameter
+    density: Parameter
 
     def __init__(
         self,
-        chemical_structure: str,
-        density: Parameter,
+        chemical_structure: Union[str, None] = None,
+        density: Union[Parameter, float, None] = None,
         name: str = 'EasyMaterialDensity',
         interface=None,
-    ) -> MaterialDensity:
+    ):
         """Constructor.
 
         :param chemical_structure: Chemical formula for the material.
         :param density: Mass density for the material.
-        :param name: Identifier, defaults to :py:attr:`EasyMaterialDensity`.
-        :param interface: Interface object, defaults to :py:attr:`None`.
+        :param name: Identifier, defaults to `EasyMaterialDensity`.
+        :param interface: Interface object, defaults to `None`.
         """
+        if chemical_structure is None:
+            chemical_structure = DEFAULTS['chemical_structure']
+
+        density = get_as_parameter('density', density, DEFAULTS)
+
         scattering_length = neutron_scattering_length(chemical_structure)
-        default_options = deepcopy(MATERIALDENSITY_DEFAULTS)
-        del default_options['molecular_weight']['value']
-        del default_options['sl']['value']
-        del default_options['isl']['value']
-        mw = Parameter('molecular_weight', molecular_weight(chemical_structure), **default_options['molecular_weight'])
-        scattering_length_real = Parameter('scattering_length_real', scattering_length.real, **default_options['sl'])
-        scattering_length_imag = Parameter('scattering_length_imag', scattering_length.imag, **default_options['isl'])
-        default_options = deepcopy(MATERIAL_DEFAULTS)
-        del default_options['sld']['value']
-        del default_options['isld']['value']
-        sld = Parameter(
-            'sld',
-            density_to_sld(scattering_length_real.raw_value, mw.raw_value, density.raw_value),
-            **default_options['sld'],
+
+        mw = get_as_parameter('molecular_weight', molecular_weight(chemical_structure), DEFAULTS)
+        scattering_length_real = get_as_parameter(
+            name='scattering_length_real',
+            value=scattering_length.real,
+            default_dict=DEFAULTS['sld'],
         )
-        isld = Parameter(
-            'isld',
-            density_to_sld(scattering_length_imag.raw_value, mw.raw_value, density.raw_value),
-            **default_options['isld'],
+        scattering_length_imag = get_as_parameter('scattering_length_imag', scattering_length.imag, DEFAULTS['isld'])
+
+        sld = get_as_parameter(
+            'sld', density_to_sld(scattering_length_real.raw_value, mw.raw_value, density.raw_value), DEFAULTS
+        )
+        isld = get_as_parameter(
+            'isld', density_to_sld(scattering_length_imag.raw_value, mw.raw_value, density.raw_value), DEFAULTS
         )
 
         constraint = FunctionalConstraint(sld, density_to_sld, [scattering_length_real, mw, density])
         scattering_length_real.user_constraints['sld'] = constraint
         mw.user_constraints['sld'] = constraint
         density.user_constraints['sld'] = constraint
         iconstraint = FunctionalConstraint(isld, density_to_sld, [scattering_length_imag, mw, density])
@@ -112,47 +111,14 @@
         self._add_component('scattering_length_real', scattering_length_real)
         self._add_component('scattering_length_imag', scattering_length_imag)
         self._add_component('molecular_weight', mw)
         self._add_component('density', density)
         self._chemical_structure = chemical_structure
         self.interface = interface
 
-    # Class methods for instance creation
-    @classmethod
-    def default(cls, interface=None) -> MaterialDensity:
-        """Default instance of material defined by density and chemical structure.
-
-        :param interface: Interface object, defaults to :py:attr:`None`
-        """
-        density = Parameter('density', **MATERIALDENSITY_DEFAULTS['density'])
-        return cls(MATERIALDENSITY_DEFAULTS['chemical_structure'], density, interface=interface)
-
-    @classmethod
-    def from_pars(
-        cls,
-        chemical_structure: str,
-        density: float,
-        name: str = 'EasyMaterialDensity',
-        interface=None,
-    ) -> MaterialDensity:
-        """Instance of a material from mass density and chemical structure,
-        where these are known.
-        :param chemical_structure: Chemical formula for the material
-        :param density: Mass density for the material
-        :param name: Identifier, defaults to :py:attr:`EasyMaterialDensity`
-        :param interface: Interface object, defaults to :py:attr:`None`
-        :return: Material container
-        """
-        default_options = deepcopy(MATERIALDENSITY_DEFAULTS)
-        del default_options['density']['value']
-
-        density = Parameter('density', density, **default_options['density'])
-
-        return cls(chemical_structure, density, name=name, interface=interface)
-
     @property
     def chemical_structure(self) -> str:
         """Get the chemical structure string."""
         return self._chemical_structure
 
     @chemical_structure.setter
     def chemical_structure(self, structure_string: str) -> None:
@@ -171,15 +137,15 @@
         mat_dict = super()._dict_repr
         mat_dict['chemical_structure'] = self._chemical_structure
         mat_dict['density'] = f'{self.density.raw_value:.2e} {self.density.unit}'
         return mat_dict
 
     def as_dict(self, skip: list = []) -> dict[str, str]:
         """Produces a cleaned dict using a custom as_dict method to skip necessary things.
-        The resulting dict matches the paramters in __init__
+        The resulting dict matches the parameters in __init__
 
         :param skip: List of keys to skip, defaults to `None`.
         """
         this_dict = super().as_dict(skip=skip)
         # From Material
         del this_dict['sld']
         del this_dict['isld']
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_mixture.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/sample/elements/materials/material_mixture.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,74 @@
-from __future__ import annotations
-
-from copy import deepcopy
-from typing import Optional
+from typing import Union
 
 from easyCore.Fitting.Constraints import FunctionalConstraint
 from easyCore.Objects.ObjectClasses import Parameter
 
+from EasyReflectometry.parameter_utils import get_as_parameter
 from EasyReflectometry.special.calculations import weighted_average
 
 from ...base_core import BaseCore
-from .material import MATERIAL_DEFAULTS
+from .material import DEFAULTS as MATERIAL_DEFAULTS
 from .material import Material
 
-MATERIALMIXTURE_DEFAULTS = {
+DEFAULTS = {
     'fraction': {
         'description': 'The fraction of material b in material a',
         'value': 0.5,
         'units': 'dimensionless',
         'min': 0,
         'max': 1,
         'fixed': True,
     }
 }
+DEFAULTS.update(MATERIAL_DEFAULTS)
 
 
 class MaterialMixture(BaseCore):
     # Added in super().__init__
     _material_a: Material
     _material_b: Material
     _fraction: Parameter
 
     def __init__(
         self,
-        material_a: Material,
-        material_b: Material,
-        fraction: Parameter,
-        name: Optional[str] = None,
+        material_a: Union[Material, None] = None,
+        material_b: Union[Material, None] = None,
+        fraction: Union[Parameter, float, None] = None,
+        name: Union[str, None] = None,
         interface=None,
     ):
         """Constructor.
 
         :param material_a: The first material.
         :param material_b: The second material.
         :param fraction: The fraction of material_b in material_a.
         :param name: Name of the material, defaults to None that causes the name to be constructed.
         :param interface: Calculator interface, defaults to `None`.
         """
+        if material_a is None:
+            material_a = Material(interface=interface)
+        if material_b is None:
+            material_b = Material(interface=interface)
+
+        fraction = get_as_parameter('fraction', fraction, DEFAULTS)
+
         sld = weighted_average(
             a=material_a.sld.raw_value,
             b=material_b.sld.raw_value,
             p=fraction.raw_value,
         )
         isld = weighted_average(
             a=material_a.isld.raw_value,
             b=material_b.isld.raw_value,
             p=fraction.raw_value,
         )
-        default_options = deepcopy(MATERIAL_DEFAULTS)
-        del default_options['sld']['value']
-        del default_options['isld']['value']
 
-        self._sld = Parameter('sld', sld, **default_options['sld'])
-        self._isld = Parameter('isld', isld, **default_options['isld'])
+        self._sld = get_as_parameter('sld', sld, DEFAULTS)
+        self._isld = get_as_parameter('isld', isld, DEFAULTS)
 
         # To avoid problems when setting the interface
         # self._sld and self._isld need to be declared before calling the super constructor
         super().__init__(
             name,
             _material_a=material_a,
             _material_b=material_b,
@@ -74,57 +77,14 @@
         )
         if name is None:
             self._update_name()
 
         self._materials_constraints()
         self.interface = interface
 
-    # Class constructors
-    @classmethod
-    def default(cls, interface=None) -> MaterialMixture:
-        """Default instance for a mixture of two materials."""
-        material_a = Material.default()
-        material_b = Material.default()
-        fraction = Parameter('fraction', **MATERIALMIXTURE_DEFAULTS['fraction'])
-        return cls(
-            material_a=material_a,
-            material_b=material_b,
-            fraction=fraction,
-            interface=interface,
-        )
-
-    @classmethod
-    def from_pars(
-        cls,
-        material_a: Material,
-        material_b: Material,
-        fraction: float,
-        name: Optional[str] = None,
-        interface=None,
-    ) -> MaterialMixture:
-        """Instance of mixture of two materials where the parameters are known.
-
-        :param material_a: The first material.
-        :param material_b: The second material.
-        :param fraction: The fraction of material_b in material_a.
-        :param name: Name of the material, defaults to 'EasyMaterialMixture'.
-        :param interface: Calculator interface, defaults to `None`.
-        """
-        default_options = deepcopy(MATERIALMIXTURE_DEFAULTS)
-        del default_options['fraction']['value']
-        fraction = Parameter('fraction', fraction, **default_options['fraction'])
-
-        return cls(
-            material_a=material_a,
-            material_b=material_b,
-            fraction=fraction,
-            name=name,
-            interface=interface,
-        )
-
     def _get_linkable_attributes(self):
         return [self._sld, self._isld]
 
     @property
     def sld(self) -> float:
         return self._sld.raw_value
 
@@ -218,15 +178,15 @@
                 'material_a': self._material_a._dict_repr,
                 'material_b': self._material_b._dict_repr,
             }
         }
 
     def as_dict(self, skip: list = None) -> dict[str, str]:
         """Produces a cleaned dict using a custom as_dict method to skip necessary things.
-        The resulting dict matches the paramters in __init__
+        The resulting dict matches the parameters in __init__
 
         :param skip: List of keys to skip, defaults to `None`.
         """
         this_dict = super().as_dict(skip=skip)
         this_dict['material_a'] = self._material_a.as_dict()
         this_dict['material_b'] = self._material_b.as_dict()
         this_dict['fraction'] = self._fraction.as_dict()
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_solvated.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/sample/elements/materials/material_solvated.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,102 +1,63 @@
-from __future__ import annotations
-
-from copy import deepcopy
+from typing import Union
 
 from easyCore.Objects.ObjectClasses import Parameter
 
+from EasyReflectometry.parameter_utils import get_as_parameter
+
 from .material import Material
 from .material_mixture import MaterialMixture
 
-MATERIAL_SOLVATED_DETAILS = {
+DEFAULTS = {
     'solvent_fraction': {
         'description': 'Fraction of solvent in layer.',
         'value': 0.2,
         'units': 'dimensionless',
         'min': 0,
         'max': 1,
         'fixed': True,
     },
 }
 
 
 class MaterialSolvated(MaterialMixture):
     def __init__(
         self,
-        material: Material,
-        solvent: Material,
-        solvent_fraction: Parameter,
+        material: Union[Material, None] = None,
+        solvent: Union[Material, None] = None,
+        solvent_fraction: Union[Parameter, float, None] = None,
         name=None,
         interface=None,
     ):
         """Constructor.
 
         :param material: The material being solvated.
         :param solvent: The solvent material.
         :param solvent_fraction: Fraction of solvent in layer. E.g. solvation or surface coverage.
         :param name: Name of the material, defaults to None that causes the name to be constructed.
         :param interface: Calculator interface, defaults to `None`.
         """
+        if material is None:
+            material = Material(sld=6.36, isld=0, name='D2O', interface=interface)
+        if solvent is None:
+            solvent = Material(sld=-0.561, isld=0, name='H2O', interface=interface)
+
+        solvent_fraction = get_as_parameter('solvent_fraction', solvent_fraction, DEFAULTS)
+
         # In super class, the fraction is the fraction of material b in material a
         super().__init__(
             material_a=material,
             material_b=solvent,
             fraction=solvent_fraction,
             name=name,
             interface=interface,
         )
         if name is None:
             self._update_name()
 
-    # Class methods for instance creation
-    @classmethod
-    def default(cls, interface=None) -> MaterialSolvated:
-        """A default instance for layer defined from molecule formula and area per molecule.
-
-        :param interface: Calculator interface, defaults to `None`.
-        """
-        solvent_fraction = Parameter('solvent_fraction', **MATERIAL_SOLVATED_DETAILS['solvent_fraction'])
-        material = Material.from_pars(6.36, 0, 'D2O', interface=interface)
-        solvent = Material.from_pars(-0.561, 0, 'H2O', interface=interface)
-        return cls(
-            material=material,
-            solvent=solvent,
-            solvent_fraction=solvent_fraction,
-            interface=interface,
-        )
-
-    @classmethod
-    def from_pars(
-        cls,
-        material: Material,
-        solvent: Material,
-        solvent_fraction: float,
-        name: str = 'EasyMaterialSolvated',
-        interface=None,
-    ) -> MaterialSolvated:
-        """An instance for a layer described with the area per molecule, where the parameters are known.
-
-        :param material: Material in the layer.
-        :param solvent: Solvent in the layer.
-        :param solvent_fraction: Fraction of solvent in layer. Fx solvation or surface coverage.
-        :param name: Identifier, defaults to 'EasyMaterialSolvated'.
-        :param interface: Calculator interface, defaults to `None`.
-        """
-        default_options = deepcopy(MATERIAL_SOLVATED_DETAILS)
-        del default_options['solvent_fraction']['value']
-        solvent_fraction = Parameter('coverage', solvent_fraction, **default_options['solvent_fraction'])
-
-        return cls(
-            material=material,
-            solvent=solvent,
-            solvent_fraction=solvent_fraction,
-            name=name,
-            interface=interface,
-        )
-
     @property
     def material(self) -> Material:
         """Get material."""
         return self._material_a
 
     @material.setter
     def material(self, new_material: Material) -> None:
@@ -116,14 +77,19 @@
         """Set the solvent.
 
         :param new_solvent: Solvent to be used.
         """
         self.material_b = new_solvent
 
     @property
+    def solvent_fraction_parameter(self) -> Parameter:
+        """Get the parameter for the fraction of layer described by the solvent."""
+        return self._fraction
+
+    @property
     def solvent_fraction(self) -> float:
         """Get the fraction of layer described by the solvent.
         This might be fraction of:
         Solvation where solvent is within the layer
         Patches of solvent in the layer where no material is present.
         """
         return self.fraction
@@ -159,15 +125,15 @@
                 'material': self.material._dict_repr,
                 'solvent': self.solvent._dict_repr,
             }
         }
 
     def as_dict(self, skip: list = None) -> dict[str, str]:
         """Produces a cleaned dict using a custom as_dict method to skip necessary things.
-        The resulting dict matches the paramters in __init__
+        The resulting dict matches the parameters in __init__
 
         :param skip: List of keys to skip, defaults to `None`.
         """
         this_dict = super().as_dict(skip=skip)
         this_dict['material'] = self.material.as_dict()
         this_dict['solvent'] = self.solvent.as_dict()
         this_dict['solvent_fraction'] = self._fraction.as_dict()
```

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/special/calculations.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/special/calculations.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/EasyReflectometry/special/parsing.py` & `easyreflectometrylib-0.0.7/EasyReflectometry/special/parsing.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/Makefile` & `easyreflectometrylib-0.0.7/docs/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line.
 SPHINXOPTS    =
 SPHINXBUILD   = python -msphinx
 SPHINXPROJ    = EasyReflectometry
-SOURCEDIR     = .
+SOURCEDIR     = ./src
 BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
```

### Comparing `easyreflectometrylib-0.0.6/docs/calculators.rst` & `easyreflectometrylib-0.0.7/docs/src/calculators.rst`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/conf.py` & `easyreflectometrylib-0.0.7/docs/src/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 #
 import datetime
 import os
 import sys
 import toml
 from pathlib import Path
 
-sys.path.insert(0, os.path.abspath('..'))
+sys.path.insert(0, os.path.abspath('../src'))
 
-main_root = Path(__file__).parents[1]
+main_root = Path(__file__).parents[2]
 sys.path.append(str(main_root))
 project_info = toml.load(os.path.join(main_root, 'pyproject.toml'))
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
@@ -112,15 +112,14 @@
 html_logo = os.path.join('_static', 'logo.png')
 html_favicon = os.path.join('_static', 'favicon.ico')
 html_theme_options = {
 #    'logo_only': True,
     'navigation_with_keys': True
 }
 html_baseurl = 'https://docs.easyreflectometry.org'
-
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
```

### Comparing `easyreflectometrylib-0.0.6/docs/installation.rst` & `easyreflectometrylib-0.0.7/docs/src/installation.rst`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/make.bat` & `easyreflectometrylib-0.0.7/docs/make.bat`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pushd %~dp0
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=python -msphinx
 )
-set SOURCEDIR=.
+set SOURCEDIR=./src
 set BUILDDIR=_build
 set SPHINXPROJ=orsopy
 
 if "%1" == "" goto help
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
```

### Comparing `easyreflectometrylib-0.0.6/docs/_static/favicon.ico` & `easyreflectometrylib-0.0.7/docs/src/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/_static/logo.png` & `easyreflectometrylib-0.0.7/docs/src/_static/logo.png`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/_static/logo.svg` & `easyreflectometrylib-0.0.7/docs/src/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/api/api.rst` & `easyreflectometrylib-0.0.7/docs/src/api/api.rst`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/sample/layer_library.rst` & `easyreflectometrylib-0.0.7/docs/src/sample/layer_library.rst`

 * *Files 8% similar despite different names*

```diff
@@ -10,50 +10,72 @@
 So we construct a :py:class:`Layer` as follows for a 100 Å thick layer of boron with a roughness of 10 Å. 
 
 .. code-block:: python
 
     from EasyReflectometry.sample import Material
     from EasyReflectometry.sample import Layer
 
-    b = Material.from_pars(
+    boron = Material(
         sld=6.908,
         isld=-0.278,
-        'Boron'
+        name='Boron'
     )
-    boron_layer = Layer.from_pars(
-        material=b,
+    boron_layer = Layer(
+        material=boron,
         thickness=100, 
         roughness=10,
         name='Boron Layer'
     )
 
 This type of layer is used extensively in the `tutorials`_
 
+To create a semi-infinite layer one needs to set the thickness to 0 and the roughness to 0.
+
+.. code-block:: python
+
+    from EasyReflectometry.sample import Material
+    from EasyReflectometry.sample import Layer
+
+    si = Material(
+        sld=2.07,
+        isld=0,
+        name='Si'
+    )
+    semi_infinite_layer = Layer(
+        material=si,
+        thickness=0,
+        roughness=0,
+        name='Si layer'
+    )
+
 :py:class:`LayerAreaPerMolecule`
 --------------------------------
 
 The :py:class:`LayerAreaPerMolecule` layer type is the fundation of the :py:class:`SurfactantLayer` assemblies type (further information on this can be found in the `assemblies library`_).
 The purpose of the :py:class:`LayerAreaPerMolecule` is to allow a layer to be defined in terms of the chemical formula of the material and the area per molecule of the layer. 
 The area per molecule is a common description of surface density in the surfactant monolayer and bilayer community. 
 
 We can construct a 10 Å thick :py:class:`LayerAreaPerMolecule` of phosphatidylcholine, with an area per molecule of 48 Å squared and a roughness of 3 Å that has 20 % solvent surface coverage with D2O using the following.
 
 .. code-block:: python
 
     from EasyReflectometry.sample import Material
     from EasyReflectometry.sample import LayerAreaPerMolecule
 
-    d2o = Material.from_pars(6.36, 0, 'D2O')
-
-    pc_formula = 'C10H18NO8P'
-    pc = LayerAreaPerMolecule.from_pars(
-        chemical_formula=pc_formula, 
+    d2o = Material(
+        sld=6.36,
+        isld=0,
+        name='D2O'
+    )
+    molecular_formula = 'C10H18NO8P'
+    pc = LayerAreaPerMolecule(
+        molecular_formula=molecular_formula, 
         thickness=10, 
         solvent=d2o, 
-        solvent_surface_coverage=.2,
+        solvent_fraction=.2,
         area_per_molecule=48, 
         roughness=3,
         name='PC Layer'
     )
 
 It is expected that the typical user will not interface directly with the :py:class:`LayerAreaPerMolecule` assembly type, but instead the :py:class:`SurfactantLayer` `assemblies library`_ will be used instead.
```

### Comparing `easyreflectometrylib-0.0.6/docs/sample/material_library.rst` & `easyreflectometrylib-0.0.7/docs/src/sample/material_library.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,66 +10,75 @@
 
 The simplest type of material that is available is the :py:class:`Material`.
 This allows the user to define a single type of material, with a real and imaginary component to the scattering length density. 
 The construction of a :py:class:`Material` is achieved as shown below. 
 
 .. code-block:: python 
 
-    from EasyReflectometry.sample.material import Material
+    from EasyReflectometry.sample import Material
 
-    b = Material.from_pars(6.908, -0.278, 'Boron')
+    boron = Material(
+        sld=6.908,
+        isld=-0.278,
+        name='Boron'
+    )
 
 The above object will have the properties of :py:attr:`sld` and :py:attr:`isld`, which will have values of :code:`6.908 1 / angstrom ** 2` and :code:`-0.278 1 / angstrom ** 2` respectively. 
 As is shown in the `tutorials`_, a material can be used to construct a :py:class:`Layer` from which `slab models`_ are created.
 
 :py:class:`MaterialDensity`
 ---------------------------
 
 In addition to defining a material by its scattering length density, it may be useful to define a material by the mass density and chemical formula. 
 This is possible with the :py:class:`MaterialDensity` material type, which uses the scattering length and atomic mass from the chemical formula and the density to determine the scattering length density. 
 It is then possible to vary the density, which defines the scattering length density in turn. 
 The :py:class:`MaterialDensity` material can be create as follows. 
 
 .. code-block:: python 
 
-    from EasyReflectometry.sample.material import MaterialDensity 
+    from EasyReflectometry.sample import MaterialDensity 
 
-    si = MaterialDensity.from_pars('SiO2', 2.65, 'SiO2 Material')
+    chemical_structure = 'SiO2'
+    si = MaterialDensity(
+        chemical_structure=chemical_structure,
+        density=2.65,
+        name='SiO2 Material'
+    )
 
 The density should be in units of grams per cubic centimeter and the scattering length is calculated from :code:`'SiO2'`. 
 
 :py:class:`MaterialSolvated`
 ----------------------------
 
 Sometimes it is desirable to have a layer that consists of a material and a solvent in some ratio.
 An example of this is shown in the `solvation tutorial`_, where a polymer film solvated with D2O is modelled. 
 To produce a material that is described by such a mixture, there is :py:class:`MaterialSolvated`. 
 This is constructed from two constituent :py:class:`Materials` and the fractional amount of the material in the solvent. 
 So to produce a :py:class:`MaterialSolvated` that is 20 % D2O in a polymer, the following is used. 
 
 .. code-block:: python
 
-    from EasyReflectometry.sample.material import Material 
-    from EasyReflectometry.sample.material import MaterialSolvated
+    from EasyReflectometry.sample import Material 
+    from EasyReflectometry.sample import MaterialSolvated
 
-    polymer = Material.from_pars(
+    polymer = Material(
         sld=2.,
         isld=0.,
         name='Polymer'
     )
-    d2o = Material.from_pars(
+    d2o = Material(
         sld=6.36,
         isld=0, 
         name='D2O'
     )
 
-    solvated_polymer = MaterialSolvated.from_pars(
+    solvated_polymer = MaterialSolvated(
         material=polymer, 
         solvent=d2o, 
-        solvent_surface_coverage=0.2, 
+        solvent_fraction=0.2, 
         name='Solvated Polymer'
     )
 
 For the :py:attr:`solvated_polymer` object, the :py:attr:`sld` will be :code:`2.872 1 / angstrom ** 2` (the weighted average of the two scattering length densities). 
 The :py:class:`MaterialSolvated` includes a constraint such that if the value of either constituent scattering length densities (both real and imaginary components) or the fraction changes, then the resulting material :py:attr:`sld` and :py:attr:`isld` will change appropriately. 
 
 .. _`assemblies`: ./assemblies_library.html
```

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/material_solvated.ipynb` & `easyreflectometrylib-0.0.7/docs/src/tutorials/material_solvated.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9917235392720307%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(12, 'from EasyReflectometry.experiment import Model\\n'), "*

 * *            "(13, 'from EasyReflectometry.experiment import "*

 * *            'percentage_fhwm_resolution_function\\n\')], delete: [12]}}, 8: {\'source\': ["si = '*

 * *            'Material(sld=2.07, isld=0, name=\'Si\')\\n", "sio2 = Material(sld=3.47, isld=0, '*

 * *            'name=\'SiO2\')\\n", "film = Material(sld=2.0, isld=0, name=\'Film\')\\n", "d2o = '*

 * *            'Material(sld=6.36, isld=0, name=\'D2O\')"]}, 10:  […]*

```diff
@@ -38,15 +38,16 @@
                 "import refnx\n",
                 "from EasyReflectometry.data import load\n",
                 "from EasyReflectometry.sample import Layer\n",
                 "from EasyReflectometry.sample import Sample\n",
                 "from EasyReflectometry.sample import Material\n",
                 "from EasyReflectometry.sample import MaterialSolvated\n",
                 "from EasyReflectometry.sample import Multilayer\n",
-                "from EasyReflectometry.experiment.model import Model\n",
+                "from EasyReflectometry.experiment import Model\n",
+                "from EasyReflectometry.experiment import percentage_fhwm_resolution_function\n",
                 "from EasyReflectometry.calculators import CalculatorFactory\n",
                 "from EasyReflectometry.fitting import Fitter\n",
                 "from EasyReflectometry.plot import plot"
             ]
         },
         {
             "cell_type": "markdown",
@@ -101,18 +102,18 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "60e5a3c5-58a8-429a-a446-a115f489af0f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "si = Material.from_pars(2.07, 0, 'Si')\n",
-                "sio2 = Material.from_pars(3.47, 0, 'SiO2')\n",
-                "film = Material.from_pars(2.0, 0, 'Film')\n",
-                "d2o = Material.from_pars(6.36, 0, 'D2O')"
+                "si = Material(sld=2.07, isld=0, name='Si')\n",
+                "sio2 = Material(sld=3.47, isld=0, name='SiO2')\n",
+                "film = Material(sld=2.0, isld=0, name='Film')\n",
+                "d2o = Material(sld=6.36, isld=0, name='D2O')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "64c79212-98f8-472c-8bb2-afbc09d7fe98",
             "metadata": {},
             "source": [
@@ -123,15 +124,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f2b910db-530f-49c5-907a-67712ba939d2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "solvated_film = MaterialSolvated.from_pars(\n",
+                "solvated_film = MaterialSolvated(\n",
                 "    material=film,\n",
                 "    solvent=d2o,\n",
                 "    solvent_fraction=0.25,\n",
                 "    name='Solvated Film'\n",
                 ")"
             ]
         },
@@ -169,24 +170,31 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f1ea2e41-f50e-4fbb-989f-aecc0e3e9860",
             "metadata": {},
             "outputs": [],
             "source": [
-                "si_layer = Layer.from_pars(si, 0, 0, 'Si layer')\n",
-                "sio2_layer = Layer.from_pars(sio2, 30, 3, 'SiO2 layer')\n",
-                "superphase = Multilayer.from_pars([si_layer, sio2_layer], name='Si/SiO2 Superphase')\n",
+                "si_layer = Layer(material=si, thickness=0, roughness=0, name='Si layer')\n",
+                "sio2_layer = Layer(material=sio2, thickness=30, roughness=3, name='SiO2 layer')\n",
+                "superphase = Multilayer([si_layer, sio2_layer], name='Si/SiO2 Superphase')\n",
                 "\n",
-                "solvated_film_layer = Layer.from_pars(solvated_film, 250, 3, 'Film Layer')\n",
+                "solvated_film_layer = Layer(material=solvated_film, thickness=250, roughness=3, name='Film Layer')\n",
                 "\n",
-                "subphase = Layer.from_pars(d2o, 0, 3, 'D2O Subphase')\n",
+                "subphase = Layer(material=d2o, thickness=0, roughness=3, name='D2O Subphase')\n",
                 "\n",
-                "sample = Sample.from_pars(superphase, solvated_film_layer, subphase, name='Film Structure')\n",
-                "model = Model.from_pars(sample, 1, 1e-6, 0.02, 'Film Model')"
+                "resolution_function = percentage_fhwm_resolution_function(0.02)\n",
+                "sample = Sample(superphase, solvated_film_layer, subphase, name='Film Structure')\n",
+                "model = Model(\n",
+                "    sample=sample,\n",
+                "    scale=1,\n",
+                "    background=1e-6,\n",
+                "    resolution_function=resolution_function,\n",
+                "    name='Film Model'\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "902042ee-0b7d-4515-9e4d-f7d34bae85af",
             "metadata": {},
             "source": [
@@ -333,27 +341,27 @@
             "source": [
                 "The fit reproducing the measured reflectivity curve yields that the scattering length density (SLD) of the layer is 2.36E-6 \u00c5<sup>-2</sup>.  Remember this layer is composed of 75% of the polymer film layer (SLD of 1.026E-6 \u00c5<sup>-2</sup> fitted) and 25% of D2O (SLD of 6.36E-6  \u00c5<sup>-2</sup> known) making (0.75 * 1.026 + 0.25 * 6.36)E-6 = 2.36E-6 \u00c5<sup>-2</sup>.  This is the same as the result from the [previous tutorial](./simple_fitting.rst)."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "erl_d",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.7"
+            "version": "3.11.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/monolayer.ipynb` & `easyreflectometrylib-0.0.7/docs/src/tutorials/monolayer.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090227166967125%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(10, 'from EasyReflectometry.sample import "*

 * *            "LayerAreaPerMolecule\\n'), (13, 'from EasyReflectometry.experiment import Model\\n'), "*

 * *            "(14, 'from EasyReflectometry.experiment import "*

 * *            'percentage_fhwm_resolution_function\\n\')], delete: [12]}}, 8: {\'source\': ["d2o = '*

 * *            'Material(sld=6.36, isld=0, name=\'D2O\')\\n", "air = Material(sld=0, isld=0, '*

 * *            'name=\'Air\')"]}, 18: {\'source\': {insert: [(0, \'tail_layer  […]*

```diff
@@ -33,17 +33,19 @@
                 "\n",
                 "import EasyReflectometry\n",
                 "from EasyReflectometry.calculators import CalculatorFactory\n",
                 "from EasyReflectometry.data import load\n",
                 "from EasyReflectometry.plot import plot\n",
                 "from EasyReflectometry.sample import Material\n",
                 "from EasyReflectometry.sample import SurfactantLayer\n",
+                "from EasyReflectometry.sample import LayerAreaPerMolecule\n",
                 "from EasyReflectometry.sample import Layer\n",
                 "from EasyReflectometry.sample import Sample\n",
-                "from EasyReflectometry.experiment.model import Model\n",
+                "from EasyReflectometry.experiment import Model\n",
+                "from EasyReflectometry.experiment import percentage_fhwm_resolution_function\n",
                 "from EasyReflectometry.fitting import Fitter\n",
                 "from EasyReflectometry.plot import plot\n",
                 "\n"
             ]
         },
         {
             "cell_type": "markdown",
@@ -123,16 +125,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "80c8d71f-d309-4104-bae6-3941daa525d3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "d2o = Material.from_pars(6.36, 0, 'D2O')\n",
-                "air = Material.from_pars(0, 0, 'Air')"
+                "d2o = Material(sld=6.36, isld=0, name='D2O')\n",
+                "air = Material(sld=0, isld=0, name='Air')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "31473f8e-7491-4d9a-8a7f-c1fc51abcc31",
             "metadata": {},
             "source": [
@@ -233,27 +235,33 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "4576f0b9-8815-46bc-b759-9f03379d2d0b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "dspc = SurfactantLayer.from_pars(\n",
-                "    tail_layer_molecular_formula=tail_formula,\n",
-                "    tail_layer_thickness=tail_thickness,\n",
-                "    tail_layer_solvent=air,\n",
-                "    tail_layer_solvent_fraction=tail_solvent_fraction, \n",
-                "    tail_layer_area_per_molecule=area_per_molecule,\n",
-                "    tail_layer_roughness=roughness,\n",
-                "    head_layer_molecular_formula=head_formula,\n",
-                "    head_layer_thickness=head_thickness,\n",
-                "    head_layer_solvent=d2o,\n",
-                "    head_layer_solvent_fraction=head_solvent_fraction, \n",
-                "    head_layer_area_per_molecule=area_per_molecule,\n",
-                "    head_layer_roughness=roughness\n",
+                "tail_layer = LayerAreaPerMolecule(\n",
+                "    molecular_formula=tail_formula,\n",
+                "    thickness=tail_thickness,\n",
+                "    solvent=air,\n",
+                "    solvent_fraction=tail_solvent_fraction, \n",
+                "    area_per_molecule=area_per_molecule,\n",
+                "    roughness=roughness\n",
+                ")\n",
+                "head_layer = LayerAreaPerMolecule(\n",
+                "    molecular_formula=head_formula,\n",
+                "    thickness=head_thickness,\n",
+                "    solvent=d2o,\n",
+                "    solvent_fraction=head_solvent_fraction, \n",
+                "    area_per_molecule=area_per_molecule,\n",
+                "    roughness=roughness\n",
+                ")\n",
+                "dspc = SurfactantLayer(\n",
+                "    tail_layer=tail_layer,\n",
+                "    head_layer=head_layer\n",
                 ")\n",
                 "dspc.constrain_area_per_molecule = True\n",
                 "dspc.conformal_roughness = True\n",
                 "dspc"
             ]
         },
         {
@@ -267,16 +275,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c17ecc32-c578-4a22-a12c-da13af1e0347",
             "metadata": {},
             "outputs": [],
             "source": [
-                "d2o_layer = Layer.from_pars(d2o, 0, 3, 'D2O Subphase')\n",
-                "air_layer = Layer.from_pars(air, 0, 0, 'Air Superphase')"
+                "d2o_layer = Layer(material=d2o, thickness=0, roughness=3, name='D2O Subphase')\n",
+                "air_layer = Layer(material=air, thickness=0, roughness=0, name='Air Superphase')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c8c3db09-b68a-4a8c-8b0c-61c716147a6c",
             "metadata": {},
             "source": [
@@ -305,16 +313,22 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "216bfe40-a97c-4437-a2f9-8bc7966ae58d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sample = Sample.from_pars(air_layer, dspc, d2o_layer)\n",
-                "model = Model.from_pars(sample, 1, data['data']['R_0'].values.min(), 5)"
+                "resolution_function = percentage_fhwm_resolution_function(5)\n",
+                "sample = Sample(air_layer, dspc, d2o_layer)\n",
+                "model = Model(\n",
+                "    sample=sample,\n",
+                "    scale=1,\n",
+                "    background=data['data']['R_0'].values.min(),\n",
+                "    resolution_function=resolution_function\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2f056fc0-347d-4946-af19-39245c39ca96",
             "metadata": {},
             "source": [
@@ -331,16 +345,16 @@
             "id": "d30eaa0f-be7f-4cbe-a7d6-11f43512f014",
             "metadata": {},
             "outputs": [],
             "source": [
                 "model.scale.bounds = (0.05, 1.5)\n",
                 "model.background.bounds = (4e-7, 1e-6)\n",
                 "\n",
-                "dspc.tail_layer.area_per_molecule.bounds = (30, 60)\n",
-                "dspc.head_layer.solvent_fraction.bounds = (0.4, 0.7)"
+                "dspc.tail_layer.area_per_molecule_parameter.bounds = (30, 60)\n",
+                "dspc.head_layer.solvent_fraction_parameter.bounds = (0.4, 0.7)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "514afa7a-cfa4-4ef9-a2c9-105c4d56ec6a",
             "metadata": {},
             "source": [
@@ -389,15 +403,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8dd6ead8-5019-44eb-9fc9-d8309443bc46",
             "metadata": {},
             "source": [
-                "We can see above that the solvent surface coverage of the surfactant was found to be around 60 % and the area per molecule around 50 \u00c5<sup>2</sup>, in agreement with [previous investigations](#mccluskey2019). "
+                "We can see above that the solvent surface coverage of the surfactant was found to be around 60 % (solvent_fraction in head_layer) and the area per molecule around 50 \u00c5<sup>2</sup>, in agreement with [previous investigations](#mccluskey2019). "
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0f056472-34f5-4c4a-9195-36a505087536",
             "metadata": {},
             "source": [
@@ -446,28 +460,14 @@
                 "McCluskey, A. R., Cooper, J. F. K., Arnold, T., Snow, T., **2020**,\n",
                 "*A general approach to maximise information density in neutron reflectometry analysis*,\n",
                 "[Machine Learning: Science and Technology, 1, 035002](https://doi.org/10.1088/2632-2153/ab94c4)"
             ]
         }
     ],
     "metadata": {
-        "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
-            "language": "python",
-            "name": "python3"
-        },
         "language_info": {
-            "codemirror_mode": {
-                "name": "ipython",
-                "version": 3
-            },
-            "file_extension": ".py",
-            "mimetype": "text/x-python",
-            "name": "python",
-            "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.11.7"
+            "name": "python"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/multi_contrast.ipynb` & `easyreflectometrylib-0.0.7/docs/src/tutorials/multi_contrast.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.894070350718635%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(9, 'from EasyReflectometry.sample import "*

 * *            "LayerAreaPerMolecule\\n'), (11, 'from EasyReflectometry.experiment import Model\\n'), "*

 * *            "(12, 'from EasyReflectometry.experiment import "*

 * *            'percentage_fhwm_resolution_function\\n\')], delete: [10]}}, 11: {\'source\': ["d2o = '*

 * *            'Material(sld=6.36, isld=0, name=\'D2O\')\\n", "acmw = Material(sld=0, isld=0, '*

 * *            'name=\'ACMW\')"]}, 13: {\'source\': ["air = Material(sld=0, i […]*

```diff
@@ -32,16 +32,18 @@
                 "import EasyReflectometry\n",
                 "import refnx\n",
                 "from EasyReflectometry.data import load\n",
                 "from EasyReflectometry.plot import plot\n",
                 "from EasyReflectometry.sample import Material\n",
                 "from EasyReflectometry.sample import SurfactantLayer\n",
                 "from EasyReflectometry.sample import Layer\n",
+                "from EasyReflectometry.sample import LayerAreaPerMolecule\n",
                 "from EasyReflectometry.sample import Sample\n",
-                "from EasyReflectometry.experiment.model import Model\n",
+                "from EasyReflectometry.experiment import Model\n",
+                "from EasyReflectometry.experiment import percentage_fhwm_resolution_function\n",
                 "from EasyReflectometry.calculators import CalculatorFactory\n",
                 "from EasyReflectometry.fitting import Fitter\n",
                 "print(f'EasyReflectometry: {EasyReflectometry.__version__}')\n",
                 "print(f'refnx: {refnx.__version__}')"
             ]
         },
         {
@@ -131,16 +133,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "58855c68-c95b-40de-9fee-a662771c247b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "d2o = Material.from_pars(6.36, 0, 'D2O')\n",
-                "acmw = Material.from_pars(0, 0, 'ACMW')"
+                "d2o = Material(sld=6.36, isld=0, name='D2O')\n",
+                "acmw = Material(sld=0, isld=0, name='ACMW')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f249860e-10a7-4ca6-82d5-44f275949dee",
             "metadata": {},
             "source": [
@@ -150,15 +152,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "08112c21-2027-47ba-845b-a3135439d862",
             "metadata": {},
             "outputs": [],
             "source": [
-                "air = Material.from_pars(0, 0, 'Air')"
+                "air = Material(sld=0, isld=0, name='Air')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b0fb931b-fa81-42ab-a907-fe5d384d003e",
             "metadata": {},
             "source": [
@@ -168,17 +170,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e7caedc2-8305-4f3b-bad2-c042bacb363b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "d2o_layer = Layer.from_pars(d2o, 0, 3, 'D2O Subphase')\n",
-                "acmw_layer = Layer.from_pars(acmw, 0, 3, 'D2O Subphase')\n",
-                "air_layer = Layer.from_pars(air, 0, 0, 'Air Superphase')"
+                "d2o_layer = Layer(material=d2o, thickness=0, roughness=3, name='D2O Subphase')\n",
+                "acmw_layer = Layer(material=acmw, thickness=0, roughness=3, name='D2O Subphase')\n",
+                "air_layer = Layer(material=air, thickness=0, roughness=0, name='Air Superphase')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "bb3c7fa9-162a-43b3-b70b-4d2813db2d29",
             "metadata": {},
             "source": [
@@ -197,67 +199,127 @@
                 "head_solvent_fraction = 0.5\n",
                 "tail_solvent_fraction = 0.0\n",
                 "area_per_molecule = 45\n",
                 "roughness = 3"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "e50a2ffd",
+            "metadata": {},
+            "source": [
+                "The `'d13DSPC-D2O'` surfactant layer "
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
-            "id": "021272e0-7abb-4703-a4cd-92daed10ae50",
+            "id": "c4aa6c00",
             "metadata": {},
             "outputs": [],
             "source": [
-                "d13d2o = SurfactantLayer.from_pars(\n",
-                "    tail_layer_molecular_formula=dspc['h-tail'], \n",
-                "    tail_layer_thickness=tail_thickness,\n",
-                "    tail_layer_solvent=d2o, \n",
-                "    tail_layer_solvent_fraction=tail_solvent_fraction, \n",
-                "    tail_layer_area_per_molecule=area_per_molecule,\n",
-                "    tail_layer_roughness=roughness,\n",
-                "    head_layer_molecular_formula=dspc['d-head'],\n",
-                "    head_layer_thickness=head_thickness, \n",
-                "    head_layer_solvent=d2o,\n",
-                "    head_layer_solvent_fraction=head_solvent_fraction, \n",
-                "    head_layer_area_per_molecule=area_per_molecule,\n",
-                "    head_layer_roughness=roughness\n",
+                "tail_layer_d13d2o = LayerAreaPerMolecule(\n",
+                "    molecular_formula=dspc['h-tail'],\n",
+                "    thickness=tail_thickness,\n",
+                "    solvent=air,\n",
+                "    solvent_fraction=tail_solvent_fraction,\n",
+                "    area_per_molecule=area_per_molecule,\n",
+                "    roughness=roughness\n",
+                ")\n",
+                "head_layer_d13d2o = LayerAreaPerMolecule(\n",
+                "    molecular_formula=dspc['d-head'],\n",
+                "    thickness=head_thickness,\n",
+                "    solvent=d2o,\n",
+                "    solvent_fraction=head_solvent_fraction,\n",
+                "    area_per_molecule=area_per_molecule,\n",
+                "    roughness=roughness\n",
+                ")\n",
+                "d13d2o = SurfactantLayer(\n",
+                "    tail_layer=tail_layer_d13d2o,\n",
+                "    head_layer=head_layer_d13d2o\n",
                 ")\n",
                 "d13d2o.constrain_area_per_molecule = True\n",
                 "d13d2o.conformal_roughness = True\n",
-                "d13d2o.constrain_solvent_roughness(d2o_layer)\n",
-                "d70d2o = SurfactantLayer.from_pars(\n",
-                "    tail_layer_molecular_formula=dspc['d-tail'],\n",
-                "    tail_layer_thickness=tail_thickness,\n",
-                "    tail_layer_solvent=d2o,\n",
-                "    tail_layer_solvent_fraction=tail_solvent_fraction, \n",
-                "    tail_layer_area_per_molecule=area_per_molecule,\n",
-                "    tail_layer_roughness=roughness,\n",
-                "    head_layer_molecular_formula=dspc['h-head'],\n",
-                "    head_layer_thickness=head_thickness,\n",
-                "    head_layer_solvent=d2o,\n",
-                "    head_layer_solvent_fraction=head_solvent_fraction, \n",
-                "    head_layer_area_per_molecule=area_per_molecule,\n",
-                "    head_layer_roughness=roughness\n",
+                "d13d2o.constrain_solvent_roughness(d2o_layer)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "55fe44f5",
+            "metadata": {},
+            "source": [
+                "The `'d70DSPC-D2O'` surfactant layer "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "16a970d8",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "tail_layer_d70d2o = LayerAreaPerMolecule(\n",
+                "    molecular_formula=dspc['d-tail'],\n",
+                "    thickness=tail_thickness,\n",
+                "    solvent=air,\n",
+                "    solvent_fraction=tail_solvent_fraction,\n",
+                "    area_per_molecule=area_per_molecule,\n",
+                "    roughness=roughness\n",
+                ")\n",
+                "head_layer_d70d2o = LayerAreaPerMolecule(\n",
+                "    molecular_formula=dspc['h-head'],\n",
+                "    thickness=head_thickness,\n",
+                "    solvent=d2o,\n",
+                "    solvent_fraction=head_solvent_fraction,\n",
+                "    area_per_molecule=area_per_molecule,\n",
+                "    roughness=roughness\n",
+                ")\n",
+                "d70d2o = SurfactantLayer(\n",
+                "    tail_layer=tail_layer_d70d2o,\n",
+                "    head_layer=head_layer_d70d2o\n",
                 ")\n",
                 "d70d2o.constrain_area_per_molecule = True\n",
                 "d70d2o.conformal_roughness = True\n",
-                "d70d2o.constrain_solvent_roughness(d2o_layer)\n",
-                "d83acmw = SurfactantLayer.from_pars(\n",
-                "    tail_layer_molecular_formula=dspc['d-tail'],\n",
-                "    tail_layer_thickness=tail_thickness,\n",
-                "    tail_layer_solvent=acmw,\n",
-                "    tail_layer_solvent_fraction=tail_solvent_fraction, \n",
-                "    tail_layer_area_per_molecule=area_per_molecule,\n",
-                "    tail_layer_roughness=roughness,\n",
-                "    head_layer_molecular_formula=dspc['d-head'],\n",
-                "    head_layer_thickness=head_thickness,\n",
-                "    head_layer_solvent=acmw,\n",
-                "    head_layer_solvent_fraction=head_solvent_fraction, \n",
-                "    head_layer_area_per_molecule=area_per_molecule,\n",
-                "    head_layer_roughness=roughness\n",
+                "d70d2o.constrain_solvent_roughness(d2o_layer)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "6f57d61d",
+            "metadata": {},
+            "source": [
+                "The `'d83DSPC-ACMW'` surfactant layer "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "021272e0-7abb-4703-a4cd-92daed10ae50",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "tail_layer_d83acmw = LayerAreaPerMolecule(\n",
+                "    molecular_formula=dspc['d-tail'],\n",
+                "    thickness=tail_thickness,\n",
+                "    solvent=air,\n",
+                "    solvent_fraction=tail_solvent_fraction,\n",
+                "    area_per_molecule=area_per_molecule,\n",
+                "    roughness=roughness\n",
+                ")\n",
+                "head_layer_d83acmw = LayerAreaPerMolecule(\n",
+                "    molecular_formula=dspc['d-head'],\n",
+                "    thickness=head_thickness,\n",
+                "    solvent=acmw,\n",
+                "    solvent_fraction=head_solvent_fraction,\n",
+                "    area_per_molecule=area_per_molecule,\n",
+                "    roughness=roughness\n",
+                ")\n",
+                "d83acmw = SurfactantLayer(\n",
+                "    tail_layer=tail_layer_d83acmw,\n",
+                "    head_layer=head_layer_d83acmw\n",
                 ")\n",
                 "d83acmw.constrain_area_per_molecule = True\n",
                 "d83acmw.conformal_roughness = True\n",
                 "d83acmw.constrain_solvent_roughness(acmw_layer)"
             ]
         },
         {
@@ -275,18 +337,18 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "24808923-ba02-4a7d-9be3-8d717b08aa8e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# These four lines should be removed in future\n",
-                "d70d2o.head_layer.area_per_molecule.enabled = True\n",
-                "d70d2o.tail_layer.area_per_molecule.enabled = True\n",
-                "d83acmw.head_layer.area_per_molecule.enabled = True\n",
-                "d83acmw.tail_layer.area_per_molecule.enabled = True\n",
+                "d70d2o.head_layer.area_per_molecule_parameter.enabled = True\n",
+                "d70d2o.tail_layer.area_per_molecule_parameter.enabled = True\n",
+                "d83acmw.head_layer.area_per_molecule_parameter.enabled = True\n",
+                "d83acmw.tail_layer.area_per_molecule_parameter.enabled = True\n",
                 "\n",
                 "d70d2o.constain_multiple_contrast(d13d2o)\n",
                 "d83acmw.constain_multiple_contrast(d70d2o)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -339,20 +401,37 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6e92498a-581b-445d-94cd-dda6474f1984",
             "metadata": {},
             "outputs": [],
             "source": [
-                "d13d2o_structure = Sample.from_pars(air_layer, d13d2o, d2o_layer)\n",
-                "d70d2o_structure = Sample.from_pars(air_layer, d70d2o, d2o_layer)\n",
-                "d83acmw_structure = Sample.from_pars(air_layer, d83acmw, acmw_layer)\n",
-                "d13d2o_model = Model.from_pars(d13d2o_structure, 0.1, data['data']['R_d13DSPC-D2O'].values.min(), 5)\n",
-                "d70d2o_model = Model.from_pars(d70d2o_structure, 0.1, data['data']['R_d70DSPC-D2O'].values.min(), 5)\n",
-                "d83acmw_model = Model.from_pars(d83acmw_structure, 0.1, data['data']['R_d83DSPC-ACMW'].values.min(), 5)"
+                "resolution_function = percentage_fhwm_resolution_function(5)\n",
+                "\n",
+                "d13d2o_sample = Sample(air_layer, d13d2o, d2o_layer)\n",
+                "d70d2o_sample = Sample(air_layer, d70d2o, d2o_layer)\n",
+                "d83acmw_sample = Sample(air_layer, d83acmw, acmw_layer)\n",
+                "d13d2o_model = Model(\n",
+                "    sample=d13d2o_sample,\n",
+                "    scale=0.1,\n",
+                "    background=data['data']['R_d13DSPC-D2O'].values.min(),\n",
+                "    resolution_function=resolution_function\n",
+                ")\n",
+                "d70d2o_model = Model(\n",
+                "    sample=d70d2o_sample,\n",
+                "    scale=0.1,\n",
+                "    background=data['data']['R_d70DSPC-D2O'].values.min(),\n",
+                "    resolution_function=resolution_function\n",
+                ")\n",
+                "d83acmw_model = Model(\n",
+                "    sample=d83acmw_sample,\n",
+                "    scale=0.1,\n",
+                "    background=data['data']['R_d83DSPC-ACMW'].values.min(),\n",
+                "    resolution_function=resolution_function\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f40ff64a-2777-4d9a-b7ff-ad0ac66f7916",
             "metadata": {},
             "source": [
@@ -373,16 +452,16 @@
                 "d13d2o_model.scale.bounds = (0.05, 1.5)\n",
                 "d13d2o_model.background.bounds = (4e-8, 1e-5)\n",
                 "d70d2o_model.scale.bounds = (0.05, 1.5)\n",
                 "d70d2o_model.background.bounds = (4e-8, 1e-5)\n",
                 "d83acmw_model.scale.bounds = (0.05, 1.5)\n",
                 "d83acmw_model.background.bounds = (4e-8, 1e-5)\n",
                 "\n",
-                "d13d2o.tail_layer.area_per_molecule.bounds = (40, 50)\n",
-                "d13d2o.head_layer.solvent_fraction.bounds = (0.2, 0.6)\n",
+                "d13d2o.tail_layer.area_per_molecule_parameter.bounds = (40, 50)\n",
+                "d13d2o.head_layer.solvent_fraction_parameter.bounds = (0.2, 0.6)\n",
                 "d13d2o.tail_layer.thickness.bounds = (18, 24)\n",
                 "d13d2o.head_layer.thickness.bounds = (8, 12)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "de0f41e9-785a-4591-8dfe-d694ef0d52b3",
@@ -445,43 +524,29 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "28f5d3e2-0e2f-4ef0-bc70-0f508b7fbc52",
             "metadata": {},
             "outputs": [],
             "source": [
-                "d13d2o.head_layer.area_per_molecule.raw_value, d70d2o.head_layer.area_per_molecule.raw_value, d83acmw.head_layer.area_per_molecule.raw_value"
+                "d13d2o.head_layer.area_per_molecule, d70d2o.head_layer.area_per_molecule, d83acmw.head_layer.area_per_molecule"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "faf00d17-55ea-45c3-be9e-772bf5cea70f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "plot(analysed)"
             ]
         }
     ],
     "metadata": {
-        "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
-            "language": "python",
-            "name": "python3"
-        },
         "language_info": {
-            "codemirror_mode": {
-                "name": "ipython",
-                "version": 3
-            },
-            "file_extension": ".py",
-            "mimetype": "text/x-python",
-            "name": "python",
-            "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.11.7"
+            "name": "python"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/repeating.ipynb` & `easyreflectometrylib-0.0.7/docs/src/tutorials/repeating.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090001123906353%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(11, 'from EasyReflectometry.experiment import Model\\n'), "*

 * *            "(12, 'from EasyReflectometry.experiment import "*

 * *            'percentage_fhwm_resolution_function\\n\')], delete: [11]}}, 10: {\'source\': ["vacuum '*

 * *            '= Material(sld=0, isld=0, name=\'Vacuum\')\\n", "ti = Material(sld=-1.9493, isld=0, '*

 * *            'name=\'Ti\')\\n", "ni = Material(sld=9.4245, isld=0, name=\'Ni\')\\n", "si = '*

 * *            'Material(sld=2.0704, isld=0, name=\'Si\')"]},  […]*

```diff
@@ -38,15 +38,16 @@
                 "import EasyReflectometry\n",
                 "import refl1d\n",
                 "from EasyReflectometry.data import load\n",
                 "from EasyReflectometry.sample import Layer\n",
                 "from EasyReflectometry.sample import Sample\n",
                 "from EasyReflectometry.sample import Material\n",
                 "from EasyReflectometry.sample import RepeatingMultilayer\n",
-                "from EasyReflectometry.experiment.model import Model\n",
+                "from EasyReflectometry.experiment import Model\n",
+                "from EasyReflectometry.experiment import percentage_fhwm_resolution_function\n",
                 "from EasyReflectometry.calculators import CalculatorFactory\n",
                 "from EasyReflectometry.fitting import Fitter\n",
                 "from EasyReflectometry.plot import plot"
             ]
         },
         {
             "cell_type": "markdown",
@@ -132,31 +133,31 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0f95d620-35b7-4b47-a3b4-9e33d5525b50",
             "metadata": {},
             "outputs": [],
             "source": [
-                "vacuum = Material.from_pars(0, 0, 'Vacuum')\n",
-                "ti = Material.from_pars(-1.9493, 0, 'Ti')\n",
-                "ni = Material.from_pars(9.4245, 0, 'Ni')\n",
-                "si = Material.from_pars(2.0704, 0, 'Si')"
+                "vacuum = Material(sld=0, isld=0, name='Vacuum')\n",
+                "ti = Material(sld=-1.9493, isld=0, name='Ti')\n",
+                "ni = Material(sld=9.4245, isld=0, name='Ni')\n",
+                "si = Material(sld=2.0704, isld=0, name='Si')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9a0b37ed-8714-4614-b49f-1e86ac232ac1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "superphase = Layer.from_pars(vacuum, 0, 0, 'Vacuum Superphase')\n",
-                "ti_layer = Layer.from_pars(ti, 40, 0, 'Ti Layer')\n",
-                "ni_layer = Layer.from_pars(ni, 70, 0, 'Ni Layer')\n",
-                "subphase = Layer.from_pars(si, 0, 0, 'Si Subphase')"
+                "superphase = Layer(material=vacuum, thickness=0, roughness=0, name='Vacuum Superphase')\n",
+                "ti_layer = Layer(material=ti, thickness=40, roughness=0, name='Ti Layer')\n",
+                "ni_layer = Layer(material=ni, thickness=70, roughness=0, name='Ni Layer')\n",
+                "subphase = Layer(material=si, thickness=0, roughness=0, name='Si Subphase')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f63ec440-089f-46cf-8ff5-be5012ad8dc8",
             "metadata": {},
             "source": [
@@ -167,15 +168,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "311b25a1-6d5d-4e91-a72e-394ad8dcf464",
             "metadata": {},
             "outputs": [],
             "source": [
-                "rep_multilayer = RepeatingMultilayer.from_pars([ti_layer, ni_layer], repetitions=10, name='NiTi Multilayer')\n",
+                "rep_multilayer = RepeatingMultilayer([ti_layer, ni_layer], repetitions=10, name='NiTi Multilayer')\n",
                 "rep_multilayer"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1c32d8ad-9baf-41bf-9fd8-419b92be36c4",
             "metadata": {},
@@ -186,16 +187,23 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fed8d60f-a4a7-40f1-8063-eb975bfa6115",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sample = Sample.from_pars(superphase, rep_multilayer, subphase, name='Multilayer Structure')\n",
-                "model = Model.from_pars(sample, 1, 0, 0, 'Multilayer Model')"
+                "resolution_function = percentage_fhwm_resolution_function(0)\n",
+                "sample = Sample(superphase, rep_multilayer, subphase, name='Multilayer Structure')\n",
+                "model = Model(\n",
+                "    sample=sample,\n",
+                "    scale=1,\n",
+                "    background=0,\n",
+                "    resolution_function=resolution_function,\n",
+                "    name='Multilayer Model'\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4a7dbfcf-05e8-4795-926b-b9c6af0f26dc",
             "metadata": {},
             "source": [
@@ -240,15 +248,15 @@
         {
             "cell_type": "markdown",
             "id": "defd6dd5-c618-4af6-a5c7-17532207f0a0",
             "metadata": {},
             "source": [
                 "## Performing an optimisation\n",
                 "\n",
-                "The [easyScience](https://easyscience.github.io/easyCore/) framework allows us to access a broad range of optimisation methods.\n",
+                "The [easyScience](https://easyscience.github.io/easyscience/) framework allows us to access a broad range of optimisation methods.\n",
                 "Below, we have selected the [differential evolution method from lmfit](https://lmfit.github.io/lmfit-py/examples/example_diffev.rst)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "880d10d7-b655-4ef1-b376-21b2e4394160",
@@ -303,28 +311,14 @@
             "metadata": {},
             "source": [
                 "This result of a thickness of 30 \u00c5 is the same as that which is used to produce the data. "
             ]
         }
     ],
     "metadata": {
-        "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
-            "language": "python",
-            "name": "python3"
-        },
         "language_info": {
-            "codemirror_mode": {
-                "name": "ipython",
-                "version": 3
-            },
-            "file_extension": ".py",
-            "mimetype": "text/x-python",
-            "name": "python",
-            "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.11.7"
+            "name": "python"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/simple_fitting.ipynb` & `easyreflectometrylib-0.0.7/docs/src/tutorials/simple_fitting.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9095143110435664%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(9, 'from EasyReflectometry.experiment import Model\\n'), "*

 * *            "(10, 'from EasyReflectometry.experiment import "*

 * *            'percentage_fhwm_resolution_function\\n\')], delete: [9]}}, 12: {\'source\': ["si = '*

 * *            'Material(sld=2.07, isld=0, name=\'Si\')\\n", "sio2 = Material(sld=3.47, isld=0, '*

 * *            'name=\'SiO2\')\\n", "film = Material(sld=2.0, isld=0, name=\'Film\')\\n", "d2o = '*

 * *            'Material(sld=6.36, isld=0, name=\'D2O\')"]}, 16: { […]*

```diff
@@ -32,15 +32,16 @@
                 "import EasyReflectometry\n",
                 "import refnx\n",
                 "from EasyReflectometry.data import load\n",
                 "from EasyReflectometry.sample import Layer\n",
                 "from EasyReflectometry.sample import Sample\n",
                 "from EasyReflectometry.sample import Material\n",
                 "from EasyReflectometry.sample import Multilayer\n",
-                "from EasyReflectometry.experiment.model import Model\n",
+                "from EasyReflectometry.experiment import Model\n",
+                "from EasyReflectometry.experiment import percentage_fhwm_resolution_function\n",
                 "from EasyReflectometry.calculators import CalculatorFactory\n",
                 "from EasyReflectometry.fitting import Fitter\n",
                 "from EasyReflectometry.plot import plot"
             ]
         },
         {
             "cell_type": "markdown",
@@ -148,18 +149,18 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1fd5d9ba-a912-40f1-96a9-8d8d85c35c18",
             "metadata": {},
             "outputs": [],
             "source": [
-                "si = Material.from_pars(2.07, 0, 'Si')\n",
-                "sio2 = Material.from_pars(3.47, 0, 'SiO2')\n",
-                "film = Material.from_pars(2.0, 0, 'Film')\n",
-                "d2o = Material.from_pars(6.36, 0, 'D2O')"
+                "si = Material(sld=2.07, isld=0, name='Si')\n",
+                "sio2 = Material(sld=3.47, isld=0, name='SiO2')\n",
+                "film = Material(sld=2.0, isld=0, name='Film')\n",
+                "d2o = Material(sld=6.36, isld=0, name='D2O')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "7c31f6ab-6a22-4ac6-a058-b7bbac241211",
             "metadata": {},
             "source": [
@@ -187,18 +188,18 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "bfd2d8a1-35fe-4a6c-aeee-93f1b4066b61",
             "metadata": {},
             "outputs": [],
             "source": [
-                "si_layer = Layer.from_pars(si, 0, 0, 'Si layer')\n",
-                "sio2_layer = Layer.from_pars(sio2, 30, 3, 'SiO2 layer')\n",
-                "film_layer = Layer.from_pars(film, 250, 3, 'Film Layer')\n",
-                "subphase = Layer.from_pars(d2o, 0, 3, 'D2O Subphase')"
+                "si_layer = Layer(material=si, thickness=0, roughness=0, name='Si layer')\n",
+                "sio2_layer = Layer(material=sio2, thickness=30, roughness=3, name='SiO2 layer')\n",
+                "film_layer = Layer(material=film, thickness=250, roughness=3, name='Film Layer')\n",
+                "subphase = Layer(material=d2o, thickness=0, roughness=3, name='D2O Subphase')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8e165a80-66d9-469f-a013-e776e63513e6",
             "metadata": {},
             "source": [
@@ -226,15 +227,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a6508395-d292-4338-9fbe-77e19b011ae6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "superphase = Multilayer.from_pars([si_layer, sio2_layer], name='Si/SiO2 Superphase')"
+                "superphase = Multilayer([si_layer, sio2_layer], name='Si/SiO2 Superphase')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a3a2df9b-8ddb-4b3e-a5c3-55b72280b651",
             "metadata": {},
             "source": [
@@ -244,15 +245,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2a0aee2a-e77e-4558-a8b0-ef2d1cffd4d0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sample = Sample.from_pars(superphase, film_layer, subphase, name='Film Structure')"
+                "sample = Sample(superphase, film_layer, subphase, name='Film Structure')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b3e5d88e-3da4-4a3e-8067-80e9cd35be8f",
             "metadata": {},
             "source": [
@@ -282,25 +283,32 @@
                 "    \n",
                 "Note\n",
                 "    \n",
                 "Currently, only constant with resolution is supported. We are working to include more complex resolution in future.\n",
                 "\n",
                 "</div>\n",
                 "\n",
-                "the `Model` constructor takes our smple, a scale factor, a uniform background level and a resolution width. "
+                "the `Model` constructor takes our smple, a scale factor, a uniform background level and a resolution function. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8646c977-28b4-4cd4-adbd-fc263359ca1c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "model = Model.from_pars(sample, 1, 1e-6, 0.02, 'Film Model')"
+                "resolution_function = percentage_fhwm_resolution_function(0.02)\n",
+                "model = Model(\n",
+                "    sample=sample,\n",
+                "    scale=1,\n",
+                "    background=1e-6,\n",
+                "    resolution_function=resolution_function,\n",
+                "    name='Film Model'\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d22153d8-63d9-4542-8b29-4ff7dd73b79a",
             "metadata": {},
             "source": [
@@ -501,28 +509,14 @@
             "metadata": {},
             "source": [
                 "We note here that the results obtained are very similar to those from the [*refnx* tutorial](https://refnx.readthedocs.io/en/latest/getting_started.html#Fitting-a-neutron-reflectometry-dataset), which is hardly surprising given that we have used the *refnx* engine in this example."
             ]
         }
     ],
     "metadata": {
-        "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
-            "language": "python",
-            "name": "python3"
-        },
         "language_info": {
-            "codemirror_mode": {
-                "name": "ipython",
-                "version": 3
-            },
-            "file_extension": ".py",
-            "mimetype": "text/x-python",
-            "name": "python",
-            "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.11.7"
+            "name": "python"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/_static/d70d2o.ort` & `easyreflectometrylib-0.0.7/docs/src/tutorials/_static/d70d2o.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/_static/dspc.png` & `easyreflectometrylib-0.0.7/docs/src/tutorials/_static/dspc.png`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/_static/example.ort` & `easyreflectometrylib-0.0.7/docs/src/tutorials/_static/example.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/_static/monolayer.png` & `easyreflectometrylib-0.0.7/docs/src/tutorials/_static/monolayer.png`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/_static/monolayer.svg` & `easyreflectometrylib-0.0.7/docs/src/tutorials/_static/monolayer.svg`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/_static/multiple.ort` & `easyreflectometrylib-0.0.7/docs/src/tutorials/_static/multiple.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/_static/polymer_film.png` & `easyreflectometrylib-0.0.7/docs/src/tutorials/_static/polymer_film.png`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/_static/polymer_film.svg` & `easyreflectometrylib-0.0.7/docs/src/tutorials/_static/polymer_film.svg`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/_static/repeating.png` & `easyreflectometrylib-0.0.7/docs/src/tutorials/_static/repeating.png`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/_static/repeating.svg` & `easyreflectometrylib-0.0.7/docs/src/tutorials/_static/repeating.svg`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/docs/tutorials/_static/repeating_layers.ort` & `easyreflectometrylib-0.0.7/docs/src/tutorials/_static/repeating_layers.ort`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #         affiliation: European Spallation Source
 #         contact: andrew.mccluskey@ess.eu
 #     experiment:
 #         facility: Simulated
 #         start_date: 2022-02-01
 #         title: Ni-Ti Multilayer
 #         instrument: Simulation
-#         probe: x-rays
+#         probe: x-ray
 #     sample:
 #         name: Ni-Ti Multilayer on Si
 #         category: gas / lsolidiquid
 #         composition: Air / (Ni / Ti) x 10 / Si
 #     measurement:
 #         instrument_settings:
 #             wavelength:
```

### Comparing `easyreflectometrylib-0.0.6/tests/test_data.py` & `easyreflectometrylib-0.0.7/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/tests/test_fitting.py` & `easyreflectometrylib-0.0.7/tests/test_fitting.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,44 +2,46 @@
 
 import os
 import unittest
 
 import EasyReflectometry
 from EasyReflectometry.calculators import CalculatorFactory
 from EasyReflectometry.data import load
-from EasyReflectometry.experiment.model import Model
+from EasyReflectometry.experiment import Model
+from EasyReflectometry.experiment import percentage_fhwm_resolution_function
 from EasyReflectometry.fitting import Fitter
 from EasyReflectometry.sample import Layer
 from EasyReflectometry.sample import Material
 from EasyReflectometry.sample import Sample
 
 
 class TestFitting(unittest.TestCase):
     def test_fitting(self):
         fpath = os.path.join(
             os.path.dirname(os.path.dirname(EasyReflectometry.__file__)),
             'tests/_static/example.ort',
         )
         data = load(fpath)
-        si = Material.from_pars(2.07, 0, 'Si')
-        sio2 = Material.from_pars(3.47, 0, 'SiO2')
-        film = Material.from_pars(2.0, 0, 'Film')
-        d2o = Material.from_pars(6.36, 0, 'D2O')
-        si_layer = Layer.from_pars(si, 0, 0, 'Si layer')
-        sio2_layer = Layer.from_pars(sio2, 30, 3, 'SiO2 layer')
-        film_layer = Layer.from_pars(film, 250, 3, 'Film Layer')
-        superphase = Layer.from_pars(d2o, 0, 3, 'D2O Subphase')
-        sample = Sample.from_pars(
+        si = Material(2.07, 0, 'Si')
+        sio2 = Material(3.47, 0, 'SiO2')
+        film = Material(2.0, 0, 'Film')
+        d2o = Material(6.36, 0, 'D2O')
+        si_layer = Layer(si, 0, 0, 'Si layer')
+        sio2_layer = Layer(sio2, 30, 3, 'SiO2 layer')
+        film_layer = Layer(film, 250, 3, 'Film Layer')
+        superphase = Layer(d2o, 0, 3, 'D2O Subphase')
+        sample = Sample(
             si_layer,
             sio2_layer,
             film_layer,
             superphase,
             name='Film Structure',
         )
-        model = Model.from_pars(sample, 1, 1e-6, 0.02, 'Film Model')
+        resolution_function = percentage_fhwm_resolution_function(0.02)
+        model = Model(sample, 1, 1e-6, resolution_function, 'Film Model')
         # Thicknesses
         sio2_layer.thickness.bounds = (15, 50)
         film_layer.thickness.bounds = (200, 300)
         # Roughnesses
         sio2_layer.roughness.bounds = (1, 15)
         film_layer.roughness.bounds = (1, 15)
         superphase.roughness.bounds = (1, 15)
```

### Comparing `easyreflectometrylib-0.0.6/tests/_static/example.ort` & `easyreflectometrylib-0.0.7/tests/_static/example.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/tests/_static/test_example1.ort` & `easyreflectometrylib-0.0.7/tests/_static/test_example1.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/tests/_static/test_example2.ort` & `easyreflectometrylib-0.0.7/tests/_static/test_example2.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/tests/_static/test_example3.ort` & `easyreflectometrylib-0.0.7/tests/_static/test_example3.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/tests/_static/test_example4.ort` & `easyreflectometrylib-0.0.7/tests/_static/test_example4.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/tests/calculators/bornagain/test_bornagain_calculator.py` & `easyreflectometrylib-0.0.7/tests/calculators/bornagain/test_bornagain_calculator.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/tests/calculators/bornagain/test_bornagain_wrapper.py` & `easyreflectometrylib-0.0.7/tests/calculators/bornagain/test_bornagain_wrapper.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/tests/calculators/refl1d/test_refl1d_calculator.py` & `easyreflectometrylib-0.0.7/tests/calculators/refl1d/test_refl1d_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Tests for Refnx calculator.
 """
+
 __author__ = 'github.com/arm61'
 __version__ = '0.0.1'
 
 import unittest
 
 import numpy as np
 from numpy.testing import assert_almost_equal
@@ -20,27 +21,26 @@
         assert_equal(p._material_link['sld'], 'rho')
         assert_equal(p._material_link['isld'], 'irho')
         assert_equal(p._layer_link['thickness'], 'thickness')
         assert_equal(p._layer_link['roughness'], 'interface')
         assert_equal(p._item_link['repetitions'], 'repeat')
         assert_equal(p._model_link['scale'], 'scale')
         assert_equal(p._model_link['background'], 'bkg')
-        assert_equal(p._model_link['resolution'], 'dq')
         assert_equal(p.name, 'refl1d')
 
     def test_fit_func(self):
         p = Refl1d()
         p._wrapper.create_material('Material1')
         p._wrapper.update_material('Material1', rho=0.000, irho=0.000)
         p._wrapper.create_material('Material2')
         p._wrapper.update_material('Material2', rho=2.000, irho=0.000)
         p._wrapper.create_material('Material3')
         p._wrapper.update_material('Material3', rho=4.000, irho=0.000)
         p._wrapper.create_model('MyModel')
-        p._wrapper.update_model('MyModel', bkg=1e-7, dq=5.0)
+        p._wrapper.update_model('MyModel', bkg=1e-7)
         p._wrapper.create_layer('Layer1')
         p._wrapper.assign_material_to_layer('Material1', 'Layer1')
         p._wrapper.create_layer('Layer2')
         p._wrapper.assign_material_to_layer('Material2', 'Layer2')
         p._wrapper.update_layer('Layer2', thickness=10, interface=1.0)
         p._wrapper.create_layer('Layer3')
         p._wrapper.assign_material_to_layer('Material3', 'Layer3')
@@ -70,15 +70,15 @@
         p._wrapper.create_material('Material1')
         p._wrapper.update_material('Material1', rho=0.000, irho=0.000)
         p._wrapper.create_material('Material2')
         p._wrapper.update_material('Material2', rho=2.000, irho=0.000)
         p._wrapper.create_material('Material3')
         p._wrapper.update_material('Material3', rho=4.000, irho=0.000)
         p._wrapper.create_model('MyModel')
-        p._wrapper.update_model('MyModel', bkg=1e-7, dq=5.0)
+        p._wrapper.update_model('MyModel', bkg=1e-7)
         p._wrapper.create_layer('Layer1')
         p._wrapper.assign_material_to_layer('Material1', 'Layer1')
         p._wrapper.create_layer('Layer2')
         p._wrapper.assign_material_to_layer('Material2', 'Layer2')
         p._wrapper.update_layer('Layer2', thickness=10, interface=1.0)
         p._wrapper.create_layer('Layer3')
         p._wrapper.assign_material_to_layer('Material3', 'Layer3')
```

### Comparing `easyreflectometrylib-0.0.6/tests/calculators/refnx/test_refnx_calculator.py` & `easyreflectometrylib-0.0.7/tests/calculators/refnx/test_refnx_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Tests for Refnx calculator.
 """
+
 __author__ = 'github.com/arm61'
 __version__ = '0.0.1'
 
 import unittest
 
 import numpy as np
 from numpy.testing import assert_almost_equal
@@ -20,15 +21,14 @@
         assert_equal(p._material_link['sld'], 'real')
         assert_equal(p._material_link['isld'], 'imag')
         assert_equal(p._layer_link['thickness'], 'thick')
         assert_equal(p._layer_link['roughness'], 'rough')
         assert_equal(p._item_link['repetitions'], 'repeats')
         assert_equal(p._model_link['scale'], 'scale')
         assert_equal(p._model_link['background'], 'bkg')
-        assert_equal(p._model_link['resolution'], 'dq')
         assert_equal(p.name, 'refnx')
 
     def test_fit_func(self):
         p = Refnx()
         p._wrapper.create_material('Material1')
         p._wrapper.update_material('Material1', real=0.000, imag=0.000)
         p._wrapper.create_material('Material2')
```

### Comparing `easyreflectometrylib-0.0.6/tests/experiment/test_model.py` & `easyreflectometrylib-0.0.7/tests/experiment/test_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,33 +3,36 @@
 """
 
 __author__ = 'github.com/arm61'
 __version__ = '0.0.1'
 
 
 import unittest
+from unittest.mock import MagicMock
 
 import numpy as np
 import pytest
 from numpy.testing import assert_equal
 
 from EasyReflectometry.calculators import CalculatorFactory
-from EasyReflectometry.experiment.model import Model
+from EasyReflectometry.experiment import Model
+from EasyReflectometry.experiment import linear_spline_resolution_function
+from EasyReflectometry.experiment import percentage_fhwm_resolution_function
 from EasyReflectometry.sample import Layer
 from EasyReflectometry.sample import LayerCollection
 from EasyReflectometry.sample import Material
 from EasyReflectometry.sample import Multilayer
 from EasyReflectometry.sample import RepeatingMultilayer
 from EasyReflectometry.sample import Sample
 from EasyReflectometry.sample import SurfactantLayer
 
 
 class TestModel(unittest.TestCase):
     def test_default(self):
-        p = Model.default()
+        p = Model()
         assert_equal(p.name, 'EasyModel')
         assert_equal(p.interface, None)
         assert_equal(p.sample.name, 'EasySample')
         assert_equal(p.scale.display_name, 'scale')
         assert_equal(str(p.scale.unit), 'dimensionless')
         assert_equal(p.scale.value.value.magnitude, 1.0)
         assert_equal(p.scale.min, 0.0)
@@ -37,32 +40,35 @@
         assert_equal(p.scale.fixed, True)
         assert_equal(p.background.display_name, 'background')
         assert_equal(str(p.background.unit), 'dimensionless')
         assert_equal(p.background.value.value.magnitude, 1.0e-8)
         assert_equal(p.background.min, 0.0)
         assert_equal(p.background.max, np.Inf)
         assert_equal(p.background.fixed, True)
-        assert_equal(p.resolution.display_name, 'resolution')
-        assert_equal(str(p.resolution.unit), 'dimensionless')
-        assert_equal(p.resolution.value.value.magnitude, 5.0)
-        assert_equal(p.resolution.min, 0.0)
-        assert_equal(p.resolution.max, 100.0)
-        assert_equal(p.resolution.fixed, True)
+        assert p._resolution_function([1]) == 5.0
+        assert p._resolution_function([100]) == 5.0
 
     def test_from_pars(self):
-        m1 = Material.from_pars(6.908, -0.278, 'Boron')
-        m2 = Material.from_pars(0.487, 0.000, 'Potassium')
-        l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
-        l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
-        ls1 = LayerCollection.from_pars(l1, l2, name='twoLayer1')
-        ls2 = LayerCollection.from_pars(l2, l1, name='twoLayer2')
-        o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
-        o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
-        d = Sample.from_pars(o1, o2, name='myModel')
-        mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel')
+        m1 = Material(6.908, -0.278, 'Boron')
+        m2 = Material(0.487, 0.000, 'Potassium')
+        l1 = Layer(m1, 5.0, 2.0, 'thinBoron')
+        l2 = Layer(m2, 50.0, 1.0, 'thickPotassium')
+        ls1 = LayerCollection(l1, l2, name='twoLayer1')
+        ls2 = LayerCollection(l2, l1, name='twoLayer2')
+        o1 = RepeatingMultilayer(ls1, 2.0, 'twoLayerItem1')
+        o2 = RepeatingMultilayer(ls2, 1.0, 'oneLayerItem2')
+        d = Sample(o1, o2, name='myModel')
+        resolution_function = percentage_fhwm_resolution_function(2.0)
+        mod = Model(
+            sample=d,
+            scale=2,
+            background=1e-5,
+            resolution_function=resolution_function,
+            name='newModel',
+        )
         assert_equal(mod.name, 'newModel')
         assert_equal(mod.interface, None)
         assert_equal(mod.sample.name, 'myModel')
         assert_equal(mod.scale.display_name, 'scale')
         assert_equal(str(mod.scale.unit), 'dimensionless')
         assert_equal(mod.scale.value.value.magnitude, 2.0)
         assert_equal(mod.scale.min, 0.0)
@@ -70,83 +76,82 @@
         assert_equal(mod.scale.fixed, True)
         assert_equal(mod.background.display_name, 'background')
         assert_equal(str(mod.background.unit), 'dimensionless')
         assert_equal(mod.background.value.value.magnitude, 1.0e-5)
         assert_equal(mod.background.min, 0.0)
         assert_equal(mod.background.max, np.Inf)
         assert_equal(mod.background.fixed, True)
-        assert_equal(mod.resolution.display_name, 'resolution')
-        assert_equal(str(mod.resolution.unit), 'dimensionless')
-        assert_equal(mod.resolution.value.value.magnitude, 2.0)
-        assert_equal(mod.resolution.min, 0.0)
-        assert_equal(mod.resolution.max, 100.0)
-        assert_equal(mod.resolution.fixed, True)
+        assert mod._resolution_function([1]) == 2.0
+        assert mod._resolution_function([100]) == 2.0
 
     def test_add_item(self):
-        m1 = Material.from_pars(6.908, -0.278, 'Boron')
-        m2 = Material.from_pars(0.487, 0.000, 'Potassium')
-        l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
-        l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
-        ls1 = LayerCollection.from_pars(l1, l2, name='twoLayer1')
-        ls2 = LayerCollection.from_pars(l2, l1, name='twoLayer2')
-        o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
-        o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
-        surfactant = SurfactantLayer.default()
-        multilayer = Multilayer.default()
-        d = Sample.from_pars(o1, name='myModel')
-        mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel')
+        m1 = Material(6.908, -0.278, 'Boron')
+        m2 = Material(0.487, 0.000, 'Potassium')
+        l1 = Layer(m1, 5.0, 2.0, 'thinBoron')
+        l2 = Layer(m2, 50.0, 1.0, 'thickPotassium')
+        ls1 = LayerCollection(l1, l2, name='twoLayer1')
+        ls2 = LayerCollection(l2, l1, name='twoLayer2')
+        o1 = RepeatingMultilayer(ls1, 2.0, 'twoLayerItem1')
+        o2 = RepeatingMultilayer(ls2, 1.0, 'oneLayerItem2')
+        surfactant = SurfactantLayer()
+        multilayer = Multilayer()
+        d = Sample(o1, name='myModel')
+        resolution_function = percentage_fhwm_resolution_function(2.0)
+        mod = Model(d, 2, 1e-5, resolution_function, 'newModel')
         assert_equal(len(mod.sample), 1)
         mod.add_item(o2)
         assert_equal(len(mod.sample), 2)
         assert_equal(mod.sample[1].name, 'oneLayerItem2')
         assert_equal(issubclass(mod.sample[1].__class__, RepeatingMultilayer), True)
         mod.add_item(surfactant)
         assert_equal(len(mod.sample), 3)
         mod.add_item(multilayer)
         assert_equal(len(mod.sample), 4)
 
     def test_add_item_exception(self):
         # When
-        mod = Model.default()
+        mod = Model()
 
         # Then Expect
         with pytest.raises(ValueError):
             mod.add_item('not an assembly')
 
     def test_add_item_with_interface_refnx(self):
         interface = CalculatorFactory()
-        m1 = Material.from_pars(6.908, -0.278, 'Boron')
-        m2 = Material.from_pars(0.487, 0.000, 'Potassium')
-        l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
-        l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
-        ls1 = LayerCollection.from_pars(l1, l2, name='twoLayer1')
-        ls2 = LayerCollection.from_pars(l2, l1, name='twoLayer2')
-        o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
-        o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
-        d = Sample.from_pars(o1, name='myModel')
-        mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel', interface=interface)
+        m1 = Material(6.908, -0.278, 'Boron')
+        m2 = Material(0.487, 0.000, 'Potassium')
+        l1 = Layer(m1, 5.0, 2.0, 'thinBoron')
+        l2 = Layer(m2, 50.0, 1.0, 'thickPotassium')
+        ls1 = LayerCollection(l1, l2, name='twoLayer1')
+        ls2 = LayerCollection(l2, l1, name='twoLayer2')
+        o1 = RepeatingMultilayer(ls1, 2.0, 'twoLayerItem1')
+        o2 = RepeatingMultilayer(ls2, 1.0, 'oneLayerItem2')
+        d = Sample(o1, name='myModel')
+        resolution_function = percentage_fhwm_resolution_function(2.0)
+        mod = Model(d, 2, 1e-5, resolution_function, 'newModel', interface=interface)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 1)
         assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
         mod.add_item(o2)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 2)
         assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
 
     def test_add_item_with_interface_refl1d(self):
         interface = CalculatorFactory()
         interface.switch('refl1d')
-        m1 = Material.from_pars(6.908, -0.278, 'Boron')
-        m2 = Material.from_pars(0.487, 0.000, 'Potassium')
-        l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
-        l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
-        ls1 = LayerCollection.from_pars(l1, l2, name='twoLayer1')
-        ls2 = LayerCollection.from_pars(l2, l1, name='twoLayer2')
-        o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
-        o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
-        d = Sample.from_pars(o1, name='myModel')
-        mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel', interface=interface)
+        m1 = Material(6.908, -0.278, 'Boron')
+        m2 = Material(0.487, 0.000, 'Potassium')
+        l1 = Layer(m1, 5.0, 2.0, 'thinBoron')
+        l2 = Layer(m2, 50.0, 1.0, 'thickPotassium')
+        ls1 = LayerCollection(l1, l2, name='twoLayer1')
+        ls2 = LayerCollection(l2, l1, name='twoLayer2')
+        o1 = RepeatingMultilayer(ls1, 2.0, 'twoLayerItem1')
+        o2 = RepeatingMultilayer(ls2, 1.0, 'oneLayerItem2')
+        d = Sample(o1, name='myModel')
+        resolution_function = percentage_fhwm_resolution_function(2.0)
+        mod = Model(d, 2, 1e-5, resolution_function, 'newModel', interface=interface)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 1)
         assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
         mod.add_item(o2)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 2)
         assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
 
     # def test_add_item_with_interface_bornagain(self):
@@ -157,71 +162,74 @@
     #     l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
     #     l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
     #     ls1 = Layers.from_pars(l1, l2, name='twoLayer1')
     #     ls2 = Layers.from_pars(l2, l1, name='twoLayer2')
     #     o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
     #     o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
     #     d = Sample.from_pars(o1, name='myModel')
-    #     mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel', interface=interface)
+    #     mod = Model(d, 2, 1e-5, 2.0, 'newModel', interface=interface)
     #     assert_equal(len(mod.interface()._wrapper.storage['item']), 1)
     #     assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
     #     mod.add_item(o2)
     #     assert_equal(len(mod.interface()._wrapper.storage['item']), 2)
     #     assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
 
     def test_duplicate_item(self):
-        m1 = Material.from_pars(6.908, -0.278, 'Boron')
-        m2 = Material.from_pars(0.487, 0.000, 'Potassium')
-        l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
-        l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
-        ls1 = LayerCollection.from_pars(l1, l2, name='twoLayer1')
-        ls2 = LayerCollection.from_pars(l2, l1, name='twoLayer2')
-        o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
-        o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
-        d = Sample.from_pars(o1, name='myModel')
-        mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel')
+        m1 = Material(6.908, -0.278, 'Boron')
+        m2 = Material(0.487, 0.000, 'Potassium')
+        l1 = Layer(m1, 5.0, 2.0, 'thinBoron')
+        l2 = Layer(m2, 50.0, 1.0, 'thickPotassium')
+        ls1 = LayerCollection(l1, l2, name='twoLayer1')
+        ls2 = LayerCollection(l2, l1, name='twoLayer2')
+        o1 = RepeatingMultilayer(ls1, 2.0, 'twoLayerItem1')
+        o2 = RepeatingMultilayer(ls2, 1.0, 'oneLayerItem2')
+        d = Sample(o1, name='myModel')
+        resolution_function = percentage_fhwm_resolution_function(2.0)
+        mod = Model(d, 2, 1e-5, resolution_function, 'newModel')
         assert_equal(len(mod.sample), 1)
         mod.add_item(o2)
         assert_equal(len(mod.sample), 2)
         mod.duplicate_item(1)
         assert_equal(len(mod.sample), 3)
         assert_equal(mod.sample[2].name, 'oneLayerItem2 duplicate')
         assert_equal(issubclass(mod.sample[2].__class__, RepeatingMultilayer), True)
 
     def test_duplicate_item_with_interface_refnx(self):
         interface = CalculatorFactory()
-        m1 = Material.from_pars(6.908, -0.278, 'Boron')
-        m2 = Material.from_pars(0.487, 0.000, 'Potassium')
-        l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
-        l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
-        ls1 = LayerCollection.from_pars(l1, l2, name='twoLayer1')
-        ls2 = LayerCollection.from_pars(l2, l1, name='twoLayer2')
-        o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
-        o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
-        d = Sample.from_pars(o1, name='myModel')
-        mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel', interface=interface)
+        m1 = Material(6.908, -0.278, 'Boron')
+        m2 = Material(0.487, 0.000, 'Potassium')
+        l1 = Layer(m1, 5.0, 2.0, 'thinBoron')
+        l2 = Layer(m2, 50.0, 1.0, 'thickPotassium')
+        ls1 = LayerCollection(l1, l2, name='twoLayer1')
+        ls2 = LayerCollection(l2, l1, name='twoLayer2')
+        o1 = RepeatingMultilayer(ls1, 2.0, 'twoLayerItem1')
+        o2 = RepeatingMultilayer(ls2, 1.0, 'oneLayerItem2')
+        d = Sample(o1, name='myModel')
+        resolution_function = percentage_fhwm_resolution_function(2.0)
+        mod = Model(d, 2, 1e-5, resolution_function, 'newModel', interface=interface)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 1)
         mod.add_item(o2)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 2)
         mod.duplicate_item(1)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 3)
 
     def test_duplicate_item_with_interface_refl1d(self):
         interface = CalculatorFactory()
         interface.switch('refl1d')
-        m1 = Material.from_pars(6.908, -0.278, 'Boron')
-        m2 = Material.from_pars(0.487, 0.000, 'Potassium')
-        l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
-        l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
-        ls1 = LayerCollection.from_pars(l1, l2, name='twoLayer1')
-        ls2 = LayerCollection.from_pars(l2, l1, name='twoLayer2')
-        o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
-        o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
-        d = Sample.from_pars(o1, name='myModel')
-        mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel', interface=interface)
+        m1 = Material(6.908, -0.278, 'Boron')
+        m2 = Material(0.487, 0.000, 'Potassium')
+        l1 = Layer(m1, 5.0, 2.0, 'thinBoron')
+        l2 = Layer(m2, 50.0, 1.0, 'thickPotassium')
+        ls1 = LayerCollection(l1, l2, name='twoLayer1')
+        ls2 = LayerCollection(l2, l1, name='twoLayer2')
+        o1 = RepeatingMultilayer(ls1, 2.0, 'twoLayerItem1')
+        o2 = RepeatingMultilayer(ls2, 1.0, 'oneLayerItem2')
+        d = Sample(o1, name='myModel')
+        resolution_function = percentage_fhwm_resolution_function(2.0)
+        mod = Model(d, 2, 1e-5, resolution_function, 'newModel', interface=interface)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 1)
         mod.add_item(o2)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 2)
         mod.duplicate_item(1)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 3)
 
     # def test_duplicate_item_with_interface_bornagain(self):
@@ -232,72 +240,75 @@
     #     l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
     #     l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
     #     ls1 = Layers.from_pars(l1, l2, name='twoLayer1')
     #     ls2 = Layers.from_pars(l2, l1, name='twoLayer2')
     #     o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
     #     o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
     #     d = Sample.from_pars(o1, name='myModel')
-    #     mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel', interface=interface)
+    #     mod = Model(d, 2, 1e-5, 2.0, 'newModel', interface=interface)
     #     assert_equal(len(mod.interface()._wrapper.storage['item']), 1)
     #     mod.add_item(o2)
     #     assert_equal(len(mod.interface()._wrapper.storage['item']), 2)
     #     mod.duplicate_item(1)
     #     assert_equal(len(mod.interface()._wrapper.storage['item']), 3)
 
     def test_remove_item(self):
-        m1 = Material.from_pars(6.908, -0.278, 'Boron')
-        m2 = Material.from_pars(0.487, 0.000, 'Potassium')
-        l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
-        l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
-        ls1 = LayerCollection.from_pars(l1, l2, name='twoLayer1')
-        ls2 = LayerCollection.from_pars(l2, l1, name='twoLayer2')
-        o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
-        o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
-        d = Sample.from_pars(o1, name='myModel')
-        mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel')
+        m1 = Material(6.908, -0.278, 'Boron')
+        m2 = Material(0.487, 0.000, 'Potassium')
+        l1 = Layer(m1, 5.0, 2.0, 'thinBoron')
+        l2 = Layer(m2, 50.0, 1.0, 'thickPotassium')
+        ls1 = LayerCollection(l1, l2, name='twoLayer1')
+        ls2 = LayerCollection(l2, l1, name='twoLayer2')
+        o1 = RepeatingMultilayer(ls1, 2.0, 'twoLayerItem1')
+        o2 = RepeatingMultilayer(ls2, 1.0, 'oneLayerItem2')
+        d = Sample(o1, name='myModel')
+        resolution_function = percentage_fhwm_resolution_function(2.0)
+        mod = Model(d, 2, 1e-5, resolution_function, 'newModel')
         assert_equal(len(mod.sample), 1)
         mod.add_item(o2)
         assert_equal(len(mod.sample), 2)
         mod.remove_item(0)
         assert_equal(len(mod.sample), 1)
 
     def test_remove_item_with_interface_refnx(self):
         interface = CalculatorFactory()
-        m1 = Material.from_pars(6.908, -0.278, 'Boron')
-        m2 = Material.from_pars(0.487, 0.000, 'Potassium')
-        l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
-        l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
-        ls1 = LayerCollection.from_pars(l1, l2, name='twoLayer1')
-        ls2 = LayerCollection.from_pars(l2, l1, name='twoLayer2')
-        o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
-        o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
-        d = Sample.from_pars(o1, name='myModel')
-        mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel', interface=interface)
+        m1 = Material(6.908, -0.278, 'Boron')
+        m2 = Material(0.487, 0.000, 'Potassium')
+        l1 = Layer(m1, 5.0, 2.0, 'thinBoron')
+        l2 = Layer(m2, 50.0, 1.0, 'thickPotassium')
+        ls1 = LayerCollection(l1, l2, name='twoLayer1')
+        ls2 = LayerCollection(l2, l1, name='twoLayer2')
+        o1 = RepeatingMultilayer(ls1, 2.0, 'twoLayerItem1')
+        o2 = RepeatingMultilayer(ls2, 1.0, 'oneLayerItem2')
+        d = Sample(o1, name='myModel')
+        resolution_function = percentage_fhwm_resolution_function(2.0)
+        mod = Model(d, 2, 1e-5, resolution_function, 'newModel', interface=interface)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 1)
         assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
         mod.add_item(o2)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 2)
         assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
         mod.remove_item(0)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 1)
         assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
 
     def test_remove_item_with_interface_refl1d(self):
         interface = CalculatorFactory()
         interface.switch('refl1d')
-        m1 = Material.from_pars(6.908, -0.278, 'Boron')
-        m2 = Material.from_pars(0.487, 0.000, 'Potassium')
-        l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
-        l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
-        ls1 = LayerCollection.from_pars(l1, l2, name='twoLayer1')
-        ls2 = LayerCollection.from_pars(l2, l1, name='twoLayer2')
-        o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
-        o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
-        d = Sample.from_pars(o1, name='myModel')
-        mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel', interface=interface)
+        m1 = Material(6.908, -0.278, 'Boron')
+        m2 = Material(0.487, 0.000, 'Potassium')
+        l1 = Layer(m1, 5.0, 2.0, 'thinBoron')
+        l2 = Layer(m2, 50.0, 1.0, 'thickPotassium')
+        ls1 = LayerCollection(l1, l2, name='twoLayer1')
+        ls2 = LayerCollection(l2, l1, name='twoLayer2')
+        o1 = RepeatingMultilayer(ls1, 2.0, 'twoLayerItem1')
+        o2 = RepeatingMultilayer(ls2, 1.0, 'oneLayerItem2')
+        d = Sample(o1, name='myModel')
+        resolution_function = percentage_fhwm_resolution_function(2.0)
+        mod = Model(d, 2, 1e-5, resolution_function, 'newModel', interface=interface)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 1)
         assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
         mod.add_item(o2)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 2)
         assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
         mod.remove_item(0)
         assert_equal(len(mod.interface()._wrapper.storage['item']), 1)
@@ -311,40 +322,94 @@
     #     l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
     #     l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
     #     ls1 = Layers.from_pars(l1, l2, name='twoLayer1')
     #     ls2 = Layers.from_pars(l2, l1, name='twoLayer2')
     #     o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
     #     o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
     #     d = Sample.from_pars(o1, name='myModel')
-    #     mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel', interface=interface)
+    #     mod = Model(d, 2, 1e-5, 2.0, 'newModel', interface=interface)
     #     assert_equal(len(mod.interface()._wrapper.storage['item']), 1)
     #     assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
     #     mod.add_item(o2)
     #     assert_equal(len(mod.interface()._wrapper.storage['item']), 2)
     #     assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
     #     mod.remove_item(0)
     #     assert_equal(len(mod.interface()._wrapper.storage['item']), 1)
     #     assert_equal(len(mod.interface()._wrapper.storage['layer']), 2)
 
     def test_uid(self):
-        p = Model.default()
+        p = Model()
         assert_equal(p.uid, p._borg.map.convert_id_to_key(p))
 
+    def test_resolution_function(self):
+        mock_resolution_function = MagicMock()
+        interface = CalculatorFactory()
+        interface.switch('refl1d')
+        model = Model(interface=interface)
+
+        # Then
+        model.resolution_function = mock_resolution_function
+
+        # Expect
+        assert model.resolution_function == mock_resolution_function
+
+    def test_resolution_function_interface_refl1d(self):
+        mock_resolution_function = MagicMock()
+        interface = CalculatorFactory()
+        interface.switch('refl1d')
+        model = Model(interface=interface)
+
+        # Then
+        model.resolution_function = mock_resolution_function
+
+        # Expect
+        assert model.interface()._wrapper._resolution_function == mock_resolution_function
+
+    def test_set_resolution_function_interface_refnx(self):
+        mock_resolution_function = MagicMock()
+        interface = CalculatorFactory()
+        interface.switch('refnx')
+        model = Model(interface=interface)
+
+        # Then
+        model.resolution_function = mock_resolution_function
+
+        # Expect
+        assert model.interface()._wrapper._resolution_function == mock_resolution_function
+
     def test_repr(self):
-        p = Model.default()
+        model = Model()
+
         assert (
-            p.__repr__()
+            model.__repr__()
             == 'EasyModel:\n  scale: 1.0\n  background: 1.0e-08\n  resolution: 5.0 %\n  sample:\n    EasySample:\n    - EasyMultilayer:\n        EasyLayers:\n        - EasyLayer:\n            material:\n              EasyMaterial:\n                sld: 4.186e-6 1 / angstrom ** 2\n                isld: 0.000e-6 1 / angstrom ** 2\n            thickness: 10.000 angstrom\n            roughness: 3.300 angstrom\n        - EasyLayer:\n            material:\n              EasyMaterial:\n                sld: 4.186e-6 1 / angstrom ** 2\n                isld: 0.000e-6 1 / angstrom ** 2\n            thickness: 10.000 angstrom\n            roughness: 3.300 angstrom\n    - EasyMultilayer:\n        EasyLayers:\n        - EasyLayer:\n            material:\n              EasyMaterial:\n                sld: 4.186e-6 1 / angstrom ** 2\n                isld: 0.000e-6 1 / angstrom ** 2\n            thickness: 10.000 angstrom\n            roughness: 3.300 angstrom\n        - EasyLayer:\n            material:\n              EasyMaterial:\n                sld: 4.186e-6 1 / angstrom ** 2\n                isld: 0.000e-6 1 / angstrom ** 2\n            thickness: 10.000 angstrom\n            roughness: 3.300 angstrom\n'  # noqa: E501
         )
 
+    def test_repr_resolution_function(self):
+        resolution_function = linear_spline_resolution_function([0, 10], [0, 10])
+        model = Model()
+        model.resolution_function = resolution_function
+        assert (
+            model.__repr__()
+            == 'EasyModel:\n  scale: 1.0\n  background: 1.0e-08\n  resolution: function of Q\n  sample:\n    EasySample:\n    - EasyMultilayer:\n        EasyLayers:\n        - EasyLayer:\n            material:\n              EasyMaterial:\n                sld: 4.186e-6 1 / angstrom ** 2\n                isld: 0.000e-6 1 / angstrom ** 2\n            thickness: 10.000 angstrom\n            roughness: 3.300 angstrom\n        - EasyLayer:\n            material:\n              EasyMaterial:\n                sld: 4.186e-6 1 / angstrom ** 2\n                isld: 0.000e-6 1 / angstrom ** 2\n            thickness: 10.000 angstrom\n            roughness: 3.300 angstrom\n    - EasyMultilayer:\n        EasyLayers:\n        - EasyLayer:\n            material:\n              EasyMaterial:\n                sld: 4.186e-6 1 / angstrom ** 2\n                isld: 0.000e-6 1 / angstrom ** 2\n            thickness: 10.000 angstrom\n            roughness: 3.300 angstrom\n        - EasyLayer:\n            material:\n              EasyMaterial:\n                sld: 4.186e-6 1 / angstrom ** 2\n                isld: 0.000e-6 1 / angstrom ** 2\n            thickness: 10.000 angstrom\n            roughness: 3.300 angstrom\n'  # noqa: E501
+        )
+
     def test_dict_round_trip(self):
+        # When
+        resolution_function = linear_spline_resolution_function([0, 10], [0, 10])
         interface = CalculatorFactory()
-        p = Model.default(interface)
-        surfactant = SurfactantLayer.default()
-        p.add_item(surfactant)
-        multilayer = Multilayer.default()
-        p.add_item(multilayer)
-        repeating = RepeatingMultilayer.default()
-        p.add_item(repeating)
-        src_dict = p.as_dict()
-        q = Model.from_dict(src_dict)
-        assert p.as_data_dict() == q.as_data_dict()
+        model = Model(interface=interface)
+        model.resolution_function = resolution_function
+        surfactant = SurfactantLayer()
+        model.add_item(surfactant)
+        multilayer = Multilayer()
+        model.add_item(multilayer)
+        repeating = RepeatingMultilayer()
+        model.add_item(repeating)
+        src_dict = model.as_dict()
+
+        # Then
+        model_from_dict = Model.from_dict(src_dict)
+
+        # Expect
+        assert model.as_data_dict() == model_from_dict.as_data_dict()
+        assert model._resolution_function(5.5) == model_from_dict._resolution_function(5.5)
```

### Comparing `easyreflectometrylib-0.0.6/tests/sample/test_sample.py` & `easyreflectometrylib-0.0.7/tests/sample/test_sample.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,62 +16,66 @@
 from EasyReflectometry.sample import RepeatingMultilayer
 from EasyReflectometry.sample import Sample
 from EasyReflectometry.sample import SurfactantLayer
 
 
 class TestSample(unittest.TestCase):
     def test_default(self):
-        p = Sample.default()
+        p = Sample()
         assert_equal(p.name, 'EasySample')
         assert_equal(p.interface, None)
         assert_equal(p[0].name, 'EasyMultilayer')
         assert_equal(p[1].name, 'EasyMultilayer')
 
     def test_from_pars(self):
-        m1 = Material.from_pars(6.908, -0.278, 'Boron')
-        m2 = Material.from_pars(0.487, 0.000, 'Potassium')
-        l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
-        l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
-        ls1 = LayerCollection.from_pars(l1, l2, name='twoLayer1')
-        ls2 = LayerCollection.from_pars(l2, l1, name='twoLayer2')
-        o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
-        o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
-        d = Sample.from_pars(o1, o2, name='myModel')
+        m1 = Material(6.908, -0.278, 'Boron')
+        m2 = Material(0.487, 0.000, 'Potassium')
+        l1 = Layer(m1, 5.0, 2.0, 'thinBoron')
+        l2 = Layer(m2, 50.0, 1.0, 'thickPotassium')
+        ls1 = LayerCollection(l1, l2, name='twoLayer1')
+        ls2 = LayerCollection(l2, l1, name='twoLayer2')
+        o1 = RepeatingMultilayer(ls1, 2.0, 'twoLayerItem1')
+        o2 = RepeatingMultilayer(ls2, 1.0, 'oneLayerItem2')
+        d = Sample(o1, o2, name='myModel')
         assert_equal(d.name, 'myModel')
         assert_equal(d.interface, None)
         assert_equal(d[0].name, 'twoLayerItem1')
         assert_equal(d[1].name, 'oneLayerItem2')
 
     def test_from_pars_layers(self):
-        m1 = Material.from_pars(6.908, -0.278, 'Boron')
-        m2 = Material.from_pars(0.487, 0.000, 'Potassium')
-        l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
-        l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
-        d = Sample.from_pars(l1, l2, name='myModel')
+        m1 = Material(6.908, -0.278, 'Boron')
+        m2 = Material(0.487, 0.000, 'Potassium')
+        l1 = Layer(m1, 5.0, 2.0, 'thinBoron')
+        l2 = Layer(m2, 50.0, 1.0, 'thickPotassium')
+        d = Sample(l1, l2, name='myModel')
         assert_equal(d.name, 'myModel')
         assert_equal(d.interface, None)
         assert_equal(d[0].name, 'thinBoron')
         assert_equal(d[1].name, 'thickPotassium')
 
     def test_from_pars_error(self):
-        m1 = Material.from_pars(6.908, -0.278, 'Boron')
+        m1 = Material(6.908, -0.278, 'Boron')
         with self.assertRaises(ValueError):
-            _ = Sample.from_pars(m1, name='myModel')
+            _ = Sample(m1, name='myModel')
 
     def test_repr(self):
-        p = Sample.default()
+        p = Sample()
         assert (
             p.__repr__()
             == 'EasySample:\n- EasyMultilayer:\n    EasyLayers:\n    - EasyLayer:\n        material:\n          EasyMaterial:\n            sld: 4.186e-6 1 / angstrom ** 2\n            isld: 0.000e-6 1 / angstrom ** 2\n        thickness: 10.000 angstrom\n        roughness: 3.300 angstrom\n    - EasyLayer:\n        material:\n          EasyMaterial:\n            sld: 4.186e-6 1 / angstrom ** 2\n            isld: 0.000e-6 1 / angstrom ** 2\n        thickness: 10.000 angstrom\n        roughness: 3.300 angstrom\n- EasyMultilayer:\n    EasyLayers:\n    - EasyLayer:\n        material:\n          EasyMaterial:\n            sld: 4.186e-6 1 / angstrom ** 2\n            isld: 0.000e-6 1 / angstrom ** 2\n        thickness: 10.000 angstrom\n        roughness: 3.300 angstrom\n    - EasyLayer:\n        material:\n          EasyMaterial:\n            sld: 4.186e-6 1 / angstrom ** 2\n            isld: 0.000e-6 1 / angstrom ** 2\n        thickness: 10.000 angstrom\n        roughness: 3.300 angstrom\n'  # noqa: E501
         )
 
     def test_dict_round_trip(self):
-        p = Sample.default()
-        surfactant = SurfactantLayer.default()
+        # When
+        p = Sample()
+        surfactant = SurfactantLayer()
         p.append(surfactant)
-        multilayer = Multilayer.default()
+        multilayer = Multilayer()
         p.append(multilayer)
-        repeating = RepeatingMultilayer.default()
+        repeating = RepeatingMultilayer()
         p.append(repeating)
 
+        # Then
         q = Sample.from_dict(p.as_dict())
+
+        # Expect
         assert p.as_data_dict() == q.as_data_dict()
```

### Comparing `easyreflectometrylib-0.0.6/tests/sample/assemblies/test_base_assembly.py` & `easyreflectometrylib-0.0.7/tests/sample/assemblies/test_base_assembly.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/tests/sample/assemblies/test_gradient_layer.py` & `easyreflectometrylib-0.0.7/tests/sample/assemblies/test_gradient_layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from EasyReflectometry.sample.assemblies.gradient_layer import _prepare_gradient_layers
 from EasyReflectometry.sample.elements.materials.material import Material
 
 
 class TestGradientLayer:
     @pytest.fixture
     def gradient_layer(self) -> GradientLayer:
-        self.front = Material.from_pars(10.0, -10.0, 'Material_1')
-        self.back = Material.from_pars(0.0, 0.0, 'Material_2')
+        self.front = Material(10.0, -10.0, 'Material_1')
+        self.back = Material(0.0, 0.0, 'Material_2')
 
         return GradientLayer(
             front_material=self.front,
             back_material=self.back,
             thickness=1.0,
             roughness=2.0,
             discretisation_elements=10,
@@ -44,29 +44,29 @@
         assert gradient_layer.back_layer.material.sld.raw_value == 1.0
         assert gradient_layer.front_layer.material.isld.raw_value == -10.0
         assert gradient_layer.layers[5].material.isld.raw_value == -5.0
         assert gradient_layer.back_layer.material.isld.raw_value == -1.0
 
     def test_default(self) -> None:
         # When Then
-        result = GradientLayer.default('default-layer')
+        result = GradientLayer(name='default-layer')
 
         # Expect
         assert result.name == 'default-layer'
         assert result._type, 'Gradient-layer'
         assert result.interface is None
         assert len(result.layers) == 10
 
     def test_from_pars(self) -> None:
         # When
-        front = Material.from_pars(6.908, -0.278, 'Boron')
-        back = Material.from_pars(0.487, 0.000, 'Potassium')
+        front = Material(6.908, -0.278, 'Boron')
+        back = Material(0.487, 0.000, 'Potassium')
 
         # Then
-        result = GradientLayer.from_pars(
+        result = GradientLayer(
             front_material=front,
             back_material=back,
             thickness=10.0,
             roughness=1.0,
             discretisation_elements=5,
             name='gradientItem',
         )
@@ -154,34 +154,33 @@
 
 def test_prepare_gradient_layers(monkeypatch):
     # When
     mock_material_1 = MagicMock()
     mock_material_2 = MagicMock()
     mock_Layer = MagicMock()
     mock_LayerCollection = MagicMock()
-    mock_Material = MagicMock()
-    mock_Material.from_pars = MagicMock(return_value='Material_from_pars')
+    mock_Material = MagicMock(return_value='Material_from_mock')
     mock_linear_gradient = MagicMock(return_value=[1.0, 2.0, 3.0])
     monkeypatch.setattr(EasyReflectometry.sample.assemblies.gradient_layer, '_linear_gradient', mock_linear_gradient)
     monkeypatch.setattr(EasyReflectometry.sample.assemblies.gradient_layer, 'Layer', mock_Layer)
     monkeypatch.setattr(EasyReflectometry.sample.assemblies.gradient_layer, 'Material', mock_Material)
     monkeypatch.setattr(EasyReflectometry.sample.assemblies.gradient_layer, 'LayerCollection', mock_LayerCollection)
 
     # Then
     _prepare_gradient_layers(mock_material_1, mock_material_2, 3, None)
 
     # When
-    assert mock_Material.from_pars.call_count == 3
-    assert mock_Material.from_pars.call_args_list[0][0] == (1.0, 1.0)
-    assert mock_Material.from_pars.call_args_list[1][0] == (2.0, 2.0)
-    assert mock_Material.from_pars.call_args_list[2][0] == (3.0, 3.0)
-    assert mock_Layer.from_pars.call_count == 3
-    assert mock_Layer.from_pars.call_args_list[0][1]['material'] == 'Material_from_pars'
-    assert mock_Layer.from_pars.call_args_list[0][1]['thickness'] == 0.0
-    assert mock_Layer.from_pars.call_args_list[0][1]['name'] == '0'
-    assert mock_Layer.from_pars.call_args_list[0][1]['interface'] is None
+    assert mock_Material.call_count == 3
+    assert mock_Material.call_args_list[0][0] == (1.0, 1.0)
+    assert mock_Material.call_args_list[1][0] == (2.0, 2.0)
+    assert mock_Material.call_args_list[2][0] == (3.0, 3.0)
+    assert mock_Layer.call_count == 3
+    assert mock_Layer.call_args_list[0][1]['material'] == 'Material_from_mock'
+    assert mock_Layer.call_args_list[0][1]['thickness'] == 0.0
+    assert mock_Layer.call_args_list[0][1]['name'] == '0'
+    assert mock_Layer.call_args_list[0][1]['interface'] is None
 
 
 def test_dict_round_trip():
-    p = GradientLayer.default()
+    p = GradientLayer()
     q = GradientLayer.from_dict(p.as_dict())
     assert p.as_data_dict() == q.as_data_dict()
```

### Comparing `easyreflectometrylib-0.0.6/tests/sample/assemblies/test_multilayer.py` & `easyreflectometrylib-0.0.7/tests/sample/assemblies/test_repeating_multilayer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,111 +1,133 @@
 """
-Tests for MultiLayer class module
+Tests for RepeatingMultiLayer module
 """
 
 __author__ = 'github.com/arm61'
 __version__ = '0.0.1'
 
+
 import unittest
 
 from numpy.testing import assert_equal
 from numpy.testing import assert_raises
 
-from EasyReflectometry.calculators.factory import CalculatorFactory
-from EasyReflectometry.sample.assemblies.multilayer import Multilayer
+from EasyReflectometry.calculators import CalculatorFactory
+from EasyReflectometry.sample.assemblies.repeating_multilayer import RepeatingMultilayer
 from EasyReflectometry.sample.elements.layers.layer import Layer
 from EasyReflectometry.sample.elements.layers.layer_collection import LayerCollection
 from EasyReflectometry.sample.elements.materials.material import Material
 
 
-class TestMultilayer(unittest.TestCase):
+class TestRepeatingMultilayer(unittest.TestCase):
     def test_default(self):
-        p = Multilayer.default()
-        assert_equal(p.name, 'EasyMultilayer')
-        assert_equal(p._type, 'Multi-layer')
+        p = RepeatingMultilayer()
+        assert_equal(p.name, 'EasyRepeatingMultilayer')
+        assert_equal(p._type, 'Repeating Multi-layer')
         assert_equal(p.interface, None)
         assert_equal(len(p.layers), 2)
+        assert_equal(p.repetitions.display_name, 'repetitions')
+        assert_equal(str(p.repetitions.unit), 'dimensionless')
+        assert_equal(p.repetitions.value.value.magnitude, 1.0)
+        assert_equal(p.repetitions.min, 1)
+        assert_equal(p.repetitions.max, 9999)
+        assert_equal(p.repetitions.fixed, True)
         assert_equal(p.layers.name, 'EasyLayers')
 
     def test_from_pars(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        k = Material.from_pars(0.487, 0.000, 'Potassium')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium')
-        layers = LayerCollection.from_pars(p, q, name='twoLayer')
-        o = Multilayer.from_pars(layers, 'twoLayerItem')
+        m = Material(6.908, -0.278, 'Boron')
+        k = Material(0.487, 0.000, 'Potassium')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        q = Layer(k, 50.0, 1.0, 'thickPotassium')
+        layers = LayerCollection(p, q, name='twoLayer')
+        o = RepeatingMultilayer(layers, 2.0, 'twoLayerItem')
         assert_equal(o.name, 'twoLayerItem')
-        assert_equal(o._type, 'Multi-layer')
+        assert_equal(o._type, 'Repeating Multi-layer')
         assert_equal(o.interface, None)
+        assert_equal(o.repetitions.display_name, 'repetitions')
+        assert_equal(str(o.repetitions.unit), 'dimensionless')
+        assert_equal(o.repetitions.value.value.magnitude, 2.0)
+        assert_equal(o.repetitions.min, 1)
+        assert_equal(o.repetitions.max, 9999)
+        assert_equal(o.repetitions.fixed, True)
         assert_equal(o.layers.name, 'twoLayer')
 
     def test_from_pars_layer(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        o = Multilayer.from_pars(p, 'twoLayerItem')
+        m = Material(6.908, -0.278, 'Boron')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        o = RepeatingMultilayer(p, 2.0, 'twoLayerItem')
         assert_equal(o.name, 'twoLayerItem')
         assert_equal(o.interface, None)
+        assert_equal(o.repetitions.display_name, 'repetitions')
+        assert_equal(str(o.repetitions.unit), 'dimensionless')
+        assert_equal(o.repetitions.value.value.magnitude, 2.0)
+        assert_equal(o.repetitions.min, 1)
+        assert_equal(o.repetitions.max, 9999)
+        assert_equal(o.repetitions.fixed, True)
         assert_equal(o.layers.name, 'thinBoron')
 
     def test_from_pars_layer_list(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        k = Material.from_pars(0.487, 0.000, 'Potassium')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        q = Layer.from_pars(k, 15.0, 2.0, 'layerPotassium')
-        o = Multilayer.from_pars([p, q], 'twoLayerItem')
+        m = Material(6.908, -0.278, 'Boron')
+        k = Material(0.487, 0.000, 'Potassium')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        q = Layer(k, 15.0, 2.0, 'layerPotassium')
+        o = RepeatingMultilayer([p, q], 10, 'twoLayerItem')
         assert_equal(o.name, 'twoLayerItem')
         assert_equal(o.interface, None)
         assert_equal(o.layers.name, 'thinBoron/layerPotassium')
+        assert_equal(o.repetitions.value.value.magnitude, 10.0)
+        assert_equal(o.repetitions.min, 1)
+        assert_equal(o.repetitions.max, 9999)
 
     def test_add_layer(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        k = Material.from_pars(0.487, 0.000, 'Potassium')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium')
-        o = Multilayer.from_pars(p, 'twoLayerItem')
+        m = Material(6.908, -0.278, 'Boron')
+        k = Material(0.487, 0.000, 'Potassium')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        q = Layer(k, 50.0, 1.0, 'thickPotassium')
+        o = RepeatingMultilayer(p, 2.0, 'twoLayerItem')
         assert_equal(len(o.layers), 1)
         o.add_layer(q)
         assert_equal(len(o.layers), 2)
         assert_equal(o.layers[1].name, 'thickPotassium')
 
     def test_add_layer_with_interface_refnx(self):
         interface = CalculatorFactory()
         interface.switch('refnx')
-        m = Material.from_pars(6.908, -0.278, 'Boron', interface=interface)
-        k = Material.from_pars(0.487, 0.000, 'Potassium', interface=interface)
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron', interface=interface)
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium', interface=interface)
-        o = Multilayer.from_pars(p, 'twoLayerItem', interface=interface)
+        m = Material(6.908, -0.278, 'Boron', interface=interface)
+        k = Material(0.487, 0.000, 'Potassium', interface=interface)
+        p = Layer(m, 5.0, 2.0, 'thinBoron', interface=interface)
+        q = Layer(k, 50.0, 1.0, 'thickPotassium', interface=interface)
+        o = RepeatingMultilayer(p, 2.0, 'twoLayerItem', interface=interface)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 1)
         o.add_layer(q)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 2)
         assert_equal(o.interface()._wrapper.storage['item'][o.uid].components[1].thick.value, 50.0)
 
     def test_duplicate_layer(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        k = Material.from_pars(0.487, 0.000, 'Potassium')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium')
-        o = Multilayer.from_pars(p, 'twoLayerItem')
+        m = Material(6.908, -0.278, 'Boron')
+        k = Material(0.487, 0.000, 'Potassium')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        q = Layer(k, 50.0, 1.0, 'thickPotassium')
+        o = RepeatingMultilayer(p, 2.0, 'twoLayerItem')
         assert_equal(len(o.layers), 1)
         o.add_layer(q)
         assert_equal(len(o.layers), 2)
         o.duplicate_layer(1)
         assert_equal(len(o.layers), 3)
         assert_equal(o.layers[1].name, 'thickPotassium')
         assert_equal(o.layers[2].name, 'thickPotassium duplicate')
 
     def test_duplicate_layer_with_interface_refnx(self):
         interface = CalculatorFactory()
         interface.switch('refnx')
-        m = Material.from_pars(6.908, -0.278, 'Boron', interface=interface)
-        k = Material.from_pars(0.487, 0.000, 'Potassium', interface=interface)
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron', interface=interface)
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium', interface=interface)
-        o = Multilayer.from_pars(p, 'twoLayerItem', interface=interface)
+        m = Material(6.908, -0.278, 'Boron', interface=interface)
+        k = Material(0.487, 0.000, 'Potassium', interface=interface)
+        p = Layer(m, 5.0, 2.0, 'thinBoron', interface=interface)
+        q = Layer(k, 50.0, 1.0, 'thickPotassium', interface=interface)
+        o = RepeatingMultilayer(p, 2.0, 'twoLayerItem', interface=interface)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 1)
         o.add_layer(q)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 2)
         assert_equal(o.interface()._wrapper.storage['item'][o.uid].components[1].thick.value, 50.0)
         o.duplicate_layer(1)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 3)
         assert_equal(o.interface()._wrapper.storage['item'][o.uid].components[2].thick.value, 50.0)
@@ -113,47 +135,47 @@
             AssertionError,
             assert_equal,
             o.interface()._wrapper.storage['item'][o.uid].components[1].name,
             o.interface()._wrapper.storage['item'][o.uid].components[2].name,
         )
 
     def test_remove_layer(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        k = Material.from_pars(0.487, 0.000, 'Potassium')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium')
-        o = Multilayer.from_pars(p, 'twoLayerItem')
+        m = Material(6.908, -0.278, 'Boron')
+        k = Material(0.487, 0.000, 'Potassium')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        q = Layer(k, 50.0, 1.0, 'thickPotassium')
+        o = RepeatingMultilayer(p, 2.0, 'twoLayerItem')
         assert_equal(len(o.layers), 1)
         o.add_layer(q)
         assert_equal(len(o.layers), 2)
         assert_equal(o.layers[1].name, 'thickPotassium')
         o.remove_layer(1)
         assert_equal(len(o.layers), 1)
         assert_equal(o.layers[0].name, 'thinBoron')
 
     def test_remove_layer_with_interface_refnx(self):
         interface = CalculatorFactory()
         interface.switch('refnx')
-        m = Material.from_pars(6.908, -0.278, 'Boron', interface=interface)
-        k = Material.from_pars(0.487, 0.000, 'Potassium', interface=interface)
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron', interface=interface)
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium', interface=interface)
-        o = Multilayer.from_pars(p, name='twoLayerItem', interface=interface)
+        m = Material(6.908, -0.278, 'Boron', interface=interface)
+        k = Material(0.487, 0.000, 'Potassium', interface=interface)
+        p = Layer(m, 5.0, 2.0, 'thinBoron', interface=interface)
+        q = Layer(k, 50.0, 1.0, 'thickPotassium', interface=interface)
+        o = RepeatingMultilayer(p, repetitions=2.0, name='twoLayerItem', interface=interface)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 1)
         o.add_layer(q)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 2)
         assert_equal(o.layers[1].name, 'thickPotassium')
         o.remove_layer(1)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 1)
         assert_equal(o.layers[0].name, 'thinBoron')
 
     def test_repr(self):
-        p = Multilayer.default()
+        p = RepeatingMultilayer()
         assert (
             p.__repr__()
-            == 'EasyMultilayer:\n  EasyLayers:\n  - EasyLayer:\n      material:\n        EasyMaterial:\n          sld: 4.186e-6 1 / angstrom ** 2\n          isld: 0.000e-6 1 / angstrom ** 2\n      thickness: 10.000 angstrom\n      roughness: 3.300 angstrom\n  - EasyLayer:\n      material:\n        EasyMaterial:\n          sld: 4.186e-6 1 / angstrom ** 2\n          isld: 0.000e-6 1 / angstrom ** 2\n      thickness: 10.000 angstrom\n      roughness: 3.300 angstrom\n'  # noqa: E501
+            == 'EasyRepeatingMultilayer:\n  EasyLayers:\n  - EasyLayer:\n      material:\n        EasyMaterial:\n          sld: 4.186e-6 1 / angstrom ** 2\n          isld: 0.000e-6 1 / angstrom ** 2\n      thickness: 10.000 angstrom\n      roughness: 3.300 angstrom\n  - EasyLayer:\n      material:\n        EasyMaterial:\n          sld: 4.186e-6 1 / angstrom ** 2\n          isld: 0.000e-6 1 / angstrom ** 2\n      thickness: 10.000 angstrom\n      roughness: 3.300 angstrom\n  repetitions: 1.0\n'  # noqa: E501
         )
 
     def test_dict_round_trip(self):
-        p = Multilayer.default()
-        q = Multilayer.from_dict(p.as_dict())
+        p = RepeatingMultilayer()
+        q = RepeatingMultilayer.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
```

### Comparing `easyreflectometrylib-0.0.6/tests/sample/assemblies/test_repeating_multilayer.py` & `easyreflectometrylib-0.0.7/tests/sample/assemblies/test_multilayer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,133 +1,111 @@
 """
-Tests for RepeatingMultiLayer module
+Tests for MultiLayer class module
 """
 
 __author__ = 'github.com/arm61'
 __version__ = '0.0.1'
 
-
 import unittest
 
 from numpy.testing import assert_equal
 from numpy.testing import assert_raises
 
-from EasyReflectometry.calculators import CalculatorFactory
-from EasyReflectometry.sample.assemblies.repeating_multilayer import RepeatingMultilayer
+from EasyReflectometry.calculators.factory import CalculatorFactory
+from EasyReflectometry.sample.assemblies.multilayer import Multilayer
 from EasyReflectometry.sample.elements.layers.layer import Layer
 from EasyReflectometry.sample.elements.layers.layer_collection import LayerCollection
 from EasyReflectometry.sample.elements.materials.material import Material
 
 
-class TestRepeatingMultilayer(unittest.TestCase):
+class TestMultilayer(unittest.TestCase):
     def test_default(self):
-        p = RepeatingMultilayer.default()
-        assert_equal(p.name, 'EasyRepeatingMultilayer')
-        assert_equal(p._type, 'Repeating Multi-layer')
+        p = Multilayer()
+        assert_equal(p.name, 'EasyMultilayer')
+        assert_equal(p._type, 'Multi-layer')
         assert_equal(p.interface, None)
         assert_equal(len(p.layers), 2)
-        assert_equal(p.repetitions.display_name, 'repetitions')
-        assert_equal(str(p.repetitions.unit), 'dimensionless')
-        assert_equal(p.repetitions.value.value.magnitude, 1.0)
-        assert_equal(p.repetitions.min, 1)
-        assert_equal(p.repetitions.max, 9999)
-        assert_equal(p.repetitions.fixed, True)
         assert_equal(p.layers.name, 'EasyLayers')
 
     def test_from_pars(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        k = Material.from_pars(0.487, 0.000, 'Potassium')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium')
-        layers = LayerCollection.from_pars(p, q, name='twoLayer')
-        o = RepeatingMultilayer.from_pars(layers, 2.0, 'twoLayerItem')
+        m = Material(6.908, -0.278, 'Boron')
+        k = Material(0.487, 0.000, 'Potassium')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        q = Layer(k, 50.0, 1.0, 'thickPotassium')
+        layers = LayerCollection(p, q, name='twoLayer')
+        o = Multilayer(layers, 'twoLayerItem')
         assert_equal(o.name, 'twoLayerItem')
-        assert_equal(o._type, 'Repeating Multi-layer')
+        assert_equal(o._type, 'Multi-layer')
         assert_equal(o.interface, None)
-        assert_equal(o.repetitions.display_name, 'repetitions')
-        assert_equal(str(o.repetitions.unit), 'dimensionless')
-        assert_equal(o.repetitions.value.value.magnitude, 2.0)
-        assert_equal(o.repetitions.min, 1)
-        assert_equal(o.repetitions.max, 9999)
-        assert_equal(o.repetitions.fixed, True)
         assert_equal(o.layers.name, 'twoLayer')
 
     def test_from_pars_layer(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        o = RepeatingMultilayer.from_pars(p, 2.0, 'twoLayerItem')
+        m = Material(6.908, -0.278, 'Boron')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        o = Multilayer(p, 'twoLayerItem')
         assert_equal(o.name, 'twoLayerItem')
         assert_equal(o.interface, None)
-        assert_equal(o.repetitions.display_name, 'repetitions')
-        assert_equal(str(o.repetitions.unit), 'dimensionless')
-        assert_equal(o.repetitions.value.value.magnitude, 2.0)
-        assert_equal(o.repetitions.min, 1)
-        assert_equal(o.repetitions.max, 9999)
-        assert_equal(o.repetitions.fixed, True)
         assert_equal(o.layers.name, 'thinBoron')
 
     def test_from_pars_layer_list(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        k = Material.from_pars(0.487, 0.000, 'Potassium')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        q = Layer.from_pars(k, 15.0, 2.0, 'layerPotassium')
-        o = RepeatingMultilayer.from_pars([p, q], 10, 'twoLayerItem')
+        m = Material(6.908, -0.278, 'Boron')
+        k = Material(0.487, 0.000, 'Potassium')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        q = Layer(k, 15.0, 2.0, 'layerPotassium')
+        o = Multilayer([p, q], 'twoLayerItem')
         assert_equal(o.name, 'twoLayerItem')
         assert_equal(o.interface, None)
         assert_equal(o.layers.name, 'thinBoron/layerPotassium')
-        assert_equal(o.repetitions.value.value.magnitude, 10.0)
-        assert_equal(o.repetitions.min, 1)
-        assert_equal(o.repetitions.max, 9999)
 
     def test_add_layer(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        k = Material.from_pars(0.487, 0.000, 'Potassium')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium')
-        o = RepeatingMultilayer.from_pars(p, 2.0, 'twoLayerItem')
+        m = Material(6.908, -0.278, 'Boron')
+        k = Material(0.487, 0.000, 'Potassium')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        q = Layer(k, 50.0, 1.0, 'thickPotassium')
+        o = Multilayer(p, 'twoLayerItem')
         assert_equal(len(o.layers), 1)
         o.add_layer(q)
         assert_equal(len(o.layers), 2)
         assert_equal(o.layers[1].name, 'thickPotassium')
 
     def test_add_layer_with_interface_refnx(self):
         interface = CalculatorFactory()
         interface.switch('refnx')
-        m = Material.from_pars(6.908, -0.278, 'Boron', interface=interface)
-        k = Material.from_pars(0.487, 0.000, 'Potassium', interface=interface)
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron', interface=interface)
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium', interface=interface)
-        o = RepeatingMultilayer.from_pars(p, 2.0, 'twoLayerItem', interface=interface)
+        m = Material(6.908, -0.278, 'Boron', interface=interface)
+        k = Material(0.487, 0.000, 'Potassium', interface=interface)
+        p = Layer(m, 5.0, 2.0, 'thinBoron', interface=interface)
+        q = Layer(k, 50.0, 1.0, 'thickPotassium', interface=interface)
+        o = Multilayer(p, 'twoLayerItem', interface=interface)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 1)
         o.add_layer(q)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 2)
         assert_equal(o.interface()._wrapper.storage['item'][o.uid].components[1].thick.value, 50.0)
 
     def test_duplicate_layer(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        k = Material.from_pars(0.487, 0.000, 'Potassium')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium')
-        o = RepeatingMultilayer.from_pars(p, 2.0, 'twoLayerItem')
+        m = Material(6.908, -0.278, 'Boron')
+        k = Material(0.487, 0.000, 'Potassium')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        q = Layer(k, 50.0, 1.0, 'thickPotassium')
+        o = Multilayer(p, 'twoLayerItem')
         assert_equal(len(o.layers), 1)
         o.add_layer(q)
         assert_equal(len(o.layers), 2)
         o.duplicate_layer(1)
         assert_equal(len(o.layers), 3)
         assert_equal(o.layers[1].name, 'thickPotassium')
         assert_equal(o.layers[2].name, 'thickPotassium duplicate')
 
     def test_duplicate_layer_with_interface_refnx(self):
         interface = CalculatorFactory()
         interface.switch('refnx')
-        m = Material.from_pars(6.908, -0.278, 'Boron', interface=interface)
-        k = Material.from_pars(0.487, 0.000, 'Potassium', interface=interface)
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron', interface=interface)
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium', interface=interface)
-        o = RepeatingMultilayer.from_pars(p, 2.0, 'twoLayerItem', interface=interface)
+        m = Material(6.908, -0.278, 'Boron', interface=interface)
+        k = Material(0.487, 0.000, 'Potassium', interface=interface)
+        p = Layer(m, 5.0, 2.0, 'thinBoron', interface=interface)
+        q = Layer(k, 50.0, 1.0, 'thickPotassium', interface=interface)
+        o = Multilayer(p, 'twoLayerItem', interface=interface)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 1)
         o.add_layer(q)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 2)
         assert_equal(o.interface()._wrapper.storage['item'][o.uid].components[1].thick.value, 50.0)
         o.duplicate_layer(1)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 3)
         assert_equal(o.interface()._wrapper.storage['item'][o.uid].components[2].thick.value, 50.0)
@@ -135,47 +113,47 @@
             AssertionError,
             assert_equal,
             o.interface()._wrapper.storage['item'][o.uid].components[1].name,
             o.interface()._wrapper.storage['item'][o.uid].components[2].name,
         )
 
     def test_remove_layer(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        k = Material.from_pars(0.487, 0.000, 'Potassium')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium')
-        o = RepeatingMultilayer.from_pars(p, 2.0, 'twoLayerItem')
+        m = Material(6.908, -0.278, 'Boron')
+        k = Material(0.487, 0.000, 'Potassium')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        q = Layer(k, 50.0, 1.0, 'thickPotassium')
+        o = Multilayer(p, 'twoLayerItem')
         assert_equal(len(o.layers), 1)
         o.add_layer(q)
         assert_equal(len(o.layers), 2)
         assert_equal(o.layers[1].name, 'thickPotassium')
         o.remove_layer(1)
         assert_equal(len(o.layers), 1)
         assert_equal(o.layers[0].name, 'thinBoron')
 
     def test_remove_layer_with_interface_refnx(self):
         interface = CalculatorFactory()
         interface.switch('refnx')
-        m = Material.from_pars(6.908, -0.278, 'Boron', interface=interface)
-        k = Material.from_pars(0.487, 0.000, 'Potassium', interface=interface)
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron', interface=interface)
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium', interface=interface)
-        o = RepeatingMultilayer.from_pars(p, repetitions=2.0, name='twoLayerItem', interface=interface)
+        m = Material(6.908, -0.278, 'Boron', interface=interface)
+        k = Material(0.487, 0.000, 'Potassium', interface=interface)
+        p = Layer(m, 5.0, 2.0, 'thinBoron', interface=interface)
+        q = Layer(k, 50.0, 1.0, 'thickPotassium', interface=interface)
+        o = Multilayer(p, name='twoLayerItem', interface=interface)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 1)
         o.add_layer(q)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 2)
         assert_equal(o.layers[1].name, 'thickPotassium')
         o.remove_layer(1)
         assert_equal(len(o.interface()._wrapper.storage['item'][o.uid].components), 1)
         assert_equal(o.layers[0].name, 'thinBoron')
 
     def test_repr(self):
-        p = RepeatingMultilayer.default()
+        p = Multilayer()
         assert (
             p.__repr__()
-            == 'EasyRepeatingMultilayer:\n  EasyLayers:\n  - EasyLayer:\n      material:\n        EasyMaterial:\n          sld: 4.186e-6 1 / angstrom ** 2\n          isld: 0.000e-6 1 / angstrom ** 2\n      thickness: 10.000 angstrom\n      roughness: 3.300 angstrom\n  - EasyLayer:\n      material:\n        EasyMaterial:\n          sld: 4.186e-6 1 / angstrom ** 2\n          isld: 0.000e-6 1 / angstrom ** 2\n      thickness: 10.000 angstrom\n      roughness: 3.300 angstrom\n  repetitions: 1.0\n'  # noqa: E501
+            == 'EasyMultilayer:\n  EasyLayers:\n  - EasyLayer:\n      material:\n        EasyMaterial:\n          sld: 4.186e-6 1 / angstrom ** 2\n          isld: 0.000e-6 1 / angstrom ** 2\n      thickness: 10.000 angstrom\n      roughness: 3.300 angstrom\n  - EasyLayer:\n      material:\n        EasyMaterial:\n          sld: 4.186e-6 1 / angstrom ** 2\n          isld: 0.000e-6 1 / angstrom ** 2\n      thickness: 10.000 angstrom\n      roughness: 3.300 angstrom\n'  # noqa: E501
         )
 
     def test_dict_round_trip(self):
-        p = RepeatingMultilayer.default()
-        q = RepeatingMultilayer.from_dict(p.as_dict())
+        p = Multilayer()
+        q = Multilayer.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
```

### Comparing `easyreflectometrylib-0.0.6/tests/sample/assemblies/test_surfactant_layer.py` & `easyreflectometrylib-0.0.7/tests/sample/assemblies/test_surfactant_layer.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,31 +11,32 @@
 from EasyReflectometry.sample.assemblies.surfactant_layer import SurfactantLayer
 from EasyReflectometry.sample.elements.layers.layer import Layer
 from EasyReflectometry.sample.elements.materials.material import Material
 
 
 class TestSurfactantLayer(unittest.TestCase):
     def test_default(self):
-        p = SurfactantLayer.default()
+        p = SurfactantLayer()
         assert p.name == 'EasySurfactantLayer'
         assert p._type == 'Surfactant Layer'
 
         assert p.layers[0].name == 'DPPC Tail'
         assert p.front_layer.name == 'DPPC Tail'
         assert p.tail_layer.name == 'DPPC Tail'
         assert p.tail_layer.molecular_formula == 'C32D64'
 
         assert p.layers[1].name == 'DPPC Head'
         assert p.back_layer.name == 'DPPC Head'
         assert p.head_layer.name == 'DPPC Head'
         assert p.head_layer.molecular_formula == 'C10H18NO8P'
 
+    @unittest.skip('It is no longer possible to create a surfactant layer without specifying the materials.')
     def test_from_pars(self):
-        h2o = Material.from_pars(-0.561, 0, 'H2O')
-        noth2o = Material.from_pars(0.561, 0, 'nH2O')
+        h2o = Material(-0.561, 0, 'H2O')
+        noth2o = Material(0.561, 0, 'nH2O')
         p = SurfactantLayer.from_pars('C8O10H12P', 12, h2o, 0.5, 50, 2, 'C10H24', 10, noth2o, 0.2, 40, 3, name='A Test')
         assert p.layers[0].name == 'A Test Tail Layer'
         assert p.tail_layer.name == 'A Test Tail Layer'
         assert p.tail_layer.molecular_formula == 'C8O10H12P'
         assert p.tail_layer.thickness.raw_value == 12
         assert p.tail_layer.solvent.as_data_dict() == h2o.as_data_dict()
         assert p.tail_layer.solvent_fraction == 0.5
@@ -47,43 +48,43 @@
         assert p.head_layer.thickness.raw_value == 10
         assert p.head_layer.solvent.as_data_dict() == noth2o.as_data_dict()
         assert p.head_layer.solvent_fraction == 0.2
         assert p.head_layer.area_per_molecule == 40
         assert p.name == 'A Test'
 
     def test_constraint_area_per_molecule(self):
-        p = SurfactantLayer.default()
+        p = SurfactantLayer()
         p.tail_layer._area_per_molecule.value = 30
         assert p.tail_layer.area_per_molecule == 30.0
         assert p.head_layer.area_per_molecule == 48.2
         assert p.constrain_area_per_molecule is False
         p.constrain_area_per_molecule = True
         assert p.tail_layer.area_per_molecule == 30
         assert p.head_layer.area_per_molecule == 30
         assert p.constrain_area_per_molecule is True
         p.tail_layer._area_per_molecule.value = 40
         assert p.tail_layer.area_per_molecule == 40
         assert p.head_layer.area_per_molecule == 40
 
     def test_conformal_roughness(self):
-        p = SurfactantLayer.default()
+        p = SurfactantLayer()
         p.tail_layer.roughness.value = 2
         assert p.tail_layer.roughness.raw_value == 2
         assert p.head_layer.roughness.raw_value == 3
         p.conformal_roughness = True
         assert p.tail_layer.roughness.raw_value == 2
         assert p.head_layer.roughness.raw_value == 2
         assert p.conformal_roughness is True
         p.tail_layer.roughness.value = 4
         assert p.tail_layer.roughness.raw_value == 4
         assert p.head_layer.roughness.raw_value == 4
 
     def test_constain_solvent_roughness(self):
-        p = SurfactantLayer.default()
-        layer = Layer.default()
+        p = SurfactantLayer()
+        layer = Layer()
         p.tail_layer.roughness.value = 2
         assert p.tail_layer.roughness.raw_value == 2
         assert p.head_layer.roughness.raw_value == 3
         assert layer.roughness.raw_value == 3.3
         p.conformal_roughness = True
         p.constrain_solvent_roughness(layer.roughness)
         assert p.tail_layer.roughness.raw_value == 2
@@ -92,15 +93,15 @@
         assert p.conformal_roughness is True
         p.tail_layer.roughness.value = 4
         assert p.tail_layer.roughness.raw_value == 4
         assert p.head_layer.roughness.raw_value == 4
         assert layer.roughness.raw_value == 4
 
     def test_dict_repr(self):
-        p = SurfactantLayer.default()
+        p = SurfactantLayer()
         assert p._dict_repr == {
             'EasySurfactantLayer': {
                 'head_layer': {
                     'DPPC Head': {
                         'material': {
                             'C10H18NO8P in D2O': {
                                 'solvent_fraction': '0.200 dimensionless',
@@ -144,77 +145,77 @@
                 'area per molecule constrained': False,
                 'conformal roughness': False,
             }
         }
 
     def test_get_head_layer(self):
         # When
-        p = SurfactantLayer.default()
+        p = SurfactantLayer()
 
         # Then Expect
         assert p.head_layer == p.back_layer
         assert p.head_layer == p.layers[1]
 
     def test_set_head_layer(self):
         # When
-        p = SurfactantLayer.default()
-        new_layer = Layer.default()
+        p = SurfactantLayer()
+        new_layer = Layer()
 
         # Then
         p.head_layer = new_layer
 
         # Expect
         assert p.head_layer == new_layer
         assert p.back_layer == new_layer
         assert p.layers[1] == new_layer
 
     def test_get_tail_layer(self):
         # When
-        p = SurfactantLayer.default()
+        p = SurfactantLayer()
 
         # Then Expect
         assert p.tail_layer == p.front_layer
         assert p.tail_layer == p.layers[0]
 
     def test_set_tail_layer(self):
         # When
-        p = SurfactantLayer.default()
-        new_layer = Layer.default()
+        p = SurfactantLayer()
+        new_layer = Layer()
 
         # Then
         p.tail_layer = new_layer
 
         # Expect
         assert p.tail_layer == new_layer
         assert p.front_layer == new_layer
         assert p.layers[0] == new_layer
 
     def test_dict_round_trip(self):
-        p = SurfactantLayer.default()
+        p = SurfactantLayer()
         q = SurfactantLayer.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
 
     def test_dict_round_trip_area_per_molecule_constraint_enabled(self):
-        p = SurfactantLayer.default()
+        p = SurfactantLayer()
         p.constrain_area_per_molecule = True
         q = SurfactantLayer.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
 
     def test_dict_round_trip_area_per_molecule_constraint_disabled(self):
-        p = SurfactantLayer.default()
+        p = SurfactantLayer()
         p.constrain_area_per_molecule = True
         p.constrain_area_per_molecule = False
         q = SurfactantLayer.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
 
     def test_dict_round_trip_roughness_constraint_enabled(self):
-        p = SurfactantLayer.default()
+        p = SurfactantLayer()
         p.conformal_roughness = True
         q = SurfactantLayer.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
 
     def test_dict_round_trip_roughness_constraint_disabled(self):
-        p = SurfactantLayer.default()
+        p = SurfactantLayer()
         p.conformal_roughness = True
         p.conformal_roughness = False
         q = SurfactantLayer.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
```

### Comparing `easyreflectometrylib-0.0.6/tests/sample/elements/test_layer_collection.py` & `easyreflectometrylib-0.0.7/tests/sample/elements/layers/test_layer_collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,43 +13,43 @@
 from EasyReflectometry.sample.elements.layers.layer import Layer
 from EasyReflectometry.sample.elements.layers.layer_collection import LayerCollection
 from EasyReflectometry.sample.elements.materials.material import Material
 
 
 class TestLayerCollection(unittest.TestCase):
     def test_default(self):
-        p = LayerCollection.default()
+        p = LayerCollection()
         assert_equal(p.name, 'EasyLayers')
         assert_equal(p.interface, None)
         assert_equal(len(p), 2)
         assert_equal(p[0].name, 'EasyLayer')
         assert_equal(p[1].name, 'EasyLayer')
 
     def test_from_pars(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        k = Material.from_pars(0.487, 0.000, 'Potassium')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        q = Layer.from_pars(k, 50.0, 1.0, 'thickPotassium')
-        layers = LayerCollection.from_pars(p, q, name='twoLayer')
+        m = Material(6.908, -0.278, 'Boron')
+        k = Material(0.487, 0.000, 'Potassium')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        q = Layer(k, 50.0, 1.0, 'thickPotassium')
+        layers = LayerCollection(p, q, name='twoLayer')
         assert_equal(layers.name, 'twoLayer')
         assert_equal(layers.interface, None)
         assert_equal(len(layers), 2)
         assert_equal(layers[0].name, 'thinBoron')
         assert_equal(layers[1].name, 'thickPotassium')
 
     def test_from_pars_item(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        i = RepeatingMultilayer.from_pars(LayerCollection.default(), 2)
-        layers = LayerCollection.from_pars(p, i, name='twoLayer')
+        m = Material(6.908, -0.278, 'Boron')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        i = RepeatingMultilayer(LayerCollection(), 2)
+        layers = LayerCollection(p, i, name='twoLayer')
         assert_equal(layers.name, 'twoLayer')
         assert_equal(layers.interface, None)
 
     def test_dict_repr(self):
-        p = LayerCollection.default()
+        p = LayerCollection()
         assert p._dict_repr == {
             'EasyLayers': [
                 {
                     'EasyLayer': {
                         'material': {
                             'EasyMaterial': {'sld': '4.186e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}
                         },
@@ -66,17 +66,28 @@
                         'roughness': '3.300 angstrom',
                     }
                 },
             ]
         }
 
     def test_repr(self):
-        p = LayerCollection.default()
+        p = LayerCollection()
         assert (
             p.__repr__()
             == 'EasyLayers:\n- EasyLayer:\n    material:\n      EasyMaterial:\n        sld: 4.186e-6 1 / angstrom ** 2\n        isld: 0.000e-6 1 / angstrom ** 2\n    thickness: 10.000 angstrom\n    roughness: 3.300 angstrom\n- EasyLayer:\n    material:\n      EasyMaterial:\n        sld: 4.186e-6 1 / angstrom ** 2\n        isld: 0.000e-6 1 / angstrom ** 2\n    thickness: 10.000 angstrom\n    roughness: 3.300 angstrom\n'  # noqa: E501
         )
 
     def test_dict_round_trip(self):
-        p = LayerCollection.default()
-        q = LayerCollection.from_dict(p.as_dict())
-        assert p.as_data_dict() == q.as_data_dict()
+        # When
+        m = Material(6.908, -0.278, 'Boron')
+        k = Material(0.487, 0.000, 'Potassium')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        q = Layer(k, 50.0, 1.0, 'thickPotassium')
+        r = LayerCollection()
+        r.insert(0, p)
+        r.append(q)
+
+        # Then
+        s = LayerCollection.from_dict(r.as_dict())
+
+        # Expect
+        assert s.as_data_dict() == r.as_data_dict()
```

### Comparing `easyreflectometrylib-0.0.6/tests/sample/elements/layers/test_layer.py` & `easyreflectometrylib-0.0.7/tests/sample/elements/layers/test_layer.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 import unittest
 
 import numpy as np
 from numpy.testing import assert_almost_equal
 from numpy.testing import assert_equal
 
 from EasyReflectometry.calculators.factory import CalculatorFactory
+from EasyReflectometry.parameter_utils import get_as_parameter
+from EasyReflectometry.sample.elements.layers.layer import DEFAULTS
 from EasyReflectometry.sample.elements.layers.layer import Layer
 from EasyReflectometry.sample.elements.materials.material import Material
 
 
 class TestLayer(unittest.TestCase):
-    def test_default(self):
-        p = Layer.default()
+    def test_no_arguments(self):
+        p = Layer()
         assert_equal(p.name, 'EasyLayer')
         assert_equal(p.interface, None)
         assert_equal(p.material.name, 'EasyMaterial')
         assert_equal(p.thickness.display_name, 'thickness')
         assert_equal(str(p.thickness.unit), 'angstrom')
         assert_equal(p.thickness.value.value.magnitude, 10.0)
         assert_equal(p.thickness.min, 0.0)
@@ -31,17 +33,17 @@
         assert_equal(p.roughness.display_name, 'roughness')
         assert_equal(str(p.roughness.unit), 'angstrom')
         assert_equal(p.roughness.value.value.magnitude, 3.3)
         assert_equal(p.roughness.min, 0.0)
         assert_equal(p.roughness.max, np.Inf)
         assert_equal(p.roughness.fixed, True)
 
-    def test_from_pars(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
+    def test_shuffled_arguments(self):
+        m = Material(6.908, -0.278, 'Boron')
+        p = Layer(thickness=5.0, material=m, roughness=2.0, name='thinBoron')
         assert_equal(p.name, 'thinBoron')
         assert_equal(p.interface, None)
         assert_equal(p.material.name, 'Boron')
         assert_equal(p.thickness.display_name, 'thickness')
         assert_equal(str(p.thickness.unit), 'angstrom')
         assert_equal(p.thickness.value.value.magnitude, 5.0)
         assert_equal(p.thickness.min, 0.0)
@@ -50,49 +52,81 @@
         assert_equal(p.roughness.display_name, 'roughness')
         assert_equal(str(p.roughness.unit), 'angstrom')
         assert_equal(p.roughness.value.value.magnitude, 2.0)
         assert_equal(p.roughness.min, 0.0)
         assert_equal(p.roughness.max, np.Inf)
         assert_equal(p.roughness.fixed, True)
 
+    def test_only_roughness_key(self):
+        p = Layer(roughness=10.0)
+        assert_equal(p.roughness.display_name, 'roughness')
+        assert_equal(str(p.roughness.unit), 'angstrom')
+        assert_equal(p.roughness.value.value.magnitude, 10.0)
+        assert_equal(p.roughness.min, 0.0)
+        assert_equal(p.roughness.max, np.Inf)
+        assert_equal(p.roughness.fixed, True)
+
+    def test_only_roughness_key_paramter(self):
+        roughness = get_as_parameter('roughness', 10, DEFAULTS)
+        roughness.min = -10.0
+        p = Layer(roughness=roughness)
+        assert_equal(p.roughness.value.value.magnitude, 10.0)
+        assert_equal(p.roughness.min, -10.0)
+
+    def test_only_thickness_key(self):
+        p = Layer(thickness=10.0)
+        assert_equal(p.thickness.display_name, 'thickness')
+        assert_equal(str(p.thickness.unit), 'angstrom')
+        assert_equal(p.thickness.value.value.magnitude, 10.0)
+        assert_equal(p.thickness.min, 0.0)
+        assert_equal(p.thickness.max, np.Inf)
+        assert_equal(p.thickness.fixed, True)
+
+    def test_only_thickness_key_paramter(self):
+        thickness = get_as_parameter('thickness', 10, DEFAULTS)
+        thickness.min = -10.0
+        p = Layer(thickness=thickness)
+        assert_equal(p.thickness.value.value.magnitude, 10.0)
+        assert_equal(p.thickness.min, -10.0)
+
     def test_assign_material(self):
-        m = Material.from_pars(6.908, -0.278, 'Boron')
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron')
-        k = Material.from_pars(2.074, 0.0, 'Silicon')
+        m = Material(6.908, -0.278, 'Boron')
+        p = Layer(m, 5.0, 2.0, 'thinBoron')
+        k = Material(2.074, 0.0, 'Silicon')
         assert_almost_equal(p.material.sld.raw_value, 6.908)
         assert_almost_equal(p.material.isld.raw_value, -0.278)
         p.assign_material(k)
         assert_almost_equal(p.material.sld.raw_value, 2.074)
         assert_almost_equal(p.material.isld.raw_value, 0.0)
 
     def test_assign_material_with_interface_refnx(self):
         interface = CalculatorFactory()
-        m = Material.from_pars(6.908, -0.278, 'Boron', interface=interface)
-        p = Layer.from_pars(m, 5.0, 2.0, 'thinBoron', interface=interface)
-        k = Material.from_pars(2.074, 0.0, 'Silicon', interface=interface)
+        m = Material(6.908, -0.278, 'Boron', interface=interface)
+        p = Layer(m, 5.0, 2.0, 'thinBoron', interface=interface)
+        k = Material(2.074, 0.0, 'Silicon', interface=interface)
         assert_almost_equal(p.interface()._wrapper.storage['layer'][p.uid].sld.real.value, 6.908)
         assert_almost_equal(p.interface()._wrapper.storage['layer'][p.uid].sld.imag.value, -0.278)
         p.assign_material(k)
         assert_almost_equal(p.interface()._wrapper.storage['layer'][p.uid].sld.real.value, 2.074)
         assert_almost_equal(p.interface()._wrapper.storage['layer'][p.uid].sld.imag.value, 0.0)
 
     def test_dict_repr(self):
-        p = Layer.default()
+        p = Layer()
         assert p._dict_repr == {
             'EasyLayer': {
                 'material': {'EasyMaterial': {'isld': '0.000e-6 1 / angstrom ** 2', 'sld': '4.186e-6 1 / angstrom ** 2'}},
                 'roughness': '3.300 angstrom',
                 'thickness': '10.000 angstrom',
             }
         }
 
     def test_repr(self):
-        p = Layer.default()
+        p = Layer()
         assert (
             p.__repr__()
             == 'EasyLayer:\n  material:\n    EasyMaterial:\n      sld: 4.186e-6 1 / angstrom ** 2\n      isld: 0.000e-6 1 / angstrom ** 2\n  thickness: 10.000 angstrom\n  roughness: 3.300 angstrom\n'  # noqa: E501
         )  # noqa: E501
 
     def test_dict_round_trip(self):
-        p = Layer.default()
+        p = Layer()
         q = Layer.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
```

### Comparing `easyreflectometrylib-0.0.6/tests/sample/elements/layers/test_layer_area_per_molecule.py` & `easyreflectometrylib-0.0.7/tests/sample/elements/layers/test_layer_area_per_molecule.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from EasyReflectometry.sample.elements.layers.layer_area_per_molecule import LayerAreaPerMolecule
 from EasyReflectometry.sample.elements.materials.material import Material
 
 
 class TestLayerAreaPerMolecule(unittest.TestCase):
     def test_default(self):
-        p = LayerAreaPerMolecule.default()
+        p = LayerAreaPerMolecule()
         assert p.molecular_formula == 'C10H18NO8P'
         assert p.area_per_molecule == 48.2
         assert str(p._area_per_molecule.unit) == 'angstrom ** 2'
         assert p._area_per_molecule.fixed is True
         assert p.thickness.raw_value == 10.0
         assert str(p.thickness.unit) == 'angstrom'
         assert p.thickness.fixed is True
@@ -30,16 +30,16 @@
         assert p.solvent.isld.raw_value == 0
         assert p.solvent.name == 'D2O'
         assert p.solvent_fraction == 0.2
         assert str(p.material._fraction.unit) == 'dimensionless'
         assert p.material._fraction.fixed is True
 
     def test_from_pars(self):
-        h2o = Material.from_pars(-0.561, 0, 'H2O')
-        p = LayerAreaPerMolecule.from_pars(
+        h2o = Material(-0.561, 0, 'H2O')
+        p = LayerAreaPerMolecule(
             molecular_formula='C8O10H12P',
             thickness=12,
             solvent=h2o,
             solvent_fraction=0.5,
             area_per_molecule=50,
             roughness=2,
             name='PG/H2O',
@@ -49,16 +49,16 @@
         assert p.thickness.raw_value == 12
         assert p.roughness.raw_value == 2
         assert p.solvent.sld.raw_value == -0.561
         assert p.solvent.isld.raw_value == 0
         assert p.solvent_fraction == 0.5
 
     def test_from_pars_constraint(self):
-        h2o = Material.from_pars(-0.561, 0, 'H2O')
-        p = LayerAreaPerMolecule.from_pars(
+        h2o = Material(-0.561, 0, 'H2O')
+        p = LayerAreaPerMolecule(
             molecular_formula='C8O10H12P',
             thickness=12,
             solvent=h2o,
             solvent_fraction=0.5,
             area_per_molecule=50,
             roughness=2,
             name='PG/H2O',
@@ -75,16 +75,16 @@
         assert p.area_per_molecule == 30
         assert_almost_equal(p.material.sld, 0.712227778)
         p.thickness.value = 10
         assert p.thickness.raw_value == 10
         assert_almost_equal(p.material.sld, 0.910773333)
 
     def test_solvent_change(self):
-        h2o = Material.from_pars(-0.561, 0, 'H2O')
-        p = LayerAreaPerMolecule.from_pars(
+        h2o = Material(-0.561, 0, 'H2O')
+        p = LayerAreaPerMolecule(
             molecular_formula='C8O10H12P',
             thickness=12,
             solvent=h2o,
             solvent_fraction=0.5,
             area_per_molecule=50,
             roughness=2,
             name='PG/H2O',
@@ -94,28 +94,28 @@
         print(p.material)
         assert_almost_equal(p.material.sld, 0.31513666667)
         assert p.thickness.raw_value == 12
         assert p.roughness.raw_value == 2
         assert p.solvent.sld.raw_value == -0.561
         assert p.solvent.isld.raw_value == 0
         assert p.solvent_fraction == 0.5
-        d2o = Material.from_pars(6.335, 0, 'D2O')
+        d2o = Material(6.335, 0, 'D2O')
         p.solvent = d2o
         assert p.molecular_formula == 'C8O10H12P'
         assert p.area_per_molecule == 50
         assert_almost_equal(p.material.sld, 3.7631366667)
         assert p.thickness.raw_value == 12
         assert p.roughness.raw_value == 2
         assert p.solvent.sld.raw_value == 6.335
         assert p.solvent.isld.raw_value == 0
         assert p.solvent_fraction == 0.5
 
     def test_molecular_formula_change(self):
-        h2o = Material.from_pars(-0.561, 0, 'H2O')
-        p = LayerAreaPerMolecule.from_pars(
+        h2o = Material(-0.561, 0, 'H2O')
+        p = LayerAreaPerMolecule(
             molecular_formula='C8O10H12P',
             thickness=12,
             solvent=h2o,
             solvent_fraction=0.5,
             area_per_molecule=50,
             roughness=2,
             name='PG/H2O',
@@ -138,15 +138,15 @@
         assert p.roughness.raw_value == 2
         assert p.solvent.sld.raw_value == -0.561
         assert p.solvent.isld.raw_value == 0
         assert p.solvent_fraction == 0.5
         assert p.material.name == 'C8O10D12P in H2O'
 
     def test_dict_repr(self):
-        p = LayerAreaPerMolecule.default()
+        p = LayerAreaPerMolecule()
         assert p._dict_repr == {
             'EasyLayerAreaPerMolecule': {
                 'material': {
                     'C10H18NO8P in D2O': {
                         'solvent_fraction': '0.200 dimensionless',
                         'sld': '2.269e-6 1 / angstrom ** 2',
                         'isld': '0.000e-6 1 / angstrom ** 2',
@@ -160,10 +160,10 @@
                 'roughness': '3.300 angstrom',
             },
             'molecular_formula': 'C10H18NO8P',
             'area_per_molecule': '48.20 angstrom ** 2',
         }
 
     def test_dict_round_trip(self):
-        p = LayerAreaPerMolecule.default()
+        p = LayerAreaPerMolecule()
         q = LayerAreaPerMolecule.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
```

### Comparing `easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material.py` & `easyreflectometrylib-0.0.7/tests/sample/elements/materials/test_material.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 __version__ = '0.0.1'
 
 
 import unittest
 
 import numpy as np
 
+from EasyReflectometry.parameter_utils import get_as_parameter
+from EasyReflectometry.sample.elements.materials.material import DEFAULTS
 from EasyReflectometry.sample.elements.materials.material import Material
 
 
 class TestMaterial(unittest.TestCase):
-    def test_default(self):
-        p = Material.default()
+    def test_no_arguments(self):
+        p = Material()
         assert p.name == 'EasyMaterial'
         assert p.interface is None
         assert p.sld.display_name == 'sld'
         assert str(p.sld.unit) == '1 / angstrom ** 2'
         assert p.sld.value.value.magnitude == 4.186
         assert p.sld.min == -np.Inf
         assert p.sld.max == np.Inf
@@ -27,16 +29,16 @@
         assert p.isld.display_name == 'isld'
         assert str(p.isld.unit) == '1 / angstrom ** 2'
         assert p.isld.value.value.magnitude == 0.0
         assert p.isld.min == -np.Inf
         assert p.isld.max == np.Inf
         assert p.isld.fixed is True
 
-    def test_from_pars(self):
-        p = Material.from_pars(6.908, -0.278, 'Boron')
+    def test_shuffled_arguments(self):
+        p = Material(name='Boron', sld=6.908, isld=-0.278)
         assert p.name == 'Boron'
         assert p.interface is None
         assert p.sld.display_name == 'sld'
         assert str(p.sld.unit) == '1 / angstrom ** 2'
         assert p.sld.value.value.magnitude == 6.908
         assert p.sld.min == -np.Inf
         assert p.sld.max == np.Inf
@@ -44,19 +46,51 @@
         assert p.isld.display_name == 'isld'
         assert str(p.isld.unit) == '1 / angstrom ** 2'
         assert p.isld.value.value.magnitude == -0.278
         assert p.isld.min == -np.Inf
         assert p.isld.max == np.Inf
         assert p.isld.fixed is True
 
+    def test_only_sld_key(self):
+        p = Material(sld=10)
+        assert p.sld.display_name == 'sld'
+        assert str(p.sld.unit) == '1 / angstrom ** 2'
+        assert p.sld.value.value.magnitude == 10
+        assert p.sld.min == -np.Inf
+        assert p.sld.max == np.Inf
+        assert p.sld.fixed is True
+
+    def test_only_sld_key_parameter(self):
+        sld = get_as_parameter('sld', 10, DEFAULTS)
+        sld.min = -10.0
+        p = Material(sld=sld)
+        assert p.sld.value.value.magnitude == 10
+        assert p.sld.min == -10
+
+    def test_only_isld_key(self):
+        p = Material(isld=10)
+        assert p.isld.display_name == 'isld'
+        assert str(p.isld.unit) == '1 / angstrom ** 2'
+        assert p.isld.value.value.magnitude == 10
+        assert p.isld.min == -np.Inf
+        assert p.isld.max == np.Inf
+        assert p.isld.fixed is True
+
+    def test_only_isld_key_parameter(self):
+        isld = get_as_parameter('isld', 10, DEFAULTS)
+        isld.min = -10.0
+        p = Material(isld=isld)
+        assert p.isld.value.value.magnitude == 10
+        assert p.isld.min == -10
+
     def test_dict_repr(self):
-        p = Material.default()
+        p = Material()
         assert p._dict_repr == {'EasyMaterial': {'sld': '4.186e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}}
 
     def test_repr(self):
-        p = Material.default()
+        p = Material()
         assert p.__repr__() == 'EasyMaterial:\n  sld: 4.186e-6 1 / angstrom ** 2\n  isld: 0.000e-6 1 / angstrom ** 2\n'
 
     def test_dict_round_trip(self):
-        p = Material.default()
+        p = Material()
         q = Material.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
```

### Comparing `easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material_density.py` & `easyreflectometrylib-0.0.7/tests/sample/elements/materials/test_material_density.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,55 +4,55 @@
 from numpy.testing import assert_almost_equal
 
 from EasyReflectometry.sample.elements.materials.material_density import MaterialDensity
 
 
 class TestMaterialDensity(unittest.TestCase):
     def test_default(self):
-        p = MaterialDensity.default()
+        p = MaterialDensity()
         assert p.name == 'EasyMaterialDensity'
         assert p.interface is None
         assert p.density.display_name == 'density'
         assert str(p.density.unit) == 'gram / centimeter ** 3'
         assert p.density.value.value.magnitude == 2.33
         assert p.density.min == 0
         assert p.density.max == np.Inf
         assert p.density.fixed is True
 
     def test_default_constraint(self):
-        p = MaterialDensity.default()
+        p = MaterialDensity()
         assert p.density.value.value.magnitude == 2.33
         assert_almost_equal(p.sld.value.value.magnitude, 2.073705382)
         p.density.value = 2
         assert_almost_equal(p.sld.value.value.magnitude, 1.780004619)
 
     def test_from_pars(self):
-        p = MaterialDensity.from_pars('Co', 8.9, 'Cobalt')
+        p = MaterialDensity('Co', 8.9, 'Cobalt')
         assert p.density.value.value.magnitude == 8.9
         assert_almost_equal(p.sld.value.value.magnitude, 2.2645412328256)
         assert p.chemical_structure == 'Co'
 
     def test_chemical_structure_change(self):
-        p = MaterialDensity.from_pars('Co', 8.9, 'Cobolt')
+        p = MaterialDensity('Co', 8.9, 'Cobolt')
         assert p.density.value.value.magnitude == 8.9
         assert_almost_equal(p.sld.value.value.magnitude, 2.2645412328256)
         assert_almost_equal(p.isld.value.value.magnitude, 0.0)
         assert p.chemical_structure == 'Co'
         p.chemical_structure = 'B'
         assert p.density.value.value.magnitude == 8.9
         assert_almost_equal(p.sld.value.value.magnitude, 4.820107844970)
         assert_almost_equal(p.isld.value.value.magnitude, -0.19098540517806603)
         assert p.chemical_structure == 'B'
 
     def test_dict_repr(self):
-        p = MaterialDensity.default()
+        p = MaterialDensity()
         print(p._dict_repr)
         assert p._dict_repr == {
             'EasyMaterialDensity': {'sld': '2.074e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'},
             'chemical_structure': 'Si',
             'density': '2.33e+00 gram / centimeter ** 3',
         }
 
     def test_dict_round_trip(self):
-        p = MaterialDensity.default()
+        p = MaterialDensity()
         q = MaterialDensity.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
```

### Comparing `easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material_mixture.py` & `easyreflectometrylib-0.0.7/tests/sample/elements/materials/test_material_mixture.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,125 +5,125 @@
 
 from EasyReflectometry.sample.elements.materials.material import Material
 from EasyReflectometry.sample.elements.materials.material_mixture import MaterialMixture
 
 
 class TestMaterialMixture(unittest.TestCase):
     def test_default(self):
-        p = MaterialMixture.default()
+        p = MaterialMixture()
         assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert p.sld == Material.default().sld.raw_value
-        assert p.isld == Material.default().isld.raw_value
+        assert p.sld == Material().sld.raw_value
+        assert p.isld == Material().isld.raw_value
         assert str(p._sld.unit) == '1 / angstrom ** 2'
         assert str(p._isld.unit) == '1 / angstrom ** 2'
 
     def test_default_constraint(self):
-        p = MaterialMixture.default()
+        p = MaterialMixture()
         assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert p.sld == Material.default().sld.raw_value
-        assert p.isld == Material.default().isld.raw_value
+        assert p.sld == Material().sld.raw_value
+        assert p.isld == Material().isld.raw_value
         p.material_a.sld.value = 0
         p.material_b.isld.value = -1
         assert_almost_equal(p.sld, 2.093)
         assert_almost_equal(p.isld, -0.5)
         assert str(p._sld.unit) == '1 / angstrom ** 2'
         assert str(p._isld.unit) == '1 / angstrom ** 2'
 
     def test_fraction_constraint(self):
-        p = Material.default()
-        q = Material.from_pars(6.908, -0.278, 'Boron')
-        r = MaterialMixture.from_pars(p, q, 0.2)
+        p = Material()
+        q = Material(6.908, -0.278, 'Boron')
+        r = MaterialMixture(p, q, 0.2)
         assert r.fraction == 0.2
         assert_almost_equal(r.sld, 4.7304)
         assert_almost_equal(r.isld, -0.0556)
         r._fraction.value = 0.5
         assert r.fraction == 0.5
         assert_almost_equal(r.sld, 5.54700)
         assert_almost_equal(r.isld, -0.1390)
 
     def test_material_a_change(self):
-        p = MaterialMixture.default()
+        p = MaterialMixture()
         assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert p.sld == Material.default().sld.raw_value
-        assert p.isld == Material.default().isld.raw_value
-        q = Material.from_pars(6.908, -0.278, 'Boron')
+        assert p.sld == Material().sld.raw_value
+        assert p.isld == Material().isld.raw_value
+        q = Material(6.908, -0.278, 'Boron')
         p.material_a = q
         assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
         assert_almost_equal(p.sld, 5.54700)
         assert_almost_equal(p.isld, -0.1390)
 
     def test_material_b_change(self):
-        p = MaterialMixture.default()
+        p = MaterialMixture()
         assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert p.sld == Material.default().sld.raw_value
-        assert p.isld == Material.default().isld.raw_value
-        q = Material.from_pars(6.908, -0.278, 'Boron')
+        assert p.sld == Material().sld.raw_value
+        assert p.isld == Material().isld.raw_value
+        q = Material(6.908, -0.278, 'Boron')
         p.material_b = q
         assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
         assert_almost_equal(p.sld, 5.54700)
         assert_almost_equal(p.isld, -0.1390)
 
     def test_material_b_change_double(self):
-        p = MaterialMixture.default()
+        p = MaterialMixture()
         assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert p.sld == Material.default().sld.raw_value
-        assert p.isld == Material.default().isld.raw_value
-        q = Material.from_pars(6.908, -0.278, 'Boron')
+        assert p.sld == Material().sld.raw_value
+        assert p.isld == Material().isld.raw_value
+        q = Material(6.908, -0.278, 'Boron')
         p.material_b = q
         assert p.name == 'EasyMaterial/Boron'
         assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
         assert_almost_equal(p.sld, 5.54700)
         assert_almost_equal(p.isld, -0.1390)
-        r = Material.from_pars(0.00, 0.00, 'ACMW')
+        r = Material(0.00, 0.00, 'ACMW')
         p.material_b = r
         assert p.name == 'EasyMaterial/ACMW'
         assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
         assert_almost_equal(p.sld, 2.0930)
         assert_almost_equal(p.isld, 0.0000)
 
     def test_from_pars(self):
-        p = Material.default()
-        q = Material.from_pars(6.908, -0.278, 'Boron')
-        r = MaterialMixture.from_pars(p, q, 0.2)
+        p = Material()
+        q = Material(6.908, -0.278, 'Boron')
+        r = MaterialMixture(p, q, 0.2)
         assert r.fraction == 0.2
         assert str(r._fraction.unit) == 'dimensionless'
         assert_almost_equal(r.sld, 4.7304)
         assert_almost_equal(r.isld, -0.0556)
         assert str(r._sld.unit) == '1 / angstrom ** 2'
         assert str(r._isld.unit) == '1 / angstrom ** 2'
 
     def test_dict_repr(self):
-        p = MaterialMixture.default()
+        p = MaterialMixture()
         assert p._dict_repr == {
             'EasyMaterial/EasyMaterial': {
                 'fraction': '0.500 dimensionless',
                 'sld': '4.186e-6 1 / angstrom ** 2',
                 'isld': '0.000e-6 1 / angstrom ** 2',
                 'material_a': {'EasyMaterial': {'sld': '4.186e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}},
                 'material_b': {'EasyMaterial': {'sld': '4.186e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}},
             }
         }
 
     def test_dict_round_trip(self):
-        p = MaterialMixture.default()
+        p = MaterialMixture()
         q = MaterialMixture.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
 
     def test_update_name(self):
         # When
-        p = MaterialMixture.default()
+        p = MaterialMixture()
         mock_material_a = MagicMock()
         mock_material_a.name = 'name_a'
         p._material_a = mock_material_a
         mock_material_b = MagicMock()
         mock_material_b.name = 'name_b'
         p._material_b = mock_material_b
```

### Comparing `easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material_solvated.py` & `easyreflectometrylib-0.0.7/tests/sample/elements/materials/test_material_solvated.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from unittest.mock import MagicMock
 
 import pytest
+from easyCore.Objects.ObjectClasses import Parameter
 
 import EasyReflectometry.sample.elements.materials.material_mixture
 import EasyReflectometry.sample.elements.materials.material_solvated
+from EasyReflectometry.sample.elements.materials.material import Material
 from EasyReflectometry.sample.elements.materials.material_solvated import MaterialSolvated
 
 
 class TestMaterialSolvated:
     @pytest.fixture
     def material_solvated(self, monkeypatch) -> MaterialSolvated:
-        self.mock_material = MagicMock()
-        self.mock_material.name = 'material'
-        self.mock_solvent = MagicMock()
-        self.mock_solvent.name = 'solvent'
-        self.mock_solvent_fraction = MagicMock()
+        self.material = Material(sld=1.0, isld=0, name='material')
+        self.solvent = Material(sld=2.0, isld=0, name='solvent')
+        self.mock_solvent_fraction = MagicMock(spec=Parameter)
         self.mock_solvent_fraction.raw_value = 0.1
         self.mock_interface = MagicMock()
         self.mock_Parameter = MagicMock()
         self.mock_FunctionalConstraint = MagicMock()
         monkeypatch.setattr(EasyReflectometry.sample.elements.materials.material_mixture, 'Parameter', self.mock_Parameter)
         monkeypatch.setattr(
             EasyReflectometry.sample.elements.materials.material_mixture,
             'FunctionalConstraint',
             self.mock_FunctionalConstraint,
         )
         return MaterialSolvated(
-            material=self.mock_material,
-            solvent=self.mock_solvent,
+            material=self.material,
+            solvent=self.solvent,
             solvent_fraction=self.mock_solvent_fraction,
             name='name',
             interface=self.mock_interface,
         )
 
     def test_init(self, material_solvated: MaterialSolvated) -> None:
         # When Then Expect
-        assert material_solvated.material_a == self.mock_material
-        assert material_solvated.material_b == self.mock_solvent
+        assert material_solvated.material_a == self.material
+        assert material_solvated.material_b == self.solvent
         assert material_solvated.fraction == 0.1
         assert material_solvated.name == 'name'
         assert material_solvated.interface == self.mock_interface
         self.mock_interface.generate_bindings.call_count == 2
 
     def test_material(self, material_solvated: MaterialSolvated) -> None:
         # When Then Expect
-        assert material_solvated.material == self.mock_material
+        assert material_solvated.material == self.material
 
     def test_set_material(self, material_solvated: MaterialSolvated) -> None:
         # When
         new_material = MagicMock()
         new_material.name = 'new_material'
 
         # Then
@@ -56,15 +56,15 @@
 
         # Expect
         assert material_solvated.material == new_material
         assert material_solvated.name == 'new_material in solvent'
 
     def test_solvent(self, material_solvated: MaterialSolvated) -> None:
         # When Then Expect
-        assert material_solvated.solvent == self.mock_solvent
+        assert material_solvated.solvent == self.solvent
 
     def test_set_solvent(self, material_solvated: MaterialSolvated) -> None:
         # When
         new_solvent = MagicMock()
         new_solvent.name = 'new_solvent'
 
         # Then
@@ -100,29 +100,29 @@
         material_solvated.solvent_fraction = 0.0
 
         # When Then Expect (no exception)
         material_solvated.solvent_fraction = 1.0
 
     def test_dict_repr(self) -> None:
         # When Then
-        p = MaterialSolvated.default()
+        p = MaterialSolvated()
 
         # Expect
         assert p._dict_repr == {
             'D2O in H2O': {
                 'solvent_fraction': '0.200 dimensionless',
                 'sld': '4.976e-6 1 / angstrom ** 2',
                 'isld': '0.000e-6 1 / angstrom ** 2',
                 'material': {'D2O': {'sld': '6.360e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}},
                 'solvent': {'H2O': {'sld': '-0.561e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}},
             }
         }
 
     def test_dict_round_trip(self):
-        p = MaterialSolvated.default()
+        p = MaterialSolvated()
         q = MaterialSolvated.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
 
     def test_update_name(self, material_solvated: MaterialSolvated) -> None:
         # When
         mock_material_a = MagicMock()
         mock_material_a.name = 'name_a'
```

### Comparing `easyreflectometrylib-0.0.6/tests/special/test_calculations.py` & `easyreflectometrylib-0.0.7/tests/special/test_calculations.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/LICENSE` & `easyreflectometrylib-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.6/README.rst` & `easyreflectometrylib-0.0.7/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-.. image:: https://github.com/easyScience/EasyReflectometryLib/raw/main/docs/_static/logo.png
+.. image:: https://github.com/easyScience/EasyReflectometryLib/raw/master/docs/src/_static/logo.png
         :target: https://easyscience.github.io/EasyReflectometryLib/
 
 |
 
 .. image:: https://github.com/easyScience/EasyReflectometryLib/actions/workflows/python-ci.yml/badge.svg
         :target: https://github.com/easyScience/easyReflectometryLib/actions/workflows/python-ci.yml
-.. image:: https://codecov.io/gh/easyScience/EasyReflectometryLib/branch/main/graph/badge.svg?token=LcnB8AMGkw
+.. image:: https://codecov.io/gh/easyScience/EasyReflectometryLib/branch/master/graph/badge.svg?token=LcnB8AMGkw
         :target: https://codecov.io/gh/easyScience/EasyReflectometryLib
 .. image:: https://www.codefactor.io/repository/github/easyscience/easyreflectometrylib/badge
         :target: https://www.codefactor.io/repository/github/easyscience/easyreflectometrylib
         :alt: CodeFactor
 .. image:: https://img.shields.io/badge/docs-built-blue
         :target: http://docs.easyreflectometry.org
         :alt: Docs
```

### Comparing `easyreflectometrylib-0.0.6/pyproject.toml` & `easyreflectometrylib-0.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling<=1.21.0"]  
 build-backend = "hatchling.build"
 
 [project]
 name = "EasyReflectometryLib"
-version = "0.0.6"
+version = "0.0.7"
 description = "A reflectometry python package built on the EasyScience framework."
 readme = "README.rst"
 authors = [
     {name = "Andrew R. McCluskey", email = "andrew.mccluskey@ess.eu"}, 
     {name = "Andrew Sazonov"}, 
     {name = "Simon Ward"},
     {name = "Andreas Pedersen", email = "andreas.pedersen@ess.eu"}
@@ -80,18 +80,14 @@
 exclude = [
     "docs",
 ]
 
 [tool.ruff.format]
 quote-style = "single"
 
-[tool.ruff.per-file-ignores]
-# allow asserts in test files
-"*test_*.py" = ["S101"]
-
 [tool.ruff.lint]
 ignore-init-module-imports = true
 select = [
     # flake8 settings from existing CI setup
     "E9", "F63", "F7", "F82",
     # Code should be polished to fulfill all cases bellow
     # https://docs.astral.sh/ruff/rules/
@@ -110,14 +106,18 @@
     # flake8-bandit
     "S",
 ]
 
 [tool.ruff.lint.isort]
 force-single-line = true
 
+[tool.ruff.lint.per-file-ignores]
+# allow asserts in test files
+"*test_*.py" = ["S101"]
+
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = True
 envlist = py{39,310,311}
 [gh-actions]
 python =
```

### Comparing `easyreflectometrylib-0.0.6/PKG-INFO` & `easyreflectometrylib-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyReflectometryLib
-Version: 0.0.6
+Version: 0.0.7
 Summary: A reflectometry python package built on the EasyScience framework.
 Project-URL: homepage, https://docs.easyreflectometry.org
 Project-URL: documentation, https://docs.easyreflectometry.org
 Author: Andrew Sazonov, Simon Ward
 Author-email: "Andrew R. McCluskey" <andrew.mccluskey@ess.eu>, Andreas Pedersen <andreas.pedersen@ess.eu>
 Maintainer-email: "Andrew R. McCluskey" <andrew.mccluskey@ess.eu>, Andreas Pedersen <andreas.pedersen@ess.eu>
 License-Expression: BSD-3-Clause
@@ -39,22 +39,22 @@
 Provides-Extra: docs
 Requires-Dist: nbsphinx; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-book-theme; extra == 'docs'
 Requires-Dist: toml; extra == 'docs'
 Description-Content-Type: text/x-rst
 
-.. image:: https://github.com/easyScience/EasyReflectometryLib/raw/main/docs/_static/logo.png
+.. image:: https://github.com/easyScience/EasyReflectometryLib/raw/master/docs/src/_static/logo.png
         :target: https://easyscience.github.io/EasyReflectometryLib/
 
 |
 
 .. image:: https://github.com/easyScience/EasyReflectometryLib/actions/workflows/python-ci.yml/badge.svg
         :target: https://github.com/easyScience/easyReflectometryLib/actions/workflows/python-ci.yml
-.. image:: https://codecov.io/gh/easyScience/EasyReflectometryLib/branch/main/graph/badge.svg?token=LcnB8AMGkw
+.. image:: https://codecov.io/gh/easyScience/EasyReflectometryLib/branch/master/graph/badge.svg?token=LcnB8AMGkw
         :target: https://codecov.io/gh/easyScience/EasyReflectometryLib
 .. image:: https://www.codefactor.io/repository/github/easyscience/easyreflectometrylib/badge
         :target: https://www.codefactor.io/repository/github/easyscience/easyreflectometrylib
         :alt: CodeFactor
 .. image:: https://img.shields.io/badge/docs-built-blue
         :target: http://docs.easyreflectometry.org
         :alt: Docs
```

