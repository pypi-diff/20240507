# Comparing `tmp/reqstool-0.4.3.tar.gz` & `tmp/reqstool-0.4.4.tar.gz`

## Comparing `reqstool-0.4.3.tar` & `reqstool-0.4.4.tar`

### file list

```diff
@@ -1,204 +1,204 @@
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/dependabot.yml
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/workflows/check_release.yml
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/workflows/publish_gh_pages.yml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/workflows/publish_pypi_prod.yml
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/workflows/publish_pypi_test.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/antora-playbook.yml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/antora.yml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/examples/requirements/manual_verification_results.yml
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/examples/requirements/requirements_external.yml
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/examples/requirements/requirements_microservice.yml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/examples/requirements/requirements_system.yml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/examples/requirements/software_verification_cases.yml
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/nav.adoc
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/background.adoc
--rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/data.adoc
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/file_and_directory_set.adoc
--rw-r--r--   0        0        0     6723 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/how_it_works.adoc
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/index.adoc
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/installation.adoc
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/overview.adoc
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/quickstart.adoc
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/terminology.adoc
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/usage.adoc
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/annotations.adoc
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/manual_verification_results.adoc
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/reqstool_config.adoc
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements.adoc
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_annotations.adoc
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_external.adoc
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_microservice.adoc
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_system.adoc
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/software_verification_cases.adoc
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/svcs_annotations.adoc
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/partials/C4_Component.puml
--rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/partials/C4_Sequence.puml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/examples/partials/requirements/manual_verification_results.yml
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/examples/partials/requirements/reqstool_config.yml
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/examples/partials/requirements/requirements_external.yml
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/examples/partials/requirements/requirements_microservice.yml
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/examples/partials/requirements/requirements_system.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/examples/partials/requirements/software_verification_cases.yml
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/reqstool/manual_verification_results.yml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/reqstool/reqstool_config.yml
--rw-r--r--   0        0        0    10690 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/reqstool/requirements.yml
--rw-r--r--   0        0        0     6822 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/reqstool/software_verification_cases.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/__init__.py
--rwxr-xr-x   0        0        0    10652 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/command.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/exit_codes.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/generate_json/generate_json.py
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/report.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/criterias/group_by.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/criterias/sort_by.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/annotation_impls.j2
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/annotation_tests.j2
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/mvrs.j2
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/report.j2
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/req_references.j2
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/requirements.j2
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/svcs.j2
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/total_statistics.j2
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/status/statistics_container.py
--rw-r--r--   0        0        0    13322 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/status/statistics_generator.py
--rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/status/status.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/common/jinja2.py
--rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/common/utils.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/common/validator_error_holder.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/common/dataclasses/urn_id.py
--rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/common/validators/semantic_validator.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/common/validators/syntax_validator.py
--rwxr-xr-x   0        0        0     2575 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/expression_languages/generic_el.py
--rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/expression_languages/requirements_el.py
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/expression_languages/svcs_el.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/filters/id_filters.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/filters/requirements_filters.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/filters/svcs_filters.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/location_resolver/location_resolver.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/locations/git_location.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/locations/local_location.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/locations/location.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/locations/maven_location.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/annotations_model_generator.py
--rw-r--r--   0        0        0    29242 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/combined_indexed_dataset_generator.py
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/combined_raw_datasets_generator.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/mvrs_model_generator.py
--rw-r--r--   0        0        0    12619 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/requirements_model_generator.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/svcs_model_generator.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/testdata_model_generator.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/annotations.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/combined_indexed_dataset.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/implementations.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/imports.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/mvrs.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/raw_datasets.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/requirements.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/svcs.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/test_data.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/reqstool_config/reqstool_config.py
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/requirements_indata/requirements_indata.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/requirements_indata/requirements_indata_paths.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/requirements_indata/java/java_maven_requirements_indata_paths.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/requirements_indata/python/python_requirements_indata_paths.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/resources/schemas/v1/annotations.schema.json
--rw-r--r--   0        0        0    11026 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/resources/schemas/v1/common.schema.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/resources/schemas/v1/manual_verification_results.schema.json
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/resources/schemas/v1/reqstool_config.schema.json
--rw-r--r--   0        0        0    10841 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/resources/schemas/v1/requirements.schema.json
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/integration/reqstool/model_generators/test_included_models_generator.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/annotations.yml
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/manual_verification_results.yml
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/requirements.yml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/software_verification_cases.yml
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/pom.xml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/manual_verification_results.yml -> ../../../../../../baseline/ms-101/manual_verification_results.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/requirements.yml -> ../../../../../../baseline/ms-101/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/software_verification_cases.yml -> ../../../../../../baseline/ms-101/software_verification_cases.yml
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/with_requirements_config/README.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/manual_verification_results.yml -> ../../baseline/ms-101/manual_verification_results.yml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/reqstool_config.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/requirements.yml -> ../../baseline/ms-101/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/software_verification_cases.yml -> ../../baseline/ms-101/software_verification_cases.yml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/annotations.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/errors.adoc
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/manual_verification_results.yml
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/requirements.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/software_verification_cases.yml
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/visualization.adoc
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/annotations.yml
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/manual_verification_results.yml
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/requirements.yml
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/software_verification_cases.yml
--rw-r--r--   0        0        0     7126 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml
--rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/requirements.yml
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/software_verification_cases.yml
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-001/requirements.yml
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-002/requirements.yml
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/annotations.yml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/requirements.yml
--rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml
--rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/manual_verification_results.yml
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/requirements.yml
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/software_verification_cases.yml
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-001/requirements.yml
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-002/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/annotations.yml -> ../../../../local/test_standard/baseline/ms-001/annotations.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/manual_verification_results.yml -> ../../../../local/test_standard/baseline/ms-001/manual_verification_results.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/requirements.yml -> ../../../../local/test_standard/baseline/ms-001/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/software_verification_cases.yml -> ../../../../local/test_standard/baseline/ms-001/software_verification_cases.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/annotations.yml -> ../../../../local/test_standard/baseline/sys-001/annotations.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/manual_verification_results.yml -> ../../../../local/test_standard/baseline/sys-001/manual_verification_results.yml
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/software_verification_cases.yml -> ../../../../local/test_standard/baseline/sys-001/software_verification_cases.yml
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_annotations_model_generator/test_annotations_model_generator/annotations.yml
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_mvrs_model_generator/test_mvrs_model_generator/manual_verification_results.yml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_external_requirements_model_generator/requirements.yml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_microservice_requirements_model_generator/requirements.yml
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_rational_optional_model_generator/requirements.yml
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_system_requirements_model_generator/requirements.yml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_svcs_model_generator/test_svcs_model_generator/software_verification_cases.yml
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/conftest.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/commands/generate_json/test_generate_json.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/commands/report/test_report.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/commands/report/criterias/test_criterias.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/commands/status/test_statistics_container.py
--rw-r--r--   0        0        0    18426 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/commands/status/test_statistics_generator.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/commands/status/test_status.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/common/test_locations.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/common/test_utils.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/common/validators/test_semantic_validator.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/expression_languages/test_requirements_el.py
--rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/expression_languages/test_svcs_el.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/filters/test_requirements_filters.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/filters/test_software_verification_cases_filters.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/locations/test_git_location.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/locations/test_local_location.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_annotations_model_generator.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_combined_indexed_dataset_generator.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_combined_raw_datasets_generator.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_mvrs_model_generator.py
--rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_requirements_model_generator.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_svcs_model_generator.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_testdata_model_generator.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/models/test_annotations.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/models/test_implementations.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/models/test_imports.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/models/test_mvrs.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/models/test_requirements.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/models/test_svcs.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/reqstool_config/test_reqstool_config.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/requirements_indata/test_requirements_indata_paths.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/resources/schemas/v1/test_json_schemas.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 reqstool-0.4.3/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 reqstool-0.4.3/LICENSE
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 reqstool-0.4.3/README.md
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 reqstool-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 reqstool-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 reqstool-0.4.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 reqstool-0.4.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 reqstool-0.4.4/.github/workflows/check_release.yml
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 reqstool-0.4.4/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 reqstool-0.4.4/.github/workflows/publish_gh_pages.yml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 reqstool-0.4.4/.github/workflows/publish_pypi_prod.yml
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 reqstool-0.4.4/.github/workflows/publish_pypi_test.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/antora-playbook.yml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/antora.yml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/examples/requirements/manual_verification_results.yml
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/examples/requirements/requirements_external.yml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/examples/requirements/requirements_microservice.yml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/examples/requirements/requirements_system.yml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/examples/requirements/software_verification_cases.yml
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/nav.adoc
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/background.adoc
+-rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/data.adoc
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/file_and_directory_set.adoc
+-rw-r--r--   0        0        0     6723 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/how_it_works.adoc
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/index.adoc
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/installation.adoc
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/overview.adoc
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/quickstart.adoc
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/terminology.adoc
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/usage.adoc
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/yml/annotations.adoc
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/yml/manual_verification_results.adoc
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/yml/reqstool_config.adoc
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/yml/requirements.adoc
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/yml/requirements_annotations.adoc
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/yml/requirements_external.adoc
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/yml/requirements_microservice.adoc
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/yml/requirements_system.adoc
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/yml/software_verification_cases.adoc
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/pages/yml/svcs_annotations.adoc
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/partials/C4_Component.puml
+-rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/ROOT/partials/C4_Sequence.puml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/examples/partials/requirements/manual_verification_results.yml
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/examples/partials/requirements/reqstool_config.yml
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/examples/partials/requirements/requirements_external.yml
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/examples/partials/requirements/requirements_microservice.yml
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/examples/partials/requirements/requirements_system.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/modules/examples/partials/requirements/software_verification_cases.yml
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/reqstool/manual_verification_results.yml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/reqstool/reqstool_config.yml
+-rw-r--r--   0        0        0    10690 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/reqstool/requirements.yml
+-rw-r--r--   0        0        0     6822 2020-02-02 00:00:00.000000 reqstool-0.4.4/docs/reqstool/software_verification_cases.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/__init__.py
+-rwxr-xr-x   0        0        0    10652 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/command.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/exit_codes.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/generate_json/generate_json.py
+-rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/report/report.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/report/criterias/group_by.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/report/criterias/sort_by.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/report/templates/annotation_impls.j2
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/report/templates/annotation_tests.j2
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/report/templates/mvrs.j2
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/report/templates/report.j2
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/report/templates/req_references.j2
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/report/templates/requirements.j2
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/report/templates/svcs.j2
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/report/templates/total_statistics.j2
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/status/statistics_container.py
+-rw-r--r--   0        0        0    13322 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/status/statistics_generator.py
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/commands/status/status.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/common/jinja2.py
+-rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/common/utils.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/common/validator_error_holder.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/common/dataclasses/urn_id.py
+-rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/common/validators/semantic_validator.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/common/validators/syntax_validator.py
+-rwxr-xr-x   0        0        0     2575 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/expression_languages/generic_el.py
+-rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/expression_languages/requirements_el.py
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/expression_languages/svcs_el.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/filters/id_filters.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/filters/requirements_filters.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/filters/svcs_filters.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/location_resolver/location_resolver.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/locations/git_location.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/locations/local_location.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/locations/location.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/locations/maven_location.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/model_generators/annotations_model_generator.py
+-rw-r--r--   0        0        0    29242 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/model_generators/combined_indexed_dataset_generator.py
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/model_generators/combined_raw_datasets_generator.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/model_generators/mvrs_model_generator.py
+-rw-r--r--   0        0        0    12619 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/model_generators/requirements_model_generator.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/model_generators/svcs_model_generator.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/model_generators/testdata_model_generator.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/models/annotations.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/models/combined_indexed_dataset.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/models/implementations.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/models/imports.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/models/mvrs.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/models/raw_datasets.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/models/requirements.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/models/svcs.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/models/test_data.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/reqstool_config/reqstool_config.py
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/requirements_indata/requirements_indata.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/requirements_indata/requirements_indata_paths.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/requirements_indata/java/java_maven_requirements_indata_paths.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/requirements_indata/python/python_requirements_indata_paths.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/resources/schemas/v1/annotations.schema.json
+-rw-r--r--   0        0        0    11310 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/resources/schemas/v1/common.schema.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/resources/schemas/v1/manual_verification_results.schema.json
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/resources/schemas/v1/reqstool_config.schema.json
+-rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/resources/schemas/v1/requirements.schema.json
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 reqstool-0.4.4/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/integration/reqstool/model_generators/test_included_models_generator.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/baseline/ms-101/annotations.yml
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/baseline/ms-101/manual_verification_results.yml
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/baseline/ms-101/requirements.yml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/baseline/ms-101/software_verification_cases.yml
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/pom.xml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/manual_verification_results.yml -> ../../../../../../baseline/ms-101/manual_verification_results.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/requirements.yml -> ../../../../../../baseline/ms-101/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/software_verification_cases.yml -> ../../../../../../baseline/ms-101/software_verification_cases.yml
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/with_requirements_config/README.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/manual_verification_results.yml -> ../../baseline/ms-101/manual_verification_results.yml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/reqstool_config.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/requirements.yml -> ../../baseline/ms-101/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/software_verification_cases.yml -> ../../baseline/ms-101/software_verification_cases.yml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_errors/ms-101/annotations.yml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_errors/ms-101/errors.adoc
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_errors/ms-101/manual_verification_results.yml
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_errors/ms-101/requirements.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_errors/ms-101/software_verification_cases.yml
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_errors/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_errors/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/visualization.adoc
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/ms-001/annotations.yml
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/ms-001/manual_verification_results.yml
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/ms-001/requirements.yml
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/ms-001/software_verification_cases.yml
+-rw-r--r--   0        0        0     7126 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml
+-rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/sys-001/requirements.yml
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/sys-001/software_verification_cases.yml
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-001/requirements.yml
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-002/requirements.yml
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/annotations.yml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/requirements.yml
+-rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml
+-rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/manual_verification_results.yml
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/requirements.yml
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/software_verification_cases.yml
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-001/requirements.yml
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-002/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/annotations.yml -> ../../../../local/test_standard/baseline/ms-001/annotations.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/manual_verification_results.yml -> ../../../../local/test_standard/baseline/ms-001/manual_verification_results.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/requirements.yml -> ../../../../local/test_standard/baseline/ms-001/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/software_verification_cases.yml -> ../../../../local/test_standard/baseline/ms-001/software_verification_cases.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/annotations.yml -> ../../../../local/test_standard/baseline/sys-001/annotations.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/manual_verification_results.yml -> ../../../../local/test_standard/baseline/sys-001/manual_verification_results.yml
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/software_verification_cases.yml -> ../../../../local/test_standard/baseline/sys-001/software_verification_cases.yml
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/unit/reqstool/model_generators/test_annotations_model_generator/test_annotations_model_generator/annotations.yml
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/unit/reqstool/model_generators/test_mvrs_model_generator/test_mvrs_model_generator/manual_verification_results.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_external_requirements_model_generator/requirements.yml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_microservice_requirements_model_generator/requirements.yml
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_rational_optional_model_generator/requirements.yml
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_system_requirements_model_generator/requirements.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/resources/unit/reqstool/model_generators/test_svcs_model_generator/test_svcs_model_generator/software_verification_cases.yml
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/conftest.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/commands/generate_json/test_generate_json.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/commands/report/test_report.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/commands/report/criterias/test_criterias.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/commands/status/test_statistics_container.py
+-rw-r--r--   0        0        0    18426 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/commands/status/test_statistics_generator.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/commands/status/test_status.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/common/test_locations.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/common/test_utils.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/common/validators/test_semantic_validator.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/expression_languages/test_requirements_el.py
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/expression_languages/test_svcs_el.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/filters/test_requirements_filters.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/filters/test_software_verification_cases_filters.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/locations/test_git_location.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/locations/test_local_location.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/model_generators/test_annotations_model_generator.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/model_generators/test_combined_indexed_dataset_generator.py
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/model_generators/test_combined_raw_datasets_generator.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/model_generators/test_mvrs_model_generator.py
+-rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/model_generators/test_requirements_model_generator.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/model_generators/test_svcs_model_generator.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/model_generators/test_testdata_model_generator.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/models/test_annotations.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/models/test_implementations.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/models/test_imports.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/models/test_mvrs.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/models/test_requirements.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/models/test_svcs.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/reqstool_config/test_reqstool_config.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/requirements_indata/test_requirements_indata_paths.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 reqstool-0.4.4/tests/unit/reqstool/resources/schemas/v1/test_json_schemas.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 reqstool-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 reqstool-0.4.4/LICENSE
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 reqstool-0.4.4/README.md
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 reqstool-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 reqstool-0.4.4/PKG-INFO
```

### Comparing `reqstool-0.4.3/.github/dependabot.yml` & `reqstool-0.4.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/.github/workflows/build.yml` & `reqstool-0.4.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/.github/workflows/lint.yml` & `reqstool-0.4.4/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/.github/workflows/publish_gh_pages.yml` & `reqstool-0.4.4/.github/workflows/publish_gh_pages.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/.github/workflows/publish_pypi_prod.yml` & `reqstool-0.4.4/.github/workflows/publish_pypi_prod.yml`

 * *Files 24% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   publish-to-pypi:
     needs: 
       - check-release
       - build
     runs-on: ubuntu-latest
     environment:
       name: prod
-      url: https://pypi.org/p/reqstool-client
+      url: https://pypi.org/p/reqstool
     permissions:
       id-token: write # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
       # Download artifacts from the build job
       - name: Download Artifacts
         uses: actions/download-artifact@v4
         with:
```

### Comparing `reqstool-0.4.3/.github/workflows/publish_pypi_test.yml` & `reqstool-0.4.4/.github/workflows/publish_pypi_test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
   publish-to-test-pypi:
     needs: build
     runs-on: ubuntu-latest
     # Specifying a GitHub environment is optional, but strongly encouraged
     environment:
       name: test
-      url: https://test.pypi.org/p/reqstool-client
+      url: https://test.pypi.org/p/reqstool
     permissions:
       id-token: write # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
       # Download artifacts from the build job
       - name: Download Artifacts
         uses: actions/download-artifact@v4
         with:
```

### Comparing `reqstool-0.4.3/docs/antora-playbook.yml` & `reqstool-0.4.4/docs/antora-playbook.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/examples/requirements/requirements_external.yml` & `reqstool-0.4.4/docs/examples/requirements/requirements_external.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/examples/requirements/requirements_microservice.yml` & `reqstool-0.4.4/docs/examples/requirements/requirements_microservice.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/examples/requirements/requirements_system.yml` & `reqstool-0.4.4/docs/examples/requirements/requirements_system.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/examples/requirements/software_verification_cases.yml` & `reqstool-0.4.4/docs/examples/requirements/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/background.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/background.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/data.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/data.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/file_and_directory_set.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/file_and_directory_set.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/how_it_works.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/how_it_works.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/index.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/index.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/overview.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/overview.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/terminology.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/terminology.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/usage.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/usage.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/yml/annotations.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/yml/annotations.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/yml/requirements.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_annotations.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/yml/requirements_annotations.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_external.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/yml/requirements_external.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_microservice.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/yml/requirements_microservice.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_system.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/yml/requirements_system.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/yml/software_verification_cases.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/yml/software_verification_cases.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/pages/yml/svcs_annotations.adoc` & `reqstool-0.4.4/docs/modules/ROOT/pages/yml/svcs_annotations.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/partials/C4_Component.puml` & `reqstool-0.4.4/docs/modules/ROOT/partials/C4_Component.puml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/ROOT/partials/C4_Sequence.puml` & `reqstool-0.4.4/docs/modules/ROOT/partials/C4_Sequence.puml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/examples/partials/requirements/requirements_external.yml` & `reqstool-0.4.4/docs/modules/examples/partials/requirements/requirements_external.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/examples/partials/requirements/requirements_microservice.yml` & `reqstool-0.4.4/docs/modules/examples/partials/requirements/requirements_microservice.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/examples/partials/requirements/requirements_system.yml` & `reqstool-0.4.4/docs/modules/examples/partials/requirements/requirements_system.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/modules/examples/partials/requirements/software_verification_cases.yml` & `reqstool-0.4.4/docs/modules/examples/partials/requirements/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/reqstool/manual_verification_results.yml` & `reqstool-0.4.4/docs/reqstool/manual_verification_results.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/reqstool/requirements.yml` & `reqstool-0.4.4/docs/reqstool/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/docs/reqstool/software_verification_cases.yml` & `reqstool-0.4.4/docs/reqstool/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/command.py` & `reqstool-0.4.4/src/reqstool/command.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/commands/generate_json/generate_json.py` & `reqstool-0.4.4/src/reqstool/commands/generate_json/generate_json.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/commands/report/report.py` & `reqstool-0.4.4/src/reqstool/commands/report/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,18 +101,18 @@
 
         # group_by, List(asciidoc for each req)
         template_data: Dict[str, List[str]] = {
             group_by: [self.__extract_template_data(req_template=aggregated_data[urn_id]) for urn_id in urn_ids]
             for group_by, urn_ids in grouped_requirements.items()
         }
 
-        asciidoc: str = "== REQUIREMENTS DOCUMENTATION\n" + statistics_table
+        asciidoc: str = "= REQUIREMENTS DOCUMENTATION\n" + statistics_table
 
         for group_by in template_data.keys():
-            asciidoc += f"=== {group_by[0].upper() + group_by[1:] }\n"
+            asciidoc += f"== {group_by[0].upper() + group_by[1:] }\n"
 
             for template in template_data[group_by]:
 
                 asciidoc += template
 
         return asciidoc
```

### Comparing `reqstool-0.4.3/src/reqstool/commands/report/criterias/group_by.py` & `reqstool-0.4.4/src/reqstool/commands/report/criterias/group_by.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/commands/report/templates/total_statistics.j2` & `reqstool-0.4.4/src/reqstool/commands/report/templates/total_statistics.j2`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
-=== TOTAL STATISTICS
+== TOTAL STATISTICS
 
 [cols="0.5,1a"]
 |===
 | Total Requirements: {{data.nr_of_total_requirements}}|
-!====
+!===
 !Implemented and Verified ! Implemented ! Not Implemented 
 !{{data.nr_of_completed_requirements}}
 !{{data.nr_of_reqs_with_implementation - data.nr_of_completed_requirements}}
 !{{data.nr_of_total_requirements - data.nr_of_reqs_with_implementation}}
 !===
 | Total Tests / SVCs: ( {{data.nr_of_total_tests}} / {{data.nr_of_total_svcs}} )|
 !===
```

### Comparing `reqstool-0.4.3/src/reqstool/commands/status/statistics_container.py` & `reqstool-0.4.4/src/reqstool/commands/status/statistics_container.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/commands/status/statistics_generator.py` & `reqstool-0.4.4/src/reqstool/commands/status/statistics_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/commands/status/status.py` & `reqstool-0.4.4/src/reqstool/commands/status/status.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/common/jinja2.py` & `reqstool-0.4.4/src/reqstool/common/jinja2.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/common/utils.py` & `reqstool-0.4.4/src/reqstool/common/utils.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/common/validator_error_holder.py` & `reqstool-0.4.4/src/reqstool/common/validator_error_holder.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/common/dataclasses/urn_id.py` & `reqstool-0.4.4/src/reqstool/common/dataclasses/urn_id.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/common/validators/semantic_validator.py` & `reqstool-0.4.4/src/reqstool/common/validators/semantic_validator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/common/validators/syntax_validator.py` & `reqstool-0.4.4/src/reqstool/common/validators/syntax_validator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/expression_languages/generic_el.py` & `reqstool-0.4.4/src/reqstool/expression_languages/generic_el.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/filters/id_filters.py` & `reqstool-0.4.4/src/reqstool/filters/id_filters.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/location_resolver/location_resolver.py` & `reqstool-0.4.4/src/reqstool/location_resolver/location_resolver.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/locations/git_location.py` & `reqstool-0.4.4/src/reqstool/locations/git_location.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/locations/local_location.py` & `reqstool-0.4.4/src/reqstool/locations/local_location.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/locations/maven_location.py` & `reqstool-0.4.4/src/reqstool/locations/maven_location.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/model_generators/annotations_model_generator.py` & `reqstool-0.4.4/src/reqstool/model_generators/annotations_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/model_generators/combined_indexed_dataset_generator.py` & `reqstool-0.4.4/src/reqstool/model_generators/combined_indexed_dataset_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/model_generators/combined_raw_datasets_generator.py` & `reqstool-0.4.4/src/reqstool/model_generators/combined_raw_datasets_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/model_generators/mvrs_model_generator.py` & `reqstool-0.4.4/src/reqstool/model_generators/mvrs_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/model_generators/requirements_model_generator.py` & `reqstool-0.4.4/src/reqstool/model_generators/requirements_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/model_generators/svcs_model_generator.py` & `reqstool-0.4.4/src/reqstool/model_generators/svcs_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/model_generators/testdata_model_generator.py` & `reqstool-0.4.4/src/reqstool/model_generators/testdata_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/models/combined_indexed_dataset.py` & `reqstool-0.4.4/src/reqstool/models/combined_indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/models/raw_datasets.py` & `reqstool-0.4.4/src/reqstool/models/raw_datasets.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/models/requirements.py` & `reqstool-0.4.4/src/reqstool/models/requirements.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/models/svcs.py` & `reqstool-0.4.4/src/reqstool/models/svcs.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/reqstool_config/reqstool_config.py` & `reqstool-0.4.4/src/reqstool/reqstool_config/reqstool_config.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/requirements_indata/requirements_indata.py` & `reqstool-0.4.4/src/reqstool/requirements_indata/requirements_indata.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,22 +103,22 @@
                 item.exists = os.path.exists(item.path)
         else:
             raise TypeError(type(original))
 
     def _handle_custom(self):
         # replace default values with custom if specified
 
-        if self.reqstool_config.locations:
+        if self.reqstool_config.locations.test_results:
             test_results = self.reqstool_config.locations.test_results
 
             if isinstance(test_results, Sequence):
                 r_test_results = []
 
                 for test_result_dir in test_results:
                     r_test_results.append(RequirementsIndataPathItem(path=test_result_dir))
 
                 self.requirements_indata_paths.test_results_dirs = r_test_results
 
-            if self.reqstool_config.locations.annotations:
-                self.requirements_indata_paths.annotations_yml = RequirementsIndataPathItem(
-                    path=self.reqstool_config.locations.annotations
-                )
+        if self.reqstool_config.locations.annotations:
+            self.requirements_indata_paths.annotations_yml = RequirementsIndataPathItem(
+                path=self.reqstool_config.locations.annotations
+            )
```

### Comparing `reqstool-0.4.3/src/reqstool/requirements_indata/java/java_maven_requirements_indata_paths.py` & `reqstool-0.4.4/src/reqstool/requirements_indata/java/java_maven_requirements_indata_paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 class JavaMavenRequirementsIndataPaths(RequirementsIndataPaths):
     def __init__(self):
         super().__init__()
 
         self.annotations_yml = RequirementsIndataPathItem(path="target/reqstool/annotations.yml")
 
         self.test_results_dirs = [
-            RequirementsIndataPathItem(path="target/failfire-reports"),
+            RequirementsIndataPathItem(path="target/failsafe-reports"),
             RequirementsIndataPathItem(path="target/surefire-reports"),
         ]
```

### Comparing `reqstool-0.4.3/src/reqstool/resources/schemas/v1/annotations.schema.json` & `reqstool-0.4.4/src/reqstool/resources/schemas/v1/annotations.schema.json`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/resources/schemas/v1/common.schema.json` & `reqstool-0.4.4/src/reqstool/resources/schemas/v1/common.schema.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'$defs'": "{'urnid': OrderedDict([('type', 'string'), ('pattern', '^[^:].*'), ('description', "*

 * *            '"An identifier that can be on the form \'SYSTEM:ID\' or \'ID\'. If the system urn is '*

 * *            'omitted then it defaults to the system urn that the the current file is part of.")])}'}*

```diff
@@ -256,12 +256,17 @@
                     "type": "object"
                 }
             },
             "type": "object"
         },
         "reqid": {
             "type": "string"
+        },
+        "urnid": {
+            "description": "An identifier that can be on the form 'SYSTEM:ID' or 'ID'. If the system urn is omitted then it defaults to the system urn that the the current file is part of.",
+            "pattern": "^[^:].*",
+            "type": "string"
         }
     },
     "$id": "https://raw.githubusercontent.com/Luftfartsverket/reqstool-client/main/src/reqstool/resources/schemas/v1/common.schema.json",
     "$schema": "https://json-schema.org/draft/2020-12/schema"
 }
```

### Comparing `reqstool-0.4.3/src/reqstool/resources/schemas/v1/manual_verification_results.schema.json` & `reqstool-0.4.4/src/reqstool/resources/schemas/v1/manual_verification_results.schema.json`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/resources/schemas/v1/reqstool_config.schema.json` & `reqstool-0.4.4/src/reqstool/resources/schemas/v1/reqstool_config.schema.json`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/src/reqstool/resources/schemas/v1/requirements.schema.json` & `reqstool-0.4.4/src/reqstool/resources/schemas/v1/requirements.schema.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999997820172991%*

 * *Differences: {"'$defs'": "{'requirements': {'properties': {'references': {'properties': {'requirement_ids': "*

 * *            "{'items': {'$ref': 'common.schema.json#/$defs/urnid', delete: ['description']}}}}}}}"}*

```diff
@@ -180,16 +180,15 @@
                 "references": {
                     "additionalProperties": false,
                     "description": "References to related requirements",
                     "properties": {
                         "requirement_ids": {
                             "description": "Array of requirements related to this requirement",
                             "items": {
-                                "$ref": "common.schema.json#/$defs/reqid",
-                                "description": "Requirement id that links to another requirement in this document"
+                                "$ref": "common.schema.json#/$defs/urnid"
                             },
                             "type": "array"
                         }
                     },
                     "required": [
                         "requirement_ids"
                     ],
```

### Comparing `reqstool-0.4.3/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json` & `reqstool-0.4.4/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999468537414966%*

 * *Differences: {"'$defs'": "{'cases': {'properties': {'requirement_ids': {'items': {replace: "*

 * *            "OrderedDict([('$ref', 'common.schema.json#/$defs/urnid')])}}}}}"}*

```diff
@@ -14,16 +14,15 @@
                 "instructions": {
                     "description": "Instructional steps for how to verify, if it is manual",
                     "type": "string"
                 },
                 "requirement_ids": {
                     "description": "Array of related Requirement ids",
                     "items": {
-                        "description": "Requirement id",
-                        "type": "string"
+                        "$ref": "common.schema.json#/$defs/urnid"
                     },
                     "type": "array"
                 },
                 "revision": {
                     "description": "Version the Software Verification Case was revised",
                     "pattern": "^(\\d+\\.)?(\\d+\\.)?(\\*|\\d+)$",
                     "type": "string"
```

### Comparing `reqstool-0.4.3/tests/integration/reqstool/model_generators/test_included_models_generator.py` & `reqstool-0.4.4/tests/integration/reqstool/model_generators/test_included_models_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/annotations.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/baseline/ms-101/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/requirements.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/baseline/ms-101/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/software_verification_cases.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/baseline/ms-101/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/pom.xml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/pom.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/with_requirements_config/README.md` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_basic/with_requirements_config/README.md`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/annotations.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_errors/ms-101/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/requirements.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_errors/ms-101/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/software_verification_cases.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_errors/ms-101/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_errors/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_errors/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/visualization.adoc` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/visualization.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/annotations.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/ms-001/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/requirements.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/ms-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/software_verification_cases.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/ms-001/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/requirements.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/sys-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/software_verification_cases.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/sys-001/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-001/requirements.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-002/requirements.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-002/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/annotations.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/requirements.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/software_verification_cases.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-001/requirements.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-002/requirements.yml` & `reqstool-0.4.4/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-002/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/requirements.yml` & `reqstool-0.4.4/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_annotations_model_generator/test_annotations_model_generator/annotations.yml` & `reqstool-0.4.4/tests/resources/unit/reqstool/model_generators/test_annotations_model_generator/test_annotations_model_generator/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_external_requirements_model_generator/requirements.yml` & `reqstool-0.4.4/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_external_requirements_model_generator/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_microservice_requirements_model_generator/requirements.yml` & `reqstool-0.4.4/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_microservice_requirements_model_generator/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_rational_optional_model_generator/requirements.yml` & `reqstool-0.4.4/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_rational_optional_model_generator/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_system_requirements_model_generator/requirements.yml` & `reqstool-0.4.4/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_system_requirements_model_generator/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_svcs_model_generator/test_svcs_model_generator/software_verification_cases.yml` & `reqstool-0.4.4/tests/resources/unit/reqstool/model_generators/test_svcs_model_generator/test_svcs_model_generator/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/conftest.py` & `reqstool-0.4.4/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/commands/report/test_report.py` & `reqstool-0.4.4/tests/unit/reqstool/commands/report/test_report.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/commands/report/criterias/test_criterias.py` & `reqstool-0.4.4/tests/unit/reqstool/commands/report/criterias/test_criterias.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/commands/status/test_statistics_container.py` & `reqstool-0.4.4/tests/unit/reqstool/commands/status/test_statistics_container.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/commands/status/test_statistics_generator.py` & `reqstool-0.4.4/tests/unit/reqstool/commands/status/test_statistics_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/commands/status/test_status.py` & `reqstool-0.4.4/tests/unit/reqstool/commands/status/test_status.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/common/test_locations.py` & `reqstool-0.4.4/tests/unit/reqstool/common/test_locations.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/common/validators/test_semantic_validator.py` & `reqstool-0.4.4/tests/unit/reqstool/common/validators/test_semantic_validator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/expression_languages/test_requirements_el.py` & `reqstool-0.4.4/tests/unit/reqstool/expression_languages/test_requirements_el.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/expression_languages/test_svcs_el.py` & `reqstool-0.4.4/tests/unit/reqstool/expression_languages/test_svcs_el.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/filters/test_requirements_filters.py` & `reqstool-0.4.4/tests/unit/reqstool/filters/test_requirements_filters.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/filters/test_software_verification_cases_filters.py` & `reqstool-0.4.4/tests/unit/reqstool/filters/test_software_verification_cases_filters.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/locations/test_git_location.py` & `reqstool-0.4.4/tests/unit/reqstool/locations/test_git_location.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_annotations_model_generator.py` & `reqstool-0.4.4/tests/unit/reqstool/model_generators/test_annotations_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_combined_indexed_dataset_generator.py` & `reqstool-0.4.4/tests/unit/reqstool/model_generators/test_combined_indexed_dataset_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_combined_raw_datasets_generator.py` & `reqstool-0.4.4/tests/unit/reqstool/model_generators/test_combined_raw_datasets_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_mvrs_model_generator.py` & `reqstool-0.4.4/tests/unit/reqstool/model_generators/test_mvrs_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_requirements_model_generator.py` & `reqstool-0.4.4/tests/unit/reqstool/model_generators/test_requirements_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_svcs_model_generator.py` & `reqstool-0.4.4/tests/unit/reqstool/model_generators/test_svcs_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_testdata_model_generator.py` & `reqstool-0.4.4/tests/unit/reqstool/model_generators/test_testdata_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/models/test_annotations.py` & `reqstool-0.4.4/tests/unit/reqstool/models/test_annotations.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/models/test_implementations.py` & `reqstool-0.4.4/tests/unit/reqstool/models/test_implementations.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/models/test_imports.py` & `reqstool-0.4.4/tests/unit/reqstool/models/test_imports.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/models/test_mvrs.py` & `reqstool-0.4.4/tests/unit/reqstool/models/test_mvrs.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/models/test_requirements.py` & `reqstool-0.4.4/tests/unit/reqstool/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/models/test_svcs.py` & `reqstool-0.4.4/tests/unit/reqstool/models/test_svcs.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/reqstool_config/test_reqstool_config.py` & `reqstool-0.4.4/tests/unit/reqstool/reqstool_config/test_reqstool_config.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/tests/unit/reqstool/requirements_indata/test_requirements_indata_paths.py` & `reqstool-0.4.4/tests/unit/reqstool/requirements_indata/test_requirements_indata_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,9 +46,9 @@
 
     assert java_merged_instance.requirements_yml.path == "requirements.yml"
     assert java_merged_instance.svcs_yml.path == "software_verification_cases.yml"
     assert java_merged_instance.mvrs_yml.path == "manual_verification_results.yml"
     assert java_merged_instance.annotations_yml.path == "target/reqstool/annotations.yml"
     assert len(java_merged_instance.test_results_dirs) == 2
 
-    expected_paths = ["target/failfire-reports", "target/surefire-reports"]
+    expected_paths = ["target/failsafe-reports", "target/surefire-reports"]
     assert all(item.path in expected_paths for item in java_merged_instance.test_results_dirs)
```

### Comparing `reqstool-0.4.3/tests/unit/reqstool/resources/schemas/v1/test_json_schemas.py` & `reqstool-0.4.4/tests/unit/reqstool/resources/schemas/v1/test_json_schemas.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/.gitignore` & `reqstool-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/LICENSE` & `reqstool-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/README.md` & `reqstool-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.3/pyproject.toml` & `reqstool-0.4.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     "Development Status :: 3 - Alpha",
 ]
 
 requires-python = ">=3.10"
 
 dependencies = [
     "colorama==0.4.6",
-    "Jinja2==3.1.3",
-    "jsonpickle==3.0.3",
-    "jsonschema[format-nongpl]==4.21.1",
+    "Jinja2==3.1.4",
+    "jsonpickle==3.0.4",
+    "jsonschema[format-nongpl]==4.22.0",
     "lark==1.1.9",
     "maven-artifact==0.3.4",
     "pygit2==1.14.1",
-    "referencing==0.34.0",
+    "referencing==0.35.1",
     "requests-file==2.0.0",
     "ruamel.yaml==0.18.6",
     "tabulate==0.9.0",
     "xmldict==0.4.1",
     "reqstool-python-decorators==0.0.4",
     "packaging==24.0",
 ]
```

### Comparing `reqstool-0.4.3/PKG-INFO` & `reqstool-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.3
 Name: reqstool
-Version: 0.4.3
+Version: 0.4.4
 Summary: A tool for managing requirements with related tests and test results.
 Project-URL: Source, https://github.com/Luftfartsverket/reqstool-client
 Author-email: LFV <info@lfv.se>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: colorama==0.4.6
-Requires-Dist: jinja2==3.1.3
-Requires-Dist: jsonpickle==3.0.3
-Requires-Dist: jsonschema[format-nongpl]==4.21.1
+Requires-Dist: jinja2==3.1.4
+Requires-Dist: jsonpickle==3.0.4
+Requires-Dist: jsonschema[format-nongpl]==4.22.0
 Requires-Dist: lark==1.1.9
 Requires-Dist: maven-artifact==0.3.4
 Requires-Dist: packaging==24.0
 Requires-Dist: pygit2==1.14.1
-Requires-Dist: referencing==0.34.0
+Requires-Dist: referencing==0.35.1
 Requires-Dist: reqstool-python-decorators==0.0.4
 Requires-Dist: requests-file==2.0.0
 Requires-Dist: ruamel-yaml==0.18.6
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: xmldict==0.4.1
 Description-Content-Type: text/markdown
```

